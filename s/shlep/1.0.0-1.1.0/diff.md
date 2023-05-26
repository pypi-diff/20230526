# Comparing `tmp/shlep-1.0.0.tar.gz` & `tmp/shlep-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.0.0.tar", last modified: Fri May 26 04:44:27 2023, max compression
+gzip compressed data, was "shlep-1.1.0.tar", last modified: Fri May 26 06:42:46 2023, max compression
```

## Comparing `shlep-1.0.0.tar` & `shlep-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.0.0/LICENSE
--rw-r--r--   0        0        0     2221 2023-05-26 04:43:52.285127 shlep-1.0.0/README.md
--rw-r--r--   0        0        0      429 2023-05-26 04:44:27.338135 shlep-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.0.0/shlep/__init__.py
--rw-r--r--   0        0        0     3930 2023-05-26 04:40:35.731758 shlep-1.0.0/shlep/main.py
--rw-r--r--   0        0        0     2470 1970-01-01 00:00:00.000000 shlep-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2221 2023-05-26 04:43:52.285127 shlep-1.1.0/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 06:42:46.679781 shlep-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.1.0/shlep/__init__.py
+-rw-r--r--   0        0        0     3921 2023-05-26 06:41:59.127320 shlep-1.1.0/shlep/main.py
+-rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 shlep-1.1.0/PKG-INFO
```

### Comparing `shlep-1.0.0/LICENSE` & `shlep-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.0.0/README.md` & `shlep-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `shlep-1.0.0/shlep/main.py` & `shlep-1.1.0/shlep/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 import argparse
 import json
 import logging
 import os
 from pathlib import Path
 
+from pathspec import PathSpec
+
 DEFAULT_EXCLUDED = [
     ".git/",
     ".idea/",
     ".pytest_cache/",
 ]
 
 logger = logging.getLogger(__name__)
 
 
-def get_excluded_patterns(directory, additional_excludes):
-    excluded_patterns = DEFAULT_EXCLUDED + additional_excludes
-    gitignore_path = os.path.join(directory, ".gitignore")
-    if os.path.exists(gitignore_path):
-        with open(gitignore_path) as f:
-            for line in f:
-                if line.strip() and not line.startswith("#"):
-                    excluded_patterns.append(line.strip())
-    return excluded_patterns
-
-
-def is_excluded(path, excluded_patterns):
-    return any(p in str(path) for p in excluded_patterns)
+def _is_excluded(base: Path, path: Path, spec: PathSpec = None):
+    if not spec:
+        return True
+    return spec.match_file(str(path.relative_to(base)))
 
 
 def create_output(
     directory: str,
     indent: int,
     additional_excludes: list[str],
     output_format: str,
@@ -44,20 +37,31 @@
         additional_excludes: Additional files or directories to exclude.
         output_format: The output format. Can be 'json', 'csv', or 'plaintext'. Default is 'json'.
         output_file: The output file to generate. If not specified, output is printed to stdout.
 
     Returns:
         None
     """
-    excluded_patterns = get_excluded_patterns(directory, additional_excludes)
-
     files_list = []
+    base = Path(directory).expanduser()
+
+    if (gitignore := base / ".gitignore").exists():
+        with gitignore.open() as f:
+            additional_excludes.extend(
+                line.strip() for line in f if line.strip() and not line.startswith("#")
+            )
+        spec = PathSpec.from_lines(
+            "gitwildmatch",
+            DEFAULT_EXCLUDED + additional_excludes,
+        )
+    else:
+        spec = None
 
-    for path in Path(directory).rglob("*"):
-        if path.is_file() and not is_excluded(path, excluded_patterns):
+    for path in base.rglob("*"):
+        if path.is_file() and not _is_excluded(base, path, spec):
             try:
                 content = path.read_text()
             except UnicodeDecodeError:
                 logger.error(f"Could not read {path}")
             else:
                 files_list.append({"path": str(path), "content": content})
 
@@ -78,24 +82,23 @@
             output += f"`{filepath}`"
             output += os.linesep
             output += f"```{os.linesep + file_content}```"
             if not i == len_files_list:
                 output += os.linesep * 2 + "---" + os.linesep * 2
 
     if output_file:
-        with open(output_file, "w") as f:
+        with Path(output_file).expanduser().open("w") as f:
             f.write(output)
     else:
         print(output)
 
 
 def cli():
     parser = argparse.ArgumentParser(
-        prog="shlep",
-        description="Gather directory contents into a single output."
+        prog="shlep", description="Gather directory contents into a single output."
     )
     parser.add_argument("directory", help="The directory to analyze.")
     parser.add_argument(
         "-o",
         "--output-file",
         help="The output file to generate. If not specified, output is printed to stdout.",
     )
```

### Comparing `shlep-1.0.0/PKG-INFO` & `shlep-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.0.0
+Version: 1.1.0
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
+Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
 
 # shlep
 
 <img src="static/ai.png" alt="mascot" style="width: 400px; height: auto;">   
 
 `shlep` lets you package your directory's content in a format that can be easily passed to ChatGPT. This is especially
```


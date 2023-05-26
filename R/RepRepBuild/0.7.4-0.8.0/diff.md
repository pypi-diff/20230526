# Comparing `tmp/RepRepBuild-0.7.4.tar.gz` & `tmp/RepRepBuild-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.7.4.tar", last modified: Mon May 15 07:29:27 2023, max compression
+gzip compressed data, was "RepRepBuild-0.8.0.tar", last modified: Fri May 26 15:53:59 2023, max compression
```

## Comparing `RepRepBuild-0.7.4.tar` & `RepRepBuild-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/HEADER
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.927795 RepRepBuild-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:29:27.931795 RepRepBuild-0.7.4/src/reprepbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 07:29:27.000000 RepRepBuild-0.7.4/src/reprepbuild/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/articlezip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/latexdep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/repeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-15 07:29:17.000000 RepRepBuild-0.7.4/src/reprepbuild/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/HEADER
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.205849 RepRepBuild-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:53:59.209849 RepRepBuild-0.8.0/src/reprepbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11553 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:53:59.000000 RepRepBuild-0.8.0/src/reprepbuild/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/articlezip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/latexdep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 15:53:48.000000 RepRepBuild-0.8.0/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.7.4/.github/workflows/pypi.yaml` & `RepRepBuild-0.8.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/.pre-commit-config.yaml` & `RepRepBuild-0.8.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
   hooks:
     - id: remove-crlf
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.265'
+  rev: 'v0.0.269'
   hooks:
     - id: ruff
 - repo: https://github.com/python-jsonschema/check-jsonschema
   rev: 0.23.0
   hooks:
     - id: check-github-workflows
```

### Comparing `RepRepBuild-0.7.4/CHANGELOG.md` & `RepRepBuild-0.8.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.8.0] - 2023-05-26
+
+### Fixed
+
+- Added sanity check to `rrr` command.
+
+### Changed
+
+- Optional customization of formatting and parsing of script arguments when using
+  `reprepbuild_cases`.
+
 ## [0.7.4] - 2023-05-15
 
 ### Fixed
 
 - Make local imports of Python scripts work when executed through RepRepBuild.
 
 ## [0.7.3] - 2023-05-10
```

### Comparing `RepRepBuild-0.7.4/COPYING` & `RepRepBuild-0.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/HEADER` & `RepRepBuild-0.8.0/HEADER`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/PKG-INFO` & `RepRepBuild-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.4
+Version: 0.8.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.4/README.md` & `RepRepBuild-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/pyproject.toml` & `RepRepBuild-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ]
 dependencies = [
     "ninja",
     "pymupdf",
     "tqdm",
     "watchdog",
     "bibsane",
+    "parse",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Issues = "https://github.com/reproducible-reporting/reprepbuild/issues"
 Source = "https://github.com/reproducible-reporting/reprepbuild/"
 Changelog = "https://github.com/reproducible-reporting/reprepbuild/blob/main/CHANGELOG.md"
```

### Comparing `RepRepBuild-0.7.4/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.8.0/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.4
+Version: 0.8.0
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.4/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.8.0/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/__init__.py` & `RepRepBuild-0.8.0/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/__main__.py` & `RepRepBuild-0.8.0/src/reprepbuild/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import re
 import subprocess
 import sys
 from glob import glob
 
 from ninja.ninja_syntax import Writer
 
-from .utils import check_script_args, import_python_path
+from .utils import format_case_args, import_python_path
 
 __all__ = ("main",)
 
 
 LATEXDIFF_CONTEXT2CMD = ",".join(
     [
         "abstract",
@@ -62,15 +62,15 @@
     "copy": {"command": "cp $in $out"},
     "latexdiff": {"command": f"latexdiff --append-context2cmd={LATEXDIFF_CONTEXT2CMD} $in > $out"},
     "reprozip": {"command": "rr-zip $out $in"},
     "reproarticlezip": {"command": "rr-article-zip $out $in"},
     "svgtopdf": {
         "command": "inkscape $in --export-filename=$out --export-type=pdf; rr-normalize-pdf $out"
     },
-    "pythonscript": {"command": "rr-python-script $in -- $args > $out", "depfile": "$noext.d"},
+    "pythonscript": {"command": "rr-python-script $in -- $argstr > $out", "depfile": "$noext.d"},
 }
 
 
 def latex_pattern(path):
     """Make ninja build commands to compile latex with pdflatex."""
     result = re.match(r"latex-(?P<prefix>[a-z0-9-]+)/(?P=prefix).tex$", path)
     if not result:
@@ -220,34 +220,36 @@
             yield "Skipped: missing reprepbuild_info"
             return
         reprepbuild_cases = getattr(pythonscript, "reprepbuild_cases", None)
         if reprepbuild_cases is None:
             build_cases = [[]]
         else:
             build_cases = reprepbuild_cases()
+        case_fmt = getattr(pythonscript, "REPREPBUILD_CASE_FMT", None)
 
         def fixpath(fn_local):
             return os.path.normpath(os.path.join(workdir, fn_local))
 
         # Loop over all cases to make build records
         for script_args in build_cases:
             build_info = reprepbuild_info(*script_args)
-            strargs = check_script_args(script_args)
-            fn_log = fixpath(f"{prefix}{strargs}.log")
+            argstr = format_case_args(script_args, case_fmt)
+            prefix_argstr = prefix if len(argstr) == 0 else f"{prefix}_{argstr}"
+            fn_log = fixpath(f"{prefix_argstr}.log")
             implicit_inputs = [fixpath(ipath) for ipath in build_info.get("inputs", [])]
             implicit_outputs = [fixpath(opath) for opath in build_info.get("outputs", [])]
             yield {
                 "inputs": path,
                 "implicit": implicit_inputs,
                 "rule": "pythonscript",
                 "implicit_outputs": implicit_outputs,
                 "outputs": fn_log,
                 "variables": {
-                    "args": " ".join(str(arg) for arg in script_args),
-                    "noext": fixpath(f"{prefix}{strargs}"),
+                    "argstr": argstr,
+                    "noext": fixpath(f"{prefix_argstr}"),
                 },
                 "default": True,
             }
     finally:
         os.chdir(orig_workdir)
```

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/articlezip.py` & `RepRepBuild-0.8.0/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/bibtex.py` & `RepRepBuild-0.8.0/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/latex.py` & `RepRepBuild-0.8.0/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/latexdep.py` & `RepRepBuild-0.8.0/src/reprepbuild/latexdep.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.8.0/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.8.0/src/reprepbuild/pythonscript.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,45 +26,34 @@
 
 """
 
 import argparse
 import os
 import sys
 
-from .utils import check_script_args, import_python_path, write_dep
+from .utils import import_python_path, parse_case_args, write_dep
 
 
 def main():
     """Main program."""
     args = parse_args()
-    script_args = [convert(script_arg) for script_arg in args.script_args]
-    return run_script(args.path_py, script_args)
+    return run_script(args.path_py, args.argstr)
 
 
 def parse_args():
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser("rr-python-script")
     parser.add_argument("path_py", help="The python script whose main function will be executed.")
     parser.add_argument(
-        "script_args", nargs="*", help="Command-line arguments for the script, if any"
+        "argstr", nargs="?", default="", help="Command-line argument for the script, if any"
     )
     return parser.parse_args()
 
 
-def convert(script_arg):
-    """Try to convert to int, then float, fallback to string."""
-    for dtype in int, float:
-        try:
-            return dtype(script_arg)
-        except ValueError:
-            pass
-    return script_arg
-
-
-def run_script(path_py, script_args):
+def run_script(path_py, argstr):
     """Run the python script and collected module dependencies."""
     if not path_py.endswith(".py"):
         print(f"Python script must have `.py` extension. Got {path_py}")
         return 2
     workdir, fn_py = os.path.split(path_py)
     prefix = fn_py[:-3]
     orig_workdir = os.getcwd()
@@ -84,17 +73,19 @@
         if reprepbuild_info is None:
             print(f"The script {path_py} has no reprepbuild_info function.")
             return -1
         script_main = getattr(pythonscript, "main", None)
         if script_main is None:
             print(f"The script {path_py} has no main function.")
             return -1
+        case_fmt = getattr(pythonscript, "REPREPBUILD_CASE_FMT", None)
 
         # Execute the functions as if the script is running inside its own dir.
-        build_info = reprepbuild_info(*script_args)
+        script_args, script_kwargs = parse_case_args(argstr, case_fmt)
+        build_info = reprepbuild_info(*script_args, **script_kwargs)
         result = script_main(**build_info)
     finally:
         os.chdir(orig_workdir)
 
     # Analyze the imported modules for the depfile.
     # Note that a depfile is sufficient and no dyndep is needed
     # because imported Python modules are not the output of previous build tasks.
@@ -106,16 +97,15 @@
         imported_paths.add(module_path)
 
     # Write the depfile.
     def fixpath(fn_local):
         return os.path.normpath(os.path.join(workdir, fn_local))
 
     # Note: only explicit outputs must be added to the depfile, not the implicit ones.
-    strargs = check_script_args(script_args)
-    noext = fixpath(f"{prefix}{strargs}")
+    noext = fixpath(prefix if len(argstr) == 0 else f"{prefix}_{argstr}")
     outputs = [(f"{noext}.log")]
     path_dep = f"{noext}.d"
     write_dep(path_dep, outputs, imported_paths)
 
     return result
```

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/repeat.py` & `RepRepBuild-0.8.0/src/reprepbuild/repeat.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import os
 import subprocess
 import time
 
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
-from .__main__ import DEFAULT_PATTERNS, DEFAULT_RULES, parse_args, write_ninja
+from .__main__ import DEFAULT_PATTERNS, DEFAULT_RULES, parse_args, sanity_check, write_ninja
 
 
 class AnyChangeHandler(FileSystemEventHandler):
     """Report file changes in the current directory."""
 
     def __init__(self):
         self._changed = True
@@ -67,14 +67,15 @@
             return
         print("  File changed:", path)
         self._changed = True
 
 
 def main():
     """Main program."""
+    sanity_check()
     args = parse_args()
     observer = Observer()
     event_handler = AnyChangeHandler()
     observer.schedule(event_handler, ".", True)
     observer.start()
     try:
         while True:
```

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/utils.py` & `RepRepBuild-0.8.0/src/reprepbuild/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,23 +34,25 @@
 
 A `dyndep` is more powerful and general, but also a bit more complicated to set up.
 """
 
 
 import importlib.util
 import os
-import re
 import sys
 
+from parse import parse
+
 __all__ = (
     "parse_inputs_fls",
     "write_dep",
     "write_dyndep",
     "import_python_path",
-    "check_script_args",
+    "format_case_args",
+    "parse_case_args",
 )
 
 
 def parse_inputs_fls(path_fls):
     """Get local inputs from an fls file."""
     # Collect inputs and outputs
     workdir = os.path.dirname(path_fls)
@@ -131,17 +133,71 @@
         # Ignore the script if it cannot be imported correctly.
         module = None
     finally:
         sys.path.remove(cwd)
     return module
 
 
-def check_script_args(script_args):
-    for script_arg in script_args:
-        if isinstance(script_arg, str):
-            if not re.match(r"^[a-zA-Z0-9_-]*$", script_arg):
-                raise ValueError(
-                    "Script argument must only contain letters, numbers, underscores, and hyphens."
-                )  # E:lin101
-        elif not isinstance(script_arg, int | float):
-            raise TypeError("A script argument must be int, float or str.")
-    return "".join(f"_{script_arg}" for script_arg in script_args)
+def format_case_args(script_args, case_fmt=None):
+    # Compatibility with old API.
+    check_underscores = False
+    if case_fmt is None:
+        check_underscores = True
+        case_fmt = "_".join(["{}"] * len(script_args))
+
+    # Interpret the yield value of reprepbuild_cases as args and kwargs.
+    args = []
+    kwargs = {}
+    if isinstance(script_args, list | tuple):
+        if (
+            len(script_args) == 2
+            and isinstance(script_args[0], list | tuple)
+            and isinstance(script_args[1], dict)
+        ):
+            args, kwargs = script_args
+        else:
+            args = script_args
+    elif isinstance(script_args, dict):
+        kwargs = script_args
+    else:
+        args = [script_args]
+
+    # Check validity of kwargs
+    if not all(isinstance(key, str) for key in kwargs):
+        raise ValueError("Keys of kwargs must be strings.")
+
+    # Format and check
+    result = case_fmt.format(*args, **kwargs)
+    if check_underscores and result.count("_") != max(0, len(script_args) - 1):
+        raise ValueError(
+            "When using underscores in script arguments, specify a REPREPBUILD_CASE_FMT"
+        )
+    if " " in result:
+        raise ValueError("Script arguments cannot contain whitespace.")
+    return result
+
+
+def parse_case_args(argstr, case_fmt=None):
+    convert = False
+    if case_fmt is None:
+        convert = True
+        if len(argstr) == 0:
+            case_fmt = ""
+        else:
+            case_fmt = "_".join(["{}"] * (argstr.count("_") + 1))
+    result = parse(case_fmt, argstr, case_sensitive=True)
+    if result is None:
+        raise ValueError(f"Could not parse argstr '{argstr}' with case_fmt '{case_fmt}'.")
+    if convert:
+        args = tuple(_naive_convert(word) for word in result.fixed)
+    else:
+        args = result.fixed
+    return args, result.named
+
+
+def _naive_convert(word):
+    for dtype in int, float:
+        try:
+            return dtype(word)
+        except ValueError:
+            pass
+    return word
```

### Comparing `RepRepBuild-0.7.4/src/reprepbuild/zip.py` & `RepRepBuild-0.8.0/src/reprepbuild/zip.py`

 * *Files identical despite different names*


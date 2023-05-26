# Comparing `tmp/calligraphy_scripting-1.1.3.tar.gz` & `tmp/calligraphy_scripting-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calligraphy_scripting-1.1.3.tar", max compression
+gzip compressed data, was "calligraphy_scripting-1.1.4.tar", max compression
```

## Comparing `calligraphy_scripting-1.1.3.tar` & `calligraphy_scripting-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1068 2022-03-07 22:50:26.146824 calligraphy_scripting-1.1.3/LICENSE
--rw-r--r--   0        0        0     2199 2022-03-07 22:50:26.146824 calligraphy_scripting-1.1.3/README.md
--rw-r--r--   0        0        0       97 2023-04-25 16:28:43.423407 calligraphy_scripting-1.1.3/calligraphy_scripting/__init__.py
--rw-r--r--   0        0        0     6395 2022-05-05 22:39:53.835662 calligraphy_scripting-1.1.3/calligraphy_scripting/cli.py
--rw-r--r--   0        0        0     7596 2022-03-22 15:31:13.712149 calligraphy_scripting-1.1.3/calligraphy_scripting/data/header.py
--rw-r--r--   0        0        0    11011 2022-05-05 22:22:36.675662 calligraphy_scripting-1.1.3/calligraphy_scripting/parser.py
--rw-r--r--   0        0        0     1536 2022-05-05 22:40:11.905662 calligraphy_scripting-1.1.3/calligraphy_scripting/runner.py
--rw-r--r--   0        0        0     4318 2022-03-08 16:20:36.089213 calligraphy_scripting-1.1.3/calligraphy_scripting/transpiler.py
--rw-r--r--   0        0        0      449 2022-05-05 22:21:51.975662 calligraphy_scripting-1.1.3/calligraphy_scripting/utils.py
--rw-r--r--   0        0        0      657 2023-04-25 16:28:45.934103 calligraphy_scripting-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 calligraphy_scripting-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2199 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/README.md
+-rw-r--r--   0        0        0       97 2023-05-26 16:53:08.118443 calligraphy_scripting-1.1.4/calligraphy_scripting/__init__.py
+-rw-r--r--   0        0        0     6395 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/calligraphy_scripting/cli.py
+-rw-r--r--   0        0        0     7596 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/calligraphy_scripting/data/header.py
+-rw-r--r--   0        0        0    13807 2023-05-26 16:59:42.732735 calligraphy_scripting-1.1.4/calligraphy_scripting/parser.py
+-rw-r--r--   0        0        0     1536 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/calligraphy_scripting/runner.py
+-rw-r--r--   0        0        0     4319 2022-11-01 14:47:03.588773 calligraphy_scripting-1.1.4/calligraphy_scripting/transpiler.py
+-rw-r--r--   0        0        0      449 2022-11-01 14:21:21.820573 calligraphy_scripting-1.1.4/calligraphy_scripting/utils.py
+-rw-r--r--   0        0        0      657 2023-05-26 16:53:07.128438 calligraphy_scripting-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 calligraphy_scripting-1.1.4/setup.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 calligraphy_scripting-1.1.4/PKG-INFO
```

### Comparing `calligraphy_scripting-1.1.3/LICENSE` & `calligraphy_scripting-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `calligraphy_scripting-1.1.3/README.md` & `calligraphy_scripting-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `calligraphy_scripting-1.1.3/calligraphy_scripting/cli.py` & `calligraphy_scripting-1.1.4/calligraphy_scripting/cli.py`

 * *Files identical despite different names*

### Comparing `calligraphy_scripting-1.1.3/calligraphy_scripting/data/header.py` & `calligraphy_scripting-1.1.4/calligraphy_scripting/data/header.py`

 * *Files identical despite different names*

### Comparing `calligraphy_scripting-1.1.3/calligraphy_scripting/parser.py` & `calligraphy_scripting-1.1.4/calligraphy_scripting/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=C0301, R1702, R0912, R0914, R0915, W1401
+# pylint: disable=C0301, R1702, R0912, R0914, R0915, W1401, C0206
 """Module to parse Calligraphy scripts into token representation"""
 
 from __future__ import annotations
 import re
 import os
 from calligraphy_scripting import transpiler
 from calligraphy_scripting import utils
@@ -229,39 +229,41 @@
     ]
     inline_bash_pattern = (
         r'[\$?]\((.*)\)(?=([^"\\]*(\\.|"([^"\\]*\\.)*[^"\\]*"))*[^"]*$)'
     )
     assignment_pattern = r"^[ \t]*\(?((?:[a-zA-Z0-9_]+\s*,?\s*)+)\)?[ \t]$"
 
     lines = [line for line in code.split("\n") if len(line.strip()) > 0]
-    variables = ["env.", "shellopts."]
+    variables = ["env", "shellopts"]
     langs = []
     imports = get_imports(code)
     functions = get_functions(code)
 
     for line in lines:
         is_python = False
         stripped = line.lstrip()
         if stripped.startswith("#") or stripped.startswith('"""'):
             langs.append("COMMENT")
             continue
+
+        parts = get_parts(stripped)
         for keyword in keywords:
-            if stripped.startswith(keyword):
+            if parts[0] == keyword:
                 is_python = True
                 break
         for var in variables:
-            if stripped.startswith(var):
+            if parts[0] == var:
                 is_python = True
                 break
         for imp in imports:
-            if stripped.startswith(imp):
+            if parts[0] == imp:
                 is_python = True
                 break
         for func in functions:
-            if stripped.startswith(func):
+            if parts[0] == func:
                 is_python = True
                 break
         if not is_python:
             inline_removed = re.sub(inline_bash_pattern, "<INLINE_BASH>", line)
             parts = inline_removed.split("=")
             if len(parts) > 1:
                 match = re.search(assignment_pattern, parts[0])
@@ -389,7 +391,100 @@
                 inline_paren_depth = depths["PAREN"]
                 in_inline = True
                 inline_indices.append([line_idx, char_idx, None])
 
         output += token
         char_idx += 1
     return output, inline_indices
+
+
+def get_in_depths(ignore: str, depths: dict) -> bool:
+    """Determine if all depths other than ignore key are 0
+
+    Args:
+        ignore (str): Key to not check for depth
+        depths (dict): Depths dictionary to check
+
+    Returns:
+        bool: Are all other depths 0
+    """
+
+    for key in depths:
+        if key == ignore:
+            continue
+        if depths[key] > 0:
+            return True
+    return False
+
+
+def get_parts(line: str) -> list[str]:
+    """Get parts of line broken by spaces and special characters
+
+    Args:
+        line (str): Line of code to split
+
+    Returns:
+        list[str]: List of split out tokens
+    """
+
+    output = []
+    buffer = ""
+    depths = {
+        "double_quote": 0,
+        "single_quote": 0,
+        "colon": 0,
+        "paren": 0,
+        "brace": 0,
+        "bracket": 0,
+    }
+    chars = {
+        "double_quote": {"char": '"'},
+        "single_quote": {"char": "'"},
+        "colon": {"char": ":"},
+        "paren": {"start": "(", "end": ")"},
+        "brace": {"start": "{", "end": "}"},
+        "bracket": {"start": "[", "end": "]"},
+    }
+
+    look_behind = ""
+    for idx, token in enumerate(line):
+        if idx > 0:
+            look_behind = line[idx - 1]
+        if token in [" ", "."]:
+            if buffer != "":
+                output.append(buffer)
+                buffer = ""
+            continue
+        special = False
+        for key in depths:
+            if not get_in_depths(key, depths):
+                if key in ["double_quote", "single_quote", "colon"]:
+                    if token == chars[key]["char"] and look_behind != "\\":
+                        if not key in ["colon"]:
+                            buffer += token
+                        if depths[key] == 0:
+                            depths[key] += 1
+                        else:
+                            depths[key] -= 1
+                            output.append(buffer)
+                            buffer = ""
+                        special = True
+                else:
+                    if token == chars[key]["start"]:
+                        if depths[key] == 0:
+                            output.append(buffer)
+                            buffer = ""
+                        depths[key] += 1
+                        buffer += chars[key]["start"]
+                        special = True
+                    elif token == chars[key]["end"]:
+                        depths[key] -= 1
+                        buffer += chars[key]["end"]
+                        if depths[key] == 0:
+                            output.append(buffer)
+                            buffer = ""
+                        special = True
+        if not special:
+            buffer += token
+    if buffer != "":
+        output.append(buffer)
+    return output
```

### Comparing `calligraphy_scripting-1.1.3/calligraphy_scripting/runner.py` & `calligraphy_scripting-1.1.4/calligraphy_scripting/runner.py`

 * *Files identical despite different names*

### Comparing `calligraphy_scripting-1.1.3/calligraphy_scripting/transpiler.py` & `calligraphy_scripting-1.1.4/calligraphy_scripting/transpiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,9 @@
             base64_cmd = base64_cmd_bytes.decode("utf8")
             if "if" in line[: inline_idx[1]].split(" "):
                 output += f'{line[:inline_idx[1]]}shell("{base64_cmd}", get_rc=True, silent={raw[0]=="?"}, format_dict={{**globals(), **locals()}}){line[inline_idx[2]:]}\n'
             else:
                 output += f'{line[:inline_idx[1]]}shell("{base64_cmd}", get_stdout=True, silent={raw[0]=="?"}, format_dict={{**globals(), **locals()}}){line[inline_idx[2]:]}\n'
 
     output = output.replace("<CALLIGRAPHY_NEWLINE>", "\n")
+
     return output
```

### Comparing `calligraphy_scripting-1.1.3/pyproject.toml` & `calligraphy_scripting-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calligraphy-scripting"
-version = "1.1.3"
+version = "1.1.4"
 description = "A hybrid language for a modern approach to shell scripting"
 authors = ["John Carter <jfcarter2358@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jfcarter2358/calligraphy"
 keywords = ["scripting", "calligraphy"]
```

### Comparing `calligraphy_scripting-1.1.3/PKG-INFO` & `calligraphy_scripting-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calligraphy-scripting
-Version: 1.1.3
+Version: 1.1.4
 Summary: A hybrid language for a modern approach to shell scripting
 Home-page: https://github.com/jfcarter2358/calligraphy
 License: MIT
 Keywords: scripting,calligraphy
 Author: John Carter
 Author-email: jfcarter2358@gmail.com
 Requires-Python: >=3.8,<4.0
```


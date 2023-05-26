# Comparing `tmp/aish-0.1.7.tar.gz` & `tmp/aish-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.7.tar", last modified: Fri May 26 11:39:04 2023, max compression
+gzip compressed data, was "aish-0.1.8.tar", last modified: Fri May 26 13:28:18 2023, max compression
```

## Comparing `aish-0.1.7.tar` & `aish-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.399951 aish-0.1.7/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.7/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:39:04.399565 aish-0.1.7/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.7/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.396050 aish-0.1.7/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.7/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)    11601 2023-05-26 11:35:44.000000 aish-0.1.7/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.7/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.398351 aish-0.1.7/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-26 11:39:04.400107 aish-0.1.7/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-26 11:38:12.000000 aish-0.1.7/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.399110 aish-0.1.7/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.7/tests/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     5006 2023-05-26 11:07:59.000000 aish-0.1.7/tests/test_chat.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 13:28:18.309225 aish-0.1.8/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.8/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 13:28:18.308816 aish-0.1.8/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.8/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 13:28:18.305218 aish-0.1.8/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.8/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)    11769 2023-05-26 13:25:41.000000 aish-0.1.8/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.8/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 13:28:18.307437 aish-0.1.8/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-26 13:28:18.000000 aish-0.1.8/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-26 13:28:18.309342 aish-0.1.8/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-26 13:25:41.000000 aish-0.1.8/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 13:28:18.308261 aish-0.1.8/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.8/tests/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     5458 2023-05-26 13:25:41.000000 aish-0.1.8/tests/test_chat.py
```

### Comparing `aish-0.1.7/LICENCE` & `aish-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1.7/PKG-INFO` & `aish-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.7
+Version: 0.1.8
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.7/README.md` & `aish-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aish-0.1.7/aish/aish.py` & `aish-0.1.8/aish/aish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 import json
 import os
 import re
-import sys
 
 import requests
 from distro import name as distro_name
 from rich import print as pprint
 from rich.console import Console
 from rich.syntax import Syntax
 
@@ -104,20 +103,20 @@
 
     for line in response.iter_lines():
         data = line.lstrip(b"data: ").decode("utf-8")
 
         if not data:
             continue
 
-        answer = process_delta(data, answer)
+        answer = process_delta(data, answer, config)
 
     return answer
 
 
-def process_delta(data, answer):
+def process_delta(data, answer, config):
     """
     Extracts and processes response from a remote server.
 
     Args:
         response: A requests.Response object containing the response from the
                   remote server.
         config: A dictionary containing configuration information.
@@ -145,24 +144,29 @@
             next_line = "\n".join(next_line)
             in_code_block = answer.count("```") % 2 == 1
             language = answer.split("```")[-1].split("\n")[0]
             if chunk.count("\n") > 0 or finish_reason == "stop":
                 console.print("", end="\r")
                 if finish_reason == "stop" and answer.count("\n") == 0:
                     ll = answer.split("\n")[-1]
-                    if not re.search("this is not a .* command", ll):
+                    if (
+                        not re.search("this is not a .* command", ll)
+                        and config["role"] == "shell"
+                    ):
                         syntax = Syntax(ll, language)
                         console.print(syntax, end="\n")
                     else:
                         console.print("", end="\n")
                 elif in_code_block and "```" not in current_line:
                     syntax = Syntax(current_line, language)
                     console.print(syntax, end="\n")
                 else:
                     console.print("", end="\n")
+            elif "```" in current_line:
+                pass
             else:
                 if not re.match(r"^[` ]+$", current_line):
                     console.print(chunk, end="")
                 else:
                     c = chunk.replace("`", " ")
                     console.print(c, end="")
             if "content" in delta:
```

### Comparing `aish-0.1.7/aish/proxy.py` & `aish-0.1.8/aish/proxy.py`

 * *Files identical despite different names*

### Comparing `aish-0.1.7/aish.egg-info/PKG-INFO` & `aish-0.1.8/aish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.7
+Version: 0.1.8
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.7/setup.py` & `aish-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aish",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
         "rich",
         "flask",
         "requests",
         "distro",
     ],
```

### Comparing `aish-0.1.7/tests/test_chat.py` & `aish-0.1.8/tests/test_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,49 +101,60 @@
         "test_responses",
     )
     with open(os.path.join(test_dir, "oneliner.txt"), "r") as f:
         lines = f.readlines()
         result = ""
         for line in lines:
             data = line.lstrip("data: ")
-            result = aish.process_delta(data, result)
+            result = aish.process_delta(data, result, {"role": "shell"})
     captured = capsys.readouterr()
-    expected_output = "test1\rtest1"
-    assert expected_output == captured.out.strip()
+    expected_output = "test1\rtest1\n"
+    assert expected_output == captured.out.replace(" ", "")
 
     with open(os.path.join(test_dir, "codeblock_short.txt"), "r") as f:
         lines = f.readlines()
         result = ""
         for line in lines:
             data = line.lstrip("data: ")
-            result = aish.process_delta(data, result)
+            result = aish.process_delta(data, result, {"role": "shell"})
     print("->", captured.out)
     captured = capsys.readouterr()
-    # remove spaces from captured
-    captured = captured.out.replace(" ", "")
-    expected_output = "test1\r\n\r\ntest2\rtest2\n\r\ntest3\r\n\r\ntest4\rtest4\ntest5\r\n->test1\rtest1\n\n"
-    assert expected_output == captured
+    expected_output = (
+        "test1\r\n\r\ntest2\rtest2\n\r\ntest3\r\n\r\n"
+        "test4\rtest4\n\r\ntest5\r\n->test1\rtest1\n\n"
+    )
+    assert expected_output == captured.out.replace(" ", "")
 
     with open(
         os.path.join(test_dir, "codeblock_ends_at_last_line_short.txt"), "r"
     ) as f:
         lines = f.readlines()
         result = ""
         for line in lines:
             data = line.lstrip("data: ")
-            result += aish.process_delta(data, result)
+            result += aish.process_delta(data, result, {"role": "shell"})
     captured = capsys.readouterr()
     expected_output = "\r\npythonsetup.pybdist_wheel\r\n\r\n"
-    captured = captured.out.replace(" ", "")
-    assert expected_output == captured
+    assert expected_output == captured.out.replace(" ", "")
+
+    with open(os.path.join(test_dir, "python_code.txt"), "r") as f:
+        lines = f.readlines()
+        result = ""
+        for line in lines:
+            data = line.lstrip("data: ")
+            result = aish.process_delta(data, result, {"role": "shell"})
+    captured = capsys.readouterr()
+    expected_output = "Test1\r\n\r\n\rtest\n\r\nTest2.\r\n"
+    assert expected_output == captured.out.replace(" ", "")
+
     with open(os.path.join(test_dir, "not_command.txt"), "r") as f:
         lines = f.readlines()
         result = ""
         for line in lines:
             data = line.lstrip("data: ")
-            result = aish.process_delta(data, result)
+            result = aish.process_delta(data, result, {"role": "shell"})
     captured = capsys.readouterr()
     expected_output = "Test. However, this is not a zsh command for Darwin 22.4.0.\r\n"
     assert expected_output == captured.out
 
 
 # python_code.txt
```


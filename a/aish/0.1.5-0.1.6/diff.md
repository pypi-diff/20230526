# Comparing `tmp/aish-0.1.5.tar.gz` & `tmp/aish-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.5.tar", last modified: Thu May 25 17:14:24 2023, max compression
+gzip compressed data, was "aish-0.1.6.tar", last modified: Fri May 26 11:17:45 2023, max compression
```

## Comparing `aish-0.1.5.tar` & `aish-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.683937 aish-0.1.5/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.5/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-25 17:14:24.683490 aish-0.1.5/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.5/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.679848 aish-0.1.5/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.5/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)    11594 2023-05-25 17:03:57.000000 aish-0.1.5/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.5/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.682029 aish-0.1.5/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-25 17:14:24.000000 aish-0.1.5/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-25 17:14:24.684069 aish-0.1.5/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-25 16:28:27.000000 aish-0.1.5/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-25 17:14:24.682841 aish-0.1.5/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.5/tests/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     6008 2023-05-25 17:12:37.000000 aish-0.1.5/tests/test_chat.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.591064 aish-0.1.6/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.6/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:17:45.590564 aish-0.1.6/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.6/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.586084 aish-0.1.6/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.6/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)    11531 2023-05-26 11:11:20.000000 aish-0.1.6/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.6/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.589011 aish-0.1.6/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-26 11:17:45.591139 aish-0.1.6/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-26 11:09:39.000000 aish-0.1.6/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.589882 aish-0.1.6/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.6/tests/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     5006 2023-05-26 11:07:59.000000 aish-0.1.6/tests/test_chat.py
```

### Comparing `aish-0.1.5/LICENCE` & `aish-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1.5/PKG-INFO` & `aish-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.5/README.md` & `aish-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aish-0.1.5/aish/aish.py` & `aish-0.1.6/aish/aish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import json
 import os
 import re
+import sys
 
 import requests
 from distro import name as distro_name
 from rich import print as pprint
 from rich.console import Console
 from rich.syntax import Syntax
 
@@ -126,61 +127,49 @@
     """
 
     global user_shell
 
     try:
         language = ""
         data = json.loads(data)
-        delta = data["choices"][0]["delta"]
-        finish_reason = data["choices"][0]["finish_reason"]
-        chunk = ""
-        if "content" in delta:
-            answer += delta["content"]
-            chunk = delta["content"]
-        elif finish_reason:
-            if answer.count("\n") == 1:
-                ll = answer.split("\n")[-1]
-                if not re.search("this is not a .* command.", ll):
-                    answer = f"```\n{ll}\n```"
-                    chunk = "```"
-                    syntax = Syntax(ll, language)
+        if data["choices"]:
+            delta = data["choices"][0]["delta"]
+            finish_reason = data["choices"][0]["finish_reason"]
+            chunk = ""
+            current_line = ""
+            current_line = answer.split("\n")[-1]
+            if "content" in delta:
+                chunk = delta["content"]
+                current_line += chunk.split("\n")[0]
+
+            next_line = chunk.split("\n")[1:]
+            next_line = "\n".join(next_line)
+            in_code_block = answer.count("```") % 2 == 1
+            if chunk.count("\n") > 0 or finish_reason == "stop":
+                console.print("", end="\r")
+                if finish_reason == "stop" and answer.count("\n") == 0:
+                    ll = answer.split("\n")[-1]
+                    if not re.search("this is not a .* command", ll):
+                        syntax = Syntax(ll, language)
+                        console.print(syntax, end="\n")
+                    else:
+                        console.print("", end="\n")
+                elif in_code_block and "```" not in current_line:
+                    syntax = Syntax(current_line, language)
                     console.print(syntax, end="\n")
                 else:
-                    console.print(ll, end="\n")
+                    console.print("", end="\n")
             else:
-                ll = answer.split("\n")[-1]
-                console.print(ll, end="\r")
-                pass
-        else:
-            answer += "\n"
-            chunk = "\n"
-        count = answer.count("```")
-        last_line = answer.split("\n")[-1]
-        in_code_block = count % 2 == 1
-
-        line_ends = chunk.count("\n")
-        if line_ends > 0 or "```" in last_line:
-            last_line = answer.split("\n")[-1 - line_ends]
-            if "```" in last_line:
-                # TODO: Handle language printout
-                console.print("            ", end="\n")
-                if in_code_block:
-                    parts = last_line.split("```")
-                    if len(parts) > 1:
-                        language = parts[1]
-                    else:
-                        language = user_shell
-
-            elif in_code_block:
-                syntax = Syntax(last_line, language)
-                console.print(syntax, end="\n")
-            else:
-                console.print(last_line, end="\n")
-        else:
-            console.print(last_line, end="\r")
+                if not re.match(r"^[` ]+$", current_line):
+                    console.print(chunk, end="")
+                else:
+                    c = chunk.replace("`", " ")
+                    console.print(c, end="")
+            if "content" in delta:
+                answer += delta["content"]
     except json.decoder.JSONDecodeError:
         pass
 
     return answer
 
 
 def get_code_blocks(answer, config):
@@ -196,15 +185,16 @@
     """
 
     code_blocks = []
     if config["role"] == "shell":
         lines = answer.split("\n")
 
         if len(lines) == 1:
-            code_blocks.append(lines[0].strip())
+            if not re.search("this is not a .* command", lines[0]):
+                code_blocks.append(lines[0].strip())
         else:
             in_code_block = False
             is_block_start = False
             for line in lines:
                 has_triple_backtick = "```" in line
                 if has_triple_backtick:
                     is_block_start = not is_block_start
@@ -244,15 +234,16 @@
         timeout=config["timeout"],
         stream=True,
     ) as response:
         response.raise_for_status()
 
         answer = process_response(response, config)
         code_blocks = get_code_blocks(answer, config)
-        execute_shell_commands(code_blocks)
+        if config["role"] == "shell":
+            execute_shell_commands(code_blocks)
 
 
 def chat(prompt, config, record=None, playback=None):
     """
     This function takes a prompt, configuration dictionary, and optional playback
     arguments. It sends a request to the OpenAI API to generate a response to the
     prompt using the specified model, temperature, and top_p values from the
```

### Comparing `aish-0.1.5/aish/proxy.py` & `aish-0.1.6/aish/proxy.py`

 * *Files identical despite different names*

### Comparing `aish-0.1.5/aish.egg-info/PKG-INFO` & `aish-0.1.6/aish.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.5/setup.py` & `aish-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aish",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         "rich",
         "flask",
         "requests",
         "distro",
     ],
```


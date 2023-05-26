# Comparing `tmp/aish-0.1.6.tar.gz` & `tmp/aish-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aish-0.1.6.tar", last modified: Fri May 26 11:17:45 2023, max compression
+gzip compressed data, was "aish-0.1.7.tar", last modified: Fri May 26 11:39:04 2023, max compression
```

## Comparing `aish-0.1.6.tar` & `aish-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.591064 aish-0.1.6/
--rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.6/LICENCE
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:17:45.590564 aish-0.1.6/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.6/README.md
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.586084 aish-0.1.6/aish/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.6/aish/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)    11531 2023-05-26 11:11:20.000000 aish-0.1.6/aish/aish.py
--rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.6/aish/proxy.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.589011 aish-0.1.6/aish.egg-info/
--rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/PKG-INFO
--rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/SOURCES.txt
--rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/dependency_links.txt
--rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/entry_points.txt
--rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/requires.txt
--rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-26 11:17:45.000000 aish-0.1.6/aish.egg-info/top_level.txt
--rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-26 11:17:45.591139 aish-0.1.6/setup.cfg
--rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-26 11:09:39.000000 aish-0.1.6/setup.py
-drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:17:45.589882 aish-0.1.6/tests/
--rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.6/tests/__init__.py
--rw-r--r--   0 toni       (501) staff       (20)     5006 2023-05-26 11:07:59.000000 aish-0.1.6/tests/test_chat.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.399951 aish-0.1.7/
+-rw-r--r--   0 toni       (501) staff       (20)     1054 2023-05-19 19:01:29.000000 aish-0.1.7/LICENCE
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:39:04.399565 aish-0.1.7/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)     1532 2023-05-22 15:47:59.000000 aish-0.1.7/README.md
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.396050 aish-0.1.7/aish/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:02.000000 aish-0.1.7/aish/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)    11601 2023-05-26 11:35:44.000000 aish-0.1.7/aish/aish.py
+-rw-r--r--   0 toni       (501) staff       (20)     3412 2023-05-25 16:56:37.000000 aish-0.1.7/aish/proxy.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.398351 aish-0.1.7/aish.egg-info/
+-rw-r--r--   0 toni       (501) staff       (20)     1772 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/PKG-INFO
+-rw-r--r--   0 toni       (501) staff       (20)      277 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/SOURCES.txt
+-rw-r--r--   0 toni       (501) staff       (20)        1 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/dependency_links.txt
+-rw-r--r--   0 toni       (501) staff       (20)       40 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/entry_points.txt
+-rw-r--r--   0 toni       (501) staff       (20)       27 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/requires.txt
+-rw-r--r--   0 toni       (501) staff       (20)       11 2023-05-26 11:39:04.000000 aish-0.1.7/aish.egg-info/top_level.txt
+-rw-r--r--   0 toni       (501) staff       (20)       38 2023-05-26 11:39:04.400107 aish-0.1.7/setup.cfg
+-rw-r--r--   0 toni       (501) staff       (20)      556 2023-05-26 11:38:12.000000 aish-0.1.7/setup.py
+drwxr-xr-x   0 toni       (501) staff       (20)        0 2023-05-26 11:39:04.399110 aish-0.1.7/tests/
+-rw-r--r--   0 toni       (501) staff       (20)        0 2023-05-21 13:54:28.000000 aish-0.1.7/tests/__init__.py
+-rw-r--r--   0 toni       (501) staff       (20)     5006 2023-05-26 11:07:59.000000 aish-0.1.7/tests/test_chat.py
```

### Comparing `aish-0.1.6/LICENCE` & `aish-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `aish-0.1.6/PKG-INFO` & `aish-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.6/README.md` & `aish-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aish-0.1.6/aish/aish.py` & `aish-0.1.7/aish/aish.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,29 +125,30 @@
     Returns:
         The answer as a string.
     """
 
     global user_shell
 
     try:
-        language = ""
+        language = user_shell
         data = json.loads(data)
         if data["choices"]:
             delta = data["choices"][0]["delta"]
             finish_reason = data["choices"][0]["finish_reason"]
             chunk = ""
             current_line = ""
             current_line = answer.split("\n")[-1]
             if "content" in delta:
                 chunk = delta["content"]
                 current_line += chunk.split("\n")[0]
 
             next_line = chunk.split("\n")[1:]
             next_line = "\n".join(next_line)
             in_code_block = answer.count("```") % 2 == 1
+            language = answer.split("```")[-1].split("\n")[0]
             if chunk.count("\n") > 0 or finish_reason == "stop":
                 console.print("", end="\r")
                 if finish_reason == "stop" and answer.count("\n") == 0:
                     ll = answer.split("\n")[-1]
                     if not re.search("this is not a .* command", ll):
                         syntax = Syntax(ll, language)
                         console.print(syntax, end="\n")
```

### Comparing `aish-0.1.6/aish/proxy.py` & `aish-0.1.7/aish/proxy.py`

 * *Files identical despite different names*

### Comparing `aish-0.1.6/aish.egg-info/PKG-INFO` & `aish-0.1.7/aish.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aish
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command-line application that interacts with the OpenAI ChatGPT API.
 Author: Toni Leino
 Author-email: toni@leino.net
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # Aish - ChatGPT CLI
```

### Comparing `aish-0.1.6/setup.py` & `aish-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aish",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         "rich",
         "flask",
         "requests",
         "distro",
     ],
```

### Comparing `aish-0.1.6/tests/test_chat.py` & `aish-0.1.7/tests/test_chat.py`

 * *Files identical despite different names*


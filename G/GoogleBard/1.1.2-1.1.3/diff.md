# Comparing `tmp/GoogleBard-1.1.2.tar.gz` & `tmp/GoogleBard-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.1.2.tar", last modified: Fri May 26 00:41:21 2023, max compression
+gzip compressed data, was "GoogleBard-1.1.3.tar", last modified: Fri May 26 13:06:24 2023, max compression
```

## Comparing `GoogleBard-1.1.2.tar` & `GoogleBard-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:06:24.071500 GoogleBard-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-05-26 13:06:01.000000 GoogleBard-1.1.3/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:06:24.067500 GoogleBard-1.1.3/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 13:06:24.000000 GoogleBard-1.1.3/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.1.2/LICENSE` & `GoogleBard-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.2/PKG-INFO` & `GoogleBard-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.1.2/README.md` & `GoogleBard-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.2/setup.py` & `GoogleBard-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.1.2",
+    version="1.1.3",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.1.2/src/Bard.py` & `GoogleBard-1.1.3/src/Bard.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,17 @@
         chat_data = json.loads(resp.content.splitlines()[3])[0][2]
         if not chat_data:
             return {"content": f"Google Bard encountered an error: {resp.content}."}
         json_chat_data = json.loads(chat_data)
         images = set()
         if len(json_chat_data) >= 3:
             if len(json_chat_data[4][0]) >= 4:
-                for img in json_chat_data[4][0][4]:
-                    images.add(img[0][0][0])
+                if json_chat_data[4][0][4]:
+                    for img in json_chat_data[4][0][4]:
+                        images.add(img[0][0][0])
         results = {
             "content": json_chat_data[0][0],
             "conversation_id": json_chat_data[1][0],
             "response_id": json_chat_data[1][1],
             "factualityQueries": json_chat_data[3],
             "textQuery": json_chat_data[2][0] if json_chat_data[2] is not None else "",
             "choices": [{"id": i[0], "content": i[1]} for i in json_chat_data[4]],
```

### Comparing `GoogleBard-1.1.2/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.1.3/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```


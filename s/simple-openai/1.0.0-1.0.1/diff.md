# Comparing `tmp/simple-openai-1.0.0.tar.gz` & `tmp/simple-openai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openai-1.0.0.tar", last modified: Sun Apr 16 15:16:14 2023, max compression
+gzip compressed data, was "simple-openai-1.0.1.tar", last modified: Fri May 26 20:36:45 2023, max compression
```

## Comparing `simple-openai-1.0.0.tar` & `simple-openai-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.679849 simple-openai-1.0.0/
--rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-1.0.0/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    16536 2023-04-16 15:16:14.679631 simple-openai-1.0.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     2639 2023-04-16 15:14:11.000000 simple-openai-1.0.0/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1179 2023-04-16 15:15:35.000000 simple-openai-1.0.0/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 15:16:14.679896 simple-openai-1.0.0/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.674804 simple-openai-1.0.0/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.677631 simple-openai-1.0.0/src/simple_openai/
--rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-1.0.0/src/simple_openai/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-1.0.0/src/simple_openai/async_simple_openai.py
--rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-1.0.0/src/simple_openai/constants.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.678643 simple-openai-1.0.0/src/simple_openai/models/
--rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-1.0.0/src/simple_openai/models/open_ai_models.py
--rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-1.0.0/src/simple_openai/responses.py
--rw-r--r--   0 steve      (501) staff       (20)     5924 2023-04-16 13:48:53.000000 simple-openai-1.0.0/src/simple_openai/simple_openai.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.678498 simple-openai-1.0.0/src/simple_openai.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    16536 2023-04-16 15:16:14.000000 simple-openai-1.0.0/src/simple_openai.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      506 2023-04-16 15:16:14.000000 simple-openai-1.0.0/src/simple_openai.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 15:16:14.000000 simple-openai-1.0.0/src/simple_openai.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       89 2023-04-16 15:16:14.000000 simple-openai-1.0.0/src/simple_openai.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2023-04-16 15:16:14.000000 simple-openai-1.0.0/src/simple_openai.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 15:16:14.679275 simple-openai-1.0.0/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 13:13:06.000000 simple-openai-1.0.0/tests/test_AsyncSimpleOpenai.py
--rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-1.0.0/tests/test_SimpleOpenai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.108009 simple-openai-1.0.1/
+-rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-1.0.1/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)    16536 2023-05-26 20:36:45.107792 simple-openai-1.0.1/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     2639 2023-04-16 15:14:11.000000 simple-openai-1.0.1/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     1179 2023-05-26 20:21:22.000000 simple-openai-1.0.1/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-26 20:36:45.108061 simple-openai-1.0.1/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.103318 simple-openai-1.0.1/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.105650 simple-openai-1.0.1/src/simple_openai/
+-rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-1.0.1/src/simple_openai/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-1.0.1/src/simple_openai/async_simple_openai.py
+-rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-1.0.1/src/simple_openai/constants.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.106804 simple-openai-1.0.1/src/simple_openai/models/
+-rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-1.0.1/src/simple_openai/models/open_ai_models.py
+-rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-1.0.1/src/simple_openai/responses.py
+-rw-r--r--   0 steve      (501) staff       (20)     6034 2023-05-26 20:20:10.000000 simple-openai-1.0.1/src/simple_openai/simple_openai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.106604 simple-openai-1.0.1/src/simple_openai.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    16536 2023-05-26 20:36:45.000000 simple-openai-1.0.1/src/simple_openai.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      506 2023-05-26 20:36:45.000000 simple-openai-1.0.1/src/simple_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-26 20:36:45.000000 simple-openai-1.0.1/src/simple_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       89 2023-05-26 20:36:45.000000 simple-openai-1.0.1/src/simple_openai.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-05-26 20:36:45.000000 simple-openai-1.0.1/src/simple_openai.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-26 20:36:45.107382 simple-openai-1.0.1/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 19:32:12.000000 simple-openai-1.0.1/tests/test_AsyncSimpleOpenai.py
+-rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-1.0.1/tests/test_SimpleOpenai.py
```

### Comparing `simple-openai-1.0.0/LICENSE` & `simple-openai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/PKG-INFO` & `simple-openai-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-1.0.0/README.md` & `simple-openai-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/pyproject.toml` & `simple-openai-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-openai"
-version = "1.0.0"
+version = "1.0.1"
 description = "Simple OpenAI API wrapper"
 readme = "README.md"
 authors = [{ name = "Stephen Schleising", email = "stephen@schleising.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `simple-openai-1.0.0/src/simple_openai/async_simple_openai.py` & `simple-openai-1.0.1/src/simple_openai/async_simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/src/simple_openai/models/open_ai_models.py` & `simple-openai-1.0.1/src/simple_openai/models/open_ai_models.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/src/simple_openai/responses.py` & `simple-openai-1.0.1/src/simple_openai/responses.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/src/simple_openai/simple_openai.py` & `simple-openai-1.0.1/src/simple_openai/simple_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             if __name__ == "__main__":
                 main()
             ```
 
         """
 
         # Create the request body
+        system_message = open_ai_models.ChatMessage(role='system', content='You are a saucy British person.')
         chat_message = open_ai_models.ChatMessage(content=prompt)
         request_body = open_ai_models.ChatRequest(messages=[chat_message])
 
         # Send the request
         response = requests.post(constants.FULL_CHAT_URL, json=request_body.dict(), headers=self._headers)
 
         # Check the status code
```

### Comparing `simple-openai-1.0.0/src/simple_openai.egg-info/PKG-INFO` & `simple-openai-1.0.1/src/simple_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-1.0.0/tests/test_AsyncSimpleOpenai.py` & `simple-openai-1.0.1/tests/test_AsyncSimpleOpenai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.0/tests/test_SimpleOpenai.py` & `simple-openai-1.0.1/tests/test_SimpleOpenai.py`

 * *Files identical despite different names*


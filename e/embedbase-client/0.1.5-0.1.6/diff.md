# Comparing `tmp/embedbase_client-0.1.5.tar.gz` & `tmp/embedbase_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.5.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.6.tar", max compression
```

## Comparing `embedbase_client-0.1.5.tar` & `embedbase_client-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/README.md
--rw-r--r--   0        0        0      389 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/__init__.py
--rw-r--r--   0        0        0    16730 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/base.py
--rw-r--r--   0        0        0     1150 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/errors.py
--rw-r--r--   0        0        0     1694 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/split.py
--rw-r--r--   0        0        0    16681 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-05-25 18:21:51.616626 embedbase_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/README.md
+-rw-r--r--   0        0        0      389 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    16767 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1717 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/split.py
+-rw-r--r--   0        0        0    16718 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3535 2023-05-26 05:43:27.430994 embedbase_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.6/PKG-INFO
```

### Comparing `embedbase_client-0.1.5/LICENSE` & `embedbase_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/README.md` & `embedbase_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/embedbase_client/async_client.py` & `embedbase_client-0.1.6/embedbase_client/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
             prompt (str): The text prompt to send to the API for generating responses.
             options (dict, optional): Options for the generation process, including history.
                                     Defaults to None.
 
         Returns:
             CustomAsyncGenerator[str, None, None]: An asynchronous generator that yields generated text data in chunks.
         """
-        url = "https://app.embedbase.xyz/api/chat"
+        url = (options and options.get("url")) or f"https://app.embedbase.xyz/api/chat"
 
         options = options or {
             "history": [],
         }
 
         system = ""
         if options.get("history"):
```

### Comparing `embedbase_client-0.1.5/embedbase_client/base.py` & `embedbase_client-0.1.6/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/embedbase_client/errors.py` & `embedbase_client-0.1.6/embedbase_client/errors.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/embedbase_client/model.py` & `embedbase_client-0.1.6/embedbase_client/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,7 +75,8 @@
 class Chat(BaseModel):
     role: str
     content: str
 
 
 class GenerateOptions(BaseModel):
     history: List[Chat]
+    url: Optional[str]
```

### Comparing `embedbase_client-0.1.5/embedbase_client/split.py` & `embedbase_client-0.1.6/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/embedbase_client/sync_client.py` & `embedbase_client-0.1.6/embedbase_client/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,15 @@
             prompt (str): The text prompt to send to the API for generating responses.
             options (dict, optional): Options for the generation process, including history.
                                     Defaults to None.
 
         Returns:
             Generator[str, None, None]: A synchronous generator that yields generated text data in chunks.
         """
-        url = "https://app.embedbase.xyz/api/chat"
+        url = (options and options.get("url")) or f"https://app.embedbase.xyz/api/chat"
 
         options = options or {
             "history": [],
         }
 
         system = ""
         if options.get("history"):
```

### Comparing `embedbase_client-0.1.5/embedbase_client/utils.py` & `embedbase_client-0.1.6/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.5/pyproject.toml` & `embedbase_client-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.5"
+version = "0.1.6"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
```

### Comparing `embedbase_client-0.1.5/PKG-INFO` & `embedbase_client-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.5 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.6 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```


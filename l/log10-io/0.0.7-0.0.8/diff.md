# Comparing `tmp/log10_io-0.0.7.tar.gz` & `tmp/log10_io-0.0.8.tar.gz`

## Comparing `log10_io-0.0.7.tar` & `log10_io-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.7/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.7/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/completion_ada.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/get_url.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.7/examples/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/        __init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/bigquery.py
--rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.7/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.7/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.7/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.7/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.8/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/completion_ada.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/get_url.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.8/examples/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/bigquery.py
+-rw-r--r--   0        0        0    11138 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.8/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.8/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.8/PKG-INFO
```

### Comparing `log10_io-0.0.7/.github/workflows/release.yml` & `log10_io-0.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/chatcompletion_async_vs_sync.py` & `log10_io-0.0.8/examples/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/get_url.py` & `log10_io-0.0.8/examples/get_url.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/langchain_babyagi.py` & `log10_io-0.0.8/examples/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/langchain_multiple_tools.py` & `log10_io-0.0.8/examples/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/langchain_qa.py` & `log10_io-0.0.8/examples/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/langchain_simple_sequential.py` & `log10_io-0.0.8/examples/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/langchain_sqlagent.py` & `log10_io-0.0.8/examples/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/examples/multiple_sessions.py` & `log10_io-0.0.8/examples/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/log10/bigquery.py` & `log10_io-0.0.8/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/log10/load.py` & `log10_io-0.0.8/log10/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from aiohttp import ClientSession
 import asyncio
 import threading
 import queue
 from contextlib import contextmanager
 import logging
 from dotenv import load_dotenv
+import backoff  # for exponential backoff
+from openai.error import RateLimitError
 
 load_dotenv()
 
 url = os.environ.get("LOG10_URL")
 token = os.environ.get("LOG10_TOKEN")
 org_id = os.environ.get("LOG10_ORG_ID")
 
@@ -28,14 +30,19 @@
     bigquery_client, bigquery_table = initialize_bigquery()
     import uuid
     from datetime import datetime, timezone
 elif target_service is None:
     target_service = "log10"  # default to log10
 
 
+@backoff.on_exception(backoff.expo, RateLimitError)
+def func_with_backoff(func, *args, **kwargs):
+    return func(*args, **kwargs)
+
+
 def get_session_id():
     if target_service == "bigquery":
         return str(uuid.uuid4())
 
     try:
         session_url = url + "/api/sessions"
         res = requests.request("POST",
@@ -181,15 +188,15 @@
             current_stack_frame = traceback.extract_stack()
             stacktrace = ([{"file": frame.filename,
                           "line": frame.line,
                            "lineno": frame.lineno,
                             "name": frame.name} for frame in current_stack_frame])
 
             start_time = time.perf_counter()
-            output = func(*args, **kwargs)
+            output = func_with_backoff(func, *args, **kwargs)
             duration = time.perf_counter() - start_time
             logging.debug(
                 f"LOG10: TIMED BLOCK - OpenAI call duration: {duration}")
 
             if USE_ASYNC:
                 with timed_block("extra time spent waiting for log10 call"):
                     while result_queue.empty():
```

### Comparing `log10_io-0.0.7/log10/schemas/bigquery.json` & `log10_io-0.0.8/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/LICENSE` & `log10_io-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/README.md` & `log10_io-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.7/pyproject.toml` & `log10_io-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.7"
+version = "0.0.8"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.7/PKG-INFO` & `log10_io-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


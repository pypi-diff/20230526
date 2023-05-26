# Comparing `tmp/strangeworks_qiskit-0.4.2.tar.gz` & `tmp/strangeworks_qiskit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit-0.4.2.tar", max compression
+gzip compressed data, was "strangeworks_qiskit-0.4.3.tar", max compression
```

## Comparing `strangeworks_qiskit-0.4.2.tar` & `strangeworks_qiskit-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      457 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/LICENSE
--rw-r--r--   0        0        0     1126 2023-05-10 12:45:43.763761 strangeworks_qiskit-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      392 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/__init__.py
--rw-r--r--   0        0        0     6009 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/_runtime_client.py
--rw-r--r--   0        0        0      916 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/__init__.py
--rw-r--r--   0        0        0     1427 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/_utils.py
--rw-r--r--   0        0        0     1563 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/aws.py
--rw-r--r--   0        0        0      604 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/honeywell.py
--rw-r--r--   0        0        0     8413 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/ibm.py
--rw-r--r--   0        0        0      599 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/ionq.py
--rw-r--r--   0        0        0      932 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/rigetti.py
--rw-r--r--   0        0        0     3497 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/strangeworks.py
--rw-r--r--   0        0        0        0 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/jobs/__init__.py
--rw-r--r--   0        0        0     5014 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/jobs/job.py
--rw-r--r--   0        0        0      884 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/jobs/status.py
--rw-r--r--   0        0        0       74 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/platform/__init__.py
--rw-r--r--   0        0        0     4649 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/platform/backends.py
--rw-r--r--   0        0        0     4350 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/provider.py
--rw-r--r--   0        0        0     9110 2023-05-10 12:45:30.755578 strangeworks_qiskit-0.4.2/strangeworks_qiskit/runtimes.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1126 2023-05-26 06:38:52.581667 strangeworks_qiskit-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/__init__.py
+-rw-r--r--   0        0        0     6009 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/_runtime_client.py
+-rw-r--r--   0        0        0      916 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/__init__.py
+-rw-r--r--   0        0        0     1427 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/_utils.py
+-rw-r--r--   0        0        0     1563 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/aws.py
+-rw-r--r--   0        0        0      604 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/honeywell.py
+-rw-r--r--   0        0        0     8413 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ibm.py
+-rw-r--r--   0        0        0      599 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ionq.py
+-rw-r--r--   0        0        0      932 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/rigetti.py
+-rw-r--r--   0        0        0     3497 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/strangeworks.py
+-rw-r--r--   0        0        0        0 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/__init__.py
+-rw-r--r--   0        0        0     5038 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/job.py
+-rw-r--r--   0        0        0      884 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/status.py
+-rw-r--r--   0        0        0       74 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/__init__.py
+-rw-r--r--   0        0        0     4649 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/backends.py
+-rw-r--r--   0        0        0     4350 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/provider.py
+-rw-r--r--   0        0        0     9110 2023-05-26 06:38:27.673478 strangeworks_qiskit-0.4.3/strangeworks_qiskit/runtimes.py
+-rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 strangeworks_qiskit-0.4.3/PKG-INFO
```

### Comparing `strangeworks_qiskit-0.4.2/LICENSE` & `strangeworks_qiskit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/pyproject.toml` & `strangeworks_qiskit-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 max-line-length = 88
 per-file-ignores = [
     "__init__.py:F401"
 ]
 
 [tool.poetry]
 name = "strangeworks-qiskit"
-version = "0.4.2"
+version = "0.4.3"
 description = "Strangeworks Qiskit SDK Extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_qiskit"},
 ]
```

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/_runtime_client.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/_runtime_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/__init__.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/_utils.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/_utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/aws.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/aws.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/honeywell.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/honeywell.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/ibm.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ibm.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/ionq.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/rigetti.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/rigetti.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/backends/strangeworks.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/backends/strangeworks.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/jobs/job.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
                     product_slug=self._product_slug,
                     payload={"slug": self._job_slug},
                     endpoint="get_job_results",
                 )
                 files = sw_job.get("files")
                 if files:
                     result_file = [
-                        f.get("url")
+                        f.get("file").get("url")
                         for f in files
-                        if f.get("file_name") == "job_results.json"
+                        if f.get("file").get("file_name") == "job_results.json"
                     ]
                     results_json = self._sdk_client.download_job_files(result_file)
                     self._result = Result.from_dict(results_json[0])
 
         return self._result
 
     def submit(self, **kwargs):
```

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/jobs/status.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/jobs/status.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/platform/backends.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/platform/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/provider.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/provider.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/strangeworks_qiskit/runtimes.py` & `strangeworks_qiskit-0.4.3/strangeworks_qiskit/runtimes.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit-0.4.2/PKG-INFO` & `strangeworks_qiskit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qiskit
-Version: 0.4.2
+Version: 0.4.3
 Summary: Strangeworks Qiskit SDK Extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


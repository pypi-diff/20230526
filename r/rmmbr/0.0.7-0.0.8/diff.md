# Comparing `tmp/rmmbr-0.0.7.tar.gz` & `tmp/rmmbr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmmbr-0.0.7.tar", last modified: Sun May 21 21:03:59 2023, max compression
+gzip compressed data, was "rmmbr-0.0.8.tar", last modified: Fri May 26 10:28:25 2023, max compression
```

## Comparing `rmmbr-0.0.7.tar` & `rmmbr-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-21 21:03:59.344741 rmmbr-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/rmmbr/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-21 21:03:48.000000 rmmbr-0.0.7/rmmbr/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:03:59.344741 rmmbr-0.0.7/rmmbr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 21:03:59.000000 rmmbr-0.0.7/rmmbr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:03:59.344741 rmmbr-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-21 21:03:48.000000 rmmbr-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 10:28:25.170658 rmmbr-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/rmmbr/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 10:28:15.000000 rmmbr-0.0.8/rmmbr/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:28:25.170658 rmmbr-0.0.8/rmmbr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 10:28:25.000000 rmmbr-0.0.8/rmmbr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:28:25.170658 rmmbr-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 10:28:15.000000 rmmbr-0.0.8/setup.py
```

### Comparing `rmmbr-0.0.7/PKG-INFO` & `rmmbr-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -49,25 +49,23 @@
 ```sh
 pip install rmmbr
 ```
 
 ```python
 from rmmbr import cloud_cache
 
-cacher = cloud_cache(
+n_called = 0
+
+@cloud_cache(
     "https://rmmbr.net",
     "your-service-token",
     "some name for the cache",
     60 * 60 * 24, # TTL is one day.
     "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
 )
-
-n_called = 0
-
-@cacher
 async def f(x: int):
   nonlocal n_called
   n_called += 1
   return x
 
 await f(3)
 await f(3)
@@ -114,7 +112,13 @@
 | ----------- | --------- | ----------------- | -------------- | --------- |
 | Free        | 10,000    | 10 MB             | 1 KB           | 1000      |
 | \$100/month | 1,000,000 | 1 GB              | 100 KB         | Unlimited |
 
 ## Regions
 
 We currently deploy a backend in us-east region. Please post an issue if you have a need to configure this.
+
+## Performance and benchmarking
+
+Currently the cloud cache adds around 190ms to the call in miss cases and takes 124ms in hit cases.
+
+![Benchmark](benchmark.png)
```

### Comparing `rmmbr-0.0.7/rmmbr/crypto.py` & `rmmbr-0.0.8/rmmbr/crypto.py`

 * *Files identical despite different names*

### Comparing `rmmbr-0.0.7/rmmbr/main.py` & `rmmbr-0.0.8/rmmbr/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,27 +115,35 @@
 
 
 def local_cache(id: str):
     read, write = _make_local_read_write(id)
     return lambda f: _abstract_cache_params(_key_arguments, f, read, write)
 
 
+class RmmbrAuthError(Exception):
+    pass
+
+
 async def _call_api(url: str, token: str, method: str, params):
     async with httpx.AsyncClient() as client:
         response = await client.post(
             url=url,
             json={
                 "method": method,
                 "params": params,
             },
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {token}",
             },
         )
+        if response.status_code == 401:
+            raise RmmbrAuthError(
+                "rmmbr authentication failure. Is the API token valid?"
+            )
         return response.json()
 
 
 def _set_remote(
     url: str,
     token: str,
     cache_id: str,
```

### Comparing `rmmbr-0.0.7/rmmbr/main_test.py` & `rmmbr-0.0.8/rmmbr/main_test.py`

 * *Files identical despite different names*

### Comparing `rmmbr-0.0.7/rmmbr.egg-info/PKG-INFO` & `rmmbr-0.0.8/rmmbr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmmbr
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple persistent caching.
 Home-page: https://github.com/uriva/rmmbr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
@@ -49,25 +49,23 @@
 ```sh
 pip install rmmbr
 ```
 
 ```python
 from rmmbr import cloud_cache
 
-cacher = cloud_cache(
+n_called = 0
+
+@cloud_cache(
     "https://rmmbr.net",
     "your-service-token",
     "some name for the cache",
     60 * 60 * 24, # TTL is one day.
     "Cqq33cbHu9AEUaP_wS3LCDQN7wy40XKWzALoPHbU5S8=",
 )
-
-n_called = 0
-
-@cacher
 async def f(x: int):
   nonlocal n_called
   n_called += 1
   return x
 
 await f(3)
 await f(3)
@@ -114,7 +112,13 @@
 | ----------- | --------- | ----------------- | -------------- | --------- |
 | Free        | 10,000    | 10 MB             | 1 KB           | 1000      |
 | \$100/month | 1,000,000 | 1 GB              | 100 KB         | Unlimited |
 
 ## Regions
 
 We currently deploy a backend in us-east region. Please post an issue if you have a need to configure this.
+
+## Performance and benchmarking
+
+Currently the cloud cache adds around 190ms to the call in miss cases and takes 124ms in hit cases.
+
+![Benchmark](benchmark.png)
```

### Comparing `rmmbr-0.0.7/setup.py` & `rmmbr-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 _repo_dir = os.environ.get("GITHUB_WORKSPACE")
 assert _repo_dir
 setup(
     name="rmmbr",
-    version="0.0.7",
+    version="0.0.8",
     description="Simple persistent caching.",
     long_description=(pathlib.Path(_repo_dir) / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/uriva/rmmbr",
     packages=find_packages(),
     install_requires=[
         "redis>=3.5.3",
```


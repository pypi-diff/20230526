# Comparing `tmp/openet_client-2023.5.25.tar.gz` & `tmp/openet_client-2023.5.251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openet_client-2023.5.25.tar", last modified: Thu May 25 21:37:47 2023, max compression
+gzip compressed data, was "dist\openet_client-2023.5.251.tar", last modified: Thu May 25 22:49:54 2023, max compression
```

## Comparing `openet_client-2023.5.25.tar` & `openet_client-2023.5.251.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 21:37:47.622959 openet_client-2023.5.25/
--rw-rw-rw-   0        0        0     1117 2022-06-02 20:57:06.000000 openet_client-2023.5.25/LICENSE
--rw-rw-rw-   0        0        0      768 2023-05-25 21:37:47.620958 openet_client-2023.5.25/PKG-INFO
--rw-rw-rw-   0        0        0     7465 2022-06-03 18:24:14.000000 openet_client-2023.5.25/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 21:37:47.579699 openet_client-2023.5.25/openet_client/
--rw-rw-rw-   0        0        0      221 2023-05-25 21:35:35.000000 openet_client-2023.5.25/openet_client/__init__.py
--rw-rw-rw-   0        0        0     3673 2022-06-10 22:55:07.000000 openet_client-2023.5.25/openet_client/cache.py
--rw-rw-rw-   0        0        0     4627 2023-05-24 18:17:48.000000 openet_client-2023.5.25/openet_client/client.py
--rw-rw-rw-   0        0        0      459 2022-06-02 20:57:06.000000 openet_client-2023.5.25/openet_client/exceptions.py
--rw-rw-rw-   0        0        0    13578 2022-06-09 21:19:37.000000 openet_client-2023.5.25/openet_client/geodatabase.py
--rw-rw-rw-   0        0        0    11901 2022-09-07 21:16:48.000000 openet_client-2023.5.25/openet_client/raster.py
--rw-rw-rw-   0        0        0    12542 2022-06-13 23:47:47.000000 openet_client-2023.5.25/openet_client/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:37:47.602549 openet_client-2023.5.25/openet_client.egg-info/
--rw-rw-rw-   0        0        0      768 2023-05-25 21:37:47.000000 openet_client-2023.5.25/openet_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-05-25 21:37:47.000000 openet_client-2023.5.25/openet_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 21:37:47.000000 openet_client-2023.5.25/openet_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 21:37:47.000000 openet_client-2023.5.25/openet_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 21:37:47.000000 openet_client-2023.5.25/openet_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 21:37:47.622959 openet_client-2023.5.25/setup.cfg
--rw-rw-rw-   0        0        0     1297 2022-06-13 23:24:29.000000 openet_client-2023.5.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 21:37:47.615945 openet_client-2023.5.25/tests/
--rw-rw-rw-   0        0        0     1590 2022-06-02 20:57:06.000000 openet_client-2023.5.25/tests/test_basic.py
--rw-rw-rw-   0        0        0      881 2022-06-02 20:57:06.000000 openet_client-2023.5.25/tests/test_geodatabase.py
--rw-rw-rw-   0        0        0     1345 2022-06-10 22:54:32.000000 openet_client-2023.5.25/tests/test_raster_timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:49:54.000000 openet_client-2023.5.251/
+-rw-rw-rw-   0        0        0     1117 2022-06-02 20:57:06.000000 openet_client-2023.5.251/LICENSE
+-rw-rw-rw-   0        0        0      776 2023-05-25 22:49:54.000000 openet_client-2023.5.251/PKG-INFO
+-rw-rw-rw-   0        0        0     7465 2022-06-03 18:24:14.000000 openet_client-2023.5.251/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 22:49:54.000000 openet_client-2023.5.251/openet_client/
+-rw-rw-rw-   0        0        0      222 2023-05-25 22:48:42.000000 openet_client-2023.5.251/openet_client/__init__.py
+-rw-rw-rw-   0        0        0     3673 2022-06-10 22:55:07.000000 openet_client-2023.5.251/openet_client/cache.py
+-rw-rw-rw-   0        0        0     5180 2023-05-25 22:15:55.000000 openet_client-2023.5.251/openet_client/client.py
+-rw-rw-rw-   0        0        0      459 2022-06-02 20:57:06.000000 openet_client-2023.5.251/openet_client/exceptions.py
+-rw-rw-rw-   0        0        0    13578 2023-05-25 22:49:04.000000 openet_client-2023.5.251/openet_client/geodatabase.py
+-rw-rw-rw-   0        0        0    11901 2022-09-07 21:16:48.000000 openet_client-2023.5.251/openet_client/raster.py
+-rw-rw-rw-   0        0        0    12542 2022-06-13 23:47:47.000000 openet_client-2023.5.251/openet_client/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:49:54.000000 openet_client-2023.5.251/openet_client.egg-info/
+-rw-rw-rw-   0        0        0      776 2023-05-25 22:49:53.000000 openet_client-2023.5.251/openet_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-05-25 22:49:53.000000 openet_client-2023.5.251/openet_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:49:53.000000 openet_client-2023.5.251/openet_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 22:49:53.000000 openet_client-2023.5.251/openet_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 22:49:53.000000 openet_client-2023.5.251/openet_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 22:49:54.000000 openet_client-2023.5.251/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2022-06-13 23:24:29.000000 openet_client-2023.5.251/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:49:54.000000 openet_client-2023.5.251/tests/
+-rw-rw-rw-   0        0        0     1590 2022-06-02 20:57:06.000000 openet_client-2023.5.251/tests/test_basic.py
+-rw-rw-rw-   0        0        0      881 2022-06-02 20:57:06.000000 openet_client-2023.5.251/tests/test_geodatabase.py
+-rw-rw-rw-   0        0        0     1345 2022-06-10 22:54:32.000000 openet_client-2023.5.251/tests/test_raster_timeseries.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `openet_client-2023.5.25/LICENSE` & `openet_client-2023.5.251/LICENSE`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/PKG-INFO` & `openet_client-2023.5.251/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: openet_client
-Version: 2023.5.25
+Version: 2023.5.251
 Summary: Client for the OpenET web API with useful wrappers to support common workflows and needs with the API
 Home-page: https://github.com/water3d/openet/
 Author: nickrsan
 Author-email: nsantos5@ucmerced.edu
 License: MIT
-License-File: LICENSE
-
-See README at https://github.com/water3d/openet/ for more details. Make sure to install package extras (e.g. pip install 'openet-client[spatial]') for spatial data support in the geodatabase API. It depends on Geopandas, which depends on fiona - this can be challenging to get set up correctly, so it's worth checking the documentation for those projects to install on your system, or use a conda environment and install the conda geopandas package.
+Description: See README at https://github.com/water3d/openet/ for more details. Make sure to install package extras (e.g. pip install 'openet-client[spatial]') for spatial data support in the geodatabase API. It depends on Geopandas, which depends on fiona - this can be challenging to get set up correctly, so it's worth checking the documentation for those projects to install on your system, or use a conda environment and install the conda geopandas package.
+Platform: UNKNOWN
```

### Comparing `openet_client-2023.5.25/README.md` & `openet_client-2023.5.251/README.md`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/openet_client/cache.py` & `openet_client-2023.5.251/openet_client/cache.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/openet_client/client.py` & `openet_client-2023.5.251/openet_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .cache import Cacher
 
 
 class OpenETClient(object):
     token = None
     _base_url = "https://openet.dri.edu/"
     _validate_ssl = False
-    force_raise_request_errors = False # raises errors for all request errors before sending data for processing. Default is False to let calling code receive and handle errors, but can be set to True here to catch all errors labeled HTTP 400 - 599 regardless of if we handle them
+    force_raise_request_errors = True # raises errors for all request errors before sending data for processing. Default is False to let calling code receive and handle errors, but can be set to True here to catch all errors labeled HTTP 400 - 599 regardless of if we handle them. Need to change how geodatabase code handles rate limiting before can change to True
 
     def __init__(self, token=None):
         self.token = token
         self.raster = RasterManager(client=self)
         self.geodatabase = Geodatabase(client=self)
         self.cache = Cacher()
         self._last_request = None  # just for debugging
@@ -31,27 +31,38 @@
             raise AuthenticationError("Token missing/undefined - you must set the value of your token before proceeding")
 
     def _check_status(self):
         if self._last_request.status_code >= 200 and self._last_request.status_code < 400:
             return
 
         r = self._last_request
-        text = json.loads(r.text)
+        try:
+            text = r.json()
+        except json.decoder.JSONDecodeError:
+            text = r.text
+
+        if "description" in text:
+            description = text["description"]
+        else:
+            description = ""
 
         if r.status_code == 401 and "detail" in text and text["detail"] == "Invalid API token":
             raise AuthenticationError("The API reports that your token is invalid - it may have expired and you will need to get your token reiussed."
                                       " As of mid-2023, you do this by contacting OpenET staff via their API documentation contact form at"
                                       " https://openetdata.org/contact/")
 
-        if r.status_code in (500, 404) and "reached your maximum rate limit" in r.json()["description"]:
+        if r.status_code in (500, 404) and "reached your maximum rate limit" in description:
             raise RateLimitError("Server indicates we've reached our rate limit - try increasing the wait time between requests")
 
         if r.status_code >= 400 and r.status_code <= 599:
             if self.force_raise_request_errors:
                 raise BadRequestError(f"API Reported HTTP {r.status_code} and text information of {r.text}")
+            else:
+                print(f"Warning: Received an HTTP 400 or 500 status code from the API - proceeding in case we can handle it"
+                      f"but if you get a crash, the API API Reported HTTP {r.status_code} and text information of {text}")
 
     def send_request(self, endpoint, method="get", disable_encoding=False, **kwargs):
         """
             Handles sending most requests to the API - they provide the endpoint and the args.
             Since the API is in the process of switching from GET to POST requests, we have logic that switches between
             those depending on the request method
         :param endpoint: The text path to the OpenET endpoint - e.g. raster/export - skip the base URL.
@@ -89,13 +100,14 @@
             body = json.dumps(send_kwargs)
             result = requester(url, headers={"Authorization": self.token}, data=body, **extra_kwargs)
         else:
             body = send_kwargs
             result = requester(url, headers={"Authorization": self.token}, params=body, **extra_kwargs)
         self._last_request = result
 
+        self._check_status()
+
         # cache the request and response so that if anything goes wrong, we've saved the data
         self.cache.cache_request(url, body, result.status_code, json.dumps(result.json()))
 
-        self._check_status()
 
         return result
```

### Comparing `openet_client-2023.5.25/openet_client/geodatabase.py` & `openet_client-2023.5.251/openet_client/geodatabase.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/openet_client/raster.py` & `openet_client-2023.5.251/openet_client/raster.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/openet_client/timeseries.py` & `openet_client-2023.5.251/openet_client/timeseries.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/openet_client.egg-info/PKG-INFO` & `openet_client-2023.5.251/openet_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: openet-client
-Version: 2023.5.25
+Version: 2023.5.251
 Summary: Client for the OpenET web API with useful wrappers to support common workflows and needs with the API
 Home-page: https://github.com/water3d/openet/
 Author: nickrsan
 Author-email: nsantos5@ucmerced.edu
 License: MIT
-License-File: LICENSE
-
-See README at https://github.com/water3d/openet/ for more details. Make sure to install package extras (e.g. pip install 'openet-client[spatial]') for spatial data support in the geodatabase API. It depends on Geopandas, which depends on fiona - this can be challenging to get set up correctly, so it's worth checking the documentation for those projects to install on your system, or use a conda environment and install the conda geopandas package.
+Description: See README at https://github.com/water3d/openet/ for more details. Make sure to install package extras (e.g. pip install 'openet-client[spatial]') for spatial data support in the geodatabase API. It depends on Geopandas, which depends on fiona - this can be challenging to get set up correctly, so it's worth checking the documentation for those projects to install on your system, or use a conda environment and install the conda geopandas package.
+Platform: UNKNOWN
```

### Comparing `openet_client-2023.5.25/setup.py` & `openet_client-2023.5.251/setup.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/tests/test_basic.py` & `openet_client-2023.5.251/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/tests/test_geodatabase.py` & `openet_client-2023.5.251/tests/test_geodatabase.py`

 * *Files identical despite different names*

### Comparing `openet_client-2023.5.25/tests/test_raster_timeseries.py` & `openet_client-2023.5.251/tests/test_raster_timeseries.py`

 * *Files identical despite different names*


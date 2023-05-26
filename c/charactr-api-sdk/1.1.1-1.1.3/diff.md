# Comparing `tmp/charactr_api_sdk-1.1.1.tar.gz` & `tmp/charactr_api_sdk-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charactr_api_sdk-1.1.1.tar", last modified: Fri May 19 12:09:20 2023, max compression
+gzip compressed data, was "charactr_api_sdk-1.1.3.tar", last modified: Fri May 26 13:11:30 2023, max compression
```

## Comparing `charactr_api_sdk-1.1.1.tar` & `charactr_api_sdk-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 12:09:20.297010 charactr_api_sdk-1.1.1/
--rw-r--r--   0 wiktormazur   (501) staff       (20)    15061 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/LICENSE.rst
--rw-r--r--   0 wiktormazur   (501) staff       (20)       24 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/MANIFEST.in
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-19 12:09:20.297127 charactr_api_sdk-1.1.1/PKG-INFO
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1423 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/README.md
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 12:09:20.290975 charactr_api_sdk-1.1.1/charactr_api/
--rw-r--r--   0 wiktormazur   (501) staff       (20)      119 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/charactr_api/__init__.py
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 12:09:20.295302 charactr_api_sdk-1.1.1/charactr_api/sdk/
--rw-r--r--   0 wiktormazur   (501) staff       (20)        0 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/__init__.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      139 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/config.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1059 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/conversion_module.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      780 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/data_objects.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1135 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/errors.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)      269 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/sdk.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     2387 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/tts.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     3983 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/tts_stream_duplex.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1961 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/tts_stream_simplex.py
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1478 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.1/charactr_api/sdk/vc.py
-drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-19 12:09:20.296765 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/
--rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-19 12:09:19.000000 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 wiktormazur   (501) staff       (20)      595 2023-05-19 12:09:20.000000 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)        1 2023-05-19 12:09:19.000000 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-19 12:09:20.000000 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/requires.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       13 2023-05-19 12:09:20.000000 charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.1/requirements.txt
--rw-r--r--   0 wiktormazur   (501) staff       (20)      107 2023-05-19 12:09:20.297563 charactr_api_sdk-1.1.1/setup.cfg
--rw-r--r--   0 wiktormazur   (501) staff       (20)      660 2023-05-19 12:09:09.000000 charactr_api_sdk-1.1.1/setup.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-26 13:11:30.330376 charactr_api_sdk-1.1.3/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)    15061 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/LICENSE.rst
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       24 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/MANIFEST.in
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-26 13:11:30.330536 charactr_api_sdk-1.1.3/PKG-INFO
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1423 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/README.md
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-26 13:11:30.322315 charactr_api_sdk-1.1.3/charactr_api/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      119 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/charactr_api/__init__.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-26 13:11:30.327343 charactr_api_sdk-1.1.3/charactr_api/sdk/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)        0 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/__init__.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      139 2023-05-26 13:06:49.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/config.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1059 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/conversion_module.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      780 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/data_objects.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1135 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/errors.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      269 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/sdk.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     2387 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/tts.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     3983 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/tts_stream_duplex.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     2052 2023-05-26 13:06:50.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/tts_stream_simplex.py
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1478 2023-05-15 14:22:09.000000 charactr_api_sdk-1.1.3/charactr_api/sdk/vc.py
+drwxr-xr-x   0 wiktormazur   (501) staff       (20)        0 2023-05-26 13:11:30.329977 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/
+-rw-r--r--   0 wiktormazur   (501) staff       (20)     1754 2023-05-26 13:11:30.000000 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      595 2023-05-26 13:11:30.000000 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)        1 2023-05-26 13:11:30.000000 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-26 13:11:30.000000 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       13 2023-05-26 13:11:30.000000 charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)       81 2023-05-19 12:05:52.000000 charactr_api_sdk-1.1.3/requirements.txt
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      107 2023-05-26 13:11:30.331126 charactr_api_sdk-1.1.3/setup.cfg
+-rw-r--r--   0 wiktormazur   (501) staff       (20)      660 2023-05-26 13:07:40.000000 charactr_api_sdk-1.1.3/setup.py
```

### Comparing `charactr_api_sdk-1.1.1/LICENSE.rst` & `charactr_api_sdk-1.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/PKG-INFO` & `charactr_api_sdk-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: charactr_api_sdk
-Version: 1.1.1
+Version: 1.1.3
 Summary: Python SDK to interact with the charactr API.
 Home-page: https://github.com/charactr-platform/charactr-api-sdk-python
 Author: charactr
 Author-email: support@charactr.com
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # charactr-api-sdk-python
 
 Python SDK to interact with the charactr API.
```

### Comparing `charactr_api_sdk-1.1.1/README.md` & `charactr_api_sdk-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/conversion_module.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/conversion_module.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/data_objects.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/data_objects.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/errors.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/tts.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/tts.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/tts_stream_duplex.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/tts_stream_duplex.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/tts_stream_simplex.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/tts_stream_simplex.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         self.text = text
         self.on_data = on_data
         self.on_close = on_close
         self.__on_close_event = threading.Event()
 
         self.ws = websocket.WebSocketApp(
             WS_API_URL + "/v1/tts/stream/simplex/ws?voiceId=" + str(self.voice_id),
+            header={
+              "User-Agent": "charactr-api-sdk-python",
+            },
             on_open=self.__on_open,
             on_message=self.__on_message,
             on_close=self.__on_close,
         )
 
         wst = threading.Thread(
             target=self.ws.run_forever, kwargs={"ping_interval": 5, "ping_timeout": 2}
```

### Comparing `charactr_api_sdk-1.1.1/charactr_api/sdk/vc.py` & `charactr_api_sdk-1.1.3/charactr_api/sdk/vc.py`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/PKG-INFO` & `charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: charactr-api-sdk
-Version: 1.1.1
+Version: 1.1.3
 Summary: Python SDK to interact with the charactr API.
 Home-page: https://github.com/charactr-platform/charactr-api-sdk-python
 Author: charactr
 Author-email: support@charactr.com
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # charactr-api-sdk-python
 
 Python SDK to interact with the charactr API.
```

### Comparing `charactr_api_sdk-1.1.1/charactr_api_sdk.egg-info/SOURCES.txt` & `charactr_api_sdk-1.1.3/charactr_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `charactr_api_sdk-1.1.1/setup.py` & `charactr_api_sdk-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     requirements = req_f.read().splitlines()
 
 setup(
     name="charactr_api_sdk",
     description="Python SDK to interact with the charactr API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
-    version="1.1.1",
+    version="1.1.3",
     author="charactr",
     author_email="support@charactr.com",
     url="https://github.com/charactr-platform/charactr-api-sdk-python",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
-    python_requires=">=3.8.0",
+    python_requires=">=3.9.0",
     setup_requires=["setuptools==58.0.4"],
 )
```


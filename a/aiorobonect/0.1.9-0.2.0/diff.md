# Comparing `tmp/aiorobonect-0.1.9.tar.gz` & `tmp/aiorobonect-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.1.9.tar", last modified: Sat May 20 16:21:07 2023, max compression
+gzip compressed data, was "aiorobonect-0.2.0.tar", last modified: Fri May 26 07:51:54 2023, max compression
```

## Comparing `aiorobonect-0.1.9.tar` & `aiorobonect-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-20 16:20:46.000000 aiorobonect-0.1.9/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 16:21:07.000000 aiorobonect-0.1.9/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 16:21:07.226376 aiorobonect-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 16:20:49.000000 aiorobonect-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.275972 aiorobonect-0.2.0/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.275972 aiorobonect-0.2.0/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 07:51:30.000000 aiorobonect-0.2.0/setup.py
```

### Comparing `aiorobonect-0.1.9/LICENSE` & `aiorobonect-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.9/PKG-INFO` & `aiorobonect-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.9
+Version: 0.2.0
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.9/README.md` & `aiorobonect-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.1.9/aiorobonect/client.py` & `aiorobonect-0.2.0/aiorobonect/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,49 @@
 """Robonect library using aiohttp."""
 from __future__ import annotations
 
+import json
 import logging
 import urllib.parse
 
 import aiohttp
 
 from .const import TIMEOUT
 from .utils import transform_json_to_single_depth
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def encode_dict_values_to_utf8(dictionary):
+    encoded_dict = {}
+    for key, value in dictionary.items():
+        if isinstance(value, dict):
+            encoded_dict[key] = encode_dict_values_to_utf8(value)
+        elif isinstance(value, str):
+            encoded_dict[key] = value.encode("utf-8")
+        else:
+            encoded_dict[key] = value
+    return encoded_dict
+
+
+def validate_json(json_str):
+    """Validate json string."""
+    if type(json_str) is dict:
+        return True
+    try:
+        return json.loads(json_str)
+    except ValueError as error:
+        print(error)
+        return False
+
+
+class RobonectException(Exception):
+    """Raised when an update has failed."""
+
+
 class RobonectClient:
     """Class to communicate with the Robonect API."""
 
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
         self.auth = None
         self.host = host
@@ -42,48 +70,79 @@
             await self.session.close()
         self.session = None
 
     async def async_cmd(self, command=None, params={}) -> list[dict]:
         """Send command to mower."""
         if command is None:
             return False
-        params = urllib.parse.urlencode(params)
+        if params is None:
+            params = ""
+        else:
+            params = urllib.parse.urlencode(params)
+
         if command == "job":
             _LOGGER.debug(f"Job params: {params}")
             return
 
         self.session_start()
-        async with self.session.get(
-            f"http://{self.host}/json?cmd={command}&{params}"
-        ) as response:
-            if response.status == 200:
-                try:
-                    result = await response.json(content_type=None)
-                except Exception as e:
-                    _LOGGER.error(e)
-                    return False
-                _LOGGER.debug("Result mower data: %s", result)
-            if response.status >= 400:
-                await self.session_close()
-                response.raise_for_status()
-        if self.transform_json:
-            return transform_json_to_single_depth(result)
-        return result
+        try:
+            async with self.session.get(
+                f"http://{self.host}/json?cmd={command}&{params}"
+            ) as response:
+                if response.status == 200:
+                    result = await response.json(encoding="iso-8859-15")
+                    _LOGGER.debug("Result mower data: %s", result)
+                if response.status >= 400:
+                    await self.session_close()
+                    response.raise_for_status()
+            await self.session_close()
+            if self.transform_json:
+                return transform_json_to_single_depth(result)
+            return result
+        except Exception as exception:
+            await self.session_close()
+            raise exception
 
-    async def async_cmds(self, commands=None, bypass_sleeping=False) -> list[dict]:
+    async def async_cmds(self, commands=None, bypass_sleeping=False) -> dict:
         """Send command to mower."""
         self.session_start()
-        result = []
-        result.append({"status": await self.state()})
-        if not self.sleeping or bypass_sleeping:
-            for cmd in commands:
-                result.append({cmd: await self.async_cmd(cmd)})
-        await self.session_close()
+        result = await self.state()
+        if result:
+            result = {"status": result}
+            if not self.sleeping or bypass_sleeping:
+                for cmd in commands:
+                    result.update({cmd: await self.async_cmd(cmd)})
+            await self.session_close()
         return result
 
-    async def state(self) -> list[dict]:
+    async def state(self) -> dict:
         """Send status command to mower."""
         self.session_start()
         result = await self.async_cmd("status")
-        self.sleeping = result.get("status").get("status") == 17
-        await self.session_close()
+        if result:
+            self.sleeping = result.get("status").get("status") == 17
+            await self.session_close()
         return result
+
+    async def async_start(self) -> bool:
+        """Start the mower."""
+        return await self.async_cmd("start")
+
+    async def async_stop(self) -> bool:
+        """Stop the mower."""
+        return await self.async_cmd("stop")
+
+    async def async_reboot(self) -> bool:
+        """Reboot Robonect."""
+        return await self.async_cmd("service", {"service": "reboot"})
+
+    async def async_shutdown(self) -> bool:
+        """Shutdown Robonect."""
+        return await self.async_cmd("service", {"service": "shutdown"})
+
+    async def async_sleep(self) -> bool:
+        """Make Robonect sleep."""
+        return await self.async_cmd("service", {"service": "sleep"})
+
+    def sleeping(self) -> int:
+        """Return if the mower is sleeping."""
+        return self.sleeping
```

### Comparing `aiorobonect-0.1.9/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.2.0/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.1.9
+Version: 0.2.0
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.1.9/setup.py` & `aiorobonect-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.1.9",
+    version="v0.2.0",
 )
```


# Comparing `tmp/pysqueezebox-0.6.2.tar.gz` & `tmp/pysqueezebox-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqueezebox-0.6.2.tar", last modified: Thu May 25 21:48:54 2023, max compression
+gzip compressed data, was "pysqueezebox-0.6.3.tar", last modified: Fri May 26 12:14:14 2023, max compression
```

## Comparing `pysqueezebox-0.6.2.tar` & `pysqueezebox-0.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.016906 pysqueezebox-0.6.2/
--rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/LICENSE
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-25 21:48:54.017194 pysqueezebox-0.6.2/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/README.md
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.009246 pysqueezebox-0.6.2/pysqueezebox/
--rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/const.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    23556 2023-05-25 21:25:21.000000 pysqueezebox-0.6.2/pysqueezebox/player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    13353 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/server.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.011841 pysqueezebox-0.6.2/pysqueezebox.egg-info/
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/SOURCES.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/dependency_links.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/requires.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/top_level.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-25 21:48:54.018183 pysqueezebox-0.6.2/setup.cfg
--rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-25 21:47:05.000000 pysqueezebox-0.6.2/setup.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.016167 pysqueezebox-0.6.2/tests/
--rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.6.2/tests/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1520 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/conftest.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.6.2/tests/test_discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    18297 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_integration.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.191446 pysqueezebox-0.6.3/
+-rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/LICENSE
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 12:14:14.191630 pysqueezebox-0.6.3/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/README.md
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.184958 pysqueezebox-0.6.3/pysqueezebox/
+-rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/const.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    23569 2023-05-26 12:06:19.000000 pysqueezebox-0.6.3/pysqueezebox/player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    13353 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/pysqueezebox/server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.187531 pysqueezebox-0.6.3/pysqueezebox.egg-info/
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/SOURCES.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/dependency_links.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/requires.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/top_level.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-26 12:14:14.192225 pysqueezebox-0.6.3/setup.cfg
+-rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-26 12:13:38.000000 pysqueezebox-0.6.3/setup.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.190955 pysqueezebox-0.6.3/tests/
+-rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.6.3/tests/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1520 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/tests/conftest.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.6.3/tests/test_discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    18297 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/tests/test_integration.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/tests/test_player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/tests/test_server.py
```

### Comparing `pysqueezebox-0.6.2/LICENSE` & `pysqueezebox-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/PKG-INFO` & `pysqueezebox-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.2
+Version: 0.6.3
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.6.2/README.md` & `pysqueezebox-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/pysqueezebox/__init__.py` & `pysqueezebox-0.6.3/pysqueezebox/__init__.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/pysqueezebox/discovery.py` & `pysqueezebox-0.6.3/pysqueezebox/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/pysqueezebox/player.py` & `pysqueezebox-0.6.3/pysqueezebox/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,27 +365,27 @@
                 self._playlist_timestamp = response["playlist_timestamp"]
                 self._playlist_tags = set(tags)
                 # poll server again for full playlist, which has either changed
                 # or about which we are seeking new tags
                 response = await self.async_query(
                     "status", "0", response["playlist_tracks"], f"tags:{tags}"
                 )
+
+                if response is False:
+                    _LOGGER.debug("Error updating status - unable to retrieve playlist")
+                    return False
             else:
                 response.pop("playlist_loop", None)
         else:
             # no current playlist
             self._status.update({"playlist_loop": None})
 
         # preserve the playlist between updates
         self._status = {"playlist_loop": self._status.get("playlist_loop")}
-        try:
-            self._status.update(response)
-        except TypeError:
-            _LOGGER.debug("Error updating status - empty response from server")
-            return False
+        self._status.update(response)
 
         # check if any property futures have been satisfied
         property_futures = []
         interval = None
         for property_future in self._property_futures:
             if not property_future["future"].done():
                 if property_future["test"](getattr(self, property_future["prop"])):
```

### Comparing `pysqueezebox-0.6.2/pysqueezebox/server.py` & `pysqueezebox-0.6.3/pysqueezebox/server.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/pysqueezebox.egg-info/PKG-INFO` & `pysqueezebox-0.6.3/pysqueezebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.2
+Version: 0.6.3
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.6.2/setup.py` & `pysqueezebox-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysqueezebox",
-    version="0.6.2",
+    version="0.6.3",
     license="apache-2.0",
     author="Raj Laud",
     author_email="raj.laud@gmail.com",
     description="Asynchronous library to control Logitech Media Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rajlaud/pysqueezebox",
```

### Comparing `pysqueezebox-0.6.2/tests/conftest.py` & `pysqueezebox-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/tests/test_discovery.py` & `pysqueezebox-0.6.3/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/tests/test_integration.py` & `pysqueezebox-0.6.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/tests/test_player.py` & `pysqueezebox-0.6.3/tests/test_player.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.2/tests/test_server.py` & `pysqueezebox-0.6.3/tests/test_server.py`

 * *Files identical despite different names*


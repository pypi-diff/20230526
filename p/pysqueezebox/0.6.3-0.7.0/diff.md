# Comparing `tmp/pysqueezebox-0.6.3.tar.gz` & `tmp/pysqueezebox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqueezebox-0.6.3.tar", last modified: Fri May 26 12:14:14 2023, max compression
+gzip compressed data, was "pysqueezebox-0.7.0.tar", last modified: Fri May 26 18:37:32 2023, max compression
```

## Comparing `pysqueezebox-0.6.3.tar` & `pysqueezebox-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.191446 pysqueezebox-0.6.3/
--rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/LICENSE
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 12:14:14.191630 pysqueezebox-0.6.3/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/README.md
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.184958 pysqueezebox-0.6.3/pysqueezebox/
--rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/const.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/pysqueezebox/discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    23569 2023-05-26 12:06:19.000000 pysqueezebox-0.6.3/pysqueezebox/player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    13353 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/pysqueezebox/server.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.187531 pysqueezebox-0.6.3/pysqueezebox.egg-info/
--rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/SOURCES.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/dependency_links.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/requires.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-26 12:14:14.000000 pysqueezebox-0.6.3/pysqueezebox.egg-info/top_level.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-26 12:14:14.192225 pysqueezebox-0.6.3/setup.cfg
--rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-26 12:13:38.000000 pysqueezebox-0.6.3/setup.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 12:14:14.190955 pysqueezebox-0.6.3/tests/
--rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.6.3/tests/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1520 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/tests/conftest.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.6.3/tests/test_discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    18297 2023-05-26 11:37:04.000000 pysqueezebox-0.6.3/tests/test_integration.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/tests/test_player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.6.3/tests/test_server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.057189 pysqueezebox-0.7.0/
+-rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/LICENSE
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 18:37:32.057454 pysqueezebox-0.7.0/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/README.md
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.046707 pysqueezebox-0.7.0/pysqueezebox/
+-rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/const.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/pysqueezebox/discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    23556 2023-05-26 15:26:42.000000 pysqueezebox-0.7.0/pysqueezebox/player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    13244 2023-05-26 15:27:06.000000 pysqueezebox-0.7.0/pysqueezebox/server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.050874 pysqueezebox-0.7.0/pysqueezebox.egg-info/
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-26 18:37:32.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/SOURCES.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/dependency_links.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/requires.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-26 18:37:31.000000 pysqueezebox-0.7.0/pysqueezebox.egg-info/top_level.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-26 18:37:32.058441 pysqueezebox-0.7.0/setup.cfg
+-rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-26 18:34:14.000000 pysqueezebox-0.7.0/setup.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-26 18:37:32.056281 pysqueezebox-0.7.0/tests/
+-rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.7.0/tests/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1686 2023-05-26 18:32:29.000000 pysqueezebox-0.7.0/tests/conftest.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.7.0/tests/test_discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    18376 2023-05-26 18:32:50.000000 pysqueezebox-0.7.0/tests/test_integration.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/tests/test_player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.7.0/tests/test_server.py
```

### Comparing `pysqueezebox-0.6.3/LICENSE` & `pysqueezebox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/PKG-INFO` & `pysqueezebox-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.3
+Version: 0.7.0
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.6.3/README.md` & `pysqueezebox-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/pysqueezebox/__init__.py` & `pysqueezebox-0.7.0/pysqueezebox/__init__.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/pysqueezebox/discovery.py` & `pysqueezebox-0.7.0/pysqueezebox/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/pysqueezebox/player.py` & `pysqueezebox-0.7.0/pysqueezebox/player.py`

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
-
-                if response is False:
-                    _LOGGER.debug("Error updating status - unable to retrieve playlist")
-                    return False
             else:
                 response.pop("playlist_loop", None)
         else:
             # no current playlist
             self._status.update({"playlist_loop": None})
 
         # preserve the playlist between updates
         self._status = {"playlist_loop": self._status.get("playlist_loop")}
-        self._status.update(response)
+        try:
+            self._status.update(response)
+        except TypeError:
+            _LOGGER.debug("Error updating status - empty response from server")
+            return False
 
         # check if any property futures have been satisfied
         property_futures = []
         interval = None
         for property_future in self._property_futures:
             if not property_future["future"].done():
                 if property_future["test"](getattr(self, property_future["prop"])):
```

### Comparing `pysqueezebox-0.6.3/pysqueezebox/server.py` & `pysqueezebox-0.7.0/pysqueezebox/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         session,
         host,
         port=DEFAULT_PORT,
         username=None,
         password=None,
         uuid=None,
         name=None,
+        https=False,
     ):
         """
         Initialize the Logitech device.
 
         Parameters:
             session: aiohttp.ClientSession for connecting to server (required)
             host: LMS server to connect with (required)
@@ -46,14 +47,15 @@
             name: LMS server name (optional, only available through discovery)
         """
         self.host = host
         self.port = port
         self.session = session
         self._username = username
         self._password = password
+        self._prefix = "https" if https else "http"
 
         self.http_status = None
         self.uuid = uuid
         self.name = name  # often None, can only be found during discovery
 
         self.status = None
         self._browse_cache = {}  # key: category; value: (lastscan, limit, items)
@@ -63,15 +65,16 @@
         return (
             f"Server({self.session}, "
             f"{self.host}, "
             f"{self.port}, "
             f"{self._username}, "
             f"{self._password}, "
             f"{self.uuid}, "
-            f"{self.name})"
+            f"{self.name}, "
+            f"{self._prefix})"
         )
 
     async def async_get_players(self, search=None):
         """
         Return Player for each device connected to LMS.
 
         Parameters:
@@ -140,15 +143,15 @@
     async def async_query(self, *command, player=""):
         """Return result of query on the JSON-RPC connection."""
         auth = (
             None
             if self._username is None
             else aiohttp.BasicAuth(self._username, self._password)
         )
-        url = f"http://{self.host}:{self.port}/jsonrpc.js"
+        url = f"{self._prefix}://{self.host}:{self.port}/jsonrpc.js"
         data = json.dumps(
             {"id": "1", "method": "slim.request", "params": [player, command]}
         )
 
         _LOGGER.debug("URL: %s Data: %s", url, data)
 
         if self.session is None:
@@ -336,20 +339,14 @@
 
     def generate_image_url_from_track_id(self, track_id):
         """Generate an image url using a track id."""
         return self.generate_image_url(f"/music/{track_id}/cover.jpg")
 
     def generate_image_url(self, image_url):
         """Add the appropriate base_url to a relative image_url."""
+        base_url = f"{self._prefix}://"
         if self._username:
-            base_url = "http://{username}:{password}@{server}:{port}/".format(
-                username=self._username,
-                password=self._password,
-                server=self.host,
-                port=self.port,
-            )
-        else:
-            base_url = "http://{server}:{port}/".format(
-                server=self.host, port=self.port
-            )
+            base_url += f"{self._username}:{self._password}@"
+
+        base_url += f"{self.host}:{self.port}/"
 
         return urllib.parse.urljoin(base_url, image_url)
```

### Comparing `pysqueezebox-0.6.3/pysqueezebox.egg-info/PKG-INFO` & `pysqueezebox-0.7.0/pysqueezebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.3
+Version: 0.7.0
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pysqueezebox-0.6.3/setup.py` & `pysqueezebox-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysqueezebox",
-    version="0.6.3",
+    version="0.7.0",
     license="apache-2.0",
     author="Raj Laud",
     author_email="raj.laud@gmail.com",
     description="Asynchronous library to control Logitech Media Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rajlaud/pysqueezebox",
```

### Comparing `pysqueezebox-0.6.3/tests/conftest.py` & `pysqueezebox-0.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,34 +12,43 @@
     """
     loop = asyncio.get_event_loop()
     yield loop
     loop.close()
 
 
 def pytest_addoption(parser):
-    """Add the --ip and --port commandline options"""
+    """Add the commandline options"""
     parser.addoption(
-        "--ip",
+        "--host",
         type=str,
         default=None,
         action="store",
-        dest="IP",
-        help="the IP address for the squeezebox server to be used for the integration tests",
+        dest="HOST",
+        help="the host for the squeezebox server to be used for the integration tests",
     )
 
     parser.addoption(
         "--port",
         type=int,
         default=9000,
         action="store",
         dest="PORT",
         help="the port for the squeezebox server to be used for the integration tests",
     )
 
     parser.addoption(
+        "--https",
+        type=bool,
+        default=False,
+        action="store",
+        dest="HTTPS",
+        help="whether to use https to connect",
+    )
+
+    parser.addoption(
         "--prefer-player",
         type=str,
         default=None,
         action="append",
         dest="PREFER",
         help="prefer this player in tests",
     )
```

### Comparing `pysqueezebox-0.6.3/tests/test_discovery.py` & `pysqueezebox-0.7.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/tests/test_integration.py` & `pysqueezebox-0.7.0/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 REMOTE_STREAM = "https://stream.wbez.org/wbez128-tunein.mp3"
 
 
 @pytest.fixture(name="lms", scope="module")
 async def fixture_lms(request):
     """Return a working Server object."""
     # Get the ip address and port from the command line
-    ip = IP if IP else request.config.option.IP
+    ip = request.config.option.HOST if request.config.option.HOST else IP
     port = request.config.option.PORT
+    https = request.config.option.HTTPS
 
     if ip is None:
         pytest.fail("No ip address specified. Use the --ip option.")
 
     async with aiohttp.ClientSession() as session:
-        server = Server(session, ip, port)
+        server = Server(session, ip, port, https=https)
         # confirm server is working
         assert await server.async_status()
         yield server
 
 
 @pytest.fixture(name="players", scope="module")
 async def fixture_players(lms, request):
```

### Comparing `pysqueezebox-0.6.3/tests/test_player.py` & `pysqueezebox-0.7.0/tests/test_player.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.3/tests/test_server.py` & `pysqueezebox-0.7.0/tests/test_server.py`

 * *Files identical despite different names*


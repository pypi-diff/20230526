# Comparing `tmp/aiobtclientapi-1.1.0.tar.gz` & `tmp/aiobtclientapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobtclientapi-1.1.0.tar", last modified: Thu May 25 10:32:09 2023, max compression
+gzip compressed data, was "aiobtclientapi-1.1.1.tar", last modified: Fri May 26 15:23:33 2023, max compression
```

## Comparing `aiobtclientapi-1.1.0.tar` & `aiobtclientapi-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.984227 aiobtclientapi-1.1.0/
--rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.0/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.0/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi/
--rw-------   0 ich       (1000) ich       (1000)     1930 2023-05-25 10:12:34.000000 aiobtclientapi-1.1.0/aiobtclientapi/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3976 2023-05-14 09:04:17.000000 aiobtclientapi-1.1.0/aiobtclientapi/cli.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi/clients/
--rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/
--rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    18437 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/base/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/
--rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6016 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/
--rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5897 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/api.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/
--rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6595 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/api.py
--rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/utils.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/
--rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6480 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/api.py
--rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/enums.py
--rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.0/aiobtclientapi/constants.py
--rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/errors.py
--rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.0/aiobtclientapi/response.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.980227 aiobtclientapi-1.1.0/aiobtclientapi/utils/
--rw-------   0 ich       (1000) ich       (1000)     6024 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6674 2022-08-01 15:15:03.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/monitor.py
--rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/aiobtclientapi/utils/torrent.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-05-25 10:32:09.976227 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1021 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       57 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)       60 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       15 2023-05-25 10:32:09.000000 aiobtclientapi-1.1.0/aiobtclientapi.egg-info/top_level.txt
--rw-------   0 ich       (1000) ich       (1000)       38 2023-05-25 10:32:09.984227 aiobtclientapi-1.1.0/setup.cfg
--rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.0/setup.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.1/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)      592 2022-08-27 13:56:53.000000 aiobtclientapi-1.1.1/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.614157 aiobtclientapi-1.1.1/aiobtclientapi/
+-rw-------   0 ich       (1000) ich       (1000)     1930 2023-05-26 14:25:52.000000 aiobtclientapi-1.1.1/aiobtclientapi/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3976 2023-05-14 09:04:17.000000 aiobtclientapi-1.1.1/aiobtclientapi/cli.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/
+-rw-------   0 ich       (1000) ich       (1000)      208 2022-08-04 15:44:22.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/
+-rw-------   0 ich       (1000) ich       (1000)       25 2022-06-16 09:50:40.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    18437 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/base/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/
+-rw-------   0 ich       (1000) ich       (1000)       27 2022-07-26 09:47:43.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6016 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/
+-rw-------   0 ich       (1000) ich       (1000)       32 2022-07-27 09:37:07.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5830 2023-05-26 14:24:26.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/api.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/
+-rw-------   0 ich       (1000) ich       (1000)       29 2022-07-27 15:40:51.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6595 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/api.py
+-rw-------   0 ich       (1000) ich       (1000)     1558 2023-05-18 09:45:43.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/utils.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.622157 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/
+-rw-------   0 ich       (1000) ich       (1000)       33 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6480 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/api.py
+-rw-------   0 ich       (1000) ich       (1000)      418 2022-07-30 14:17:58.000000 aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/enums.py
+-rw-------   0 ich       (1000) ich       (1000)       69 2022-07-05 13:26:49.000000 aiobtclientapi-1.1.1/aiobtclientapi/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     5466 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/errors.py
+-rw-------   0 ich       (1000) ich       (1000)     7696 2022-08-05 11:03:47.000000 aiobtclientapi-1.1.1/aiobtclientapi/response.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/aiobtclientapi/utils/
+-rw-------   0 ich       (1000) ich       (1000)     6024 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6674 2022-08-01 15:15:03.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/monitor.py
+-rw-------   0 ich       (1000) ich       (1000)     2634 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/aiobtclientapi/utils/torrent.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-05-26 15:23:33.618157 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     1198 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1021 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       57 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)       60 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       15 2023-05-26 15:23:33.000000 aiobtclientapi-1.1.1/aiobtclientapi.egg-info/top_level.txt
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-05-26 15:23:33.626157 aiobtclientapi-1.1.1/setup.cfg
+-rw-------   0 ich       (1000) ich       (1000)     1384 2023-05-25 09:54:57.000000 aiobtclientapi-1.1.1/setup.py
```

### Comparing `aiobtclientapi-1.1.0/LICENSE` & `aiobtclientapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/PKG-INFO` & `aiobtclientapi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.1.0/README.rst` & `aiobtclientapi-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/__init__.py` & `aiobtclientapi-1.1.1/aiobtclientapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Asynchronous high-level communication with BitTorrent clients
 """
 
 __project_name__ = 'aiobtclientapi'
 __description__ = 'Asynchronous high-level communication with BitTorrent clients'
 __homepage__ = 'https://codeberg.org/plotski/aiobtclientapi'
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 __author__ = 'plotski'
 __author_email__ = 'plotski@example.org'
 
 # isort:skip_file
 
 from .clients import APIBase
 from .clients import DelugeAPI, QbittorrentAPI, RtorrentAPI, TransmissionAPI
```

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/cli.py` & `aiobtclientapi-1.1.1/aiobtclientapi/cli.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/base/api.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/base/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/deluge/api.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/deluge/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/qbittorrent/api.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/qbittorrent/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
                 r'not a valid torrent': errors.InvalidTorrentError(torrent),
             })
 
         else:
             if response == 'Fails.':
                 # qBittorrent doesn't report duplicate torrents, it just "Fails."
                 # with HTTP status "200 OK"
-                print(infohash, 'in', await self.get_infohashes())
                 if infohash in await self.get_infohashes():
                     yield ('already_added', infohash)
                     yield errors.TorrentAlreadyAdded(infohash, name=torrent)
                 else:
                     raise errors.InvalidTorrentError(torrent)
 
             else:
```

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/api.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/rtorrent/utils.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/rtorrent/utils.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/clients/transmission/api.py` & `aiobtclientapi-1.1.1/aiobtclientapi/clients/transmission/api.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/errors.py` & `aiobtclientapi-1.1.1/aiobtclientapi/errors.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/response.py` & `aiobtclientapi-1.1.1/aiobtclientapi/response.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/utils/__init__.py` & `aiobtclientapi-1.1.1/aiobtclientapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/utils/monitor.py` & `aiobtclientapi-1.1.1/aiobtclientapi/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi/utils/torrent.py` & `aiobtclientapi-1.1.1/aiobtclientapi/utils/torrent.py`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi.egg-info/PKG-INFO` & `aiobtclientapi-1.1.1/aiobtclientapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobtclientapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous high-level communication with BitTorrent clients
 Home-page: https://codeberg.org/plotski/aiobtclientapi
 Author: plotski
 Author-email: plotski@example.org
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `aiobtclientapi-1.1.0/aiobtclientapi.egg-info/SOURCES.txt` & `aiobtclientapi-1.1.1/aiobtclientapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobtclientapi-1.1.0/setup.py` & `aiobtclientapi-1.1.1/setup.py`

 * *Files identical despite different names*


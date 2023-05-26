# Comparing `tmp/acestream_search-1.6.1.tar.gz` & `tmp/acestream_search-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acestream_search-1.6.1.tar", last modified: Fri Feb 10 16:59:54 2023, max compression
+gzip compressed data, was "acestream_search-1.6.2.tar", last modified: Fri May 26 16:37:51 2023, max compression
```

## Comparing `acestream_search-1.6.1.tar` & `acestream_search-1.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:59:54.404366 acestream_search-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-10 16:59:41.000000 acestream_search-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-10 16:59:41.000000 acestream_search-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-10 16:59:54.404366 acestream_search-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-10 16:59:41.000000 acestream_search-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:59:54.404366 acestream_search-1.6.1/acestream_search/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-10 16:59:41.000000 acestream_search-1.6.1/acestream_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-10 16:59:54.404366 acestream_search-1.6.1/acestream_search/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-02-10 16:59:41.000000 acestream_search-1.6.1/acestream_search/acestream_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:59:54.404366 acestream_search-1.6.1/acestream_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-10 16:59:54.000000 acestream_search-1.6.1/acestream_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-10 16:59:54.404366 acestream_search-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-10 16:59:41.000000 acestream_search-1.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-02-10 16:59:41.000000 acestream_search-1.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:37:51.620071 acestream_search-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 16:37:40.000000 acestream_search-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 16:37:40.000000 acestream_search-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 16:37:51.620071 acestream_search-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-26 16:37:40.000000 acestream_search-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:37:51.624071 acestream_search-1.6.2/acestream_search/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 16:37:40.000000 acestream_search-1.6.2/acestream_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 16:37:51.624071 acestream_search-1.6.2/acestream_search/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10716 2023-05-26 16:37:40.000000 acestream_search-1.6.2/acestream_search/acestream_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:37:51.620071 acestream_search-1.6.2/acestream_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:37:51.000000 acestream_search-1.6.2/acestream_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-26 16:37:51.620071 acestream_search-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-26 16:37:40.000000 acestream_search-1.6.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-26 16:37:40.000000 acestream_search-1.6.2/versioneer.py
```

### Comparing `acestream_search-1.6.1/LICENSE` & `acestream_search-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acestream_search-1.6.1/PKG-INFO` & `acestream_search-1.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acestream_search
-Version: 1.6.1
+Version: 1.6.2
 Summary: Produces acestream m3u playlist, xml epg or json data.
 Home-page: https://github.com/vstavrinov/acestream_search
 Author: Vladimir Stavrinov
 Author-email: vstavrinov@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `acestream_search-1.6.1/acestream_search/acestream_search.py` & `acestream_search-1.6.2/acestream_search/acestream_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         stop = datetime.fromtimestamp(
             int(group['epg'][0]['stop'])).strftime('%Y%m%d%H%M%S')
         channel_id = str(group['items'][0]['channel_id'])
         channel = ET.Element('channel')
         channel.set('id', channel_id)
         display = ET.SubElement(channel, 'display-name')
         display.set('lang', 'ru')
-        display.text = group['name']
+        display.text = str(group['name'])
         if 'icon' in group:
             icon = ET.SubElement(channel, 'icon')
             icon.set('src', group['icon'])
         programme = ET.Element('programme')
         programme.set('start', start + ' +0300')
         programme.set('stop', stop + ' +0300')
         programme.set('channel', channel_id)
```

### Comparing `acestream_search-1.6.1/acestream_search.egg-info/PKG-INFO` & `acestream_search-1.6.2/acestream_search.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acestream-search
-Version: 1.6.1
+Version: 1.6.2
 Summary: Produces acestream m3u playlist, xml epg or json data.
 Home-page: https://github.com/vstavrinov/acestream_search
 Author: Vladimir Stavrinov
 Author-email: vstavrinov@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `acestream_search-1.6.1/setup.py` & `acestream_search-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `acestream_search-1.6.1/versioneer.py` & `acestream_search-1.6.2/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/apidevtools-3.3.2.tar.gz` & `tmp/apidevtools-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.3.2.tar", last modified: Wed May 24 23:22:58 2023, max compression
+gzip compressed data, was "apidevtools-3.3.3.tar", last modified: Fri May 26 17:49:22 2023, max compression
```

## Comparing `apidevtools-3.3.2.tar` & `apidevtools-3.3.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.765849 apidevtools-3.3.2/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3271 2023-05-24 23:22:58.764848 apidevtools-3.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.2/README.md
--rw-rw-rw-   0        0        0     1772 2023-05-24 23:20:35.000000 apidevtools-3.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 23:22:58.765849 apidevtools-3.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.651859 apidevtools-3.3.2/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.665055 apidevtools-3.3.2/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.2/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0     1179 2023-05-13 20:33:43.000000 apidevtools-3.3.2/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.692355 apidevtools-3.3.2/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.2/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.2/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.2/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.3.2/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.698800 apidevtools-3.3.2/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.2/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-05-24 23:21:34.000000 apidevtools-3.3.2/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.2/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.716057 apidevtools-3.3.2/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.747516 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.763881 apidevtools-3.3.2/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.2/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.2/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 23:22:58.676133 apidevtools-3.3.2/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3271 2023-05-24 23:22:58.000000 apidevtools-3.3.2/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1012 2023-05-24 23:22:58.000000 apidevtools-3.3.2/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 23:22:58.000000 apidevtools-3.3.2/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-24 23:22:58.000000 apidevtools-3.3.2/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.394604 apidevtools-3.3.3/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-05-26 17:49:22.393603 apidevtools-3.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.3/README.md
+-rw-rw-rw-   0        0        0     2155 2023-05-26 17:11:55.000000 apidevtools-3.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:49:22.394604 apidevtools-3.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.188561 apidevtools-3.3.3/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.203674 apidevtools-3.3.3/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.3/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0     1179 2023-05-13 20:33:43.000000 apidevtools-3.3.3/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.237056 apidevtools-3.3.3/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.3/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.3/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.3/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.3/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.244055 apidevtools-3.3.3/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.3/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     1986 2023-05-26 17:48:06.000000 apidevtools-3.3.3/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.3/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.265182 apidevtools-3.3.3/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.344648 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.389079 apidevtools-3.3.3/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.3/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.3/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:49:22.221907 apidevtools-3.3.3/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      245 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 17:49:22.000000 apidevtools-3.3.3/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.3.2/LICENSE.txt` & `apidevtools-3.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/PKG-INFO` & `apidevtools-3.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.2
+Version: 3.3.3
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -38,14 +38,25 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: orm
+Provides-Extra: redis
+Provides-Extra: sqlite
+Provides-Extra: mysql
+Provides-Extra: postgresql
+Provides-Extra: encryptor
+Provides-Extra: compressed
+Provides-Extra: hasher
+Provides-Extra: imgproc
+Provides-Extra: telegraph
+Provides-Extra: speedup
 License-File: LICENSE.txt
 
 ## Overview
 ## Documentation
 ## Installation
 ```
 pip install apidevtools
```

### Comparing `apidevtools-3.3.2/README.md` & `apidevtools-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/logman.py` & `apidevtools-3.3.3/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.3.3/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/media/imgproc.py` & `apidevtools-3.3.3/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/media/telegraph.py` & `apidevtools-3.3.3/src/apidevtools/media/telegraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import contextlib as _contextlib
 import aiohttp as _aiohttp
 import io
 
+import ujson as _json
+
 
 async def upload(file: io.BytesIO, mime: str = 'image/png') -> str | None:
     """
     Upload media to telegra.ph
     :param file:
     :param mime:
     :return:
     """
     data = _aiohttp.FormData(dict(name='file', value=file.read(), content_type=mime, filename=f"file.{mime.split('/')[1]}"))
     with _contextlib.suppress(_aiohttp.ClientError):
-        async with _aiohttp.ClientSession(connector=_aiohttp.TCPConnector(ssl=False)) as session:
+        async with _aiohttp.ClientSession(
+            connector=_aiohttp.TCPConnector(ssl=False),
+            json_serialize=_json.dumps
+        ) as session:
             async with session.post(url='https://telegra.ph/upload', data=data) as response:
                 sources = await response.json()
                 if not (isinstance(sources, dict) and sources.get('error')):
                     return f"https://telegra.ph{sources[-1]['src']}"
 
 
 async def download(url: str) -> bytes | None:
```

### Comparing `apidevtools-3.3.2/src/apidevtools/security/hasher.py` & `apidevtools-3.3.3/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.3.3/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools/utils.py` & `apidevtools-3.3.3/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.2/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.3.3/src/apidevtools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.2
+Version: 3.3.3
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -38,14 +38,25 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: orm
+Provides-Extra: redis
+Provides-Extra: sqlite
+Provides-Extra: mysql
+Provides-Extra: postgresql
+Provides-Extra: encryptor
+Provides-Extra: compressed
+Provides-Extra: hasher
+Provides-Extra: imgproc
+Provides-Extra: telegraph
+Provides-Extra: speedup
 License-File: LICENSE.txt
 
 ## Overview
 ## Documentation
 ## Installation
 ```
 pip install apidevtools
```

### Comparing `apidevtools-3.3.2/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.3.3/src/apidevtools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/__init__.py
 src/apidevtools/__init__.py
 src/apidevtools/logman.py
 src/apidevtools/utils.py
 src/apidevtools.egg-info/PKG-INFO
 src/apidevtools.egg-info/SOURCES.txt
 src/apidevtools.egg-info/dependency_links.txt
+src/apidevtools.egg-info/requires.txt
 src/apidevtools.egg-info/top_level.txt
 src/apidevtools/media/ARIALNB.TTF
 src/apidevtools/media/__init__.py
 src/apidevtools/media/imgproc.py
 src/apidevtools/media/telegraph.py
 src/apidevtools/security/__init__.py
 src/apidevtools/security/encryptor.py
```


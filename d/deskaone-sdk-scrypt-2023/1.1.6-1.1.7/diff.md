# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.6.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.6.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.7.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.6.tar` & `deskaone_sdk_scrypt_2023-1.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-05-22 14:31:50.221475 deskaone_sdk_scrypt_2023-1.1.6/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.6/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-22 14:31:55.838997 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.6/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0      775 2023-05-26 01:51:11.195238 deskaone_sdk_scrypt_2023-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.7/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-26 01:51:18.077237 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.7/setup.py
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.7/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.6"
+version = "1.1.7"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -19,12 +19,13 @@
 pysocks = "^1.7.1"
 flask = "^2.2.3"
 gunicorn = "^20.1.0"
 html5lib = "^1.1"
 bs4 = "^0.0.1"
 polling2 = "^0.5.0"
 polling = "^0.3.2"
+psycopg2 = "^2.9.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.7/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/setup.py` & `deskaone_sdk_scrypt_2023-1.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,24 +22,25 @@
  'colorama>=0.4.6,<0.5.0',
  'flask>=2.2.3,<3.0.0',
  'gunicorn>=20.1.0,<21.0.0',
  'html5lib>=1.1,<2.0',
  'install-jdk>=0.3.0,<0.4.0',
  'polling2>=0.5.0,<0.6.0',
  'polling>=0.3.2,<0.4.0',
+ 'psycopg2>=2.9.6,<3.0.0',
  'pycryptodome>=3.17,<4.0',
  'pysocks>=1.7.1,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.6',
+    'version': '1.1.7',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.6/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.6
+Version: 1.1.7
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: install-jdk (>=0.3.0,<0.4.0)
 Requires-Dist: polling (>=0.3.2,<0.4.0)
 Requires-Dist: polling2 (>=0.5.0,<0.6.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Requires-Dist: requests[socks] (>=2.28.2,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.29)
 Description-Content-Type: text/markdown
```


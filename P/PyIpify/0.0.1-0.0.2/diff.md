# Comparing `tmp/PyIpify-0.0.1.tar.gz` & `tmp/PyIpify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIpify-0.0.1.tar", last modified: Fri May 26 06:33:06 2023, max compression
+gzip compressed data, was "PyIpify-0.0.2.tar", last modified: Fri May 26 11:14:28 2023, max compression
```

## Comparing `PyIpify-0.0.1.tar` & `PyIpify-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.479036 PyIpify-0.0.1/
--rw-rw-rw-   0        0        0     1061 2023-05-26 06:33:06.479036 PyIpify-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.464523 PyIpify-0.0.1/PyIpify.egg-info/
--rw-rw-rw-   0        0        0     1061 2023-05-26 06:33:06.000000 PyIpify-0.0.1/PyIpify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2023-05-26 06:33:06.000000 PyIpify-0.0.1/PyIpify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:33:06.000000 PyIpify-0.0.1/PyIpify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-26 06:33:06.000000 PyIpify-0.0.1/PyIpify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 06:33:06.000000 PyIpify-0.0.1/PyIpify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-05-26 06:09:27.000000 PyIpify-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.464523 PyIpify-0.0.1/ipify/
--rw-rw-rw-   0        0        0       38 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/__init__.py
--rw-rw-rw-   0        0        0     1352 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.464523 PyIpify-0.0.1/ipify/__pycache__/
--rw-rw-rw-   0        0        0      164 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      184 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2174 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/__pycache__/__main__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.464523 PyIpify-0.0.1/ipify/asyncronous/
--rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.479036 PyIpify-0.0.1/ipify/asyncronous/__pycache__/
--rw-rw-rw-   0        0        0      201 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      247 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      522 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0     1294 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      523 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0     1295 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      234 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      229 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/asyncronous/find_ipv6.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.479036 PyIpify-0.0.1/ipify/syncronous/
--rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:33:06.479036 PyIpify-0.0.1/ipify/syncronous/__pycache__/
--rw-rw-rw-   0        0        0      200 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      246 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      373 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0      516 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      374 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0      517 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      169 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      178 2023-05-26 06:09:27.000000 PyIpify-0.0.1/ipify/syncronous/find_ipv6.py
--rw-rw-rw-   0        0        0    11549 2023-05-26 06:09:27.000000 PyIpify-0.0.1/license.md
--rw-rw-rw-   0        0        0      230 2023-05-26 06:09:27.000000 PyIpify-0.0.1/main.py
--rw-rw-rw-   0        0        0       28 2023-05-26 06:09:27.000000 PyIpify-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 06:33:06.479036 PyIpify-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1766 2023-05-26 06:32:22.000000 PyIpify-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.674994 PyIpify-0.0.2/
+-rw-rw-rw-   0        0        0     1061 2023-05-26 11:14:28.674994 PyIpify-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.532848 PyIpify-0.0.2/PyIpify/
+-rw-rw-rw-   0        0        0       38 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/__init__.py
+-rw-rw-rw-   0        0        0     1352 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.632495 PyIpify-0.0.2/PyIpify/asyncronous/
+-rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.659474 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/
+-rw-rw-rw-   0        0        0      201 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      247 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      522 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1294 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
+-rw-rw-rw-   0        0        0      523 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1295 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
+-rw-rw-rw-   0        0        0      234 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      230 2023-05-26 11:09:37.000000 PyIpify-0.0.2/PyIpify/asyncronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.659474 PyIpify-0.0.2/PyIpify/syncronous/
+-rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.674994 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/
+-rw-rw-rw-   0        0        0      200 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      246 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      373 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
+-rw-rw-rw-   0        0        0      516 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
+-rw-rw-rw-   0        0        0      374 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
+-rw-rw-rw-   0        0        0      517 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
+-rw-rw-rw-   0        0        0      169 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      179 2023-05-26 11:09:54.000000 PyIpify-0.0.2/PyIpify/syncronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.628628 PyIpify-0.0.2/PyIpify.egg-info/
+-rw-rw-rw-   0        0        0     1061 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-05-26 06:09:27.000000 PyIpify-0.0.2/README.md
+-rw-rw-rw-   0        0        0    11549 2023-05-26 06:09:27.000000 PyIpify-0.0.2/license.md
+-rw-rw-rw-   0        0        0      232 2023-05-26 11:10:17.000000 PyIpify-0.0.2/main.py
+-rw-rw-rw-   0        0        0       28 2023-05-26 06:09:27.000000 PyIpify-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 11:14:28.674994 PyIpify-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1772 2023-05-26 11:11:20.000000 PyIpify-0.0.2/setup.py
```

### Comparing `PyIpify-0.0.1/PKG-INFO` & `PyIpify-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIpify
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple python library to find the public ip address of the system.
 Home-page: https://github.com/SigireddyBalasai/ipify
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
 Author: SigireddyBalasai
 Author-email: sigireddybalasai@gmail.com
 License: MIT
 Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asyncronous,ipify syncronous
```

### Comparing `PyIpify-0.0.1/PyIpify.egg-info/PKG-INFO` & `PyIpify-0.0.2/PyIpify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIpify
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple python library to find the public ip address of the system.
 Home-page: https://github.com/SigireddyBalasai/ipify
 Download-URL: https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz
 Author: SigireddyBalasai
 Author-email: sigireddybalasai@gmail.com
 License: MIT
 Keywords: ipify,ip,ip address,ipify.org,ipify api,ipify python,ipify python library,ipify python api,ipify python library,ipify python api,ipify python package,ipify,ipify cli,ipify asyncronous,ipify syncronous
```

### Comparing `PyIpify-0.0.1/PyIpify.egg-info/SOURCES.txt` & `PyIpify-0.0.2/PyIpify.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 README.md
 license.md
 main.py
 requirements.txt
 setup.py
+PyIpify/__init__.py
+PyIpify/__main__.py
 PyIpify.egg-info/PKG-INFO
 PyIpify.egg-info/SOURCES.txt
 PyIpify.egg-info/dependency_links.txt
 PyIpify.egg-info/requires.txt
 PyIpify.egg-info/top_level.txt
-ipify/__init__.py
-ipify/__main__.py
-ipify/__pycache__/__init__.cpython-310.pyc
-ipify/__pycache__/__init__.cpython-311.pyc
-ipify/__pycache__/__main__.cpython-311.pyc
-ipify/asyncronous/__init__.py
-ipify/asyncronous/find_ipv4.py
-ipify/asyncronous/find_ipv6.py
-ipify/asyncronous/__pycache__/__init__.cpython-310.pyc
-ipify/asyncronous/__pycache__/__init__.cpython-311.pyc
-ipify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
-ipify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
-ipify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
-ipify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
-ipify/syncronous/__init__.py
-ipify/syncronous/find_ipv4.py
-ipify/syncronous/find_ipv6.py
-ipify/syncronous/__pycache__/__init__.cpython-310.pyc
-ipify/syncronous/__pycache__/__init__.cpython-311.pyc
-ipify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
-ipify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
-ipify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
-ipify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
+PyIpify/asyncronous/__init__.py
+PyIpify/asyncronous/find_ipv4.py
+PyIpify/asyncronous/find_ipv6.py
+PyIpify/asyncronous/__pycache__/__init__.cpython-310.pyc
+PyIpify/asyncronous/__pycache__/__init__.cpython-311.pyc
+PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
+PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
+PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
+PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
+PyIpify/syncronous/__init__.py
+PyIpify/syncronous/find_ipv4.py
+PyIpify/syncronous/find_ipv6.py
+PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
+PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
+PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
+PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
+PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
+PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
```

### Comparing `PyIpify-0.0.1/ipify/__main__.py` & `PyIpify-0.0.2/PyIpify/__main__.py`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc` & `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc` & `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc` & `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc` & `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv4.cpython-311.pyc` & `PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/ipify/syncronous/__pycache__/find_ipv6.cpython-311.pyc` & `PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/license.md` & `PyIpify-0.0.2/license.md`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.1/setup.py` & `PyIpify-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r") as f:
         requirements = [line.strip() for line in f]
         return requirements
 
 
 setup(
     name="PyIpify",
-    packages=['ipify', 'ipify.syncronous', 'ipify.asyncronous'],
-    version="0.0.1",
+    packages=['PyIpify', 'PyIpify.syncronous', 'PyIpify.asyncronous'],
+    version="0.0.2",
     setup_requires=['setuptools_scm'],
     license="MIT",
     description="A simple python library to find the public ip address of the system.",
     author="SigireddyBalasai",
     author_email="sigireddybalasai@gmail.com",
     url="https://github.com/SigireddyBalasai/ipify",
     download_url="https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz",
```


# Comparing `tmp/idun_guardian_client-1.1.4.tar.gz` & `tmp/idun_guardian_client-1.1b17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1.4.tar", last modified: Fri May 26 11:27:04 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1b17.tar", last modified: Fri May 26 09:10:06 2023, max compression
```

## Comparing `idun_guardian_client-1.1.4.tar` & `idun_guardian_client-1.1b17.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 11:27:04.828649 idun_guardian_client-1.1.4/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-05-26 11:27:04.828338 idun_guardian_client-1.1.4/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1.4/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      864 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-05-26 11:27:04.828702 idun_guardian_client-1.1.4/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 11:27:04.822939 idun_guardian_client-1.1.4/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 11:27:04.826258 idun_guardian_client-1.1.4/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     9408 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1591 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    12613 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20719 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    34157 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 11:27:04.827371 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-05-26 11:27:04.000000 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-05-26 11:27:04.000000 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-05-26 11:27:04.000000 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-05-26 11:27:04.000000 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-05-26 11:27:04.000000 idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 11:27:04.828007 idun_guardian_client-1.1.4/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1677 2023-05-26 11:26:35.000000 idun_guardian_client-1.1.4/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1.4/tests/test_utils.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.585058 idun_guardian_client-1.1b17/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-05-26 09:10:06.584856 idun_guardian_client-1.1b17/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 13:19:07.000000 idun_guardian_client-1.1b17/README.md
+-rw-r--r--   0 waddaben   (501) staff       (20)      870 2023-05-26 09:09:21.000000 idun_guardian_client-1.1b17/pyproject.toml
+-rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-05-26 09:10:06.585110 idun_guardian_client-1.1b17/setup.cfg
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.578138 idun_guardian_client-1.1b17/src/
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.582225 idun_guardian_client-1.1b17/src/idun_guardian_client/
+-rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/__init__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/__main__.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     9408 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/client.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1591 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/config.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    12613 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/debug_logs.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    20719 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_api.py
+-rw-r--r--   0 waddaben   (501) staff       (20)    34157 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_bluetooth.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-14 11:38:29.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/mock_utils.py
+-rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/setup.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/src/idun_guardian_client/test_producer_consumer.py
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.583798 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/
+-rw-r--r--   0 waddaben   (501) staff       (20)     8992 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/requires.txt
+-rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-05-26 09:10:06.000000 idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/top_level.txt
+drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-05-26 09:10:06.584559 idun_guardian_client-1.1b17/tests/
+-rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/tests/test_ble.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1677 2023-05-26 09:04:35.000000 idun_guardian_client-1.1b17/tests/test_ble_record.py
+-rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b17/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1.4/PKG-INFO` & `idun_guardian_client-1.1b17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun_guardian_client
-Version: 1.1.4
+Version: 1.1b17
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.4/README.md` & `idun_guardian_client-1.1b17/README.md`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/pyproject.toml` & `idun_guardian_client-1.1b17/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idun_guardian_client"
-version = "1.1.4"
+version = "1.1.beta.17"
 authors = [
   { name="IDUN Technologies", email="contact@iduntechnologies.com" },
 ]
 description = "Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/client.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/config.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/debug_logs.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_api.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/igeb_utils.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b17/src/idun_guardian_client/test_producer_consumer.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idun-guardian-client
-Version: 1.1.4
+Version: 1.1b17
 Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
 Author-email: IDUN Technologies <contact@iduntechnologies.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `idun_guardian_client-1.1.4/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1b17/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/tests/test_ble.py` & `idun_guardian_client-1.1b17/tests/test_ble.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/tests/test_ble_record.py` & `idun_guardian_client-1.1b17/tests/test_ble_record.py`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1.4/tests/test_utils.py` & `idun_guardian_client-1.1b17/tests/test_utils.py`

 * *Files identical despite different names*


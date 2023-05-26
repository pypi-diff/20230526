# Comparing `tmp/tarn-0.5.0.tar.gz` & `tmp/tarn-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.5.0.tar", last modified: Wed May 17 14:00:49 2023, max compression
+gzip compressed data, was "tarn-0.5.1.tar", last modified: Fri May 26 11:27:46 2023, max compression
```

## Comparing `tarn-0.5.0.tar` & `tarn-0.5.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.308767 tarn-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-17 14:00:44.000000 tarn-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 14:00:44.000000 tarn-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-17 14:00:49.308767 tarn-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-17 14:00:44.000000 tarn-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-17 14:00:44.000000 tarn-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 14:00:44.000000 tarn-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:00:49.312767 tarn-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-17 14:00:44.000000 tarn-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.300767 tarn-0.5.0/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.304767 tarn-0.5.0/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.304767 tarn-0.5.0/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.304767 tarn-0.5.0/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.308767 tarn-0.5.0/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.308767 tarn-0.5.0/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.308767 tarn-0.5.0/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.308767 tarn-0.5.0/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-17 14:00:44.000000 tarn-0.5.0/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:00:49.304767 tarn-0.5.0/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-17 14:00:49.000000 tarn-0.5.0/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-17 14:00:49.000000 tarn-0.5.0/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:00:49.000000 tarn-0.5.0/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 14:00:49.000000 tarn-0.5.0/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 14:00:49.000000 tarn-0.5.0/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-26 11:27:43.000000 tarn-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 11:27:43.000000 tarn-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 11:27:46.196085 tarn-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 11:27:43.000000 tarn-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-26 11:27:43.000000 tarn-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:27:43.000000 tarn-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:27:46.196085 tarn-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-26 11:27:43.000000 tarn-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.192085 tarn-0.5.1/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.196085 tarn-0.5.1/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-26 11:27:43.000000 tarn-0.5.1/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:27:46.188084 tarn-0.5.1/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 11:27:46.000000 tarn-0.5.1/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.5.0/LICENSE` & `tarn-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/PKG-INFO` & `tarn-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.5.0
+Version: 0.5.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.5.0/README.md` & `tarn-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/pyproject.toml` & `tarn-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/setup.py` & `tarn-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/cache/storage.py` & `tarn-0.5.1/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/compat.py` & `tarn-0.5.1/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/config.py` & `tarn-0.5.1/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/digest.py` & `tarn-0.5.1/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/interface.py` & `tarn-0.5.1/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/local/storage.py` & `tarn-0.5.1/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/location/disk_dict.py` & `tarn-0.5.1/tarn/location/disk_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 import os
+import random
 import shutil
+import string
 from contextlib import contextmanager
 from pathlib import Path
 from typing import ContextManager, Iterable, Optional, Tuple
 
 from ..compat import copy_file, remove_file, rmtree
 from ..config import load_config, root_params
 from ..digest import key_to_relative
@@ -25,14 +27,17 @@
         config = load_config(root)
         self.levels = config.levels
         self.hash = config.hash.build()
         assert self.hash().digest_size == sum(self.levels)
 
         self.root = root
         self.permissions, self.group = root_params(self.root)
+        self.tmp = root / '.tmp'
+        create_folders(self.tmp, self.permissions, self.group)
+
         # TODO: create these folders only if needed
         usage_folder = self.root / 'tools/usage'
         labels_folder = self.root / 'tools/labels'
         create_folders(usage_folder, self.permissions, self.group)
         create_folders(labels_folder, self.permissions, self.group)
 
         self.locker: Locker = config.make_locker()
@@ -91,40 +96,40 @@
                     return
 
                 # make sure we can write
                 if not self._writeable():
                     yield
                     return
 
+                tmp = self.tmp / (key.hex() + ''.join(random.choices(string.ascii_lowercase, k=8)))
                 try:
                     # create base folders
                     create_folders(file.parent, self.permissions, self.group)
-                    # populate the folder
-                    # TODO: make this an atomic operation
-                    #  now this is just an ugly crutch
-                    try:
-                        if _is_pathlike(value):
-                            copy_file(value, file)
-                        else:
-                            with open(file, 'wb') as dst:
-                                shutil.copyfileobj(value, dst)
-
-                    except PermissionError:
-                        if not file.exists():
-                            raise
-                        _match(value, file, key)
 
+                    # write to a temp location
+                    if _is_pathlike(value):
+                        copy_file(value, tmp)
                     else:
-                        adjust_permissions(file, self.permissions, self.group, read_only=True)
+                        with open(tmp, 'wb') as dst:
+                            shutil.copyfileobj(value, dst)
+                    # permissions
+                    adjust_permissions(tmp, self.permissions, self.group, read_only=True)
+
+                    # move the file to the right location
+                    shutil.move(tmp, file)
 
                 except BaseException as e:
                     if file.exists():
                         remove_file(file)
                     raise RuntimeError('An error occurred while copying the file') from e
 
+                finally:
+                    if tmp.exists():
+                        remove_file(tmp)
+
                 # metadata
                 self.size_tracker.inc(get_size(file))
                 self.usage_tracker.update(key)
                 self.labels.update(key, labels)
 
                 yield file
```

### Comparing `tarn-0.5.0/tarn/location/fanout.py` & `tarn-0.5.1/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/location/interface.py` & `tarn-0.5.1/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/location/levels.py` & `tarn-0.5.1/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/location/nginx.py` & `tarn-0.5.1/tarn/location/nginx.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,16 +36,24 @@
 
     @contextmanager
     def _read_single(self, key: Key) -> ContextManager[MaybeValue]:
         if self.levels is None:
             yield None
             return
 
-        with requests.get(urljoin(self.url, str(key_to_relative(key, self.levels))), stream=True) as request:
+        relative = key_to_relative(key, self.levels)
+        with requests.get(urljoin(self.url, str(relative)), stream=True) as request:
             if not request.ok:
+                # TODO: this is probably an old format directory
+                with requests.get(urljoin(self.url, str(relative / 'data')), stream=True) as req:
+                    if req.ok:
+                        with req.raw as raw:
+                            yield raw
+                            return
+
                 yield None
                 return
 
             with request.raw as raw:
                 yield raw
 
     def _get_config(self):
```

### Comparing `tarn-0.5.0/tarn/location/scp.py` & `tarn-0.5.1/tarn/location/scp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import socket
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
-from typing import ContextManager, Iterable, Sequence, Tuple, Union
+from typing import Any, ContextManager, Iterable, Sequence, Tuple, Union
 
 import paramiko
 from paramiko import AuthenticationException, SSHClient, SSHException
 from paramiko.config import SSH_PORT, SSHConfig
 from paramiko.ssh_exception import NoValidConnectionsError
 from scp import SCPClient, SCPException
 
@@ -44,14 +44,17 @@
                 key = host.get('identityfile', key)
 
         self.hostname, self.port, self.username, self.password, self.key = hostname, port, username, password, key
         self.root = Path(root)
         self.ssh = ssh
         self.levels = self.hash = None
 
+    def __reduce__(self):
+        return self.__class__, (self.hostname, self.root, self.port, self.username, self.password, self.key)
+
     @property
     def key_size(self):
         return sum(self.levels) if self.levels is not None else None
 
     @contextmanager
     def read(self, key: Key) -> ContextManager[MaybeValue]:
         with self._connect() as scp:
```

### Comparing `tarn-0.5.0/tarn/pickler/compat.py` & `tarn-0.5.1/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/pickler/interface.py` & `tarn-0.5.1/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/pool/hash_key.py` & `tarn-0.5.1/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/pool/pickle_key.py` & `tarn-0.5.1/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/serializers.py` & `tarn-0.5.1/tarn/serializers.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/tools/labels.py` & `tarn-0.5.1/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/tools/locker.py` & `tarn-0.5.1/tarn/tools/locker.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,19 +53,20 @@
         finally:
             self._lock.release()
 
     write = read
 
 
 class RedisLocker(Locker):
-    def __init__(self, *args, prefix: AnyStr, expire: int):
+    def __init__(self, *args, prefix: AnyStr, expire: int, **kwargs):
         if len(args) == 1 and isinstance(args[0], Redis):
+            assert not kwargs, kwargs
             redis, = args
         else:
-            redis = Redis(*args)
+            redis = Redis(*args, **kwargs)
         if isinstance(prefix, str):
             prefix = prefix.encode()
 
         self._redis = redis
         self._prefix = prefix + b':'
         self._expire = expire
         self._volume_key = prefix + b'.V'
@@ -80,42 +81,41 @@
         sleep_time = 0.1
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_reading, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
-            success = self._safe_eval(self._stop_reading_script, 1, self._prefix + key)
-        if not success:
-            raise RuntimeError('The locker is in a wrong state. Did it expire?')
+            lock = self._safe_eval(self._stop_reading_script, 1, self._prefix + key)
+        if lock != b'1':
+            raise RuntimeError(f'The locker is in a wrong state ({lock}). Did it expire?')
 
     @contextmanager
     def write(self, key: Key) -> ContextManager[None]:
         sleep_time = 0.1
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_writing, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
-            success = self._safe_eval(self._stop_writing_script, 1, self._prefix + key)
-        if not success:
-            raise RuntimeError('The locker is in a wrong state. Did it expire?')
+            lock = self._safe_eval(self._stop_writing_script, 1, self._prefix + key)
+        if lock != b'-1':
+            raise RuntimeError(f'The locker is in a wrong state ({lock}). Did it expire?')
 
     def _update_scripts(self):
         expire = self._expire
         # TODO: how slow are these checks?
         # language=Lua
         self._stop_writing_script = self._redis.script_load('''
-        if redis.call('get', KEYS[1]) == '-1' then
+        local lock = redis.call('get', KEYS[1])
+        if lock == '-1' then
             redis.call('del', KEYS[1])
-            return 1
-        else
-            return 0
-        end''')
+        end
+        return lock''')
         # language=Lua
         self._start_reading_script = self._redis.script_load(f'''
         local lock = redis.call('get', KEYS[1])
         if lock == '-1' then
             return 0
         elseif lock == false then
             redis.call('set', KEYS[1], 1, 'EX', {expire})
@@ -124,23 +124,23 @@
             redis.call('set', KEYS[1], lock + 1, 'EX', {expire})
             return 1
         end''')
         # language=Lua
         self._stop_reading_script = self._redis.script_load(f'''
         local lock = redis.call('get', KEYS[1])
         if lock == false then 
-            return 0
+            return lock
         elseif lock == '1' then
             redis.call('del', KEYS[1])
-            return 1
+            return lock
         elseif tonumber(lock) < 1 then
-            return 0
+            return lock
         else
             redis.call('set', KEYS[1], lock - 1, 'EX', {expire})
-            return 1
+            return '1'
         end''')
 
     def _safe_eval(self, *args):
         try:
             return self._redis.evalsha(*args)
         except NoScriptError:
             pass
@@ -150,14 +150,21 @@
 
     def _start_writing(self, key: Key) -> bool:
         return bool(self._redis.set(self._prefix + key, -1, nx=True, ex=self._expire))
 
     def _start_reading(self, key: Key) -> bool:
         return bool(self._safe_eval(self._start_reading_script, 1, self._prefix + key))
 
+    @classmethod
+    def _from_args(cls, prefix, expire, kwargs):
+        return cls(prefix=prefix, expire=expire, **kwargs)
+
+    def __reduce__(self):
+        return self._from_args, (self._prefix[:-1], self._expire, self._redis.get_connection_kwargs())
+
 
 def wait_for_true(func, key, sleep_time, max_iterations):
     i = 0
     while not func(key):
         if i >= max_iterations:
             logger.error('Potential deadlock detected for %s', key)
             raise PotentialDeadLock(f"It seems like you've hit a deadlock for key {key}.")
```

### Comparing `tarn-0.5.0/tarn/tools/size.py` & `tarn-0.5.1/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/tools/usage.py` & `tarn-0.5.1/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn/utils.py` & `tarn-0.5.1/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.5.0/tarn.egg-info/PKG-INFO` & `tarn-0.5.1/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.5.0
+Version: 0.5.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.5.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.5.0/tarn.egg-info/SOURCES.txt` & `tarn-0.5.1/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*


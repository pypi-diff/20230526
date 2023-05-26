# Comparing `tmp/resoto-plugin-cleanup-expired-3.4.2.tar.gz` & `tmp/resoto-plugin-cleanup-expired-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-expired-3.4.2.tar", last modified: Wed May 10 12:21:11 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-expired-3.5.0.tar", last modified: Fri May 26 18:23:22 2023, max compression
```

## Comparing `resoto-plugin-cleanup-expired-3.4.2.tar` & `resoto-plugin-cleanup-expired-3.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 12:21:11.000000 resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:11.063937 resoto-plugin-cleanup-expired-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-10 12:19:31.000000 resoto-plugin-cleanup-expired-3.4.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:21.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 18:23:22.000000 resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:22.011146 resoto-plugin-cleanup-expired-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-26 18:21:42.000000 resoto-plugin-cleanup-expired-3.5.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-expired-3.4.2/PKG-INFO` & `resoto-plugin-cleanup-expired-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto Expired Resource Cleanup Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.4.2/README.md` & `resoto-plugin-cleanup-expired-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired/__init__.py` & `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/PKG-INFO` & `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-expired
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto Expired Resource Cleanup Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_expired
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-expired-3.4.2/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-expired-3.5.0/resoto_plugin_cleanup_expired.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-expired-3.4.2/setup.py` & `resoto-plugin-cleanup-expired-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-expired",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto Expired Resource Cleanup Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["cleanup_expired = resoto_plugin_cleanup_expired:CleanupExpiredPlugin"]},
     include_package_data=True,
```


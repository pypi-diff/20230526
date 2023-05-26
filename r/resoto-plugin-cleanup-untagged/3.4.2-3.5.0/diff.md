# Comparing `tmp/resoto-plugin-cleanup-untagged-3.4.2.tar.gz` & `tmp/resoto-plugin-cleanup-untagged-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-untagged-3.4.2.tar", last modified: Wed May 10 12:21:42 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-untagged-3.5.0.tar", last modified: Fri May 26 18:23:52 2023, max compression
```

## Comparing `resoto-plugin-cleanup-untagged-3.4.2.tar` & `resoto-plugin-cleanup-untagged-3.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 12:21:42.000000 resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:42.566348 resoto-plugin-cleanup-untagged-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-10 12:19:33.000000 resoto-plugin-cleanup-untagged-3.4.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:52.016915 resoto-plugin-cleanup-untagged-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-26 18:23:52.016915 resoto-plugin-cleanup-untagged-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:52.012915 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:52.016915 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 18:23:52.000000 resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:52.016915 resoto-plugin-cleanup-untagged-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:52.016915 resoto-plugin-cleanup-untagged-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-26 18:21:40.000000 resoto-plugin-cleanup-untagged-3.5.0/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto Cleanup Untagged Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/README.md` & `resoto-plugin-cleanup-untagged-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged/__init__.py` & `resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged/config.py` & `resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO` & `resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-untagged
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto Cleanup Untagged Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/cleanup_untagged
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-untagged-3.5.0/resoto_plugin_cleanup_untagged.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/setup.py` & `resoto-plugin-cleanup-untagged-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-cleanup-untagged",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto Cleanup Untagged Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["cleanup_untagged = resoto_plugin_cleanup_untagged:CleanupUntaggedPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-cleanup-untagged-3.4.2/test/test_config.py` & `resoto-plugin-cleanup-untagged-3.5.0/test/test_config.py`

 * *Files identical despite different names*


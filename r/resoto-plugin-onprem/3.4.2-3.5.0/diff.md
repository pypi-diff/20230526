# Comparing `tmp/resoto-plugin-onprem-3.4.2.tar.gz` & `tmp/resoto-plugin-onprem-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onprem-3.4.2.tar", last modified: Wed May 10 12:24:46 2023, max compression
+gzip compressed data, was "resoto-plugin-onprem-3.5.0.tar", last modified: Fri May 26 18:26:37 2023, max compression
```

## Comparing `resoto-plugin-onprem-3.4.2.tar` & `resoto-plugin-onprem-3.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 12:24:45.000000 resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:45.994246 resoto-plugin-onprem-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-10 12:22:27.000000 resoto-plugin-onprem-3.4.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 18:26:37.000000 resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:26:37.762365 resoto-plugin-onprem-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:26:37.758365 resoto-plugin-onprem-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-26 18:24:44.000000 resoto-plugin-onprem-3.5.0/test/test_config.py
```

### Comparing `resoto-plugin-onprem-3.4.2/PKG-INFO` & `resoto-plugin-onprem-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto On-Premises Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onprem
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/__init__.py` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/config.py` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/resources.py` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem/ssh.py` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/PKG-INFO` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto On-Premises Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/onprem
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.4.2/resoto_plugin_onprem.egg-info/SOURCES.txt` & `resoto-plugin-onprem-3.5.0/resoto_plugin_onprem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.4.2/setup.py` & `resoto-plugin-onprem-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-onprem",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto On-Premises Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["onprem = resoto_plugin_onprem:OnpremCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-onprem-3.4.2/test/test_config.py` & `resoto-plugin-onprem-3.5.0/test/test_config.py`

 * *Files identical despite different names*


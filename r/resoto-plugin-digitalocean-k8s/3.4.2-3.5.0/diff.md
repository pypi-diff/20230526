# Comparing `tmp/resoto-plugin-digitalocean-k8s-3.4.2.tar.gz` & `tmp/resoto-plugin-digitalocean-k8s-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.4.2.tar", last modified: Wed May 10 12:22:15 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.0.tar", last modified: Fri May 26 18:23:45 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-k8s-3.4.2.tar` & `resoto-plugin-digitalocean-k8s-3.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:15.732103 resoto-plugin-digitalocean-k8s-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 12:22:15.732103 resoto-plugin-digitalocean-k8s-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:15.728103 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:15.728103 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 12:22:15.000000 resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:22:15.732103 resoto-plugin-digitalocean-k8s-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:15.732103 resoto-plugin-digitalocean-k8s-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 12:19:38.000000 resoto-plugin-digitalocean-k8s-3.4.2/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.664591 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 18:23:45.000000 resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:45.668591 resoto-plugin-digitalocean-k8s-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-k8s-3.5.0/test/test_collector.py
```

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s/__init__.py` & `resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-k8s-3.5.0/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/setup.py` & `resoto-plugin-digitalocean-k8s-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-digitalocean-k8s",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto DigitalOcean-K8s Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": ["digitalocean_k8s_collector = resoto_plugin_digitalocean_k8s:DigitalOceanK8sCollectorPlugin"]
```

### Comparing `resoto-plugin-digitalocean-k8s-3.4.2/test/test_collector.py` & `resoto-plugin-digitalocean-k8s-3.5.0/test/test_collector.py`

 * *Files identical despite different names*


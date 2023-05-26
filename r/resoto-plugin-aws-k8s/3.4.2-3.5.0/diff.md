# Comparing `tmp/resoto-plugin-aws-k8s-3.4.2.tar.gz` & `tmp/resoto-plugin-aws-k8s-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-k8s-3.4.2.tar", last modified: Wed May 10 12:22:02 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-k8s-3.5.0.tar", last modified: Fri May 26 18:24:18 2023, max compression
```

## Comparing `resoto-plugin-aws-k8s-3.4.2.tar` & `resoto-plugin-aws-k8s-3.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 12:22:02.000000 resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:02.174882 resoto-plugin-aws-k8s-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 12:19:39.000000 resoto-plugin-aws-k8s-3.4.2/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.441372 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.441372 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 18:24:18.000000 resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:18.445371 resoto-plugin-aws-k8s-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 18:21:41.000000 resoto-plugin-aws-k8s-3.5.0/test/test_collector.py
```

### Comparing `resoto-plugin-aws-k8s-3.4.2/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto AWS-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s/__init__.py` & `resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-k8s-3.4.2/resoto_plugin_aws_k8s.egg-info/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.0/resoto_plugin_aws_k8s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto AWS-K8s Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-aws-k8s-3.4.2/setup.py` & `resoto-plugin-aws-k8s-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-aws-k8s",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto AWS-K8s Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["aws_k8s_collector = resoto_plugin_aws_k8s:AWSK8sCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-aws-k8s-3.4.2/test/test_collector.py` & `resoto-plugin-aws-k8s-3.5.0/test/test_collector.py`

 * *Files identical despite different names*


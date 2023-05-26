# Comparing `tmp/cdk8s-plus-24-2.8.1.tar.gz` & `tmp/cdk8s-plus-24-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-24-2.8.1.tar", last modified: Thu May 25 02:26:51 2023, max compression
+gzip compressed data, was "cdk8s-plus-24-2.8.2.tar", last modified: Fri May 26 02:27:10 2023, max compression
```

## Comparing `cdk8s-plus-24-2.8.1.tar` & `cdk8s-plus-24-2.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.826203 cdk8s-plus-24-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 02:26:51.826203 cdk8s-plus-24-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 02:26:51.826203 cdk8s-plus-24-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.818203 cdk8s-plus-24-2.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.822203 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/
--rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.822203 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1279933 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.822203 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:26:40.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:26:51.822203 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 02:26:51.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 02:26:51.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:26:51.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-25 02:26:51.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 02:26:51.000000 cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.656157 cdk8s-plus-24-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-26 02:27:10.656157 cdk8s-plus-24-2.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:27:10.656157 cdk8s-plus-24-2.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.644157 cdk8s-plus-24-2.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.648157 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161790 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.652157 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1279935 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/_jsii/cdk8s-plus-24@2.8.2.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.652157 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2878966 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:26:56.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:27:10.652157 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-26 02:27:10.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-26 02:27:10.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:27:10.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 02:27:10.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 02:27:10.000000 cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-24-2.8.1/LICENSE` & `cdk8s-plus-24-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.1/PKG-INFO` & `cdk8s-plus-24-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.1
+Version: 2.8.2
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-24-2.8.1/README.md` & `cdk8s-plus-24-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.1/setup.py` & `cdk8s-plus-24-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-24",
-    "version": "2.8.1",
+    "version": "2.8.2",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,24 +23,24 @@
     "packages": [
         "cdk8s_plus_24",
         "cdk8s_plus_24._jsii",
         "cdk8s_plus_24.k8s"
     ],
     "package_data": {
         "cdk8s_plus_24._jsii": [
-            "cdk8s-plus-24@2.8.1.jsii.tgz"
+            "cdk8s-plus-24@2.8.2.jsii.tgz"
         ],
         "cdk8s_plus_24": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s>=2.7.75, <3.0.0",
-        "constructs>=10.2.32, <11.0.0",
+        "constructs>=10.2.33, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/__init__.py` & `cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.1/src/cdk8s_plus_24/k8s/__init__.py` & `cdk8s-plus-24-2.8.2/src/cdk8s_plus_24/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-24-2.8.1/src/cdk8s_plus_24.egg-info/PKG-INFO` & `cdk8s-plus-24-2.8.2/src/cdk8s_plus_24.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-24
-Version: 2.8.1
+Version: 2.8.2
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-24 synthesizes Kubernetes manifests for Kubernetes 1.24.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


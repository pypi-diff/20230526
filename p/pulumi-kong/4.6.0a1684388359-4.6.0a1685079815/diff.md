# Comparing `tmp/pulumi_kong-4.6.0a1684388359.tar.gz` & `tmp/pulumi_kong-4.6.0a1685079815.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kong-4.6.0a1684388359.tar", last modified: Thu May 18 05:47:48 2023, max compression
+gzip compressed data, was "pulumi_kong-4.6.0a1685079815.tar", last modified: Fri May 26 06:05:51 2023, max compression
```

## Comparing `pulumi_kong-4.6.0a1684388359.tar` & `pulumi_kong-4.6.0a1685079815.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/pulumi_kong/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/pulumi_kong/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_key_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14562 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54615 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/target.py
--rw-r--r--   0 runner    (1001) docker     (123)    73091 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong/upstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 05:47:48.000000 pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 05:47:48.214657 pulumi_kong-4.6.0a1684388359/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-18 05:47:47.000000 pulumi_kong-4.6.0a1684388359/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/pulumi_kong/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/pulumi_kong/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_key_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14562 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54615 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73091 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong/upstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:05:51.769602 pulumi_kong-4.6.0a1685079815/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-26 06:05:51.000000 pulumi_kong-4.6.0a1685079815/setup.py
```

### Comparing `pulumi_kong-4.6.0a1684388359/PKG-INFO` & `pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_kong
-Version: 4.6.0a1684388359
+Name: pulumi-kong
+Version: 4.6.0a1685079815
 Summary: A Pulumi package for creating and managing Kong resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi kong
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1684388359/README.md` & `pulumi_kong-4.6.0a1685079815/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/__init__.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/_inputs.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/_utilities.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/certificate.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/config/vars.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_acl.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_basic_auth.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_jwt_auth.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_key_auth.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_key_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/consumer_oauth2.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/consumer_oauth2.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/outputs.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/plugin.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/provider.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/route.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/service.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/target.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/target.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong/upstream.py` & `pulumi_kong-4.6.0a1685079815/pulumi_kong/upstream.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/PKG-INFO` & `pulumi_kong-4.6.0a1685079815/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-kong
-Version: 4.6.0a1684388359
+Name: pulumi_kong
+Version: 4.6.0a1685079815
 Summary: A Pulumi package for creating and managing Kong resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi kong
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1684388359/pulumi_kong.egg-info/SOURCES.txt` & `pulumi_kong-4.6.0a1685079815/pulumi_kong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1684388359/setup.py` & `pulumi_kong-4.6.0a1685079815/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.6.0a1684388359"
-PLUGIN_VERSION = "4.6.0-alpha.1684388359+1895b42a"
+VERSION = "4.6.0a1685079815"
+PLUGIN_VERSION = "4.6.0-alpha.1685079815+299437e7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'kong', PLUGIN_VERSION])
         except OSError as error:
```

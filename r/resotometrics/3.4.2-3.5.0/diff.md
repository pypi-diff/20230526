# Comparing `tmp/resotometrics-3.4.2.tar.gz` & `tmp/resotometrics-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.4.2.tar", last modified: Wed May 10 12:24:37 2023, max compression
+gzip compressed data, was "resotometrics-3.5.0.tar", last modified: Fri May 26 18:23:55 2023, max compression
```

## Comparing `resotometrics-3.4.2.tar` & `resotometrics-3.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:37.029779 resotometrics-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 12:22:09.000000 resotometrics-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-10 12:24:37.029779 resotometrics-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-10 12:22:09.000000 resotometrics-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:22:09.000000 resotometrics-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:37.025779 resotometrics-3.4.2/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 12:22:09.000000 resotometrics-3.4.2/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:37.029779 resotometrics-3.4.2/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 12:24:37.000000 resotometrics-3.4.2/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:24:37.029779 resotometrics-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-10 12:22:09.000000 resotometrics-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:24:37.029779 resotometrics-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-10 12:22:09.000000 resotometrics-3.4.2/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:55.768649 resotometrics-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 18:21:43.000000 resotometrics-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-26 18:23:55.768649 resotometrics-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-26 18:21:43.000000 resotometrics-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:21:43.000000 resotometrics-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:55.768649 resotometrics-3.5.0/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-26 18:21:43.000000 resotometrics-3.5.0/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:55.768649 resotometrics-3.5.0/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 18:23:55.000000 resotometrics-3.5.0/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:23:55.768649 resotometrics-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-26 18:21:43.000000 resotometrics-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:23:55.768649 resotometrics-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 18:21:43.000000 resotometrics-3.5.0/test/test_args.py
```

### Comparing `resotometrics-3.4.2/PKG-INFO` & `resotometrics-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.4.2
+Version: 3.5.0
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.4.2/README.md` & `resotometrics-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics/__main__.py` & `resotometrics-3.5.0/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics/config.py` & `resotometrics-3.5.0/resotometrics/config.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics/default_metrics.yaml` & `resotometrics-3.5.0/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics/metrics.py` & `resotometrics-3.5.0/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics/search.py` & `resotometrics-3.5.0/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.5.0/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.4.2
+Version: 3.5.0
 Summary: Exports Resoto metrics in Prometheus format.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotometrics
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.4.2/setup.py` & `resotometrics-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.4.2/test/test_args.py` & `resotometrics-3.5.0/test/test_args.py`

 * *Files identical despite different names*


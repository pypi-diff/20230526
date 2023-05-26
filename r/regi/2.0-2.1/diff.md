# Comparing `tmp/regi-2.0.tar.gz` & `tmp/regi-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regi-2.0.tar", last modified: Sat May 27 00:00:10 2023, max compression
+gzip compressed data, was "regi-2.1.tar", last modified: Sat May 27 02:17:12 2023, max compression
```

## Comparing `regi-2.0.tar` & `regi-2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.736354 regi-2.0/
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regi-2.0/LICENCE.txt
--rw-rw-rw-   0        0        0      180 2023-05-27 00:00:10.734354 regi-2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regi-2.0/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.671391 regi-2.0/regi/
--rw-rw-rw-   0        0        0       42 2023-05-26 23:59:55.000000 regi-2.0/regi/__init__.py
--rw-rw-rw-   0        0        0     2033 2023-05-26 23:59:52.000000 regi-2.0/regi/regi.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.729359 regi-2.0/regi.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 00:00:10.736354 regi-2.0/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-05-26 23:59:54.000000 regi-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:17:12.033275 regi-2.1/
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regi-2.1/LICENCE.txt
+-rw-rw-rw-   0        0        0      180 2023-05-27 02:17:12.031273 regi-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regi-2.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 02:17:11.993295 regi-2.1/regi/
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:59:55.000000 regi-2.1/regi/__init__.py
+-rw-rw-rw-   0        0        0     2438 2023-05-27 02:16:39.000000 regi-2.1/regi/regi.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:17:12.026278 regi-2.1/regi.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:17:12.034273 regi-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      353 2023-05-27 02:16:55.000000 regi-2.1/setup.py
```

### Comparing `regi-2.0/regi/regi.py` & `regi-2.1/regi/regi.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,8 +74,26 @@
     y_pred = np.dot(X, model)
     
     return y_pred
 
 
 
 
+def mean_absolute_error(y_actual, y_pred):
+    return np.mean(np.abs(y_actual - y_pred))
+
+import numpy as np
+
+def root_mean_squared_error(y_actual, y_pred):
+    return np.sqrt(np.mean((y_actual - y_pred)**2))
+
+import numpy as np
+
+def r_squared(y_actual, y_pred):
+    ssr = np.sum((y_actual - y_pred)**2)
+    sst = np.sum((y_actual - np.mean(y_actual))**2)
+    return 1 - (ssr / sst)
+
+
+
+
```


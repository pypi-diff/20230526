# Comparing `tmp/regi-2.1.tar.gz` & `tmp/regi-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regi-2.1.tar", last modified: Sat May 27 02:17:12 2023, max compression
+gzip compressed data, was "regi-3.0.tar", last modified: Sat May 27 02:21:05 2023, max compression
```

## Comparing `regi-2.1.tar` & `regi-3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 02:17:12.033275 regi-2.1/
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regi-2.1/LICENCE.txt
--rw-rw-rw-   0        0        0      180 2023-05-27 02:17:12.031273 regi-2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regi-2.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 02:17:11.993295 regi-2.1/regi/
--rw-rw-rw-   0        0        0       42 2023-05-26 23:59:55.000000 regi-2.1/regi/__init__.py
--rw-rw-rw-   0        0        0     2438 2023-05-27 02:16:39.000000 regi-2.1/regi/regi.py
-drwxrwxrwx   0        0        0        0 2023-05-27 02:17:12.026278 regi-2.1/regi.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 02:17:11.000000 regi-2.1/regi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 02:17:12.034273 regi-2.1/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-05-27 02:16:55.000000 regi-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:21:05.434562 regi-3.0/
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regi-3.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      180 2023-05-27 02:21:05.431546 regi-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regi-3.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 02:21:05.382576 regi-3.0/regi/
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:59:55.000000 regi-3.0/regi/__init__.py
+-rw-rw-rw-   0        0        0     2438 2023-05-27 02:16:39.000000 regi-3.0/regi/regi.py
+drwxrwxrwx   0        0        0        0 2023-05-27 02:21:05.425552 regi-3.0/regi.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-05-27 02:21:05.000000 regi-3.0/regi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-27 02:21:05.000000 regi-3.0/regi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 02:21:05.000000 regi-3.0/regi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-27 02:21:05.000000 regi-3.0/regi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 02:21:05.436543 regi-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      353 2023-05-27 02:20:56.000000 regi-3.0/setup.py
```

### Comparing `regi-2.1/regi/regi.py` & `regi-3.0/regi/regi.py`

 * *Files identical despite different names*


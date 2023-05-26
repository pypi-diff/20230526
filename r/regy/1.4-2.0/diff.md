# Comparing `tmp/regy-1.4.tar.gz` & `tmp/regy-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regy-1.4.tar", last modified: Fri May 26 23:40:56 2023, max compression
+gzip compressed data, was "regy-2.0.tar", last modified: Fri May 26 23:43:04 2023, max compression
```

## Comparing `regy-1.4.tar` & `regy-2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:40:56.962747 regy-1.4/
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regy-1.4/LICENCE.txt
--rw-rw-rw-   0        0        0      180 2023-05-26 23:40:56.960749 regy-1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regy-1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 23:40:56.923769 regy-1.4/reg/
--rw-rw-rw-   0        0        0       42 2023-05-26 23:25:57.000000 regy-1.4/reg/__init__.py
--rw-rw-rw-   0        0        0     2029 2023-05-26 23:40:30.000000 regy-1.4/reg/regi.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:40:56.946757 regy-1.4/regy.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-26 23:40:56.000000 regy-1.4/regy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-05-26 23:40:56.000000 regy-1.4/regy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:40:56.000000 regy-1.4/regy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-26 23:40:56.000000 regy-1.4/regy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 23:40:56.962747 regy-1.4/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-05-26 23:40:43.000000 regy-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:43:04.254082 regy-2.0/
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regy-2.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      180 2023-05-26 23:43:04.248086 regy-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regy-2.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 23:43:04.214105 regy-2.0/reg/
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:25:57.000000 regy-2.0/reg/__init__.py
+-rw-rw-rw-   0        0        0     2029 2023-05-26 23:40:30.000000 regy-2.0/reg/regi.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:43:04.235093 regy-2.0/regy.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-05-26 23:43:03.000000 regy-2.0/regy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-05-26 23:43:04.000000 regy-2.0/regy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 23:43:03.000000 regy-2.0/regy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-26 23:43:03.000000 regy-2.0/regy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:43:04.254082 regy-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-05-26 23:42:55.000000 regy-2.0/setup.py
```

### Comparing `regy-1.4/reg/regi.py` & `regy-2.0/reg/regi.py`

 * *Files identical despite different names*


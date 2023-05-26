# Comparing `tmp/regi-1.0.tar.gz` & `tmp/regi-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regi-1.0.tar", last modified: Fri May 26 23:00:19 2023, max compression
+gzip compressed data, was "regi-1.2.tar", last modified: Fri May 26 23:14:39 2023, max compression
```

## Comparing `regi-1.0.tar` & `regi-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:00:19.530195 regi-1.0/
--rw-rw-rw-   0        0        0        0 2023-05-26 22:43:45.000000 regi-1.0/LICENCE.txt
--rw-rw-rw-   0        0        0      180 2023-05-26 23:00:19.527194 regi-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 23:00:19.482219 regi-1.0/main_file/
--rw-rw-rw-   0        0        0        0 2023-05-26 22:42:48.000000 regi-1.0/main_file/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-05-26 22:56:58.000000 regi-1.0/main_file/regi.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:00:19.513202 regi-1.0/regi.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-26 23:00:19.000000 regi-1.0/regi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-26 23:00:19.000000 regi-1.0/regi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:00:19.000000 regi-1.0/regi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 23:00:19.000000 regi-1.0/regi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 23:00:19.531191 regi-1.0/setup.cfg
--rw-rw-rw-   0        0        0      283 2023-05-26 22:59:30.000000 regi-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.122681 regi-1.2/
+-rw-rw-rw-   0        0        0        0 2023-05-26 22:43:45.000000 regi-1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0      180 2023-05-26 23:14:39.119684 regi-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.053722 regi-1.2/main/
+-rw-rw-rw-   0        0        0        0 2023-05-26 22:42:48.000000 regi-1.2/main/__init__.py
+-rw-rw-rw-   0        0        0     3177 2023-05-26 22:56:58.000000 regi-1.2/main/regi.py
+drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.114686 regi-1.2/regi.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:14:39.122681 regi-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      278 2023-05-26 23:14:20.000000 regi-1.2/setup.py
```

### Comparing `regi-1.0/main_file/regi.py` & `regi-1.2/main/regi.py`

 * *Files identical despite different names*


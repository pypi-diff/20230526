# Comparing `tmp/sciform-0.2.0.tar.gz` & `tmp/sciform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciform-0.2.0.tar", last modified: Fri May 26 14:38:14 2023, max compression
+gzip compressed data, was "sciform-0.2.1.tar", last modified: Fri May 26 14:44:32 2023, max compression
```

## Comparing `sciform-0.2.0.tar` & `sciform-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:38:14.717423 sciform-0.2.0/
--rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      314 2023-05-26 14:38:14.716424 sciform-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-26 03:37:34.000000 sciform-0.2.0/README.md
--rw-rw-rw-   0        0        0      487 2023-05-26 14:37:55.000000 sciform-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 14:38:14.717423 sciform-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 14:38:14.609823 sciform-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:38:14.700045 sciform-0.2.0/src/sciform/
--rw-rw-rw-   0        0        0       84 2023-05-26 14:35:02.000000 sciform-0.2.0/src/sciform/__init__.py
--rw-rw-rw-   0        0        0     6268 2023-05-26 02:13:00.000000 sciform-0.2.0/src/sciform/format.py
--rw-rw-rw-   0        0        0     6178 2023-05-26 01:43:12.000000 sciform-0.2.0/src/sciform/format_utils.py
--rw-rw-rw-   0        0        0     2185 2023-05-26 01:33:01.000000 sciform-0.2.0/src/sciform/grouping.py
--rw-rw-rw-   0        0        0     2388 2023-05-25 23:32:37.000000 sciform-0.2.0/src/sciform/modes.py
--rw-rw-rw-   0        0        0     1772 2023-05-25 23:32:37.000000 sciform-0.2.0/src/sciform/prefix.py
--rw-rw-rw-   0        0        0     2509 2023-05-26 13:43:50.000000 sciform-0.2.0/src/sciform/sfloat.py
--rw-rw-rw-   0        0        0     3535 2023-05-26 03:59:52.000000 sciform-0.2.0/src/sciform/unc_format.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:38:14.714421 sciform-0.2.0/src/sciform.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-26 14:38:14.000000 sciform-0.2.0/src/sciform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-26 14:38:14.000000 sciform-0.2.0/src/sciform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:38:14.000000 sciform-0.2.0/src/sciform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 14:38:14.000000 sciform-0.2.0/src/sciform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 14:38:14.715421 sciform-0.2.0/tests/
--rw-rw-rw-   0        0        0     4440 2023-05-26 13:54:12.000000 sciform-0.2.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.505710 sciform-0.2.1/
+-rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      376 2023-05-26 14:44:32.504451 sciform-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-26 03:37:34.000000 sciform-0.2.1/README.md
+-rw-rw-rw-   0        0        0      557 2023-05-26 14:41:29.000000 sciform-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:44:32.505710 sciform-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.471731 sciform-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.484733 sciform-0.2.1/src/sciform/
+-rw-rw-rw-   0        0        0       84 2023-05-26 14:43:39.000000 sciform-0.2.1/src/sciform/__init__.py
+-rw-rw-rw-   0        0        0     6268 2023-05-26 02:13:00.000000 sciform-0.2.1/src/sciform/format.py
+-rw-rw-rw-   0        0        0     6178 2023-05-26 01:43:12.000000 sciform-0.2.1/src/sciform/format_utils.py
+-rw-rw-rw-   0        0        0     2185 2023-05-26 01:33:01.000000 sciform-0.2.1/src/sciform/grouping.py
+-rw-rw-rw-   0        0        0     2388 2023-05-25 23:32:37.000000 sciform-0.2.1/src/sciform/modes.py
+-rw-rw-rw-   0        0        0     1772 2023-05-25 23:32:37.000000 sciform-0.2.1/src/sciform/prefix.py
+-rw-rw-rw-   0        0        0     2509 2023-05-26 13:43:50.000000 sciform-0.2.1/src/sciform/sfloat.py
+-rw-rw-rw-   0        0        0     3535 2023-05-26 03:59:52.000000 sciform-0.2.1/src/sciform/unc_format.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.503449 sciform-0.2.1/src/sciform.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.504451 sciform-0.2.1/tests/
+-rw-rw-rw-   0        0        0     4440 2023-05-26 13:54:12.000000 sciform-0.2.1/tests/test.py
```

### Comparing `sciform-0.2.0/LICENSE` & `sciform-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/format.py` & `sciform-0.2.1/src/sciform/format.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/format_utils.py` & `sciform-0.2.1/src/sciform/format_utils.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/grouping.py` & `sciform-0.2.1/src/sciform/grouping.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/modes.py` & `sciform-0.2.1/src/sciform/modes.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/prefix.py` & `sciform-0.2.1/src/sciform/prefix.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/sfloat.py` & `sciform-0.2.1/src/sciform/sfloat.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/src/sciform/unc_format.py` & `sciform-0.2.1/src/sciform/unc_format.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.0/tests/test.py` & `sciform-0.2.1/tests/test.py`

 * *Files identical despite different names*


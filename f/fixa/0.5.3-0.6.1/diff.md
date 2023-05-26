# Comparing `tmp/fixa-0.5.3.tar.gz` & `tmp/fixa-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.5.3.tar", last modified: Fri May 12 18:00:50 2023, max compression
+gzip compressed data, was "fixa-0.6.1.tar", last modified: Fri May 26 17:33:49 2023, max compression
```

## Comparing `fixa-0.5.3.tar` & `fixa-0.6.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.518517 fixa-0.5.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.5.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.5.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.5.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 18:00:50.518370 fixa-0.5.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.5.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.514682 fixa-0.5.3/fixa/
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-12 18:00:33.000000 fixa-0.5.3/fixa/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.5.3/fixa/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.5.3/fixa/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.5.3/fixa/dataclass_dataframe.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515384 fixa-0.5.3/fixa/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.5.3/fixa/git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.5.3/fixa/iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.5.3/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.5.3/fixa/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.5.3/fixa/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.5.3/fixa/rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.5.3/fixa/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515601 fixa-0.5.3/fixa/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.5.3/fixa/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.5.3/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.515263 fixa-0.5.3/fixa.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      889 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-12 18:00:50.000000 fixa-0.5.3/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2338 2023-05-12 17:59:25.000000 fixa-0.5.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.5.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-12 18:00:50.518560 fixa-0.5.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.5.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-12 18:00:50.518108 fixa-0.5.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.5.3/tests/test_better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.5.3/tests/test_better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.5.3/tests/test_binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.5.3/tests/test_dataclass_dataframe.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.5.3/tests/test_git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.5.3/tests/test_hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.5.3/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.5.3/tests/test_iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.5.3/tests/test_nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.5.3/tests/test_rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.5.3/tests/test_timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.302509 fixa-0.6.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.6.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.6.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.6.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-26 17:33:49.302368 fixa-0.6.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.6.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.298437 fixa-0.6.1/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 17:22:04.000000 fixa-0.6.1/fixa/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.6.1/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      533 2023-05-06 03:13:06.000000 fixa-0.6.1/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 fixa-0.6.1/fixa/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.6.1/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299376 fixa-0.6.1/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2383 2023-05-06 03:09:12.000000 fixa-0.6.1/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5877 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.6.1/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.6.1/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.6.1/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.6.1/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.6.1/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.6.1/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299607 fixa-0.6.1/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.6.1/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.6.1/fixa/timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.299260 fixa-0.6.1/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-26 17:33:49.000000 fixa-0.6.1/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-26 17:22:09.000000 fixa-0.6.1/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2541 2023-05-26 17:22:50.000000 fixa-0.6.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-26 17:19:20.000000 fixa-0.6.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.6.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 17:33:49.302554 fixa-0.6.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.6.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 17:33:49.302088 fixa-0.6.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.6.1/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      663 2023-05-06 02:16:38.000000 fixa-0.6.1/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.6.1/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.6.1/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      740 2023-05-06 03:08:57.000000 fixa-0.6.1/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2178 2023-05-06 01:48:41.000000 fixa-0.6.1/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.6.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.6.1/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.6.1/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.6.1/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.6.1/tests/test_timer.py
```

### Comparing `fixa-0.5.3/LICENSE.txt` & `fixa-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/PKG-INFO` & `fixa-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.3
+Version: 0.6.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.3#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.6.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.3/README.rst` & `fixa-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/better_enum.py` & `fixa-0.6.1/fixa/better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/better_pathlib.py` & `fixa-0.6.1/fixa/better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/binarysearch.py` & `fixa-0.6.1/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/dataclass_dataframe.py` & `fixa-0.6.1/fixa/dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/git_cli.py` & `fixa-0.6.1/fixa/git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/hashes.py` & `fixa-0.6.1/fixa/hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/iterable.py` & `fixa-0.6.1/fixa/iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/nest_logger.py` & `fixa-0.6.1/fixa/nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/pytest_cov_helper.py` & `fixa-0.6.1/fixa/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/rnd.py` & `fixa-0.6.1/fixa/rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/runtime.py` & `fixa-0.6.1/fixa/runtime.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/tests/__init__.py` & `fixa-0.6.1/fixa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa/timer.py` & `fixa-0.6.1/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/fixa.egg-info/PKG-INFO` & `fixa-0.6.1/fixa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.5.3
+Version: 0.6.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.5.3#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.6.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.5.3/fixa.egg-info/SOURCES.txt` & `fixa-0.6.1/fixa.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 release-history.rst
 requirements-dev.txt
 requirements-doc.txt
 requirements-test.txt
 requirements.txt
 setup.py
 fixa/__init__.py
 fixa/_version.py
 fixa/better_enum.py
 fixa/better_pathlib.py
 fixa/binarysearch.py
+fixa/build_dist.py
 fixa/dataclass_dataframe.py
 fixa/git_cli.py
 fixa/hashes.py
 fixa/iterable.py
 fixa/nest_logger.py
 fixa/os_platform.py
 fixa/pytest_cov_helper.py
```

### Comparing `fixa-0.5.3/release-history.rst` & `fixa-0.6.1/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.6.1 (2023-05-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``build_dist`` module to build the source distribution of Python.
+
+
 0.5.3 (2023-05-12)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - allow mini string template in ``nest_logger.NestedLogger.pretty_log``, ``nest_logger.NestedLogger.start_and_end``.
```

### Comparing `fixa-0.5.3/requirements-doc.txt` & `fixa-0.6.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/setup.py` & `fixa-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_better_enum.py` & `fixa-0.6.1/tests/test_better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_better_pathlib.py` & `fixa-0.6.1/tests/test_better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_binarysearch.py` & `fixa-0.6.1/tests/test_binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_dataclass_dataframe.py` & `fixa-0.6.1/tests/test_dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_git_cli.py` & `fixa-0.6.1/tests/test_git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_hashes.py` & `fixa-0.6.1/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_iterable.py` & `fixa-0.6.1/tests/test_iterable.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_nest_logger.py` & `fixa-0.6.1/tests/test_nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_rnd.py` & `fixa-0.6.1/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.5.3/tests/test_timer.py` & `fixa-0.6.1/tests/test_timer.py`

 * *Files identical despite different names*


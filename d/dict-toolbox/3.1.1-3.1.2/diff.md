# Comparing `tmp/dict-toolbox-3.1.1.tar.gz` & `tmp/dict-toolbox-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict-toolbox-3.1.1.tar", last modified: Fri May 12 20:21:26 2023, max compression
+gzip compressed data, was "dict-toolbox-3.1.2.tar", last modified: Fri May 26 17:20:56 2023, max compression
```

## Comparing `dict-toolbox-3.1.1.tar` & `dict-toolbox-3.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/
--rw-r--r--   0 root         (0) root         (0)    19053 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6418 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5499 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/dict_toolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6418 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-12 20:21:26.000000 dict-toolbox-3.1.1/dict_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/dict_tools/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/args.py
--rw-r--r--   0 root         (0) root         (0)    28208 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/data.py
--rw-r--r--   0 root         (0) root         (0)    15032 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/differ.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/trim.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/typing.py
--rw-r--r--   0 root         (0) root         (0)     9583 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/update.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/xml.py
--rw-r--r--   0 root         (0) root         (0)    12072 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/dict_tools/yamlex.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 20:21:26.843874 dict-toolbox-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2687 2023-05-12 20:21:11.000000 dict-toolbox-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/
+-rw-r--r--   0 root         (0) root         (0)    19053 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/dict_toolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/dict_tools/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/args.py
+-rw-r--r--   0 root         (0) root         (0)    28296 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/data.py
+-rw-r--r--   0 root         (0) root         (0)    15032 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/differ.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/trim.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/typing.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/update.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/xml.py
+-rw-r--r--   0 root         (0) root         (0)    12072 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/yamlex.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 17:20:56.424106 dict-toolbox-3.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/setup.py
```

### Comparing `dict-toolbox-3.1.1/LICENSE` & `dict-toolbox-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/PKG-INFO` & `dict-toolbox-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.1
+Version: 3.1.2
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `dict-toolbox-3.1.1/README.rst` & `dict-toolbox-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_toolbox.egg-info/PKG-INFO` & `dict-toolbox-3.1.2/dict_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.1
+Version: 3.1.2
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `dict-toolbox-3.1.1/dict_tools/aggregation.py` & `dict-toolbox-3.1.2/dict_tools/aggregation.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/args.py` & `dict-toolbox-3.1.2/dict_tools/args.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/data.py` & `dict-toolbox-3.1.2/dict_tools/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,16 +497,19 @@
                 )
                 if not res:  # Equal
                     del ret_old[key]
                     del ret_new[key]
                 else:
                     ret_old[key] = res["old"]
                     ret_new[key] = res["new"]
-            elif ignore_missing_keys and key in old:
-                del ret_old[key]
+            elif ignore_missing_keys:
+                if key in old:
+                    del ret_old[key]
+                if key in new:
+                    del ret_new[key]
         ret = {"old": ret_old, "new": ret_new} if ret_old or ret_new else {}
     elif isinstance(old, set) and isinstance(new, set):
         ret = {"old": old - new, "new": new - old} if old - new or new - old else {}
     elif (
         isinstance(old, Iterable)
         and not isinstance(old, str)
         and isinstance(new, Iterable)
```

### Comparing `dict-toolbox-3.1.1/dict_tools/differ.py` & `dict-toolbox-3.1.2/dict_tools/differ.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/mysql.py` & `dict-toolbox-3.1.2/dict_tools/mysql.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/trim.py` & `dict-toolbox-3.1.2/dict_tools/trim.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/typing.py` & `dict-toolbox-3.1.2/dict_tools/typing.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/update.py` & `dict-toolbox-3.1.2/dict_tools/update.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/utils.py` & `dict-toolbox-3.1.2/dict_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/xml.py` & `dict-toolbox-3.1.2/dict_tools/xml.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/dict_tools/yamlex.py` & `dict-toolbox-3.1.2/dict_tools/yamlex.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.1/setup.py` & `dict-toolbox-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "dict_tools"
 DESC = "Dict tools for Python projects"
 
 # Version info -- read without importing
-VERSION = "3.1.1"
+VERSION = "3.1.2"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
```


# Comparing `tmp/llsd-1.2.2.dev1.tar.gz` & `tmp/llsd-1.2.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llsd-1.2.2.dev1.tar", last modified: Thu May 25 23:54:23 2023, max compression
+gzip compressed data, was "llsd-1.2.2.dev3.tar", last modified: Fri May 26 00:06:28 2023, max compression
```

## Comparing `llsd-1.2.2.dev1.tar` & `llsd-1.2.2.dev3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/dependabot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/bench.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/llsd/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/fastest_elementtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/llsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/llsd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.465992 llsd-1.2.2.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.461992 llsd-1.2.2.dev3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.github/dependabot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.461992 llsd-1.2.2.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.github/workflows/bench.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-26 00:06:28.465992 llsd-1.2.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.461992 llsd-1.2.2.dev3/llsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/fastest_elementtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/serde_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/serde_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/llsd/serde_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.461992 llsd-1.2.2.dev3/llsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-26 00:06:28.000000 llsd-1.2.2.dev3/llsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-26 00:06:28.000000 llsd-1.2.2.dev3/llsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:06:28.000000 llsd-1.2.2.dev3/llsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 00:06:28.000000 llsd-1.2.2.dev3/llsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 00:06:28.000000 llsd-1.2.2.dev3/llsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:06:28.465992 llsd-1.2.2.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:06:28.465992 llsd-1.2.2.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/tests/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/tests/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/tests/llsd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 00:05:27.000000 llsd-1.2.2.dev3/tox.ini
```

### Comparing `llsd-1.2.2.dev1/.github/workflows/bench.yaml` & `llsd-1.2.2.dev3/.github/workflows/bench.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/.github/workflows/ci.yaml` & `llsd-1.2.2.dev3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/.github/workflows/cla.yaml` & `llsd-1.2.2.dev3/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/.gitignore` & `llsd-1.2.2.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/LICENSE` & `llsd-1.2.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/PKG-INFO` & `llsd-1.2.2.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.2.dev1
+Version: 1.2.2.dev3
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.2.dev1/README.md` & `llsd-1.2.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/__init__.py` & `llsd-1.2.2.dev3/llsd/__init__.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/base.py` & `llsd-1.2.2.dev3/llsd/base.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/fastest_elementtree.py` & `llsd-1.2.2.dev3/llsd/fastest_elementtree.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/serde_binary.py` & `llsd-1.2.2.dev3/llsd/serde_binary.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/serde_notation.py` & `llsd-1.2.2.dev3/llsd/serde_notation.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd/serde_xml.py` & `llsd-1.2.2.dev3/llsd/serde_xml.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/llsd.egg-info/PKG-INFO` & `llsd-1.2.2.dev3/llsd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.2.dev1
+Version: 1.2.2.dev3
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.2.dev1/llsd.egg-info/SOURCES.txt` & `llsd-1.2.2.dev3/llsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/setup.py` & `llsd-1.2.2.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/tests/bench.py` & `llsd-1.2.2.dev3/tests/bench.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/tests/fuzz.py` & `llsd-1.2.2.dev3/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.2.dev1/tests/llsd_test.py` & `llsd-1.2.2.dev3/tests/llsd_test.py`

 * *Files identical despite different names*


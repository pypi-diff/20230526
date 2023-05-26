# Comparing `tmp/pointing_utils-0.0.1.tar.gz` & `tmp/pointing_utils-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointing_utils-0.0.1.tar", max compression
+gzip compressed data, was "pointing_utils-0.0.2.dev0.tar", max compression
```

## Comparing `pointing_utils-0.0.1.tar` & `pointing_utils-0.0.2.dev0.tar`

### file list

```diff
@@ -1,6 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-02-27 15:53:16.902111 pointing_utils-0.0.1/LICENSE
--rw-r--r--   0        0        0       68 2023-02-27 16:16:08.268395 pointing_utils-0.0.1/pointing_utils/__init__.py
--rw-r--r--   0        0        0    12142 2023-02-28 09:19:38.408395 pointing_utils-0.0.1/pointing_utils/utils.py
--rw-r--r--   0        0        0      627 2023-02-28 10:31:58.351109 pointing_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      744 2023-02-28 10:38:10.282204 pointing_utils-0.0.1/setup.py
--rw-r--r--   0        0        0      592 2023-02-28 10:38:10.282381 pointing_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-02-27 15:53:16.902111 pointing_utils-0.0.2.dev0/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-26 13:29:27.058838 pointing_utils-0.0.2.dev0/pointing_utils/__init__.py
+-rw-r--r--   0        0        0      826 2023-04-22 10:42:33.409210 pointing_utils-0.0.2.dev0/pointing_utils/filter.py
+-rw-r--r--   0        0        0      435 2023-04-21 14:01:45.646640 pointing_utils-0.0.2.dev0/pointing_utils/interpolate.py
+-rw-r--r--   0        0        0     2769 2023-05-26 13:15:33.663048 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/SOFCstepper.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:15:00.443690 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/__init__.py
+-rw-r--r--   0        0        0     9751 2023-05-26 13:19:41.402247 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/li2018.py
+-rw-r--r--   0        0        0     2759 2023-05-26 13:18:27.395684 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/lqg_ih.py
+-rw-r--r--   0        0        0     6225 2023-05-26 13:18:55.879131 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/phillis1985family.py
+-rw-r--r--   0        0        0     7430 2023-05-26 13:18:36.379510 pointing_utils-0.0.2.dev0/pointing_utils/optimal_control/qian2013.py
+-rw-r--r--   0        0        0    14281 2023-05-02 13:11:13.018821 pointing_utils-0.0.2.dev0/pointing_utils/segment.py
+-rw-r--r--   0        0        0    25559 2023-03-08 16:36:03.279075 pointing_utils-0.0.2.dev0/pointing_utils/throughput.py
+-rw-r--r--   0        0        0      671 2023-05-26 13:29:27.058838 pointing_utils-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-26 13:29:35.314462 pointing_utils-0.0.2.dev0/setup.py
+-rw-r--r--   0        0        0      680 2023-05-26 13:29:35.314719 pointing_utils-0.0.2.dev0/PKG-INFO
```

### Comparing `pointing_utils-0.0.1/LICENSE` & `pointing_utils-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pointing_utils-0.0.1/setup.py` & `pointing_utils-0.0.2.dev0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pointing_utils']
+['pointing_utils', 'pointing_utils.optimal_control']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['emgregs>=0.0.4,<0.0.5',
+['control>=0.9.3,<0.10.0',
+ 'emgregs>=0.0.4,<0.0.5',
  'matplotlib>=3.7.0,<4.0.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
- 'statsmodels>=0.13.5,<0.14.0']
+ 'statsmodels>=0.13.5,<0.14.0',
+ 'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pointing-utils',
-    'version': '0.0.1',
+    'version': '0.0.2.dev0',
     'description': 'Utilities for dealing with pointing data',
     'long_description': None,
     'author': 'jgori',
     'author_email': 'juliengori@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pointing_utils-0.0.1/PKG-INFO` & `pointing_utils-0.0.2.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: pointing-utils
-Version: 0.0.1
+Version: 0.0.2.dev0
 Summary: Utilities for dealing with pointing data
 Author: jgori
 Author-email: juliengori@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: control (>=0.9.3,<0.10.0)
 Requires-Dist: emgregs (>=0.0.4,<0.0.5)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
```


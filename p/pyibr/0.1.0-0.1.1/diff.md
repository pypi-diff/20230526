# Comparing `tmp/pyibr-0.1.0.tar.gz` & `tmp/pyibr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyibr-0.1.0.tar", last modified: Sat Sep 24 00:17:40 2022, max compression
+gzip compressed data, was "pyibr-0.1.1.tar", last modified: Fri May 26 16:47:11 2023, max compression
```

## Comparing `pyibr-0.1.0.tar` & `pyibr-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-09-24 00:17:40.022570 pyibr-0.1.0/
--rw-rw-rw-   0        0        0     1088 2022-08-29 10:59:36.000000 pyibr-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3115 2022-09-24 00:17:40.022570 pyibr-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2938 2022-09-24 00:17:19.000000 pyibr-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-24 00:17:40.029570 pyibr-0.1.0/ibr/
--rw-rw-rw-   0        0        0      272 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/__init__.py
--rw-rw-rw-   0        0        0      518 2022-09-24 00:17:40.029570 pyibr-0.1.0/ibr/_version.py
--rw-rw-rw-   0        0        0      936 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/efficiency.py
--rw-rw-rw-   0        0        0     1659 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/indebtedness.py
--rw-rw-rw-   0        0        0     1194 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/profitability.py
--rw-rw-rw-   0        0        0     2160 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/reader.py
--rw-rw-rw-   0        0        0      611 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/utils.py
--rw-rw-rw-   0        0        0     4451 2022-09-24 00:17:19.000000 pyibr-0.1.0/ibr/valuation.py
-drwxrwxrwx   0        0        0        0 2022-09-24 00:17:40.020570 pyibr-0.1.0/pyibr.egg-info/
--rw-rw-rw-   0        0        0     3115 2022-09-24 00:17:39.000000 pyibr-0.1.0/pyibr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2022-09-24 00:17:39.000000 pyibr-0.1.0/pyibr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-24 00:17:39.000000 pyibr-0.1.0/pyibr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2022-09-24 00:17:39.000000 pyibr-0.1.0/pyibr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-09-24 00:17:39.000000 pyibr-0.1.0/pyibr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2022-09-24 00:17:40.025570 pyibr-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1119 2022-09-24 00:17:19.000000 pyibr-0.1.0/setup.py
--rw-rw-rw-   0        0        0    84600 2022-09-24 00:17:19.000000 pyibr-0.1.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:47:11.926757 pyibr-0.1.1/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 16:41:47.000000 pyibr-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3124 2023-05-26 16:47:11.926757 pyibr-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2938 2022-10-07 11:36:56.000000 pyibr-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:47:11.930774 pyibr-0.1.1/ibr/
+-rw-rw-rw-   0        0        0      272 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-26 16:47:11.930774 pyibr-0.1.1/ibr/_version.py
+-rw-rw-rw-   0        0        0      936 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/efficiency.py
+-rw-rw-rw-   0        0        0     1659 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/indebtedness.py
+-rw-rw-rw-   0        0        0     1194 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/profitability.py
+-rw-rw-rw-   0        0        0     2160 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/reader.py
+-rw-rw-rw-   0        0        0      611 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/utils.py
+-rw-rw-rw-   0        0        0     4451 2022-10-07 11:36:56.000000 pyibr-0.1.1/ibr/valuation.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:47:11.924584 pyibr-0.1.1/pyibr.egg-info/
+-rw-rw-rw-   0        0        0     3124 2023-05-26 16:47:11.000000 pyibr-0.1.1/pyibr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-26 16:47:11.000000 pyibr-0.1.1/pyibr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:47:11.000000 pyibr-0.1.1/pyibr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-26 16:47:11.000000 pyibr-0.1.1/pyibr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-26 16:47:11.000000 pyibr-0.1.1/pyibr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2023-05-26 16:47:11.928773 pyibr-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-05-26 16:42:25.000000 pyibr-0.1.1/setup.py
+-rw-rw-rw-   0        0        0    84600 2022-10-07 11:36:56.000000 pyibr-0.1.1/versioneer.py
```

### Comparing `pyibr-0.1.0/LICENSE` & `pyibr-0.1.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Giovanni L
+Copyright (c) 2022-2023 Giovanni Lourenço Fernandes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyibr-0.1.0/PKG-INFO` & `pyibr-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyibr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculates fundamental analysis indicators of Brazilian companies
-Home-page: https://github.com/callmegiorgio/pyibr/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pyibr/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

### Comparing `pyibr-0.1.0/README.md` & `pyibr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/efficiency.py` & `pyibr-0.1.1/ibr/efficiency.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/indebtedness.py` & `pyibr-0.1.1/ibr/indebtedness.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/profitability.py` & `pyibr-0.1.1/ibr/profitability.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/reader.py` & `pyibr-0.1.1/ibr/reader.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/utils.py` & `pyibr-0.1.1/ibr/utils.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/ibr/valuation.py` & `pyibr-0.1.1/ibr/valuation.py`

 * *Files identical despite different names*

### Comparing `pyibr-0.1.0/pyibr.egg-info/PKG-INFO` & `pyibr-0.1.1/pyibr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyibr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculates fundamental analysis indicators of Brazilian companies
-Home-page: https://github.com/callmegiorgio/pyibr/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pyibr/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

### Comparing `pyibr-0.1.0/versioneer.py` & `pyibr-0.1.1/versioneer.py`

 * *Files identical despite different names*


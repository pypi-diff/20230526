# Comparing `tmp/pybov-0.1.1.tar.gz` & `tmp/pybov-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybov-0.1.1.tar", last modified: Fri Sep 23 23:52:12 2022, max compression
+gzip compressed data, was "pybov-0.1.2.tar", last modified: Fri May 26 17:05:58 2023, max compression
```

## Comparing `pybov-0.1.1.tar` & `pybov-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.080290 pybov-0.1.1/
--rw-rw-rw-   0        0        0     1088 2022-08-28 20:57:15.000000 pybov-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1909 2022-09-23 23:52:12.080290 pybov-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2022-09-23 22:13:26.000000 pybov-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.091307 pybov-0.1.1/b3/
--rw-rw-rw-   0        0        0      158 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/__init__.py
--rw-rw-rw-   0        0        0      518 2022-09-23 23:52:12.091307 pybov-0.1.1/b3/_version.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.047292 pybov-0.1.1/b3/datatypes/
--rw-rw-rw-   0        0        0      286 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/__init__.py
--rw-rw-rw-   0        0        0      671 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/company.py
--rw-rw-rw-   0        0        0      168 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/contract_correction.py
--rw-rw-rw-   0        0        0     4174 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/daily_bulletin.py
--rw-rw-rw-   0        0        0      670 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/market.py
--rw-rw-rw-   0        0        0      422 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/quotes.py
--rw-rw-rw-   0        0        0      555 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/datatypes/specification.py
--rw-rw-rw-   0        0        0       81 2022-08-28 20:00:41.000000 pybov-0.1.1/b3/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.051290 pybov-0.1.1/b3/net/
--rw-rw-rw-   0        0        0       26 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/net/__init__.py
--rw-rw-rw-   0        0        0     2615 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/net/query.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.055291 pybov-0.1.1/b3/parsing/
--rw-rw-rw-   0        0        0       42 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/parsing/__init__.py
--rw-rw-rw-   0        0        0     5557 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/parsing/historical_quotes.py
--rw-rw-rw-   0        0        0      828 2022-09-23 22:13:26.000000 pybov-0.1.1/b3/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:52:12.078291 pybov-0.1.1/pybov.egg-info/
--rw-rw-rw-   0        0        0     1909 2022-09-23 23:52:11.000000 pybov-0.1.1/pybov.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2022-09-23 23:52:11.000000 pybov-0.1.1/pybov.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 23:52:11.000000 pybov-0.1.1/pybov.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2022-09-23 23:52:11.000000 pybov-0.1.1/pybov.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2022-09-23 23:52:12.089290 pybov-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2022-09-23 23:51:34.000000 pybov-0.1.1/setup.py
--rw-rw-rw-   0        0        0    84600 2022-09-23 22:13:26.000000 pybov-0.1.1/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.928337 pybov-0.1.2/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 17:04:29.000000 pybov-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1918 2023-05-26 17:05:58.928337 pybov-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2022-10-07 11:33:08.000000 pybov-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.932135 pybov-0.1.2/b3/
+-rw-rw-rw-   0        0        0      158 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-26 17:05:58.932135 pybov-0.1.2/b3/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.842948 pybov-0.1.2/b3/datatypes/
+-rw-rw-rw-   0        0        0      286 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/__init__.py
+-rw-rw-rw-   0        0        0      671 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/company.py
+-rw-rw-rw-   0        0        0      168 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/contract_correction.py
+-rw-rw-rw-   0        0        0     4174 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/daily_bulletin.py
+-rw-rw-rw-   0        0        0      670 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/market.py
+-rw-rw-rw-   0        0        0      422 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/quotes.py
+-rw-rw-rw-   0        0        0      555 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/datatypes/specification.py
+-rw-rw-rw-   0        0        0       81 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.872689 pybov-0.1.2/b3/net/
+-rw-rw-rw-   0        0        0       26 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/net/__init__.py
+-rw-rw-rw-   0        0        0     2615 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/net/query.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.901334 pybov-0.1.2/b3/parsing/
+-rw-rw-rw-   0        0        0       42 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/parsing/__init__.py
+-rw-rw-rw-   0        0        0     5557 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/parsing/historical_quotes.py
+-rw-rw-rw-   0        0        0      828 2022-10-07 11:33:08.000000 pybov-0.1.2/b3/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:05:58.926334 pybov-0.1.2/pybov.egg-info/
+-rw-rw-rw-   0        0        0     1918 2023-05-26 17:05:58.000000 pybov-0.1.2/pybov.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-26 17:05:58.000000 pybov-0.1.2/pybov.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:05:58.000000 pybov-0.1.2/pybov.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-26 17:05:58.000000 pybov-0.1.2/pybov.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-05-26 17:05:58.931133 pybov-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-05-26 17:04:51.000000 pybov-0.1.2/setup.py
+-rw-rw-rw-   0        0        0    84600 2022-10-07 11:33:08.000000 pybov-0.1.2/versioneer.py
```

### Comparing `pybov-0.1.1/LICENSE` & `pybov-0.1.2/LICENSE`

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

### Comparing `pybov-0.1.1/PKG-INFO` & `pybov-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pybov
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for processing data from B3
-Home-page: https://github.com/callmegiorgio/pybov/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pybov/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybov-0.1.1/README.md` & `pybov-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/datatypes/company.py` & `pybov-0.1.2/b3/datatypes/company.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/datatypes/daily_bulletin.py` & `pybov-0.1.2/b3/datatypes/daily_bulletin.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/datatypes/market.py` & `pybov-0.1.2/b3/datatypes/market.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/datatypes/specification.py` & `pybov-0.1.2/b3/datatypes/specification.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/net/query.py` & `pybov-0.1.2/b3/net/query.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/parsing/historical_quotes.py` & `pybov-0.1.2/b3/parsing/historical_quotes.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/b3/utils.py` & `pybov-0.1.2/b3/utils.py`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/pybov.egg-info/PKG-INFO` & `pybov-0.1.2/pybov.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pybov
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for processing data from B3
-Home-page: https://github.com/callmegiorgio/pybov/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pybov/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybov-0.1.1/pybov.egg-info/SOURCES.txt` & `pybov-0.1.2/pybov.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybov-0.1.1/setup.py` & `pybov-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 setup(name                          = 'pybov',
       version                       = versioneer.get_version(),
       cmdclass                      = versioneer.get_cmdclass(),
       description                   = 'Python library for processing data from B3',
       long_description              = readme_en_us,
       long_description_content_type = 'text/markdown',
-      author                        = 'Giovanni L',
-      author_email                  = 'callmegiorgio@hotmail.com',
-      url                           = 'https://github.com/callmegiorgio/pybov/',
+      author                        = 'Giovanni Lourenço',
+      author_email                  = 'gvnl.developer@outlook.com',
+      url                           = 'https://github.com/glourencoffee/pybov/',
       license                       = 'MIT',
       packages                      = find_packages(),
       keywords                      = ['investment', 'finances'],
       install_requires              = [],
       python_requires               = '>=3.7'
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybov-0.1.1/versioneer.py` & `pybov-0.1.2/versioneer.py`

 * *Files identical despite different names*


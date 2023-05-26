# Comparing `tmp/rlist_files-0.0.2.tar.gz` & `tmp/rlist_files-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlist_files-0.0.2.tar", last modified: Thu Mar 16 19:22:31 2023, max compression
+gzip compressed data, was "rlist_files-0.0.3.tar", last modified: Fri May 26 20:40:18 2023, max compression
```

## Comparing `rlist_files-0.0.2.tar` & `rlist_files-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-03-16 19:22:31.785966 rlist_files-0.0.2/
--rw-rw-r--   0 matias    (1000) matias    (1000)      161 2023-03-16 15:21:45.000000 rlist_files-0.0.2/AUTHORS.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)     3556 2023-03-16 15:21:45.000000 rlist_files-0.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)       89 2023-03-16 15:21:45.000000 rlist_files-0.0.2/HISTORY.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)     1072 2023-03-16 15:21:45.000000 rlist_files-0.0.2/LICENSE
--rw-rw-r--   0 matias    (1000) matias    (1000)      262 2023-03-16 15:21:45.000000 rlist_files-0.0.2/MANIFEST.in
--rw-rw-r--   0 matias    (1000) matias    (1000)     2075 2023-03-16 19:22:31.785966 rlist_files-0.0.2/PKG-INFO
--rw-rw-r--   0 matias    (1000) matias    (1000)     1194 2023-03-16 17:29:02.000000 rlist_files-0.0.2/README.rst
-drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-03-16 19:22:31.785966 rlist_files-0.0.2/docs/
--rw-rw-r--   0 matias    (1000) matias    (1000)      611 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/Makefile
--rw-rw-r--   0 matias    (1000) matias    (1000)       28 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/authors.rst
--rwxrwxr-x   0 matias    (1000) matias    (1000)     4820 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/conf.py
--rw-rw-r--   0 matias    (1000) matias    (1000)       33 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/contributing.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)       28 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/history.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)      307 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/index.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)     1161 2023-03-16 19:19:56.000000 rlist_files-0.0.2/docs/installation.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)      808 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/make.bat
--rw-rw-r--   0 matias    (1000) matias    (1000)       27 2023-03-16 15:21:45.000000 rlist_files-0.0.2/docs/readme.rst
--rw-rw-r--   0 matias    (1000) matias    (1000)      263 2023-03-16 19:19:04.000000 rlist_files-0.0.2/docs/usage.rst
-drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-03-16 19:22:31.785966 rlist_files-0.0.2/rlist_files/
--rw-rw-r--   0 matias    (1000) matias    (1000)      179 2023-03-16 19:15:41.000000 rlist_files-0.0.2/rlist_files/__init__.py
--rw-rw-r--   0 matias    (1000) matias    (1000)     3104 2023-03-16 15:41:22.000000 rlist_files-0.0.2/rlist_files/list_files.py
-drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-03-16 19:22:31.785966 rlist_files-0.0.2/rlist_files.egg-info/
--rw-rw-r--   0 matias    (1000) matias    (1000)     2075 2023-03-16 19:22:31.000000 rlist_files-0.0.2/rlist_files.egg-info/PKG-INFO
--rw-rw-r--   0 matias    (1000) matias    (1000)      522 2023-03-16 19:22:31.000000 rlist_files-0.0.2/rlist_files.egg-info/SOURCES.txt
--rw-rw-r--   0 matias    (1000) matias    (1000)        1 2023-03-16 19:22:31.000000 rlist_files-0.0.2/rlist_files.egg-info/dependency_links.txt
--rw-rw-r--   0 matias    (1000) matias    (1000)        1 2023-03-16 15:57:56.000000 rlist_files-0.0.2/rlist_files.egg-info/not-zip-safe
--rw-rw-r--   0 matias    (1000) matias    (1000)       12 2023-03-16 19:22:31.000000 rlist_files-0.0.2/rlist_files.egg-info/top_level.txt
--rw-rw-r--   0 matias    (1000) matias    (1000)      427 2023-03-16 19:22:31.785966 rlist_files-0.0.2/setup.cfg
--rw-rw-r--   0 matias    (1000) matias    (1000)     1341 2023-03-16 19:20:28.000000 rlist_files-0.0.2/setup.py
-drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-03-16 19:22:31.785966 rlist_files-0.0.2/tests/
--rw-rw-r--   0 matias    (1000) matias    (1000)       40 2023-03-16 15:21:45.000000 rlist_files-0.0.2/tests/__init__.py
--rw-rw-r--   0 matias    (1000) matias    (1000)     1338 2023-03-16 15:41:16.000000 rlist_files-0.0.2/tests/test_list_files.py
+drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-05-26 20:40:18.798531 rlist_files-0.0.3/
+-rw-rw-r--   0 matias    (1000) matias    (1000)      161 2023-03-16 15:21:45.000000 rlist_files-0.0.3/AUTHORS.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)     3556 2023-03-16 15:21:45.000000 rlist_files-0.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)       89 2023-03-16 15:21:45.000000 rlist_files-0.0.3/HISTORY.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)     1072 2023-03-16 15:21:45.000000 rlist_files-0.0.3/LICENSE
+-rw-rw-r--   0 matias    (1000) matias    (1000)      262 2023-03-16 15:21:45.000000 rlist_files-0.0.3/MANIFEST.in
+-rw-rw-r--   0 matias    (1000) matias    (1000)     2075 2023-05-26 20:40:18.798531 rlist_files-0.0.3/PKG-INFO
+-rw-rw-r--   0 matias    (1000) matias    (1000)     1194 2023-03-16 17:29:02.000000 rlist_files-0.0.3/README.rst
+drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-05-26 20:40:18.798531 rlist_files-0.0.3/docs/
+-rw-rw-r--   0 matias    (1000) matias    (1000)      611 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/Makefile
+-rw-rw-r--   0 matias    (1000) matias    (1000)       28 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/authors.rst
+-rwxrwxr-x   0 matias    (1000) matias    (1000)     4820 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/conf.py
+-rw-rw-r--   0 matias    (1000) matias    (1000)       33 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/contributing.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)       28 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/history.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)      307 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/index.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)     1161 2023-03-16 19:19:56.000000 rlist_files-0.0.3/docs/installation.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)      808 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/make.bat
+-rw-rw-r--   0 matias    (1000) matias    (1000)       27 2023-03-16 15:21:45.000000 rlist_files-0.0.3/docs/readme.rst
+-rw-rw-r--   0 matias    (1000) matias    (1000)      263 2023-03-16 19:19:04.000000 rlist_files-0.0.3/docs/usage.rst
+drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-05-26 20:40:18.798531 rlist_files-0.0.3/rlist_files/
+-rw-rw-r--   0 matias    (1000) matias    (1000)      179 2023-03-16 19:15:41.000000 rlist_files-0.0.3/rlist_files/__init__.py
+-rw-rw-r--   0 matias    (1000) matias    (1000)     3133 2023-05-26 20:38:20.000000 rlist_files-0.0.3/rlist_files/list_files.py
+drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-05-26 20:40:18.798531 rlist_files-0.0.3/rlist_files.egg-info/
+-rw-rw-r--   0 matias    (1000) matias    (1000)     2075 2023-05-26 20:40:18.000000 rlist_files-0.0.3/rlist_files.egg-info/PKG-INFO
+-rw-rw-r--   0 matias    (1000) matias    (1000)      522 2023-05-26 20:40:18.000000 rlist_files-0.0.3/rlist_files.egg-info/SOURCES.txt
+-rw-rw-r--   0 matias    (1000) matias    (1000)        1 2023-05-26 20:40:18.000000 rlist_files-0.0.3/rlist_files.egg-info/dependency_links.txt
+-rw-rw-r--   0 matias    (1000) matias    (1000)        1 2023-03-16 15:57:56.000000 rlist_files-0.0.3/rlist_files.egg-info/not-zip-safe
+-rw-rw-r--   0 matias    (1000) matias    (1000)       12 2023-05-26 20:40:18.000000 rlist_files-0.0.3/rlist_files.egg-info/top_level.txt
+-rw-rw-r--   0 matias    (1000) matias    (1000)      427 2023-05-26 20:40:18.798531 rlist_files-0.0.3/setup.cfg
+-rw-rw-r--   0 matias    (1000) matias    (1000)     1341 2023-05-26 20:34:41.000000 rlist_files-0.0.3/setup.py
+drwxrwxr-x   0 matias    (1000) matias    (1000)        0 2023-05-26 20:40:18.798531 rlist_files-0.0.3/tests/
+-rw-rw-r--   0 matias    (1000) matias    (1000)       40 2023-03-16 15:21:45.000000 rlist_files-0.0.3/tests/__init__.py
+-rw-rw-r--   0 matias    (1000) matias    (1000)     1338 2023-03-16 15:41:16.000000 rlist_files-0.0.3/tests/test_list_files.py
```

### Comparing `rlist_files-0.0.2/CONTRIBUTING.rst` & `rlist_files-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/LICENSE` & `rlist_files-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/PKG-INFO` & `rlist_files-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlist_files
-Version: 0.0.2
+Version: 0.0.3
 Summary: Function to list the files in directory with pattern recognition and regular expression support.
 Home-page: https://github.com/matiasandina/rlist_files
 Author: Matias Andina
 Author-email: matiasandina@gmail.com
 License: MIT license
 Keywords: list_files
 Platform: UNKNOWN
```

### Comparing `rlist_files-0.0.2/README.rst` & `rlist_files-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/docs/Makefile` & `rlist_files-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/docs/conf.py` & `rlist_files-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/docs/installation.rst` & `rlist_files-0.0.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/docs/make.bat` & `rlist_files-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/rlist_files/list_files.py` & `rlist_files-0.0.3/rlist_files/list_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             matches.append(os.path.join(path, dirname))
           else:
             matches.append(dirname)
 
   if not all_files:
     matches = [m for m in matches if not os.path.isdir(m)]
 
+  # sort
+  matches.sort()
+  
   return matches
 
 
 import re
 import os
 
 def list_files_fast(path=os.getcwd(), pattern=None, all_files=False, full_names=False, recursive=False, ignore_case=False, include_dirs=False, no_dot=False):
```

### Comparing `rlist_files-0.0.2/rlist_files.egg-info/PKG-INFO` & `rlist_files-0.0.3/rlist_files.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlist-files
-Version: 0.0.2
+Version: 0.0.3
 Summary: Function to list the files in directory with pattern recognition and regular expression support.
 Home-page: https://github.com/matiasandina/rlist_files
 Author: Matias Andina
 Author-email: matiasandina@gmail.com
 License: MIT license
 Keywords: list_files
 Platform: UNKNOWN
```

### Comparing `rlist_files-0.0.2/rlist_files.egg-info/SOURCES.txt` & `rlist_files-0.0.3/rlist_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlist_files-0.0.2/setup.py` & `rlist_files-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='list_files',
     name='rlist_files',
     packages=find_packages(include=['rlist_files', 'list_files.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/matiasandina/rlist_files',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

### Comparing `rlist_files-0.0.2/tests/test_list_files.py` & `rlist_files-0.0.3/tests/test_list_files.py`

 * *Files identical despite different names*


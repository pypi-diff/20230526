# Comparing `tmp/pyqt5_fugueicons-3.5.6.1.tar.gz` & `tmp/pyqt5_fugueicons-3.5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5_fugueicons-3.5.6.1.tar", last modified: Fri Aug 26 20:13:26 2022, max compression
+gzip compressed data, was "pyqt5_fugueicons-3.5.6.2.tar", last modified: Fri May 26 16:32:26 2023, max compression
```

## Comparing `pyqt5_fugueicons-3.5.6.1.tar` & `pyqt5_fugueicons-3.5.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 20:13:26.015947 pyqt5_fugueicons-3.5.6.1/
--rw-rw-rw-   0        0        0     1088 2022-08-26 18:44:10.000000 pyqt5_fugueicons-3.5.6.1/LICENSE
--rw-rw-rw-   0        0        0     4320 2022-08-26 20:13:26.014947 pyqt5_fugueicons-3.5.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     3971 2022-08-26 19:38:37.000000 pyqt5_fugueicons-3.5.6.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-26 20:13:25.928948 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/
--rw-rw-rw-   0        0        0      150 2022-08-26 17:40:05.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/__init__.py
--rw-rw-rw-   0        0        0     2864 2022-08-26 20:10:29.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/icon.py
--rw-rw-rw-   0        0        0     2797 2022-08-26 20:08:54.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/movie.py
--rw-rw-rw-   0        0        0 18159192 2022-08-26 16:19:30.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/resources.py
-drwxrwxrwx   0        0        0        0 2022-08-26 20:13:26.012947 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/
--rw-rw-rw-   0        0        0     4320 2022-08-26 20:13:25.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2022-08-26 20:13:25.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 20:13:25.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-08-26 20:13:25.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-08-26 20:13:25.000000 pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-26 20:13:26.016949 pyqt5_fugueicons-3.5.6.1/setup.cfg
--rw-rw-rw-   0        0        0      565 2022-08-26 20:12:57.000000 pyqt5_fugueicons-3.5.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:32:26.331895 pyqt5_fugueicons-3.5.6.2/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 16:28:43.000000 pyqt5_fugueicons-3.5.6.2/LICENSE
+-rw-rw-rw-   0        0        0     4283 2023-05-26 16:32:26.330880 pyqt5_fugueicons-3.5.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3925 2022-08-26 20:23:55.000000 pyqt5_fugueicons-3.5.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:32:26.176858 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/
+-rw-rw-rw-   0        0        0      150 2022-08-26 17:40:05.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/__init__.py
+-rw-rw-rw-   0        0        0     2864 2022-08-26 20:10:29.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/icon.py
+-rw-rw-rw-   0        0        0     2797 2022-08-26 20:08:54.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/movie.py
+-rw-rw-rw-   0        0        0 18159192 2022-08-26 16:19:30.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/resources.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:32:26.328300 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/
+-rw-rw-rw-   0        0        0     4283 2023-05-26 16:32:25.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-05-26 16:32:25.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:32:25.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 16:32:25.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-26 16:32:25.000000 pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 16:32:26.332899 pyqt5_fugueicons-3.5.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      574 2023-05-26 16:29:17.000000 pyqt5_fugueicons-3.5.6.2/setup.py
```

### Comparing `pyqt5_fugueicons-3.5.6.1/LICENSE` & `pyqt5_fugueicons-3.5.6.2/LICENSE`

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

### Comparing `pyqt5_fugueicons-3.5.6.1/PKG-INFO` & `pyqt5_fugueicons-3.5.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyqt5_fugueicons
-Version: 3.5.6.1
+Version: 3.5.6.2
 Summary: Fugue Icons for PyQt5
-Home-page: https://github.com/callmegiorgio/pyqt5_fugueicons
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pyqt5_fugueicons
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: pyqt5,icons
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
@@ -65,17 +65,17 @@
 In the above code, if the shadowed version of the icon "application-blue" is
 not found with dimensions 24x24, the function will try to find the shadowed version
 of the same icon with dimensions 16x16. If still no icon is found, an empty
 `QIcon` is returned. `size` accepts the values 16, 24, and 32.
 
 ## Icon Names
 
-Icon names can be found in the author's [website][fugue-website] or in the file under
-`resources/FILENAME.txt`. An icon name is simply its file name without the extension.
-The function `iconNames()` returns all icon names:
+Icon names can be found in the author's [website][fugue-website]. An icon name
+is simply its file name without the extension. The function `iconNames()` returns
+all icon names:
 
 ```py
 for name in fugue.iconNames():
     print(name)
 ```
 
 ## Animated Icons
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt5_fugueicons-3.5.6.1/README.md` & `pyqt5_fugueicons-3.5.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 In the above code, if the shadowed version of the icon "application-blue" is
 not found with dimensions 24x24, the function will try to find the shadowed version
 of the same icon with dimensions 16x16. If still no icon is found, an empty
 `QIcon` is returned. `size` accepts the values 16, 24, and 32.
 
 ## Icon Names
 
-Icon names can be found in the author's [website][fugue-website] or in the file under
-`resources/FILENAME.txt`. An icon name is simply its file name without the extension.
-The function `iconNames()` returns all icon names:
+Icon names can be found in the author's [website][fugue-website]. An icon name
+is simply its file name without the extension. The function `iconNames()` returns
+all icon names:
 
 ```py
 for name in fugue.iconNames():
     print(name)
 ```
 
 ## Animated Icons
```

### Comparing `pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/icon.py` & `pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/icon.py`

 * *Files identical despite different names*

### Comparing `pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/movie.py` & `pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/movie.py`

 * *Files identical despite different names*

### Comparing `pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons/resources.py` & `pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons/resources.py`

 * *Files identical despite different names*

### Comparing `pyqt5_fugueicons-3.5.6.1/pyqt5_fugueicons.egg-info/PKG-INFO` & `pyqt5_fugueicons-3.5.6.2/pyqt5_fugueicons.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyqt5-fugueicons
-Version: 3.5.6.1
+Version: 3.5.6.2
 Summary: Fugue Icons for PyQt5
-Home-page: https://github.com/callmegiorgio/pyqt5_fugueicons
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pyqt5_fugueicons
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: pyqt5,icons
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
@@ -65,17 +65,17 @@
 In the above code, if the shadowed version of the icon "application-blue" is
 not found with dimensions 24x24, the function will try to find the shadowed version
 of the same icon with dimensions 16x16. If still no icon is found, an empty
 `QIcon` is returned. `size` accepts the values 16, 24, and 32.
 
 ## Icon Names
 
-Icon names can be found in the author's [website][fugue-website] or in the file under
-`resources/FILENAME.txt`. An icon name is simply its file name without the extension.
-The function `iconNames()` returns all icon names:
+Icon names can be found in the author's [website][fugue-website]. An icon name
+is simply its file name without the extension. The function `iconNames()` returns
+all icon names:
 
 ```py
 for name in fugue.iconNames():
     print(name)
 ```
 
 ## Animated Icons
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt5_fugueicons-3.5.6.1/setup.py` & `pyqt5_fugueicons-3.5.6.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='pyqt5_fugueicons',
-    version='3.5.6.1',
+    version='3.5.6.2',
     description='Fugue Icons for PyQt5',
     long_description=readme,
     long_description_content_type='text/markdown',
-    author='Giovanni L',
-    author_email='callmegiorgio@hotmail.com',
-    url='https://github.com/callmegiorgio/pyqt5_fugueicons',
+    author='Giovanni Lourenço',
+    author_email='gvnl.developer@outlook.com',
+    url='https://github.com/glourencoffee/pyqt5_fugueicons',
     license='MIT',
     packages=['pyqt5_fugueicons'],
     keywords=['pyqt5', 'icons'],
 
     install_requires=['PyQt5'],
 
     python_requires='>=3.6'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


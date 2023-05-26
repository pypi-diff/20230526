# Comparing `tmp/numtoname-0.1.2.tar.gz` & `tmp/numtoname-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numtoname-0.1.2.tar", last modified: Fri May 26 01:09:10 2023, max compression
+gzip compressed data, was "numtoname-0.1.3.tar", last modified: Fri May 26 01:13:45 2023, max compression
```

## Comparing `numtoname-0.1.2.tar` & `numtoname-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 01:09:10.939337 numtoname-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-05-26 01:09:10.939337 numtoname-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-26 00:55:44.000000 numtoname-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 01:09:10.894349 numtoname-0.1.2/numtoname/
--rw-rw-rw-   0        0        0      658 2023-05-25 23:33:05.000000 numtoname-0.1.2/numtoname/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-05-26 00:54:09.000000 numtoname-0.1.2/numtoname/functions.py
--rw-rw-rw-   0        0        0     3649 2023-05-25 17:01:14.000000 numtoname-0.1.2/numtoname/tests.py
-drwxrwxrwx   0        0        0        0 2023-05-26 01:09:10.935338 numtoname-0.1.2/numtoname.egg-info/
--rw-rw-rw-   0        0        0      693 2023-05-26 01:09:10.000000 numtoname-0.1.2/numtoname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-26 01:09:10.000000 numtoname-0.1.2/numtoname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 01:09:10.000000 numtoname-0.1.2/numtoname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 01:09:10.000000 numtoname-0.1.2/numtoname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-26 01:09:10.942335 numtoname-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-05-26 01:08:09.000000 numtoname-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 01:13:45.485424 numtoname-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-05-26 01:13:45.485424 numtoname-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-26 00:55:44.000000 numtoname-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 01:13:45.464433 numtoname-0.1.3/numtoname/
+-rw-rw-rw-   0        0        0      658 2023-05-26 01:11:29.000000 numtoname-0.1.3/numtoname/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-05-26 00:54:09.000000 numtoname-0.1.3/numtoname/functions.py
+-rw-rw-rw-   0        0        0     3649 2023-05-25 17:01:14.000000 numtoname-0.1.3/numtoname/tests.py
+drwxrwxrwx   0        0        0        0 2023-05-26 01:13:45.483460 numtoname-0.1.3/numtoname.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-05-26 01:13:45.000000 numtoname-0.1.3/numtoname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-26 01:13:45.000000 numtoname-0.1.3/numtoname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 01:13:45.000000 numtoname-0.1.3/numtoname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 01:13:45.000000 numtoname-0.1.3/numtoname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-26 01:13:45.489420 numtoname-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2023-05-26 01:11:38.000000 numtoname-0.1.3/setup.py
```

### Comparing `numtoname-0.1.2/LICENSE.txt` & `numtoname-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numtoname-0.1.2/PKG-INFO` & `numtoname-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: numtoname
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python module to convert a number or list of numbers into a variable name or list of variable names
 Home-page: https://github.com/benjaminmesser/Numtoname
-Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_012.tar.gz
+Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_013.tar.gz
 Author: Ben Messer
 Author-email: benjamin.messer@outlook.com
 License: MIT
 Keywords: tools,development,naming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `numtoname-0.1.2/numtoname/__init__.py` & `numtoname-0.1.3/numtoname/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from Numtoname.functions import generate_name_fixed
-from Numtoname.functions import generate_names_fixed
-from Numtoname.functions import generate_name
-from Numtoname.functions import generate_names
-from Numtoname.functions import generate_name_fixed_alpha
-from Numtoname.functions import generate_names_fixed_alpha
-from Numtoname.functions import generate_name_alpha
-from Numtoname.functions import generate_names_alpha
-from Numtoname.functions import generate_name_fixed_alpha2
-from Numtoname.functions import generate_names_fixed_alpha2
-from Numtoname.functions import generate_name_alpha2
-from Numtoname.functions import generate_names_alpha2
+from numtoname.functions import generate_name_fixed
+from numtoname.functions import generate_names_fixed
+from numtoname.functions import generate_name
+from numtoname.functions import generate_names
+from numtoname.functions import generate_name_fixed_alpha
+from numtoname.functions import generate_names_fixed_alpha
+from numtoname.functions import generate_name_alpha
+from numtoname.functions import generate_names_alpha
+from numtoname.functions import generate_name_fixed_alpha2
+from numtoname.functions import generate_names_fixed_alpha2
+from numtoname.functions import generate_name_alpha2
+from numtoname.functions import generate_names_alpha2
```

### Comparing `numtoname-0.1.2/numtoname/functions.py` & `numtoname-0.1.3/numtoname/functions.py`

 * *Files identical despite different names*

### Comparing `numtoname-0.1.2/numtoname/tests.py` & `numtoname-0.1.3/numtoname/tests.py`

 * *Files identical despite different names*

### Comparing `numtoname-0.1.2/numtoname.egg-info/PKG-INFO` & `numtoname-0.1.3/numtoname.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: numtoname
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python module to convert a number or list of numbers into a variable name or list of variable names
 Home-page: https://github.com/benjaminmesser/Numtoname
-Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_012.tar.gz
+Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_013.tar.gz
 Author: Ben Messer
 Author-email: benjamin.messer@outlook.com
 License: MIT
 Keywords: tools,development,naming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `numtoname-0.1.2/setup.py` & `numtoname-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'numtoname',         # How you named your package folder (MyLib)
   packages = ['numtoname'],   # Chose the same as "name"
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A python module to convert a number or list of numbers into a variable name or list of variable names',
   author = 'Ben Messer',
   author_email = 'benjamin.messer@outlook.com',
   url = 'https://github.com/benjaminmesser/Numtoname',
-  download_url = 'https://github.com/benjaminmesser/Numtoname/archive/v_012.tar.gz',
+  download_url = 'https://github.com/benjaminmesser/Numtoname/archive/v_013.tar.gz',
   keywords = ['tools', 'development', 'naming'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```


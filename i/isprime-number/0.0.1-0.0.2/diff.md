# Comparing `tmp/isprime_number-0.0.1.tar.gz` & `tmp/isprime_number-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isprime_number-0.0.1.tar", last modified: Fri May 26 11:52:41 2023, max compression
+gzip compressed data, was "isprime_number-0.0.2.tar", last modified: Fri May 26 14:45:41 2023, max compression
```

## Comparing `isprime_number-0.0.1.tar` & `isprime_number-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:52:41.045817 isprime_number-0.0.1/
--rw-rw-rw-   0        0        0      544 2023-05-26 11:52:41.043805 isprime_number-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 11:52:40.987806 isprime_number-0.0.1/isprime_number/
--rw-rw-rw-   0        0        0        0 2023-05-26 11:38:05.000000 isprime_number-0.0.1/isprime_number/__init__.py
--rw-rw-rw-   0        0        0       49 2023-05-26 11:49:59.000000 isprime_number-0.0.1/isprime_number/a.py
--rw-rw-rw-   0        0        0       29 2023-05-26 11:31:45.000000 isprime_number-0.0.1/isprime_number/add.py
--rw-rw-rw-   0        0        0      267 2023-05-26 11:50:05.000000 isprime_number-0.0.1/isprime_number/isprime.py
--rw-rw-rw-   0        0        0       29 2023-05-26 11:31:52.000000 isprime_number-0.0.1/isprime_number/sub.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:52:41.037800 isprime_number-0.0.1/isprime_number.egg-info/
--rw-rw-rw-   0        0        0      544 2023-05-26 11:52:40.000000 isprime_number-0.0.1/isprime_number.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-05-26 11:52:40.000000 isprime_number-0.0.1/isprime_number.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:52:40.000000 isprime_number-0.0.1/isprime_number.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 11:52:40.000000 isprime_number-0.0.1/isprime_number.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 11:52:41.046811 isprime_number-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-05-26 11:52:16.000000 isprime_number-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:41.118833 isprime_number-0.0.2/
+-rw-rw-rw-   0        0        0      544 2023-05-26 14:45:41.115849 isprime_number-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:41.024829 isprime_number-0.0.2/isprime_number/
+-rw-rw-rw-   0        0        0        0 2023-05-26 11:38:05.000000 isprime_number-0.0.2/isprime_number/__init__.py
+-rw-rw-rw-   0        0        0       49 2023-05-26 11:49:59.000000 isprime_number-0.0.2/isprime_number/a.py
+-rw-rw-rw-   0        0        0       29 2023-05-26 11:31:45.000000 isprime_number-0.0.2/isprime_number/add.py
+-rw-rw-rw-   0        0        0      267 2023-05-26 11:50:05.000000 isprime_number-0.0.2/isprime_number/isprime.py
+-rw-rw-rw-   0        0        0       29 2023-05-26 11:31:52.000000 isprime_number-0.0.2/isprime_number/sub.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:45:41.098837 isprime_number-0.0.2/isprime_number.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-05-26 14:45:40.000000 isprime_number-0.0.2/isprime_number.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-26 14:45:40.000000 isprime_number-0.0.2/isprime_number.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:45:40.000000 isprime_number-0.0.2/isprime_number.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-26 14:45:40.000000 isprime_number-0.0.2/isprime_number.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 14:45:40.000000 isprime_number-0.0.2/isprime_number.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:45:41.121823 isprime_number-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-05-26 14:45:29.000000 isprime_number-0.0.2/setup.py
```

### Comparing `isprime_number-0.0.1/PKG-INFO` & `isprime_number-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isprime_number
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: Aviral Srivastava
 Author-email: <youremail@email.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `isprime_number-0.0.1/isprime_number.egg-info/PKG-INFO` & `isprime_number-0.0.2/isprime_number.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isprime-number
-Version: 0.0.1
+Version: 0.0.2
 Summary: My first Python package
 Author: Aviral Srivastava
 Author-email: <youremail@email.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `isprime_number-0.0.1/setup.py` & `isprime_number-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package with a slightly longer description'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="isprime_number", 
         version=VERSION,
         author="Aviral Srivastava",
         author_email="<youremail@email.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=[], # add any additional packages that 
+        install_requires=['numpy', 'pandas'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
```


# Comparing `tmp/pycliwrapper-1.0.tar.gz` & `tmp/pycliwrapper-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycliwrapper-1.0.tar", last modified: Fri May 26 07:43:10 2023, max compression
+gzip compressed data, was "pycliwrapper-1.1.tar", last modified: Fri May 26 07:48:45 2023, max compression
```

## Comparing `pycliwrapper-1.0.tar` & `pycliwrapper-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:43:10.692983 pycliwrapper-1.0/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-26 07:43:10.692983 pycliwrapper-1.0/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      299 2023-05-25 14:23:47.000000 pycliwrapper-1.0/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:43:10.692983 pycliwrapper-1.0/pycliwrapper/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2085 2023-05-26 07:40:09.000000 pycliwrapper-1.0/pycliwrapper/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:43:10.692983 pycliwrapper-1.0/pycliwrapper.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      718 2023-05-26 07:43:10.000000 pycliwrapper-1.0/pycliwrapper.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      187 2023-05-26 07:43:10.000000 pycliwrapper-1.0/pycliwrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-26 07:43:10.000000 pycliwrapper-1.0/pycliwrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       13 2023-05-26 07:43:10.000000 pycliwrapper-1.0/pycliwrapper.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-26 07:43:10.692983 pycliwrapper-1.0/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      673 2023-05-26 07:42:35.000000 pycliwrapper-1.0/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:48:45.604865 pycliwrapper-1.1/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2472 2023-05-26 07:48:45.604865 pycliwrapper-1.1/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2053 2023-05-26 07:47:18.000000 pycliwrapper-1.1/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:48:45.604865 pycliwrapper-1.1/pycliwrapper/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2085 2023-05-26 07:40:09.000000 pycliwrapper-1.1/pycliwrapper/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-26 07:48:45.604865 pycliwrapper-1.1/pycliwrapper.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2472 2023-05-26 07:48:45.000000 pycliwrapper-1.1/pycliwrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      187 2023-05-26 07:48:45.000000 pycliwrapper-1.1/pycliwrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-26 07:48:45.000000 pycliwrapper-1.1/pycliwrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       13 2023-05-26 07:48:45.000000 pycliwrapper-1.1/pycliwrapper.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-26 07:48:45.604865 pycliwrapper-1.1/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      673 2023-05-26 07:47:47.000000 pycliwrapper-1.1/setup.py
```

### Comparing `pycliwrapper-1.0/pycliwrapper/__init__.py` & `pycliwrapper-1.1/pycliwrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pycliwrapper-1.0/setup.py` & `pycliwrapper-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = "1.0"
+__version__ = "1.1"
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
```


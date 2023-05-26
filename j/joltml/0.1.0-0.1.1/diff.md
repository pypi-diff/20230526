# Comparing `tmp/joltml-0.1.0.tar.gz` & `tmp/joltml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltml-0.1.0.tar", last modified: Tue Apr 18 13:52:47 2023, max compression
+gzip compressed data, was "joltml-0.1.1.tar", last modified: Fri May 26 06:52:54 2023, max compression
```

## Comparing `joltml-0.1.0.tar` & `joltml-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:52:47.041474 joltml-0.1.0/
--rw-rw-rw-   0        0        0       59 2023-04-18 13:14:57.000000 joltml-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 joltml-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-04-18 13:47:07.000000 joltml-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      101 2023-04-18 13:49:35.000000 joltml-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      393 2023-04-18 13:52:47.040471 joltml-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-18 13:52:28.000000 joltml-0.1.0/README.md
--rw-rw-rw-   0        0        0        5 2023-04-18 13:15:36.000000 joltml-0.1.0/VERSION
-drwxrwxrwx   0        0        0        0 2023-04-18 13:52:47.022216 joltml-0.1.0/joltml/
--rw-rw-rw-   0        0        0       73 2023-04-18 13:50:16.000000 joltml-0.1.0/joltml/__init__.py
--rw-rw-rw-   0        0        0       72 2023-04-04 00:49:25.000000 joltml-0.1.0/joltml/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-04-18 13:20:40.000000 joltml-0.1.0/joltml/cli.py
--rw-rw-rw-   0        0        0       21 2023-04-18 13:48:06.000000 joltml-0.1.0/joltml/jolt.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:52:47.039325 joltml-0.1.0/joltml.egg-info/
--rw-rw-rw-   0        0        0      393 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 13:52:46.000000 joltml-0.1.0/joltml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 13:52:47.041474 joltml-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-04-18 13:49:17.000000 joltml-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:54.106510 joltml-0.1.1/
+-rw-rw-rw-   0        0        0       66 2023-04-18 13:47:07.000000 joltml-0.1.1/.gitattributes
+-rw-rw-rw-   0        0        0     2938 2023-05-04 04:57:29.000000 joltml-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0      156 2023-05-26 06:52:17.000000 joltml-0.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 joltml-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-04-18 13:47:07.000000 joltml-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      108 2023-05-09 01:02:13.000000 joltml-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      495 2023-05-26 06:52:54.105522 joltml-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-05-24 02:20:35.000000 joltml-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:53.987014 joltml-0.1.1/examples/
+-rw-rw-rw-   0        0        0     7768 2023-05-26 06:52:17.000000 joltml-0.1.1/examples/demo.ipynb
+-rw-rw-rw-   0        0        0      841 2023-05-26 06:52:17.000000 joltml-0.1.1/examples/jolt.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:53.998592 joltml-0.1.1/examples/pytorch/
+-rw-rw-rw-   0        0        0      636 2023-05-24 02:19:13.000000 joltml-0.1.1/examples/pytorch/basic_demo.ipynb
+-rw-rw-rw-   0        0        0      256 2023-05-11 05:25:03.000000 joltml-0.1.1/examples/pytorch/transformer.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:54.049521 joltml-0.1.1/joltml/
+-rw-rw-rw-   0        0        0        5 2023-05-03 11:26:55.000000 joltml-0.1.1/joltml/VERSION
+-rw-rw-rw-   0        0        0      394 2023-05-09 07:51:10.000000 joltml-0.1.1/joltml/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 joltml-0.1.1/joltml/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-04-18 13:20:40.000000 joltml-0.1.1/joltml/cli.py
+-rw-rw-rw-   0        0        0     3471 2023-05-26 06:52:17.000000 joltml-0.1.1/joltml/experiment.py
+-rw-rw-rw-   0        0        0     7068 2023-05-26 06:52:17.000000 joltml-0.1.1/joltml/fit.py
+-rw-rw-rw-   0        0        0     1606 2023-05-09 12:18:19.000000 joltml-0.1.1/joltml/joltmeter.py
+-rw-rw-rw-   0        0        0       23 2023-05-06 12:49:30.000000 joltml-0.1.1/joltml/joltml.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:54.104508 joltml-0.1.1/joltml/model/
+-rw-rw-rw-   0        0        0     2352 2023-05-10 13:23:42.000000 joltml-0.1.1/joltml/model/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-09 06:53:43.000000 joltml-0.1.1/joltml/model/keras.py
+-rw-rw-rw-   0        0        0     4037 2023-05-26 06:52:17.000000 joltml-0.1.1/joltml/model/pytorch.py
+-rw-rw-rw-   0        0        0     1079 2023-05-09 06:08:57.000000 joltml-0.1.1/joltml/model/sklearn.py
+-rw-rw-rw-   0        0        0      173 2023-05-08 02:49:46.000000 joltml-0.1.1/joltml/model/statsmodel.py
+-rw-rw-rw-   0        0        0     2491 2023-05-24 12:22:21.000000 joltml-0.1.1/joltml/model/xgboost.py
+-rw-rw-rw-   0        0        0      142 2023-05-02 08:06:19.000000 joltml-0.1.1/joltml/status.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 joltml-0.1.1/joltml/version.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:52:54.067508 joltml-0.1.1/joltml.egg-info/
+-rw-rw-rw-   0        0        0      495 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       46 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 06:52:53.000000 joltml-0.1.1/joltml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:52:54.106510 joltml-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1150 2023-05-24 02:23:12.000000 joltml-0.1.1/setup.py
```

### Comparing `joltml-0.1.0/CONTRIBUTING.rst` & `joltml-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `joltml-0.1.0/LICENSE` & `joltml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joltml-0.1.0/joltml/cli.py` & `joltml-0.1.1/joltml/cli.py`

 * *Files identical despite different names*

### Comparing `joltml-0.1.0/setup.py` & `joltml-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 here = Path(__file__).resolve().parent
 README = (here / "README.md").read_text(encoding="utf-8")
-VERSION = (here / "VERSION").read_text(encoding="utf-8").strip()
+VERSION = (here / 'joltml' / "VERSION").read_text(encoding="utf-8").strip()
 
 setup(
     name='joltml',
     packages=['joltml',
               ] + find_packages(exclude=['tests', 'tests.*']),
     include_package_data=True,
     entry_points={
@@ -17,14 +17,17 @@
     license='mit',
     description='joltml unravels the dark side of machine learning models',
     long_description=README,
     long_description_content_type='text/markdown',
     author='Sherif Abdulkader Tawfik Abbas',
     author_email='sherif.tawfic@gmail.com',
     url='https://github.com/sheriftawfikabbas/joltml',
-    keywords=['ai', 'machine learning',
-              'model testing'],
+    keywords=['ai', 'machine learning', 'machine learning workflow'
+              'model tracking'],
     install_requires=['xgboost',
                       'pandas',
-                      'numpy'],
+                      'numpy',
+                      'torch',
+                      'tensorflow',
+                      'sklearn'],
 
 )
```


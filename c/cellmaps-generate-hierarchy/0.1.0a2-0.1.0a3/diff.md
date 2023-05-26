# Comparing `tmp/cellmaps_generate_hierarchy-0.1.0a2.tar.gz` & `tmp/cellmaps_generate_hierarchy-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a2.tar", last modified: Mon May 22 19:43:10 2023, max compression
+gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a3.tar", last modified: Fri May 26 18:12:10 2023, max compression
```

## Comparing `cellmaps_generate_hierarchy-0.1.0a2.tar` & `cellmaps_generate_hierarchy-0.1.0a3.tar`

### file list

```diff
@@ -1,50 +1,57 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.545096 cellmaps_generate_hierarchy-0.1.0a2/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a2/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6025 2023-05-22 19:43:10.545232 cellmaps_generate_hierarchy-0.1.0a2/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     3967 2023-05-19 20:14:40.000000 cellmaps_generate_hierarchy-0.1.0a2/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.535190 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/
--rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-22 19:42:33.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     5013 2023-05-19 20:29:56.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     1337 2023-05-11 18:25:18.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     3679 2023-05-11 18:16:55.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/ppi.py
--rw-r--r--   0 churas     (504) staff       (20)    10251 2023-05-22 19:38:02.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.537789 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6025 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1229 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-22 19:43:10.000000 cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.543460 cellmaps_generate_hierarchy-0.1.0a2/docs/
--rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/Makefile
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/authors.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-22 19:43:10.545660 cellmaps_generate_hierarchy-0.1.0a2/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-19 20:12:33.000000 cellmaps_generate_hierarchy-0.1.0a2/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.544686 cellmaps_generate_hierarchy-0.1.0a2/tests/
--rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-22 19:43:10.544909 cellmaps_generate_hierarchy-0.1.0a2/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/data/fake_4_node_coembedding.tsv
--rw-r--r--   0 churas     (504) staff       (20)     1182 2023-05-11 00:02:02.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/test_cdapshierarchygenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/test_cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/test_cellmapsgeneratehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/test_cosinesimilarityppigenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a2/tests/test_integration_cellmaps_generate_hierarchy.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917830 cellmaps_generate_hierarchy-0.1.0a3/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a3/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-26 18:12:10.917994 cellmaps_generate_hierarchy-0.1.0a3/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-25 22:06:47.000000 cellmaps_generate_hierarchy-0.1.0a3/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.909363 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/
+-rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-25 22:56:56.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     5400 2023-05-26 17:59:09.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    17269 2023-05-26 18:04:18.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-25 21:26:59.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/ppi.py
+-rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:09:44.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.910874 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1369 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.914943 cellmaps_generate_hierarchy-0.1.0a3/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.903726 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.903827 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.915724 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/cellmaps_generate_hierarchy.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-26 18:12:10.918537 cellmaps_generate_hierarchy-0.1.0a3/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a3/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917324 cellmaps_generate_hierarchy-0.1.0a3/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917595 cellmaps_generate_hierarchy-0.1.0a3/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/data/fake_4_node_coembedding.tsv
+-rw-r--r--   0 churas     (504) staff       (20)     1182 2023-05-11 00:02:02.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cdapshierarchygenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmapsgeneratehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cosinesimilarityppigenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_integration_cellmaps_generate_hierarchy.py
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/CONTRIBUTING.rst` & `cellmaps_generate_hierarchy-0.1.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/LICENSE` & `cellmaps_generate_hierarchy-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_generate_hierarchy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
@@ -32,15 +32,26 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `cdapsutil <https://pypi.org/project/cdapsutil>`__
+        * `HiDef <https://github.com/fanzheng10/HiDeF>`__
+           HiDef must be built directly from source which can be done by running the following commands:
+        
+          .. code-block:: python
+        
+            git clone https://github.com/fanzheng10/HiDeF.git
+            cd HiDeF
+            make dist
+            pip install dist/hidef*whl
+        
+        
+        
         
         Compatibility
         -------------
         
         * Python 3.8+
         
         Installation
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/README.rst` & `cellmaps_generate_hierarchy-0.1.0a3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,26 @@
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 * `pandas <https://pypi.org/project/pandas>`__
 * `numpy <https://pypi.org/project/numpy>`__
 * `ndex2 <https://pypi.org/project/ndex2>`__
-* `cdapsutil <https://pypi.org/project/cdapsutil>`__
+* `HiDef <https://github.com/fanzheng10/HiDeF>`__
+   HiDef must be built directly from source which can be done by running the following commands:
+
+  .. code-block:: python
+
+    git clone https://github.com/fanzheng10/HiDeF.git
+    cd HiDeF
+    make dist
+    pip install dist/hidef*whl
+
+
+
 
 Compatibility
 -------------
 
 * Python 3.8+
 
 Installation
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import argparse
 import sys
 import logging
 import logging.config
 
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
+from cellmaps_utils.provenance import ProvenanceUtil
 import cellmaps_generate_hierarchy
 from cellmaps_generate_hierarchy.ppi import CosineSimilarityPPIGenerator
-from cellmaps_generate_hierarchy.hierarchy import CDAPSHierarchyGenerator
+from cellmaps_generate_hierarchy.hierarchy import CDAPSHiDeFHierarchyGenerator
 from cellmaps_generate_hierarchy.runner import CellmapsGenerateHierarchy
 
 logger = logging.getLogger(__name__)
 
 
 CO_EMBEDDINGDIR='--coembedding_dir'
 
@@ -99,23 +100,26 @@
                coembedding_dir=CO_EMBEDDINGDIR)
     theargs = _parse_arguments(desc, args[1:])
     theargs.program = args[0]
     theargs.version = cellmaps_generate_hierarchy.__version__
 
     try:
         logutils.setup_cmd_logging(theargs)
-
+        provenance = ProvenanceUtil()
         ppigen = CosineSimilarityPPIGenerator(embeddingdir=theargs.coembedding_dir)
 
-        hiergen = CDAPSHierarchyGenerator()
+        hiergen = CDAPSHiDeFHierarchyGenerator(author=cellmaps_generate_hierarchy.__author__,
+                                               version=cellmaps_generate_hierarchy.__version__,
+                                               provenance_utils=provenance)
         return CellmapsGenerateHierarchy(outdir=theargs.outdir,
                                          inputdir=theargs.coembedding_dir,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
-                                         input_data_dict=theargs.__dict__).run()
+                                         input_data_dict=theargs.__dict__,
+                                         provenance_utils=provenance).run()
     except Exception as e:
         logger.exception('Caught exception: ' + str(e))
         return 2
     finally:
         logging.shutdown()
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/ppi.py` & `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/ppi.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     .. code-block::
 
         ID # # # #
 
     Where ID is gene and #'s is embedding vector
     """
     def __init__(self, embeddingdir=None,
-                 cutoffs=[0.01]):
+                 cutoffs=[0.001, 0.002, 0.005, 0.01, 0.02, 0.05]):
         """
         Constructor
         """
         super().__init__()
         if embeddingdir is None:
             raise CellmapsGenerateHierarchyError('embeddingdir is None')
 
@@ -89,13 +89,14 @@
                                                    target_field=constants.PPI_EDGELIST_GENEB_COL,
                                                    edge_attr=[constants.WEIGHTED_PPI_EDGELIST_WEIGHT_COL])
             net.set_name('cellmaps_generate_hierarchy PPI ' + str(cutoff) + ' cutoff')
             net.set_network_attribute(name='description',
                                       values='Protein to Protein Interaction\n'
                                              'network generated by cellmaps_generate_hierarchy\n'
                                              'tool from embedding XXX where top ' +
-                                             str(round(cutoff*100.0)) + '% of interactions sorted by\n')
+                                             str(round(cutoff*100.0)) +
+                                             '% of interactions sorted by weight\n')
             net.set_network_attribute(name='cutoff', values=str(cutoff))
             #             # Todo add generated by
             #  author and other information
             yield net
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy/runner.py` & `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                                                                     author=cellmaps_generate_hierarchy.__author__,
                                                                     version=cellmaps_generate_hierarchy.__version__,
                                                                     file_format='.py',
                                                                     url=cellmaps_generate_hierarchy.__repo_url__)
 
     def _register_computation(self, generated_dataset_ids=[]):
         """
-        # Todo: added inused dataset, software and what is being generated
+        # Todo: added in used dataset, software and what is being generated
         :return:
         """
         logger.debug('Getting id of input rocrate')
         input_dataset_id = self._provenance_utils.get_id_of_rocrate(self._inputdir)
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_generate_hierarchy.__name__ + ' computation',
                                                     run_by=str(self._provenance_utils.get_login()),
@@ -122,35 +122,107 @@
         :param ppi_network: PPI Network
         :type ppi_network: :py:class:`ndex2.nice_cx_network.NiceCXNetwork`
         :return: Path on filesystem to write the PPI network
         :rtype: str
         """
         cutoff = ppi_network.get_network_attribute('cutoff')['v']
         return os.path.join(self._outdir, constants.PPI_NETWORK_PREFIX +
-                            '_cutoff_' + str(cutoff) + constants.CX_SUFFIX)
+                            '_cutoff_' + str(cutoff))
 
     def get_hierarchy_dest_file(self, hierarchy):
         """
-        Gets the path where the hierarchy should be written to.
-        Current implementation appends `_#cutoff` to filename
-        where `#` is the cutoff value used in making the PPI network
+        Creates file path prefix for hierarchy
+
+        Example path: ``/tmp/foo/hierarchy``
 
         :param hierarchy: Hierarchy Network
         :type hierarchy: :py:class:`ndex2.nice_cx_network.NiceCXNetwork`
-        :return: Path on filesystem to write Hierarchy Network
+        :return: Prefix path on filesystem to write Hierarchy Network
         :rtype: str
         """
-        cutoff = 'unknown'
-        try:
-            cutoff = hierarchy.get_network_attribute('cutoff')['v']
-        except Exception as e:
-            logger.error('Unable to get cutoff from hierarchy network ' + str(e))
+        return os.path.join(self._outdir, constants.HIERARCHY_NETWORK_PREFIX)
+
+    def _write_and_register_ppi_network_as_cx(self, ppi_network, dest_path=None):
+        """
+
+        :param network:
+        :return:
+        """
+        logger.debug('Writing PPI network ' + str(ppi_network.get_name()))
+        # write PPI to filesystem
 
-        return os.path.join(self._outdir, constants.HIERARCHY_NETWORK_PREFIX +
-                            '_cutoff_' + str(cutoff) + constants.CX_SUFFIX)
+        with open(dest_path, 'w') as f:
+            json.dump(ppi_network.to_cx(), f)
+
+        # register ppi network file with fairscape
+        data_dict = {'name': os.path.basename(dest_path) + ' PPI network file',
+                     'description': 'PPI Network file',
+                     'data-format': 'CX',
+                     'author': cellmaps_generate_hierarchy.__name__,
+                     'version': cellmaps_generate_hierarchy.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        return self._provenance_utils.register_dataset(self._outdir,
+                                                       source_file=dest_path,
+                                                       data_dict=data_dict)
+
+    def _write_and_register_ppi_network_as_edgelist(self, ppi_network, dest_path=None):
+        """
+        Writes out **ppi_network** passed in as edge list file
+
+        :param ppi_network:
+        :type ppi_network: :py:class:`~ndex2.nice_cx_network.NiceCXNetwork`
+        :return: (dataset id, path to output file)
+        :rtype: tuple
+        """
+        logger.debug('Writing PPI network ' + str(ppi_network.get_name()))
+
+        # build dict of node ids to gene names
+        name_dict = {}
+        for node_id, node_obj in ppi_network.get_nodes():
+            name_dict[node_id] = node_obj['n']
+
+        # write PPI to filesystem
+        with open(dest_path, 'w') as f:
+            for edge_id, edge_obj in ppi_network.get_edges():
+                # todo get weight
+                f.write(name_dict[edge_obj['s']] + '\t' + str(name_dict[edge_obj['t']]) + '\n')
+
+        # register ppi network file with fairscape
+        data_dict = {'name': os.path.basename(dest_path) + ' PPI edgelist file',
+                     'description': 'PPI Edgelist file',
+                     'data-format': 'tsv',
+                     'author': cellmaps_generate_hierarchy.__name__,
+                     'version': cellmaps_generate_hierarchy.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        dataset_id = self._provenance_utils.register_dataset(self._outdir,
+                                                             source_file=dest_path,
+                                                             data_dict=data_dict)
+        return dataset_id
+
+    def _write_and_register_hierarchy_network(self, hierarchy):
+        """
+
+        :param network:
+        :return:
+        """
+        logger.debug('Writing hierarchy')
+        hierarchy_out_file = self.get_hierarchy_dest_file(hierarchy) + constants.CX_SUFFIX
+        with open(hierarchy_out_file, 'w') as f:
+            json.dump(hierarchy.to_cx(), f)
+            # register ppi network file with fairscape
+            data_dict = {'name': os.path.basename(hierarchy_out_file) + ' Hierarchy network file',
+                         'description': 'Hierarchy network file',
+                         'data-format': 'CX',
+                         'author': cellmaps_generate_hierarchy.__name__,
+                         'version': cellmaps_generate_hierarchy.__version__,
+                         'date-published': date.today().strftime('%m-%d-%Y')}
+            dataset_id = self._provenance_utils.register_dataset(self._outdir,
+                                                                 source_file=hierarchy_out_file,
+                                                                 data_dict=data_dict)
+        return dataset_id, hierarchy_out_file
 
     def run(self):
         """
         Runs CM4AI Generate Hierarchy
 
 
         :return:
@@ -171,51 +243,36 @@
                                            start_time=self._start_time,
                                            data={'commandlineargs': self._input_data_dict},
                                            version=cellmaps_generate_hierarchy.__version__)
 
             self._create_rocrate()
 
             self._register_software()
+
             generated_dataset_ids = []
+            ppi_network_prefix_paths = []
+            # generate PPI networks
             for ppi_network in tqdm(self._ppigen.get_next_network(), desc='Generating hierarchy'):
+                dest_prefix = self.get_ppi_network_dest_file(ppi_network)
+                ppi_network_prefix_paths.append(dest_prefix)
+                cx_path = dest_prefix + constants.CX_SUFFIX
+                generated_dataset_ids.append(self._write_and_register_ppi_network_as_cx(ppi_network,
+                                                                                        dest_path=cx_path))
+
+            # generate hierarchy
+            hierarchy = self._hiergen.get_hierarchy(ppi_network_prefix_paths)
+
+            # write out hierarchy
+            dataset_id, hierarchy_out_file = self._write_and_register_hierarchy_network(hierarchy)
+            generated_dataset_ids.append(dataset_id)
 
-                logger.debug('Writing PPI network ' + str(ppi_network.get_name()))
-                # write PPI to filesystem
-                ppi_out_file = self.get_ppi_network_dest_file(ppi_network)
-                with open(ppi_out_file, 'w') as f:
-                    json.dump(ppi_network.to_cx(), f)
-
-                # register ppi network file with fairscape
-                data_dict = {'name': os.path.basename(ppi_out_file) + ' PPI network file',
-                             'description': 'PPI Network file',
-                             'data-format': 'CX',
-                             'author': cellmaps_generate_hierarchy.__name__,
-                             'version': cellmaps_generate_hierarchy.__version__,
-                             'date-published': date.today().strftime('%m-%d-%Y')}
-                generated_dataset_ids.append(self._provenance_utils.register_dataset(self._outdir,
-                                                                                     source_file=ppi_out_file,
-                                                                                     data_dict=data_dict))
-
-                # generate hierarchy
-                logger.info('Creating hierarchy')
-                hierarchy = self._hiergen.get_hierarchy(ppi_network)
-                hierarchy_out_file = self.get_hierarchy_dest_file(hierarchy)
-                with open(hierarchy_out_file, 'w') as f:
-                    json.dump(hierarchy.to_cx(), f)
-                    # register ppi network file with fairscape
-                    data_dict = {'name': os.path.basename(hierarchy_out_file) + ' Hierarchy network file',
-                                 'description': 'Hierarchy network file',
-                                 'data-format': 'CX',
-                                 'author': cellmaps_generate_hierarchy.__name__,
-                                 'version': cellmaps_generate_hierarchy.__version__,
-                                 'date-published': date.today().strftime('%m-%d-%Y')}
-                    generated_dataset_ids.append(self._provenance_utils.register_dataset(self._outdir,
-                                                                                         source_file=hierarchy_out_file,
-                                                                                         data_dict=data_dict))
+            # add datasets created by hiergen object
+            generated_dataset_ids.extend(self._hiergen.get_generated_dataset_ids())
 
+            # register generated datasets
             self._register_computation(generated_dataset_ids=generated_dataset_ids)
             exitcode = 0
         finally:
             logutils.write_task_finish_json(outdir=self._outdir,
                                             start_time=self._start_time,
                                             status=exitcode)
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-generate-hierarchy
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
@@ -32,15 +32,26 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `cdapsutil <https://pypi.org/project/cdapsutil>`__
+        * `HiDef <https://github.com/fanzheng10/HiDeF>`__
+           HiDef must be built directly from source which can be done by running the following commands:
+        
+          .. code-block:: python
+        
+            git clone https://github.com/fanzheng10/HiDeF.git
+            cd HiDeF
+            make dist
+            pip install dist/hidef*whl
+        
+        
+        
         
         Compatibility
         -------------
         
         * Python 3.8+
         
         Installation
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/cellmaps_generate_hierarchy.egg-info/SOURCES.txt` & `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,32 @@
 cellmaps_generate_hierarchy.egg-info/SOURCES.txt
 cellmaps_generate_hierarchy.egg-info/dependency_links.txt
 cellmaps_generate_hierarchy.egg-info/not-zip-safe
 cellmaps_generate_hierarchy.egg-info/requires.txt
 cellmaps_generate_hierarchy.egg-info/top_level.txt
 docs/Makefile
 docs/authors.rst
+docs/cellmaps_generate_hierarchy.rst
 docs/conf.py
 docs/contributing.rst
 docs/devbranches.rst
 docs/developer.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/integrationtesting.rst
 docs/make.bat
 docs/modules.rst
 docs/newrelease.rst
 docs/pypircfile.rst
 docs/usage.rst
 docs/versioningscheme.rst
+docs/_build/html/_static/file.png
+docs/_build/html/_static/minus.png
+docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cdapshierarchygenerator.py
 tests/test_cellmaps_generate_hierarchycmd.py
 tests/test_cellmapsgeneratehierarchy.py
 tests/test_cosinesimilarityppigenerator.py
 tests/test_integration_cellmaps_generate_hierarchy.py
 tests/data/fake_4_node_coembedding.tsv
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/Makefile` & `cellmaps_generate_hierarchy-0.1.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/conf.py` & `cellmaps_generate_hierarchy-0.1.0a3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/index.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/installation.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/make.bat` & `cellmaps_generate_hierarchy-0.1.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/newrelease.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/pypircfile.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/usage.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/docs/versioningscheme.rst` & `cellmaps_generate_hierarchy-0.1.0a3/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/setup.py` & `cellmaps_generate_hierarchy-0.1.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/data/fake_4_node_coembedding.tsv` & `cellmaps_generate_hierarchy-0.1.0a3/tests/data/fake_4_node_coembedding.tsv`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/test_cdapshierarchygenerator.py` & `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cdapshierarchygenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/test_cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmaps_generate_hierarchycmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/test_cellmapsgeneratehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmapsgeneratehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/test_cosinesimilarityppigenerator.py` & `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cosinesimilarityppigenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a2/tests/test_integration_cellmaps_generate_hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a3/tests/test_integration_cellmaps_generate_hierarchy.py`

 * *Files identical despite different names*


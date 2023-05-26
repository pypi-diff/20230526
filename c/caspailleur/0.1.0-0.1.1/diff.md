# Comparing `tmp/caspailleur-0.1.0.tar.gz` & `tmp/caspailleur-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caspailleur-0.1.0.tar", last modified: Fri May 26 18:01:24 2023, max compression
+gzip compressed data, was "caspailleur-0.1.1.tar", last modified: Fri May 26 18:15:04 2023, max compression
```

## Comparing `caspailleur-0.1.0.tar` & `caspailleur-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:01:24.435217 caspailleur-0.1.0/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    35149 2023-04-11 14:13:18.000000 caspailleur-0.1.0/LICENSE
--rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:01:24.435069 caspailleur-0.1.0/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)    11966 2023-05-26 17:59:35.000000 caspailleur-0.1.0/README.md
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:01:24.433260 caspailleur-0.1.0/caspailleur/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      455 2023-05-26 17:59:35.000000 caspailleur-0.1.0/caspailleur/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4096 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/base_functions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4202 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/definitions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6900 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/implication_bases.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3905 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/indices.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7027 2023-05-25 13:00:43.000000 caspailleur-0.1.0/caspailleur/mine_equivalence_classes.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2386 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/orchestrator.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     5982 2023-04-11 14:13:18.000000 caspailleur-0.1.0/caspailleur/order.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:01:24.433874 caspailleur-0.1.0/caspailleur.egg-info/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:01:24.000000 caspailleur-0.1.0/caspailleur.egg-info/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)      605 2023-05-26 18:01:24.000000 caspailleur-0.1.0/caspailleur.egg-info/SOURCES.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-05-26 18:01:24.000000 caspailleur-0.1.0/caspailleur.egg-info/dependency_links.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)       53 2023-05-26 18:01:24.000000 caspailleur-0.1.0/caspailleur.egg-info/requires.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)       12 2023-05-26 18:01:24.000000 caspailleur-0.1.0/caspailleur.egg-info/top_level.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)      833 2023-05-26 17:59:35.000000 caspailleur-0.1.0/pyproject.toml
--rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-05-26 18:01:24.435251 caspailleur-0.1.0/setup.cfg
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:01:24.434816 caspailleur-0.1.0/tests/
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2769 2023-04-11 14:13:18.000000 caspailleur-0.1.0/tests/test_base_functions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4679 2023-04-11 14:13:18.000000 caspailleur-0.1.0/tests/test_definitions.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1423 2023-04-11 14:13:18.000000 caspailleur-0.1.0/tests/test_implication_bases.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3840 2023-05-25 13:00:43.000000 caspailleur-0.1.0/tests/test_mine_equivalence_classes.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2859 2023-04-11 14:13:18.000000 caspailleur-0.1.0/tests/test_orchestrator.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2334 2023-04-11 14:13:18.000000 caspailleur-0.1.0/tests/test_order.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.964982 caspailleur-0.1.1/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35149 2023-04-11 14:13:18.000000 caspailleur-0.1.1/LICENSE
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:15:04.964853 caspailleur-0.1.1/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    11966 2023-05-26 17:59:35.000000 caspailleur-0.1.1/README.md
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.962882 caspailleur-0.1.1/caspailleur/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      401 2023-05-26 18:09:18.000000 caspailleur-0.1.1/caspailleur/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4096 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/base_functions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4202 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/definitions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6900 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/implication_bases.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3905 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/indices.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7027 2023-05-25 13:00:43.000000 caspailleur-0.1.1/caspailleur/mine_equivalence_classes.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2386 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/orchestrator.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5982 2023-04-11 14:13:18.000000 caspailleur-0.1.1/caspailleur/order.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.963583 caspailleur-0.1.1/caspailleur.egg-info/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    53111 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      605 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/SOURCES.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/dependency_links.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       48 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/requires.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       12 2023-05-26 18:15:04.000000 caspailleur-0.1.1/caspailleur.egg-info/top_level.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      825 2023-05-26 18:14:49.000000 caspailleur-0.1.1/pyproject.toml
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-05-26 18:15:04.965017 caspailleur-0.1.1/setup.cfg
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-05-26 18:15:04.964600 caspailleur-0.1.1/tests/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2769 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_base_functions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4679 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_definitions.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1423 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_implication_bases.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3840 2023-05-25 13:00:43.000000 caspailleur-0.1.1/tests/test_mine_equivalence_classes.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2859 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_orchestrator.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2334 2023-04-11 14:13:18.000000 caspailleur-0.1.1/tests/test_order.py
```

### Comparing `caspailleur-0.1.0/LICENSE` & `caspailleur-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/PKG-INFO` & `caspailleur-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caspailleur
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minimalistic python package for mining many concise data representations. Part of SmartFCA project
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `caspailleur-0.1.0/README.md` & `caspailleur-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/base_functions.py` & `caspailleur-0.1.1/caspailleur/base_functions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/definitions.py` & `caspailleur-0.1.1/caspailleur/definitions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/implication_bases.py` & `caspailleur-0.1.1/caspailleur/implication_bases.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/indices.py` & `caspailleur-0.1.1/caspailleur/indices.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/mine_equivalence_classes.py` & `caspailleur-0.1.1/caspailleur/mine_equivalence_classes.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/orchestrator.py` & `caspailleur-0.1.1/caspailleur/orchestrator.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur/order.py` & `caspailleur-0.1.1/caspailleur/order.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/caspailleur.egg-info/PKG-INFO` & `caspailleur-0.1.1/caspailleur.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caspailleur
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minimalistic python package for mining many concise data representations. Part of SmartFCA project
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `caspailleur-0.1.0/caspailleur.egg-info/SOURCES.txt` & `caspailleur-0.1.1/caspailleur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/pyproject.toml` & `caspailleur-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "caspailleur"
-version = "0.1.0"
+version = "0.1.1"
 description = "Minimalistic python package for mining many concise data representations. Part of SmartFCA project"
 readme = "README.md"
 authors = [{ name = "Egor Dudyrev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 keywords = ["python", "fca", "itemset-mining"]
 dependencies = [
-    'numpy>=1.20', 'scikit-mine>=1', 'bitarray>=2.5.1', 'tqdm', 'toml',
+    'numpy>=1.20', 'scikit-mine>=1', 'bitarray>=2.5.1', 'tqdm',
 ]
 requires-python = ">=3.8"
 
 
 [project.urls]
 Homepage = "https://github.com/EgorDudyrev/caspailleur"
```

### Comparing `caspailleur-0.1.0/tests/test_base_functions.py` & `caspailleur-0.1.1/tests/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/tests/test_definitions.py` & `caspailleur-0.1.1/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/tests/test_implication_bases.py` & `caspailleur-0.1.1/tests/test_implication_bases.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/tests/test_mine_equivalence_classes.py` & `caspailleur-0.1.1/tests/test_mine_equivalence_classes.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/tests/test_orchestrator.py` & `caspailleur-0.1.1/tests/test_orchestrator.py`

 * *Files identical despite different names*

### Comparing `caspailleur-0.1.0/tests/test_order.py` & `caspailleur-0.1.1/tests/test_order.py`

 * *Files identical despite different names*


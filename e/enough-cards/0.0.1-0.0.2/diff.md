# Comparing `tmp/enough_cards-0.0.1.tar.gz` & `tmp/enough_cards-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enough_cards-0.0.1.tar", last modified: Fri May 26 16:41:28 2023, max compression
+gzip compressed data, was "enough_cards-0.0.2.tar", last modified: Fri May 26 16:52:33 2023, max compression
```

## Comparing `enough_cards-0.0.1.tar` & `enough_cards-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:41:28.358815 enough_cards-0.0.1/
--rw-r--r--   0 frank      (501) staff       (20)    11357 2023-05-25 20:32:03.000000 enough_cards-0.0.1/LICENSE
--rw-rw-r--   0 frank      (501) staff       (20)      111 2023-04-27 10:12:58.000000 enough_cards-0.0.1/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)     1143 2023-05-26 16:41:28.358689 enough_cards-0.0.1/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      343 2023-05-26 16:29:23.000000 enough_cards-0.0.1/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:41:28.357063 enough_cards-0.0.1/enough_cards/
--rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 16:41:05.000000 enough_cards-0.0.1/enough_cards/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)     2068 2023-05-26 16:41:05.000000 enough_cards-0.0.1/enough_cards/_modidx.py
--rw-r--r--   0 frank      (501) staff       (20)      994 2023-05-26 16:41:05.000000 enough_cards-0.0.1/enough_cards/card.py
--rw-r--r--   0 frank      (501) staff       (20)     1350 2023-05-26 16:41:05.000000 enough_cards-0.0.1/enough_cards/deck.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:41:28.357937 enough_cards-0.0.1/enough_cards.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)     1143 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      498 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)       46 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 16:41:10.000000 enough_cards-0.0.1/enough_cards.egg-info/not-zip-safe
--rw-r--r--   0 frank      (501) staff       (20)        7 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       29 2023-05-26 16:41:28.000000 enough_cards-0.0.1/enough_cards.egg-info/top_level.txt
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:41:28.358420 enough_cards-0.0.1/nbdev_cards/
--rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 16:30:05.000000 enough_cards-0.0.1/nbdev_cards/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)     2020 2023-05-26 16:30:05.000000 enough_cards-0.0.1/nbdev_cards/_modidx.py
--rw-r--r--   0 frank      (501) staff       (20)      994 2023-05-26 16:30:05.000000 enough_cards-0.0.1/nbdev_cards/card.py
--rw-r--r--   0 frank      (501) staff       (20)     1339 2023-05-26 16:30:05.000000 enough_cards-0.0.1/nbdev_cards/deck.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:41:28.358533 enough_cards-0.0.1/nbs/
--rw-r--r--   0 frank      (501) staff       (20)        0 2023-05-26 09:16:44.000000 enough_cards-0.0.1/nbs/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      981 2023-05-26 16:40:44.000000 enough_cards-0.0.1/settings.ini
--rw-r--r--   0 frank      (501) staff       (20)       38 2023-05-26 16:41:28.358850 enough_cards-0.0.1/setup.cfg
--rw-rw-r--   0 frank      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 enough_cards-0.0.1/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:52:33.702577 enough_cards-0.0.2/
+-rw-r--r--   0 frank      (501) staff       (20)    11357 2023-05-25 20:32:03.000000 enough_cards-0.0.2/LICENSE
+-rw-rw-r--   0 frank      (501) staff       (20)      111 2023-04-27 10:12:58.000000 enough_cards-0.0.2/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)     1143 2023-05-26 16:52:33.702456 enough_cards-0.0.2/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      343 2023-05-26 16:47:36.000000 enough_cards-0.0.2/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:52:33.700876 enough_cards-0.0.2/enough_cards/
+-rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 16:48:40.000000 enough_cards-0.0.2/enough_cards/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)     2068 2023-05-26 16:48:40.000000 enough_cards-0.0.2/enough_cards/_modidx.py
+-rw-r--r--   0 frank      (501) staff       (20)      994 2023-05-26 16:48:40.000000 enough_cards-0.0.2/enough_cards/card.py
+-rw-r--r--   0 frank      (501) staff       (20)     1339 2023-05-26 16:48:40.000000 enough_cards-0.0.2/enough_cards/deck.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:52:33.701670 enough_cards-0.0.2/enough_cards.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)     1143 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      498 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)       46 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2023-05-26 16:41:10.000000 enough_cards-0.0.2/enough_cards.egg-info/not-zip-safe
+-rw-r--r--   0 frank      (501) staff       (20)        7 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       29 2023-05-26 16:52:33.000000 enough_cards-0.0.2/enough_cards.egg-info/top_level.txt
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:52:33.702153 enough_cards-0.0.2/nbdev_cards/
+-rw-r--r--   0 frank      (501) staff       (20)       22 2023-05-26 16:30:05.000000 enough_cards-0.0.2/nbdev_cards/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)     2055 2023-05-26 16:47:38.000000 enough_cards-0.0.2/nbdev_cards/_modidx.py
+-rw-r--r--   0 frank      (501) staff       (20)      994 2023-05-26 16:30:05.000000 enough_cards-0.0.2/nbdev_cards/card.py
+-rw-r--r--   0 frank      (501) staff       (20)     1339 2023-05-26 16:30:05.000000 enough_cards-0.0.2/nbdev_cards/deck.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-05-26 16:52:33.702295 enough_cards-0.0.2/nbs/
+-rw-r--r--   0 frank      (501) staff       (20)        0 2023-05-26 09:16:44.000000 enough_cards-0.0.2/nbs/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      982 2023-05-26 16:52:31.000000 enough_cards-0.0.2/settings.ini
+-rw-r--r--   0 frank      (501) staff       (20)       38 2023-05-26 16:52:33.702614 enough_cards-0.0.2/setup.cfg
+-rw-rw-r--   0 frank      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 enough_cards-0.0.2/setup.py
```

### Comparing `enough_cards-0.0.1/LICENSE` & `enough_cards-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enough_cards-0.0.1/PKG-INFO` & `enough_cards-0.0.2/enough_cards.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enough_cards
-Version: 0.0.1
+Name: enough-cards
+Version: 0.0.2
 Summary: A sample of how to create a deck of cards lib using nbdev
 Home-page: https://github.com/genughaben/enough_cards
 Author: Frank Wolf
 Author-email: fwolf@posteo.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,34 +16,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# nbdev_cards
+# enough_cards
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
-``` sh
-pip install nbdev_cards
+```sh
+pip install enough_cards
 ```
 
 ## How to use
 
 The lib
-[`Card`](https://genughaben.github.io/nbdev_cards/card.html#card) helps
+[`Card`](https://genughaben.github.io/enough_cards/card.html#card) helps
 to create and compare playing cards
 
-``` python
+```python
 Card(1,2)
 ```
 
     ♠️2
 
-``` python
+```python
 Card(1,2) < Card(1,1)
 ```
 
     False
```

### Comparing `enough_cards-0.0.1/enough_cards/_modidx.py` & `enough_cards-0.0.2/enough_cards/_modidx.py`

 * *Files identical despite different names*

### Comparing `enough_cards-0.0.1/enough_cards/card.py` & `enough_cards-0.0.2/enough_cards/card.py`

 * *Files identical despite different names*

### Comparing `enough_cards-0.0.1/enough_cards/deck.py` & `enough_cards-0.0.2/enough_cards/deck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_deck.ipynb.
 
 # %% auto 0
 __all__ = ['Deck']
 
 # %% ../nbs/01_deck.ipynb 2
 import random
-from nbdev_cards.card import *
+from .card import *
 from fastcore.utils import *
 
 # %% ../nbs/01_deck.ipynb 4
 class Deck:
     'A deck of 52 cards'
     def __init__(self):
         self.cards = [Card(s, r) for s in range(4) for r in range(2,15)]
```

### Comparing `enough_cards-0.0.1/enough_cards.egg-info/PKG-INFO` & `enough_cards-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enough-cards
-Version: 0.0.1
+Name: enough_cards
+Version: 0.0.2
 Summary: A sample of how to create a deck of cards lib using nbdev
 Home-page: https://github.com/genughaben/enough_cards
 Author: Frank Wolf
 Author-email: fwolf@posteo.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,34 +16,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# nbdev_cards
+# enough_cards
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
 
-``` sh
-pip install nbdev_cards
+```sh
+pip install enough_cards
 ```
 
 ## How to use
 
 The lib
-[`Card`](https://genughaben.github.io/nbdev_cards/card.html#card) helps
+[`Card`](https://genughaben.github.io/enough_cards/card.html#card) helps
 to create and compare playing cards
 
-``` python
+```python
 Card(1,2)
 ```
 
     ♠️2
 
-``` python
+```python
 Card(1,2) < Card(1,1)
 ```
 
     False
```

### Comparing `enough_cards-0.0.1/nbdev_cards/_modidx.py` & `enough_cards-0.0.2/nbdev_cards/_modidx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
-                'doc_baseurl': '/nbdev_cards',
+                'doc_baseurl': '/enough_cards',
                 'doc_host': 'https://genughaben.github.io',
-                'git_url': 'https://github.com/genughaben/nbdev_cards',
-                'lib_path': 'nbdev_cards'},
-  'syms': { 'nbdev_cards.card': { 'nbdev_cards.card.Card': ('card.html#card', 'nbdev_cards/card.py'),
-                                  'nbdev_cards.card.Card.__eq__': ('card.html#card.__eq__', 'nbdev_cards/card.py'),
-                                  'nbdev_cards.card.Card.__gt__': ('card.html#card.__gt__', 'nbdev_cards/card.py'),
-                                  'nbdev_cards.card.Card.__init__': ('card.html#card.__init__', 'nbdev_cards/card.py'),
-                                  'nbdev_cards.card.Card.__lt__': ('card.html#card.__lt__', 'nbdev_cards/card.py'),
-                                  'nbdev_cards.card.Card.__str__': ('card.html#card.__str__', 'nbdev_cards/card.py')},
-            'nbdev_cards.deck': { 'nbdev_cards.deck.Deck': ('deck.html#deck', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.__contains__': ('deck.html#deck.__contains__', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.__init__': ('deck.html#deck.__init__', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.__len__': ('deck.html#deck.__len__', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.__str__': ('deck.html#deck.__str__', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.draw': ('deck.html#deck.draw', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.pop': ('deck.html#deck.pop', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.remove': ('deck.html#deck.remove', 'nbdev_cards/deck.py'),
-                                  'nbdev_cards.deck.Deck.shuffle': ('deck.html#deck.shuffle', 'nbdev_cards/deck.py')}}}
+                'git_url': 'https://github.com/genughaben/enough_cards',
+                'lib_path': 'enough_cards'},
+  'syms': { 'enough_cards.card': { 'enough_cards.card.Card': ('card.html#card', 'enough_cards/card.py'),
+                                  'enough_cards.card.Card.__eq__': ('card.html#card.__eq__', 'enough_cards/card.py'),
+                                  'enough_cards.card.Card.__gt__': ('card.html#card.__gt__', 'enough_cards/card.py'),
+                                  'enough_cards.card.Card.__init__': ('card.html#card.__init__', 'enough_cards/card.py'),
+                                  'enough_cards.card.Card.__lt__': ('card.html#card.__lt__', 'enough_cards/card.py'),
+                                  'enough_cards.card.Card.__str__': ('card.html#card.__str__', 'enough_cards/card.py')},
+            'enough_cards.deck': { 'enough_cards.deck.Deck': ('deck.html#deck', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.__contains__': ('deck.html#deck.__contains__', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.__init__': ('deck.html#deck.__init__', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.__len__': ('deck.html#deck.__len__', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.__str__': ('deck.html#deck.__str__', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.draw': ('deck.html#deck.draw', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.pop': ('deck.html#deck.pop', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.remove': ('deck.html#deck.remove', 'enough_cards/deck.py'),
+                                  'enough_cards.deck.Deck.shuffle': ('deck.html#deck.shuffle', 'enough_cards/deck.py')}}}
```

### Comparing `enough_cards-0.0.1/nbdev_cards/card.py` & `enough_cards-0.0.2/nbdev_cards/card.py`

 * *Files identical despite different names*

### Comparing `enough_cards-0.0.1/nbdev_cards/deck.py` & `enough_cards-0.0.2/nbdev_cards/deck.py`

 * *Files identical despite different names*

### Comparing `enough_cards-0.0.1/settings.ini` & `enough_cards-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = enough_cards
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = enough_cards
@@ -36,8 +36,8 @@
 language = English
 status = 3
 user = genughaben
 
 ### Optional ###
 # requirements = fastcore pandas
 # dev_requirements = 
-# console_scripts =
+# console_scripts =
```

### Comparing `enough_cards-0.0.1/setup.py` & `enough_cards-0.0.2/setup.py`

 * *Files identical despite different names*


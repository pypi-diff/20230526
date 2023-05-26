# Comparing `tmp/ndtorch-0.1.1.tar.gz` & `tmp/ndtorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtorch-0.1.1.tar", last modified: Tue May 23 12:09:24 2023, max compression
+gzip compressed data, was "ndtorch-0.1.2.tar", last modified: Fri May 26 04:30:25 2023, max compression
```

## Comparing `ndtorch-0.1.1.tar` & `ndtorch-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.166386 ndtorch-0.1.1/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1799 2023-05-21 12:40:27.000000 ndtorch-0.1.1/.gitignore
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-21 12:40:27.000000 ndtorch-0.1.1/.readthedocs.yml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-21 12:40:27.000000 ndtorch-0.1.1/LICENSE
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2014 2023-05-23 12:09:24.166386 ndtorch-0.1.1/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1630 2023-05-23 12:03:31.000000 ndtorch-0.1.1/README.MD
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.162386 ndtorch-0.1.1/docs/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-21 12:40:27.000000 ndtorch-0.1.1/docs/Makefile
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-21 12:40:27.000000 ndtorch-0.1.1/docs/make.bat
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       37 2023-05-21 12:40:27.000000 ndtorch-0.1.1/docs/requirements.txt
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.162386 ndtorch-0.1.1/docs/source/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2163 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/conf.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.162386 ndtorch-0.1.1/docs/source/examples/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)   513941 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/examples/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      940 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/index.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.166386 ndtorch-0.1.1/docs/source/modules/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/derivative.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/evaluate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/index.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/jet.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/pfp.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/propagate.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/series.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/signature.rst
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 12:03:31.000000 ndtorch-0.1.1/docs/source/modules/util.rst
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.166386 ndtorch-0.1.1/ndtorch/
--rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8286 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/__init__.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6769 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/derivative.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5887 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/evaluate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3475 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/index.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22741 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/jet.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    16434 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/pfp.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7450 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/propagate.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11429 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/series.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5563 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/signature.py
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2976 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch/util.py
-drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-23 12:09:24.166386 ndtorch-0.1.1/ndtorch.egg-info/
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2014 2023-05-23 12:09:24.000000 ndtorch-0.1.1/ndtorch.egg-info/PKG-INFO
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      822 2023-05-23 12:09:24.000000 ndtorch-0.1.1/ndtorch.egg-info/SOURCES.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-05-23 12:09:24.000000 ndtorch-0.1.1/ndtorch.egg-info/dependency_links.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       32 2023-05-23 12:09:24.000000 ndtorch-0.1.1/ndtorch.egg-info/requires.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-05-23 12:09:24.000000 ndtorch-0.1.1/ndtorch.egg-info/top_level.txt
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)   513941 2023-05-23 12:03:31.000000 ndtorch-0.1.1/ndtorch.ipynb
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      545 2023-05-23 12:03:31.000000 ndtorch-0.1.1/pyproject.toml
--rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-05-23 12:09:24.166386 ndtorch-0.1.1/setup.cfg
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1816 2023-05-23 16:05:19.000000 ndtorch-0.1.2/.gitignore
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      152 2023-05-23 16:04:29.000000 ndtorch-0.1.2/.readthedocs.yml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     1069 2023-05-23 16:04:29.000000 ndtorch-0.1.2/LICENSE
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2627 2023-05-26 04:30:25.257227 ndtorch-0.1.2/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2142 2023-05-25 17:05:08.000000 ndtorch-0.1.2/README.MD
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.245227 ndtorch-0.1.2/docs/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      638 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/Makefile
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      804 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/make.bat
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.249227 ndtorch-0.1.2/docs/pics/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1376301 2023-05-25 16:59:32.000000 ndtorch-0.1.2/docs/pics/change.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1239706 2023-05-24 09:08:54.000000 ndtorch-0.1.2/docs/pics/collision.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    92012 2023-05-25 15:47:52.000000 ndtorch-0.1.2/docs/pics/logo.svg
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  2852797 2023-05-25 15:55:45.000000 ndtorch-0.1.2/docs/pics/manifold.gif
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       37 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/requirements.txt
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2195 2023-05-25 16:17:36.000000 ndtorch-0.1.2/docs/source/conf.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/examples/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1140881 2023-05-26 04:18:09.000000 ndtorch-0.1.2/docs/source/examples/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      940 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/index.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.253227 ndtorch-0.1.2/docs/source/modules/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       48 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/derivative.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       46 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/evaluate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       43 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/index.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/jet.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       41 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/pfp.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/propagate.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       44 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/series.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       47 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/signature.rst
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       42 2023-05-23 16:04:29.000000 ndtorch-0.1.2/docs/source/modules/util.rst
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/ndtorch/
+-rwxrwxr-x   0 imorozov  (1000) imorozov  (1000)     8286 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/__init__.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     6769 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/derivative.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7451 2023-05-25 16:03:14.000000 ndtorch-0.1.2/ndtorch/evaluate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     3475 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/index.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    22741 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/jet.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    16434 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/pfp.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     7699 2023-05-25 16:03:21.000000 ndtorch-0.1.2/ndtorch/propagate.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)    11429 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/series.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     5563 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/signature.py
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2976 2023-05-23 16:04:29.000000 ndtorch-0.1.2/ndtorch/util.py
+drwxrwxr-x   0 imorozov  (1000) imorozov  (1000)        0 2023-05-26 04:30:25.257227 ndtorch-0.1.2/ndtorch.egg-info/
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)     2627 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/PKG-INFO
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      909 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        1 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      135 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/requires.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)        8 2023-05-26 04:30:25.000000 ndtorch-0.1.2/ndtorch.egg-info/top_level.txt
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)  1140881 2023-05-26 04:18:09.000000 ndtorch-0.1.2/ndtorch.ipynb
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)      736 2023-05-26 04:27:32.000000 ndtorch-0.1.2/pyproject.toml
+-rw-rw-r--   0 imorozov  (1000) imorozov  (1000)       38 2023-05-26 04:30:25.257227 ndtorch-0.1.2/setup.cfg
```

### Comparing `ndtorch-0.1.1/.gitignore` & `ndtorch-0.1.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Dev
+dev.ipynb
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `ndtorch-0.1.1/LICENSE` & `ndtorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/PKG-INFO` & `ndtorch-0.1.2/README.MD`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-Metadata-Version: 2.1
-Name: ndtorch
-Version: 0.1.1
-Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables
-Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
-License: MIT
-Keywords: torch,derivative
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/ndtorch/badge/?version=latest)](https://ndtorch.readthedocs.io/en/latest/?badge=latest)
 
 # ndtorch, 2022-2023
 ## i.a.morozov@inp.nsk.su
 
+<p align="center">
+  <img width="100" height="100" src="docs/pics/logo.svg">
+</p>
+
 Higher order partial derivatives computation with respect to one or several tensor-like variables.
 Taylor series function approximation (derivative table and series function representation).
 Parametric fixed point computation.
 
 # Install & build
 
 ```
@@ -73,7 +65,29 @@
 
 # Desription
 
 ```python
 >>> import ndtorch
 >>> ndtorch.__about__
 ```
+
+# Animations
+
+Stable and unstable invariant manifolds approximation
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/manifold.gif">
+</p>
+
+Collision of fixed points
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/collision.gif">
+</p>
+
+Reduce real part of a hyperbolic fixed point
+
+Collision of fixed points
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/change.gif">
+</p>
```

### Comparing `ndtorch-0.1.1/docs/Makefile` & `ndtorch-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/docs/make.bat` & `ndtorch-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/docs/source/conf.py` & `ndtorch-0.1.2/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 exclude_patterns = []
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
+html_logo = '../pics/logo.svg'
 # html_static_path = ['_static']
 
 # -- Autodoc Configuration ---------------------------------------------------
 
 # Add here all modules to be mocked up. When the dependencies are not met
 # at building time. Here used to have PyQT mocked.
-autodoc_mock_imports = ['PyQt5', 'PyQt5.QtGui', 'PyQt5.QtCore', 'PyQt5.QtWidgets', "matplotlib.backends.backend_qt5agg"]
+autodoc_mock_imports = ['PyQt5', 'PyQt5.QtGui', 'PyQt5.QtCore', 'PyQt5.QtWidgets', "matplotlib.backends.backend_qt5agg"]
```

### Comparing `ndtorch-0.1.1/docs/source/index.rst` & `ndtorch-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/__init__.py` & `ndtorch-0.1.2/ndtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/derivative.py` & `ndtorch-0.1.2/ndtorch/derivative.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/evaluate.py` & `ndtorch-0.1.2/ndtorch/propagate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,209 +1,253 @@
 """
-Evaluate
---------
+Propagate
+---------
 
-Table and series evaluation
+Propagate table and series representations
 
 """
 
-from math import factorial
-
 from typing import TypeAlias
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 from multimethod import multimethod
 
 import torch
 from torch import Tensor
 
+from .util import flatten
 from .derivative import derivative
+from .signature import set
+from .signature import get
+from .series import series
+from .evaluate import evaluate
 
 Mapping  : TypeAlias = Callable
 Point    : TypeAlias = list[Tensor]
 Delta    : TypeAlias = list[Tensor]
 State    : TypeAlias = Tensor
 Knobs    : TypeAlias = list[Tensor]
 Table    : TypeAlias = list
 Series   : TypeAlias = dict[tuple[int, ...], Tensor]
 Signature: TypeAlias = Union[list[tuple[int, ...]], list[tuple[tuple[int, ...], float]]]
 
 
-@multimethod
-def evaluate(table:Table,
-             delta:Delta) -> Tensor:
+def identity(order:tuple[int, ...],
+             point:Point, *,
+             flag:bool=False,
+             parametric:Optional[Table]=None,
+             jacobian:Optional[Callable]=None) -> Union[Table, Series]:
     """
-    Evaluate input derivative table representation at a given delta deviation
+    Generate identity derivative table or identity series
 
-    Note, input table is expected to represent a vector or scalar valued function
+    Note, identity table or series represent an identity mapping
 
     Parameters
     ----------
-    table: Table
-        input derivative table representation
-    delta: Delta
-        delta deviation
+    order: tuple[int, ...], non-negative
+        maximum derivative orders
+    point: Point
+        evaluation point
+    flag: bool, default=False
+        flag to return identity series instead of table
+    parametric: Optional[Table]
+        optional parametric table
+    jacobian: Optional[Callable]
+        torch.func.jacfwd (default) or torch.func.jacrev
 
     Returns
     -------
-    Tensor
+    Union[Table, Series]
+        identity derivative table or series
 
     Examples
     --------
     >>> import torch
-    >>> from ndtorch.derivative import derivative
-    >>> def fn(x, y):
-    ...    x1, x2 = x
-    ...    y1, y2 = y
-    ...    return torch.stack([x1*(1 + y1), x2*(1 + y2)])
-    >>> x = torch.tensor([0.0, 0.0])
-    >>> y = torch.zeros_like(x)
-    >>> t = derivative((2, 1), fn, x, y)
-    >>> dx = 1.0E-3*torch.ones_like(x)
-    >>> dy = 1.0E-3*torch.ones_like(x)
-    >>> torch.allclose(fn(x + dx, y + dy), evaluate(t, [dx, dy]))
-    True
+    >>> state = torch.tensor([0.0, 0.0])
+    >>> knobs = [torch.tensor([0.0, 0.0])]
+    >>> point = [state, *knobs]
+    >>> identity((1, 1), point)
+    [[tensor([0., 0.]),
+    tensor([[0., 0.],
+            [0., 0.]])],
+    [tensor([[1., 0.],
+            [0., 1.]]),
+    tensor([[[0., 0.],
+            [0., 0.]],
+    
+            [[0., 0.],
+            [0., 0.]]])]]
+    >>> identity((1, 1), point, flag=True)
+    {(0, 0, 0, 0): tensor([0., 0.]),
+    (0, 0, 1, 0): tensor([0., 0.]),
+    (0, 0, 0, 1): tensor([0., 0.]),
+    (1, 0, 0, 0): tensor([1., 0.]),
+    (0, 1, 0, 0): tensor([0., 1.]),
+    (1, 0, 1, 0): tensor([0., 0.]),
+    (1, 0, 0, 1): tensor([0., 0.]),
+    (0, 1, 1, 0): tensor([0., 0.]),
+    (0, 1, 0, 1): tensor([0., 0.])}
 
     """
-    return sum(evaluate([i], subtable, delta) for i, subtable in enumerate(table))
+    jacobian = torch.func.jacfwd if jacobian is None else jacobian
 
+    table = derivative(order, lambda x, *xs: x, point, intermediate=True, jacobian=jacobian)
 
-@multimethod
-def evaluate(index:list[int], table:Table, delta:Delta):
-    """ (auxiliary) """
-    return sum(evaluate(index + [i], subtable, delta) for i, subtable in enumerate(table))
+    if parametric is not None:
+        set(table, (0, ),  get(parametric, (0, )))
 
+    if not flag:
+        return table
 
-@multimethod
-def evaluate(index:list[int], table:Tensor, delta:Delta):
-    """ (auxiliary) """
-    total = 1.0
-    for count, order in enumerate(index):
-        total *= 1.0/factorial(order)
-        value  = delta[count]
-        if value.ndim > 0:
-            for _ in range(order):
-                table @= value
-        else:
-            for _ in range(order):
-                table *= value
-    return total*table
+    return series(tuple(map(len, point)), order, table)
 
 
 @multimethod
-def evaluate(series:Series,
-             delta:Delta,
-             epsilon:Optional[float]=None) -> Tensor:
+def propagate(dimension:tuple[int, ...],
+              order:tuple[int, ...],
+              data:Table,
+              knobs:Knobs,
+              mapping:Mapping,
+              *pars:tuple,
+              intermediate:bool=True,
+              jacobian:Optional[Callable]=None) -> Union[Table, Tensor]:
     """
-    Evaluate series representation at a given deviation delta
-
-    Note, input series is expected to represent a vector valued function
-    For epsilon != None, fast evaluation is performed
+    Propagate derivative table representation through a given mapping
 
     Parameters
     ----------
-    series: Series
-        input series representation
-    delta: Delta
-        delta deviation
-    epsilon: Optional[float], non-negative, default=None
-        fast series evaluation / tolerance epsilon
+    dimension: tuple[int, ...], positive
+        dimensions
+    order: tuple[int, ...], non-negative
+        maximum derivative orders
+    data: Table
+        input derivative table
+    knobs: Knobs
+        input parametric variables
+    mapping: Mapping
+        input mapping
+    *pars: tuple
+        additional mapping fixed arguments
+    intermediate: bool, default=True
+        flag to return intermediate derivatives
+    jacobian: Optional[Callable]
+        torch.func.jacfwd (default) or torch.func.jacrev
 
     Returns
     -------
-    Tensor
+    Union[Table, Tensor]
 
     Examples
     --------
     >>> import torch
+    >>> from ndtorch.util import flatten
     >>> from ndtorch.derivative import derivative
-    >>> from ndtorch.series import series
-    >>> def fn(x, y):
-    ...    x1, x2 = x
-    ...    y1, y2 = y
-    ...    return torch.stack([x1*(1 + y1), x2*(1 + y2)])
-    >>> x = torch.tensor([0.0, 0.0])
-    >>> y = torch.zeros_like(x)
-    >>> t = derivative((2, 1), fn, x, y)
-    >>> s = series((2, 2), (2, 1), t)
-    >>> dx = 1.0E-3*torch.ones_like(x)
-    >>> dy = 1.0E-3*torch.ones_like(x)
-    >>> torch.allclose(fn(x + dx, y + dy), evaluate(s, [dx, dy]))
-
-    """
-    state = torch.cat(delta)
-
-    if epsilon is not None:
-        state = epsilon + state
-        index = torch.tensor([*series.keys()], dtype=torch.int64, device=state.device)
-        value = torch.stack([*series.values()])
-        return (value.T*(state**index).prod(-1)).sum(-1)
-
-    total, *_ = series.values()
-    total = torch.zeros_like(total)
-    for key, value in series.items():
-        local = torch.ones_like(state).prod()
-        for i, x in zip(key, state):
-            for _ in range(i):
-                local = x * local
-        total = total + value * local
-    return total
-
-
-def table(dimension:tuple[int, ...],
-          order:tuple[int, ...],
-          series:Series, *,
-          epsilon:Optional[float]=None,
-          jacobian:Optional[Callable]=None) -> Table:
+    >>> state = torch.tensor([0.0, 0.0])
+    >>> knobs = torch.tensor([1.0, 1.0])
+    >>> def fn(state, knobs):
+    ...     x1, x2 = state
+    ...     y1, y2 = knobs
+    ...     return torch.stack([x1 + x2*y1, x2 + x1*y2])
+    >>> def gn(state, knobs):
+    ...     x1, x2 = state
+    ...     y1, y2 = knobs
+    ...     return torch.stack([y1 + y2*x1, y2 + y1*x2])
+    >>> u = derivative((2, 2), lambda state, knobs: gn(fn(state, knobs), knobs), state, knobs)
+    >>> v = identity((2, 2), [state, knobs])
+    >>> v = propagate((2, 2), (2, 2), v, [knobs], fn)
+    >>> v = propagate((2, 2), (2, 2), v, [knobs], gn)
+    >>> all(torch.allclose(x, y) for x, y in zip(*map(lambda t: flatten(t, target=list), (u, v))))
+    True
+
     """
-    Generate derivative table representation from a given series representation
+    jacobian = torch.func.jacfwd if jacobian is None else jacobian
 
-    Note, table is generated by taking derivatives of evaluated series at zero deviation delta.
-    For epsilon != None can be used for fast series evaluation, but can generate incorrect table
+    def auxiliary(*args) -> Tensor:
+        state, *args = args
+        state = evaluate(data, [state, *args])
+        args = [arg + knob for arg, knob in zip(args, knobs)]
+        return mapping(state, *args, *pars)
+
+    value, *_ = flatten(data, target=list)
+    delta = [torch.zeros(i, dtype=value.dtype, device=value.device) for i in dimension]
+
+    return derivative(order, auxiliary, delta, intermediate=intermediate, jacobian=jacobian)
+
+
+@multimethod
+def propagate(dimension:tuple[int, ...],
+              order:tuple[int, ...],
+              data:Series,
+              knobs:Knobs,
+              mapping:Mapping,
+              *pars:tuple,
+              epsilon:Optional[float]=None,
+              jacobian:Optional[Callable]=None) -> Series:
+    """
+    Propagate series representation through a given mapping
+
+    Note, input series are expected to contain all indices
 
     Parameters
     ----------
     dimension: tuple[int, ...], positive
         dimensions
     order: tuple[int, ...], non-negative
         maximum derivative orders
-    series: Series
-        input series representation
+    data: Series
+        input series
+    knobs: Knobs
+        input parametric variables
+    mapping: Mapping
+        input mapping
+    *pars: tuple
+        additional mapping fixed arguments
     epsilon: Optional[float], non-negative, default=None
         fast series evaluation / tolerance epsilon
+    intermediate: bool, default=True
+        flag to return intermediate derivatives
     jacobian: Optional[Callable]
         torch.func.jacfwd (default) or torch.func.jacrev
 
     Returns
     -------
-    Table
+    Series
 
     Examples
     --------
     >>> import torch
+    >>> from ndtorch.util import flatten
     >>> from ndtorch.derivative import derivative
     >>> from ndtorch.series import series
-    >>> def fn(x, y):
-    ...    x1, x2 = x
-    ...    y1, y2 = y
-    ...    return torch.stack([x1*(1 + y1), x2*(1 + y2)])
-    >>> x = torch.tensor([0.0, 0.0])
-    >>> y = torch.zeros_like(x)
-    >>> t = derivative((2, 1), fn, x, y)
-    >>> s = series((2, 2), (2, 1), t)
-    >>> t = table((2, 2), (2, 1), s)
-    >>> dx = 1.0E-3*torch.ones_like(x)
-    >>> dy = 1.0E-3*torch.ones_like(x)
-    >>> torch.allclose(fn(x + dx, y + dy), evaluate(t, [dx, dy]))
+    >>> state = torch.tensor([0.0, 0.0])
+    >>> knobs = torch.tensor([1.0, 1.0])
+    >>> def fn(state, knobs):
+    ...     x1, x2 = state
+    ...     y1, y2 = knobs
+    ...     return torch.stack([x1 + x2*y1, x2 + x1*y2])
+    >>> def gn(state, knobs):
+    ...     x1, x2 = state
+    ...     y1, y2 = knobs
+    ...     return torch.stack([y1 + y2*x1, y2 + y1*x2])
+    >>> u = derivative((2, 2), lambda state, knobs: gn(fn(state, knobs), knobs), state, knobs)
+    >>> u = series((2, 2), (2, 2), u)
+    >>> v = identity((2, 2), [state, knobs], flag=True)
+    >>> v = propagate((2, 2), (2, 2), v, [knobs], fn)
+    >>> v = propagate((2, 2), (2, 2), v, [knobs], gn)
+    >>> all(torch.allclose(x, y) for x, y in zip(u.values(), v.values()))
+    True
 
     """
     jacobian = torch.func.jacfwd if jacobian is None else jacobian
 
-    def function(*args):
-        return evaluate(series, [*args], epsilon=epsilon)
+    def auxiliary(*args) -> Tensor:
+        state, *args = torch.stack([*args]).split(dimension)
+        state = evaluate(data, [state, *args], epsilon=epsilon)
+        args = [arg + knob for arg, knob in zip(args, torch.cat(knobs))]
+        return mapping(state, *args, *pars)
 
-    value, *_ = series.values()
-    delta = [torch.zeros(i, dtype=value.dtype, device=value.device) for i in dimension]
+    value, *_ = data.values()
+    delta = torch.cat([torch.zeros(i, dtype=value.dtype, device=value.device) for i in dimension])
 
-    return derivative(order, function, delta, intermediate=True, jacobian=jacobian)
+    return series([*data.keys()], auxiliary, *delta, jacobian=jacobian)
```

### Comparing `ndtorch-0.1.1/ndtorch/index.py` & `ndtorch-0.1.2/ndtorch/index.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/jet.py` & `ndtorch-0.1.2/ndtorch/jet.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/pfp.py` & `ndtorch-0.1.2/ndtorch/pfp.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/series.py` & `ndtorch-0.1.2/ndtorch/series.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/signature.py` & `ndtorch-0.1.2/ndtorch/signature.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch/util.py` & `ndtorch-0.1.2/ndtorch/util.py`

 * *Files identical despite different names*

### Comparing `ndtorch-0.1.1/ndtorch.egg-info/PKG-INFO` & `ndtorch-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: ndtorch
-Version: 0.1.1
-Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables
+Version: 0.1.2
+Summary: Higher order partial derivatives computation with respect to one or several tensor-like variables, application to nonlinear dynamics
 Author-email: Ivan Morozov <i.a.morozov@inp.nsk.su>
 License: MIT
 Keywords: torch,derivative
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: examples
+Provides-Extra: test
+Provides-Extra: all
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/ndtorch/badge/?version=latest)](https://ndtorch.readthedocs.io/en/latest/?badge=latest)
 
 # ndtorch, 2022-2023
 ## i.a.morozov@inp.nsk.su
 
+<p align="center">
+  <img width="100" height="100" src="docs/pics/logo.svg">
+</p>
+
 Higher order partial derivatives computation with respect to one or several tensor-like variables.
 Taylor series function approximation (derivative table and series function representation).
 Parametric fixed point computation.
 
 # Install & build
 
 ```
@@ -73,7 +80,29 @@
 
 # Desription
 
 ```python
 >>> import ndtorch
 >>> ndtorch.__about__
 ```
+
+# Animations
+
+Stable and unstable invariant manifolds approximation
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/manifold.gif">
+</p>
+
+Collision of fixed points
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/collision.gif">
+</p>
+
+Reduce real part of a hyperbolic fixed point
+
+Collision of fixed points
+
+<p align="center">
+  <img width="576" height="576" src="docs/pics/change.gif">
+</p>
```

### Comparing `ndtorch-0.1.1/ndtorch.egg-info/SOURCES.txt` & `ndtorch-0.1.2/ndtorch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 LICENSE
 README.MD
 ndtorch.ipynb
 pyproject.toml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
+docs/pics/change.gif
+docs/pics/collision.gif
+docs/pics/logo.svg
+docs/pics/manifold.gif
 docs/source/conf.py
 docs/source/index.rst
 docs/source/examples/ndtorch.ipynb
 docs/source/modules/derivative.rst
 docs/source/modules/evaluate.rst
 docs/source/modules/index.rst
 docs/source/modules/jet.rst
```


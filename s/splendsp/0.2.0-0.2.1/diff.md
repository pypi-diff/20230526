# Comparing `tmp/splendsp-0.2.0.tar.gz` & `tmp/splendsp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendsp-0.2.0.tar", last modified: Thu May 25 16:50:17 2023, max compression
+gzip compressed data, was "splendsp-0.2.1.tar", last modified: Fri May 26 19:27:02 2023, max compression
```

## Comparing `splendsp-0.2.0.tar` & `splendsp-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.568360 splendsp-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.564360 splendsp-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.564360 splendsp-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 16:50:02.000000 splendsp-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-25 16:50:02.000000 splendsp-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 16:50:02.000000 splendsp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-25 16:50:17.568360 splendsp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-25 16:50:02.000000 splendsp-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 16:50:02.000000 splendsp-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 16:50:17.568360 splendsp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 16:50:02.000000 splendsp-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.564360 splendsp-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.564360 splendsp-0.2.0/src/splendsp/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.568360 splendsp-0.2.0/src/splendsp/cut/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/cut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28326 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/cut/_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/cut/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.568360 splendsp-0.2.0/src/splendsp/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/_de_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)    60035 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/_of_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/dsp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.568360 splendsp-0.2.0/src/splendsp/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27646 2023-05-25 16:50:02.000000 splendsp-0.2.0/src/splendsp/plot/_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:17.568360 splendsp-0.2.0/src/splendsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:50:17.000000 splendsp-0.2.0/src/splendsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.221493 splendsp-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.217493 splendsp-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.217493 splendsp-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 19:26:48.000000 splendsp-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-26 19:26:48.000000 splendsp-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-26 19:26:48.000000 splendsp-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 19:27:02.221493 splendsp-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 19:26:48.000000 splendsp-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-26 19:26:48.000000 splendsp-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 19:27:02.221493 splendsp-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 19:26:48.000000 splendsp-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.217493 splendsp-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.217493 splendsp-0.2.1/src/splendsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.221493 splendsp-0.2.1/src/splendsp/cut/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/cut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28326 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/cut/_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/cut/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.221493 splendsp-0.2.1/src/splendsp/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/_de_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60035 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/_of_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/dsp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.221493 splendsp-0.2.1/src/splendsp/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-05-26 19:26:48.000000 splendsp-0.2.1/src/splendsp/plot/_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:27:02.217493 splendsp-0.2.1/src/splendsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:27:01.000000 splendsp-0.2.1/src/splendsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 19:27:02.000000 splendsp-0.2.1/src/splendsp.egg-info/top_level.txt
```

### Comparing `splendsp-0.2.0/.github/workflows/python-publish.yml` & `splendsp-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/.gitignore` & `splendsp-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/LICENSE` & `splendsp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/PKG-INFO` & `splendsp-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendsp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Splendid Digital Signal Processing of time series data for small physics experiments
 Home-page: https://github.com/splendor-collab/splendsp
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendsp-0.2.0/README.md` & `splendsp-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/setup.cfg` & `splendsp-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/cut/_cut.py` & `splendsp-0.2.1/src/splendsp/cut/_cut.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/cut/_utils.py` & `splendsp-0.2.1/src/splendsp/cut/_utils.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/dsp/_de_pileup.py` & `splendsp-0.2.1/src/splendsp/dsp/_de_pileup.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/dsp/_fitting.py` & `splendsp-0.2.1/src/splendsp/dsp/_fitting.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/dsp/_noise.py` & `splendsp-0.2.1/src/splendsp/dsp/_noise.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/dsp/_of_pileup.py` & `splendsp-0.2.1/src/splendsp/dsp/_of_pileup.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/dsp/_utils.py` & `splendsp-0.2.1/src/splendsp/dsp/_utils.py`

 * *Files identical despite different names*

### Comparing `splendsp-0.2.0/src/splendsp/plot/_plot.py` & `splendsp-0.2.1/src/splendsp/plot/_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import colors as clrs
 from matplotlib.patches import Ellipse
 from scipy import stats
 import types
 
 
@@ -900,8 +901,8 @@
     )
 
     ax_ell = ax.add_patch(ell)
 
     if autoscale_axes:
         ax.autoscale()
 
-    return fig, ax
+    return fig, ax
```

### Comparing `splendsp-0.2.0/src/splendsp.egg-info/PKG-INFO` & `splendsp-0.2.1/src/splendsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendsp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Splendid Digital Signal Processing of time series data for small physics experiments
 Home-page: https://github.com/splendor-collab/splendsp
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendsp-0.2.0/src/splendsp.egg-info/SOURCES.txt` & `splendsp-0.2.1/src/splendsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/circuitpython-display_ht16k33-0.1.0.tar.gz` & `tmp/circuitpython-display_ht16k33-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-display_ht16k33-0.1.0.tar", last modified: Wed May 24 00:40:35 2023, max compression
+gzip compressed data, was "circuitpython-display_ht16k33-0.2.0.tar", last modified: Fri May 26 19:54:26 2023, max compression
```

## Comparing `circuitpython-display_ht16k33-0.1.0.tar` & `circuitpython-display_ht16k33-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:35.007892 circuitpython-display_ht16k33-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:34.999892 circuitpython-display_ht16k33-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:34.999892 circuitpython-display_ht16k33-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-24 00:40:35.003892 circuitpython-display_ht16k33-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:34.999892 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-24 00:40:34.000000 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-24 00:40:34.000000 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:40:34.000000 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 00:40:34.000000 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 00:40:34.000000 circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:34.999892 circuitpython-display_ht16k33-0.1.0/display_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:26.000000 circuitpython-display_ht16k33-0.1.0/display_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-24 00:40:26.000000 circuitpython-display_ht16k33-0.1.0/display_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-24 00:40:26.000000 circuitpython-display_ht16k33-0.1.0/display_ht16k33/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:35.003892 circuitpython-display_ht16k33-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/7mwahe.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:35.003892 circuitpython-display_ht16k33-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:40:35.003892 circuitpython-display_ht16k33-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-24 00:40:26.000000 circuitpython-display_ht16k33-0.1.0/examples/display_ht16k33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-24 00:40:26.000000 circuitpython-display_ht16k33-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 00:40:15.000000 circuitpython-display_ht16k33-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:40:35.007892 circuitpython-display_ht16k33-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.413729 circuitpython-display_ht16k33-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 19:54:26.000000 circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/display_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/display_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.417729 circuitpython-display_ht16k33-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/7mwahe.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_segments_count_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-26 19:54:19.000000 circuitpython-display_ht16k33-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 19:54:05.000000 circuitpython-display_ht16k33-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:54:26.421728 circuitpython-display_ht16k33-0.2.0/setup.cfg
```

### Comparing `circuitpython-display_ht16k33-0.1.0/.github/workflows/build.yml` & `circuitpython-display_ht16k33-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-display_ht16k33-0.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/.gitignore` & `circuitpython-display_ht16k33-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/.pre-commit-config.yaml` & `circuitpython-display_ht16k33-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/.pylintrc` & `circuitpython-display_ht16k33-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/LICENSE` & `circuitpython-display_ht16k33-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/PKG-INFO` & `circuitpython-display_ht16k33-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-display_ht16k33
-Version: 0.1.0
+Version: 0.2.0
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
-Author-email: JDM <xxx@mailmeto.mozmail.com>
+Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
@@ -29,16 +29,16 @@
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/circuitpython-display-ht16k33
 
 .. image:: https://static.pepy.tech/personalized-badge/circuitpython-display-ht16k33?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/circuitpython-display-ht16k33
 
-.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/workflows/Build%20CI/badge.svg
-    :target: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/actions
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/workflows/Build%20CI/badge.svg
+    :target: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
```

### Comparing `circuitpython-display_ht16k33-0.1.0/README.rst` & `circuitpython-display_ht16k33-0.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/circuitpython-display-ht16k33
 
 .. image:: https://static.pepy.tech/personalized-badge/circuitpython-display-ht16k33?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/circuitpython-display-ht16k33
 
-.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/workflows/Build%20CI/badge.svg
-    :target: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/actions
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/workflows/Build%20CI/badge.svg
+    :target: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
```

### Comparing `circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/PKG-INFO` & `circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: circuitpython-display-ht16k33
-Version: 0.1.0
+Version: 0.2.0
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
-Author-email: JDM <xxx@mailmeto.mozmail.com>
+Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
@@ -29,16 +29,16 @@
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/circuitpython-display-ht16k33
 
 .. image:: https://static.pepy.tech/personalized-badge/circuitpython-display-ht16k33?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/circuitpython-display-ht16k33
 
-.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/workflows/Build%20CI/badge.svg
-    :target: https://github.com/jposada202020/CircuitPython_DISPLAY-HT16K33/actions
+.. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/workflows/Build%20CI/badge.svg
+    :target: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
```

### Comparing `circuitpython-display_ht16k33-0.1.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt` & `circuitpython-display_ht16k33-0.2.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,20 +14,25 @@
 circuitpython_display_ht16k33.egg-info/SOURCES.txt
 circuitpython_display_ht16k33.egg-info/dependency_links.txt
 circuitpython_display_ht16k33.egg-info/requires.txt
 circuitpython_display_ht16k33.egg-info/top_level.txt
 display_ht16k33/__init__.py
 display_ht16k33/ht16k33.py
 display_ht16k33/matrix.py
+display_ht16k33/segments.py
 docs/7mwahe.gif
 docs/api.rst
 docs/conf.py
 docs/examples.rst
+docs/font5x8.bin
 docs/index.rst
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
-examples/display_ht16k33_simpletest.py
+examples/display_ht16k33_segments_count_down.py
+examples/display_ht16k33_segments_simpletest.py
+examples/display_ht16k33_simpletest.py
+examples/display_ht16k33_text.py
```

### Comparing `circuitpython-display_ht16k33-0.1.0/display_ht16k33/ht16k33.py` & `circuitpython-display_ht16k33-0.2.0/display_ht16k33/ht16k33.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 Based on some code from https://github.com/adafruit/Adafruit_CircuitPython_HT16K33.git
 Authors: Radomir Dopieralski and Tony DiCola License: MIT
 
 * Author(s): Jose D. Montoya
 
 
 """
-
+import gc
 from vectorio import Circle
 import displayio
 import ulab.numpy as np
 
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 class HT16K33:
     """
     Main class
     """
@@ -49,15 +49,15 @@
 
         self.length = register_width
 
         self.group = displayio.Group()
 
         palette = displayio.Palette(3)
         palette[0] = 0x123456
-        palette[1] = 0x00000
+        palette[1] = 0x123456
         palette[2] = 0xFF5500
 
         self.matrix = []
         for j in range(1, self.rows + 1):
             row_buff = []
             for coord_x in range(1, self.cols + 1):
                 value = Circle(
@@ -81,15 +81,15 @@
     def set(self, y, new_value: int) -> None:
         """
         Set a particular value in an specific row defined by y
         """
         reg = 0
 
         if self.length == 2:
-            order = range(self.length - 1, 0, -1)
+            order = range(0, 2)
         if self.length == 1:
             order = range(0, 1)
 
         for ind in order:
             reg = (reg << 8) | self.buffer_rows[y][ind]
 
         reg &= ~self.bit_mask
@@ -103,15 +103,15 @@
         self.update(y)
 
     def pixel(self, x: int, y: int, color=True) -> None:
         """
         Set a specific pixel in the matrix
         """
         reg = 0
-        order = range(0, len(self.buffer))
+        order = range(0, self.length)
 
         for i in order:
             reg = (reg << 8) | self.buffer_rows[y][i]
 
         mask = 1 << x
 
         if color:
@@ -162,14 +162,15 @@
         """
         if rotate:
             pass
         self.array = np.roll(self.array, y, axis=0)
         self.array = np.roll(self.array, x, axis=1)
 
         self.update_all()
+        gc.collect()
 
     def shift_right(self, rotate: bool = False) -> None:
         """
         Shift all pixels right
 
         :param rotate: (Optional) Rotate the shifted pixels to the left side (default=False)
         """
@@ -194,7 +195,36 @@
     def shift_down(self, rotate: bool = False) -> None:
         """
         Shift all pixels down
 
         :param rotate: (Optional) Rotate the shifted pixels to top (default=False)
         """
         self.shift(0, -1, rotate)
+
+    def fill(self, color: bool) -> None:
+        """
+        fill the entire matrix
+        """
+        if color:
+            new_value = 0xFFFF
+        else:
+            new_value = 0x0000
+        for ele in range(self.rows):
+            reg = 0
+
+            if self.length == 2:
+                order = range(0, 2)
+            if self.length == 1:
+                order = range(0, 1)
+
+            for ind in order:
+                reg = (reg << 8) | self.buffer_rows[ele][ind]
+
+            reg &= ~self.bit_mask
+            reg |= new_value
+
+            for ind2 in order:
+                self.buffer_rows[ele][ind2] = reg & 0xFF
+                reg >>= 8
+
+            self.convert_to_leds(ele)
+        self.update_all()
```

### Comparing `circuitpython-display_ht16k33-0.1.0/docs/7mwahe.gif` & `circuitpython-display_ht16k33-0.2.0/docs/7mwahe.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/docs/_static/Logo.png` & `circuitpython-display_ht16k33-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/docs/_static/favicon.ico` & `circuitpython-display_ht16k33-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/docs/conf.py` & `circuitpython-display_ht16k33-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.1.0/examples/display_ht16k33_simpletest.py` & `circuitpython-display_ht16k33-0.2.0/examples/display_ht16k33_simpletest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
 
+# Copied and adapted in ht16k33_matrix_simpletest.py example for the Adafruit_ht16k33 library here:
+
 import time
 import board
 from display_ht16k33 import matrix
 
 display = board.DISPLAY
 matrix = matrix.Matrix8x8()
 display.show(matrix.group)
```

### Comparing `circuitpython-display_ht16k33-0.1.0/pyproject.toml` & `circuitpython-display_ht16k33-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-display_ht16k33"
 description = "On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices."
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
-    {name = "JDM", email = "xxx@mailmeto.mozmail.com"}
+    {name = "JDM", email = "xxxy@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33"}
 keywords = [
     "sensor",
     "blinka",
     "circuitpython",
     "micropython",
```


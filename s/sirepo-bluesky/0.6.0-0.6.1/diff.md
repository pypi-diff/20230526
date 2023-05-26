# Comparing `tmp/sirepo-bluesky-0.6.0.tar.gz` & `tmp/sirepo-bluesky-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirepo-bluesky-0.6.0.tar", last modified: Thu Feb 23 15:24:53 2023, max compression
+gzip compressed data, was "sirepo-bluesky-0.6.1.tar", last modified: Fri May 26 14:22:52 2023, max compression
```

## Comparing `sirepo-bluesky-0.6.0.tar` & `sirepo-bluesky-0.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.459029 sirepo-bluesky-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-23 15:24:53.463029 sirepo-bluesky-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.459029 sirepo-bluesky-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.459029 sirepo-bluesky-0.6.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/notebooks-new-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/notebooks-old-api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/docs/source/simulations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-23 15:24:53.463029 sirepo-bluesky-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.463029 sirepo-bluesky-0.6.0/sirepo_bluesky/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-23 15:24:53.463029 sirepo-bluesky-0.6.0/sirepo_bluesky/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/madx_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/madx_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/shadow_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/shadow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_ophyd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/srw_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/srw_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.459029 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_shadow_det.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_srw_det.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 15:24:53.459029 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-23 15:24:53.000000 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-23 15:24:53.000000 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 15:24:53.000000 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-23 15:24:53.000000 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-23 15:24:53.000000 sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-02-23 15:24:40.000000 sirepo-bluesky-0.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.021771 sirepo-bluesky-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.021771 sirepo-bluesky-0.6.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/notebooks-new-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/notebooks-old-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/docs/source/simulations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/madx_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/madx_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_ophyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/srw_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/srw_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.029771 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_shadow_det.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_srw_det.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:22:52.025771 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 14:22:51.000000 sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-05-26 14:22:38.000000 sirepo-bluesky-0.6.1/versioneer.py
```

### Comparing `sirepo-bluesky-0.6.0/CONTRIBUTING.rst` & `sirepo-bluesky-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/LICENSE` & `sirepo-bluesky-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/PKG-INFO` & `sirepo-bluesky-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirepo-bluesky
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sirepo-Bluesky interface
 Home-page: https://github.com/NSLS-II/sirepo-bluesky
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sirepo-bluesky-0.6.0/README.rst` & `sirepo-bluesky-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/docs/Makefile` & `sirepo-bluesky-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/docs/make.bat` & `sirepo-bluesky-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/docs/source/conf.py` & `sirepo-bluesky-0.6.1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
-import cloud_sptheme as sptheme
-
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -104,16 +102,15 @@
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "cloud"
-html_theme_path = [sptheme.get_theme_dir()]
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -121,23 +118,14 @@
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
-# This is required for the alabaster theme
-# refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
-html_sidebars = {
-    "**": [
-        "globaltoc.html",
-        "searchbox.html",
-    ]
-}
-
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "sirepo-bluesky"
```

### Comparing `sirepo-bluesky-0.6.0/docs/source/installation.rst` & `sirepo-bluesky-0.6.1/docs/source/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -70,36 +70,39 @@
 
 
 Installation
 ------------
 
 .. note::
 
-  The installation requires the SRW and Shadow3 packages to be installed to make
-  use of all features of the library, however the packages are not available on
-  PyPI for all versions of Python we support (e.g. the ``srwpy`` package's
-  wheels are only available for Python versions up to 3.8, and the ``shadow3``
-  package's wheels have issues with installation/usage). Those packages are
+  The installation requires the ``srwpy`` and ``shadow3`` simulation packages to
+  be installed to make use of all features of the library. Those packages are
   primarily used by the corresponding handlers to be able to load the data from
-  the package-specific formats.  That is why we hightly recommend using the
-  packages from the ``conda-forge`` conda channel:
+  the package-specific formats. The packages are installed automatically when
+  the ``sirepo-bluesky`` package is installed via ``pip``:
+
+  - https://pypi.org/project/srwpy
+  - https://pypi.org/project/shadow3
+
+  One can also install the packages using ``conda`` from the ``conda-forge``
+  channel:
 
   - https://anaconda.org/conda-forge/srwpy
   - https://anaconda.org/conda-forge/shadow3
 
 Start with creating a conda environment. If you do not have conda installation,
 one of the packages from `https://github.com/conda-forge/miniforge
 <https://github.com/conda-forge/miniforge>`_ can be used to quickly install the
 appropriate conda infrastructure.
 
 At the command line:
 
 .. code:: bash
 
-   $ conda create -n sirepo-bluesky -c conda-forge -y python=3.9 srwpy shadow3
+   $ conda create -n sirepo-bluesky -c conda-forge -y python=3.10
    $ conda activate sirepo-bluesky
 
 Then, to install the released version, run one of the following commands:
 
 .. code:: bash
 
    $ python3 -m pip install sirepo-bluesky        # to install from PyPI, OR
```

### Comparing `sirepo-bluesky-0.6.0/docs/source/release-history.rst` & `sirepo-bluesky-0.6.1/docs/source/release-history.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,52 @@
 ===============
 Release History
 ===============
 
+v0.6.1 (2023-05-26)
+-------------------
+This is a maintenance release primarily addressing the packaging, continuous
+integration, and testing matters.
+
+API
+...
+- Fixed the deprecated API call ``bluesky-auth`` -> ``auth-bluesky-login`` to
+  authenticate with Sirepo using the _bluesky_ auth method.
+
+Tests
+.....
+- Recreated `vcrpy <https://vcrpy.readthedocs.io/en/latest/>`_ cassettes for the
+  tests using old API (to be deprecated in the future).
+- Fixed beam statistics report test.
+
+CI improvements
+...............
+- Applied `NSLS-II/start-sirepo-action
+  <https://github.com/NSLS-II/start-sirepo-action>`_ to start Sirepo in the CI
+  workflows (used in other repositories which need Sirepo with predefined
+  examples).
+- Fixed the Sirepo startup script to use ``radiasoft/sirepo:beta`` docker
+  image. The action above uses the script from this repository.
+- Added ``workflow_dispatch`` trigger to CI workflows to be able to start them
+  manually.
+
+Packaging
+.........
+- All dependencies, including ``srwpy`` and ``shadow3`` are now installed along
+  with ``sirepo-bluesky`` from the same source (either PyPI or conda-forge),
+  therefore users do not need to preinstall them.
+- Temporary fix for incompatibility between the ``requests`` package and
+  ``urllib3`` v2+.
+
+Documentation
+.............
+- Change Sphinx theme to `furo <https://pradyunsg.me/furo/>`_.
+- Update installation instructions.
+
+
 v0.6.0 (2023-02-23)
 -------------------
 This is a major release dropping support of `intake
 <https://intake.readthedocs.io/en/latest/>`_ and extending support of MAD-X
 simulations.
 
 API
```

### Comparing `sirepo-bluesky-0.6.0/docs/source/simulations.rst` & `sirepo-bluesky-0.6.1/docs/source/simulations.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/setup.py` & `sirepo-bluesky-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/__init__.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/__init__.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/madx_flyer.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/madx_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/shadow_detector.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_detector.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/shadow_handler.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/shadow_handler.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_bluesky.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_bluesky.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                     self.secret,
                 ]
             ).encode()
         )
         req["authHash"] = "v1:" + base64.urlsafe_b64encode(h.digest()).decode()
 
         self.cookies = None
-        res = self._post_json("bluesky-auth", req)
+        res = self._post_json("auth-bluesky-login", req)
         if not ("state" in res and res["state"] == "ok"):
             raise SirepoBlueskyClientException(f"bluesky_auth failed: {res}")
         self.sim_type = sim_type
         self.sim_id = sim_id
         self.schema = res["schema"]
         self.data = res["data"]
         return self.data, self.schema
```

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_flyer.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/sirepo_ophyd.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/sirepo_ophyd.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/srw_detector.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/srw_detector.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/srw_handler.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/srw_handler.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/tests/conftest.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_shadow_det.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_shadow_det.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
         "sigdix",
         "sigdiz",
         "sigmax",
         "sigmaxpzp",
         "sigmaxz",
         "sigmaz",
         "x",
+        "xi_x",
+        "xi_z",
         "xp",
         "z",
         "zp",
         "emit_x",
         "emit_z",
         "sigxdix",
         "sigzdiz",
```

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_sirepo_flyer.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_sirepo_flyer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     sb = SirepoBluesky(server_name)
     data, schema = sb.auth("srw", sim_id)
     assert "beamline" in data["models"]
 
 
 @vcr.use_cassette(f"{cassette_location}/test_smoke_sirepo.yml")
 def test_smoke_sirepo_vcr():
-    _test_smoke_sirepo(sim_id="87XJ4oEb", server_name="http://10.10.10.10:8000")
+    _test_smoke_sirepo(sim_id="00000000", server_name="http://localhost:8000")
 
 
 @pytest.mark.docker
 def test_smoke_sirepo_docker():
     _test_smoke_sirepo(sim_id="00000000", server_name="http://localhost:8000")
 
 
@@ -85,13 +85,13 @@
         durations.append(t.iloc[i]["sirepo_flyer_duration"])
 
     assert (np.array(durations) > 0.0).all(), "fly scan durations are nonpositive"
 
 
 @vcr.use_cassette(f"{cassette_location}/test_sirepo_flyer.yml")
 def test_sirepo_flyer_vcr(RE_no_plot, db, tmpdir):
-    _test_sirepo_flyer(RE_no_plot, db, tmpdir, sim_id="87XJ4oEb", server_name="http://10.10.10.10:8000")
+    _test_sirepo_flyer(RE_no_plot, db, tmpdir, sim_id="00000000", server_name="http://localhost:8000")
 
 
 @pytest.mark.docker
 def test_sirepo_flyer_docker(RE_no_plot, db, tmpdir):
     _test_sirepo_flyer(RE_no_plot, db, tmpdir, sim_id="00000000", server_name="http://localhost:8000")
```

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky/tests/test_srw_det.py` & `sirepo-bluesky-0.6.1/sirepo_bluesky/tests/test_srw_det.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 @vcr.use_cassette(f"{cassette_location}/test_srw_detector.yml")
 def test_srw_detector_vcr(RE, db, tmpdir):
     _test_srw_detector(
         RE,
         db,
         tmpdir,
         sim_type="srw",
-        sim_id="e75qHII6",
-        server_name="http://10.10.10.10:8000",
+        sim_id="00000001",
+        server_name="http://localhost:8000",
     )
 
 
 @pytest.mark.docker
 def test_srw_detector_docker(RE, db, tmpdir):
     _test_srw_detector(
         RE,
@@ -119,16 +119,16 @@
 @vcr.use_cassette(f"{cassette_location}/test_srw_det_grid_scan.yml")
 def test_srw_det_grid_scan_vcr(RE, db, tmpdir):
     _test_srw_det_grid_scan(
         RE,
         db,
         tmpdir,
         sim_type="srw",
-        sim_id="e75qHII6",
-        server_name="http://10.10.10.10:8000",
+        sim_id="00000001",
+        server_name="http://localhost:8000",
     )
 
 
 @pytest.mark.docker
 def test_srw_det_grid_scan_docker(RE, db, tmpdir):
     _test_srw_det_grid_scan(
         RE,
```

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/PKG-INFO` & `sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirepo-bluesky
-Version: 0.6.0
+Version: 0.6.1
 Summary: Sirepo-Bluesky interface
 Home-page: https://github.com/NSLS-II/sirepo-bluesky
 Author: Brookhaven National Laboratory
 Author-email: mrakitin@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `sirepo-bluesky-0.6.0/sirepo_bluesky.egg-info/SOURCES.txt` & `sirepo-bluesky-0.6.1/sirepo_bluesky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.0/versioneer.py` & `sirepo-bluesky-0.6.1/versioneer.py`

 * *Files identical despite different names*


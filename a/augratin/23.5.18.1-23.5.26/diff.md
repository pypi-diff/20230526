# Comparing `tmp/augratin-23.5.18.1.tar.gz` & `tmp/augratin-23.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.5.18.1.tar", last modified: Thu May 18 18:37:36 2023, max compression
+gzip compressed data, was "augratin-23.5.26.tar", last modified: Fri May 26 15:52:55 2023, max compression
```

## Comparing `augratin-23.5.18.1.tar` & `augratin-23.5.26.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.142726 augratin-23.5.18.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.18.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5080 2023-05-18 18:37:36.142726 augratin-23.5.18.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4303 2023-05-18 18:31:11.000000 augratin-23.5.18.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.129727 augratin-23.5.18.1/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/__init__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    41921 2023-05-18 18:27:05.000000 augratin-23.5.18.1/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.138726 augratin-23.5.18.1/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.18.1/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.141726 augratin-23.5.18.1/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.18.1/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13852 2023-05-18 16:38:33.000000 augratin-23.5.18.1/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.18.1/augratin/lib/omnirig_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       49 2023-05-18 18:32:25.000000 augratin-23.5.18.1/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-18 18:37:36.132726 augratin-23.5.18.1/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5080 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-18 18:37:36.000000 augratin-23.5.18.1/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1144 2023-05-18 18:32:28.000000 augratin-23.5.18.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-18 18:37:36.142726 augratin-23.5.18.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.631701 augratin-23.5.26/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.26/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5141 2023-05-26 15:52:55.629701 augratin-23.5.26/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4366 2023-05-26 15:51:22.000000 augratin-23.5.26/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.575701 augratin-23.5.26/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42152 2023-05-26 15:49:25.000000 augratin-23.5.26/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.613701 augratin-23.5.26/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27092 2023-05-17 23:53:10.000000 augratin-23.5.26/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.623701 augratin-23.5.26/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.26/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13852 2023-05-18 16:38:33.000000 augratin-23.5.26/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.26/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-26 15:49:50.000000 augratin-23.5.26/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 15:52:55.591701 augratin-23.5.26/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5141 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-26 15:52:55.000000 augratin-23.5.26/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-26 15:50:00.000000 augratin-23.5.26/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-26 15:52:55.631701 augratin-23.5.26/setup.cfg
```

### Comparing `augratin-23.5.18.1/LICENSE` & `augratin-23.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/PKG-INFO` & `augratin-23.5.26/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.18.1
+Version: 23.5.26
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-26] Added Ubuntu dark mode if adwaita-qt is installed.
 - [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
```

### Comparing `augratin-23.5.18.1/README.md` & `augratin-23.5.26/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-26] Added Ubuntu dark mode if adwaita-qt is installed.
 - [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
```

### Comparing `augratin-23.5.18.1/augratin/__main__.py` & `augratin-23.5.26/augratin/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 
 # from PyQt5.QtWebEngineWidgets import QWebEngineView
 
 
 import requests
 import folium
 
+if os.environ.get("XDG_CURRENT_DESKTOP", False) == "GNOME":
+    os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
+    os.environ["QT_STYLE_OVERRIDE"] = "Adwaita-Dark"
+
 try:
     from augratin.lib.version import __version__
     from augratin.lib.cat_interface import CAT
 
     if sys.platform == "win32":
         from augratin.lib.omnirig_interface import OmniRigClient
 except ModuleNotFoundError:
@@ -49,18 +53,21 @@
 
     if sys.platform == "win32":
         from lib.omnirig_interface import OmniRigClient
 
 __author__ = "Michael C. Bridak, K6GTE"
 __license__ = "GNU General Public License v3.0"
 
-os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
 
 loader = pkgutil.get_loader("augratin")
-WORKING_PATH = os.path.dirname(loader.get_filename())
+if loader is not None:
+    WORKING_PATH = os.path.dirname(loader.get_filename())
+else:
+    WORKING_PATH = "./"
+# WORKING_PATH = os.path.dirname(loader.get_filename())
 
 logger = logging.getLogger("__name__")
 handler = logging.StreamHandler()
 formatter = logging.Formatter(
     datefmt="%H:%M:%S",
     fmt="[%(asctime)s] %(levelname)s %(module)s - %(funcName)s Line %(lineno)d:\n%(message)s",
 )
```

### Comparing `augratin-23.5.18.1/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.26/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/data/dialog.ui` & `augratin-23.5.26/augratin/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.26/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.26/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.26/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/lib/cat_interface.py` & `augratin-23.5.26/augratin/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin/lib/omnirig_interface.py` & `augratin-23.5.26/augratin/lib/omnirig_interface.py`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/augratin.egg-info/PKG-INFO` & `augratin-23.5.26/augratin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.5.18.1
+Version: 23.5.26
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 All contacts are stored in an ADIF file in your home directory,
 which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-26] Added Ubuntu dark mode if adwaita-qt is installed.
 - [23-5-18] Fix crashes related to if flrig running w/ no radio, or flrig closes. Add dialog message window to initial startup if CAT control failed. For some reason I was missing the 17m band. Added back band selector for those who have CAT.
 - [23-5-17] Reworked bandmap display. Spots with QRT in comment are now muted. Center bandmap on RX freq when changing vfo or zooming display. Provided Non CAT control users to change bands.
 - [23-5-15] Start big code changes to impliment better bandmap.
 - [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
```

### Comparing `augratin-23.5.18.1/augratin.egg-info/SOURCES.txt` & `augratin-23.5.26/augratin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augratin-23.5.18.1/pyproject.toml` & `augratin-23.5.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.5.18.1"
+version = "23.5.26"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
```


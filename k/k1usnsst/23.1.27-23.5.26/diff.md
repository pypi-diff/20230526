# Comparing `tmp/k1usnsst-23.1.27.tar.gz` & `tmp/k1usnsst-23.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k1usnsst-23.1.27.tar", last modified: Fri Jan 27 16:45:29 2023, max compression
+gzip compressed data, was "k1usnsst-23.5.26.tar", last modified: Fri May 26 16:42:07 2023, max compression
```

## Comparing `k1usnsst-23.1.27.tar` & `k1usnsst-23.5.26.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.220994 k1usnsst-23.1.27/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     1071 2022-03-17 15:01:31.000000 k1usnsst-23.1.27/LICENSE
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-01-27 16:45:29.220994 k1usnsst-23.1.27/PKG-INFO
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     3883 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/README.md
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.180995 k1usnsst-23.1.27/k1usnsst/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/__init__.py
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)    42311 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/__main__.py
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.204995 k1usnsst-23.1.27/k1usnsst/data/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/JetBrainsMono-Regular.ttf
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)      256 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/cwmacros_sst.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     7208 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/dialog.ui
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)      216 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/k6gte-k1usnsst.desktop
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)    30121 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/k6gte-k1usnsst.png
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)    22264 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/main.ui
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)    16248 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/data/settings.ui
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.212994 k1usnsst-23.1.27/k1usnsst/icon/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)      605 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/icon/gear16x16.png
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/icon/radio_green.png
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/icon/radio_grey.png
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)      957 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/icon/radio_red.png
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.216994 k1usnsst-23.1.27/k1usnsst/lib/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/lib/__init__.py
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     1589 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/lib/cwinterface.py
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)    13810 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/lib/lookup.py
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     3957 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/k1usnsst/lib/settings.py
-drwxrwxr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:45:29.192995 k1usnsst-23.1.27/k1usnsst.egg-info/
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/PKG-INFO
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)      697 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/SOURCES.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)        1 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/dependency_links.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)       51 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/entry_points.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)       25 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/requires.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)       19 2023-01-27 16:45:29.000000 k1usnsst-23.1.27/k1usnsst.egg-info/top_level.txt
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)     1125 2023-01-27 16:44:51.000000 k1usnsst-23.1.27/pyproject.toml
--rw-rw-r--   0 mbridak   (1000) mbridak   (1000)       38 2023-01-27 16:45:29.220994 k1usnsst-23.1.27/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1071 2022-03-17 15:01:31.000000 k1usnsst-23.5.26/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3883 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.490455 k1usnsst-23.5.26/k1usnsst/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42473 2023-05-26 16:38:40.000000 k1usnsst-23.5.26/k1usnsst/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.496455 k1usnsst-23.5.26/k1usnsst/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      256 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/cwmacros_sst.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7208 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      216 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30121 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22264 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16248 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/data/settings.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.498455 k1usnsst-23.5.26/k1usnsst/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.499455 k1usnsst-23.5.26/k1usnsst/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1589 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13810 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3957 2023-01-27 16:44:51.000000 k1usnsst-23.5.26/k1usnsst/lib/settings.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-26 16:42:07.493455 k1usnsst-23.5.26/k1usnsst.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4652 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      697 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-05-26 16:42:07.000000 k1usnsst-23.5.26/k1usnsst.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1125 2023-05-26 16:39:22.000000 k1usnsst-23.5.26/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-26 16:42:07.500455 k1usnsst-23.5.26/setup.cfg
```

### Comparing `k1usnsst-23.1.27/LICENSE` & `k1usnsst-23.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/PKG-INFO` & `k1usnsst-23.5.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1usnsst
-Version: 23.1.27
+Version: 23.5.26
 Summary: K1USN SST Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/k1usnsst
 Project-URL: Bug Tracker, https://github.com/mbridak/k1usnsst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `k1usnsst-23.1.27/README.md` & `k1usnsst-23.5.26/README.md`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/__main__.py` & `k1usnsst-23.5.26/k1usnsst/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     from lib.cwinterface import CW
     from lib.lookup import QRZlookup
     from lib.settings import Settings
 
 
 # pylint: disable=c-extension-no-member
 
+if os.environ.get("XDG_CURRENT_DESKTOP", False) == "GNOME":
+    os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
+    os.environ["QT_STYLE_OVERRIDE"] = "Adwaita-Dark"
 
 def load_fonts_from_dir(directory: str) -> set:
     """
     Well it loads fonts from a directory...
     """
     font_families = set()
     for _fi in QDir(directory).entryInfoList(["*.ttf", "*.woff", "*.woff2"]):
```

### Comparing `k1usnsst-23.1.27/k1usnsst/data/JetBrainsMono-Regular.ttf` & `k1usnsst-23.5.26/k1usnsst/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/data/dialog.ui` & `k1usnsst-23.5.26/k1usnsst/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/data/k6gte-k1usnsst.png` & `k1usnsst-23.5.26/k1usnsst/data/k6gte-k1usnsst.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/data/main.ui` & `k1usnsst-23.5.26/k1usnsst/data/main.ui`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/data/settings.ui` & `k1usnsst-23.5.26/k1usnsst/data/settings.ui`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/icon/gear16x16.png` & `k1usnsst-23.5.26/k1usnsst/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/icon/radio_green.png` & `k1usnsst-23.5.26/k1usnsst/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/icon/radio_grey.png` & `k1usnsst-23.5.26/k1usnsst/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/icon/radio_red.png` & `k1usnsst-23.5.26/k1usnsst/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/lib/cwinterface.py` & `k1usnsst-23.5.26/k1usnsst/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/lib/lookup.py` & `k1usnsst-23.5.26/k1usnsst/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst/lib/settings.py` & `k1usnsst-23.5.26/k1usnsst/lib/settings.py`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/k1usnsst.egg-info/PKG-INFO` & `k1usnsst-23.5.26/k1usnsst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k1usnsst
-Version: 23.1.27
+Version: 23.5.26
 Summary: K1USN SST Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/k1usnsst
 Project-URL: Bug Tracker, https://github.com/mbridak/k1usnsst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `k1usnsst-23.1.27/k1usnsst.egg-info/SOURCES.txt` & `k1usnsst-23.5.26/k1usnsst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k1usnsst-23.1.27/pyproject.toml` & `k1usnsst-23.5.26/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "k1usnsst" 
-version = "23.1.27"
+version = "23.5.26"
 description = "K1USN SST Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```


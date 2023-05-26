# Comparing `tmp/Fletxible-0.5.6.tar.gz` & `tmp/Fletxible-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.6.tar", last modified: Fri May 26 17:20:55 2023, max compression
+gzip compressed data, was "Fletxible-0.5.7.tar", last modified: Fri May 26 17:44:47 2023, max compression
```

## Comparing `Fletxible-0.5.6.tar` & `Fletxible-0.5.7.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.940923 Fletxible-0.5.6/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.935411 Fletxible-0.5.6/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      693 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.6/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:20:55.940534 Fletxible-0.5.6/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.6/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.935988 Fletxible-0.5.6/components/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/block.py
--rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/typography.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.937755 Fletxible-0.5.6/core/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1034 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/drawer.py
--rw-r--r--   0 ahmad      (501) staff       (20)      996 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/header.py
--rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/left_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)      557 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/middle_panel.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/mobile_drop_down.py
--rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/mobile_navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1874 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/navigation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/right_panel.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.938928 Fletxible-0.5.6/fletxible/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:15.000000 Fletxible-0.5.6/fletxible/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3450 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2037 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/fx_template.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1022 2023-05-26 16:21:14.000000 Fletxible-0.5.6/fletxible/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     3307 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-26 17:20:55.940991 Fletxible-0.5.6/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1209 2023-05-26 17:20:27.000000 Fletxible-0.5.6/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.939190 Fletxible-0.5.6/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.6/tests/test_route.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.940210 Fletxible-0.5.6/utilities/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.6/utilities/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.6/utilities/config.py
--rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/links.py
--rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/rail.py
--rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/router.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.931901 Fletxible-0.5.7/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.924622 Fletxible-0.5.7/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      714 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       58 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-26 17:44:47.000000 Fletxible-0.5.7/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.7/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:44:47.931549 Fletxible-0.5.7/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.7/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.925396 Fletxible-0.5.7/components/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.7/components/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.7/components/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.7/components/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.927909 Fletxible-0.5.7/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1034 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      996 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      557 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1874 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.7/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.929507 Fletxible-0.5.7/fletxible/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:15.000000 Fletxible-0.5.7/fletxible/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3450 2023-05-26 14:46:31.000000 Fletxible-0.5.7/fletxible/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1844 2023-05-26 17:19:48.000000 Fletxible-0.5.7/fletxible/command.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2037 2023-05-26 14:46:31.000000 Fletxible-0.5.7/fletxible/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1022 2023-05-26 16:21:14.000000 Fletxible-0.5.7/fletxible/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3307 2023-05-26 14:46:31.000000 Fletxible-0.5.7/fletxible/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-26 17:44:47.931970 Fletxible-0.5.7/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1219 2023-05-26 17:44:43.000000 Fletxible-0.5.7/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.929792 Fletxible-0.5.7/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.7/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:44:47.931184 Fletxible-0.5.7/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.7/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.7/utilities/config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-26 14:46:31.000000 Fletxible-0.5.7/utilities/links.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-26 14:46:31.000000 Fletxible-0.5.7/utilities/rail.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.7/utilities/router.py
```

### Comparing `Fletxible-0.5.6/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.7/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.6
+Version: 0.5.7
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.6/Fletxible.egg-info/SOURCES.txt` & `Fletxible-0.5.7/Fletxible.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 core/middle_panel.py
 core/mobile_drop_down.py
 core/mobile_navigation.py
 core/navigation.py
 core/right_panel.py
 fletxible/__init__.py
 fletxible/base.py
+fletxible/command.py
 fletxible/fx_template.py
 fletxible/main.py
 fletxible/script.py
 tests/test_route.py
 utilities/__init__.py
 utilities/config.py
 utilities/links.py
```

### Comparing `Fletxible-0.5.6/LICENSE` & `Fletxible-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/PKG-INFO` & `Fletxible-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.6
+Version: 0.5.7
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.6/README.md` & `Fletxible-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/components/block.py` & `Fletxible-0.5.7/components/block.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/drawer.py` & `Fletxible-0.5.7/core/drawer.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/header.py` & `Fletxible-0.5.7/core/header.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/middle_panel.py` & `Fletxible-0.5.7/core/middle_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/mobile_drop_down.py` & `Fletxible-0.5.7/core/mobile_drop_down.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/navigation.py` & `Fletxible-0.5.7/core/navigation.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/core/right_panel.py` & `Fletxible-0.5.7/core/right_panel.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/fletxible/base.py` & `Fletxible-0.5.7/fletxible/base.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/fletxible/fx_template.py` & `Fletxible-0.5.7/fletxible/fx_template.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/fletxible/main.py` & `Fletxible-0.5.7/fletxible/main.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/fletxible/script.py` & `Fletxible-0.5.7/fletxible/script.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/setup.py` & `Fletxible-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.6",
+    version="0.5.7",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=[
@@ -19,12 +19,12 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "fletxible-init=command:init",
+            "fletxible-init=fletxible.command:init",
         ],
     },
     keywords=["python web template", "web application", "development"],
 )
```

### Comparing `Fletxible-0.5.6/utilities/links.py` & `Fletxible-0.5.7/utilities/links.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.6/utilities/rail.py` & `Fletxible-0.5.7/utilities/rail.py`

 * *Files identical despite different names*


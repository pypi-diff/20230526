# Comparing `tmp/Fletxible-0.5.4.tar.gz` & `tmp/Fletxible-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.5.4.tar", last modified: Wed May 24 15:03:39 2023, max compression
+gzip compressed data, was "Fletxible-0.5.6.tar", last modified: Fri May 26 17:20:55 2023, max compression
```

## Comparing `Fletxible-0.5.4.tar` & `Fletxible-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,41 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.740515 Fletxible-0.5.4/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.735769 Fletxible-0.5.4/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      429 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       86 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-24 15:03:39.000000 Fletxible-0.5.4/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.4/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-24 15:03:39.740275 Fletxible-0.5.4/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.4/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.738899 Fletxible-0.5.4/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-20 17:37:40.000000 Fletxible-0.5.4/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2201 2023-05-21 12:36:22.000000 Fletxible-0.5.4/logic/build.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2251 2023-05-17 15:53:13.000000 Fletxible-0.5.4/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)     7832 2023-05-21 08:03:38.000000 Fletxible-0.5.4/logic/controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1592 2023-05-23 19:03:08.000000 Fletxible-0.5.4/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)       95 2023-05-21 08:59:30.000000 Fletxible-0.5.4/logic/mapped.py
--rw-r--r--   0 ahmad      (501) staff       (20)      563 2023-05-23 18:58:11.000000 Fletxible-0.5.4/logic/route.py
--rw-r--r--   0 ahmad      (501) staff       (20)     5011 2023-05-23 19:02:08.000000 Fletxible-0.5.4/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-05-21 08:03:38.000000 Fletxible-0.5.4/logic/styles.py
--rw-r--r--   0 ahmad      (501) staff       (20)    12162 2023-05-21 08:59:39.000000 Fletxible-0.5.4/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-24 15:03:39.740601 Fletxible-0.5.4/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1182 2023-05-24 15:03:31.000000 Fletxible-0.5.4/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-24 15:03:39.739653 Fletxible-0.5.4/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)     1049 2023-05-21 07:43:28.000000 Fletxible-0.5.4/tests/test_controls.py
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.4/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.940923 Fletxible-0.5.6/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.935411 Fletxible-0.5.6/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      693 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       48 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-05-26 17:20:55.000000 Fletxible-0.5.6/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.5.6/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-26 17:20:55.940534 Fletxible-0.5.6/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.5.6/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.935988 Fletxible-0.5.6/components/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3313 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/block.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      274 2023-05-26 14:46:31.000000 Fletxible-0.5.6/components/typography.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.937755 Fletxible-0.5.6/core/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1034 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/drawer.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      996 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/header.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      318 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/left_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      557 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/middle_panel.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4525 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/mobile_drop_down.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      419 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/mobile_navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1874 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/navigation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1252 2023-05-26 14:46:31.000000 Fletxible-0.5.6/core/right_panel.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.938928 Fletxible-0.5.6/fletxible/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:15.000000 Fletxible-0.5.6/fletxible/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3450 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2037 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/fx_template.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1022 2023-05-26 16:21:14.000000 Fletxible-0.5.6/fletxible/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     3307 2023-05-26 14:46:31.000000 Fletxible-0.5.6/fletxible/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-26 17:20:55.940991 Fletxible-0.5.6/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1209 2023-05-26 17:20:27.000000 Fletxible-0.5.6/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.939190 Fletxible-0.5.6/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.5.6/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-26 17:20:55.940210 Fletxible-0.5.6/utilities/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-26 17:08:22.000000 Fletxible-0.5.6/utilities/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      195 2023-05-26 16:04:02.000000 Fletxible-0.5.6/utilities/config.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      660 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/links.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      666 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/rail.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      366 2023-05-26 14:46:31.000000 Fletxible-0.5.6/utilities/router.py
```

### Comparing `Fletxible-0.5.4/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.5.6/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.4
+Version: 0.5.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.4/LICENSE` & `Fletxible-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.4/PKG-INFO` & `Fletxible-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.5.4
+Version: 0.5.6
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.5.4/README.md` & `Fletxible-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `Fletxible-0.5.4/setup.py` & `Fletxible-0.5.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.5.4",
+    version="0.5.6",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
-    packages=["logic"],
-    install_requires=["click>=8.1.3", "flet>=0.7.1", "PyYAML>=6.0"],
+    packages=[
+        "core",
+        "components",
+        "utilities",
+        "fletxible",
+    ],
+    install_requires=["click>=8.1.3", "flet>=0.7.4", "PyYAML>=6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": [
-            "fletxible-init=logic.cli:init",
-            "fletxible-build=logic.build:build",
+            "fletxible-init=command:init",
         ],
     },
     keywords=["python web template", "web application", "development"],
 )
```


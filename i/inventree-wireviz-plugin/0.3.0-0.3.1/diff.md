# Comparing `tmp/inventree-wireviz-plugin-0.3.0.tar.gz` & `tmp/inventree-wireviz-plugin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.0.tar", last modified: Fri May 26 02:25:57 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.1.tar", last modified: Fri May 26 02:36:04 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.3.0.tar` & `inventree-wireviz-plugin-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18143 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18290 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 02:36:04.000000 inventree-wireviz-plugin-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 02:35:50.000000 inventree-wireviz-plugin-0.3.1/setup.py
```

### Comparing `inventree-wireviz-plugin-0.3.0/LICENSE` & `inventree-wireviz-plugin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.0/PKG-INFO` & `inventree-wireviz-plugin-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.3.0/README.md` & `inventree-wireviz-plugin-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.3.1/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.0/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.3.1/inventree_wireviz/wireviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,14 +522,19 @@
             unit: The unit of the quantity
             base_unit: The base unit of the part
         
         Returns:
             The converted quantity, or the original quantity if conversion failed
         """
 
+        # Ignore unit if quantity not given
+        # Will be specified in the part units anyway
+        if not unit:
+            return quantity
+
         logger.debug(f"WirevizPlugin: Converting quantity {quantity} {unit} to {base_unit}")
 
         q = f"{quantity} {unit}"
 
         try:
             val = self.ureg.Quantity(q)
```

### Comparing `inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.3.1/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.0/setup.py` & `inventree-wireviz-plugin-0.3.1/setup.py`

 * *Files identical despite different names*


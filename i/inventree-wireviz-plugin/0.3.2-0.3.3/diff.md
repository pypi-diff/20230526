# Comparing `tmp/inventree-wireviz-plugin-0.3.2.tar.gz` & `tmp/inventree-wireviz-plugin-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.2.tar", last modified: Fri May 26 02:45:17 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.3.tar", last modified: Fri May 26 06:36:34 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.3.2.tar` & `inventree-wireviz-plugin-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 02:45:17.000000 inventree-wireviz-plugin-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 02:45:09.000000 inventree-wireviz-plugin-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/setup.py
```

### Comparing `inventree-wireviz-plugin-0.3.2/LICENSE` & `inventree-wireviz-plugin-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.2/PKG-INFO` & `inventree-wireviz-plugin-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.3.2
+Version: 0.3.3
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.3.2/README.md` & `inventree-wireviz-plugin-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.2/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.2/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.3.3/inventree_wireviz/wireviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,20 @@
 
     SETTINGS = {
         "WIREVIZ_PATH": {
             'name': 'Wireviz Upload Path',
             'description': 'Path to store uploaded wireviz template files (relative to media root)',
             'default': 'wireviz',
         },
+        "DELETE_OLD_FILES": {
+            'name': 'Delete Old Files',
+            'description': 'Delete old wireviz files when uploading a new wireviz file',
+            'default': True,
+            'validator': bool,
+        },
         "EXTRACT_BOM": {
             'name': 'Extract BOM Data',
             'description': 'Automatically extract BOM data from wireviz diagrams',
             'default': True,
             'validator': bool,
         },
         "CLEAR_BOM_DATA": {
@@ -155,14 +161,28 @@
 
                 # Store a reference to the parent Part
                 self.part = attachment.part
 
                 # Check if the attachment is a .wireviz file
                 if filename.endswith(".wireviz"):
                     self.process_wireviz_file(filename)
+
+                    # Delete *old* wireviz files
+                    if self.get_setting('DELETE_OLD_FILES'):
+                        for attach in PartAttachment.objects.filter(part=self.part):
+                            # Don't delete this one!
+                            if attach.pk == attachment.pk:
+                                continue
+
+                            fn = attach.attachment.name
+
+                            # Delete old wireviz files
+                            if fn.endswith(".wireviz"):
+                                attach.delete()
+
             except PartAttachment.DoesNotExist:
                 pass
     
     def process_wireviz_file(self, wv_file: str, part: Part = None):
         """Process a wireviz file, and extract the relevant information."""
 
         logger.info(f"WirevizPlugin: Processing wireviz file: {wv_file}")
```

### Comparing `inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.3.2
+Version: 0.3.3
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.3.2/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.2/setup.py` & `inventree-wireviz-plugin-0.3.3/setup.py`

 * *Files identical despite different names*


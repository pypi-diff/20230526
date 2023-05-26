# Comparing `tmp/inventree-wireviz-plugin-0.1.0.tar.gz` & `tmp/inventree-wireviz-plugin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.1.0.tar", last modified: Wed May 24 23:25:45 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.2.0.tar", last modified: Fri May 26 00:48:56 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.1.0.tar` & `inventree-wireviz-plugin-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-24 23:25:45.000000 inventree-wireviz-plugin-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-24 23:25:35.000000 inventree-wireviz-plugin-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/setup.py
```

### Comparing `inventree-wireviz-plugin-0.1.0/LICENSE` & `inventree-wireviz-plugin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.1.0/PKG-INFO` & `inventree-wireviz-plugin-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-Metadata-Version: 2.1
-Name: inventree-wireviz-plugin
-Version: 0.1.0
-Summary: Wireviz plugin for InvenTree
-Home-page: https://github.com/inventree/inventree-wireviz-plugin
-Author: Oliver Walters
-Author-email: oliver.henry.walters@gmail.com
-License: MIT
-Keywords: inventree inventory wireviz wiring cable harness
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/inventree-wireviz-plugin)](https://pypi.org/project/inventree-wireviz-plugin/)
+![PEP](https://github.com/inventree/inventree-wireviz/actions/workflows/pep.yaml/badge.svg)
 
 # inventree-wireviz
 
 The **inventree-wireviz** plugin provides direct integration for [wireviz](https://github.com/formatc1702/WireViz), a text-based wiring harness specification tool.
 
 TODO: Description
```

### Comparing `inventree-wireviz-plugin-0.1.0/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.1.0/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.2.0/inventree_wireviz/wireviz.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.db import transaction
 
 from plugin import InvenTreePlugin
 from plugin.mixins import EventMixin, PanelMixin, SettingsMixin
 
+from company.models import ManufacturerPart, SupplierPart
 from part.models import BomItem, Part, PartAttachment
 from part.views import PartDetail
 
 from .version import PLUGIN_VERSION
 
 
 logger = logging.getLogger('inventree')
@@ -211,39 +212,34 @@
 
         subdir = self.get_setting('WIREVIZ_PATH')
 
         logger.info(f"WirevizPlugin: Prepending wireviz data from {subdir}")
 
         if subdir:
             path = os.path.join(settings.MEDIA_ROOT, subdir)
+            path = os.path.abspath(path)
 
             if os.path.exists(path):
                 for filename in os.listdir(path):
                     if filename.lower().endswith('.wireviz'):
                         filepath = os.path.join(path, filename)
 
-                        logger.debug(f"WirevizPlugin: Loading wireviz template file: {filepath}")
+                        logger.info(f"WirevizPlugin: Loading wireviz template file: {filepath}")
 
                         with open(filepath, 'r') as f:
                             prepend_data += f.read()
                             prepend_data += '\n\n'
 
         return prepend_data
 
     def add_part_images(self, harness: Harness):
         """Add part images to the wireviz harness"""
         
         logger.warning("WirevizPlugin: Adding part images is not yet supported")
         
-        # For now, strip out any images
-        for ref in harness.connectors:
-            harness.connectors[ref].image = None
-        for ref in harness.cables:
-            harness.cables[ref].image = None
-
         # TODO: Implement native image support
 
         """
         # Path to part images directory
         img_path = pathlib.Path(settings.MEDIA_ROOT)
 
         for designator, part in self.part_map.items():
@@ -301,14 +297,18 @@
 
             sub_part = self.match_part(line)
 
             if not sub_part:
                 self.add_warning(f"No matching part for line: {description}")
                 continue
 
+            if sub_part == self.part:
+                self.add_error(f"Part {sub_part} is the same as the parent part")
+                continue
+
             # Associate the internal part with the designators
             for designator in designators:
                 self.part_map[designator] = sub_part
 
             # Construct a new BomItem object
             bom_items.append(BomItem(
                 part=self.part,
@@ -331,29 +331,74 @@
         Arguments:
             line: A dictionary of BOM line item data
         
         Returns:
             A Part instance, or None
         """
 
-        part = None
-
-        # Extract part number from line
-        if pn := line.get('pn', None):
-
-            # Try to match by part name
-            part = Part.objects.filter(name=pn).first()
-
-            # Try to match by IPN
-            if not part:
-                part = Part.objects.filter(IPN=pn).first()
+        # Extract data from BOM entry
+        pn = line.get('pn', None)
+        description = line.get('description', None)
+        mpn = line.get('mpn', None)
+        spn = line.get('spn', None)
+
+        # Match pn -> part.IPN
+        if pn:
+            results = Part.objects.filter(IPN=pn)
+            if results.count() == 1:
+                return results.first()
+
+            # Match pn -> part.name
+            results = Part.objects.filter(name=pn)
+            if results.count() == 1:
+                return results.first()
+
+        # Match description -> part.description
+        if description:
+            results = Part.objects.filter(description=description)
+            if results.count() == 1:
+                return results.first()
+
+        # Match mpn -> manufacturer_part.MPN
+        if mpn:
+            results = ManufacturerPart.objects.filter(MPN=mpn)
+            if results.count() == 1:
+                return results.first().part
+        
+        # Match spn -> supplier_part.SKU
+        if spn:
+            results = SupplierPart.objects.filter(SKU=spn)
+            if results.count() == 1:
+                return results.first().part
+
+        # For a 'wire', append the wire color and try again
+        if pn and description and description.startswith('Wire, '):
+            wire_data = [x.strip() for x in description.split(',')]
+
+            """
+            For individual wires, the PN does not include the color.
+            For example, a wire might have a PN "26AWG-PTFE"
+            To fully quality the wire, we need to append the color.
+            So, we might get a value like "26AWG-PTFE-YE" for a yellow wire.
+            """
 
-        # TODO: Try to match by other methods?
+            if len(wire_data) >= 3:
+                color = wire_data[2]
+            
+            wire_pn = f"{pn}-{color}"
 
-        return part
+            # Match wire_pn -> part.IPN
+            results = Part.objects.filter(IPN=wire_pn)
+            if results.count() == 1:
+                return results.first()
+        
+            # Match wire_pn -> part.name
+            results = Part.objects.filter(name=wire_pn)
+            if results.count() == 1:
+                return results.first()
     
     @transaction.atomic
     def generate_html_output(self, harness: Harness):
         """Generate HTML output from a wireviz harness."""
 
         logger.info("WirevizPlugin: Generating HTML output for wireviz harness")
```

### Comparing `inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.1.0
+Version: 0.2.0
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/inventree-wireviz-plugin)](https://pypi.org/project/inventree-wireviz-plugin/)
+![PEP](https://github.com/inventree/inventree-wireviz/actions/workflows/pep.yaml/badge.svg)
 
 # inventree-wireviz
 
 The **inventree-wireviz** plugin provides direct integration for [wireviz](https://github.com/formatc1702/WireViz), a text-based wiring harness specification tool.
 
 TODO: Description
```

### Comparing `inventree-wireviz-plugin-0.1.0/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.1.0/setup.py` & `inventree-wireviz-plugin-0.2.0/setup.py`

 * *Files identical despite different names*


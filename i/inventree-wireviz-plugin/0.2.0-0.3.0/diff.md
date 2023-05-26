# Comparing `tmp/inventree-wireviz-plugin-0.2.0.tar.gz` & `tmp/inventree-wireviz-plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.2.0.tar", last modified: Fri May 26 00:48:56 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.0.tar", last modified: Fri May 26 02:25:57 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.2.0.tar` & `inventree-wireviz-plugin-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 00:48:56.000000 inventree-wireviz-plugin-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 00:48:46.000000 inventree-wireviz-plugin-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18143 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 02:25:57.000000 inventree-wireviz-plugin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 02:25:48.000000 inventree-wireviz-plugin-0.3.0/setup.py
```

### Comparing `inventree-wireviz-plugin-0.2.0/LICENSE` & `inventree-wireviz-plugin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.2.0/PKG-INFO` & `inventree-wireviz-plugin-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.2.0/README.md` & `inventree-wireviz-plugin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.2.0/inventree_wireviz/templates/wireviz/harness_panel.html` & `inventree-wireviz-plugin-0.3.0/inventree_wireviz/templates/wireviz/harness_panel.html`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.2.0/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.3.0/inventree_wireviz/wireviz.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from django.core.files.base import ContentFile
 from django.db import transaction
 
 from plugin import InvenTreePlugin
 from plugin.mixins import EventMixin, PanelMixin, SettingsMixin
 
 from company.models import ManufacturerPart, SupplierPart
+from InvenTree.api_version import INVENTREE_API_VERSION
 from part.models import BomItem, Part, PartAttachment
 from part.views import PartDetail
 
 from .version import PLUGIN_VERSION
 
 
 logger = logging.getLogger('inventree')
@@ -121,15 +122,15 @@
             instance = view.get_object()
         except AttributeError:
             return panels
     
         if isinstance(view, PartDetail):
             part = instance
 
-            logger.info(f"Checking for wireviz file for part {part}")
+            logger.debug(f"Checking for wireviz file for part {part}")
 
             if self.get_harness_data(part):
                 panels.append({
                     'title': 'WireViz Harness',
                     'icon': 'fas fa-plug',
                     'content_template': 'wireviz/harness_panel.html',
                     'javascript_template': 'wireviz/harness_panel.js',
@@ -162,14 +163,24 @@
                 pass
     
     def process_wireviz_file(self, wv_file: str, part: Part = None):
         """Process a wireviz file, and extract the relevant information."""
 
         logger.info(f"WirevizPlugin: Processing wireviz file: {wv_file}")
 
+        # Get a unit registry for conversion
+        if INVENTREE_API_VERSION >= 117:
+            # Modern InvenTree versions supply a unit registry
+            from InvenTree.conversion import get_unit_registry
+            self.ureg = get_unit_registry()
+        else:
+            # Fallback to pint unit registry
+            import pint
+            self.ureg = pint.UnitRegistry()
+
         self.errors = []
         self.warnings = []
         self.part_map = {}
 
         # Parse the wireviz file
         filename = os.path.join(settings.MEDIA_ROOT, wv_file)
 
@@ -180,25 +191,33 @@
         with open(filename, 'r') as f:
             wireviz_data = f.read()
 
         if prepend := self.prepend_wireviz_data():
             wireviz_data = prepend + wireviz_data
 
         # Parse the wireviz data
-        harness = parse_wireviz(
-            wireviz_data,
-            return_types='harness',
-        )
+        try:
+            harness = parse_wireviz(
+                wireviz_data,
+                return_types='harness',
+            )
+        except Exception as exc:
+            logger.error(f"WirevizPlugin: Failed to parse wireviz file: {exc}")
+
+            from InvenTree.exceptions import log_error
+            log_error("Wireviz Import")
+            return
 
         # Extract BOM data from the harness
         self.extract_bom_data(harness)
 
         if self.get_setting("ADD_IMAGES"):
             self.add_part_images(harness)
 
+        self.save_bom_data()
         self.generate_html_output(harness)
 
         # Save any error messages to a file
         self.save_error_file()
         self.save_warning_file()
 
     def prepend_wireviz_data(self):
@@ -274,24 +293,21 @@
             harness: A wireviz Harness instance
         """
         logger.info("WirevizPlugin: Extracting BOM data from wireviz harness")
 
         bom = harness.bom()
 
         # A list of BomItem objects to be created
-        bom_items = []
+        self.bom_items = []
 
         for line in bom:
             designators = line.get('designators', [])
             description = line.get('description', None)
             quantity = line.get('qty', None)
-
-            if not description:
-                self.add_error(f"No description for line: {line}")
-                continue
+            unit = line.get('unit', None)
 
             try:
                 quantity = float(quantity)
             except (TypeError, ValueError):
                 self.add_error(f"Invalid quantity for line: {line}")
                 continue
 
@@ -305,29 +321,45 @@
                 self.add_error(f"Part {sub_part} is the same as the parent part")
                 continue
 
             # Associate the internal part with the designators
             for designator in designators:
                 self.part_map[designator] = sub_part
 
+            if unit or sub_part.units:
+                quantity = self.convert_quantity(quantity, unit, sub_part.units)
+
+            if not description:
+                self.add_error(f"No description for line: {line}")
+                continue
+
             # Construct a new BomItem object
-            bom_items.append(BomItem(
+            self.bom_items.append(BomItem(
                 part=self.part,
                 sub_part=sub_part,
                 quantity=quantity,
                 note="Wireviz BOM item"
             ))
 
-        if self.get_setting('EXTRACT_BOM'):
-            if self.get_setting('CLEAR_BOM_DATA'):
-                logger.info(f"WirevizPlugin: Clearing existing BOM data for part {self.part}")
-                self.part.bom_items.all().delete()
-            
-            # Create the new BomItem objects in the database
-            BomItem.objects.bulk_create(bom_items)
+    def save_bom_data(self):
+        """Write the extracted BOM data to the database."""
+
+        if not self.get_setting('EXTRACT_BOM'):
+            return
+        
+        if len(self.errors) > 0:
+            self.add_warning("Not saving BOM data due to errors")
+            return
+
+        if self.get_setting('CLEAR_BOM_DATA'):
+            logger.info(f"WirevizPlugin: Clearing existing BOM data for part {self.part}")
+            self.part.bom_items.all().delete()
+        
+        # Create the new BomItem objects in the database
+        BomItem.objects.bulk_create(self.bom_items)
 
     def match_part(self, line: dict):
         """Attempt to match a BOM line item to an InvenTree part.
         
         Arguments:
             line: A dictionary of BOM line item data
         
@@ -392,95 +424,119 @@
                 return results.first()
         
             # Match wire_pn -> part.name
             results = Part.objects.filter(name=wire_pn)
             if results.count() == 1:
                 return results.first()
     
-    @transaction.atomic
+    def create_or_overwrite_attachment(self, fn, data, comment='Wireviz attachment'):
+        """Create a new attachment, or overwrite an existing attachment.
+        
+        - Check for an existing attachment with the same filename
+        - If it exists, overwrite the data
+        - If it does not exist, create a new attachment
+        """
+
+        for attachment in self.part.attachments.all():
+            if os.path.basename(attachment.attachment.name) == fn:
+                logger.info(f"WirevizPlugin: Overwriting existing attachment {fn}")
+
+                if len(data) == 0:
+                    attachment.delete()
+                    return
+
+                filename = os.path.join(settings.MEDIA_ROOT, attachment.attachment.name)
+
+                with open(filename, 'wb') as fo:
+                    fo.write(data)
+                
+                return
+
+        if len(data) == 0:
+            # Ignore empty file data
+            return
+
+        # No existing attachment found, create a new one
+        PartAttachment.objects.create(
+            part=self.part,
+            attachment=ContentFile(
+                data,
+                name=fn,
+            ),
+            comment=comment,
+            user=None
+        )
+
     def generate_html_output(self, harness: Harness):
         """Generate HTML output from a wireviz harness."""
 
         logger.info("WirevizPlugin: Generating HTML output for wireviz harness")
 
-        # Delete existing HTML output
-        for attachment in self.part.attachments.all():
-            if attachment.attachment.name == self.HARNESS_HTML_FILE:
-                attachment.delete()
-
         bomlist = bom_list(harness.bom())
 
         # For now, we must write to a tempfile
         # In the future, work out how to write to an in-memory file object
         out_file = os.path.join(tempfile.gettempdir(), 'harness_out')
         
         harness.output(filename=out_file, fmt=('svg',), view=False)
         generate_html_output(out_file, bomlist, harness.metadata, harness.options)
 
         # Read the data back in
         with open(out_file + '.html', 'r') as f:
             html_data = f.read()
-
-        # Create a new PartAttachment for the rendered HTML
-        PartAttachment.objects.create(
-            part=self.part,
-            attachment=ContentFile(
-                html_data,
-                name=self.HARNESS_HTML_FILE,
-            ),
-            comment='Wireviz Harness (autogenerated from .wireviz file)',
-            user=None
+        
+        self.create_or_overwrite_attachment(
+            self.HARNESS_HTML_FILE,
+            html_data.encode(),
+            comment='Wireviz Harness (autogenerated from .wireviz file)'
         )
 
     def add_error(self, msg: str):
         """Add an error message to the list of errors."""
 
         self.errors.append(msg)
         logger.error(f"WireViz: {msg}")
 
     def add_warning(self, msg: str):
         """Add a warning message to the list of errors."""
 
         self.warnings.append(msg)
         logger.warning(f"WireViz: {msg}")
 
-    @transaction.atomic
     def save_error_file(self):
         """Save an error file containing all error messages"""
 
-        # First, delete any existing error file
-        for attachment in self.part.attachments.all():
-            if attachment.attachment.name == self.ERROR_MSG_FILE:
-                attachment.delete()
-        
-        # Create a new error file
-        if len(self.errors) > 0:
-            PartAttachment.objects.create(
-                part=self.part,
-                attachment=ContentFile(
-                    '\n'.join(self.errors).encode(),
-                    name=self.ERROR_MSG_FILE,
-                ),
-                comment='Wireviz Error Messages',
-                user=None
-            )
+        data = '\n'.join(self.errors).encode()
+        self.create_or_overwrite_attachment(self.ERROR_MSG_FILE, data, comment='Wireviz error messages')
     
-    @transaction.atomic
     def save_warning_file(self):
         """Save a warning file containing all warning messages"""
 
-        # First, delete any existing warning file
-        for attachment in self.part.attachments.all():
-            if attachment.attachment.name == self.WARNING_MSG_FILE:
-                attachment.delete()
+        data = '\n'.join(self.warnings).encode()
+        self.create_or_overwrite_attachment(self.WARNING_MSG_FILE, data, comment='Wireviz warning messages')
+
+    def convert_quantity(self, quantity, unit, base_unit):
+        """Convert a provided physical quantity into the "base units" of the part.
         
-        # Create a new warning file
-        if len(self.warnings) > 0:
-            PartAttachment.objects.create(
-                part=self.part,
-                attachment=ContentFile(
-                    '\n'.join(self.warnings).encode(),
-                    name=self.WARNING_MSG_FILE,
-                ),
-                comment='Wireviz Warning Messages',
-                user=None
-            )
+        Args:
+            quantity: The quantity to convert
+            unit: The unit of the quantity
+            base_unit: The base unit of the part
+        
+        Returns:
+            The converted quantity, or the original quantity if conversion failed
+        """
+
+        logger.debug(f"WirevizPlugin: Converting quantity {quantity} {unit} to {base_unit}")
+
+        q = f"{quantity} {unit}"
+
+        try:
+            val = self.ureg.Quantity(q)
+
+            if base_unit:
+                val = val.to(base_unit)
+
+            return float(val.magnitude)
+        except Exception:
+            self.add_error(f"Could not convert quantity {quantity} {unit} to {base_unit}")
+            return quantity
```

### Comparing `inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/PKG-INFO` & `inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wireviz-plugin
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wireviz plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-wireviz-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree inventory wireviz wiring cable harness
 Requires-Python: >=3.9
```

### Comparing `inventree-wireviz-plugin-0.2.0/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.3.0/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.2.0/setup.py` & `inventree-wireviz-plugin-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     keywords="inventree inventory wireviz wiring cable harness",
     url="https://github.com/inventree/inventree-wireviz-plugin",
     license="MIT",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         'wireviz',
+        'pint',
     ],
     setup_requires=[
         "wheel",
         "twine",
     ],
     python_requires=">=3.9",
     entry_points={
```


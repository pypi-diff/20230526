# Comparing `tmp/itkdb_gtk-0.0.7.tar.gz` & `tmp/itkdb_gtk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.7.tar", last modified: Thu May 25 15:35:02 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.8.tar", last modified: Fri May 26 18:34:37 2023, max compression
```

## Comparing `itkdb_gtk-0.0.7.tar` & `itkdb_gtk-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.215579 itkdb_gtk-0.0.7/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-25 15:35:02.215180 itkdb_gtk-0.0.7/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.7/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.211917 itkdb_gtk-0.0.7/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.7/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowAttachments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowComments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowDefects.py
--rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-25 15:34:56.000000 itkdb_gtk-0.0.7/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.7/itkdb_gtk/checkJSon.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.7/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.7/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.7/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.7/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.7/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.7/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.7/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    19659 2023-05-25 15:33:19.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadMultipleTests.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.214600 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1141 2023-05-25 15:30:22.000000 itkdb_gtk-0.0.7/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-25 15:35:02.215713 itkdb_gtk-0.0.7/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.830705 itkdb_gtk-0.0.8/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-26 18:34:37.830267 itkdb_gtk-0.0.8/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.8/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.827098 itkdb_gtk-0.0.8/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.8/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.8/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowAttachments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowComments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/ShowDefects.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-26 18:34:32.000000 itkdb_gtk-0.0.8/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.8/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.8/itkdb_gtk/checkJSon.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.8/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.8/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.8/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.8/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.8/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.8/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.8/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    19648 2023-05-26 18:33:54.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadMultipleTests.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.8/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-26 18:34:37.829700 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-26 18:34:37.000000 itkdb_gtk-0.0.8/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1141 2023-05-26 18:31:37.000000 itkdb_gtk-0.0.8/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-26 18:34:37.830832 itkdb_gtk-0.0.8/setup.cfg
```

### Comparing `itkdb_gtk-0.0.7/PKG-INFO` & `itkdb_gtk-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb_gtk
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.7/README.md` & `itkdb_gtk-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.8/itkdb_gtk/GlueWeight.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.0.8/itkdb_gtk/ITkDB.svg`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.8/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.8/itkdb_gtk/ITkDButils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ShowAttachments.py` & `itkdb_gtk-0.0.8/itkdb_gtk/ShowAttachments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ShowComments.py` & `itkdb_gtk-0.0.8/itkdb_gtk/ShowComments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/ShowDefects.py` & `itkdb_gtk-0.0.8/itkdb_gtk/ShowDefects.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/__init__.py` & `itkdb_gtk-0.0.8/itkdb_gtk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import dashBoard
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 
 def dash_board():
     """Launches the dash board."""
     dashBoard.main()
```

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/checkComponent.py` & `itkdb_gtk-0.0.8/itkdb_gtk/checkComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/checkJSon.py` & `itkdb_gtk-0.0.8/itkdb_gtk/checkJSon.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.8/itkdb_gtk/dashBoard.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.8/itkdb_gtk/dbGtkUtils.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.8/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.8/itkdb_gtk/groundingTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.8/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.8/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.8/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/uploadMultipleTests.py` & `itkdb_gtk-0.0.8/itkdb_gtk/uploadMultipleTests.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
 
 
 def handle_test_date(the_date):
     """Edit date."""
     the_date = the_date[:19].replace('T', ' ')
+    return the_date
 
 
 def all_files(root, patterns='*', single_level=False, yield_folders=False):
     """A generator that reruns all files in the given folder.
 
     Args:
     ----
@@ -134,15 +135,15 @@
         button.add(image)
         button.set_tooltip_text("Click to upload test")
         button.connect("clicked", self.upload_test_gui)
         self.hb.pack_end(button)
 
         # Data panel
         grid = Gtk.Grid(column_spacing=5, row_spacing=1)
-        self.mainBox.pack_start(grid, True, False, 0)
+        self.mainBox.pack_start(grid, False, False, 0)
 
         # The test file widgets
         lbl = Gtk.Label(label="Select Test Files: ")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, 0, 1, 1)
 
         btn = Gtk.Button()
@@ -224,16 +225,16 @@
         """Button pressed on tree view."""
         # double click shows attachments
         if event.button == 1 and event.type == Gdk.EventType.DOUBLE_BUTTON_PRESS:
             select = self.tree.get_selection()
             model, iter = select.get_selected()
             if not iter:
                 return
-            
-            self.on_show_attachments(None,  (model, iter, model[iter]))
+
+            self.on_show_attachments(None, (model, iter, model[iter]))
             return
 
         if event.button != 3:
             return
 
         # Create popup menu
         select = self.tree.get_selection()
@@ -369,29 +370,29 @@
         default_site = None
         for ifile in files:
             try:
                 has_errors = False
                 data = json.loads(open(ifile).read())
                 errors, missing = check_data(data)
                 if len(missing):
-                    self.write_message(Path(ifile).name)
+                    self.write_message("{}\n".format(Path(ifile).name))
                     self.write_message("Some keys are missing in the JSon file.\n")
                     self.write_message("{}\n".format("\n".join(['\t'+line for line in missing])))
 
                     if "institution" in missing and len(missing) == 1:
                         if default_site is None:
                             site, use_default = self.get_test_institute()
                             if use_default:
                                 default_site = site
                         else:
                             site = default_site
 
                         if site:
-                            self.data["institution"] = site
-                            self.write_message("Setting Institution to {}\n".format(self.data["institution"]))
+                            data["institution"] = site
+                            self.write_message("Setting Institution to {}\n".format(data["institution"]))
 
                     else:
                         has_errors = True
                         dbGtkUtils.complain("Invalid JSON file\n{}".format('\n'.join(errors)), ifile)
 
                 if not has_errors:
                     attachments = []
@@ -407,15 +408,15 @@
                             if path.exists():
                                 attachments.append(ITkDButils.Attachment(path, att["title"], att["description"]))
                             else:
                                 self.write_message("Ignoring atachment {}".format(data["path"]))
 
                         # We need to delete tis, which is "unofficial"
                         del data["attachments"]
-                        
+
                     model = self.tree.get_model()
                     comments = data.get("comments", [])
                     defects = data.get("defects", [])
                     the_date = handle_test_date(data["date"])
                     model.append([data["component"], data["testType"], data["runNumber"], the_date,
                                   data["institution"], ifile, data, len(attachments), attachments,
                                   len(comments), comments, len(defects), defects])
```

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.8/itkdb_gtk/uploadPetalInformation.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.8/itkdb_gtk/uploadTest.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.8/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb-gtk
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `itkdb_gtk-0.0.7/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.8/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.7/pyproject.toml` & `itkdb_gtk-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```


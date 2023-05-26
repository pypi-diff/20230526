# Comparing `tmp/pqv-0.4.0.tar.gz` & `tmp/pqv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqv-0.4.0.tar", last modified: Wed Apr 26 19:47:22 2023, max compression
+gzip compressed data, was "pqv-0.5.0.tar", last modified: Fri May 26 13:50:49 2023, max compression
```

## Comparing `pqv-0.4.0.tar` & `pqv-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.797957 pqv-0.4.0/
--rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.4.0/LICENSE
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-04-26 19:47:22.797748 pqv-0.4.0/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.4.0/README.md
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.795623 pqv-0.4.0/pqv/
--rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.4.0/pqv/__init__.py
--rw-r--r--   0 pieter     (501) staff       (20)     3905 2023-04-26 19:43:56.000000 pqv-0.4.0/pqv/__main__.py
--rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.4.0/pqv/style.css
-drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-04-26 19:47:22.797468 pqv-0.4.0/pqv.egg-info/
--rw-r--r--   0 pieter     (501) staff       (20)      225 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/PKG-INFO
--rw-r--r--   0 pieter     (501) staff       (20)      236 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/SOURCES.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/dependency_links.txt
--rw-r--r--   0 pieter     (501) staff       (20)       42 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/entry_points.txt
--rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.4.0/pqv.egg-info/not-zip-safe
--rw-r--r--   0 pieter     (501) staff       (20)        4 2023-04-26 19:47:22.000000 pqv-0.4.0/pqv.egg-info/top_level.txt
--rw-r--r--   0 pieter     (501) staff       (20)       38 2023-04-26 19:47:22.798114 pqv-0.4.0/setup.cfg
--rw-r--r--   0 pieter     (501) staff       (20)      529 2023-04-26 19:44:38.000000 pqv-0.4.0/setup.py
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.435360 pqv-0.5.0/
+-rw-r--r--   0 pieter     (501) staff       (20)     1066 2023-02-26 14:17:55.000000 pqv-0.5.0/LICENSE
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-05-26 13:50:49.435047 pqv-0.5.0/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      102 2023-02-26 14:42:52.000000 pqv-0.5.0/README.md
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.432750 pqv-0.5.0/pqv/
+-rw-r--r--   0 pieter     (501) staff       (20)        0 2023-02-26 14:09:31.000000 pqv-0.5.0/pqv/__init__.py
+-rw-r--r--   0 pieter     (501) staff       (20)     4306 2023-05-26 13:42:04.000000 pqv-0.5.0/pqv/__main__.py
+-rw-r--r--   0 pieter     (501) staff       (20)      165 2023-02-26 11:16:27.000000 pqv-0.5.0/pqv/style.css
+drwxr-xr-x   0 pieter     (501) staff       (20)        0 2023-05-26 13:50:49.434770 pqv-0.5.0/pqv.egg-info/
+-rw-r--r--   0 pieter     (501) staff       (20)      225 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/PKG-INFO
+-rw-r--r--   0 pieter     (501) staff       (20)      236 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/SOURCES.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/dependency_links.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       42 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/entry_points.txt
+-rw-r--r--   0 pieter     (501) staff       (20)        1 2023-02-26 14:19:07.000000 pqv-0.5.0/pqv.egg-info/not-zip-safe
+-rw-r--r--   0 pieter     (501) staff       (20)        4 2023-05-26 13:50:49.000000 pqv-0.5.0/pqv.egg-info/top_level.txt
+-rw-r--r--   0 pieter     (501) staff       (20)       38 2023-05-26 13:50:49.435454 pqv-0.5.0/setup.cfg
+-rw-r--r--   0 pieter     (501) staff       (20)      529 2023-05-26 13:48:47.000000 pqv-0.5.0/setup.py
```

### Comparing `pqv-0.4.0/LICENSE` & `pqv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqv-0.4.0/pqv/__main__.py` & `pqv-0.5.0/pqv/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 import os
 from pyarrow.parquet import ParquetFile
 from rich.syntax import Syntax
 from textual.app import App, ComposeResult
 from textual.widgets import Static, Footer
 from textual import events
 import pyperclip
+import json
+from datetime import datetime
+
+
+class CustomEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, datetime):
+            return str(obj)
+        if isinstance(obj, bytes):
+            return obj.hex()
+        return super(CustomEncoder, self).default(obj)
 
 
 class ParquetApp(App[str]):
 
     CSS_PATH = "style.css"
     BINDINGS = [
         ("q", "quit", "Quit"),
@@ -21,20 +32,21 @@
 
     def compose(self) -> ComposeResult:
         yield Static(id="info")
         yield Static(id="json")
         yield Footer()
 
     def update_group(self):
-        self.group = self.parquet_file.read_row_group(self.group_index, columns=None).to_pandas()
+        self.group = self.parquet_file.read_row_group(self.group_index, columns=None)
 
     def read_line(self):
         if self.row_index - self.group_offset < len(self.group):
-            row = self.group.iloc[self.row_index - self.group_offset, ]
-            return row.to_json(indent=2)
+            row_dict = dict([(k, v[0]) for k, v in self.group.slice(self.row_index - self.group_offset, 1).to_pydict().items()])
+            json_str = json.dumps(row_dict, indent=2, cls=CustomEncoder)
+            return json_str
         else:
             return None
 
     def show_row(self):
         info_view = self.query_one("#info", Static)
         info = f"{self.file_path} - group {self.group_index + 1}/{self.parquet_file.num_row_groups} - row {self.row_index + 1}/{self.parquet_file.metadata.num_rows}"
         info_view.update(info)
```

### Comparing `pqv-0.4.0/setup.py` & `pqv-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="pqv",
-    version="0.4.0",
+    version="0.5.0",
     author="Pieter Provoost",
     author_email="pieterprovoost@gmail.com",
     description="Simple parquet viewer",
     url="https://github.com/pieterprovoost/pqv",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
```


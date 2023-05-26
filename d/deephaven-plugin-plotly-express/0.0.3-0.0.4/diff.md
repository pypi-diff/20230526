# Comparing `tmp/deephaven-plugin-plotly-express-0.0.3.tar.gz` & `tmp/deephaven-plugin-plotly-express-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-express-0.0.3.tar", last modified: Fri May  5 20:51:50 2023, max compression
+gzip compressed data, was "deephaven-plugin-plotly-express-0.0.4.tar", last modified: Fri May 26 17:07:41 2023, max compression
```

## Comparing `deephaven-plugin-plotly-express-0.0.3.tar` & `deephaven-plugin-plotly-express-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/DataMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/json_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/custom_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/_private_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/financial.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/hierarchial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/subplots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-26 17:07:41.060548 deephaven-plugin-plotly-express-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/DataMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/json_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/custom_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37445 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/_private_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25225 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/financial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/hierarchial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/LICENSE` & `deephaven-plugin-plotly-express-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.3/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.3
+Version: 0.0.4
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/README.md` & `deephaven-plugin-plotly-express-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.3/setup.cfg` & `deephaven-plugin-plotly-express-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/DataMapping.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/DataMapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,60 +5,63 @@
 from deephaven.table import Table
 from deephaven.plugin.object import Exporter
 
 from .json_conversion import json_link_mapping
 
 
 class DataMapping:
-    """
-    A DataMapping that maps plotly variables to table columns
+    """A DataMapping that maps plotly variables to table columns
+
+    Args:
+      table: Table: The table to use for this data mapping
+      data_mapping: list[dict[str, str]]: The variable to column
+        dictionaries used in this mapping. They should map plotly variables
+        to table columns. One of these maps to one data trace.
+      start_index: int: The index (which is an index in the plotly data)
+        that this DataMapping starts at
     """
     def __init__(
             self: DataMapping,
             table: Table,
             data_mapping: list[dict[str, str]],
             start_index: int
     ):
-        """
-        Create a DataMapping
-
-        :param table: The table to use for this data mapping
-        :param data_mapping: The variable to column dictionaries used in this
-        mapping. They should map plotly variables to table columns. One of
-        these maps to one data trace.
-        :param start_index: The index (which is an index in the plotly data)
-        that this DataMapping starts at
-        """
         self._table = table
         self._data_mapping = data_mapping
         self._start_index = start_index
 
     def get_links(
             self: DataMapping,
             exporter: Exporter
     ) -> list[dict[any]]:
-        """
-        Get the json links for this data mapping
+        """Get the json links for this data mapping
+
+        Args:
+          exporter: Exporter: The exporter, used to get the index of the table
+
+        Returns:
+          list[dict[any]]: The column to json link mapping for this DataMapping
 
-        :param exporter: The exporter, used to get the index of the table
-        :return: The column to json link mapping for this DataMapping
         """
         return json_link_mapping(
             self._data_mapping,
             exporter.reference(self._table)._index,
             self._start_index)
 
     def copy(
             self: DataMapping,
             offset: int
     ) -> DataMapping:
-        """
-        Copy this DataMapping, adding a specific offset to the start_index
+        """Copy this DataMapping, adding a specific offset to the start_index
+
+        Args:
+          offset: int: The offset to offset the copy by
+
+        Returns:
+          DataMapping: The new DataMapping
 
-        :param offset: The offset to offset the copy by
-        :return: The new DataMapping
         """
         # only need a shallow copy as the underlying data mappings are
         # never modified, only the start_index is
         new_copy = copy(self)
         new_copy._start_index += offset
         return new_copy
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/json_conversion.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/json_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,60 +3,68 @@
 from collections.abc import Generator, Iterable
 
 
 def json_links(
         i: int,
         _vars: Iterable[str]
 ) -> Generator[str]:
-    """
-    Create json links to a plotly data object at a specific index and with a
+    """Create json links to a plotly data object at a specific index and with a
     list of variables to link at that index
 
-    :param i: index to link to
-    :param _vars: variables to link to
-    :return: a generator that returns the links
+    Args:
+      i: int: index to link to
+      _vars: Iterable[str]: variables to link to
+
+    Yields:
+      str: the links
+
     """
     for var in _vars:
         yield f'/plotly/data/{i}/{var}'
 
 
 def convert_to_json_links(
         var_col_dicts: list[dict[str, str]],
         start_index: int
 ) -> Generator[dict[str, str]]:
-    """
-    Convert the provided dictionaries to json links
+    """Convert the provided dictionaries to json links
 
-    Example input:
-    [
-        {
-            "x": "Col1",
-            "y": "Col2"
-        },
-        {
-            "x": "Col1",
-            "y": "Col3"
-        }
-    ]
+    Args:
+      var_col_dicts: list[dict[str, str]]: A list of dictionaries to convert
+        to json links
+      start_index: int: What index this data mapping starts at
+
+    Yields:
+      dict[str, str]: The generated dictionaries with json links
+
+    Examples:
+        Example input:
+        [
+            {
+                "x": "Col1",
+                "y": "Col2"
+            },
+            {
+                "x": "Col1",
+                "y": "Col3"
+            }
+        ]
+
+        Example output:
+        [
+            {
+                "Col1": "/plotly/data/0/x",
+                "Col2": "/plotly/data/0/y",
+            },
+            {
+                "Col1": "/plotly/data/1/x",
+                "Col3": "/plotly/data/1/y",
+            }
+        ]
 
-    Example output:
-    [
-        {
-            "Col1": "/plotly/data/0/x",
-            "Col2": "/plotly/data/0/y",
-        },
-        {
-            "Col1": "/plotly/data/1/x",
-            "Col3": "/plotly/data/1/y",
-        }
-    ]
-
-    :param var_col_dicts: A list of dictionaries to convert to json links
-    :param start_index: What index this data mapping starts at
-    :return: The generated dictionaries with json links
     """
 
     for i, var_col_dict in zip(count(start_index), var_col_dicts):
         merged = defaultdict(list)
         for k, v in zip(
                 var_col_dict.values(),
                 json_links(i, var_col_dict.keys())):
@@ -66,41 +74,61 @@
 
 
 def json_link_mapping(
         var_col_dicts: list[dict[str, str]],
         table_index: int,
         start_index: int,
 ) -> list[dict[any]]:
-    """
-    Create a data mapping of table and cols to json link
-
+    """Create a data mapping of table and cols to json link
+    
     Example input:
     var_col_dicts = [
         {
             "x: "Col1",
             "y": "Col2
         }
     ]
-
+    
     Example output:
     [{
         table: 0,
         data_columns: {
             "Col1": "/plotly/data/0/x",
             "Col2": "/plotly/data/0/y"
         },
     }]
 
+    Args:
+      var_col_dicts: list[dict[str, str]]: A dictionary containing a mapping of
+        strings to strings and lists of strings used to compute a cartesian
+        product of all possible value groups
+      table_index: int: The index of the table that this mapping is part of
+      start_index: int:  What index this data mapping starts at
+
+    Returns:
+      list[dict[any]]: A list containing dicts that have a table to ref mapping
+        as well as a mapping from originating column to plotly data location
+
+    Examples:
+        Example input:
+        var_col_dicts = [
+            {
+                "x: "Col1",
+                "y": "Col2
+            }
+        ]
+
+        Example output:
+        [{
+            table: 0,
+            data_columns: {
+                "Col1": "/plotly/data/0/x",
+                "Col2": "/plotly/data/0/y"
+            },
+        }]
 
-    :param var_col_dicts: A dictionary containing a mapping of strings to strings
-    and lists of strings used to compute a cartesian product of all possible
-    value groups
-    :param start_index: What index this data mapping starts at
-    :param table_index: The index of the table that this mapping is part of
-    :return: A list containing dicts that have a table to ref mapping as well
-    as a mapping from originating column to plotly data location
     """
     return [
         {"table": table_index, "data_columns": json_link_dict}
         for json_link_dict in
         convert_to_json_links(var_col_dicts, start_index)
     ]
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,94 +10,102 @@
 from ..data_mapping import DataMapping
 
 
 def export_figure(
         exporter: Exporter,
         figure: DeephavenFigure
 ) -> bytes:
-    """
-    Helper to export a DeephavenFigure as json
+    """Helper to export a DeephavenFigure as json
+
+    Args:
+      exporter: Exporter: The exporter to use
+      figure: DeephavenFigure: The figure to export
+
+    Returns:
+      bytes: The figure as bytes
 
-    :param exporter: The exporter to use
-    :param figure: The figure to export
-    :return: The figure as bytes
     """
     return figure.to_json(exporter).encode()
 
 
 def has_color_args(
         call_args: dict[str, any]
 ) -> bool:
-    """
-    Check if any of the color args are in call_args
+    """Check if any of the color args are in call_args
+
+    Args:
+      call_args: dict[str, any]: A dictionary of args
+
+    Returns:
+      bool: True if color args are in, false otherwise
 
-    :param call_args: A dictionary of args
-    :return: True if color args are in, false otherwise
     """
     for arg in ["color_discrete_sequence_line",
                 "color_discrete_sequence_marker"]:
         # convert to bool to ensure empty lists don't prevent removal of
         # colors on traces
         if arg in call_args and bool(call_args[arg]):
             return True
     return False
 
 
 def has_arg(
         call_args: dict[str, any],
         check: str | Callable
 ) -> bool:
-    """
-    Given either a string to check for in call_args or function to check,
+    """Given either a string to check for in call_args or function to check,
     return True if the arg is in the call_args
 
-    :param call_args: A dictionary of args
-    :param check: Either a string or a function that takes call_args
-    :return:
+    Args:
+      call_args: dict[str, any]: A dictionary of args
+      check: str | Callable: Either a string or a function that takes call_args
+
+    Returns:
+        bool: True if the call_args passes the check, False otherwise
     """
     if call_args:
         if isinstance(check, str) and check in call_args:
             return bool(call_args[check])
         elif isinstance(check, Callable):
             return check(call_args)
     return False
     # check is either a function or string
 
 
 class DeephavenFigure:
-    """
-    A DeephavenFigure that contains a plotly figure and mapping from Deephaven
+    """A DeephavenFigure that contains a plotly figure and mapping from Deephaven
     data tables to the plotly figure
+
+    Args:
+        fig: Figure: (Default value = None) The underlying plotly fig
+        call: Callable: (Default value = None) The (usually) px drawing
+          function
+        call_args: dict[any]: (Default value = None) The arguments that were
+          used to call px
+        data_mappings: list[DataMapping]: (Default value = None) A list of data
+          mappings from table column to corresponding plotly variable
+        has_template: bool: (Default value = False) If a template is used
+        has_color: bool: (Default value = False) True if color was manually
+          applied via discrete_color_sequence
+        trace_generator: Generator[dict[str, any]]: (Default value = None)
+          A generator for modifications to traces
+        has_subplots: bool: (Default value = False) True if has subplots
     """
 
     def __init__(
             self: DeephavenFigure,
             fig: Figure = None,
             call: Callable = None,
             call_args: dict[any] = None,
             data_mappings: list[DataMapping] = None,
-            has_template: str = None,
+            has_template: bool = False,
             has_color: bool = False,
             trace_generator: Generator[dict[str, any]] = None,
             has_subplots: bool = False,
-            subplot_specs: list[dict] = None
     ):
-        """
-        Initialize a DeephavenFigure
-
-        :param fig: The underlying plotly fig
-        :param call_args: The arguments that were used to call px
-        :param call: The (usually) px drawing function
-        :param data_mappings:A list of data mappings from table column to
-        corresponding plotly variable
-        :param has_template: If a template is used
-        :param has_color: True if color was manually applied via
-        discrete_color_sequence
-        :param trace_generator: A generator for modifications to traces
-        """
         # keep track of function that called this and it's args
         self.fig = fig
         self.call = call
         self.call_args = call_args
         self.trace_generator = trace_generator
 
         self.has_template = has_template if has_template else \
@@ -110,45 +118,55 @@
 
         self.has_subplots = has_subplots
 
     def copy_mappings(
             self: DeephavenFigure,
             offset: int = 0
     ) -> list[DataMapping]:
-        """
-        Copy all DataMappings within this figure, adding a specific offset
+        """Copy all DataMappings within this figure, adding a specific offset
+
+        Args:
+          offset: int:  (Default value = 0) The offset to offset the copy by
+
+        Returns:
+          list[DataMapping]: The new DataMappings
 
-        :param offset: The offset to offset the copy by
-        :return: The new DataMappings
         """
         return [mapping.copy(offset) for mapping in self._data_mappings]
 
     def get_json_links(
             self: DeephavenFigure,
             exporter: Exporter
     ) -> list[dict[str, str]]:
-        """
-        Convert the internal data mapping to the JSON data mapping with tables
-        and proper plotly indices attached
+        """Convert the internal data mapping to the JSON data mapping with
+        tables and proper plotly indices attached
+
+        Args:
+          exporter: Exporter: The exporter to use to send tables
+
+        Returns:
+          list[dict[str, str]]: The list of json links that map table columns
+            to the plotly figure
 
-        :param exporter: The exporter to use to send tables
-        :return: The list of json links that map table columns to the plotly figure
         """
         return [links for mapping in self._data_mappings
                 for links in mapping.get_links(exporter)]
 
     def to_json(
             self: DeephavenFigure,
             exporter: Exporter
     ) -> str:
-        """
-        Convert the DeephavenFigure to JSON
+        """Convert the DeephavenFigure to JSON
+
+        Args:
+          exporter: Exporter: The exporter to use to send tables
+
+        Returns:
+          str: The DeephavenFigure as a JSON string
 
-        :param exporter: The exporter to use to send tables
-        :return: The DeephavenFigure as a JSON string
         """
         plotly = json.loads(self.fig.to_json())
         mappings = self.get_json_links(exporter)
         deephaven = {
             "mappings": mappings,
             "is_user_set_template": self.has_template,
             "is_user_set_color": self.has_color
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/_private_utils.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/_private_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,92 @@
 from functools import partial
-from itertools import chain
 from typing import Callable
-from collections.abc import Generator, Iterator
+from collections.abc import Generator
 
-from plotly import subplots
+import plotly.express as px
 from plotly.graph_objects import Figure
 
 from deephaven.table import Table
 
-from ..deephaven_figure import generate_figure, DeephavenFigure, update_traces
+from ..deephaven_figure import generate_figure, DeephavenFigure
+from ..shared import get_unique_names
 
 
 def default_callback(
-        fig
+        fig: Figure
 ) -> Figure:
-    """
-    A default callback that returns the passed fig
+    """A default callback that returns the passed fig
+
+    Args:
+      fig: Figure: The input figure
+
+    Returns:
+      Figure: The same figure
 
-    :param fig:
-    :return: The same fig
     """
     return fig
 
 
 def unsafe_figure_update_wrapper(
         unsafe_figure_update: callable,
         dh_fig: DeephavenFigure
 ) -> DeephavenFigure:
-    """
-    Wrap the callback to be applied last before a figure is returned
+    """Wrap the callback to be applied last before a figure is returned
+
+    Args:
+      unsafe_figure_update: The function to call on the plotly figure
+      dh_fig: DeephavenFigure: The DeephavenFigure to update
+
+    Returns:
+      DeephavenFigure: The resulting DeephavenFigure
 
-    :param unsafe_figure_update: The function to call on the plotly figure
-    :param dh_fig: The DeephavenFigure to update
-    :return: The resulting DeephavenFigure
     """
     # allow either returning a new fig or not from callback
     new_fig = unsafe_figure_update(dh_fig.fig)
     dh_fig.fig = new_fig if new_fig else dh_fig.fig
     return dh_fig
 
 
 def normalize_position(
         position: float,
         chart_start: float,
         chart_range: float
 ) -> float:
-    """
-    Normalize a position so that it falls between 0 and 1 (inclusive)
+    """Normalize a position so that it falls between 0 and 1 (inclusive)
 
-    :param position: The current position
-    :param chart_start: The start of the domain the existing chart has
-    :param chart_range: The range the existing chart has
-    :return:
+    Args:
+      position: float: The current position
+      chart_start: float: The start of the domain the existing chart has
+      chart_range: float: The range the existing chart has
+
+    Returns:
+      float: The normalized position
     """
     return (position - chart_start) / chart_range
 
 
 def get_new_positions(
         new_domain: list[float],
         positions: list[float],
         chart_domain: list[float]
 ) -> list[float]:
-    """
-    Get positions within the new domain of an arbitrary list of positions
+    """Get positions within the new domain of an arbitrary list of positions
     The positions will first be normalized to fall between 0 and 1 inclusive
     using the current chart_domain. Then, the positions are mapped onto
     new_domain.
     For example, if a position is at 0.5, chart_domain is [0, 1] and new_domain
     is [0, 0.6], the new position is 0.3.
 
-    :param new_domain: The new domain to map the points to
-    :param positions: The current positions of the points
-    :param chart_domain: The current domain of the whole chart
-    :return:
+    Args:
+      new_domain: list[float]: The new domain to map the points to
+      positions: list[float]: The current positions of the points
+      chart_domain: list[float]: The current domain of the whole chart
+
+    Returns:
+      list[float]: The new positions
     """
     if not isinstance(positions, list):
         positions = [positions]
     new_positions = []
     new_range = new_domain[1] - new_domain[0]
     for position in positions:
         chart_range = chart_domain[1] - chart_domain[0]
@@ -86,22 +96,22 @@
     return new_positions
 
 
 def resize_domain(
         obj: dict,
         new_domain: dict[str, list[float]]
 ) -> None:
-    """
-    Resize the domain of the given object
+    """Resize the domain of the given object
+
+    Args:
+      obj: dict: The object to resize. It should have a "domain" key that
+        references a dict that has "x" and "y" keys.
+      new_domain: dict[str, list[float]]: The new domain the map the figure to.
+        Contains keys of x and y and values of domains, such as [0,0.5]
 
-    :param obj: The object to resize. It should have a "domain" key that
-    references a dict that has "x" and "y" keys.
-    :param new_domain: The new domain the map the figure to. Contains keys of x
-    and y and values of domains, such as [0,0.5]
-    keys
     """
     new_domain_x = new_domain.get("x", None)
     new_domain_y = new_domain.get("y", None)
     obj_domain_x = obj["domain"]["x"]
     obj_domain_y = obj["domain"]["y"]
     domain_update = {}
     try:
@@ -119,25 +129,27 @@
 
 
 def resize_xy_axis(
         axis: dict,
         new_domain: dict[str, list[float]],
         which: str
 ) -> None:
-    """
-    Resize either an x or y axis.
+    """Resize either an x or y axis.
+
+    Args:
+      axis: dict: The axis object to resize.
+      new_domain: dict[str, list[float]]: The new domain the map the figure to.
+        Contains keys of x and y and values of domains, such as [0,0.5]
+      which: str: Either "x" or "y"
 
-    :param axis: The axis object to resize. It should have a "domain" key.
-    :param new_domain: The new domain the map the figure to. Contains keys of x
-    and y and values of domains, such as [0,0.5]
-    :param which: Either "x" or "y"
     """
     new_domain_x = new_domain.get("x", None)
     new_domain_y = new_domain.get("y", None)
-    axis_domain = axis["domain"]
+    # the existing domain is assumed to be 0, 1 if not set
+    axis_domain = axis.get("domain", [0, 1])
     axis_position = axis.get("position", None)
     axis_update = {}
     try:
         if which == "x":
             if new_domain_x:
                 axis_update["domain"] = get_new_positions(new_domain_x, axis_domain, [0, 1])
             if new_domain_y and axis_position is not None:
@@ -154,19 +166,20 @@
         pass
 
 
 def reassign_axes(
         trace: dict,
         axes_remapping: dict[str, str]
 ) -> None:
-    """
-    RUpdate the trace with its new axes using with the remapping
+    """Update the trace with its new axes using with the remapping
+
+    Args:
+      trace: dict: The trace to remap axes within
+      axes_remapping: dict[str, str]: The mapping of old to new axes
 
-    :param trace: The trace to remap axes within
-    :param axes_remapping: The mapping of old to new axes
     """
     if 'xaxis' in trace:
         trace.update(xaxis=axes_remapping[trace['xaxis']])
 
     if 'yaxis' in trace:
         trace.update(yaxis=axes_remapping[trace['yaxis']])
 
@@ -180,19 +193,20 @@
         trace.update(ternary=axes_remapping[trace['ternary']])
 
 
 def reassign_attributes(
         axis: dict,
         axes_remapping: dict[str, str]
 ) -> None:
-    """
-    Reassign attributes of a layout object using with the remapping
+    """Reassign attributes of a layout object using with the remapping
+
+    Args:
+      axis: dict: The axis object to remap attributes from
+      axes_remapping: dict[str, str]: The mapping of old to new axes
 
-    :param axis: The axis object to remap attributes from
-    :param axes_remapping: The mapping of old to new axes
     """
     # anchor can also be free, which does not need to be modified
     if 'anchor' in axis and axis['anchor'] in axes_remapping:
         axis.update(anchor=axes_remapping[axis['anchor']])
 
     if 'overlaying' in axis and axis['overlaying'] in axes_remapping:
         axis.update(overlaying=axes_remapping[axis['overlaying']])
@@ -201,27 +215,30 @@
 def resize_axis(
         type_: str,
         old_axis: str,
         axis: dict,
         num: str,
         new_domain: dict[str, list[float]]
 ) -> tuple[str, str, str]:
-    """
-    Maps the specified axis to new_domain and returns info to help remap axes
+    """Maps the specified axis to new_domain and returns info to help remap axes
+
+    Args:
+      type_: str: The type of axis to resize
+      old_axis: str: The old axis name
+      axis: dict: The axis object to resize
+      num: str: The number (possibly empty) of this axis within the new chart
+      new_domain: dict[str, list[float]]: The new domain the map the figure to.
+        Contains keys of x and y and values of domains, such as [0,0.5]
+
+    Returns:
+      tuple[str, str, str]: A tuple of new axis name, old axis name (for trace
+        remapping), new axis name (for trace remapping). The new axis name
+        isn't always the same within the trace as it is in the layout (such as
+        in the case of xaxis or yaxis), hence the need for both of the names.
 
-    :param type_: The type of axis to resize
-    :param old_axis: The old axis name
-    :param axis: The axis object to resize
-    :param num: The number (possibly empty) of this axis within the new chart
-    :param new_domain: The new domain the map the figure to. Contains keys of x
-    and y and values of domains, such as [0,0.5]
-    :return: A tuple of new axis name, old axis name (for trace remapping),
-    new axis name (for trace remapping). The new axis name isn't always the
-    same within the trace as it is in the layout (such as in the case of xaxis
-    or yaxis), hence the need for both of the names.
     """
     new_axis = f"{type_}{num}"
     if type_ == 'xaxis' or type_ == 'yaxis':
         which = type_[0]
         resize_xy_axis(axis, new_domain, which)
         old_trace_axis = old_axis.replace(type_, which)
         return new_axis, old_trace_axis, f"{which}{num}"
@@ -230,48 +247,56 @@
         return new_axis, old_axis, new_axis
 
 
 def get_axis_update(
         spec: dict[str, any],
         type_: str
 ) -> dict[str, any] | None:
-    """
-    Retrieve an axis update from the spec
+    """Retrieve an axis update from the spec
+
+    Args:
+      spec: dict[str, any]: The full spec object
+      type_: str: The type of axis to retrieve the update of
+
+    Returns:
+      dict[str, any] | None: A dictionary of updates to make to the x or y-axis
 
-    :param spec: The full spec object
-    :param type_: The type of axis to retrieve the update of
-    :return: A dictionary of updates to make to the x or y-axis
     """
     if 'xaxis_update' in spec and type_ == "xaxis":
         return spec["xaxis_update"]
     if 'yaxis_update' in spec and type_ == "yaxis":
         return spec["yaxis_update"]
     return None
 
 
 def resize_fig(
         fig_data: dict,
         fig_layout: dict,
         spec: dict[str, str | bool | list[float]],
         new_axes_start: dict[str, int],
 ) -> tuple[dict, dict]:
-    """
-    Resize a figure into new_domain, reindexing with the indices specified in
+    """Resize a figure into new_domain, reindexing with the indices specified in
     new_axes_start
 
-    :param fig_data: The current figure data
-    :param fig_layout: The current figure layout
-    :param spec: A dictionary that contains keys of "x" and "y"
-    that have values that are lists of two floats from 0 to 1. The chart that
-    corresponds with a domain will be resized to that domain. Either x or y can
-    be excluded if only resizing on one axis. Can also specify xaxis_update or
-    yaxis_update with a dictionary value to update all axes with that dict.
-    :param new_axes_start: A dictionary containing the start of new indices to
-    ensure there is no reindexing collisions
-    :return: A tuple of the new figure data, the new figure layout
+    Args:
+      fig_data: dict: The current figure data
+      fig_layout: dict: The current figure layout
+      spec: dict[str, str | bool | list[float]]:
+        A dictionary that contains keys of "x" and "y"
+        that have values that are lists of two floats from 0 to 1. The chart
+        that corresponds with a domain will be resized to that domain. Either
+        x or y can be excluded if only resizing on one axis. Can also specify
+        xaxis_update or yaxis_update with a dictionary value to update all axes
+        with that dict.
+      new_axes_start: dict[str, int]: A dictionary containing the start of
+        new indices to ensure there is no reindexing collisions
+
+    Returns:
+      tuple[dict, dict]: A tuple of the new figure data, the new figure layout
+
     """
     if not spec:
         # if there is no spec, nothing needs to be done
         return fig_data, fig_layout
 
     axes_remapping = {}
     new_axes = {}
@@ -343,67 +368,78 @@
 def fig_data_and_layout(
         fig: Figure,
         i: int,
         specs: list[dict[str, str | bool | list[float]]],
         which_layout: int,
         new_axes_start: dict[str, int],
 ) -> tuple[tuple | dict, dict]:
-    """
-    Get new data and layout for the specified figure
+    """Get new data and layout for the specified figure
+
+    Args:
+      fig: Figure: The current figure
+      i: int: The index of the figure, used for which_layout
+      specs: list[dict[str, str | bool | list[float]]]:
+        A list of dictionaries that contains keys of "x" and "y"
+        that have values that are lists of two floats from 0 to 1. The chart
+        that corresponds with a domain will be resized to that domain. Either
+        x or y can be excluded if only resizing on one axis. Can also specify
+        xaxis_update or yaxis_update with a dictionary value to update all axes
+        with that dict.
+      which_layout: int: None to layer layouts, or an index of which arg to
+        take the layout from
+      new_axes_start: dict[str, int]: A dict that keeps track of starting
+       points when recreating axes
+
+    Returns:
+      tuple[tuple | dict, dict]: A tuple of figure data, figure layout
 
-    :param fig: The current figure
-    :param i: The index of the figure, used for which_layout
-    :param which_layout: None to layer layouts, or an index of which arg to
-    take the layout from
-    :param specs: A list of dictionaries that contain keys of "x" and "y"
-    that have values that are lists of two floats from 0 to 1. The chart that
-    corresponds with a domain will be resized to that domain. Either x or y can
-    be excluded if only resizing on one axis. Can also specify xaxis_update or
-    yaxis_update with a dictionary value to update all axes with that dict.
-    :param new_axes_start: A dict that keeps track of starting points when
-    recreating axes
-    :return: A tuple of figure data, figure layout
     """
     if specs:
         return resize_fig(fig.to_dict()['data'], fig.to_dict()['layout'],
                           specs[i], new_axes_start)
 
     fig_layout = {}
-    if not which_layout or which_layout == i:
+    if which_layout is None or which_layout == i:
         fig_layout.update(fig.to_dict()['layout'])
 
     return fig.data, fig_layout
 
 
 def layer(
         *figs: DeephavenFigure | Figure,
         which_layout: int = None,
         specs: list[dict[str, any]] = None,
         unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Layers the provided figures. Be default, the layouts are sequentially
+    """Layers the provided figures. Be default, the layouts are sequentially
     applied, so the layouts of later figures will override the layouts of early
     figures.
 
-    :param figs: The charts to layer
-    :param which_layout: None to layer layouts, or an index of which arg to
-    take the layout from. Currently only valid if domains are not specified.
-    :param specs: A list of dictionaries that contain keys of "x" and "y"
-    that have values that are lists of two floats from 0 to 1. The chart that
-    corresponds with a domain will be resized to that domain. Either x or y can
-    be excluded if only resizing on one axis. Can also specify xaxis_update or
-    yaxis_update with a dictionary value to update all axes with that dict.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: The layered chart
+    Args:
+      *figs: DeephavenFigure | Figure: The charts to layer
+      which_layout: int:  (Default value = None) None to layer layouts, or an
+        index of which arg to take the layout from. Currently only valid if
+        domains are not specified.
+      specs: list[dict[str, str | bool | list[float]]]:
+        A list of dictionaries that contains keys of "x" and "y"
+        that have values that are lists of two floats from 0 to 1. The chart
+        that corresponds with a domain will be resized to that domain. Either
+        x or y can be excluded if only resizing on one axis. Can also specify
+        xaxis_update or yaxis_update with a dictionary value to update all axes
+        with that dict.
+      unsafe_update_figure: An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is not
+        returned, the plotly figure passed will be assumed to be the return value.
+        Used to add any custom changes to the underlying plotly figure. Note that
+        the existing data traces should not be removed. This may lead to unexpected
+        behavior if traces are modified in a way that break data mappings.
+
+    Returns:
+      DeephavenFigure: The layered chart
+
     """
     if len(figs) == 0:
         raise ValueError("No figures provided to compose")
 
     new_data = []
     new_layout = {}
     new_data_mappings = []
@@ -463,234 +499,368 @@
         )
     )
 
 
 def validate_common_args(
         args: dict
 ) -> None:
-    """
-    Validate common args amongst plots
+    """Validate common args amongst plots
+
+    Args:
+      args: dict: The args to validate
 
-    :param args: The args to validate
     """
     if not isinstance(args["table"], Table):
         raise ValueError("Argument table is not of type Table")
 
 
 def remap_scene_args(
         args: dict
 ) -> None:
-    """
-    Remap layout scenes args so that they are not converted to a list
+    """Remap layout scenes args so that they are not converted to a list
+
+    Args:
+      args: dict: The args to remap
 
-    :param args: The args to remap
     """
     for arg in ["range_x", "range_y", "range_z", "log_x", "log_y", "log_z"]:
         args[arg + '_scene'] = args.pop(arg)
 
 
-def trace_legend_generator(
-        cols: list[str]
-) -> Generator[dict]:
-    """
-    Adds the traces to the legend
-
-    :param cols: The cols to label the trace with in the legend
-    :returns: A generator that yields trace updates
-    """
-    for col in cols:
-        yield {
-            "name": col,
-            "showlegend": True
-        }
-
-
 def preprocessed_fig(
-        draw: Callable,
+        draw: callable,
         keys: list[str],
         args: dict[str, any],
+        is_list: bool,
         trace_generator: Generator[dict[str, any]],
         col: str | list[str],
-        preprocesser: Callable = None,
+        preprocesser: callable = None,
         table: Table = None,
         preprocessed_args: tuple[Table, str, list[str]] = None
 ) -> DeephavenFigure:
-    """
-    Preprocess and return a figure
+    """Preprocess and return a figure
     Either both preprocesser and table or just preprocessed_table should be
     specified
 
-    :param preprocesser: A function that returns a tuple that contains
-    (new table, first data columnn, second data column)
-    :param draw: A draw function, generally from plotly express
-    :param args: The args to pass to figure creation
-    :param keys: A list of the variables to assign the preprocessed results to
-    :param table: The table to use
-    :param args: The args to passed to generate_figure
-    :param trace_generator: The trace generator to use to pass to
-    generate_figure
-    :param col: The columns that are being plotted
-    :param preprocessed_args: If the data was already preprocessed, use that
-    tuple of data instead
-    :return: The resulting DeephavenFigure
+    Args:
+      draw: callable: A draw function, generally from plotly express
+      keys: list[str]: A list of the variables to assign the preprocessed
+        results to
+      args: The args to pass to figure creation
+      is_list: bool: True if the current column is one of a list
+      trace_generator: Generator[dict[str, any]]: The trace generator to use
+        to pass to generate_figure
+      col: str | list[str]: The columns that are being plotted
+      preprocesser: callable: (Default value = None)
+        A function that returns a tuple that contains
+        (new table, first data columnn, second data column)
+      table: Table: The table to use
+      preprocessed_args: tuple[Table, str, list[str]]:  (Default value = None)
+        If the data was already preprocessed, use that tuple of data instead
+
+    Returns:
+      DeephavenFigure: The resulting DeephavenFigure
+
     """
     # if preprocessed args are specified, the table is created,
     # but the list of columns (the last of the preprocessed args)
     # needs to be overriden with the current column
     if preprocessed_args:
         output = preprocessed_args
         output = [output[0], output[1], col]
     else:
         output = preprocesser(table, col)
 
     for k, v in zip(keys, output):
         args[k] = v
 
+    if is_list:
+        # the col is needed for proper hover text, but only if
+        # there's a list
+        args["current_col"] = col
+
     return generate_figure(
         draw=draw,
         call_args=args,
         trace_generator=trace_generator,
     )
 
 
-def update_legend_and_titles(
-        fig: DeephavenFigure,
-        var: str,
-        cols: list[str],
-        is_list: bool,
-        list_var_axis_name: str,
-        list_val_axis_name: str,
-        str_var_axis_name: str,
-        str_val_axis_name: str
-) -> None:
-    """
-    Update the legend and titles so they match plotly express (more or less)
-
-    :param fig: The figure to update
-    :param var: Which var to map to the first column. If "x", then the
-    preprocessor output is mapped to table, x, y. If "y" then preprocessor
-    output is mapped to table, y, x.
-    :param cols: The columns that are used for the sake of updating the
-    legend
-    :param is_list: True if the cols were originally passed as a list
-    :param str_var_axis_name: Name on the var axis if cols is a str
-    :param str_val_axis_name: Name on the non-var axis if cols is a str
-    :param list_var_axis_name: Name on the var axis if cols is a list
-    :param list_val_axis_name: Name on the non-var axis if cols is a list
-    """
-    layout_update = {}
-    other_var = "y" if var == "x" else "x"
-
-    if is_list:
-        update_traces(fig.fig, trace_legend_generator(cols))
-        layout_update.update(
-            legend_title_text="variable",
-            legend_tracegroupgap=0
-        )
-
-        if list_var_axis_name:
-            layout_update[f"{var}axis_title_text"] = list_var_axis_name
-
-        if list_val_axis_name:
-            layout_update[f"{other_var}axis_title_text"] = list_val_axis_name
-
-    else:
-        # ensure the legend is hidden (especially for hist)
-        layout_update["showlegend"] = False
-
-        if str_var_axis_name:
-            layout_update[f"{var}axis_title_text"] = str_var_axis_name
-
-        if str_val_axis_name:
-            layout_update[f"{other_var}axis_title_text"] = str_val_axis_name
-
-    fig.fig.update_layout(layout_update)
-
-
 def preprocess_and_layer(
-        preprocesser: Callable,
-        draw: Callable,
+        preprocesser: callable,
+        draw: callable,
         args: dict[str, any],
         var: str,
         orientation: str = None,
-        str_var_axis_name: str = None,
-        str_val_axis_name: str = None,
-        list_var_axis_name: str = None,
-        list_val_axis_name: str = None,
         is_hist: bool = False,
 ) -> DeephavenFigure:
-    """
-    Given a preprocessing function, a draw function, and several
+    """Given a preprocessing function, a draw function, and several
     columns, layer up the resulting figures
 
-    :param preprocesser: A function that takes a table, list of cols
-    and returns a tuple that contains
-    (new table, first data columnn, second data column)
-    :param draw: A draw function, generally from plotly express
-    :param args: The args to pass to figure creation
-    :param var: Which var to map to the first column. If "x", then the
-    preprocessor output is mapped to table, x, y. If "y" then preprocessor
-    output is mapped to table, y, x.
-    :param orientation: optional orientation if it is needed
-    :param str_var_axis_name: Name on the var axis if cols is a str
-    :param str_val_axis_name: Name on the non-var axis if cols is a str
-    :param list_var_axis_name: Name on the var axis if cols is a list
-    :param list_val_axis_name: Name on the non-var axis if cols is a list
-    :param is_hist: If true, the figure is a histogram and requires custom
-    processing, specifically because the preprocessing returns a single table
-    for all columns.
-    :return: The resulting DeephavenFigure
+    Args:
+      preprocesser: callable: A function that takes a table, list of cols
+        and returns a tuple that contains
+        (new table, first data columnn, second data column)
+      draw: callable: A draw function, generally from plotly express
+      args: dict[str, any]: The args to pass to figure creation
+      var: str: Which var to map to the first column. If "x", then the
+        preprocessor output is mapped to table, x, y. If "y" then preprocessor
+        output is mapped to table, y, x.
+      orientation: str:  (Default value = None)
+        optional orientation if it is needed
+      is_hist: bool:  (Default value = False)
+        If true, the figure is a histogram and requires custom
+
+    Returns:
+      DeephavenFigure: The resulting DeephavenFigure
+
     """
 
     cols = args[var]
     # to mirror px, list_var_axis_name and legend should only be used when cols
     # are a list (regardless of length)
     is_list = isinstance(cols, list)
     cols = cols if is_list else [cols]
     keys = ["table", "x", "y"] if var == "x" else ["table", "y", "x"]
     table = args["table"]
     figs = []
     trace_generator = None
+    has_color = None
+
+    # the var is needed for proper hover text
+    args["current_var"] = var
+
+    if not args.get("color_discrete_sequence_marker"):
+        # the colors need to match the plotly qualitative colors so they can be
+        # overriden, but has_color should be false as the color was not
+        # specified by the user
+        has_color = False
+        args["color_discrete_sequence_marker"] = px.colors.qualitative.Plotly
 
     if orientation:
         args["orientation"] = orientation
 
     if is_hist:
         # histograms generate one table with all info
-        str_var_axis_name = str_var_axis_name if is_list else cols[0]
         create_fig = partial(
             preprocessed_fig,
-            draw, keys, args,
             preprocessed_args=preprocesser(table, cols)
         )
     else:
+        # pivot vars need to be calculated here to be shared between layers
+        args["pivot_vars"] = get_unique_names(table, ["variable", "value"])
+
         create_fig = partial(
             preprocessed_fig,
-            draw, keys, args,
             preprocesser=preprocesser,
             table=table
         )
 
     for i, col in enumerate(cols):
 
-        new_fig = create_fig(trace_generator, col)
+        new_fig = create_fig(draw, keys, args, is_list, trace_generator, col)
         # offsetgroup is needed mostly to prevent spacing issues in
         # marginals
         # not setting the offsetgroup and having both marginals set to box,
         # violin, etc. leads to extra spacing in each marginal
         # offsetgroup needs to be unique within the subchart as columns
         # could have the same name
         new_fig.fig.update_traces(offsetgroup=f"{col}{i}")
         figs.append(new_fig)
 
         if not trace_generator:
             trace_generator = figs[0].trace_generator
 
     layered = layer(*figs, which_layout=0)
 
-    update_legend_and_titles(
-        layered, var, cols, is_list,
-        list_var_axis_name, list_val_axis_name,
-        str_var_axis_name, str_val_axis_name
+    if has_color is False:
+        layered.has_color = False
+
+    if is_list:
+        layered.fig.update_layout(legend_tracegroupgap=0)
+    else:
+        layered.fig.update_layout(showlegend=False)
+
+    return layered
+
+
+def calculate_mode(
+        base_mode: str,
+        args: dict[str, any]
+) -> str:
+    """Calculate the mode of the traces based on the arguments
+
+    Args:
+      base_mode: The mode that this trace definitely has, either lines or markers
+      args: The args to use to figure out the mode
+      base_mode: str: 
+      args: dict[str: 
+      any]: 
+
+    Returns:
+      The mode. Some combination of markers, lines, text, joined by '+'.
+
+    """
+    modes = [base_mode]
+    if base_mode == "lines" and any([
+        args.get("markers", None),
+        args.get("symbol", None),
+        args.get("symbol_sequence", None),
+        args.get("text", None)]
+    ):
+        modes.append("markers")
+    if args.get("text", None):
+        modes.append("text")
+    return "+".join(modes)
+
+
+def apply_args_groups(
+        args: dict[str, any],
+        groups: set[str]
+) -> None:
+    """Transform args depending on groups
+
+    Args:
+      args: dict[str, any]: A dictionary of args to transform
+      groups: set[str]: A set of groups used to transform the args
+
+    """
+    groups = groups if isinstance(groups, set) else {groups}
+
+    sync_dict = SyncDict(args)
+
+    if "scatter" in groups:
+        args["mode"] = calculate_mode("markers", args)
+        args["color_discrete_sequence_marker"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+
+    if "line" in groups:
+        args["mode"] = calculate_mode("lines", args)
+        args["color_discrete_sequence_marker"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+        args["color_discrete_sequence_line"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+
+    if "ecdf" in groups:
+        # ecdf should be forced to lines even if both "lines" and "markers" are False
+        base_mode = "lines" if args["lines"] or not args["markers"] else "markers"
+        args["mode"] = calculate_mode(base_mode, args)
+        args["color_discrete_sequence_marker"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+        args["color_discrete_sequence_line"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+
+    if 'scene' in groups:
+        for arg in ["range_x", "range_y", "range_z", "log_x", "log_y", "log_z"]:
+            args[arg + '_scene'] = args.pop(arg)
+
+    if 'bar' in groups:
+        args["color_discrete_sequence_marker"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+        args["pattern_shape_sequence_bar"] = sync_dict.will_pop(
+            "pattern_shape_sequence")
+
+    if 'marker' in groups:
+        args["color_discrete_sequence_marker"] = sync_dict.will_pop(
+            "color_discrete_sequence")
+
+    if 'area' in groups:
+        args["pattern_shape_sequence_area"] = sync_dict.will_pop(
+            "pattern_shape_sequence")
+
+    if "webgl" in groups:
+        args["render_mode"] = "webgl"
+
+    sync_dict.sync_pop()
+
+
+def process_args(
+        args: dict[str, any],
+        groups: set[str] = None,
+        add: dict[str, any] = None,
+        pop: list[str] = None,
+        remap: dict[str, str] = None
+) -> partial:
+    """Process the provided args
+
+    Args:
+      args: dict[str, any]: A dictionary of args to process
+      groups: set[str]:  (Default value = None)
+        A set of groups that apply transformations to the args
+      add: dict[str, any] (Default value = None)
+        A dictionary to add to the args
+      pop: list[str]:  (Default value = None)
+        A list of keys to remove from the args
+      remap: dict[str, str]:  (Default value = None)
+        A dictionary mapping of keys to keys
+
+    Returns:
+      partial: The update wrapper, based on the update function in the args
+
+    """
+    validate_common_args(args)
+
+    apply_args_groups(args, groups)
+
+    if add:
+        args.update(add)
+
+    if pop:
+        for arg in pop:
+            args.pop(arg)
+
+    if remap:
+        for old_arg, new_arg in remap.items():
+            args[new_arg] = args.pop(old_arg)
+
+    update_wrapper = partial(
+        unsafe_figure_update_wrapper,
+        args.pop("unsafe_update_figure")
     )
 
-    return layered
+    return update_wrapper
+
+
+class SyncDict:
+    """A dictionary wrapper that will queue up keys to remove and remove them
+    all at once
+
+
+    Args:
+      d: dict: the dictionary to wrap
+
+
+    """
+    def __init__(
+            self,
+            d: dict
+    ):
+        self.d = d
+        self.pop_set = set()
+
+    def will_pop(
+            self,
+            key: any
+    ) -> any:
+        """Add a key to the set of keys that will eventually be popped
+
+        Args:
+          key: The key to add to the set
+
+        Returns:
+          The value associated with the key that will be popped
+
+        """
+        self.pop_set.add(key)
+        return self.d[key]
+
+    def sync_pop(
+            self
+    ):
+        """Pop all elements from the dictionary that have been added to the pop
+        set
+
+        """
+        for k in self.pop_set:
+            self.d.pop(k)
+
+
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/area.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/area.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from functools import partial
-from typing import Callable
-
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, unsafe_figure_update_wrapper
+from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
 
 
 def area(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         size: str | list[str] = None,
+        text: str | list[str] = None,
+        hover_name: str | list[str] = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
         size_sequence: list[int] = None,
         xaxis_sequence: list[str] = None,
         yaxis_sequence: list[str] = None,
         markers: bool = False,
@@ -28,90 +28,113 @@
         range_x: list[int] | list[list[int]] = None,
         range_y: list[int] | list[list[int]] = None,
         yaxis_titles: list[str] = None,
         xaxis_titles: list[str] = None,
         line_shape: str = 'linear',
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns an area chart
+    """Returns an area chart
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x: str | list[str]:  (Default value = None)
+        A column or list of columns that contain x-axis values.
+      y: str | list[str]:  (Default value = None)
+        A column or list of columns that contain y-axis values.
+      size: str | list[str]:  (Default value = None)
+        A column or list of columns that contain size values.
+      text: str | list[str]:  (Default value = None)
+        A column or list of columns that contain text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column or list of columns that contain names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      pattern_shape_sequence: list[str]:  (Default value = None)
+        A list of patterns to sequentially apply
+        to the series. The patterns loop, so if there are more series than
+        patterns, patterns will be reused.
+      symbol_sequence: list[str]:  (Default value = None)
+        A list of symbols to sequentially apply to the
+        markers in the series. The symbols loop, so if there are more series
+        than symbols, symbols will be reused.
+      size_sequence: list[str]:  (Default value = None)
+        A list of sizes to sequentially apply to the
+        markers in the series. The sizes loop, so if there are more series than
+        symbols, sizes will be reused. This is overriden is "size" is specified.
+      xaxis_sequence: list[str]:  (Default value = None)
+        A list of x axes to assign series to. Odd numbers
+        starting with 1 are created on the bottom x axis and even numbers starting
+        with 2 are created on the top x axis. Axes are created up
+        to the maximum number specified. The axes loop, so if there are more series
+        than axes, axes will be reused.
+      yaxis_sequence: list[str]:  (Default value = None)
+        A list of y axes to assign series to. Odd numbers
+        starting with 1 are created on the left y axis and even numbers starting
+        with 2 are created on the top y axis. Axes are created up
+        to the maximum number specified. The axes loop, so if there are more series
+        than axes, axes will be reused.
+      markers: bool:  (Default value = False)
+        True to draw markers on the line, False to not. Default False
+      groupnorm: str: (Default value = None)
+        Set to 'fraction' to plot the fraction out of
+        the total value of all points at that x value, 'percent' to take the
+        fraction and multiply by 100. Note that if multiple y axes are
+        specified, the groupnorm is taken per axis.
+      log_x: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      log_y: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      range_x: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the x axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      range_y: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the y axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      yaxis_titles: list[str]:  (Default value = None)
+        A list of titles to sequentially apply to the y axes. The titles do not
+          loop.
+      xaxis_titles: list[str]:  (Default value = None)
+        A list of titles to sequentially apply to the x axes. The titles do not
+          loop.
+      line_shape: str:  (Default value = 'linear')
+        The line shape for all lines created. One of 'linear',
+        'spline', 'vhv', 'hvh', 'vh', 'hv'. Default 'linear'
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure:  Callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      DeephavenFigure: A DeephavenFigure that contains the area chart
 
-    :param table: A table to pull data from.
-    :param x: A column or list of columns that contain x-axis values.
-    :param y: A column or list of columns that contain y-axis values.
-    :param size: A column or list of columns that contain size values.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param pattern_shape_sequence: A list of patterns to sequentially apply
-    to the series. The patterns loop, so if there are more series than
-    patterns, patterns will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    markers in the series. The symbols loop, so if there are more series than
-    symbols, symbols will be reused.
-    :param size_sequence: A list of sizes to sequentially apply to the
-    markers in the series. The sizes loop, so if there are more series than
-    symbols, sizes will be reused. This is overriden is "size" is specified.
-    :param xaxis_sequence: A list of x axes to assign series to. Odd numbers
-    starting with 1 are created on the bottom x axis and even numbers starting
-    with 2 are created on the top x axis. Axes are created up
-    to the maximum number specified. The axes loop, so if there are more series
-    than axes, axes will be reused.
-    :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
-    starting with 1 are created on the left y axis and even numbers starting
-    with 2 are created on the top y axis. Axes are created up
-    to the maximum number specified. The axes loop, so if there are more series
-    than axes, axes will be reused.
-    :param markers: True to draw markers on the line, False to not. Default
-    False
-    :param groupnorm: Default None. 'fraction' to plot the fraction out of
-    the total value of all points at that x value, 'percent' to take the
-    fraction and multiply by 100. Note that if multiple y axes are
-    specified, the groupnorm is taken per axis.
-    :param log_x: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param log_y: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param range_x: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param range_y: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param yaxis_titles: A list of titles to sequentially apply to the
-    y axes. The titles do not loop.
-    :param xaxis_titles: A list of titles to sequentially apply to the
-    x axes. The titles do not loop.
-    :param line_shape: The line shape for all lines created. One of 'linear',
-    'spline', 'vhv', 'hvh', 'vh', 'hv'. Default 'linear'
-    :param title: The title of the chart
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the area chart
     """
     args = locals()
 
-    validate_common_args(args)
-
-    args["pattern_shape_sequence_area"] = args.pop("pattern_shape_sequence")
-    args["color_discrete_sequence_marker"] = args["color_discrete_sequence"]
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"area", "line"})
 
     return update_wrapper(
         generate_figure(draw=px.area, call_args=args)
     )
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/bar.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/bar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,133 @@
 from functools import partial
-from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, preprocess_and_layer, unsafe_figure_update_wrapper
+from ._private_utils import default_callback, validate_common_args, preprocess_and_layer, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_timeline, preprocess_frequency_bar
 
 
 def bar(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         error_x: str | list[str] = None,
         error_x_minus: str | list[str] = None,
         error_y: str | list[str] = None,
         error_y_minus: str | list[str] = None,
+        text: str | list[str] = None,
+        hover_name: str | list[str] = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         opacity: float = None,
         barmode: str = 'relative',
         log_x: bool = False,
         log_y: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         text_auto: bool | str = False,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns a bar chart
+    """Returns a bar chart
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x: str | list[str]:  (Default value = None)
+        A column or list of columns that contain x-axis values.
+      y: str | list[str]:  (Default value = None)
+        A column or list of columns that contain y-axis values.
+      error_x: str | list[str]:  (Default value = None)
+        A column or list of columns with x error bar
+        values. These form the error bars in both the positive and negative
+        direction if error_x_minus is not specified, and the error bars in
+        only the positive direction if error_x_minus is specified. None can be
+        used to specify no error bars on the corresponding series.
+      error_x_minus: str | list[str]:  (Default value = None)
+        A column or list of columns with x error
+        bar values. These form the error bars in the negative direction,
+        and are ignored if error_x is not specified.
+      error_y: str | list[str]:  (Default value = None)
+        A column or list of columns with x error bar
+        values. These form the error bars in both the positive and negative
+        direction if error_y_minus is not specified, and the error bars in
+        only the positive direction if error_y_minus is specified. None can be
+        used to specify no error bars on the corresponding series.
+      error_y_minus: str | list[str]:  (Default value = None)
+        A column or list of columns with y error
+        bar values. These form the error bars in the negative direction,
+        and are ignored if error_y is not specified.
+      text: str | list[str]:  (Default value = None)
+        A column or list of columns that contain text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column or list of columns that contain names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      pattern_shape_sequence: list[str]:  (Default value = None)
+        A list of patterns to sequentially apply
+        to the series. The patterns loop, so if there are more series than
+        patterns, patterns will be reused.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      barmode: str:  (Default value = 'relative')
+        If 'relative', bars are stacked. If 'overlay', bars are drawn on top
+        of each other. If 'group', bars are drawn next to each other.
+      log_x: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      log_y: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      range_x: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the x axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      range_y: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the y axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      text_auto: bool | str:  (Default value = False)
+        If True, display the value at each bar.
+        If a string, specifies a plotly texttemplate.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure: callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      DeephavenFigure: A DeephavenFigure that contains the bar chart
 
-    :param table: A table to pull data from.
-    :param x: A column or list of columns that contain x-axis values.
-    :param y: A column or list of columns that contain y-axis values.
-    :param error_x: A column or list of columns with x error bar
-    values. These form the error bars in both the positive and negative
-    direction if error_x_minus is not specified, and the error bars in only the
-    positive direction if error_x_minus is specified. None can be used to
-    specify no error bars on the corresponding series.
-    :param error_x_minus: A column or list of columns with x error
-    bar values. These form the error bars in the negative direction, and are
-    ignored if error_x is not specified.
-    :param error_y: A column or list of columns with x error bar
-    values. These form the error bars in both the positive and negative
-    direction if error_y_minus is not specified, and the error bars in only the
-    positive direction if error_y_minus is specified. None can be used to
-    specify no error bars on the corresponding series.
-    :param error_y_minus: A column or list of columns with x error
-    bar values. These form the error bars in the negative direction, and are
-    ignored if error_y is not specified.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param pattern_shape_sequence: A list of patterns to sequentially apply
-    to the series. The patterns loop, so if there are more series than
-    patterns, patterns will be reused.
-    :param opacity: Opacity to apply to all points. 0 is completely transparent
-    and 1 is completely opaque.
-    :param barmode: Default 'relative'. If 'relative', bars are stacked. If
-    'overlay', bars are drawn on top of each other. If 'group', bars are drawn
-    next to each other.
-    :param log_x: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param log_y: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param range_x: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param range_y: A list of two numbers or a list of lists of two numbers
-     that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param range_y: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param text_auto: Default False. If True, display the value at each bar.
-    If a string, specifies a plotly texttemplate.
-    :param title: The title of the chart
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the bar chart
     """
     args = locals()
-    args["pattern_shape_sequence_bar"] = args.pop("pattern_shape_sequence")
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
-    validate_common_args(args)
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"bar"})
 
     return update_wrapper(
         generate_figure(draw=px.bar, call_args=args)
     )
 
 
 def _bar_polar(
@@ -121,16 +141,38 @@
         direction: str = 'clockwise',
         start_angle: int = 90,
         range_r: list[int] = None,
         range_theta: list[int] = None,
         log_r: bool = False,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
+    """
+
+    Args:
+      table: Table:  (Default value = None)
+      r: str:  (Default value = None)
+      theta: str:  (Default value = None)
+      color_discrete_sequence: list[str]:  (Default value = None)
+      pattern_shape_sequence: list[str]:  (Default value = None)
+      # barnorm: str:  (Default value = None)
+      barmode: str:  (Default value = 'relative')
+      direction: str:  (Default value = 'clockwise')
+      start_angle: int:  (Default value = 90)
+      range_r: list[int]:  (Default value = None)
+      range_theta: list[int]:  (Default value = None)
+      log_r: bool:  (Default value = False)
+      title: str:  (Default value = None)
+      template: str:  (Default value = None)
+      unsafe_update_figure: Callable:  (Default value = default_callback)
+
+    Returns:
+
+    """
     # todo: not yet implemented
     if isinstance(table, Table):
         args = locals()
         args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
         validate_common_args(args)
 
@@ -138,138 +180,177 @@
 
 
 def timeline(
         table: str = None,
         x_start: str = None,
         x_end: str = None,
         y: str = None,
+        text: str = None,
+        hover_name: str = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         opacity: float = None,
         range_x: list[int] = None,
         range_y: list[int] = None,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ):
-    """
-    Returns a timeline (otherwise known as a gantt chart)
+    """Returns a timeline (otherwise known as a gantt chart)
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x_start: str:  (Default value = None)
+        A column that contains starting x-axis values.
+      x_end: str:  (Default value = None)
+        A column that contains ending x-axis values.
+      y: str:  (Default value = None)
+        A column that contains y-axis labels
+      text: str:  (Default value = None)
+        A column that contains text annotations.
+      hover_name: str:  (Default value = None)
+        A column that contains names to bold in the hover tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      pattern_shape_sequence: list[str]:  (Default value = None)
+        A list of patterns to sequentially apply
+        to the series. The patterns loop, so if there are more series than
+        patterns, patterns will be reused.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      range_x: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the x axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      range_y: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the y axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure: callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      A DeephavenFigure that contains the timeline chart
 
-    :param table: A table to pull data from.
-    :param x_start: A column that contains starting x-axis values.
-    :param x_end: A column that contains ending x-axis values.
-    :param y: A column or list of columns that contain y-axis labels
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param pattern_shape_sequence: A list of patterns to sequentially apply
-    to the series. The patterns loop, so if there are more series than
-    patterns, patterns will be reused.
-    :param opacity: Opacity to apply to all points. 0 is completely transparent
-    and 1 is completely opaque.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param title: The title of the chart
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the timeline chart
     """
     # TODO: add resource column?
     table, x_diff = preprocess_timeline(table, x_start, x_end, y)
     args = locals()
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
 
-    validate_common_args(args)
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"marker"})
 
     return update_wrapper(
         generate_figure(draw=px.timeline, call_args=args)
     )
 
 
 def frequency_bar(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         pattern_shape_sequence: list[str] = None,
         opacity: float = None,
         barmode: str = 'relative',
         log_x: bool = False,
         log_y: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         text_auto: bool | str = False,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ):
-    """
-    Returns a bar chart that contains the counts of the specified columns
+    """Returns a bar chart that contains the counts of the specified columns
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x: str | list[str]:  (Default value = None)
+        A column or list of columns that contain x-axis values.
+        Only one of x or y can be specified. If x is specified, the bars
+        are drawn vertically.
+      y: str | list[str]:  (Default value = None)
+        A column or list of columns that contain y-axis values.
+        Only one of x or y can be specified. If y is specified, the bars
+        are drawn horizontally.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      pattern_shape_sequence: list[str]:  (Default value = None)
+        A list of patterns to sequentially apply
+        to the series. The patterns loop, so if there are more series than
+        patterns, patterns will be reused.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      barmode: str:  (Default value = 'relative')
+        If 'relative', bars are stacked. If 'overlay', bars are drawn on top
+        of each other. If 'group', bars are drawn next to each other.
+      log_x: bool
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      log_y: bool
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      range_x: list[int]:  (Default value = None)
+        A list of two numbers that specify the range of the x-axis.
+      range_y: list[int]:  (Default value = None)
+        A list of two numbers that specify the range of the y-axis.
+      text_auto: bool | str:  (Default value = False)
+        If True, display the value at each bar.
+        If a string, specifies a plotly texttemplate.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure: callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      DeephavenFigure: A DeephavenFigure that contains the bar chart
 
-    :param table: A table to pull data from.
-    :param x: A column name or list of columns that contain x-axis values.
-    Only one of x or y can be specified. If x is specified, the bars are drawn
-    vertically.
-    :param y: A column name or list of columns that contain y-axis values.
-    Only one of x or y can be specified. If x is specified, the bars are drawn
-    horizontally.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param pattern_shape_sequence: A list of patterns to sequentially apply
-    to the series. The patterns loop, so if there are more series than
-    patterns, patterns will be reused.
-    :param opacity: Opacity to apply to all points. 0 is completely transparent
-    and 1 is completely opaque.
-    :param barmode: Default 'relative'. If 'relative', bars are stacked. If
-    'overlay', bars are drawn on top of each other. If 'group', bars are drawn
-    next to each other.
-    :param log_x: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_y: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param text_auto: Default False. If True, display the value at each bar.
-    If a string, specifies a plotly texttemplate.
-    :param title: The title of the chart
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the bar chart
     """
 
     if x and y:
         raise ValueError("Cannot specify both x and y")
 
     args = locals()
-    args["color_discrete_sequence_marker"] = args.pop("color_discrete_sequence")
-    args["pattern_shape_sequence_bar"] = args.pop("pattern_shape_sequence")
 
-    validate_common_args(args)
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"bar"})
 
     create_layered = partial(preprocess_and_layer,
                              preprocess_frequency_bar,
-                             px.bar, args, list_var_axis_name="value")
+                             px.bar, args)
 
     return update_wrapper(
         create_layered("x") if x else create_layered("y", orientation="h")
     )
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/line.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/scatter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,368 +1,471 @@
-from functools import partial
-from typing import Callable
-
 from plotly import express as px
 
 from deephaven.table import Table
 
-from ._private_utils import default_callback, validate_common_args, remap_scene_args, unsafe_figure_update_wrapper
+from .distribution import attach_marginals, get_marg_args
+from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
 
 
-# TODO: support line_shape as a list?
-def line(
+def scatter(
         table: Table = None,
         x: str | list[str] = None,
         y: str | list[str] = None,
         error_x: str | list[str] = None,
         error_x_minus: str | list[str] = None,
         error_y: str | list[str] = None,
         error_y_minus: str | list[str] = None,
         size: str | list[str] = None,
+        text: str | list[str] = None,
+        hover_name: str | list[str] = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
-        line_dash_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
         size_sequence: list[int] = None,
-        xaxis_sequence: list[str] = None,
-        yaxis_sequence: list[str] = None,
-        markers: bool = False,
+        xaxis_sequence: list[int] = None,
+        yaxis_sequence: list[int] = None,
+        opacity: float = None,
+        marginal_x: str = None,
+        marginal_y: str = None,
         log_x: bool | list[bool] = False,
         log_y: bool | list[bool] = False,
         range_x: list[int] | list[list[int]] = None,
         range_y: list[int] | list[list[int]] = None,
         yaxis_titles: list[str] = None,
         xaxis_titles: list[str] = None,
-        line_shape: str = 'linear',
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns a line chart
+    """Returns a scatter chart
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x: str | list[str]:  (Default value = None)
+        A column or list of columns that contain x-axis values.
+      y: str | list[str]:  (Default value = None)
+        A column or list of columns that contain y-axis values.
+      error_x: str | list[str]:  (Default value = None)
+        A column or list of columns with x error bar
+        values. These form the error bars in both the positive and negative
+        direction if error_x_minus is not specified, and the error bars in
+        only the positive direction if error_x_minus is specified. None can be
+        used to specify no error bars on the corresponding series.
+      error_x_minus: str | list[str]:  (Default value = None)
+        A column or list of columns with x error
+        bar values. These form the error bars in the negative direction,
+        and are ignored if error_x is not specified.
+      error_y: str | list[str]:  (Default value = None)
+        A column or list of columns with x error bar
+        values. These form the error bars in both the positive and negative
+        direction if error_y_minus is not specified, and the error bars in
+        only the positive direction if error_y_minus is specified. None can be
+        used to specify no error bars on the corresponding series.
+      error_y_minus: str | list[str]:  (Default value = None)
+        A column or list of columns with y error
+        bar values. These form the error bars in the negative direction,
+        and are ignored if error_y is not specified.
+      size: str | list[str]:  (Default value = None)
+        A column or list of columns that contain size values.
+      text: str | list[str]:  (Default value = None)
+        A column or list of columns that contain text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column or list of columns that contain names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      symbol_sequence: list[str]:  (Default value = None)
+        A list of symbols to sequentially apply to the
+        markers in the series. The symbols loop, so if there are more series than
+        symbols, symbols will be reused.
+      size_sequence: list[str]:  (Default value = None)
+        A list of sizes to sequentially apply to the
+        markers in the series. The sizes loop, so if there are more series than
+        symbols, sizes will be reused. This is overriden is "size" is specified.
+      xaxis_sequence: list[str]:  (Default value = None)
+        A list of x axes to assign series to. Odd numbers
+        starting with 1 are created on the bottom x axis and even numbers starting
+        with 2 are created on the top x axis. Axes are created up
+        to the maximum number specified. The axes loop, so if there are more series
+        than axes, axes will be reused.
+      yaxis_sequence: list[str]:  (Default value = None)
+        A list of y axes to assign series to. Odd numbers
+        starting with 1 are created on the left y axis and even numbers starting
+        with 2 are created on the top y axis. Axes are created up
+        to the maximum number specified. The axes loop, so if there are more series
+        than axes, axes will be reused.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      marginal_x: str:  (Default value = None)
+        The type of x-axis marginal; histogram, violin, rug, box
+      marginal_y: str:  (Default value = None)
+        The type of y-axis marginal; histogram, violin, rug, box
+      log_x: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      log_y: bool | list[bool]:  (Default value = False)
+        A boolean or list of booleans that specify if
+        the corresponding axis is a log axis or not. The booleans loop, so if there
+        are more series than booleans, booleans will be reused.
+      range_x: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the x axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      range_y: list[int] | list[list[int]]:  (Default value = None)
+        A list of two numbers or a list of lists of two numbers
+        that specify the range of the y axes. None can be specified for no range
+        The ranges loop, so if there are more axes than ranges, ranges will
+        be reused.
+      yaxis_titles: list[str]:  (Default value = None)
+        A list of titles to sequentially apply to the y axes. The titles do not
+          loop.
+      xaxis_titles: list[str]:  (Default value = None)
+        A list of titles to sequentially apply to the x axes. The titles do not
+          loop.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure:  callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      A DeephavenFigure that contains the scatter chart
 
-    :param table: A table to pull data from.
-    :param x: A column or list of columns that contain x-axis values.
-    :param y: A column or list of columns that contain y-axis values.
-    :param error_x: A column or list of columns with x error bar
-    values. These form the error bars in both the positive and negative
-    direction if error_x_minus is not specified, and the error bars in only the
-    positive direction if error_x_minus is specified. None can be used to
-    specify no error bars on the corresponding series.
-    :param error_x_minus: A column or list of columns with x error
-    bar values. These form the error bars in the negative direction, and are
-    ignored if error_x is not specified.
-    :param error_y: A column or list of columns with x error bar
-    values. These form the error bars in both the positive and negative
-    direction if error_y_minus is not specified, and the error bars in only the
-    positive direction if error_y_minus is specified. None can be used to
-    specify no error bars on the corresponding series.
-    :param error_y_minus: A column or list of columns with x error
-    bar values. These form the error bars in the negative direction, and are
-    ignored if error_y is not specified.
-    :param size: A column or list of columns that contain size values.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param line_dash_sequence: A list of line dashes to sequentially apply to
-    the series. The dashes loop, so if there are more series than dashes,
-    dashes will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    markers in the series. The symbols loop, so if there are more series than
-    symbols, symbols will be reused.
-    :param size_sequence: A list of sizes to sequentially apply to the
-    markers in the series. The sizes loop, so if there are more series than
-    symbols, sizes will be reused. This is overriden is "size" is specified.
-    :param xaxis_sequence: A list of x axes to assign series to. Odd numbers
-    starting with 1 are created on the bottom x axis and even numbers starting
-    with 2 are created on the top x axis. Axes are created up
-    to the maximum number specified. The axes loop, so if there are more series
-    than axes, axes will be reused.
-    :param yaxis_sequence: A list of y axes to assign series to. Odd numbers
-    starting with 1 are created on the left y axis and even numbers starting
-    with 2 are created on the top y axis. Axes are created up
-    to the maximum number specified. The axes loop, so if there are more series
-    than axes, axes will be reused.
-    :param markers: True to draw markers on the line, False to not. Default
-    False
-    :param log_x: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param log_y: Default False. A boolean or list of booleans that specify if
-    the corresponding axis is a log axis or not. The booleans loop, so if there
-    are more series than booleans, booleans will be reused.
-    :param range_x: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param range_y: A list of two numbers or a list of lists of two numbers
-    that specify the range of the x axes. None can be specified for no range
-    The ranges loop, so if there are more axes than ranges, ranges will
-    be reused.
-    :param yaxis_titles: A list of titles to sequentially apply to the
-    y axes. The titles do not loop.
-    :param xaxis_titles: A list of titles to sequentially apply to the
-    x axes. The titles do not loop.
-    :param line_shape: The line shape for all lines created. One of 'linear',
-    'spline', 'vhv', 'hvh', 'vh', 'hv'. Default 'linear'
-    :param title: The title of the chart
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the line chart
     """
     args = locals()
 
-    validate_common_args(args)
+    marg_data, marg_style = get_marg_args(args)
 
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"scatter"})
 
     return update_wrapper(
-        generate_figure(draw=px.line, call_args=args)
+        attach_marginals(
+            generate_figure(draw=px.scatter, call_args=args),
+            marg_data,
+            marg_style,
+            marginal_x=marginal_x, marginal_y=marginal_y,
+        )
     )
 
 
-def line_3d(
+def scatter_3d(
         table: Table = None,
         x: str = None,
         y: str = None,
         z: str = None,
-        error_x: str | list[str] = None,
-        error_x_minus: str | list[str] = None,
-        error_y: str | list[str] = None,
-        error_y_minus: str | list[str] = None,
-        error_z: str | list[str] = None,
-        error_z_minus: str | list[str] = None,
-        size: str | list[str] = None,
+        error_x: str = None,
+        error_x_minus: str = None,
+        error_y: str = None,
+        error_y_minus: str = None,
+        error_z: str = None,
+        error_z_minus: str = None,
+        size: str = None,
+        text: str = None,
+        hover_name: str = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
         size_sequence: list[int] = None,
-        markers: bool = False,
+        opacity: float = None,
         log_x: bool = False,
         log_y: bool = False,
         log_z: bool = False,
         range_x: list[int] = None,
         range_y: list[int] = None,
         range_z: list[int] = None,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns a 3D line chart
+    """Returns a 3D scatter chart
 
-    :param table: A table to pull data from.
-    :param x: A column that contains x-axis values.
-    :param y: A column that contains y-axis values.
-    :param z: A column that contains z-axis values.
-    :param error_x: A column with x error bar values. These form the error
-    bars in both the positive and negative direction if error_x_minus is not
-    specified, and the error bars in only the positive direction if
-    error_x_minus is specified.
-    :param error_x_minus: A column with x error bar values. These form
-    the error bars in the negative direction, and are ignored if error_x is not
-    specified.
-    :param size: A column or list of columns that contain size values.
-    :param error_y: A column with x error bar values. These form the error
-    bars in both the positive and negative direction if error_z_minus is not
-    specified, and the error bars in only the positive direction if
-    error_x_minus is specified.
-    :param error_y_minus: A column with y error bar values. These form
-    the error bars in the negative direction, and are ignored if error_x is not
-    specified.
-    :param error_z: A column with x error bar values. These form the error
-    bars in both the positive and negative direction if error_z_minus is not
-    specified, and the error bars in only the positive direction if
-    error_x_minus is specified.
-    :param error_z_minus: A column with z error bar values. These form
-    the error bars in the negative direction, and are ignored if error_x is not
-    specified.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    markers in the series. The symbols loop, so if there are more series than
-    symbols, symbols will be reused.
-    :param size_sequence: A list of sizes to sequentially apply to the
-    markers in the series. The sizes loop, so if there are more series than
-    symbols, sizes will be reused. This is overriden is "size" is specified.
-    :param markers: True to draw markers on the line, False to not. Default
-    False
-    :param log_x: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_y: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param log_z: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param range_x: A list of two numbers that specify the range of the x axis.
-    :param range_y: A list of two numbers that specify the range of the y axis.
-    :param range_z: A list of two numbers that specify the range of the z axis.
-    :param title: The title of the chart.
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the 3D line chart
-    """
-    args = locals()
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      x: str:  (Default value = None)
+        A column that contains x-axis values.
+      y: str:  (Default value = None)
+        A column that contains y-axis values.
+      z: str:  (Default value = None)
+        A column that contains z-axis values.
+      error_x: str:  (Default value = None)
+        A column with x error bar values. These form the error
+        bars in both the positive and negative direction if error_x_minus
+        is not specified, and the error bars in only the positive direction if
+        error_x_minus is specified.
+      error_x_minus: str:  (Default value = None)
+        A column with x error bar values. These form
+        the error bars in the negative direction, and are ignored if error_x
+        is not specified.
+      error_y: str:  (Default value = None)
+        A column with y error bar values. These form the error
+        bars in both the positive and negative direction if error_y_minus
+        is not specified, and the error bars in only the positive direction if
+        error_y_minus is specified.
+      error_y_minus: str:  (Default value = None)
+        A column with y error bar values. These form
+        the error bars in the negative direction, and are ignored if error_y
+        is not specified.
+      error_z: str:  (Default value = None)
+        A column with z error bar values. These form the error
+        bars in both the positive and negative direction if error_z_minus
+        is not specified, and the error bars in only the positive direction if
+        error_z_minus is specified.
+      error_z_minus: str:  (Default value = None)
+        A column with z error bar values. These form
+        the error bars in the negative direction, and are ignored if error_z
+        is not specified.
+      size: str:  (Default value = None)
+        A column that contains size values.
+      text: str:  (Default value = None)
+        A column that contains text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column that contains names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      symbol_sequence: list[str]:  (Default value = None)
+        A list of symbols to sequentially apply to the
+        markers in the series. The symbols loop, so if there are more series than
+        symbols, symbols will be reused.
+      size_sequence: list[str]:  (Default value = None)
+        A list of sizes to sequentially apply to the
+        markers in the series. The sizes loop, so if there are more series than
+        symbols, sizes will be reused. This is overriden is "size" is specified.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      log_x: bool:  (Default value = False)
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      log_y: bool:  (Default value = False)
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      log_z: bool:  (Default value = False)
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      range_x: list[int]:  (Default value = None)
+        A list of two numbers that specify the range of the x axis.
+      range_y: list[int]:  (Default value = None)
+        A list of two numbers that specify the range of the y axis.
+      range_z: list[int]:  (Default value = None)
+        A list of two numbers that specify the range of the z axis.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure:  callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
 
-    validate_common_args(args)
+    Returns:
+      A DeephavenFigure that contains the 3D scatter chart
 
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
+    """
+    args = locals()
 
-    remap_scene_args(args)
-
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"scatter", "scene"})
 
     return update_wrapper(
-        generate_figure(draw=px.line_3d, call_args=args)
+        generate_figure(draw=px.scatter_3d, call_args=args)
     )
 
 
-def line_polar(
+def scatter_polar(
         table: Table = None,
         r: str = None,
         theta: str = None,
-        size: str | list[str] = None,
+        size: str = None,
+        text: str = None,
+        hover_name: str = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
         size_sequence: list[int] = None,
-        markers: bool = False,
+        opacity: float = None,
         direction: str = 'clockwise',
         start_angle: int = 90,
-        line_close: bool = False,
-        line_shape: str = 'linear',
         range_r: list[int] = None,
         range_theta: list[int] = None,
         log_r: bool = False,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns a polar scatter chart
+    """Returns a polar scatter chart
+
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      r: str:  (Default value = None)
+        A column that contains r values.
+      theta: str:  (Default value = None)
+        A column that contains theta values.
+      size: str:  (Default value = None)
+        A column that contains size values.
+      text: str:  (Default value = None)
+        A column that contains text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column that contains names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      symbol_sequence: list[str]:  (Default value = None)
+        A list of symbols to sequentially apply to the
+        markers in the series. The symbols loop, so if there are more series than
+        symbols, symbols will be reused.
+      size_sequence: list[str]:  (Default value = None)
+        A list of sizes to sequentially apply to the
+        markers in the series. The sizes loop, so if there are more series than
+        symbols, sizes will be reused. This is overriden is "size" is specified.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      direction: (Default value = 'clockwise')
+        Which direction points are drawn. Can be 'clockwise' or
+        'counterclockwise'
+      start_angle: int:  (Default value = 90)
+        Sets start angle.
+      range_r: list[int]:
+        A list of two numbers that specify the range of r.
+      range_theta: list[int]:
+        A list of two numbers that specify the range of theta.
+      log_r: bool
+        A boolean that specifies if the corresponding axis is a log
+        axis or not.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure:  callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
+
+    Returns:
+      A DeephavenFigure that contains the polar scatter chart
 
-    :param table: A table to pull data from.
-    :param r: A column that contains r values.
-    :param theta: A column that contains theta values.
-    :param size: A column or list of columns that contain size values.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    markers in the series. The symbols loop, so if there are more series than
-    symbols, symbols will be reused.
-    :param size_sequence: A list of sizes to sequentially apply to the
-    markers in the series. The sizes loop, so if there are more series than
-    symbols, sizes will be reused. This is overriden is "size" is specified.
-    :param markers: True to draw markers on the line, False to not. Default
-    False
-    :param direction: Which direction points are drawn. Default clockwise.
-    :param start_angle: Sets start angle. Default 90.
-    :param line_close: True draw a line between first and last point, False to
-    not. Default False
-    :param line_shape: The line shape for all lines created. One of 'linear',
-    'spline'. Default 'linear'
-    :param range_r: A list of two numbers that specify the range of r.
-    :param range_theta: A list of two numbers that specify the range of theta.
-    :param log_r: A boolean that specifies if the corresponding axis is a log
-    axis or not.
-    :param title: The title of the chart.
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the polar scatter chart
     """
     args = locals()
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
-
-    validate_common_args(args)
 
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"scatter"})
 
     return update_wrapper(
-        generate_figure(draw=px.line_polar, call_args=args)
+        generate_figure(draw=px.scatter_polar, call_args=args)
     )
 
 
-def line_ternary(
+def scatter_ternary(
         table: Table = None,
         a: str = None,
         b: str = None,
         c: str = None,
-        size: str | list[str] = None,
+        size: str = None,
+        text: str= None,
+        hover_name: str = None,
+        labels: dict[str, str] = None,
         color_discrete_sequence: list[str] = None,
         symbol_sequence: list[str] = None,
         size_sequence: list[int] = None,
-        markers: bool = False,
-        line_shape: str = 'linear',
+        opacity: float = None,
         title: str = None,
         template: str = None,
-        unsafe_update_figure: Callable = default_callback
+        unsafe_update_figure: callable = default_callback
 ) -> DeephavenFigure:
-    """
-    Returns a ternary line chart
+    """Returns a ternary scatter chart
 
-    :param table: A table to pull data from.
-    :param a: A column that contains a-axis values.
-    :param b: A column that contains b-axis values.
-    :param c: A column that contains c-axis values.
-    :param size: A column or list of columns that contain size values.
-    :param color_discrete_sequence: A list of colors to sequentially apply to
-    the series. The colors loop, so if there are more series than colors,
-    colors will be reused.
-    :param symbol_sequence: A list of symbols to sequentially apply to the
-    markers in the series. The symbols loop, so if there are more series than
-    symbols, symbols will be reused.
-    :param size_sequence: A list of sizes to sequentially apply to the
-    markers in the series. The sizes loop, so if there are more series than
-    symbols, sizes will be reused. This is overriden is "size" is specified.
-    :param markers: True to draw markers on the line, False to not. Default
-    False
-    :param line_shape: The line shape for all lines created. One of 'linear',
-    'spline'. Default 'linear'
-    :param title: The title of the chart.
-    :param template: The template for the chart.
-    :param unsafe_update_figure: An update function that takes a plotly figure
-    as an argument and optionally returns a plotly figure. If a figure is not
-    returned, the plotly figure passed will be assumed to be the return value.
-    Used to add any custom changes to the underlying plotly figure. Note that
-    the existing data traces should not be removed. This may lead to unexpected
-    behavior if traces are modified in a way that break data mappings.
-    :return: A DeephavenFigure that contains the ternary line chart
-    """
-    args = locals()
+    Args:
+      table: Table:  (Default value = None)
+        A table to pull data from.
+      a: str:
+        A column that contains a-axis values.
+      b: str:
+        A column that contains b-axis values.
+      c: str:
+        A column that contains c-axis values.
+      size: str:  (Default value = None)
+        A column that contains size values.
+      text: str:  (Default value = None)
+        A column that contains text annotations.
+      hover_name: str | list[str]:  (Default value = None)
+        A column that contains names to bold in the hover
+          tooltip.
+      labels: dict[str, str]:  (Default value = None)
+        A dictionary of labels mapping columns to new labels.
+      color_discrete_sequence: list[str]:  (Default value = None)
+        A list of colors to sequentially apply to
+        the series. The colors loop, so if there are more series than colors,
+        colors will be reused.
+      symbol_sequence: list[str]:  (Default value = None)
+        A list of symbols to sequentially apply to the
+        markers in the series. The symbols loop, so if there are more series than
+        symbols, symbols will be reused.
+      size_sequence: list[str]:  (Default value = None)
+        A list of sizes to sequentially apply to the
+        markers in the series. The sizes loop, so if there are more series than
+        symbols, sizes will be reused. This is overriden is "size" is specified.
+      opacity: float:  (Default value = None)
+        Opacity to apply to all markers. 0 is completely transparent
+        and 1 is completely opaque.
+      title: str: (Default value = None)
+        The title of the chart
+      template: str:  (Default value = None)
+        The template for the chart.
+      unsafe_update_figure:  callable:  (Default value = default_callback)
+        An update function that takes a plotly figure
+        as an argument and optionally returns a plotly figure. If a figure is
+        not returned, the plotly figure passed will be assumed to be the return
+        value. Used to add any custom changes to the underlying plotly figure.
+        Note that the existing data traces should not be removed. This may lead
+        to unexpected behavior if traces are modified in a way that break data
+        mappings.
 
-    validate_common_args(args)
+    Returns:
+      A DeephavenFigure that contains the ternary scatter chart
 
-    args["color_discrete_sequence_line"] = args.pop("color_discrete_sequence")
+    """
+    args = locals()
 
-    update_wrapper = partial(
-        unsafe_figure_update_wrapper,
-        args.pop("unsafe_update_figure")
-    )
+    update_wrapper = process_args(args, {"scatter"})
 
     return update_wrapper(
-        generate_figure(draw=px.line_ternary, call_args=args)
+        generate_figure(draw=px.scatter_ternary, call_args=args)
     )
+
+
+def _scatter_matrix():
+    """ """
+    # todo: not yet implemented
+    pass
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/subplots.py` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/subplots.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,36 @@
 def get_new_specs(
         specs: list[list[dict[str, int | float]]],
         row_starts: list[float],
         row_ends: list[float],
         col_starts: list[float],
         col_ends: list[float],
 ) -> list[dict[str, list[float]]]:
-    """
-    Transforms the given specs and row and column lists to specs for layering
+    """Transforms the given specs and row and column lists to specs for layering
+
+    Args:
+      specs: list[list[dict[str, int | float]]]
+        A 2 dimensional list that contains the specs per figure
+      row_starts: list[float]:
+        A list of domain values on the y-axis where the corresponding
+        figure will start
+      row_ends: list[float]:
+        A list of domain values on the y-axis where the corresponding
+        figure will end
+      col_starts: list[float]:
+        A list of domain values on the y-axis where the corresponding
+        figure will start
+      col_ends: list[float]:
+        A list of domain values on the y-axis where the corresponding
+        figure will end
+
+    Returns:
+      list[dict[str, list[float]]]:
+        The new specs with x and y domains, to be passed to layering
 
-    :param specs: A 2 dimensional list that contains the specs per figure
-    :param row_starts: A list of domain values on the y-axis where the
-    corresponding figure will start
-    :param row_ends: A list of domain values on the y-axis where the
-    corresponding figure will end
-    :param col_starts: A list of domain values on the x-axis where the
-    corresponding figure will start
-    :param col_ends: A list of domain values on the x-axis where the
-    corresponding figure will end
-    :return: The new specs with x and y domains, to be passed to layering
     """
     new_specs = []
 
     for row, (y_0, y_1) in enumerate(zip(row_starts, row_ends)):
         for col, (x_0, x_1) in enumerate(zip(col_starts, col_ends)):
             spec = {} if not specs or specs[row][col] is None else specs[row][col]
             l = spec.get("l", 0)
@@ -47,26 +56,32 @@
     return new_specs
 
 
 def make_grid(
         items: list[any],
         rows: int,
         cols: int,
-        fill=None
+        fill: any = None
 ) -> list[list[any]]:
-    """
-    Make a grid (list of lists) out of the provided items
+    """Make a grid (list of lists) out of the provided items
+
+    Args:
+      items: int:
+        A list of items to put in the grid
+      rows: int:
+        The number of rows in the grid
+      cols: int:
+        The number of cols in the grid
+      fill: any:  (Default value = None)
+        If there are more slots (as defined by rows * columns) than
+        provided items, then the remaining items in the grid have this value.
+
+    Returns:
+      list[list[any]]: The generated grid
 
-    :param items: A list of items to put in the grid
-    :param rows: The number of rows in the grid
-    :param cols: The number of cols in the grid
-    :param fill: If there are more slots (as defined by rows * columns) than
-    provided items, then the remaining items in the grid have this value.
-    Default None.
-    :return: The generated grid
     """
     grid = []
     index = 0
     for row in range(rows):
         grid_row = []
         for col in range(cols):
             # if there are more slots in the grid then there are items, pad
@@ -79,21 +94,27 @@
     return grid
 
 
 def get_domains(
         values: list[float],
         spacing: float
 ) -> tuple[list[float], list[float]]:
-    """
-    Get the domains from a list of percentage values. The domains are
+    """Get the domains from a list of percentage values. The domains are
     cumulative and account for spacing.
 
-    :param values: The list of values to scale due to spacing then
-    :param spacing: The spacing between each value.
-    :return: A tuple of (list of domain starts, list of domain ends)
+    Args:
+      values: list[float]:
+        The list of values to scale due to spacing then
+      spacing: float:
+        The spacing between each value.
+
+    Returns:
+      tuple[list[float], list[float]]
+        A tuple of (list of domain starts, list of domain ends)
+
     """
     # scale the values by however much the spacing uses between each col or row
     scale = 1 - (spacing * (len(values) - 1))
     scaled = [v * scale for v in values]
 
     # the first start value is just 0 since there is no spacing preceeding it
     starts = [0]
@@ -118,42 +139,57 @@
         horizontal_spacing: float = None,
         vertical_spacing: float = None,
         column_widths: list[float] = None,
         row_heights: list[float] = None,
         specs: list[dict[str, int | float]] |
                list[list[dict[str, int | float]]] = None,
 ) -> DeephavenFigure:
-    """
-    Create subplots. Either figs and at least one of rows and cols or grid
+    """Create subplots. Either figs and at least one of rows and cols or grid
     should be passed.
 
-    :param figs: Figures to use. Should be used with rows and/or cols.
-    :param rows: A list of rows in the resulting subplot grid. This is
-    calculated from cols and number of figs provided if not passed but cols is.
-    One of rows or cols should be provided if passing figs directly.
-    :param cols: A list of cols in the resulting subplot grid. This is
-    calculated from rows and number of figs provided if not passed but rows is.
-    One of rows or cols should be provided if passing figs directly.
-    :param grid: A grid (list of lists) of figures to draw. None can be
-    provided in a grid entry
-    :param horizontal_spacing: Spacing between each column. Default 0.2 / cols
-    :param vertical_spacing: Spacing between each row. Default 0.3 / rows
-    :param column_widths: The widths of each column. Should sum to 1.
-    :param row_heights: The heights of each row. Should sum to 1.
-    :param specs: A list or grid of dicts that contain specs. An empty
-    dictionary represents no specs, and None represents no figure, either
-    to leave a gap on the subplots on provide room for a figure spanning
-    multiple columns.
-    'l' is a float that adds left padding
-    'r' is a float that adds right padding
-    't' is a float that adds top padding
-    'b' is a float that adds bottom padding
-    'rowspan' is an int to make this figure span multiple rows
-    'colspan' is an int to make this figure span multiple columns
-    :return: The DeephavenFigure with subplots
+    Args:
+      *figs: Figure | DeephavenFigure
+        Figures to use. Should be used with rows and/or cols.
+      rows: int: (Default value = None)
+        A list of rows in the resulting subplot grid. This is
+        calculated from cols and number of figs provided if not passed
+        but cols is.
+        One of rows or cols should be provided if passing figs directly.
+      cols: int: (Default value = None)
+        A list of cols in the resulting subplot grid. This is
+        calculated from rows and number of figs provided if not passed
+        but rows is.
+        One of rows or cols should be provided if passing figs directly.
+      grid: list[list[Figure | DeephavenFigure]] (Default value = None)
+        A grid (list of lists) of figures to draw. None can be
+        provided in a grid entry
+      horizontal_spacing: float: (Default value = None)
+        Spacing between each column. Default 0.2 / cols
+      vertical_spacing: float: (Default value = None)
+        Spacing between each row. Default 0.3 / rows
+      column_widths: list[float] (Default value = None)
+        The widths of each column. Should sum to 1.
+      row_heights: list[float] (Default value = None)
+        The heights of each row. Should sum to 1.
+      specs: list[dict[str, int | float]] | list[list[dict[str, int | float]]]
+        (Default value = None)
+        A list or grid of dicts that contain specs. An empty
+        dictionary represents no specs, and None represents no figure, either
+        to leave a gap on the subplots on provide room for a figure spanning
+        multiple columns.
+        'l' is a float that adds left padding
+        'r' is a float that adds right padding
+        't' is a float that adds top padding
+        'b' is a float that adds bottom padding
+        'rowspan' is an int to make this figure span multiple rows
+        'colspan' is an int to make this figure span multiple columns
+
+    Returns:
+      DeephavenFigure: The DeephavenFigure with subplots
+
     """
     if rows or cols:
         rows = rows if rows else math.ceil(len(figs) / cols)
         cols = cols if cols else math.ceil(len(figs) / rows)
 
     grid = grid if grid else make_grid(list(figs), rows, cols)
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.3
+Version: 0.0.4
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt` & `deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/deephaven/plot/express/__init__.py
 src/deephaven/plot/express/data_mapping/DataMapping.py
 src/deephaven/plot/express/data_mapping/__init__.py
 src/deephaven/plot/express/data_mapping/data_mapping.py
+src/deephaven/plot/express/data_mapping/data_mapping_constants.py
 src/deephaven/plot/express/data_mapping/json_conversion.py
 src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
 src/deephaven/plot/express/deephaven_figure/__init__.py
 src/deephaven/plot/express/deephaven_figure/custom_draw.py
 src/deephaven/plot/express/deephaven_figure/generate.py
 src/deephaven/plot/express/plots/__init__.py
 src/deephaven/plot/express/plots/_private_utils.py
```


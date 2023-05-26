# Comparing `tmp/deephaven-plugin-plotly-0.0.1.dev2.tar.gz` & `tmp/deephaven-plugin-plotly-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-0.0.1.dev2.tar", last modified: Fri May 26 15:21:17 2023, max compression
+gzip compressed data, was "deephaven-plugin-plotly-0.1.0.tar", last modified: Fri May 26 15:32:52 2023, max compression
```

## Comparing `deephaven-plugin-plotly-0.0.1.dev2.tar` & `deephaven-plugin-plotly-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/figure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/theme_deephaven.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.023145 deephaven-plugin-plotly-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 15:32:52.023145 deephaven-plugin-plotly-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-26 15:32:52.023145 deephaven-plugin-plotly-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.019145 deephaven-plugin-plotly-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.019145 deephaven-plugin-plotly-0.1.0/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.019145 deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.023145 deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/figure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-26 15:32:42.000000 deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/theme_deephaven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:32:52.023145 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:32:52.000000 deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/LICENSE` & `deephaven-plugin-plotly-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/PKG-INFO` & `deephaven-plugin-plotly-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly
-Version: 0.0.1.dev2
+Version: 0.1.0
 Summary: Deephaven Plugin for Plotly
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly
 Author: Devin Smith, Vlad Babich
 Author-email: vladbabich@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly/issues
 Keywords: deephaven,plugin,plotly
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/README.md` & `deephaven-plugin-plotly-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/setup.cfg` & `deephaven-plugin-plotly-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/__init__.py` & `deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from deephaven.plugin import Registration
 from plotly import io as pio
 
-__version__ = "0.0.1.dev2"
+__version__ = "0.1.0"
 
 def _init_theme():
     # Set the Deephaven style globally
     from . import theme_deephaven
     pio.templates.default = "deephaven"
     # Disable default renderer to ignore figure.show()
     pio.renderers.default = None
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/figure_type.py` & `deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/figure_type.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/theme_deephaven.py` & `deephaven-plugin-plotly-0.1.0/src/deephaven/plugin/plotly/theme_deephaven.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/PKG-INFO` & `deephaven-plugin-plotly-0.1.0/src/deephaven_plugin_plotly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly
-Version: 0.0.1.dev2
+Version: 0.1.0
 Summary: Deephaven Plugin for Plotly
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly
 Author: Devin Smith, Vlad Babich
 Author-email: vladbabich@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly/issues
 Keywords: deephaven,plugin,plotly
```


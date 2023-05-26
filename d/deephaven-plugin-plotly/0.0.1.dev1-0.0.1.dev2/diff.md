# Comparing `tmp/deephaven-plugin-plotly-0.0.1.dev1.tar.gz` & `tmp/deephaven-plugin-plotly-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/vladbabich/Sites/Deephaven/PlotlyAPI/deephaven-plugin-plotly/dist/tmpv4tu036a/deephaven-plugin-plotly-0.0.1.dev1.tar", last modified: Thu Aug 25 18:02:53 2022, max compression
+gzip compressed data, was "deephaven-plugin-plotly-0.0.1.dev2.tar", last modified: Fri May 26 15:21:17 2023, max compression
```

## Comparing `deephaven-plugin-plotly-0.0.1.dev1.tar` & `deephaven-plugin-plotly-0.0.1.dev2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/
--rw-r--r--   0 vladbabich   (501) staff       (20)    11358 2022-08-23 16:49:32.000000 deephaven-plugin-plotly-0.0.1.dev1/LICENSE
--rw-r--r--   0 vladbabich   (501) staff       (20)     2425 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 vladbabich   (501) staff       (20)     1606 2022-08-23 18:22:30.000000 deephaven-plugin-plotly-0.0.1.dev1/README.md
--rw-r--r--   0 vladbabich   (501) staff       (20)       98 2022-08-23 16:49:32.000000 deephaven-plugin-plotly-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 vladbabich   (501) staff       (20)     1160 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/setup.cfg
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/
--rw-r--r--   0 vladbabich   (501) staff       (20)      553 2022-08-25 18:00:57.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/__init__.py
--rw-r--r--   0 vladbabich   (501) staff       (20)      534 2022-08-23 17:23:18.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/figure_type.py
--rw-r--r--   0 vladbabich   (501) staff       (20)     3180 2022-08-25 17:11:10.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/theme_deephaven.py
-drwxr-xr-x   0 vladbabich   (501) staff       (20)        0 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/
--rw-r--r--   0 vladbabich   (501) staff       (20)     2425 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/PKG-INFO
--rw-r--r--   0 vladbabich   (501) staff       (20)      480 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 vladbabich   (501) staff       (20)        1 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 vladbabich   (501) staff       (20)       81 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/entry_points.txt
--rw-r--r--   0 vladbabich   (501) staff       (20)       59 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/requires.txt
--rw-r--r--   0 vladbabich   (501) staff       (20)       10 2022-08-25 18:02:53.000000 deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.921856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/figure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-26 15:21:05.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/theme_deephaven.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:21:17.925856 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:21:17.000000 deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/LICENSE` & `deephaven-plugin-plotly-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/PKG-INFO` & `deephaven-plugin-plotly-0.0.1.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Deephaven Plugin for Plotly
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly
 Author: Devin Smith, Vlad Babich
 Author-email: vladbabich@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly/issues
 Keywords: deephaven,plugin,plotly
@@ -63,20 +63,24 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin plotly
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
+
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/README.md` & `deephaven-plugin-plotly-0.0.1.dev2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -43,20 +43,24 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin plotly
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
+
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/setup.cfg` & `deephaven-plugin-plotly-0.0.1.dev2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 platforms = any
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
-	deephaven-core>=0.14.0
-	jpy>=0.11.0
 	deephaven-plugin
 	plotly
 include_package_data = True
 
 [options.packages.find]
 where = src
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/__init__.py` & `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from deephaven.plugin import Registration
 from plotly import io as pio
 
-__version__ = "0.0.1.dev1"
+__version__ = "0.0.1.dev2"
 
 def _init_theme():
     # Set the Deephaven style globally
     from . import theme_deephaven
     pio.templates.default = "deephaven"
     # Disable default renderer to ignore figure.show()
     pio.renderers.default = None
```

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/figure_type.py` & `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/figure_type.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/src/deephaven/plugin/plotly/theme_deephaven.py` & `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven/plugin/plotly/theme_deephaven.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-0.0.1.dev1/src/deephaven_plugin_plotly.egg-info/PKG-INFO` & `deephaven-plugin-plotly-0.0.1.dev2/src/deephaven_plugin_plotly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Deephaven Plugin for Plotly
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly
 Author: Devin Smith, Vlad Babich
 Author-email: vladbabich@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly/issues
 Keywords: deephaven,plugin,plotly
@@ -63,20 +63,24 @@
 ```
 
 ## Build
 
 To create your build / development environment:
 
 ```sh
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
 pip install --upgrade pip setuptools
 pip install build deephaven-plugin plotly
 ```
 
 To build:
 
 ```sh
 python -m build --wheel
 ```
 
-produces the wheel into `dist/`.
+The wheel is stored in `dist/`. 
+
+To test within [deephaven-core](https://github.com/deephaven/deephaven-core), note where this wheel is stored (using `pwd`, for example).
+Then, follow the directions in the [deephaven-js-plugins](https://github.com/deephaven/deephaven-js-plugins) repo.
+
```


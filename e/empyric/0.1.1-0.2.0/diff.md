# Comparing `tmp/empyric-0.1.1.tar.gz` & `tmp/empyric-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyric-0.1.1.tar", max compression
+gzip compressed data, was "empyric-0.2.0.tar", max compression
```

## Comparing `empyric-0.1.1.tar` & `empyric-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.1.1/LICENSE
--rw-r--r--   0        0        0     7233 2023-05-26 05:42:12.136305 empyric-0.1.1/README.md
--rw-r--r--   0        0        0     2260 2023-05-22 05:18:01.391399 empyric-0.1.1/empyric/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 05:42:12.136341 empyric-0.1.1/empyric/__main__.py
--rw-r--r--   0        0        0    39265 2023-05-17 05:28:01.619337 empyric-0.1.1/empyric/adapters.py
--rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.1.1/empyric/collection/__init__.py
--rw-r--r--   0        0        0     1711 2023-04-06 03:05:54.032558 empyric-0.1.1/empyric/collection/barometers.py
--rw-r--r--   0        0        0    11216 2023-05-17 04:53:19.432757 empyric-0.1.1/empyric/collection/controllers.py
--rw-r--r--   0        0        0     8578 2023-04-06 03:05:54.036020 empyric-0.1.1/empyric/collection/generators.py
--rw-r--r--   0        0        0     1212 2023-04-06 03:05:54.036470 empyric-0.1.1/empyric/collection/humans.py
--rw-r--r--   0        0        0     9460 2023-04-06 03:05:54.037384 empyric-0.1.1/empyric/collection/instrument.py
--rw-r--r--   0        0        0     3205 2023-04-06 03:05:54.038856 empyric-0.1.1/empyric/collection/io.py
--rw-r--r--   0        0        0    17409 2023-05-17 04:53:19.433598 empyric-0.1.1/empyric/collection/multimeters.py
--rw-r--r--   0        0        0    22050 2023-05-10 03:42:21.592096 empyric-0.1.1/empyric/collection/scopes.py
--rw-r--r--   0        0        0    28190 2023-04-14 06:00:29.449094 empyric-0.1.1/empyric/collection/sourcemeters.py
--rw-r--r--   0        0        0     3742 2023-04-06 03:05:54.041505 empyric-0.1.1/empyric/collection/spectrometers.py
--rw-r--r--   0        0        0     6851 2023-04-06 03:05:54.042207 empyric-0.1.1/empyric/collection/supplies.py
--rw-r--r--   0        0        0     2131 2023-04-06 03:05:54.042818 empyric-0.1.1/empyric/collection/thermometers.py
--rw-r--r--   0        0        0    10099 2023-04-06 03:05:54.044153 empyric-0.1.1/empyric/collection/virtual.py
--rw-r--r--   0        0        0    30149 2023-05-17 04:53:19.434369 empyric-0.1.1/empyric/experiment.py
--rw-r--r--   0        0        0    37572 2023-05-26 05:42:17.608271 empyric-0.1.1/empyric/graphics.py
--rw-r--r--   0        0        0      760 2023-04-21 03:37:51.903945 empyric-0.1.1/empyric/instruments.py
--rw-r--r--   0        0        0    32803 2023-05-26 05:42:17.608698 empyric-0.1.1/empyric/routines.py
--rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.1.1/empyric/runcard_schema.yaml
--rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.1.1/empyric/tests/__init__.py
--rw-r--r--   0        0        0     1420 2023-05-26 05:42:12.137905 empyric-0.1.1/empyric/tests/henon_runcard_example.yaml
--rw-r--r--   0        0        0      639 2022-10-24 21:12:17.723978 empyric-0.1.1/empyric/tests/test_adapter.py
--rw-r--r--   0        0        0     2123 2023-05-22 05:13:53.511443 empyric-0.1.1/empyric/tests/test_experiment.py
--rw-r--r--   0        0        0      637 2023-05-22 04:40:36.449679 empyric-0.1.1/empyric/tests/test_variable.py
--rw-r--r--   0        0        0     8006 2023-05-17 05:28:01.545894 empyric-0.1.1/empyric/tools.py
--rw-r--r--   0        0        0     6359 2023-05-26 05:42:12.138274 empyric-0.1.1/empyric/types.py
--rw-r--r--   0        0        0    16057 2023-05-17 04:53:19.436169 empyric-0.1.1/empyric/variables.py
--rw-r--r--   0        0        0      799 2023-05-26 05:45:51.692461 empyric-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8042 1970-01-01 00:00:00.000000 empyric-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7090 2023-05-26 05:49:13.218533 empyric-0.2.0/README.md
+-rw-r--r--   0        0        0     2260 2023-05-22 05:18:01.391399 empyric-0.2.0/empyric/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 05:42:12.136341 empyric-0.2.0/empyric/__main__.py
+-rw-r--r--   0        0        0    39265 2023-05-17 05:28:01.619337 empyric-0.2.0/empyric/adapters.py
+-rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.0/empyric/collection/__init__.py
+-rw-r--r--   0        0        0     1711 2023-04-06 03:05:54.032558 empyric-0.2.0/empyric/collection/barometers.py
+-rw-r--r--   0        0        0    11216 2023-05-17 04:53:19.432757 empyric-0.2.0/empyric/collection/controllers.py
+-rw-r--r--   0        0        0     8578 2023-04-06 03:05:54.036020 empyric-0.2.0/empyric/collection/generators.py
+-rw-r--r--   0        0        0     1212 2023-04-06 03:05:54.036470 empyric-0.2.0/empyric/collection/humans.py
+-rw-r--r--   0        0        0     9460 2023-04-06 03:05:54.037384 empyric-0.2.0/empyric/collection/instrument.py
+-rw-r--r--   0        0        0     3205 2023-04-06 03:05:54.038856 empyric-0.2.0/empyric/collection/io.py
+-rw-r--r--   0        0        0    17409 2023-05-17 04:53:19.433598 empyric-0.2.0/empyric/collection/multimeters.py
+-rw-r--r--   0        0        0    22050 2023-05-10 03:42:21.592096 empyric-0.2.0/empyric/collection/scopes.py
+-rw-r--r--   0        0        0    28190 2023-04-14 06:00:29.449094 empyric-0.2.0/empyric/collection/sourcemeters.py
+-rw-r--r--   0        0        0     3742 2023-04-06 03:05:54.041505 empyric-0.2.0/empyric/collection/spectrometers.py
+-rw-r--r--   0        0        0     6851 2023-04-06 03:05:54.042207 empyric-0.2.0/empyric/collection/supplies.py
+-rw-r--r--   0        0        0     2131 2023-04-06 03:05:54.042818 empyric-0.2.0/empyric/collection/thermometers.py
+-rw-r--r--   0        0        0    10099 2023-04-06 03:05:54.044153 empyric-0.2.0/empyric/collection/virtual.py
+-rw-r--r--   0        0        0    30149 2023-05-17 04:53:19.434369 empyric-0.2.0/empyric/experiment.py
+-rw-r--r--   0        0        0    37572 2023-05-26 05:42:17.608271 empyric-0.2.0/empyric/graphics.py
+-rw-r--r--   0        0        0      760 2023-04-21 03:37:51.903945 empyric-0.2.0/empyric/instruments.py
+-rw-r--r--   0        0        0    32803 2023-05-26 05:42:17.608698 empyric-0.2.0/empyric/routines.py
+-rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.0/empyric/runcard_schema.yaml
+-rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.0/empyric/tests/__init__.py
+-rw-r--r--   0        0        0     1420 2023-05-26 05:42:12.137905 empyric-0.2.0/empyric/tests/henon_runcard_example.yaml
+-rw-r--r--   0        0        0      639 2022-10-24 21:12:17.723978 empyric-0.2.0/empyric/tests/test_adapter.py
+-rw-r--r--   0        0        0     2123 2023-05-22 05:13:53.511443 empyric-0.2.0/empyric/tests/test_experiment.py
+-rw-r--r--   0        0        0      637 2023-05-22 04:40:36.449679 empyric-0.2.0/empyric/tests/test_variable.py
+-rw-r--r--   0        0        0     8006 2023-05-17 05:28:01.545894 empyric-0.2.0/empyric/tools.py
+-rw-r--r--   0        0        0     6359 2023-05-26 05:42:12.138274 empyric-0.2.0/empyric/types.py
+-rw-r--r--   0        0        0    16057 2023-05-17 04:53:19.436169 empyric-0.2.0/empyric/variables.py
+-rw-r--r--   0        0        0      799 2023-05-26 05:50:15.862611 empyric-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7899 1970-01-01 00:00:00.000000 empyric-0.2.0/PKG-INFO
```

### Comparing `empyric-0.1.1/LICENSE` & `empyric-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/README.md` & `empyric-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Empyric 
 ## A Python Library for Experiment Automation
 
 For more details, [read the docs](https://empyric.readthedocs.io/en/latest/).
 
 Empyric, at its most basic level, is an easy to use Python interface for communication with and controlling scientific instruments, such as digital multimeters, digital oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
 
-The Empyric package is managed with [poetry](https://python-poetry.org/). To install, execute the following in a console from within the cloned repository:
+The preferred method of installing Empyric is via pip:
 ```commandline
-pip install poetry  # if not already installed
-poetry install
+pip install empyric
 ```
 
 ### Instruments and Adapters
 
 Empyric contains a number of *instruments* with various associated methods of communication, such as serial or GPIB. For example, to remotely control a Keithley 2400 Sourcemeter from your PC, simply import the `Keithley2400` object from the library and instantiate it with its GPIB address:
 
 ```
```

### Comparing `empyric-0.1.1/empyric/__init__.py` & `empyric-0.2.0/empyric/__init__.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/adapters.py` & `empyric-0.2.0/empyric/adapters.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/barometers.py` & `empyric-0.2.0/empyric/collection/barometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/controllers.py` & `empyric-0.2.0/empyric/collection/controllers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/generators.py` & `empyric-0.2.0/empyric/collection/generators.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/humans.py` & `empyric-0.2.0/empyric/collection/humans.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/instrument.py` & `empyric-0.2.0/empyric/collection/instrument.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/io.py` & `empyric-0.2.0/empyric/collection/io.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/multimeters.py` & `empyric-0.2.0/empyric/collection/multimeters.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/scopes.py` & `empyric-0.2.0/empyric/collection/scopes.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/sourcemeters.py` & `empyric-0.2.0/empyric/collection/sourcemeters.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/spectrometers.py` & `empyric-0.2.0/empyric/collection/spectrometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/supplies.py` & `empyric-0.2.0/empyric/collection/supplies.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/thermometers.py` & `empyric-0.2.0/empyric/collection/thermometers.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/collection/virtual.py` & `empyric-0.2.0/empyric/collection/virtual.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/experiment.py` & `empyric-0.2.0/empyric/experiment.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/graphics.py` & `empyric-0.2.0/empyric/graphics.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/instruments.py` & `empyric-0.2.0/empyric/instruments.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/routines.py` & `empyric-0.2.0/empyric/routines.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/runcard_schema.yaml` & `empyric-0.2.0/empyric/runcard_schema.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/tests/henon_runcard_example.yaml` & `empyric-0.2.0/empyric/tests/henon_runcard_example.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/tests/test_adapter.py` & `empyric-0.2.0/empyric/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/tests/test_experiment.py` & `empyric-0.2.0/empyric/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/tests/test_variable.py` & `empyric-0.2.0/empyric/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/tools.py` & `empyric-0.2.0/empyric/tools.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/types.py` & `empyric-0.2.0/empyric/types.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/empyric/variables.py` & `empyric-0.2.0/empyric/variables.py`

 * *Files identical despite different names*

### Comparing `empyric-0.1.1/pyproject.toml` & `empyric-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empyric"
-version = "0.1.1"
+version = "0.2.0"
 description = "A package for experiment automation"
 authors = ["Daniel Merthe <dmerthe@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dmerthe/empyric"
 packages = [
     { include = "empyric"},
 ]
```

### Comparing `empyric-0.1.1/PKG-INFO` & `empyric-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyric
-Version: 0.1.1
+Version: 0.2.0
 Summary: A package for experiment automation
 Home-page: https://github.com/dmerthe/empyric
 Author: Daniel Merthe
 Author-email: dmerthe@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,18 +23,17 @@
 # Empyric 
 ## A Python Library for Experiment Automation
 
 For more details, [read the docs](https://empyric.readthedocs.io/en/latest/).
 
 Empyric, at its most basic level, is an easy to use Python interface for communication with and controlling scientific instruments, such as digital multimeters, digital oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
 
-The Empyric package is managed with [poetry](https://python-poetry.org/). To install, execute the following in a console from within the cloned repository:
+The preferred method of installing Empyric is via pip:
 ```commandline
-pip install poetry  # if not already installed
-poetry install
+pip install empyric
 ```
 
 ### Instruments and Adapters
 
 Empyric contains a number of *instruments* with various associated methods of communication, such as serial or GPIB. For example, to remotely control a Keithley 2400 Sourcemeter from your PC, simply import the `Keithley2400` object from the library and instantiate it with its GPIB address:
 
 ```
```


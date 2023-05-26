# Comparing `tmp/eodc_faas_force-2023.5.1rc2.tar.gz` & `tmp/eodc_faas_force-2023.5.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_force-2023.5.1rc2.tar", max compression
+gzip compressed data, was "eodc_faas_force-2023.5.1rc3.tar", max compression
```

## Comparing `eodc_faas_force-2023.5.1rc2.tar` & `eodc_faas_force-2023.5.1rc3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2023-05-04 07:03:46.202094 eodc_faas_force-2023.5.1rc2/README.md
--rw-r--r--   0        0        0       98 2023-05-26 09:50:29.797518 eodc_faas_force-2023.5.1rc2/force_processor_bindings/__init__.py
--rw-r--r--   0        0        0     1488 2023-05-16 12:33:42.141684 eodc_faas_force-2023.5.1rc2/force_processor_bindings/model.py
--rw-r--r--   0        0        0     4754 2023-05-23 08:20:37.440133 eodc_faas_force-2023.5.1rc2/force_processor_bindings/workflows.py
--rw-r--r--   0        0        0      679 2023-05-26 09:50:23.477519 eodc_faas_force-2023.5.1rc2/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 eodc_faas_force-2023.5.1rc2/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-04 07:19:47.659253 eodc_faas_force-2023.5.1rc3/README.md
+-rw-r--r--   0        0        0       98 2023-05-26 10:11:16.719253 eodc_faas_force-2023.5.1rc3/force_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     1488 2023-05-16 14:30:15.567253 eodc_faas_force-2023.5.1rc3/force_processor_bindings/model.py
+-rw-r--r--   0        0        0     4754 2023-05-23 08:18:00.179253 eodc_faas_force-2023.5.1rc3/force_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      679 2023-05-26 10:11:16.719253 eodc_faas_force-2023.5.1rc3/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 eodc_faas_force-2023.5.1rc3/PKG-INFO
```

### Comparing `eodc_faas_force-2023.5.1rc2/force_processor_bindings/model.py` & `eodc_faas_force-2023.5.1rc3/force_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_force-2023.5.1rc2/force_processor_bindings/workflows.py` & `eodc_faas_force-2023.5.1rc3/force_processor_bindings/workflows.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_force-2023.5.1rc2/pyproject.toml` & `eodc_faas_force-2023.5.1rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-force"
-version = "2023.5.1-rc.2"
+version = "2023.5.1-rc.3"
 description = "Bindings for the FORCE processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "force_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_force-2023.5.1rc2/PKG-INFO` & `eodc_faas_force-2023.5.1rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-force
-Version: 2023.5.1rc2
+Version: 2023.5.1rc3
 Summary: Bindings for the FORCE processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


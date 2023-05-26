# Comparing `tmp/yt_idefix-2.0.1.tar.gz` & `tmp/yt_idefix-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.0.1.tar", last modified: Tue May 23 10:05:25 2023, max compression
+gzip compressed data, was "yt_idefix-2.0.2.tar", last modified: Fri May 26 16:31:28 2023, max compression
```

## Comparing `yt_idefix-2.0.1.tar` & `yt_idefix-2.0.2.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-23 10:05:15.000000 yt_idefix-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/tests/test_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35099 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:16.000000 yt_idefix-2.0.1/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:25.445487 yt_idefix-2.0.1/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 10:05:25.000000 yt_idefix-2.0.1/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-26 16:31:18.000000 yt_idefix-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34970 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:19.000000 yt_idefix-2.0.2/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:31:28.329536 yt_idefix-2.0.2/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 16:31:28.000000 yt_idefix-2.0.2/yt_idefix.egg-info/top_level.txt
```

### Comparing `yt_idefix-2.0.1/LICENSE` & `yt_idefix-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/PKG-INFO` & `yt_idefix-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.0.1/README.md` & `yt_idefix-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/pyproject.toml` & `yt_idefix-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_idefix"
-version = "2.0.1"
+version = "2.0.2"
 description = "An extension module for yt, adding a frontend for Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `yt_idefix-2.0.1/tests/test_C_io.py` & `yt_idefix-2.0.2/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/tests/test_dmp.py` & `yt_idefix-2.0.2/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/tests/test_loading.py` & `yt_idefix-2.0.2/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/tests/test_vtk.py` & `yt_idefix-2.0.2/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/tests/test_xdmf.py` & `yt_idefix-2.0.2/tests/test_xdmf.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/_backports.py` & `yt_idefix-2.0.2/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/_io/commons.py` & `yt_idefix-2.0.2/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.0.2/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/_io/h5_io.py` & `yt_idefix-2.0.2/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.0.2/yt_idefix/_io/vtk_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/data_structures.py` & `yt_idefix-2.0.2/yt_idefix/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Final, Literal
 
 import inifix
 import numpy as np
 import numpy.testing as npt
 
+import yt
 from yt.data_objects.index_subobjects.stretched_grid import StretchedGrid
 from yt.data_objects.static_output import Dataset
 from yt.funcs import setdefaultattr
 from yt.geometry.grid_geometry_handler import GridIndex
 from yt.utilities.lib.misc_utilities import (  # type: ignore [import]
     _obtain_coords_and_widths,
 )
 from yt.utilities.on_demand_imports import _h5py as h5py
 from yt_idefix._backports import removesuffix
-from yt_idefix._typing import UnitLike
 
 from ._io import C_io, dmp_io, h5_io, vtk_io
 from ._io.commons import IdefixFieldProperties, IdefixMetadata
 from .definitions import _PlutoBaseUnits, pluto_def_constants
 from .fields import (
     IdefixDmpFields,
     IdefixVtkFields,
@@ -315,15 +315,15 @@
     _version_regexp: re.Pattern
 
     def __init__(
         self,
         filename,
         *,
         dataset_type: str | None = None,  # deleguated to child classes
-        units_override: dict[str, UnitLike] | None = None,
+        units_override: dict[str, str] | None = None,
         unit_system: Literal["cgs", "mks", "code"] = "cgs",
         default_species_fields: Literal["neutral", "ionized"] | None = None,
         # from here, frontend-specific arguments
         geometry: Literal["cartesian", "spherical", "cylindrical", "polar"]
         | None = None,
         inifile: str | os.PathLike[str] | None = None,
         definitions_header: str | os.PathLike[str] | None = None,
@@ -420,25 +420,20 @@
                 )
             geom_str = from_input
         else:
             assert from_disk
             geom_str = from_disk
 
         def parse_geometry(geom: str):
-            import yt
+            if yt.version_info >= (4, 2):
+                from yt.geometry.api import Geometry  # type: ignore [attr-defined]
 
-            if yt.version_info[:2] > (4, 1):
-                try:
-                    from yt.geometry.api import Geometry  # type: ignore [attr-defined]
-
-                    return Geometry(geom)
-                except ImportError:
-                    pass
-
-            return geom
+                return Geometry(geom)
+            else:
+                return geom
 
         self.geometry = parse_geometry(geom_str)
 
     def _parse_inifile(self) -> None:
         if not self._inifile:
             return
```

### Comparing `yt_idefix-2.0.1/yt_idefix/definitions.py` & `yt_idefix-2.0.2/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/fields.py` & `yt_idefix-2.0.2/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix/io.py` & `yt_idefix-2.0.2/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.0.1/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.0.2/yt_idefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.0.1/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.0.2/yt_idefix.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 tests/test_C_io.py
 tests/test_dmp.py
 tests/test_loading.py
 tests/test_vtk.py
 tests/test_xdmf.py
 yt_idefix/__init__.py
 yt_idefix/_backports.py
-yt_idefix/_typing.py
 yt_idefix/api.py
 yt_idefix/data_structures.py
 yt_idefix/definitions.py
 yt_idefix/fields.py
 yt_idefix/io.py
 yt_idefix/misc.py
 yt_idefix/py.typed
```


# Comparing `tmp/dicommeta-0.6.6.tar.gz` & `tmp/dicommeta-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicommeta-0.6.6.tar", max compression
+gzip compressed data, was "dicommeta-0.6.7.tar", max compression
```

## Comparing `dicommeta-0.6.6.tar` & `dicommeta-0.6.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       57 2023-05-22 22:52:50.650896 dicommeta-0.6.6/CHANGELOG.md
--rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.6/LICENSE
--rw-r--r--   0        0        0     2666 2023-05-23 15:47:43.845985 dicommeta-0.6.6/README.md
--rw-r--r--   0        0        0      673 2023-05-24 01:01:34.199258 dicommeta-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     3673 2023-05-23 11:56:02.053987 dicommeta-0.6.6/src/dicommeta/Struct.py
--rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.6/src/dicommeta/Utils.py
--rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.6/src/dicommeta/__init__.py
--rw-r--r--   0        0        0     3341 1970-01-01 00:00:00.000000 dicommeta-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-05-22 22:52:50.650896 dicommeta-0.6.7/CHANGELOG.md
+-rw-r--r--   0        0        0    11356 2023-05-09 13:28:51.971341 dicommeta-0.6.7/LICENSE
+-rw-r--r--   0        0        0     2666 2023-05-23 15:47:43.845985 dicommeta-0.6.7/README.md
+-rw-r--r--   0        0        0      673 2023-05-25 22:18:53.124312 dicommeta-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     3774 2023-05-24 11:52:28.617457 dicommeta-0.6.7/src/dicommeta/Struct.py
+-rw-r--r--   0        0        0     2342 2023-05-23 11:49:03.746665 dicommeta-0.6.7/src/dicommeta/Utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:10:29.709188 dicommeta-0.6.7/src/dicommeta/__init__.py
+-rw-r--r--   0        0        0     3341 1970-01-01 00:00:00.000000 dicommeta-0.6.7/PKG-INFO
```

### Comparing `dicommeta-0.6.6/LICENSE` & `dicommeta-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.6/README.md` & `dicommeta-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.6/pyproject.toml` & `dicommeta-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dicommeta"
-version = "0.6.6"
+version = "0.6.7"
 description = "Dicom Metadata structures"
 authors = ["Kevin Long <longke@pennmedicine.upenn.edu>",]
 maintainers = ["Kevin Long <longke@pennmedicine.upenn.edu>",]
 repository = "https://dev.azure.com/longke/Radiology/_git/DicomMeta"
 readme = "README.md"
 include = ["CHANGELOG.md"]
 packages = [
```

### Comparing `dicommeta-0.6.6/src/dicommeta/Struct.py` & `dicommeta-0.6.7/src/dicommeta/Struct.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from datetime import datetime
 from typing import Optional, Union, List, Dict, Iterable
 
 from attr import define, field
 from attrs import validators, asdict
 
-from dicommeta.Utils import validator_pass, validator_parsable_date, validator_parsable_time, Mode, calculate_age
+from dicommeta.Utils import validator_pass, validator_parsable_date, \
+    validator_parsable_time, Mode, calculate_age
 
 
 @define(kw_only=True, slots=True, order=True, frozen=True)
 class Instance:
     SOPinstanceUID: str = field(factory=str)
 
 
 @define(kw_only=True, slots=True, order=True, frozen=True)
 class Series:
     seriesUID: str = field(factory=str)
     instance_dict: Dict[str, Instance] = field(factory=dict)
 
-    def add_instance(self, instance: Instance):
+    def add_instance(self, instance: Instance) -> bool:
         if instance.SOPinstanceUID not in self.instance_dict.keys():
             self.instance_dict[instance.SOPinstanceUID] = instance
+            return True
+        else:
+            return False
 
     def get_instance(self, instance_uid: Instance) -> Instance:
-        return self.instance_dict[instance_uid]
+        return self.instance_dict[instance_uid.SOPinstanceUID]
 
-    def get_dict(self):
+    def as_dict(self) -> dict:
         return asdict(self)
 
-    def get_iter(self) -> Iterable:
-        return iter(asdict(self))
+    def iter(self) -> Iterable:
+        return iter(self.as_dict(self))
 
 
 @define(kw_only=True, slots=True, order=True, frozen=False)
 class Study(dict):
     StudyUID: str = field(factory=str, validator=validator_pass)
     StudyInstanceUID: str = field(factory=str)
     SpecificCharacterSet: str = field(factory=str, validator=validator_pass)
```

### Comparing `dicommeta-0.6.6/src/dicommeta/Utils.py` & `dicommeta-0.6.7/src/dicommeta/Utils.py`

 * *Files identical despite different names*

### Comparing `dicommeta-0.6.6/PKG-INFO` & `dicommeta-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicommeta
-Version: 0.6.6
+Version: 0.6.7
 Summary: Dicom Metadata structures
 Home-page: https://dev.azure.com/longke/Radiology/_git/DicomMeta
 Author: Kevin Long
 Author-email: longke@pennmedicine.upenn.edu
 Maintainer: Kevin Long
 Maintainer-email: longke@pennmedicine.upenn.edu
 Requires-Python: >=3.10,<4.0
```


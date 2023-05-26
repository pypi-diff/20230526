# Comparing `tmp/to_cei-0.2.0.tar.gz` & `tmp/to_cei-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to_cei-0.2.0.tar", last modified: Thu May 25 12:13:21 2023, max compression
+gzip compressed data, was "to_cei-0.2.1.tar", last modified: Fri May 26 06:46:09 2023, max compression
```

## Comparing `to_cei-0.2.0.tar` & `to_cei-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-25 12:13:21.642747 to_cei-0.2.0/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35149 2023-03-15 11:24:38.000000 to_cei-0.2.0/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)      889 2023-05-25 12:13:21.642747 to_cei-0.2.0/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      329 2023-03-15 11:24:38.000000 to_cei-0.2.0/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-25 12:13:21.642747 to_cei-0.2.0/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1012 2023-05-25 12:11:26.000000 to_cei-0.2.0/setup.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-25 12:13:21.642747 to_cei-0.2.0/test/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    52397 2023-05-25 12:11:13.000000 to_cei-0.2.0/test/test_charter.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1139 2023-03-15 11:24:38.000000 to_cei-0.2.0/test/test_charter_group.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      699 2023-03-15 11:24:38.000000 to_cei-0.2.0/test/test_helpers.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2989 2023-03-15 11:24:38.000000 to_cei-0.2.0/test/test_seal.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      287 2023-03-15 11:24:38.000000 to_cei-0.2.0/test/test_validator.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-25 12:13:21.642747 to_cei-0.2.0/to_cei/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    42892 2023-05-25 12:08:30.000000 to_cei-0.2.0/to_cei/charter.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2425 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/charter_group.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      594 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/config.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      815 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/filecache.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2114 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/helpers.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3886 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/seal.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      570 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/validator.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1854 2023-03-15 11:24:38.000000 to_cei-0.2.0/to_cei/xml_assembler.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-25 12:13:21.642747 to_cei-0.2.0/to_cei.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      889 2023-05-25 12:13:21.000000 to_cei-0.2.0/to_cei.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      441 2023-05-25 12:13:21.000000 to_cei-0.2.0/to_cei.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-25 12:13:21.000000 to_cei-0.2.0/to_cei.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       32 2023-05-25 12:13:21.000000 to_cei-0.2.0/to_cei.egg-info/requires.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        7 2023-05-25 12:13:21.000000 to_cei-0.2.0/to_cei.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-26 06:46:09.853578 to_cei-0.2.1/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35149 2023-03-15 11:24:38.000000 to_cei-0.2.1/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      889 2023-05-26 06:46:09.853578 to_cei-0.2.1/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      329 2023-03-15 11:24:38.000000 to_cei-0.2.1/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-05-26 06:46:09.853578 to_cei-0.2.1/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1012 2023-05-26 06:38:45.000000 to_cei-0.2.1/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-26 06:46:09.843577 to_cei-0.2.1/test/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    52873 2023-05-26 06:38:17.000000 to_cei-0.2.1/test/test_charter.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1139 2023-03-15 11:24:38.000000 to_cei-0.2.1/test/test_charter_group.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      699 2023-03-15 11:24:38.000000 to_cei-0.2.1/test/test_helpers.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2989 2023-03-15 11:24:38.000000 to_cei-0.2.1/test/test_seal.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      287 2023-03-15 11:24:38.000000 to_cei-0.2.1/test/test_validator.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-26 06:46:09.853578 to_cei-0.2.1/to_cei/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    43522 2023-05-26 06:42:40.000000 to_cei-0.2.1/to_cei/charter.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2425 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/charter_group.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      594 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/config.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      815 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/filecache.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2114 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/helpers.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3886 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/seal.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      570 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/validator.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1854 2023-03-15 11:24:38.000000 to_cei-0.2.1/to_cei/xml_assembler.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-26 06:46:09.853578 to_cei-0.2.1/to_cei.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      889 2023-05-26 06:46:09.000000 to_cei-0.2.1/to_cei.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      441 2023-05-26 06:46:09.000000 to_cei-0.2.1/to_cei.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-26 06:46:09.000000 to_cei-0.2.1/to_cei.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       32 2023-05-26 06:46:09.000000 to_cei-0.2.1/to_cei.egg-info/requires.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        7 2023-05-26 06:46:09.000000 to_cei-0.2.1/to_cei.egg-info/top_level.txt
```

### Comparing `to_cei-0.2.0/LICENSE` & `to_cei-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/PKG-INFO` & `to_cei-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to_cei
-Version: 0.2.0
+Version: 0.2.1
 Summary: to-CEI
 Home-page: https://github.com/icaruseu/to-cei
 Author: Daniel Jeller
 Author-email: it@icar-us.eu
 License: GPL 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `to_cei-0.2.0/setup.py` & `to_cei-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path.join(pwd, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="to_cei",
-    version="0.2.0",
+    version="0.2.1",
     description="to-CEI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/icaruseu/to-cei",
     author="Daniel Jeller",
     author_email="it@icar-us.eu",
     license="GPL 3.0",
```

### Comparing `to_cei-0.2.0/test/test_charter.py` & `to_cei-0.2.1/test/test_charter.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,14 +967,26 @@
     charter = Charter(id_text="1", abstract=abstract, issuers=issuer)
     assert isinstance(charter.issuers, str)
     assert charter.issuers == issuer
     issuer_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:abstract/cei:issuer")
     assert issuer_xml.text == issuer
 
 
+def test_has_correct_abstract_with_text_single_issuer():
+    abstract = (
+        "Konrad von Lintz, Caplan zu St. Pankraz, beurkundet den vorstehenden Vertrag."
+    )
+    issuer = "Konrad von Lintz"
+    charter = Charter(id_text="1", abstract=abstract, issuer=issuer)
+    assert isinstance(charter.issuers, str)
+    assert charter.issuers == issuer
+    issuer_xml = xps(charter, "/cei:text/cei:body/cei:chDesc/cei:abstract/cei:issuer")
+    assert issuer_xml.text == issuer
+
+
 def test_has_correct_abstract_with_text_list_issuer():
     abstract = (
         "Konrad von Lintz und Thomas von Gmunden, beurkunden den vorstehenden Vertrag."
     )
     issuers = ["Konrad von Lintz", "Thomas von Gmunden"]
     charter = Charter(id_text="1", abstract=abstract, issuers=issuers)
     assert isinstance(charter.issuers, List)
```

### Comparing `to_cei-0.2.0/test/test_charter_group.py` & `to_cei-0.2.1/test/test_charter_group.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/test/test_helpers.py` & `to_cei-0.2.1/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/test/test_seal.py` & `to_cei-0.2.1/test/test_seal.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/charter.py` & `to_cei-0.2.1/to_cei/charter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import calendar
 import re
+import warnings
 from datetime import datetime
 from typing import List, Optional, Tuple
 from urllib.parse import quote
 
 from astropy.time import Time
 from lxml import etree
 
@@ -224,14 +225,15 @@
         id_old: Optional[str] = None,
         index: Optional[List[str | etree._Element]] = [],
         index_geo_features: Optional[List[str | etree._Element]] = [],
         index_organizations: Optional[List[str | etree._Element]] = [],
         index_persons: Optional[List[str | etree._Element]] = [],
         index_places: Optional[List[str | etree._Element]] = [],
         issued_place: Optional[str | etree._Element] = None,
+        issuer: Optional[str | etree._Element] = None,
         issuers: Optional[
             str | etree._Element | List[str] | List[etree._Element]
         ] = None,
         language: Optional[str] = None,
         literature: Optional[str | List[str]] = [],
         literature_abstracts: Optional[str | List[str]] = [],
         literature_depictions: Optional[str | List[str]] = [],
@@ -268,14 +270,15 @@
             id_old: An old, now obsolete identifier of the charter.
             index: A list of terms as texts or cei:index etree._Element objects to be included in the index.
             index_geo_features: A list of geographical features as texts or cei:geogName etree._Element objects to be included in the index.
             index_organizations: A list of organizations as texts or cei:orgName etree._Element objects to be included in the index.
             index_persons: A list of persons as texts or cei:persName etree._Element objects to be included in the index.
             index_places: A list of places as texts or cei:placeName etree._Element objects to be included in the index.
             issued_place: The place the charter has been issued at either as text or a complete cei:placeName etree._Element.
+            issuer: The charters single issuer either as a text or a etree._Element object. DEPRECATED - This parameter will be removed in future versions, please use the 'issuers' parameter, it accepts the same values as well as lists.
             issuers: The charters' issuers, as either a single or list of texts or complete cei:issuer etree._Element objects.
             language: The language of the charter as text.
             literature: A single text or list of texts descibing unspecified literature for the charter.
             literature_abstracts: A single text or list of texts descibing abstracts of the charter.
             literature_depictions: A single text or list of texts descibing depictions of the charter.
             literature_editions: A single text or list of texts descibing editions of the charter.
             literature_secondary: A single text or list of texts descibing secondary literature about the charter.
@@ -313,14 +316,19 @@
         self.index = index
         self.index_geo_features = index_geo_features
         self.index_organizations = index_organizations
         self.index_persons = index_persons
         self.index_places = index_places
         self.issued_place = issued_place
         self.issuers = issuers
+        if issuer is not None:
+            warnings.warn(
+                "The 'issuer' parameter is deprecated in favor of 'issuers' which can take the same value but supports multiple issuers. Setting issuer will erase values set with issuers for legacy support reasons."
+            )
+            self.issuers = issuer
         self.language = language
         self.literature = literature
         self.literature_abstracts = literature_abstracts
         self.literature_depictions = literature_depictions
         self.literature_editions = literature_editions
         self.literature_secondary = literature_secondary
         self.material = material
```

### Comparing `to_cei-0.2.0/to_cei/charter_group.py` & `to_cei-0.2.1/to_cei/charter_group.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/config.py` & `to_cei-0.2.1/to_cei/config.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/filecache.py` & `to_cei-0.2.1/to_cei/filecache.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/helpers.py` & `to_cei-0.2.1/to_cei/helpers.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/seal.py` & `to_cei-0.2.1/to_cei/seal.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/validator.py` & `to_cei-0.2.1/to_cei/validator.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei/xml_assembler.py` & `to_cei-0.2.1/to_cei/xml_assembler.py`

 * *Files identical despite different names*

### Comparing `to_cei-0.2.0/to_cei.egg-info/PKG-INFO` & `to_cei-0.2.1/to_cei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cei
-Version: 0.2.0
+Version: 0.2.1
 Summary: to-CEI
 Home-page: https://github.com/icaruseu/to-cei
 Author: Daniel Jeller
 Author-email: it@icar-us.eu
 License: GPL 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```


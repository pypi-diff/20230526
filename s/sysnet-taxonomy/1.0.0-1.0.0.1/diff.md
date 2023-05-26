# Comparing `tmp/sysnet-taxonomy-1.0.0.tar.gz` & `tmp/sysnet-taxonomy-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-taxonomy-1.0.0.tar", last modified: Tue May 23 18:01:15 2023, max compression
+gzip compressed data, was "sysnet-taxonomy-1.0.0.1.tar", last modified: Fri May 26 15:46:46 2023, max compression
```

## Comparing `sysnet-taxonomy-1.0.0.tar` & `sysnet-taxonomy-1.0.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.850907 sysnet-taxonomy-1.0.0/
--rw-rw-rw-   0        0        0     5108 2023-05-23 18:01:15.849912 sysnet-taxonomy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4380 2023-05-23 17:57:56.000000 sysnet-taxonomy-1.0.0/README.md
--rw-rw-rw-   0        0        0      673 2023-05-23 17:55:57.000000 sysnet-taxonomy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 18:01:15.850907 sysnet-taxonomy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.806337 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/
--rw-rw-rw-   0        0        0     5108 2023-05-23 18:01:15.000000 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2023-05-23 18:01:15.000000 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 18:01:15.000000 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-23 18:01:15.000000 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 18:01:15.000000 sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.814336 sysnet-taxonomy-1.0.0/taxonomy/
--rw-rw-rw-   0        0        0      843 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.821390 sysnet-taxonomy-1.0.0/taxonomy/api/
--rw-rw-rw-   0        0        0      233 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/api/__init__.py
--rw-rw-rw-   0        0        0    11402 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/api/admins_api.py
--rw-rw-rw-   0        0        0     6827 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/api/developers_api.py
--rw-rw-rw-   0        0        0     8471 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/api/public_api.py
--rw-rw-rw-   0        0        0    25013 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/api_client.py
--rw-rw-rw-   0        0        0     8218 2023-05-23 17:54:02.000000 sysnet-taxonomy-1.0.0/taxonomy/configuration.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.830909 sysnet-taxonomy-1.0.0/taxonomy/models/
--rw-rw-rw-   0        0        0      557 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/models/__init__.py
--rw-rw-rw-   0        0        0     4522 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/models/hybrid_type.py
--rw-rw-rw-   0        0        0     6778 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/models/taxon_entry_list_type.py
--rw-rw-rw-   0        0        0     8155 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/models/taxon_entry_type.py
--rw-rw-rw-   0        0        0    25700 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/models/taxon_type.py
--rw-rw-rw-   0        0        0    12989 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/taxonomy/rest.py
-drwxrwxrwx   0        0        0        0 2023-05-23 18:01:15.846908 sysnet-taxonomy-1.0.0/test/
--rw-rw-rw-   0        0        0       15 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_admins_api.py
--rw-rw-rw-   0        0        0      962 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_developers_api.py
--rw-rw-rw-   0        0        0      844 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_hybrid_type.py
--rw-rw-rw-   0        0        0      951 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_public_api.py
--rw-rw-rw-   0        0        0      912 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_taxon_entry_list_type.py
--rw-rw-rw-   0        0        0      878 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_taxon_entry_type.py
--rw-rw-rw-   0        0        0      836 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0/test/test_taxon_type.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.182007 sysnet-taxonomy-1.0.0.1/
+-rw-rw-rw-   0        0        0     5149 2023-05-26 15:46:46.182007 sysnet-taxonomy-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4419 2023-05-26 15:44:39.000000 sysnet-taxonomy-1.0.0.1/README.md
+-rw-rw-rw-   0        0        0      677 2023-05-26 15:45:45.000000 sysnet-taxonomy-1.0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:46:46.182007 sysnet-taxonomy-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.134716 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/
+-rw-rw-rw-   0        0        0     5149 2023-05-26 15:46:46.000000 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2023-05-26 15:46:46.000000 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:46:46.000000 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-26 15:46:46.000000 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 15:46:46.000000 sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.134716 sysnet-taxonomy-1.0.0.1/taxonomy/
+-rw-rw-rw-   0        0        0      843 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.150348 sysnet-taxonomy-1.0.0.1/taxonomy/api/
+-rw-rw-rw-   0        0        0      233 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/api/__init__.py
+-rw-rw-rw-   0        0        0    11402 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/api/admins_api.py
+-rw-rw-rw-   0        0        0     6827 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/api/developers_api.py
+-rw-rw-rw-   0        0        0     8471 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/api/public_api.py
+-rw-rw-rw-   0        0        0    25013 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/api_client.py
+-rw-rw-rw-   0        0        0     8218 2023-05-26 15:44:39.000000 sysnet-taxonomy-1.0.0.1/taxonomy/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.162359 sysnet-taxonomy-1.0.0.1/taxonomy/models/
+-rw-rw-rw-   0        0        0      557 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/models/__init__.py
+-rw-rw-rw-   0        0        0     4522 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/models/hybrid_type.py
+-rw-rw-rw-   0        0        0     6778 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_entry_list_type.py
+-rw-rw-rw-   0        0        0     8366 2023-05-25 16:18:23.000000 sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_entry_type.py
+-rw-rw-rw-   0        0        0    21454 2023-05-25 16:18:23.000000 sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_type.py
+-rw-rw-rw-   0        0        0    12989 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/taxonomy/rest.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:46:46.166368 sysnet-taxonomy-1.0.0.1/test/
+-rw-rw-rw-   0        0        0       15 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_admins_api.py
+-rw-rw-rw-   0        0        0      962 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_developers_api.py
+-rw-rw-rw-   0        0        0      844 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_hybrid_type.py
+-rw-rw-rw-   0        0        0      951 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_public_api.py
+-rw-rw-rw-   0        0        0      912 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_taxon_entry_list_type.py
+-rw-rw-rw-   0        0        0      878 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_taxon_entry_type.py
+-rw-rw-rw-   0        0        0      836 2023-05-23 17:47:16.000000 sysnet-taxonomy-1.0.0.1/test/test_taxon_type.py
```

### Comparing `sysnet-taxonomy-1.0.0/PKG-INFO` & `sysnet-taxonomy-1.0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-taxonomy
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: SYSNET CITES Taxonomy REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/swagger/tree/main/clients/taxonomy
 Keywords: Swagger,API pro taxonomii CITES
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,18 +25,18 @@
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on PyPi
+If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy 
+pip install sysnet-taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
```

### Comparing `sysnet-taxonomy-1.0.0/README.md` & `sysnet-taxonomy-1.0.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on PyPi
+If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy 
+pip install sysnet-taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
```

### Comparing `sysnet-taxonomy-1.0.0/pyproject.toml` & `sysnet-taxonomy-1.0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-taxonomy"
-version = "1.0.0"
+version = "1.0.0.001"
 authors = [
   { name="Radim Jaeger", email="rjaeger@sysnet.cz" },
 ]
 description = "SYSNET CITES Taxonomy REST API client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-taxonomy-1.0.0/setup.py` & `sysnet-taxonomy-1.0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/PKG-INFO` & `sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-taxonomy
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: SYSNET CITES Taxonomy REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 Project-URL: Homepage, https://github.com/SYSNET-CZ/swagger/tree/main/clients/taxonomy
 Keywords: Swagger,API pro taxonomii CITES
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,18 +25,18 @@
 ## Requirements.
 
 Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
-If the python package is hosted on PyPi
+If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install sysnet-taxonomy 
+pip install sysnet-taxonomy
 ```
 
 Then import the package:
 ```python
 import taxonomy 
 ```
```

### Comparing `sysnet-taxonomy-1.0.0/sysnet_taxonomy.egg-info/SOURCES.txt` & `sysnet-taxonomy-1.0.0.1/sysnet_taxonomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/__init__.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/api/admins_api.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/api/admins_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/api/developers_api.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/api/developers_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/api/public_api.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/api/public_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/api_client.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/api_client.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/configuration.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/configuration.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/models/__init__.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/models/hybrid_type.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/models/hybrid_type.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/models/taxon_entry_list_type.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_entry_list_type.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/models/taxon_entry_type.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_entry_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         self.discriminator = None
         if pid is not None:
             self.pid = pid
         if name_common_cz is not None:
             self.name_common_cz = name_common_cz
         if name_common_en is not None:
             self.name_common_en = name_common_en
-        if name_scientific is not None:
-            self.name_scientific = name_scientific
+        self.name_scientific = name_scientific
         if regulation_cites is not None:
             self.regulation_cites = regulation_cites
         if regulation_eu is not None:
             self.regulation_eu = regulation_eu
 
     @property
     def pid(self):
@@ -152,14 +151,16 @@
         """Sets the name_scientific of this TaxonEntryType.
 
         Vědecký název (latinsky)  # noqa: E501
 
         :param name_scientific: The name_scientific of this TaxonEntryType.  # noqa: E501
         :type: str
         """
+        if name_scientific is None:
+            raise ValueError("Invalid value for `name_scientific`, must not be `None`")  # noqa: E501
 
         self._name_scientific = name_scientific
 
     @property
     def regulation_cites(self):
         """Gets the regulation_cites of this TaxonEntryType.  # noqa: E501
 
@@ -175,15 +176,15 @@
         """Sets the regulation_cites of this TaxonEntryType.
 
         Exemplář sledovaný podle CITES  # noqa: E501
 
         :param regulation_cites: The regulation_cites of this TaxonEntryType.  # noqa: E501
         :type: str
         """
-        allowed_values = ["I", "II", "III"]  # noqa: E501
+        allowed_values = ["I", "I/II", "II", "II/III", "III", "NC", "Not CITES. Protected by the Act 114/1992.", "Not CITES", "", ""]  # noqa: E501
         if regulation_cites not in allowed_values:
             raise ValueError(
                 "Invalid value for `regulation_cites` ({0}), must be one of {1}"  # noqa: E501
                 .format(regulation_cites, allowed_values)
             )
 
         self._regulation_cites = regulation_cites
@@ -204,15 +205,15 @@
         """Sets the regulation_eu of this TaxonEntryType.
 
         Exemplář sledovaný podle EU  # noqa: E501
 
         :param regulation_eu: The regulation_eu of this TaxonEntryType.  # noqa: E501
         :type: str
         """
-        allowed_values = ["A", "B", "C"]  # noqa: E501
+        allowed_values = ["A", "A/B", "B", "B/D", "C", "D", "", ""]  # noqa: E501
         if regulation_eu not in allowed_values:
             raise ValueError(
                 "Invalid value for `regulation_eu` ({0}), must be one of {1}"  # noqa: E501
                 .format(regulation_eu, allowed_values)
             )
 
         self._regulation_eu = regulation_eu
```

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/models/taxon_type.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/models/taxon_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,64 +10,57 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
+from taxonomy.models.taxon_entry_type import TaxonEntryType  # noqa: F401,E501
 
-class TaxonType(object):
+class TaxonType(TaxonEntryType):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id_species_plus': 'list[str]',
-        'pid': 'str',
-        'name_common_cz': 'str',
-        'name_common_en': 'str',
-        'name_scientific': 'str',
         'name_listed': 'str',
         'rank_regnum': 'str',
         'rank_phylum': 'str',
         'rank_divisio': 'str',
         'rank_classis': 'str',
         'rank_ordo': 'str',
         'rank_familia': 'str',
         'rank_genus': 'str',
         'rank_species': 'str',
         'rank_subspecies': 'str',
         'rank_hybrid': 'str',
         'regulation_102': 'bool',
-        'regulation_114': 'bool',
+        'regulation_114': 'str',
         'regulation_411': 'bool',
-        'regulation_449': 'bool',
+        'regulation_449': 'str',
         'regulation_95': 'bool',
-        'regulation_cites': 'str',
-        'regulation_eu': 'str',
         'synonyms': 'list[str]',
         'is_valid': 'bool',
         'is_published': 'bool',
         'is_deleted': 'bool',
         'hybrid': 'HybridType'
     }
+    if hasattr(TaxonEntryType, "swagger_types"):
+        swagger_types.update(TaxonEntryType.swagger_types)
 
     attribute_map = {
         'id_species_plus': 'id_species_plus',
-        'pid': 'pid',
-        'name_common_cz': 'name_common_cz',
-        'name_common_en': 'name_common_en',
-        'name_scientific': 'name_scientific',
         'name_listed': 'name_listed',
         'rank_regnum': 'rank_regnum',
         'rank_phylum': 'rank_phylum',
         'rank_divisio': 'rank_divisio',
         'rank_classis': 'rank_classis',
         'rank_ordo': 'rank_ordo',
         'rank_familia': 'rank_familia',
@@ -76,30 +69,26 @@
         'rank_subspecies': 'rank_subspecies',
         'rank_hybrid': 'rank_hybrid',
         'regulation_102': 'regulation_102',
         'regulation_114': 'regulation_114',
         'regulation_411': 'regulation_411',
         'regulation_449': 'regulation_449',
         'regulation_95': 'regulation_95',
-        'regulation_cites': 'regulation_cites',
-        'regulation_eu': 'regulation_eu',
         'synonyms': 'synonyms',
         'is_valid': 'is_valid',
         'is_published': 'is_published',
         'is_deleted': 'is_deleted',
         'hybrid': 'hybrid'
     }
+    if hasattr(TaxonEntryType, "attribute_map"):
+        attribute_map.update(TaxonEntryType.attribute_map)
 
-    def __init__(self, id_species_plus=None, pid=None, name_common_cz=None, name_common_en=None, name_scientific=None, name_listed=None, rank_regnum=None, rank_phylum=None, rank_divisio=None, rank_classis=None, rank_ordo=None, rank_familia=None, rank_genus=None, rank_species=None, rank_subspecies=None, rank_hybrid=None, regulation_102=None, regulation_114=None, regulation_411=None, regulation_449=None, regulation_95=None, regulation_cites=None, regulation_eu=None, synonyms=None, is_valid=None, is_published=None, is_deleted=None, hybrid=None):  # noqa: E501
+    def __init__(self, id_species_plus=None, name_listed=None, rank_regnum=None, rank_phylum=None, rank_divisio=None, rank_classis=None, rank_ordo=None, rank_familia=None, rank_genus=None, rank_species=None, rank_subspecies=None, rank_hybrid=None, regulation_102=None, regulation_114=None, regulation_411=None, regulation_449=None, regulation_95=None, synonyms=None, is_valid=None, is_published=None, is_deleted=None, hybrid=None, *args, **kwargs):  # noqa: E501
         """TaxonType - a model defined in Swagger"""  # noqa: E501
         self._id_species_plus = None
-        self._pid = None
-        self._name_common_cz = None
-        self._name_common_en = None
-        self._name_scientific = None
         self._name_listed = None
         self._rank_regnum = None
         self._rank_phylum = None
         self._rank_divisio = None
         self._rank_classis = None
         self._rank_ordo = None
         self._rank_familia = None
@@ -108,32 +97,22 @@
         self._rank_subspecies = None
         self._rank_hybrid = None
         self._regulation_102 = None
         self._regulation_114 = None
         self._regulation_411 = None
         self._regulation_449 = None
         self._regulation_95 = None
-        self._regulation_cites = None
-        self._regulation_eu = None
         self._synonyms = None
         self._is_valid = None
         self._is_published = None
         self._is_deleted = None
         self._hybrid = None
         self.discriminator = None
         if id_species_plus is not None:
             self.id_species_plus = id_species_plus
-        if pid is not None:
-            self.pid = pid
-        if name_common_cz is not None:
-            self.name_common_cz = name_common_cz
-        if name_common_en is not None:
-            self.name_common_en = name_common_en
-        if name_scientific is not None:
-            self.name_scientific = name_scientific
         if name_listed is not None:
             self.name_listed = name_listed
         if rank_regnum is not None:
             self.rank_regnum = rank_regnum
         if rank_phylum is not None:
             self.rank_phylum = rank_phylum
         if rank_divisio is not None:
@@ -158,28 +137,25 @@
             self.regulation_114 = regulation_114
         if regulation_411 is not None:
             self.regulation_411 = regulation_411
         if regulation_449 is not None:
             self.regulation_449 = regulation_449
         if regulation_95 is not None:
             self.regulation_95 = regulation_95
-        if regulation_cites is not None:
-            self.regulation_cites = regulation_cites
-        if regulation_eu is not None:
-            self.regulation_eu = regulation_eu
         if synonyms is not None:
             self.synonyms = synonyms
         if is_valid is not None:
             self.is_valid = is_valid
         if is_published is not None:
             self.is_published = is_published
         if is_deleted is not None:
             self.is_deleted = is_deleted
         if hybrid is not None:
             self.hybrid = hybrid
+        TaxonEntryType.__init__(self, *args, **kwargs)
 
     @property
     def id_species_plus(self):
         """Gets the id_species_plus of this TaxonType.  # noqa: E501
 
         Identifikátor species+  # noqa: E501
 
@@ -197,106 +173,14 @@
         :param id_species_plus: The id_species_plus of this TaxonType.  # noqa: E501
         :type: list[str]
         """
 
         self._id_species_plus = id_species_plus
 
     @property
-    def pid(self):
-        """Gets the pid of this TaxonType.  # noqa: E501
-
-        Identifikátor Registru CITES  # noqa: E501
-
-        :return: The pid of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._pid
-
-    @pid.setter
-    def pid(self, pid):
-        """Sets the pid of this TaxonType.
-
-        Identifikátor Registru CITES  # noqa: E501
-
-        :param pid: The pid of this TaxonType.  # noqa: E501
-        :type: str
-        """
-
-        self._pid = pid
-
-    @property
-    def name_common_cz(self):
-        """Gets the name_common_cz of this TaxonType.  # noqa: E501
-
-        Obecný název (česky)  # noqa: E501
-
-        :return: The name_common_cz of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._name_common_cz
-
-    @name_common_cz.setter
-    def name_common_cz(self, name_common_cz):
-        """Sets the name_common_cz of this TaxonType.
-
-        Obecný název (česky)  # noqa: E501
-
-        :param name_common_cz: The name_common_cz of this TaxonType.  # noqa: E501
-        :type: str
-        """
-
-        self._name_common_cz = name_common_cz
-
-    @property
-    def name_common_en(self):
-        """Gets the name_common_en of this TaxonType.  # noqa: E501
-
-        Obecný název (anglicky)  # noqa: E501
-
-        :return: The name_common_en of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._name_common_en
-
-    @name_common_en.setter
-    def name_common_en(self, name_common_en):
-        """Sets the name_common_en of this TaxonType.
-
-        Obecný název (anglicky)  # noqa: E501
-
-        :param name_common_en: The name_common_en of this TaxonType.  # noqa: E501
-        :type: str
-        """
-
-        self._name_common_en = name_common_en
-
-    @property
-    def name_scientific(self):
-        """Gets the name_scientific of this TaxonType.  # noqa: E501
-
-        Vědecký název (latinsky)  # noqa: E501
-
-        :return: The name_scientific of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._name_scientific
-
-    @name_scientific.setter
-    def name_scientific(self, name_scientific):
-        """Sets the name_scientific of this TaxonType.
-
-        Vědecký název (latinsky)  # noqa: E501
-
-        :param name_scientific: The name_scientific of this TaxonType.  # noqa: E501
-        :type: str
-        """
-
-        self._name_scientific = name_scientific
-
-    @property
     def name_listed(self):
         """Gets the name_listed of this TaxonType.  # noqa: E501
 
         listed_under (species+)  # noqa: E501
 
         :return: The name_listed of this TaxonType.  # noqa: E501
         :rtype: str
@@ -545,184 +429,138 @@
 
         self._rank_hybrid = rank_hybrid
 
     @property
     def regulation_102(self):
         """Gets the regulation_102 of this TaxonType.  # noqa: E501
 
-        Exemplář sledovaný podle zákona 102  # noqa: E501
+        Exemplář sledovaný podle zákona č. 102/19963 Sb. (rybářství)  # noqa: E501
 
         :return: The regulation_102 of this TaxonType.  # noqa: E501
         :rtype: bool
         """
         return self._regulation_102
 
     @regulation_102.setter
     def regulation_102(self, regulation_102):
         """Sets the regulation_102 of this TaxonType.
 
-        Exemplář sledovaný podle zákona 102  # noqa: E501
+        Exemplář sledovaný podle zákona č. 102/19963 Sb. (rybářství)  # noqa: E501
 
         :param regulation_102: The regulation_102 of this TaxonType.  # noqa: E501
         :type: bool
         """
 
         self._regulation_102 = regulation_102
 
     @property
     def regulation_114(self):
         """Gets the regulation_114 of this TaxonType.  # noqa: E501
 
-        Exemplář sledovaný podle zákona 114  # noqa: E501
+        Exemplář sledovaný podle zákona č. 114/1997 Sb. (ochrana přírody)  # noqa: E501
 
         :return: The regulation_114 of this TaxonType.  # noqa: E501
-        :rtype: bool
+        :rtype: str
         """
         return self._regulation_114
 
     @regulation_114.setter
     def regulation_114(self, regulation_114):
         """Sets the regulation_114 of this TaxonType.
 
-        Exemplář sledovaný podle zákona 114  # noqa: E501
+        Exemplář sledovaný podle zákona č. 114/1997 Sb. (ochrana přírody)  # noqa: E501
 
         :param regulation_114: The regulation_114 of this TaxonType.  # noqa: E501
-        :type: bool
+        :type: str
         """
+        allowed_values = ["KO", "SO", "O", "", ""]  # noqa: E501
+        if regulation_114 not in allowed_values:
+            raise ValueError(
+                "Invalid value for `regulation_114` ({0}), must be one of {1}"  # noqa: E501
+                .format(regulation_114, allowed_values)
+            )
 
         self._regulation_114 = regulation_114
 
     @property
     def regulation_411(self):
         """Gets the regulation_411 of this TaxonType.  # noqa: E501
 
-        Exemplář sledovaný podle zákona 411  # noqa: E501
+        Exemplář sledovaný podle vyhlášky č. 411/2008 Sb., kterou se stanoví druhy zvířat vyžadující zvláštní péči  # noqa: E501
 
         :return: The regulation_411 of this TaxonType.  # noqa: E501
         :rtype: bool
         """
         return self._regulation_411
 
     @regulation_411.setter
     def regulation_411(self, regulation_411):
         """Sets the regulation_411 of this TaxonType.
 
-        Exemplář sledovaný podle zákona 411  # noqa: E501
+        Exemplář sledovaný podle vyhlášky č. 411/2008 Sb., kterou se stanoví druhy zvířat vyžadující zvláštní péči  # noqa: E501
 
         :param regulation_411: The regulation_411 of this TaxonType.  # noqa: E501
         :type: bool
         """
 
         self._regulation_411 = regulation_411
 
     @property
     def regulation_449(self):
         """Gets the regulation_449 of this TaxonType.  # noqa: E501
 
-        Exemplář sledovaný podle zákona 449  # noqa: E501
+        Exemplář sledovaný podle zákona 449 (myslivost)  # noqa: E501
 
         :return: The regulation_449 of this TaxonType.  # noqa: E501
-        :rtype: bool
+        :rtype: str
         """
         return self._regulation_449
 
     @regulation_449.setter
     def regulation_449(self, regulation_449):
         """Sets the regulation_449 of this TaxonType.
 
-        Exemplář sledovaný podle zákona 449  # noqa: E501
+        Exemplář sledovaný podle zákona 449 (myslivost)  # noqa: E501
 
         :param regulation_449: The regulation_449 of this TaxonType.  # noqa: E501
-        :type: bool
+        :type: str
         """
+        allowed_values = ["A", "B", "", ""]  # noqa: E501
+        if regulation_449 not in allowed_values:
+            raise ValueError(
+                "Invalid value for `regulation_449` ({0}), must be one of {1}"  # noqa: E501
+                .format(regulation_449, allowed_values)
+            )
 
         self._regulation_449 = regulation_449
 
     @property
     def regulation_95(self):
         """Gets the regulation_95 of this TaxonType.  # noqa: E501
 
-        Exemplář sledovaný podle zákona 95  # noqa: E501
+        Exemplář sledovaný podle vyhláška č. 95/1996 Sb. (nebezpečná zvířata)  # noqa: E501
 
         :return: The regulation_95 of this TaxonType.  # noqa: E501
         :rtype: bool
         """
         return self._regulation_95
 
     @regulation_95.setter
     def regulation_95(self, regulation_95):
         """Sets the regulation_95 of this TaxonType.
 
-        Exemplář sledovaný podle zákona 95  # noqa: E501
+        Exemplář sledovaný podle vyhláška č. 95/1996 Sb. (nebezpečná zvířata)  # noqa: E501
 
         :param regulation_95: The regulation_95 of this TaxonType.  # noqa: E501
         :type: bool
         """
 
         self._regulation_95 = regulation_95
 
     @property
-    def regulation_cites(self):
-        """Gets the regulation_cites of this TaxonType.  # noqa: E501
-
-        Exemplář sledovaný podle CITES  # noqa: E501
-
-        :return: The regulation_cites of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._regulation_cites
-
-    @regulation_cites.setter
-    def regulation_cites(self, regulation_cites):
-        """Sets the regulation_cites of this TaxonType.
-
-        Exemplář sledovaný podle CITES  # noqa: E501
-
-        :param regulation_cites: The regulation_cites of this TaxonType.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["I", "II", "III"]  # noqa: E501
-        if regulation_cites not in allowed_values:
-            raise ValueError(
-                "Invalid value for `regulation_cites` ({0}), must be one of {1}"  # noqa: E501
-                .format(regulation_cites, allowed_values)
-            )
-
-        self._regulation_cites = regulation_cites
-
-    @property
-    def regulation_eu(self):
-        """Gets the regulation_eu of this TaxonType.  # noqa: E501
-
-        Exemplář sledovaný podle EU  # noqa: E501
-
-        :return: The regulation_eu of this TaxonType.  # noqa: E501
-        :rtype: str
-        """
-        return self._regulation_eu
-
-    @regulation_eu.setter
-    def regulation_eu(self, regulation_eu):
-        """Sets the regulation_eu of this TaxonType.
-
-        Exemplář sledovaný podle EU  # noqa: E501
-
-        :param regulation_eu: The regulation_eu of this TaxonType.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["A", "B", "C"]  # noqa: E501
-        if regulation_eu not in allowed_values:
-            raise ValueError(
-                "Invalid value for `regulation_eu` ({0}), must be one of {1}"  # noqa: E501
-                .format(regulation_eu, allowed_values)
-            )
-
-        self._regulation_eu = regulation_eu
-
-    @property
     def synonyms(self):
         """Gets the synonyms of this TaxonType.  # noqa: E501
 
         variantní vědecké názvy pro stejný taxon  # noqa: E501
 
         :return: The synonyms of this TaxonType.  # noqa: E501
         :rtype: list[str]
```

### Comparing `sysnet-taxonomy-1.0.0/taxonomy/rest.py` & `sysnet-taxonomy-1.0.0.1/taxonomy/rest.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_admins_api.py` & `sysnet-taxonomy-1.0.0.1/test/test_admins_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_developers_api.py` & `sysnet-taxonomy-1.0.0.1/test/test_developers_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_hybrid_type.py` & `sysnet-taxonomy-1.0.0.1/test/test_hybrid_type.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_public_api.py` & `sysnet-taxonomy-1.0.0.1/test/test_public_api.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_taxon_entry_list_type.py` & `sysnet-taxonomy-1.0.0.1/test/test_taxon_entry_list_type.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_taxon_entry_type.py` & `sysnet-taxonomy-1.0.0.1/test/test_taxon_entry_type.py`

 * *Files identical despite different names*

### Comparing `sysnet-taxonomy-1.0.0/test/test_taxon_type.py` & `sysnet-taxonomy-1.0.0.1/test/test_taxon_type.py`

 * *Files identical despite different names*


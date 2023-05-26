# Comparing `tmp/phdi-1.0.5.tar.gz` & `tmp/phdi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-1.0.5.tar", max compression
+gzip compressed data, was "phdi-1.0.6.tar", max compression
```

## Comparing `phdi-1.0.5.tar` & `phdi-1.0.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-05-17 21:57:42.655238 phdi-1.0.5/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-05-17 21:57:42.655238 phdi-1.0.5/README.md
--rw-r--r--   0        0        0       27 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2776 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     2288 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/core.py
--rw-r--r--   0        0        0    57120 2023-05-17 21:57:43.087275 phdi-1.0.5/phdi/linkage/link.py
--rw-r--r--   0        0        0    11316 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2667 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11839 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2046 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-05-17 21:57:43.091275 phdi-1.0.5/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1820 2023-05-17 21:57:43.095276 phdi-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-26 21:23:14.238944 phdi-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-05-26 21:23:14.238944 phdi-1.0.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2776 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-05-26 21:23:14.702949 phdi-1.0.6/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     8834 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     3167 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/core.py
+-rw-r--r--   0        0        0    57291 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/link.py
+-rw-r--r--   0        0        0    15429 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2752 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11838 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2046 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-05-26 21:23:14.706949 phdi-1.0.6/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1820 2023-05-26 21:23:14.714949 phdi-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    13589 1970-01-01 00:00:00.000000 phdi-1.0.6/PKG-INFO
```

### Comparing `phdi-1.0.5/LICENSE.md` & `phdi-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/README.md` & `phdi-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/cloud/azure.py` & `phdi-1.0.6/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/cloud/core.py` & `phdi-1.0.6/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/cloud/gcp.py` & `phdi-1.0.6/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/containers/base_service.py` & `phdi-1.0.6/phdi/containers/base_service.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/cloud/azure.py` & `phdi-1.0.6/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/conversion/convert.py` & `phdi-1.0.6/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/geospatial/README.md` & `phdi-1.0.6/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/geospatial/census.py` & `phdi-1.0.6/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/geospatial/core.py` & `phdi-1.0.6/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/geospatial/smarty.py` & `phdi-1.0.6/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/harmonization/README.md` & `phdi-1.0.6/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/harmonization/standardization.py` & `phdi-1.0.6/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/linkage/link.py` & `phdi-1.0.6/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/tabulation/tables.py` & `phdi-1.0.6/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/transport/export.py` & `phdi-1.0.6/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/fhir/transport/http.py` & `phdi-1.0.6/phdi/fhir/transport/http.py`

 * *Files 27% similar despite different names*

```diff
@@ -60,67 +60,80 @@
             data=data,
         )
 
     return response
 
 
 def upload_bundle_to_fhir_server(
-    bundle: dict, cred_manager: BaseCredentialManager, fhir_url: str
-) -> requests.Response:
+    bundle: dict,
+    cred_manager: BaseCredentialManager,
+    fhir_url: str,
+    max_bundle_size: int = 500,
+) -> list[requests.Response]:
     """
     Uploads a FHIR resource bundle to the FHIR server.
 
     :param bundle: A FHIR bundle (type "batch" or "transaction") to post.  Each entry in
       the bundle must contain a `request` element in addition to a `resource`.
       The FHIR API provides additional details on creating
       [FHIR-conformant batch/transaction](https://hl7.org/fhir/http.html#transaction)
       bundles.
     :param cred_manager: The credential manager used to authenticate to the FHIR server.
     :param fhir_url: The url of the FHIR server to upload to.
-    :return: A `requests.Request` object containing the response from the FHIR server.
+    :param max_bundle_size: The maximum number of resources per bundle to upload to
+      the FHIR server.
+    :return: A `requests.Response` object containing the response from the FHIR server.
     """
 
     access_token = cred_manager.get_access_token()
+    responses = []
 
-    response = http_request_with_reauth(
-        cred_manager=cred_manager,
-        url=fhir_url,
-        retry_count=3,
-        request_type="POST",
-        allowed_methods=["POST"],
-        headers={
-            "Authorization": f"Bearer {access_token}",
-            "Accept": "application/fhir+json",
-            "Content-Type": "application/fhir+json",
-        },
-        data=bundle,
-    )
-
-    # FHIR uploads are sent as a batch.  Although the batch succeeds,
-    # individual entries within the batch may fail, so we log them here
-    if response.status_code == 200:
-        response_json = response.json()
-        entries = response_json.get("entry", [])
-        for entry_index, entry in enumerate(entries):
-            entry_response = entry.get("response", {})
-
-            # FHIR bundle.entry.response.status is string type - integer status code
-            # plus may inlude a message
-            if entry_response and not entry_response.get("status", "").startswith(
-                "200"
-            ):
-                _log_fhir_server_error(
-                    status_code=int(entry_response["status"][0:3]),
-                    batch_entry_index=entry_index,
-                )
+    # ensure that bundles are below the set maximum size of resources
+    split_bundles = _split_bundle_resources(bundle, max_bundle_size)
 
-    else:
-        _log_fhir_server_error(response.status_code)
+    for single_bundle in split_bundles:
+        response = http_request_with_reauth(
+            cred_manager=cred_manager,
+            url=fhir_url,
+            retry_count=3,
+            request_type="POST",
+            allowed_methods=["POST"],
+            headers={
+                "Authorization": f"Bearer {access_token}",
+                "Accept": "application/fhir+json",
+                "Content-Type": "application/fhir+json",
+            },
+            data=single_bundle,
+        )
+        # FHIR uploads are sent as a batch.  Although the batch succeeds,
+        # individual entries within the batch may fail, so we log them here
+        if response.status_code == 200:
+            response_json = response.json()
+
+            entries = response_json.get("entry", [])
+            for entry_index, entry in enumerate(entries):
+                entry_response = entry.get("response", {})
+
+                # FHIR bundle.entry.response.status is string type - integer status code
+                # plus may inlude a message
+                if entry_response and entry_response.get("status", "") not in [
+                    "200 OK",
+                    "201 Created",
+                    "200",
+                    "201",
+                ]:
+                    _log_fhir_server_error(
+                        status_code=int(entry_response["status"][0:3]),
+                        batch_entry_index=entry_index,
+                    )
+        else:
+            _log_fhir_server_error(response.status_code)
+        responses.append(response)
 
-    return response
+    return responses
 
 
 def fhir_server_get(url: str, cred_manager: BaseCredentialManager) -> requests.Response:
     """
     Submits a GET request to a FHIR server given a url and access token for
     authentication.
 
@@ -145,14 +158,17 @@
 
 
 def _log_fhir_server_error(status_code: int, batch_entry_index: int = None) -> None:
     """
     Logs the error for a given an HTTP status code from a FHIR server's response.
 
     :param status_code: The status code returned by a FHIR server.
+    :param batch_entry_index: A zero-based index indicates which
+        resource in the FHIR bundle received the error.
+        Defaults to None.
     """
     # TODO: We may dedcide to remove logging, and instead report errors back to
     # calling function as raised exceptions.
     batch_decorator = ""
     if batch_entry_index is not None:
         batch_decorator = (
             f"in zero-based message index {batch_entry_index} of FHIR batch "
@@ -183,7 +199,35 @@
         )
 
     elif str(status_code).startswith(("4", "5")):
         error_message = (
             f"FHIR SERVER ERROR {batch_decorator}- Status code {status_code}"
         )
         logging.error(error_message)
+
+
+def _split_bundle_resources(bundle: dict, max_bundle_size: int = 500) -> list:
+    """
+    Receives a FHIR bundle and splits up the resources in the bundle
+    if there are more than 500 resources.  Otherwise it just returns the
+    orginal bundle unmodified.
+
+    :param bundle: A FHIR bundle containing a number of FHIR resources.
+    :param max_bundle_size: The maximum number of resources per bundle to
+      determine where the split of large FHIR bundles should occur.
+    :return: A list of FHIR bundles; if the bundle has <= 500 resources
+    then the list will have only one element.
+    """
+    resources = bundle.get("entry")
+    resource_count = len(resources)
+    split_bundles = []
+
+    entry_index = 0
+    while entry_index <= resource_count:
+        # grab all the resources and place them in the entry list within
+        # the new bundle dictionary up to the maximum number specified
+        partial_bundle = {"resourceType": "Bundle", "type": "batch", "entry": []}
+        partial_bundle["entry"] = resources[entry_index : entry_index + max_bundle_size]
+        # add the new split bundle to the list to be returned
+        split_bundles.append(partial_bundle)
+        entry_index = entry_index + max_bundle_size
+    return split_bundles
```

### Comparing `phdi-1.0.5/phdi/fhir/utils.py` & `phdi-1.0.6/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/geospatial/README.md` & `phdi-1.0.6/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/geospatial/census.py` & `phdi-1.0.6/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/geospatial/core.py` & `phdi-1.0.6/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/geospatial/smarty.py` & `phdi-1.0.6/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/README.md` & `phdi-1.0.6/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/__init__.py` & `phdi-1.0.6/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/double_metaphone.py` & `phdi-1.0.6/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/hl7.py` & `phdi-1.0.6/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/phdi_nicknames.csv` & `phdi-1.0.6/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/standardization.py` & `phdi-1.0.6/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/harmonization/utils.py` & `phdi-1.0.6/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/linkage/__init__.py` & `phdi-1.0.6/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/linkage/algorithms.py` & `phdi-1.0.6/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/linkage/core.py` & `phdi-1.0.6/phdi/linkage/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,22 +33,39 @@
         """
         pass  # pragma: no cover
 
     @abstractmethod
     def insert_match_patient() -> None:
         """
         If a matching person ID has been found in the MPI, inserts a new patient into
-        the patient table and updates the person table to link to the new patient; else
-        inserts a new patient into the patient table and inserts a new person into the
-        person table with a new personID, linking the new personID to the new patient.
+        the patient table, including the matched person id, to link the new patient
+        and matched person ID; else inserts a new patient into the patient table and
+        inserts a new person into the person table with a new person ID, linking the
+        new person ID to the new patient.
 
         """
         pass  # pragma: no cover
 
     @abstractmethod
     def _generate_block_query(self, block_vals: dict) -> str:
         """
         Generates a query for selecting a block of data from the patient table per the
         block_vals parameters. Accepted blocking fields include: first_name, last_name,
         birthdate, addess, city, state, zip, mrn, and sex.
         """
         pass  # pragma: no cover
+
+    @abstractmethod
+    def _insert_person() -> tuple:
+        """
+        If person id is not supplied and external person id is not supplied
+        then insert a new person record with an auto-generated person id (UUID)
+        with a Null external person id and return that new person id. If the
+        person id is not supplied but an external person id is supplied try
+        to find an existing person record with the external person id and
+        return that person id; otherwise add a new person record with an
+        auto-generated person id (UUID) with the supplied external person id
+        and return the new person id.  If person id and external person id are
+        both supplied then update the person records external person id if it
+        is Null and return the person id.
+        """
+        pass  # pragma: no cover
```

### Comparing `phdi-1.0.5/phdi/linkage/link.py` & `phdi-1.0.6/phdi/linkage/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,15 @@
     return hash_obj.hexdigest()
 
 
 def link_record_against_mpi(
     record: dict,
     algo_config: List[dict],
     db_client: BaseMPIConnectorClient,
+    external_person_id: str = None,
 ) -> tuple[bool, str]:
     """
     Runs record linkage on a single incoming record (extracted from a FHIR
     bundle) using an existing database as an MPI. Uses a flexible algorithm
     configuration to allow customization of the exact kind of linkage to
     run. Linkage is assumed to run using cluster membership (i.e. the new
     record must match a certain proportion of existing records all assigned
@@ -636,21 +637,25 @@
                         [linkage_scores[person], belongingness_ratio]
                     )
                 else:
                     linkage_scores[person] = belongingness_ratio
 
     # Didn't match any person in our database
     if len(linkage_scores) == 0:
-        new_person_id = db_client.insert_match_patient(record, person_id=None)
-        return (False, new_person_id)
+        (matched, new_person_id) = db_client.insert_match_patient(
+            record, person_id=None, external_person_id=external_person_id
+        )
+        return (matched, new_person_id)
 
     # Determine strongest match, upsert, then let the caller know
     else:
         best_person = _find_strongest_link(linkage_scores)
-        db_client.insert_match_patient(record, person_id=best_person)
+        db_client.insert_match_patient(
+            record, person_id=best_person, external_person_id=external_person_id
+        )
         return (True, best_person)
 
 
 def load_json_probs(path: pathlib.Path):
     """
     Load a dictionary of probabilities from a JSON-formatted file.
     The probabilities correspond to previously computed m-, u-, or
```

### Comparing `phdi-1.0.5/phdi/linkage/postgres.py` & `phdi-1.0.6/phdi/linkage/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -116,44 +116,46 @@
 
         return blocked_data
 
     def insert_match_patient(
         self,
         patient_resource: Dict,
         person_id=None,
-    ) -> Union[None, str]:
+        external_person_id=None,
+    ) -> Union[None, tuple]:
         """
         If a matching person ID has been found in the MPI, inserts a new patient into
-        the patient table and updates the person table to link to the new patient; else
-        inserts a new patient into the patient table and inserts a new person into the
-        person table with a new personID, linking the new personID to the new patient.
+        the patient table, including the matched person id, to link the new patient
+        and matched person ID; else inserts a new patient into the patient table and
+        inserts a new person into the person table with a new person ID, linking the
+        new person ID to the new patient.
 
         :param patient_resource: A FHIR patient resource.
-        :param person_id: The personID matching the patient record if a match has been
+        :param person_id: The person ID matching the patient record if a match has been
           found in the MPI, defaults to None.
+        :param external_person_id: The external person id for the person that matches
+          the patient record if a match has been found in the MPI, defaults to None.
+        :return: the person id
         """
+        matched = False
         db_cursor = None
         db_conn = None
         try:
             # Use context manager to handle commits and transactions
             with self.get_connection() as db_conn:
                 with db_conn.cursor() as db_cursor:
-                    # Match has not been found
-                    if person_id is None:
-                        # Insert a new record into person table to generate new
-                        # person_id
-                        insert_new_person = SQL(
-                            "INSERT INTO {person_table} (external_person_id) VALUES "
-                            "('NULL') RETURNING person_id;"
-                        ).format(person_table=Identifier(self.person_table))
-
-                        db_cursor.execute(insert_new_person)
-
-                        # Retrieve newly generated person_id
-                        person_id = db_cursor.fetchall()[0][0]
+                    # handle all logic whether to insert, update
+                    # or query to get an existing person record
+                    # then use the returned person_id to link
+                    #  to the newly create patient
+                    matched, person_id = self._insert_person(
+                        db_cursor=db_cursor,
+                        person_id=person_id,
+                        external_person_id=external_person_id,
+                    )
 
                     # Insert into patient table
                     insert_new_patient = SQL(
                         "INSERT INTO {patient_table} "
                         "(patient_id, person_id, patient_resource) VALUES (%s, %s, %s);"
                     ).format(patient_table=Identifier(self.patient_table))
                     data = [
@@ -171,15 +173,15 @@
 
         except Exception as error:  # pragma: no cover
             raise ValueError(f"{error}")
 
         finally:
             self._close_connections(db_conn=db_conn, db_cursor=db_cursor)
 
-        return person_id
+        return (matched, person_id)
 
     def _generate_block_query(self, block_vals: dict) -> Tuple[SQL, list[str]]:
         """
         Generates a query for selecting a block of data from the patient table per the
         block_vals parameters. Accepted blocking fields include: first_name, last_name,
         birthdate, addess, city, state, zip, mrn, and sex.
 
@@ -263,7 +265,84 @@
         if the `with` block terminates before safe execution, this function
         allows a `finally` clause to succinctly clean up all open connections.
         """
         if db_cursor is not None:
             db_cursor.close()
         if db_conn is not None:
             db_conn.close()
+
+    def _insert_person(
+        self,
+        db_cursor: Union[cursor, None] = None,
+        person_id: str = None,
+        external_person_id: str = None,
+    ) -> tuple:
+        """
+        If person id is not supplied and external person id is not supplied
+        then insert a new person record with an auto-generated person id (UUID)
+        with a Null external person id and return that new person id. If the
+        person id is not supplied but an external person id is supplied try
+        to find an existing person record with the external person id and
+        return that person id; otherwise add a new person record with an
+        auto-generated person id (UUID) with the supplied external person id
+        and return the new person id.  If person id and external person id are
+        both supplied then update the person records external person id if it
+        is Null and return the person id.
+
+        :param person_id: The person id for the person record to be inserted
+          or updated, defaults to None.
+        :param external_person_id: The external person id for the person record
+          to be inserted or updated, defaults to None.
+        :return: A tuple of two values; the person id either supplied or
+          auto-generated and a boolean that indicates if there was a match
+          found within the person table or not based upon the external person id
+        """
+        matched = False
+        try:
+            if external_person_id is None:
+                external_person_id = "'NULL'"
+            else:
+                # if external person id is supplied then find if there is already
+                #  a person with that external person id already within the MPI
+                #  - if so, return that person id
+                person_query = SQL(
+                    "SELECT person_id FROM {person_table} WHERE external_person_id = %s"
+                ).format(person_table=Identifier(self.person_table))
+                query_data = [external_person_id]
+                db_cursor.execute(person_query, query_data)
+                # Retrieve person_id that has the supplied external_person_id
+                returned_data = db_cursor.fetchall()
+
+                if returned_data is not None and len(returned_data) > 0:
+                    found_person_id = returned_data[0][0]
+                    matched = True
+                    return matched, found_person_id
+
+            if person_id is None:
+                # Insert a new record into person table to generate new
+                # person_id with either the supplied external person id
+                #  or a null external person id
+                insert_new_person = SQL(
+                    "INSERT INTO {person_table} (external_person_id) VALUES "
+                    "(%s) RETURNING person_id;"
+                ).format(person_table=Identifier(self.person_table))
+                person_data = [external_person_id]
+
+                db_cursor.execute(insert_new_person, person_data)
+
+                # Retrieve newly generated person_id
+                person_id = db_cursor.fetchall()[0][0]
+            # otherwise if person id is supplied and the external person id is supplied
+            # and not none and a record with the external person id was not found
+            #  then update the person record with the supplied external person id
+            elif person_id is not None and external_person_id != "'NULL'":
+                matched = True
+                update_person_query = SQL(
+                    "UPDATE {person_table} SET external_person_id = %s "
+                    "WHERE person_id = %s AND external_person_id = 'NULL' "
+                ).format(person_table=Identifier(self.person_table))
+                update_data = [external_person_id, person_id]
+                db_cursor.execute(update_person_query, update_data)
+
+        except Exception as error:  # pragma: no cover
+            raise ValueError(f"{error}")
+        return matched, person_id
```

### Comparing `phdi-1.0.5/phdi/linkage/seed.py` & `phdi-1.0.6/phdi/linkage/seed.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 
     :param data: Dictionary of patient data that optionionally includes the following
       fields: mrn, ssn, first_name, middle_name, last_name, home_phone, cell-phone, sex,
       birthdate, address, city, state, zip.
     :return: Tuple of the `iris_id` and FHIR bundle.
     """
 
+    patient_id = str(uuid.uuid4())
+
     # Iterate through each patient and convert patient data to FHIR resource
     patient_resource = {
         "resourceType": "Patient",
-        "id": str(uuid.uuid4()),
+        "id": f"{patient_id}",
         "identifier": [
             {
                 "type": {
                     "coding": [
                         {
                             "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
                             "code": "MR",
@@ -71,11 +73,11 @@
             }
         ],
     }
 
     fhir_bundle = {
         "resourceType": "Bundle",
         "id": str(uuid.uuid4()),
-        "entry": [patient_resource],
+        "entry": [{"fullUrl": f"urn:uuid:{patient_id}", "resource": patient_resource}],
     }
 
     return (data["iris_id"], fhir_bundle)
```

### Comparing `phdi-1.0.5/phdi/tabulation/tables.py` & `phdi-1.0.6/phdi/tabulation/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import pathlib
 import json
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sqlite3 as sql
 import yaml
-
 from typing import Literal, List, Union
 from jsonschema import validate
 import importlib.resources
 
 
 def load_schema(path: pathlib.Path) -> dict:
     """
```

### Comparing `phdi-1.0.5/phdi/tabulation/validation_schema.json` & `phdi-1.0.6/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/transport/http.py` & `phdi-1.0.6/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/validation/__init__.py` & `phdi-1.0.6/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/validation/validation.py` & `phdi-1.0.6/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/phdi/validation/xml_utils.py` & `phdi-1.0.6/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-1.0.5/pyproject.toml` & `phdi-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phdi"
-version = "v1.0.5"
+version = "v1.0.6"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>", "Nick Clyde <nclyde@skylight.digital", "Dan Paseltiner <dan@skylight.digital>", "Brady Fausett <brady@skylight.digital>", "Marcelle Goggins <marcelle@skylight.digital", "Nick Bristow <nick@skylight.digital>", "Bryan Britten <bryan@skylight.digital>", "Emma Stephenson <emma@skylight.digital>" , "Gordon Farrell <gordon@skylight.digital>", "Robert Mitchell <rmitchell@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
 documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
```

### Comparing `phdi-1.0.5/PKG-INFO` & `phdi-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 1.0.5
+Version: 1.0.6
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


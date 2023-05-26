# Comparing `tmp/pypromice-1.2.0.tar.gz` & `tmp/pypromice-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypromice-1.2.0.tar", last modified: Tue May 16 12:11:12 2023, max compression
+gzip compressed data, was "pypromice-1.2.1.tar", last modified: Fri May 26 15:51:24 2023, max compression
```

## Comparing `pypromice-1.2.0.tar` & `pypromice-1.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.821236 pypromice-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-16 12:11:02.000000 pypromice-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 12:11:02.000000 pypromice-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-16 12:11:12.821236 pypromice-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-16 12:11:02.000000 pypromice-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.809236 pypromice-1.2.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getBUFR
--rwxr-xr-x   0 runner    (1001) docker     (123)     1646 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getData
--rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getL0tx
--rwxr-xr-x   0 runner    (1001) docker     (123)     1484 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getL3
--rwxr-xr-x   0 runner    (1001) docker     (123)     3452 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getMsg
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/getWatsontx
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-16 12:11:02.000000 pypromice-1.2.0/bin/joinL3
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:11:12.821236 pypromice-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-16 12:11:02.000000 pypromice-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.809236 pypromice-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.809236 pypromice-1.2.0/src/pypromice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.813236 pypromice-1.2.0/src/pypromice/postprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/postprocess/csv2bufr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/postprocess/wmo_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.813236 pypromice-1.2.0/src/pypromice/process/
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/L0toL1.py
--rw-r--r--   0 runner    (1001) docker     (123)    41295 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/L1toL2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17623 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/L2toL3.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31897 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/metadata.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/process/variables.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.821236 pypromice-1.2.0/src/pypromice/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_config1.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_config2.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_email
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1626942 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_raw1.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3337781 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_raw_DataTable2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   348047 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_raw_SlimTableMem1.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1993699 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_raw_transmitted1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/test/test_raw_transmitted2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.821236 pypromice-1.2.0/src/pypromice/tx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/tx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/tx/payload_formats.csv
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/tx/payload_types.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33046 2023-05-16 12:11:02.000000 pypromice-1.2.0/src/pypromice/tx/tx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:11:12.809236 pypromice-1.2.0/src/pypromice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-16 12:11:12.000000 pypromice-1.2.0/src/pypromice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-16 12:11:12.000000 pypromice-1.2.0/src/pypromice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:11:12.000000 pypromice-1.2.0/src/pypromice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 12:11:12.000000 pypromice-1.2.0/src/pypromice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 12:11:12.000000 pypromice-1.2.0/src/pypromice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.100202 pypromice-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-26 15:51:09.000000 pypromice-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:51:09.000000 pypromice-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-26 15:51:24.100202 pypromice-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-26 15:51:09.000000 pypromice-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.088202 pypromice-1.2.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getBUFR
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1646 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getData
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6652 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getL0tx
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1484 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getL3
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3452 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getMsg
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/getWatsontx
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-26 15:51:09.000000 pypromice-1.2.1/bin/joinL3
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:51:24.100202 pypromice-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-26 15:51:09.000000 pypromice-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.088202 pypromice-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.088202 pypromice-1.2.1/src/pypromice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.088202 pypromice-1.2.1/src/pypromice/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/postprocess/csv2bufr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/postprocess/wmo_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.092202 pypromice-1.2.1/src/pypromice/process/
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/L0toL1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41295 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/L1toL2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17623 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/L2toL3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31897 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/metadata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/process/variables.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.096202 pypromice-1.2.1/src/pypromice/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_config1.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_config2.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_email
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1626942 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_raw1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3337781 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_raw_DataTable2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   348047 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_raw_SlimTableMem1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1993699 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_raw_transmitted1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/test/test_raw_transmitted2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.100202 pypromice-1.2.1/src/pypromice/tx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/tx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/tx/payload_formats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/tx/payload_types.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33046 2023-05-26 15:51:09.000000 pypromice-1.2.1/src/pypromice/tx/tx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:24.088202 pypromice-1.2.1/src/pypromice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-26 15:51:24.000000 pypromice-1.2.1/src/pypromice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-26 15:51:24.000000 pypromice-1.2.1/src/pypromice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:51:24.000000 pypromice-1.2.1/src/pypromice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 15:51:24.000000 pypromice-1.2.1/src/pypromice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:51:24.000000 pypromice-1.2.1/src/pypromice.egg-info/top_level.txt
```

### Comparing `pypromice-1.2.0/LICENSE.txt` & `pypromice-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/PKG-INFO` & `pypromice-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.2.0
+Version: 1.2.1
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -27,15 +27,15 @@
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information. 
 
 If you intend to use PROMICE AWS data and/or pypromice in your work, please cite these publications below, along with any other applicable PROMICE publications where possible:
 
 **Fausto, R.S., van As, D., Mankoff, K.D., Vandecrux, B., Citterio, M., Ahlstrøm, A.P., Andersen, S.B., Colgan, W., Karlsson, N.B., Kjeldsen, K.K., Korsgaard, N.J., Larsen, S.H., Nielsen, S., Pedersen, A.Ø., Shields, C.L., Solgaard, A.M., and Box, J.E. (2021) Programme for Monitoring of the Greenland Ice Sheet (PROMICE) automatic weather station data, Earth Syst. Sci. Data, 13, 3819–3845, [https://doi.org/10.5194/essd-13-3819-2021](https://doi.org/10.5194/essd-13-3819-2021)**
 
-**How, P., Wright, P.J., Mankoff, K., and Vandecrux, B. (2023) pypromice v1.0.0, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
+**How, P., Wright, P.J., Mankoff, K., Vandecrux, B., Fausto, R.S. and Ahlstrøm, A.P. (2023) pypromice, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
 
 
 ## Installation
 
 ### Quick install
 
 The latest release of pypromice can installed using pip:
```

### Comparing `pypromice-1.2.0/README.md` & `pypromice-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information. 
 
 If you intend to use PROMICE AWS data and/or pypromice in your work, please cite these publications below, along with any other applicable PROMICE publications where possible:
 
 **Fausto, R.S., van As, D., Mankoff, K.D., Vandecrux, B., Citterio, M., Ahlstrøm, A.P., Andersen, S.B., Colgan, W., Karlsson, N.B., Kjeldsen, K.K., Korsgaard, N.J., Larsen, S.H., Nielsen, S., Pedersen, A.Ø., Shields, C.L., Solgaard, A.M., and Box, J.E. (2021) Programme for Monitoring of the Greenland Ice Sheet (PROMICE) automatic weather station data, Earth Syst. Sci. Data, 13, 3819–3845, [https://doi.org/10.5194/essd-13-3819-2021](https://doi.org/10.5194/essd-13-3819-2021)**
 
-**How, P., Wright, P.J., Mankoff, K., and Vandecrux, B. (2023) pypromice v1.0.0, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
+**How, P., Wright, P.J., Mankoff, K., Vandecrux, B., Fausto, R.S. and Ahlstrøm, A.P. (2023) pypromice, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
 
 
 ## Installation
 
 ### Quick install
 
 The latest release of pypromice can installed using pip:
```

### Comparing `pypromice-1.2.0/bin/getBUFR` & `pypromice-1.2.1/bin/getBUFR`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/getData` & `pypromice-1.2.1/bin/getData`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/getL0tx` & `pypromice-1.2.1/bin/getL0tx`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/getL3` & `pypromice-1.2.1/bin/getL3`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/getMsg` & `pypromice-1.2.1/bin/getMsg`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/getWatsontx` & `pypromice-1.2.1/bin/getWatsontx`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/bin/joinL3` & `pypromice-1.2.1/bin/joinL3`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/setup.py` & `pypromice-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypromice",
-    version="1.2.0",
+    version="1.2.1",
     author="GEUS Glaciology and Climate",
     description="PROMICE/GC-Net data processing toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GEUS-Glaciology-and-Climate/pypromice",
     project_urls={
         "Bug Tracker": "https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues",
```

### Comparing `pypromice-1.2.0/src/pypromice/get.py` & `pypromice-1.2.1/src/pypromice/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 import xarray as xr
 import unittest, pkg_resources
 from datetime import datetime
    
 def aws_names():
     '''Return PROMICE and GC-Net AWS names that can be used in get.aws_data() 
     fetching'''
-    lookup = lookup_table(['doi:10.22008/FK2/IW73UU', 'doi:10.22008/FK2/GNYFUK'])
+    lookup = lookup_table(['doi:10.22008/FK2/IW73UU'])
     print(f'Available dataset keywords: {list(lookup.keys())}')
     return list(lookup.keys())
 
 def aws_data(aws_name):
     '''Return PROMICE and GC-Net AWS L3 v3 hourly observations
     
     Returns
     -------
     df : pandas.DataFrame
         AWS observations dataframe
     '''
-    lookup = lookup_table(['doi:10.22008/FK2/IW73UU', 'doi:10.22008/FK2/GNYFUK'])
+    lookup = lookup_table(['doi:10.22008/FK2/IW73UU'])
     assert aws_name.lower() in list(lookup.keys())
     data = pd.read_csv(lookup[aws_name], index_col=0, parse_dates=True)
     return data        
   
 def watson_discharge(t='hour'):
     '''Return PROMICE hourly Watson river discharge
     
@@ -137,15 +137,15 @@
     return df
 
 #------------------------------------------------------------------------------
         
 class TestGet(unittest.TestCase): 
     def testURL(self):
         '''Test URL retrieval'''
-        l = lookup_table(['doi:10.22008/FK2/IW73UU', 'doi:10.22008/FK2/GNYFUK'])
+        l = lookup_table(['doi:10.22008/FK2/IW73UU'])
         self.assertTrue('10.22008/FK2' in list(l.values())[0])
     
     def testAWSname(self):  
         '''Test AWS names retrieval'''
         n = aws_names()
         self.assertIsInstance(n, list)
         self.assertTrue('nuk_k_hour.csv' in n)
```

### Comparing `pypromice-1.2.0/src/pypromice/postprocess/csv2bufr.py` & `pypromice-1.2.1/src/pypromice/postprocess/csv2bufr.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/postprocess/wmo_config.py` & `pypromice-1.2.1/src/pypromice/postprocess/wmo_config.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/L0toL1.py` & `pypromice-1.2.1/src/pypromice/process/L0toL1.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/L1toL2.py` & `pypromice-1.2.1/src/pypromice/process/L1toL2.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/L2toL3.py` & `pypromice-1.2.1/src/pypromice/process/L2toL3.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/aws.py` & `pypromice-1.2.1/src/pypromice/process/aws.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/metadata.csv` & `pypromice-1.2.1/src/pypromice/process/metadata.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/process/variables.csv` & `pypromice-1.2.1/src/pypromice/process/variables.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_config1.toml` & `pypromice-1.2.1/src/pypromice/test/test_config1.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_config2.toml` & `pypromice-1.2.1/src/pypromice/test/test_config2.toml`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_email` & `pypromice-1.2.1/src/pypromice/test/test_email`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_raw1.txt` & `pypromice-1.2.1/src/pypromice/test/test_raw1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_raw_DataTable2.txt` & `pypromice-1.2.1/src/pypromice/test/test_raw_DataTable2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_raw_SlimTableMem1.txt` & `pypromice-1.2.1/src/pypromice/test/test_raw_SlimTableMem1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_raw_transmitted1.txt` & `pypromice-1.2.1/src/pypromice/test/test_raw_transmitted1.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/test/test_raw_transmitted2.txt` & `pypromice-1.2.1/src/pypromice/test/test_raw_transmitted2.txt`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/tx/payload_formats.csv` & `pypromice-1.2.1/src/pypromice/tx/payload_formats.csv`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice/tx/tx.py` & `pypromice-1.2.1/src/pypromice/tx/tx.py`

 * *Files identical despite different names*

### Comparing `pypromice-1.2.0/src/pypromice.egg-info/PKG-INFO` & `pypromice-1.2.1/src/pypromice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypromice
-Version: 1.2.0
+Version: 1.2.1
 Summary: PROMICE/GC-Net data processing toolbox
 Home-page: https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Author: GEUS Glaciology and Climate
 Project-URL: Bug Tracker, https://github.com/GEUS-Glaciology-and-Climate/pypromice/issues
 Project-URL: Documentation, https://pypromice.readthedocs.io
 Project-URL: Source Code, https://github.com/GEUS-Glaciology-and-Climate/pypromice
 Keywords: promice gc-net aws climate glaciology greenland geus
@@ -27,15 +27,15 @@
 
 It is envisioned for pypromice to be the go-to toolbox for handling and processing [PROMICE](https://promice.dk) and [GC-Net](http://cires1.colorado.edu/steffen/gcnet/) datasets. New releases of pypromice are uploaded alongside PROMICE AWS data releases to our [Dataverse](https://dataverse.geus.dk/dataverse/PROMICE) for transparency purposes and to encourage collaboration on improving our data. Please visit the pypromice [readthedocs](https://pypromice.readthedocs.io/en/latest/?badge=latest) for more information. 
 
 If you intend to use PROMICE AWS data and/or pypromice in your work, please cite these publications below, along with any other applicable PROMICE publications where possible:
 
 **Fausto, R.S., van As, D., Mankoff, K.D., Vandecrux, B., Citterio, M., Ahlstrøm, A.P., Andersen, S.B., Colgan, W., Karlsson, N.B., Kjeldsen, K.K., Korsgaard, N.J., Larsen, S.H., Nielsen, S., Pedersen, A.Ø., Shields, C.L., Solgaard, A.M., and Box, J.E. (2021) Programme for Monitoring of the Greenland Ice Sheet (PROMICE) automatic weather station data, Earth Syst. Sci. Data, 13, 3819–3845, [https://doi.org/10.5194/essd-13-3819-2021](https://doi.org/10.5194/essd-13-3819-2021)**
 
-**How, P., Wright, P.J., Mankoff, K., and Vandecrux, B. (2023) pypromice v1.0.0, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
+**How, P., Wright, P.J., Mankoff, K., Vandecrux, B., Fausto, R.S. and Ahlstrøm, A.P. (2023) pypromice, GEUS Dataverse, [https://doi.org/10.22008/FK2/3TSBF0](https://doi.org/10.22008/FK2/3TSBF0)** 
 
 
 ## Installation
 
 ### Quick install
 
 The latest release of pypromice can installed using pip:
```

### Comparing `pypromice-1.2.0/src/pypromice.egg-info/SOURCES.txt` & `pypromice-1.2.1/src/pypromice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


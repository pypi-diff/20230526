# Comparing `tmp/openpolicedata-0.5.3.tar.gz` & `tmp/openpolicedata-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpolicedata-0.5.3.tar", last modified: Wed May 17 11:30:29 2023, max compression
+gzip compressed data, was "openpolicedata-0.5.4.tar", last modified: Thu May 25 22:23:39 2023, max compression
```

## Comparing `openpolicedata-0.5.3.tar` & `openpolicedata-0.5.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.701840 openpolicedata-0.5.3/
--rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.3/LICENSE
--rw-rw-rw-   0        0        0    14926 2023-05-17 11:30:29.701840 openpolicedata-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    13810 2023-05-17 11:28:27.000000 openpolicedata-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.674685 openpolicedata-0.5.3/openpolicedata/
--rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.3/openpolicedata/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-17 11:28:49.000000 openpolicedata-0.5.3/openpolicedata/_version.py
--rw-rw-rw-   0        0        0    27852 2023-05-15 18:51:42.000000 openpolicedata-0.5.3/openpolicedata/data.py
--rw-rw-rw-   0        0        0    76281 2023-05-15 22:48:16.000000 openpolicedata-0.5.3/openpolicedata/data_loaders.py
--rw-rw-rw-   0        0        0    10789 2023-05-16 01:27:28.000000 openpolicedata-0.5.3/openpolicedata/datasets.py
--rw-rw-rw-   0        0        0     8688 2023-05-15 14:13:51.000000 openpolicedata-0.5.3/openpolicedata/defs.py
--rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.3/openpolicedata/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.685684 openpolicedata-0.5.3/openpolicedata.egg-info/
--rw-rw-rw-   0        0        0    14926 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-17 11:30:29.000000 openpolicedata-0.5.3/openpolicedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0     1318 2023-05-17 11:30:29.702841 openpolicedata-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:30:29.698841 openpolicedata-0.5.3/tests/
--rw-rw-rw-   0        0        0    21379 2023-05-15 20:54:33.000000 openpolicedata-0.5.3/tests/test_data_loaders.py
--rw-rw-rw-   0        0        0     9154 2023-05-15 21:25:37.000000 openpolicedata-0.5.3/tests/test_datasets.py
--rw-rw-rw-   0        0        0    11203 2023-05-16 01:20:33.000000 openpolicedata-0.5.3/tests/test_opd_data1.py
--rw-rw-rw-   0        0        0     7997 2023-05-15 18:44:53.000000 openpolicedata-0.5.3/tests/test_opd_data2.py
--rw-rw-rw-   0        0        0    11428 2023-05-04 00:15:34.000000 openpolicedata-0.5.3/tests/test_opd_data3.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.062993 openpolicedata-0.5.4/
+-rw-rw-rw-   0        0        0     1542 2022-02-12 00:47:00.000000 openpolicedata-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0    14953 2023-05-25 22:23:39.062993 openpolicedata-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13810 2023-05-25 21:58:14.000000 openpolicedata-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.038732 openpolicedata-0.5.4/openpolicedata/
+-rw-rw-rw-   0        0        0      569 2022-09-24 21:27:15.000000 openpolicedata-0.5.4/openpolicedata/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-25 21:52:33.000000 openpolicedata-0.5.4/openpolicedata/_version.py
+-rw-rw-rw-   0        0        0    27852 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/openpolicedata/data.py
+-rw-rw-rw-   0        0        0    76703 2023-05-25 21:52:20.000000 openpolicedata-0.5.4/openpolicedata/data_loaders.py
+-rw-rw-rw-   0        0        0    10789 2023-05-25 22:01:01.000000 openpolicedata-0.5.4/openpolicedata/datasets.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/openpolicedata/defs.py
+-rw-rw-rw-   0        0        0     1601 2022-09-24 20:54:13.000000 openpolicedata-0.5.4/openpolicedata/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.050165 openpolicedata-0.5.4/openpolicedata.egg-info/
+-rw-rw-rw-   0        0        0    14953 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-05-25 22:23:39.000000 openpolicedata-0.5.4/openpolicedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-25 22:23:38.000000 openpolicedata-0.5.4/openpolicedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      426 2023-02-11 00:12:22.000000 openpolicedata-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1369 2023-05-25 22:23:39.063996 openpolicedata-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-01-02 22:32:48.000000 openpolicedata-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 22:23:39.060994 openpolicedata-0.5.4/tests/
+-rw-rw-rw-   0        0        0    21379 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_data_loaders.py
+-rw-rw-rw-   0        0        0     9154 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    11172 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_opd_data1.py
+-rw-rw-rw-   0        0        0     7997 2023-05-17 22:48:02.000000 openpolicedata-0.5.4/tests/test_opd_data2.py
+-rw-rw-rw-   0        0        0    11428 2023-05-25 21:49:05.000000 openpolicedata-0.5.4/tests/test_opd_data3.py
```

### Comparing `openpolicedata-0.5.3/LICENSE` & `openpolicedata-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/PKG-INFO` & `openpolicedata-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: rapidfuzz
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
 
 # OpenPoliceData
 OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions.
```

### Comparing `openpolicedata-0.5.3/README.md` & `openpolicedata-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/openpolicedata/__init__.py` & `openpolicedata-0.5.4/openpolicedata/__init__.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/openpolicedata/data.py` & `openpolicedata-0.5.4/openpolicedata/data.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/openpolicedata/data_loaders.py` & `openpolicedata-0.5.4/openpolicedata/data_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 import warnings
 from time import sleep
 from tqdm import tqdm
 from math import ceil
 import re
 from xlrd.biffh import XLRDError
 
-from rapidfuzz import fuzz
-
 try:
     import geopandas as gpd
     from shapely.geometry import Point
     _has_gpd = True
 except:
     _has_gpd = False
 
@@ -593,14 +591,20 @@
                                 if len(df.columns)+cols_added == len(table.columns) and \
                                     (df.columns == table.columns[:len(df.columns)]).sum()>=len(df.columns)-3-cols_added:
                                     # Try to find a typo
                                     for m in [j for j in range(len(df.columns)) if table.columns[j]!=df.columns[j]]:
                                         for k in col_matches[m]:
                                             if table.columns[k]==df.columns[m]:
                                                 break
+                                            try:
+                                                from rapidfuzz import fuzz
+                                            except:
+                                                raise ImportError(f"{self.url} requires installation of rapidfuzz " + 
+                                                    "(https://pypi.org/project/rapidfuzz/) to load data from multiple years (pip install rapidfuzz)")
+
                                             if fuzz.ratio(table.columns[k], df.columns[m]) > 80:
                                                 print(f"Identified difference in column names when combining sheets {year_dict[y-1]} and {year_dict[y]}. " + 
                                                     f"Column names are '{table.columns[k]}' and '{df.columns[m]}'. This appears to be a typo. " + 
                                                     f"These columns are assumed to be the same and will be combined as column '{table.columns[k]}'")
                                                 df.columns = [table.columns[k] if j==m else df.columns[j] for j in range(len(df.columns))]
                                                 break
                                         else:
```

### Comparing `openpolicedata-0.5.3/openpolicedata/datasets.py` & `openpolicedata-0.5.4/openpolicedata/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         df.rename(columns={
             "Jurisdiction" : "Agency",
             "jurisdiction_field" : "agency_field"
         }, inplace=True)
 
     # Convert years to int
     df["Year"] = [int(x) if x.isdigit() else x for x in df["Year"]]
-    df["Year"] = df["Year"].apply(lambda x: "MULTIPLE" if x=="MULTI" else x)
+    df["Year"] = df["Year"].apply(lambda x: defs.MULTI if x=="MULTI" else x)
     df["SourceName"] = df["SourceName"].str.replace("Police Department", "")
-    df["Agency"] = df["Agency"].str.replace("Police Department", "").apply(lambda x: "MULTIPLE" if x=="MULTI" else x)
+    df["Agency"] = df["Agency"].str.replace("Police Department", "").apply(lambda x: defs.MULTI if x=="MULTI" else x)
 
     for col in df.columns:
         df[col] = [x.strip() if type(x)==str else x for x in df[col]]
 
     # ArcGIS datasets should have a URL ending in either /FeatureServer/# or /MapServer/#
     # Where # is a layer #
     urls = list(df["URL"])
```

### Comparing `openpolicedata-0.5.3/openpolicedata/defs.py` & `openpolicedata-0.5.4/openpolicedata/defs.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/openpolicedata/exceptions.py` & `openpolicedata-0.5.4/openpolicedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/openpolicedata.egg-info/PKG-INFO` & `openpolicedata-0.5.4/openpolicedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpolicedata
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Python library providing easy access to 276+ incident-level open datasets released by police departments including traffic stops, use of force, officer-involved shootings, and complaints data
 Home-page: https://github.com/openpolicedata/openpolicedata
 Author: Matt Sowd
 Author-email: openpolicedata@gmail.com
 Project-URL: Bug Tracker, https://github.com/openpolicedata/openpolicedata/issues
 Keywords: police data,use of force,traffic,stops,complaints,officer-involved,shootings,pandas,arcgis,socrata,police transparency,police accountability
 Classifier: License :: OSI Approved :: BSD License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: rapidfuzz
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/openpolicedata.svg)](https://badge.fury.io/py/openpolicedata)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openpolicedata/opd-examples/HEAD)
 
 # OpenPoliceData
 OpenPoliceData is a Python package that provides easy access to 365 (and growing) incident-level open datasets from police departments around the United States. Datasets include traffic stops, use of force, officer-involved shootings, complaints, and other types of police interactions.
```

### Comparing `openpolicedata-0.5.3/openpolicedata.egg-info/SOURCES.txt` & `openpolicedata-0.5.4/openpolicedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/setup.cfg` & `openpolicedata-0.5.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -67,17 +67,20 @@
 00000420: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
 00000430: 0d0a 093d 202e 0d0a 7061 636b 6167 6573  ...= ...packages
 00000440: 203d 206f 7065 6e70 6f6c 6963 6564 6174   = openpolicedat
 00000450: 610d 0a70 7974 686f 6e5f 7265 7175 6972  a..python_requir
 00000460: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
 00000470: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
 00000480: 0a09 6f70 656e 7079 786c 0d0a 096e 756d  ..openpyxl...num
-00000490: 7079 0d0a 0970 616e 6461 730d 0a09 7079  py...pandas...py
-000004a0: 7072 6f6a 0d0a 0972 6170 6964 6675 7a7a  proj...rapidfuzz
+00000490: 7079 0d0a 0970 6163 6b61 6769 6e67 0d0a  py...packaging..
+000004a0: 0970 616e 6461 730d 0a09 7079 7072 6f6a  .pandas...pyproj
 000004b0: 0d0a 0972 6571 7565 7374 730d 0a09 736f  ...requests...so
 000004c0: 6461 7079 0d0a 0974 7164 6d0d 0a09 786c  dapy...tqdm...xl
-000004d0: 7264 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  rd....[options.p
-000004e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000004f0: 6865 7265 203d 202e 0d0a 0d0a 5b65 6767  here = .....[egg
-00000500: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000510: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000520: 2030 0d0a 0d0a                            0....
+000004d0: 7264 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rd....[options.e
+000004e0: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
+000004f0: 7261 7069 6466 757a 7a20 3d20 7261 7069  rapidfuzz = rapi
+00000500: 6466 757a 7a0d 0a0d 0a5b 6f70 7469 6f6e  dfuzz....[option
+00000510: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000520: 0d0a 7768 6572 6520 3d20 2e0d 0a0d 0a5b  ..where = .....[
+00000530: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000540: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000550: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `openpolicedata-0.5.3/tests/test_data_loaders.py` & `openpolicedata-0.5.4/tests/test_data_loaders.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/tests/test_datasets.py` & `openpolicedata-0.5.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `openpolicedata-0.5.3/tests/test_opd_data1.py` & `openpolicedata-0.5.4/tests/test_opd_data1.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,22 +284,22 @@
 					f.write("\n")
 
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
-	csvfile = os.path.join("..", "opd-data", "opd_source_table.csv")
+	csvfile = r"..\opd-data\opd_source_table.csv"
 	last = None
 	last = 873-290+1
 	skip = None
-	# skip = "Bloomington"
+	skip = "Bloomington"
 	source = None
 	# source = "Mesa"
-	# tp.check_table_type_warning(csvfile, source, last, skip, None) 
-	# tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
-	# tp.test_check_version(csvfile, None, last, skip, None) #
+	tp.check_table_type_warning(csvfile, source, last, skip, None) 
+	tp.test_offsets_and_nrows(csvfile, source, last, skip, None) 
+	tp.test_check_version(csvfile, None, last, skip, None) #
 	tp.test_source_download_limitable(csvfile, source, last, skip, None) 
 	
-	# tp.test_get_count(csvfile, None, last, skip, None)
-	# tp.test_load_gen(csvfile, source, last, skip, None) 
+	tp.test_get_count(csvfile, None, last, skip, None)
+	tp.test_load_gen(csvfile, source, last, skip, None)
```

### Comparing `openpolicedata-0.5.3/tests/test_opd_data2.py` & `openpolicedata-0.5.4/tests/test_opd_data2.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 if __name__ == "__main__":
 	# For testing
 	tp = TestData()
 	# (self, csvfile, source, last, skip, loghtml)
 	csvfile = None
 	csvfile = os.path.join("..","opd-data","opd_source_table.csv")
 	last = None
-	last = 873-857+1
+	last = 863-791+1
 	source = None
 	# source = "Washington D.C."
 	skip = None
 	# skip = "Fayetteville,Seattle"
 	tp.test_get_years(csvfile, source, last, skip, None)
 	# tp.test_get_agencies(csvfile, None, None, skip, None)
 	# tp.test_get_agencies_name_match(csvfile, None, None, skip, None)
```

### Comparing `openpolicedata-0.5.3/tests/test_opd_data3.py` & `openpolicedata-0.5.4/tests/test_opd_data3.py`

 * *Files identical despite different names*


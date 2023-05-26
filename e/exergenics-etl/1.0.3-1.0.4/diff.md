# Comparing `tmp/exergenics-etl-1.0.3.tar.gz` & `tmp/exergenics-etl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.0.3.tar", last modified: Thu May 25 07:10:40 2023, max compression
+gzip compressed data, was "exergenics-etl-1.0.4.tar", last modified: Fri May 26 04:06:14 2023, max compression
```

## Comparing `exergenics-etl-1.0.3.tar` & `exergenics-etl-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48053 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/src/exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-05-25 07:10:36.000000 exergenics-etl-1.0.3/app/exergenics_etl/test/test_exergenics_etl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:10:40.000000 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 07:10:40.000000 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:10:40.000000 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 07:10:40.000000 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 07:10:40.000000 exergenics-etl-1.0.3/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:10:40.163741 exergenics-etl-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-25 07:10:38.000000 exergenics-etl-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.887457 exergenics-etl-1.0.4/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48613 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 04:06:13.000000 exergenics-etl-1.0.4/setup.py
```

### Comparing `exergenics-etl-1.0.3/LICENSE` & `exergenics-etl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.3/app/exergenics_etl/__init__.py` & `exergenics-etl-1.0.4/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.3/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.0.4/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import zipfile
 import sqlalchemy
-from exergenics.exergenics import ExergenicsLogger as Logger
+from ..src.logger import ETLLogger as Logger
 import pandas as pd
 from pytz import timezone
 from datetime import datetime
 from typing import Union, Dict
 from exergenics import exergenics
 from urllib.parse import quote_plus
 from sqlalchemy import create_engine
@@ -31,15 +31,15 @@
 N_COLUMN_LONG_DATA = 3  # The number of columns in a long-format data table
 DEFAULT_POSITION_DAY = 0  # The default position of the day of month in timestamps
 SUMMARY_COLUMNS = ['count', 'mean', 'std',
                    'min', '25%', '50%', '75%', 'max']
 
 
 logger = Logger(loggerName='Exergenics-ETL',
-                component='data_modules', subComponent='pre_merged')
+                component='python_package', subComponent='exergenics_etl')
 
 
 def hello(name: str) -> None:
     """Says hello to someone.
 
     Args:
         name (str): The name of the person to greet.
@@ -391,15 +391,16 @@
 
         # Try reading the file with different numbers of rows to skip
         skiprowsTrials = range(10)
 
         for skiprowsTrial in skiprowsTrials:
             try:
                 # Try reading the CSV file with the current number of rows to skip
-                df = pd.read_csv(zf.open(fileName), skiprows=skiprowsTrial, header=None)
+                df = pd.read_csv(zf.open(fileName),
+                                 skiprows=skiprowsTrial, header=None)
                 skiprows = skiprowsTrial
                 headerRowID = 0
 
                 self.logger.info(
                     f'Found skiprows value = {skiprowsTrial}')
                 return df, skiprows, headerRowID
 
@@ -475,17 +476,36 @@
         # Set header as column names
         df.columns = df.loc[headerRowId].values
 
         # Remove headers from values
         df.drop(labels=headerRowId, inplace=True)
         df.reset_index(inplace=True, drop=True)  # Replace and reset index
 
+        # Convert columns to best possible dtypes
+        df = df.convert_dtypes(convert_string=False, convert_boolean=False)
+
         return df
 
 
+def convertable_to_float(string: str) -> bool:
+    """Checks if a given string can be converted to a float.
+
+    Args:
+        string (str): The input string to be checked.
+
+    Returns:
+        bool: True if the string can be converted to a float, False otherwise.
+    """
+    try:
+        result = float(string)
+        return True
+    except ValueError:
+        return False
+    
+
 class InputValidation:
     """A class to provide automated validation for CSV files.
     """
 
     def __init__(self, validTimestampHeaders: list, genericColumnHeaders: list):
         """Constructs all the necessary attributes for the InputValidation object.
 
@@ -540,17 +560,17 @@
         Returns:
             bool: True if input is in a wide format.
         """
 
         # If there are only 3 columns in this data file
         if df.shape[1] == N_COLUMN_LONG_DATA:
 
-            # If the 2nd column is a column of strings
+            # If none of the values in the 2nd column can be converted to float
             col2 = df[df.columns[1]]
-            if pd.api.types.is_string_dtype(col2.dtype):
+            if not any(col2.apply(convertable_to_float)):
 
                 # If the average length of the strings in the 2nd column is longer than 10
                 if col2.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
                     return False  # We think this is a wide format dataset
 
         return True
```

### Comparing `exergenics-etl-1.0.3/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.0.4/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.3/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.0.4/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 import os
 import sys
 import pandas as pd
 from pandas import Timestamp
 import numpy as np
 import shutil
 import zipfile
-from exergenics.exergenics import ExergenicsLogger as Logger
+from ..src.logger import ETLLogger as Logger
 from dotenv import load_dotenv
 
 from ..src.exergenics_etl import (
     create_api,
     create_sql_engine,
     get_time_now,
     create_tmp_folder,
     generate_CSV_name,
     strftime_for_NaT,
     generate_one_manifest_row,
     generate_output_file_path,
     get_file_name_list,
     SkipRowsMachine,
+    convertable_to_float,
     InputValidation,
     calculate_time_interval,
     DatetimeParser,
     DEFAULT_POSITION_DAY,
     transform_columns_to_long_dataframes,
     get_point_summary,
     get_statistical_summary,
@@ -222,52 +223,69 @@
     @pytest.fixture(scope='function')
     def my_skipRowsMachine(self):
         skipRowsMachine = SkipRowsMachine()
         return skipRowsMachine
 
     def test_skiprows1(self, my_expected_first_row, my_skipRowsMachine):
         """Test for finding skiprows value with _auto_skiprows_csv and applying the value on a XLSX sheet."""
-        myTestFileNames = ["skiprows_test/skiprows2.csv", "skiprows_test/skiprows2.xlsx"]
+        myTestFileNames = ["skiprows_test/skiprows.csv", "skiprows_test/skiprows.xlsx"]
         myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test.zip"
         myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
         for fileName in myTestFileNames:
             df = my_skipRowsMachine.read(fileName, myTestZippedFile)
             assert all(df.columns.values == my_expected_first_row)
 
     def test_skiprows2(self, my_expected_first_row, my_skipRowsMachine):
         """Test for finding skiprows value with _auto_skiprows_excel and applying the value on a CSV."""
-        myTestFileNames = ["skiprows_test/skiprows2.xlsx", "skiprows_test/skiprows2.csv"]
+        myTestFileNames = ["skiprows_test/skiprows.xlsx", "skiprows_test/skiprows.csv"]
         myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test.zip"
         myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
         for fileName in myTestFileNames:
             df = my_skipRowsMachine.read(fileName, myTestZippedFile)
             assert all(df.columns.values == my_expected_first_row)
     
     def test_skiprows3(self, my_expected_first_row, my_skipRowsMachine):
         """Test for finding skiprows value with _auto_skiprows_csv and applying the value on a XLSX sheet."""
-        myTestFileNames = ["skiprows_test/skiprows.xlsx", "skiprows_test/skiprows.csv"]
+        myTestFileNames = ["skiprows_test2/skiprows.xlsx", "skiprows_test2/skiprows.csv"]
         myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test2.zip"
         myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
         for fileName in myTestFileNames:
             df = my_skipRowsMachine.read(fileName, myTestZippedFile)
             assert all(df.columns.values == my_expected_first_row)
 
     def test_skiprows4(self, my_expected_first_row, my_skipRowsMachine):
-        myTestFileNames = ["skiprows_test/skiprows.csv", "skiprows_test/skiprows.xlsx"]
+        myTestFileNames = ["skiprows_test2/skiprows.csv", "skiprows_test2/skiprows.xlsx"]
         myTestZipfilePath = "app/exergenics_etl/test/testData/skiprows_test2.zip"
         myTestZippedFile = zipfile.ZipFile(myTestZipfilePath)
 
         for fileName in myTestFileNames:
             df = my_skipRowsMachine.read(fileName, myTestZippedFile)
             assert all(df.columns.values == my_expected_first_row)
 
 
+class TestConvertableToFloatClass:
+
+    @pytest.mark.parametrize("string, expected", [
+    ("3.14", True),  # Valid float string
+    ("0", True),     # Valid float string
+    ("-5.2", True),  # Valid float string
+    ("1e-5", True),  # Valid float string
+    (np.nan, True),  # Convertable nan
+    ("abc", False),  # Invalid float string
+    ("1.23.45", False),  # Invalid float string
+    ("12a", False),  # Invalid float string
+    ("", False),     # Empty string
+    ])
+    def test_convertable_to_float(self, string, expected):
+        assert convertable_to_float(string) == expected
+
+
 class TestInputValidationClass:
 
     @pytest.fixture(scope='class')
     def my_wide_format_dataframe(self):
         filePath = 'app/exergenics_etl/test/testData/wide_data.csv'
         df = pd.read_csv(filePath)
         return df
```

### Comparing `exergenics-etl-1.0.3/setup.py` & `exergenics-etl-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.0.3",
+    version="v1.0.4",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```


# Comparing `tmp/ma_fi-0.1.1.tar.gz` & `tmp/ma_fi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_fi-0.1.1.tar", last modified: Fri May 26 13:23:01 2023, max compression
+gzip compressed data, was "ma_fi-0.1.2.tar", last modified: Fri May 26 13:54:54 2023, max compression
```

## Comparing `ma_fi-0.1.1.tar` & `ma_fi-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 13:23:01.339755 ma_fi-0.1.1/
--rw-rw-rw-   0        0        0      584 2023-05-26 13:23:01.339755 ma_fi-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 13:23:01.294755 ma_fi-0.1.1/ma_fi/
--rw-rw-rw-   0        0        0      495 2023-05-24 13:49:34.000000 ma_fi-0.1.1/ma_fi/__init__.py
--rw-rw-rw-   0        0        0     1346 2023-05-23 11:53:26.000000 ma_fi-0.1.1/ma_fi/download.py
-drwxrwxrwx   0        0        0        0 2023-05-26 13:23:01.333125 ma_fi-0.1.1/ma_fi.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-26 13:23:00.000000 ma_fi-0.1.1/ma_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-26 13:23:01.000000 ma_fi-0.1.1/ma_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 13:23:00.000000 ma_fi-0.1.1/ma_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-26 13:23:00.000000 ma_fi-0.1.1/ma_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 13:23:00.000000 ma_fi-0.1.1/ma_fi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 13:23:01.339755 ma_fi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-26 13:20:29.000000 ma_fi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.249026 ma_fi-0.1.2/
+-rw-rw-rw-   0        0        0      584 2023-05-26 13:54:54.243950 ma_fi-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.191257 ma_fi-0.1.2/ma_fi/
+-rw-rw-rw-   0        0        0      194 2023-05-26 13:53:27.000000 ma_fi-0.1.2/ma_fi/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-05-26 13:39:27.000000 ma_fi-0.1.2/ma_fi/download.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.236950 ma_fi-0.1.2/ma_fi.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 13:54:54.249026 ma_fi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-26 13:54:40.000000 ma_fi-0.1.2/setup.py
```

### Comparing `ma_fi-0.1.1/PKG-INFO` & `ma_fi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_fi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.1/ma_fi/download.py` & `ma_fi-0.1.2/ma_fi/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 import os
 import pandas as pd
 
 
 current_dir = os.path.abspath(os.path.dirname(__file__))
 parent_dir = os.path.abspath(os.path.join(current_dir,os.pardir)) #'C:\\Users\\Administrateur\\PycharmProjects\\mfinance'
-def download(self, name, start_date, end_date, period):
+
+package_dir = os.path.dirname(os.path.abspath(__file__))
+csv_path = os.path.join(package_dir, "ISIN_sectors_ma.csv")
+
+# List of available company names
+available_names = list(pd.read_csv(csv_path)["Instrument"])
+def download(name, start_date, end_date, period):
     # Check if the name is valid
-    if name not in self.available_names:
+    if name not in available_names:
         print("Invalid company name.")
         return
 
     # Check if the start date is prior to the oldest available date
     oldest_date = pd.Timestamp('2018-05-16')
     if pd.Timestamp(start_date) < oldest_date:
         print("Start date cannot be prior to 2018-05-16.")
```

### Comparing `ma_fi-0.1.1/ma_fi.egg-info/PKG-INFO` & `ma_fi-0.1.2/ma_fi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-fi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.1/setup.py` & `ma_fi-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='ma_fi',
-    version='0.1.1',
+    version='0.1.2',
     description='Library for accessing financial data of Moroccan stock exchange companies',
     author='Ali Talbi',
     author_email='alitalbi73@gmail.com',
     url='https://github.com/alitalbi/mfinance',
     packages=['ma_fi'],
     install_requires=[
         'pandas',
```


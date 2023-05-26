# Comparing `tmp/gimodules-0.0.97.tar.gz` & `tmp/gimodules-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimodules-0.0.97.tar", last modified: Fri Nov 25 09:50:37 2022, max compression
+gzip compressed data, was "gimodules-0.0.99.tar", last modified: Fri May 26 11:21:31 2023, max compression
```

## Comparing `gimodules-0.0.97.tar` & `gimodules-0.0.99.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.533174 gimodules-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2022-11-25 09:50:29.000000 gimodules-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-11-25 09:50:37.533174 gimodules-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      611 2022-11-25 09:50:29.000000 gimodules-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.529174 gimodules-0.0.97/gimodules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.529174 gimodules-0.0.97/gimodules/cloudconnect/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/cloudconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39063 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/cloudconnect/cloud_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    11740 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/cloudconnect/input_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/cloudconnect/mysql_connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/cloudconnect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.529174 gimodules-0.0.97/gimodules/domain/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/domain/csv.py
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/domain/data_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4289 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/domain/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.533174 gimodules-0.0.97/gimodules/py_q_station_connect_cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/py_q_station_connect_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8981 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/py_q_station_connect_cloud/gins_data_create_buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/py_q_station_connect_cloud/gins_data_get_buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)    15078 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/py_q_station_connect_cloud/py_q_station_connect_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.533174 gimodules-0.0.97/gimodules/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10958 2022-11-25 09:50:30.000000 gimodules-0.0.97/gimodules/visualization/definedplots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.529174 gimodules-0.0.97/gimodules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2022-11-25 09:50:37.000000 gimodules-0.0.97/gimodules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      873 2022-11-25 09:50:37.000000 gimodules-0.0.97/gimodules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 09:50:37.000000 gimodules-0.0.97/gimodules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-11-25 09:50:37.000000 gimodules-0.0.97/gimodules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-25 09:50:37.000000 gimodules-0.0.97/gimodules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-25 09:50:37.533174 gimodules-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2022-11-25 09:50:30.000000 gimodules-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:37.533174 gimodules-0.0.97/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 09:50:30.000000 gimodules-0.0.97/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      430 2022-11-25 09:50:30.000000 gimodules-0.0.97/tests/test_capital.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.947564 gimodules-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 11:21:26.000000 gimodules-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-26 11:21:31.947564 gimodules-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-26 11:21:26.000000 gimodules-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.943563 gimodules-0.0.99/gimodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.943563 gimodules-0.0.99/gimodules/cloudconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/cloudconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40659 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/cloudconnect/cloud_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/cloudconnect/input_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/cloudconnect/mysql_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/cloudconnect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.947564 gimodules-0.0.99/gimodules/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/domain/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/domain/data_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/domain/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.947564 gimodules-0.0.99/gimodules/py_q_station_connect_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/py_q_station_connect_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/py_q_station_connect_cloud/gins_data_create_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/py_q_station_connect_cloud/gins_data_get_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/py_q_station_connect_cloud/py_q_station_connect_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.947564 gimodules-0.0.99/gimodules/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-26 11:21:26.000000 gimodules-0.0.99/gimodules/visualization/definedplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.943563 gimodules-0.0.99/gimodules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-26 11:21:31.000000 gimodules-0.0.99/gimodules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 11:21:31.000000 gimodules-0.0.99/gimodules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:21:31.000000 gimodules-0.0.99/gimodules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 11:21:31.000000 gimodules-0.0.99/gimodules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 11:21:31.000000 gimodules-0.0.99/gimodules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:21:31.947564 gimodules-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-26 11:21:26.000000 gimodules-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:31.947564 gimodules-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:21:26.000000 gimodules-0.0.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-26 11:21:26.000000 gimodules-0.0.99/tests/test_capital.py
```

### Comparing `gimodules-0.0.97/LICENSE` & `gimodules-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/PKG-INFO` & `gimodules-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimodules
-Version: 0.0.97
+Version: 0.0.99
 Summary: Python package to deliver a Gantner cloud interface
 Author: gimodules devs
 Author-email: 
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gimodules-0.0.97/README.md` & `gimodules-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/cloudconnect/cloud_request.py` & `gimodules-0.0.99/gimodules/cloudconnect/cloud_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 import pandas as pd
 import json 
 import re
 import uuid
 import time 
 import logging
+import pytz
 
 from dataclasses import dataclass
 from typing import Type, List, Dict, Tuple, Optional, Union, Any
 from requests.auth import HTTPBasicAuth 
 from enum import Enum
 from dateutil import tz
 
@@ -76,14 +77,15 @@
         self.pw = ""
         self.login_token = None
         self.refresh_token = None
         self.streams = None
         self.stream_variabels = None
         self.query = ""
         self.request_measurement_res = None
+        self.timezone = 'Europe/Vienna'
 
         # enums 
         self.resolutions = Resolution 
         self.units = None
 
         # importer data
         self.import_session_res_udbf = None
@@ -299,25 +301,26 @@
             s = s+f"""
                 {i} {{
                     {agg}
                 }}
             """
         return s
 
-    def get_var_data(self, sid:str, index_list:List, start_date:str, end_date:str, resolution:str = 'nanos'):
+    def get_var_data(self, sid:str, index_list:List, start_date:str, end_date:str, resolution:str = 'nanos', custom_column_names:list = []):
         """Returns a np.matrix of data and pandas df with timestamps and values directly from a data stream
 
         Args:
             sid (str): stream_id
-            index_list (list): channel_index e.g. ["a10", "a11"]
+            index_list (list[str]): channel_index e.g. ["a10", "a11"]
             start_date (str): format: YYYY-MM-DD HH:MM:SS
             end_date (str): format: YYYY-MM-DD HH:MM:SS
             resolution (str, optional): 'MONTH','WEEK','DAY','HOUR','QUARTER_HOUR','MINUTE','SECOND','HZ10','HZ100','KHZ','KHZ10','nanos'
                 The available resolutions are accessible via the attribute ".resolutions". 
                 Do not forget at the end the .values  Defaults to 'nanos'.
+            custom_column_names (list[str]): 'use custom names for the df columns: ["Time", "your_col_name_1", "your_col_name_2", ...]'
 
         Returns:
             pandas.df: dataframe
         """
 
         tss = str(self.convert_datetime_to_unix(start_date))
         tse = str(self.convert_datetime_to_unix(end_date))
@@ -380,16 +383,22 @@
                     last_none=none_index[0][-1]
                     if last_none==len(self.data)-1:
                         self.data=self.data[0:first_none-1,:]
                     else:    
                         self.data=self.data[last_none+1:-1,:]
 
                 ### create pandas df
-                self.df = pd.DataFrame(self.data, columns=self.__get_column_names(sid, index_list))
+                if len(custom_column_names) == 0: # add option for custom names
+                    self.df = pd.DataFrame(self.data, columns=self.__get_column_names(sid, index_list))
+                else: 
+                    self.df = pd.DataFrame(self.data, columns=custom_column_names)
+
                 self.df['Time'] = pd.to_datetime(self.df['Time'], unit='ms')
+                self.__convert_df_time_from_utc_to_tz()
+                
                 return self.df 
             elif res.status_code == 401 or res.status_code == 403:
                 logging.info("Token expired. Renewing...")
                 self.refresh_access_token()
                 return self.get_var_data(sid, index_list, start_date, end_date, resolution)
             # Show error Message from Server
             else: 
@@ -513,34 +522,66 @@
         if res != None:
             for i in index_list: 
                 for x in res:
                     if x.index == i:
                         col_names.append(x.name)
             return col_names
         return None 
-
-    @staticmethod
-    def convert_datetime_to_unix(datetime:str):
-        """staticmethod for converting timestamps to UTC
+    
+    
+    def convert_datetime_to_unix(self, datetime:str):
+        """converting timestamps from the selected tz to UTC
 
         Args:
             datetime (str): required date format '%Y-%m-%d %H:%M:%S'
 
         Returns:
             int: UNIX timestamp
         """
         try: 
-            date_time_obj = dt.datetime.strptime(datetime, '%Y-%m-%d %H:%M:%S')
-            timestamp_utc = date_time_obj.replace(tzinfo=tz.gettz('UTC'))
-            timestamp_local = timestamp_utc.astimezone(tz.gettz('Europe / Paris'))
-            timestamp= int(dt.datetime.timestamp(timestamp_local)) * 1000 
-            return timestamp
+            current_tz = pytz.timezone(self.timezone)
+   
+            # Create a timezone-aware datetime object with DST information
+            datetime_obj = current_tz.localize(dt.datetime.strptime(datetime, '%Y-%m-%d %H:%M:%S'))
+
+            # Convert to UTC timezone
+            utc_obj = datetime_obj.astimezone(pytz.utc)
+
+            # Convert UTC datetime object to Unix timestamp
+            return int(utc_obj.timestamp()) * 1000
         except Exception as err:
             logging.error("Fehler beim konvertieren des Zeitstempels:", dt.datetime.now, err)
 
+
+    def set_timezone(self, timezone:str = 'Europe/Vienna'): 
+        if self.__validate_timezone(timezone): 
+            self.timezone = timezone
+            print("Now using timezone:", timezone)
+        else:
+            logging.warning('Timezone do not exist!')
+
+
+    def __validate_timezone(timezone):
+        try:
+            pytz.timezone(timezone)
+            return True
+        except pytz.UnknownTimeZoneError:
+            return False
+    
+    
+    def __convert_df_time_from_utc_to_tz(self): 
+        """ Converts the time stamps of the dataframe to the desired time zone. The default time zone is Vienna. The GI.Cloud always delivers the data in UTC.
+            Defaults to 'Europe/Vienna'.
+        """
+        try: 
+            self.df['Time'] = self.df['Time'].dt.tz_localize('UTC')
+            self.df['Time'] = self.df['Time'].dt.tz_convert(self.timezone)
+        except Exception as err:
+            logging.error("Error:", dt.datetime.now, err)
+
     def get_measurement_limit(self, sid:str, limit:str): 
         """
              'get measurement between time start and time stop'
 
         Args:
             sid (str): Stream Id
             limit (str):
```

### Comparing `gimodules-0.0.97/gimodules/cloudconnect/input_handler.py` & `gimodules-0.0.99/gimodules/cloudconnect/input_handler.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/cloudconnect/mysql_connect.py` & `gimodules-0.0.99/gimodules/cloudconnect/mysql_connect.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/cloudconnect/utils.py` & `gimodules-0.0.99/gimodules/cloudconnect/utils.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/domain/csv.py` & `gimodules-0.0.99/gimodules/domain/csv.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/domain/data_manipulator.py` & `gimodules-0.0.99/gimodules/domain/data_manipulator.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/domain/domain.py` & `gimodules-0.0.99/gimodules/domain/domain.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/py_q_station_connect_cloud/gins_data_create_buffer.py` & `gimodules-0.0.99/gimodules/py_q_station_connect_cloud/gins_data_create_buffer.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/py_q_station_connect_cloud/gins_data_get_buffer.py` & `gimodules-0.0.99/gimodules/py_q_station_connect_cloud/gins_data_get_buffer.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/py_q_station_connect_cloud/py_q_station_connect_cloud.py` & `gimodules-0.0.99/gimodules/py_q_station_connect_cloud/py_q_station_connect_cloud.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules/visualization/definedplots.py` & `gimodules-0.0.99/gimodules/visualization/definedplots.py`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/gimodules.egg-info/PKG-INFO` & `gimodules-0.0.99/gimodules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimodules
-Version: 0.0.97
+Version: 0.0.99
 Summary: Python package to deliver a Gantner cloud interface
 Author: gimodules devs
 Author-email: 
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gimodules-0.0.97/gimodules.egg-info/SOURCES.txt` & `gimodules-0.0.99/gimodules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gimodules-0.0.97/setup.py` & `gimodules-0.0.99/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.97'
+VERSION = '0.0.99'
 DESCRIPTION = 'Python package to deliver a Gantner cloud interface'
 LONG_DESCRIPTION = ''
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
     
 # Setting up
```


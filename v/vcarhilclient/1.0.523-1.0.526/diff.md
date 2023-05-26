# Comparing `tmp/vcarhilclient-1.0.523.tar.gz` & `tmp/vcarhilclient-1.0.526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.523.tar", last modified: Tue May 23 10:17:15 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.526.tar", last modified: Fri May 26 03:15:04 2023, max compression
```

## Comparing `vcarhilclient-1.0.523.tar` & `vcarhilclient-1.0.526.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.895763 vcarhilclient-1.0.523/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.523/LICENSE
--rw-rw-rw-   0        0        0     2644 2023-05-23 10:17:15.895763 vcarhilclient-1.0.523/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.523/README.md
--rw-rw-rw-   0        0        0       86 2023-05-23 10:17:15.896763 vcarhilclient-1.0.523/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-05-23 10:03:09.000000 vcarhilclient-1.0.523/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.880306 vcarhilclient-1.0.523/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-06 03:10:40.000000 vcarhilclient-1.0.523/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.523/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.523/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50292 2023-05-23 10:04:11.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    14731 2023-05-23 05:14:59.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    12030 2023-05-23 05:14:01.000000 vcarhilclient-1.0.523/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.523/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.523/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.523/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-23 10:17:15.893766 vcarhilclient-1.0.523/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2644 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 10:17:15.000000 vcarhilclient-1.0.523/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.891093 vcarhilclient-1.0.526/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.526/LICENSE
+-rw-rw-rw-   0        0        0     2596 2023-05-26 03:15:04.891093 vcarhilclient-1.0.526/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.526/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-26 03:15:04.892093 vcarhilclient-1.0.526/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-05-26 03:13:26.000000 vcarhilclient-1.0.526/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.877619 vcarhilclient-1.0.526/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.526/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.526/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.526/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50548 2023-05-26 02:40:36.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    12136 2023-05-24 08:09:40.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.526/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.526/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.526/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.889105 vcarhilclient-1.0.526/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2596 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.523/LICENSE` & `vcarhilclient-1.0.526/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/PKG-INFO` & `vcarhilclient-1.0.526/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.523
+Version: 1.0.526
 Summary: vcarhilclient
-Home-page: UNKNOWN
+Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
-
-
```

### Comparing `vcarhilclient-1.0.523/README.md` & `vcarhilclient-1.0.526/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/setup.py` & `vcarhilclient-1.0.526/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.523",
+    version="1.0.526",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.523/vcarhilclient/Enums.py` & `vcarhilclient-1.0.526/vcarhilclient/Enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     MRT_VRPC_ERR_SVC_MALLOC_FAIL = -1022,
     MRT_VRPC_ERR_SVC_IN_PROGRESS = -1021,
     MRT_VRPC_ERR_RESP_BUF_SIZE_INVALID = -1020,
     MRT_VRPC_ERR_TIMEOUT = -1019,
     MRT_VRPC_ERR_GENERIC_ERROR = -1018,
     MRT_VRPC_ERR_SVC_SIGNATURE_INVALID = -1017,
     MRT_VRPC_ERR_INVALID_ARG = -1016,
-    MRT_VRPC_ERR_CLI_SVC_NAME_INVALID = -1015,
+    MRT_VRPC_ERR_CLI_ENV_NAME_INVALID = -1015,
     MRT_VRPC_ERR_CLI_SOCK_INVALID = -1014,
     MRT_VRPC_ERR_CLI_INVALID_DATA_SIZE = -1013,
     MRT_VRPC_ERR_CLI_INVALID_FN_ID = -1012,
     MRT_VRPC_ERR_CLI_INVALID_SN = -1011,
     MRT_VRPC_ERR_CLI_INVALID_RESP = -1010,
     MRT_VRPC_ERR_CLI_RECV_FAIL = -1009,
     MRT_VRPC_ERR_CLI_SEND_FAIL = -1008,
```

### Comparing `vcarhilclient-1.0.523/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.526/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.526/vcarhilclient/kunyi_mrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,35 +907,41 @@
         mrt_lib.mrt_gen_clr_port_event.restype = mrt_status_t
         error_code = mrt_lib.mrt_gen_clr_port_event(self.context, en_pointer, c_uint64(gen_handle), c_uint32(port_index))
         return error_code
 
     def gen_write_port(self, env_name, gen_handle, port_index, data, data_type, time_interval_ms):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
-        # dt = data.encode('utf-8')
-        python_bytes = kunyi_util.data_to_bytes(data_type, data, 1)
+        python_bytes = kunyi_util.data_to_bytes(data_type, data, len(data))
         arr = bytearray.fromhex(python_bytes.hex())
         char_array = c_char * len(arr)
         buf_c = char_array.from_buffer(arr)
 
         mrt_lib.mrt_gen_write_port.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32,c_void_p,c_uint32,c_uint32]
         mrt_lib.mrt_gen_write_port.restype = c_int32
         res = mrt_lib.mrt_gen_write_port(self.context, en_pointer, c_uint64(gen_handle), c_uint32(port_index)
                                                     ,buf_c, len(arr), c_uint32(time_interval_ms))
         return res
 
-    def gen_write_queue(self, env_name, gen_handle, port_index,interval_and_data,data_size,item_number):
+    def gen_write_queue(self, env_name, gen_handle, port_index, data):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
-        dt = interval_and_data.encode('utf-8')
-        data_p = c_void_p(dt)
-        mrt_lib.mrt_gen_write_queue.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32,c_void_p,c_uint32,c_uint32]
+        python_bytes = b''
+        for i in range(len(data)):
+            python_bytes = python_bytes + kunyi_util.data_to_bytes("UInt32", data[i]["interval"], 1)
+            python_bytes = python_bytes + kunyi_util.data_to_bytes(data[i]["data_type"], data[i]["data_value"], 1)
+
+        arr = bytearray.fromhex(python_bytes.hex())
+        char_array = c_char * len(arr)
+        buf_c = char_array.from_buffer(arr)
+
+        mrt_lib.mrt_gen_write_queue.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32, c_void_p, c_uint32, c_uint32]
         mrt_lib.mrt_gen_write_queue.restype = c_int32
         res = mrt_lib.mrt_gen_write_queue(self.context, en_pointer, c_uint64(gen_handle), c_uint32(port_index)
-                                                    ,data_p,c_uint32(data_size),c_uint32(item_number))
+                                         , buf_c, 8, c_uint32(len(data)))
         return res
 
     def gen_start(self, env_name, gen_handle):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
         mrt_lib.mrt_gen_start.argtypes = [c_void_p, c_char_p, c_uint64]
         mrt_lib.mrt_gen_start.restype = mrt_status_t
@@ -1029,11 +1035,11 @@
         mrt_lib.mrt_version.argtypes = [c_void_p]
         mrt_lib.mrt_version.restype = c_char_p
         version = mrt_lib.mrt_version(buf_c)
         return version.decode('utf-8')
 
     def mrtd_version(self):
 
-        mrt_lib.mrtd_version.argtypes = [c_void_p]
-        mrt_lib.mrtd_version.restype = c_char_p
-        version = mrt_lib.mrtd_version(self.context)
+        mrt_lib.mrtd_verison.argtypes = [c_void_p]
+        mrt_lib.mrtd_verison.restype = c_char_p
+        version = mrt_lib.mrtd_verison(self.context)
         return version.decode('utf-8')
```

### Comparing `vcarhilclient-1.0.523/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.526/vcarhilclient/kunyi_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os,zipfile
 import json
 import codecs
-
+r=os.path.abspath(os.path.dirname(__file__))
+rootpath= os.path.split(r)[0]
+sys.path.append(rootpath)
 from vcarhilclient.Enums import mrt_port_type_t
 from vcarhilclient.kunyi_util import kunyi_util
 
 
 class instance_detail():
     def __init__(self):
         self.xpaths = {
@@ -19,15 +21,15 @@
 
 
 class hil_project():
 
     def __init__(self, ipr_path):
         if not os.path.isfile(ipr_path):
             raise Exception("Invalid ipr path")
-        with open(ipr_path) as ipr_file:
+        with open(ipr_path,encoding='utf-8') as ipr_file:
             try:
                 ipr_json = json.load(ipr_file)
             except Exception as ex:
                 raise Exception("ipr is not a valid json file")
         self.project_name = ipr_json["ProjectName"]
         self.version = ipr_json["Version"]
         self.hil_json_path = os.path.join(os.path.dirname(ipr_path), ipr_json["HILSystemFilePath"])
@@ -50,34 +52,40 @@
                 self.model_meta_files[item["ModelMetaFile"]] = item
                 self.modelPath[item["ModelMetaFile"]] = os.path.join(os.path.dirname(ipr_path),item["File"]["Path"])
             pass
 
         except Exception as ex:
             raise Exception("hil file content is not correct")
 
-    def get_Calibrations(self,instance,signal_type,cal_type,signal_name):
+    def get_Calibrations(self, instance, signal_type, cal_type, signal_name):
         instance_is_found = False
-        signal_name_is_found =False
-        cal_type_is_found =False
-        st,stid = self.get_signalType(signal_type)
-        for k , v in self.modelPath.items():
+        signal_name_is_found = False
+        cal_type_is_found = False
+        st, stid = self.get_signalType(signal_type)
+        for k, v in self.modelPath.items():
             if instance == k:
                 instance_is_found = True
                 with open(v) as f:
                     try:
                         instance_json = json.load(f)
                     except Exception as ex:
                         raise Exception(f"{v} is not a valid json file")
-                    for cal_t,cal_v in instance_json[st].items():
+                    for cal_t, cal_v in instance_json[st].items():
                         if cal_t.lower() == cal_type.lower():
                             cal_type_is_found = True
                             for cal in cal_v:
                                 if signal_name == cal["Name"]:
                                     signal_name_is_found = True
-                                    return signal_name , stid
+                                    if cal_type.lower() in ["curve", "map"]:
+                                        data_type = cal["FunValue"]["DataType"]
+                                    elif cal_type.lower() in ["scalar"]:
+                                        data_type = cal["Value"]["DataType"]
+                                    elif cal_type.lower() in ["vector"]:
+                                        data_type = cal["Values"]["DataType"]
+                                    return signal_name, stid, data_type
         if not instance_is_found:
             raise Exception(f"not found {instance},Please check the json parameters'var_instance'")
         if not cal_type_is_found:
             raise Exception(f"not found {cal_type},Please check the json parameters'var_cal_type'")
         if not signal_name_is_found:
             raise Exception(f"not found {signal_name},Please check the json parameters'var_signal_name'")
```

### Comparing `vcarhilclient-1.0.523/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.526/vcarhilclient/kunyi_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import struct
 import sys
 from decimal import Decimal
 from ctypes import *
 import zipfile
 import os
 import subprocess
+r=os.path.abspath(os.path.dirname(__file__))
+rootpath= os.path.split(r)[0]
+sys.path.append(rootpath)
+
 from vcarhilclient.Enums import *
 import collections.abc
 
 class kunyi_util():
     @staticmethod
     def get_signal_bytes_length(signal_type, item_count=1, struct_detail=None, **sub_struct_detail):
         type_dict = {"Int8": 1,
```

### Comparing `vcarhilclient-1.0.523/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.526/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.526/vcarhilclient/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.526/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.523/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.526/vcarhilclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.523
+Version: 1.0.526
 Summary: vcarhilclient
-Home-page: UNKNOWN
+Home-page: 
 Author: vcarsystem
 Author-email: service@vcarsystem.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
-
-
```


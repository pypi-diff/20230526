# Comparing `tmp/simply_nwb-0.0.6.tar.gz` & `tmp/simply_nwb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.6.tar", last modified: Tue May 23 19:27:04 2023, max compression
+gzip compressed data, was "simply_nwb-0.0.7.tar", last modified: Fri May 26 15:53:59 2023, max compression
```

## Comparing `simply_nwb-0.0.6.tar` & `simply_nwb-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.548498 simply_nwb-0.0.6/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-23 19:27:04.547499 simply_nwb-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-23 19:27:04.548498 simply_nwb-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.535445 simply_nwb-0.0.6/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.538655 simply_nwb-0.0.6/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.546498 simply_nwb-0.0.6/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/labjack.py
--rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/plaintext.py
--rw-rw-rw-   0        0        0     3437 2023-05-23 16:16:41.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.6/simply_nwb/acquisition/tools/yaml.py
--rw-rw-rw-   0        0        0    24781 2023-05-23 18:43:23.000000 simply_nwb-0.0.6/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0    10706 2023-05-23 18:43:23.000000 simply_nwb-0.0.6/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.547499 simply_nwb-0.0.6/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.6/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     5540 2023-05-23 18:31:52.000000 simply_nwb-0.0.6/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 19:27:04.538655 simply_nwb-0.0.6/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-23 19:27:04.000000 simply_nwb-0.0.6/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:59.001367 simply_nwb-0.0.7/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-05-26 15:53:59.000367 simply_nwb-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:53:59.001367 simply_nwb-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-05-26 15:53:51.000000 simply_nwb-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.988346 simply_nwb-0.0.7/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.992344 simply_nwb-0.0.7/simply_nwb/acquisition/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.998361 simply_nwb-0.0.7/simply_nwb/acquisition/tools/
+-rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/blackrock.py
+-rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/labjack.py
+-rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/plaintext.py
+-rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/yaml.py
+-rw-rw-rw-   0        0        0    24781 2023-05-23 18:43:23.000000 simply_nwb-0.0.7/simply_nwb/simple_nwb.py
+-rw-rw-rw-   0        0        0    12850 2023-05-25 20:43:09.000000 simply_nwb-0.0.7/simply_nwb/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.999367 simply_nwb-0.0.7/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0       31 2023-05-25 16:13:35.000000 simply_nwb-0.0.7/simply_nwb/transferring/__init__.py
+-rw-rw-rw-   0        0        0     7693 2023-05-26 15:53:17.000000 simply_nwb-0.0.7/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:59.000367 simply_nwb-0.0.7/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     7110 2023-05-25 18:00:05.000000 simply_nwb-0.0.7/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.991345 simply_nwb-0.0.7/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.6/LICENSE` & `simply_nwb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/PKG-INFO` & `simply_nwb-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.6/setup.py` & `simply_nwb-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/csv.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/labjack.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/mp4.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/mp4.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/acquisition/tools/plaintext.py` & `simply_nwb-0.0.7/simply_nwb/acquisition/tools/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/simple_nwb.py` & `simply_nwb-0.0.7/simply_nwb/simple_nwb.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.6/simply_nwb/testing.py` & `simply_nwb-0.0.7/simply_nwb/testing.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 from simply_nwb.acquisition.tools import csv_load_dataframe, yaml_read_file
 from simply_nwb.acquisition.tools import labjack_load_file
 from simply_nwb.acquisition.tools import plaintext_metadata_read
 from simply_nwb.acquisition.tools import blackrock_load_data, blackrock_all_spiketrains
 from simply_nwb.util import panda_df_to_dyn_table
 from simply_nwb import SimpleNWB
 import pendulum
+import os
+import shutil
 import numpy as np
 import pandas as pd
 
+from transferring import NWBTransfer
 
 # Data is available on Google Drive, as Spencer for access
 blackrock_nev_filename = "../data/wheel_4p3_lSC_2001.nev"
 perg_filename = "../data/pg1_A_raw.TXT"
 perg_folder = "../data/pg_folder"
 labjack_filename = "../data/labjack_data.dat"
 labjack_filename2 = "../data/labjack_data2.dat"
@@ -26,14 +29,15 @@
 tif_subfolder_kwargs = {"parent_folder": "../data/tifs/subfolder_formatted",
                         "subfolder_glob": "file*", "file_glob": "Image.tif"}
 tif_single_filename = "../data/tifs/subfolder_formatted/file/Image.tif"
 # Note: This CSV isn't formatted correctly so it will look weird when loaded
 csv_filename = "../data/20230414_unitR2_session002_leftCam-0000DLC_resnet50_licksNov3shuffle1_1030000.csv"
 dict_data = {"data1": [1, 2, 3, 4, 5], "data2": ["a", "b", "c", "d", "e"]}
 dict_data_uneven_cols = {"data1": [1, 2, 3], "data2": ["a", "b", "c", "d", "e"], "aa": 5}
+nwb_save_filename = "../data/nwb_test.nwb"
 
 
 def nwb_gen():
     return SimpleNWB.create_nwb(
         # Required
         session_description="Mouse cookie eating session",
         # Subtract 1 year so we don't run into the 'NWB start time is at a greater date than current' issue
@@ -258,22 +262,92 @@
 def util_test():
     # Note: This CSV isn't formatted correctly, so it will look weird when loaded
     r = panda_df_to_dyn_table(pd_df=csv_load_dataframe(csv_filename), table_name="test_table",
                               description="test description")
     tw = 2
 
 
+def pkl_test():
+    import pickle
+    fn = "../data/output.pkl"
+    fp = open(fn, "rb")
+    data = pickle.load(fp)
+    nwb = nwb_gen()
+    SimpleNWB.processing_add_dict(
+            nwb,
+            processed_name="asdf",
+            processed_description="asdf",
+            data_dict=data,
+            uneven_columns=True)
+    # nwb.processing["misc"]["asdf_eyePositionUncorrected"]["eyePositionUncorrected"].data[:]
+    tw = 2
+
+
+def ephys_test():
+    from open_ephys.analysis import Session
+
+
+def transfer_nwb_test():
+    nwb = nwb_gen()
+    SimpleNWB.write(nwb, nwb_save_filename)
+    transfer0 = NWBTransfer(
+        nwb_file_location=nwb_save_filename,
+        raw_data_folder_location=perg_folder,
+        transfer_location_root="../data/",
+        lab_name="MyLabName",
+        project_name="test_project",
+        session_name="session0"
+    )
+    transfer0.upload()
+
+    transfer1 = NWBTransfer(
+        nwb_file_location=nwb_save_filename,
+        raw_data_folder_location=perg_folder,
+        transfer_location_root="../data/",
+        lab_name="MyLabName",
+        project_name="test_project",
+        session_name="session1",
+        delete_zipped_raw_data_on_upload_finish=True
+    )
+    transfer1.upload(
+        zip_location_override=transfer0.zip_file_location
+    )
+    print("Transfer 1 finished")
+
+    try:
+        NWBTransfer(
+            nwb_file_location=nwb_save_filename,
+            raw_data_folder_location=perg_folder,
+            transfer_location_root="../data/",
+            lab_name="MyLabName",
+            project_name="test_project",
+            session_name="session1"
+        )
+        raise Exception("Test NWBTransfer transfer_fail should fail, but didn't!")
+    except ValueError as e:
+        tw = 2
+        # Test is supposed to fail
+        pass
+
+    print("Clearing test folder and related test things")
+    shutil.rmtree("../data/MyLabName")
+    os.mkdir("../data/MyLabName")
+
+
 if __name__ == "__main__":
     # util_test()
     # blackrock_test()
     # csv_test()
     # plaintext_metadata_test()
     # yaml_test()
     # mp4_test()
     # tif_test()
+    # pkl_test()
+    transfer_nwb_test()
+
 
     funcs_to_assert = [
         # nwb_nev,
         # nwb_perg,
         # nwb_labjack,
         # nwb_two_photon,
         # nwb_processing_module_df,
```

### Comparing `simply_nwb-0.0.6/simply_nwb/util.py` & `simply_nwb-0.0.7/simply_nwb/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -164,7 +164,65 @@
             starting_time=start_time,
             rate=sampling_rate,
             description=f"column {col_name} {description}",
             comments=comments,
         ))
 
     return timeseries_list
+
+
+def _print(val, do_print=True):
+    # Helper function
+    if do_print:
+        print(val, flush=True)
+
+
+def is_camel_case(string, do_print=True):
+    """
+    Check if the given string is in CamelCase
+
+
+    :param string: string to check
+    :param do_print: if False, will not print out anything
+    :return: bool if str is CamelCase
+    """
+
+    reg = re.compile("^[a-zA-Z]*$")
+    matched = reg.match(string)
+    if not matched:
+        _print(f"String '{string}' does not match CamelCase regex!", do_print)
+        return False
+    if not string[0].isupper():
+        _print(f"String '{string}' must start with a capital letter!", do_print)
+        return False
+    return True
+
+
+def is_snake_case(string, do_print=True):
+    """
+    Checks if the given string is snake_case
+
+    :param string: string to check if is snake_case
+    :param do_print: if False, will not print anything
+    :return: bool of if the string is snake_case
+    """
+
+    reg = re.compile("^[a-z_]*$")
+    matched = reg.match(string)
+    if not matched:
+        _print(f"String '{string}' does not match snake_case regex!", do_print)
+        return False
+    return True
+
+
+def is_filesystem_safe(string):
+    """
+    Generic check function for if a string is filesystem safe, limits to a-z A-Z 0-9 '_' '-'
+
+    :param string: String to check
+    :return: True if the given string matches the regex
+    """
+    reg = re.compile(r"^[a-zA-Z_\-0-9]*$")
+    match = reg.match(string)
+    if not match:
+        return False
+    return True
```

### Comparing `simply_nwb-0.0.6/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.0.7/simply_nwb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.6/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.0.7/simply_nwb.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 simply_nwb/acquisition/tools/csv.py
 simply_nwb/acquisition/tools/labjack.py
 simply_nwb/acquisition/tools/mp4.py
 simply_nwb/acquisition/tools/p_erg.py
 simply_nwb/acquisition/tools/plaintext.py
 simply_nwb/acquisition/tools/tif.py
 simply_nwb/acquisition/tools/yaml.py
+simply_nwb/transferring/__init__.py
+simply_nwb/transferring/nwb_transfer.py
 simply_nwb/transforms/__init__.py
```


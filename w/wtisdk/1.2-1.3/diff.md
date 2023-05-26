# Comparing `tmp/wtisdk-1.2.tar.gz` & `tmp/wtisdk-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.2.tar", last modified: Fri May 26 20:16:23 2023, max compression
+gzip compressed data, was "wtisdk-1.3.tar", last modified: Fri May 26 21:31:24 2023, max compression
```

## Comparing `wtisdk-1.2.tar` & `wtisdk-1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.736906 wtisdk-1.2/
--rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:16:23.736718 wtisdk-1.2/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      648 2023-05-26 20:13:15.000000 wtisdk-1.2/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-05-26 20:16:23.737001 wtisdk-1.2/setup.cfg
--rw-r--r--   0 MTeke1     (502) staff       (20)     2152 2023-05-26 20:16:17.000000 wtisdk-1.2/setup.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.734009 wtisdk-1.2/wtisdk/
--rw-r--r--   0 MTeke1     (502) staff       (20)       35 2023-05-26 20:16:12.000000 wtisdk-1.2/wtisdk/__init__.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.736211 wtisdk-1.2/wtisdk/tests/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-05-26 17:07:10.000000 wtisdk-1.2/wtisdk/tests/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      714 2023-05-26 19:17:23.000000 wtisdk-1.2/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 MTeke1     (502) staff       (20)    37138 2023-05-26 19:02:26.000000 wtisdk-1.2/wtisdk/wtisdk.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.735914 wtisdk-1.2/wtisdk.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      256 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)       17 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/requires.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        7 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 21:31:15.000000 wtisdk-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 21:31:24.577357 wtisdk-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-26 21:31:15.000000 wtisdk-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:31:24.581357 wtisdk-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 21:31:15.000000 wtisdk-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37138 2023-05-26 21:31:15.000000 wtisdk-1.3/wtisdk/wtisdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:31:24.577357 wtisdk-1.3/wtisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 21:31:24.000000 wtisdk-1.3/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.2/PKG-INFO` & `wtisdk-1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.2
+Version: 1.3
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
-Description: 
-                                WTI SDK: Python SDK for interacting with WTI devices
-        
-                                The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
-        
-                                Features:
-                                - Retrieve the status information of WTI devices
-                                - Add new entries to the device's operational data
-                                - Modify existing operational data entries
-                                - Update the device's configuration settings
-                                - Get detailed information about the device's configuration
-                                - Perform various other actions on both operational and configuration levels
-        
-                                With the WTI SDK, developers can streamline their integration with WTI devices, automate management tasks, and build robust applications that leverage the full capabilities of WTI devices.
-        
-                                For usage instructions and examples, please refer to the documentation available at: https://github.com/melihteke/wtisdk
-        
-                                For any questions or support, feel free to contact us at me@mteke.com.
-                                
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+                        WTI SDK: Python SDK for interacting with WTI devices
+
+                        The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
+
+                        Features:
+                        - Retrieve the status information of WTI devices
+                        - Add new entries to the device's operational data
+                        - Modify existing operational data entries
+                        - Update the device's configuration settings
+                        - Get detailed information about the device's configuration
+                        - Perform various other actions on both operational and configuration levels
+
+                        With the WTI SDK, developers can streamline their integration with WTI devices, automate management tasks, and build robust applications that leverage the full capabilities of WTI devices.
+
+                        For usage instructions and examples, please refer to the documentation available at: https://github.com/melihteke/wtisdk
+
+                        For any questions or support, feel free to contact us at me@mteke.com.
+                        
+
```

### Comparing `wtisdk-1.2/setup.py` & `wtisdk-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wtisdk',
-    version='1.2',
+    version='1.3',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description='''
                         WTI SDK: Python SDK for interacting with WTI devices
 
                         The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
```

### Comparing `wtisdk-1.2/wtisdk/wtisdk.py` & `wtisdk-1.3/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.2/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.3/wtisdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.2
+Version: 1.3
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
-Description: 
-                                WTI SDK: Python SDK for interacting with WTI devices
-        
-                                The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
-        
-                                Features:
-                                - Retrieve the status information of WTI devices
-                                - Add new entries to the device's operational data
-                                - Modify existing operational data entries
-                                - Update the device's configuration settings
-                                - Get detailed information about the device's configuration
-                                - Perform various other actions on both operational and configuration levels
-        
-                                With the WTI SDK, developers can streamline their integration with WTI devices, automate management tasks, and build robust applications that leverage the full capabilities of WTI devices.
-        
-                                For usage instructions and examples, please refer to the documentation available at: https://github.com/melihteke/wtisdk
-        
-                                For any questions or support, feel free to contact us at me@mteke.com.
-                                
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+                        WTI SDK: Python SDK for interacting with WTI devices
+
+                        The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
+
+                        Features:
+                        - Retrieve the status information of WTI devices
+                        - Add new entries to the device's operational data
+                        - Modify existing operational data entries
+                        - Update the device's configuration settings
+                        - Get detailed information about the device's configuration
+                        - Perform various other actions on both operational and configuration levels
+
+                        With the WTI SDK, developers can streamline their integration with WTI devices, automate management tasks, and build robust applications that leverage the full capabilities of WTI devices.
+
+                        For usage instructions and examples, please refer to the documentation available at: https://github.com/melihteke/wtisdk
+
+                        For any questions or support, feel free to contact us at me@mteke.com.
+                        
+
```


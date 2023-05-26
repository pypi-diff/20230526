# Comparing `tmp/clearblade-cloud-iot-2.0.1.tar.gz` & `tmp/clearblade-cloud-iot-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clearblade-cloud-iot-2.0.1.tar", last modified: Fri May 26 17:18:48 2023, max compression
+gzip compressed data, was "dist/clearblade-cloud-iot-2.0.2.tar", last modified: Fri May 26 17:24:38 2023, max compression
```

## Comparing `clearblade-cloud-iot-2.0.1.tar` & `clearblade-cloud-iot-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)    22073 2023-05-26 17:16:49.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/device_types.py
--rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/developer_tests.py
--rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/resources.py
--rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/registry.py
--rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-20 17:29:53.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/config_manager.py
--rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/registry_types.py
--rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/http_client.py
--rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/config.py
--rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-23 13:52:19.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/devices.py
--rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/client.py
--rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/pagers.py
--rw-rw-r--   0 root         (0) root         (0)     3217 2023-05-26 17:16:49.000000 clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/iot/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/iot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/iot_v1/py.typed
--rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.1/google/cloud/iot_v1/gapic_metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/unit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/unit/gapic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/unit/gapic/iot_v1/
--rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/unit/gapic/iot_v1/test_device_manager.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/unit/gapic/iot_v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/system/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/system/gapic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/tests/system/gapic/v1/
--rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/system/gapic/v1/test_system_device_manager_v1.py
--rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.1/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2835 2023-05-26 17:17:53.000000 clearblade-cloud-iot-2.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 17:18:48.000000 clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/namespace_packages.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)    22125 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/device_types.py
+-rw-rw-r--   0 root         (0) root         (0)    13659 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/developer_tests.py
+-rw-rw-r--   0 root         (0) root         (0)     6471 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/resources.py
+-rw-rw-r--   0 root         (0) root         (0)     9331 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     7497 2023-05-20 17:29:53.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8201 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry_types.py
+-rw-rw-r--   0 root         (0) root         (0)     3742 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8386 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/http_client.py
+-rw-rw-r--   0 root         (0) root         (0)     2942 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config.py
+-rw-rw-r--   0 root         (0) root         (0)    22724 2023-05-23 13:52:19.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/devices.py
+-rw-rw-r--   0 root         (0) root         (0)    10305 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/client.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/pagers.py
+-rw-rw-r--   0 root         (0) root         (0)     3255 2023-05-26 17:20:22.000000 clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11358 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1442 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     5090 2023-05-08 17:54:29.000000 clearblade-cloud-iot-2.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)       77 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/py.typed
+-rw-rw-r--   0 root         (0) root         (0)     5506 2022-11-02 06:10:48.000000 clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/gapic_metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/
+-rw-rw-r--   0 root         (0) root         (0)   235456 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/test_device_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/
+-rw-rw-r--   0 root         (0) root         (0)     1557 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/test_system_device_manager_v1.py
+-rw-rw-r--   0 root         (0) root         (0)     1181 2023-02-20 19:02:15.000000 clearblade-cloud-iot-2.0.2/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2835 2023-05-26 17:24:18.000000 clearblade-cloud-iot-2.0.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     7002 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-13 22:31:57.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 17:24:38.000000 clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/namespace_packages.txt
```

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/device_types.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/device_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,20 @@
 from .resources import GatewayType, LogLevel, PublicKeyFormat, PublicKeyCredential, DeviceCredential
 from .utils import get_value
 import os
 from proto.datetime_helpers import DatetimeWithNanoseconds
 import base64
 
 def convertCredentialsFormatsFromString(credentials):
-    # Converts public Key Format from string to object of class PublicKeyFormat
-    for index, credential in enumerate(credentials):
-        if 'publicKey' in credential:
-            credential['publicKey']['format'] = PublicKeyFormat(credential['publicKey']['format'])
-            credentials[index] = DeviceCredential(credential['publicKey'], credential['expirationTime'])
+    if credentials is not None:
+        # Converts public Key Format from string to object of class PublicKeyFormat
+        for index, credential in enumerate(credentials):
+            if 'publicKey' in credential:
+                credential['publicKey']['format'] = PublicKeyFormat(credential['publicKey']['format'])
+                credentials[index] = DeviceCredential(credential['publicKey'], credential['expirationTime'])
     return credentials
 
 class Device():
     """
     Data class for Clearblade Device
     """
     # TODO: find a better way to construct the Device object. I dont like so much parameter in a constructor
```

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/developer_tests.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/developer_tests.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/resources.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/resources.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/registry.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/config_manager.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/registry_types.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/registry_types.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/http_client.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/http_client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/config.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/config.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/devices.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/devices.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/client.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/client.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/pagers.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/pagers.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade/cloud/iot_v1/utils.py` & `clearblade-cloud-iot-2.0.2/clearblade/cloud/iot_v1/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
         project_region_registry_dict['location'] = list[3]
     if "registries" in list and len(list) >= 6:
         project_region_registry_dict['registry'] = list[5]
 
     return project_region_registry_dict
 
 def get_value(json_data, key):
-    if key in json_data:
-        return json_data[key]
+    if json_data is not None:
+        if key in json_data:
+            return json_data[key]
     return None
 
 class SingletonMetaClass(type):
 
     _instances = {}
 
     def __call__(cls, *args: Any, **kwds: Any) -> Any:
```

### Comparing `clearblade-cloud-iot-2.0.1/LICENSE` & `clearblade-cloud-iot-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/MANIFEST.in` & `clearblade-cloud-iot-2.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/README.rst` & `clearblade-cloud-iot-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/google/cloud/iot_v1/gapic_metadata.json` & `clearblade-cloud-iot-2.0.2/google/cloud/iot_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/unit/gapic/__init__.py` & `clearblade-cloud-iot-2.0.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/unit/gapic/iot_v1/test_device_manager.py` & `clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/unit/gapic/iot_v1/__init__.py` & `clearblade-cloud-iot-2.0.2/tests/unit/gapic/iot_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/unit/__init__.py` & `clearblade-cloud-iot-2.0.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/system/gapic/v1/test_system_device_manager_v1.py` & `clearblade-cloud-iot-2.0.2/tests/system/gapic/v1/test_system_device_manager_v1.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/tests/__init__.py` & `clearblade-cloud-iot-2.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/setup.py` & `clearblade-cloud-iot-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import io
 import os
 
 import setuptools
 
 name = "clearblade-cloud-iot"
 description = "Cloud IoT API client library"
-version = "2.0.1"
+version = "2.0.2"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = ["httpx", "proto-plus"]
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `clearblade-cloud-iot-2.0.1/PKG-INFO` & `clearblade-cloud-iot-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.1
+Version: 2.0.2
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/SOURCES.txt` & `clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clearblade-cloud-iot-2.0.1/clearblade_cloud_iot.egg-info/PKG-INFO` & `clearblade-cloud-iot-2.0.2/clearblade_cloud_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clearblade-cloud-iot
-Version: 2.0.1
+Version: 2.0.2
 Summary: Cloud IoT API client library
 Home-page: https://github.com/clearblade/python-iot
 Author: Clearblade
 Author-email: googleapis-packages@oogle.com
 License: Apache 2.0
 Description: .. Copyright 2023 ClearBlade Inc.
             Licensed under the Apache License, Version 2.0 (the "License");
```


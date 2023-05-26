# Comparing `tmp/abst-1.9.6.tar.gz` & `tmp/abst-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.6.tar", last modified: Fri May 26 12:27:44 2023, max compression
+gzip compressed data, was "abst-1.9.7.tar", last modified: Fri May 26 12:50:25 2023, max compression
```

## Comparing `abst-1.9.6.tar` & `abst-1.9.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 12:27:27.000000 abst-1.9.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:27:44.376497 abst-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 12:27:27.000000 abst-1.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 12:27:27.000000 abst-1.9.6/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 12:27:27.000000 abst-1.9.6/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 12:27:27.000000 abst-1.9.6/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 12:27:27.000000 abst-1.9.6/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-26 12:27:27.000000 abst-1.9.6/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-26 12:27:27.000000 abst-1.9.6/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 12:27:27.000000 abst-1.9.6/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 12:27:27.000000 abst-1.9.6/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:27:44.376497 abst-1.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 12:27:27.000000 abst-1.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 12:27:27.000000 abst-1.9.6/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 12:50:14.000000 abst-1.9.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:50:25.687347 abst-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 12:50:14.000000 abst-1.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 12:50:14.000000 abst-1.9.7/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-05-26 12:50:14.000000 abst-1.9.7/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 12:50:14.000000 abst-1.9.7/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 12:50:14.000000 abst-1.9.7/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 12:50:14.000000 abst-1.9.7/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-26 12:50:14.000000 abst-1.9.7/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:14.000000 abst-1.9.7/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-26 12:50:14.000000 abst-1.9.7/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 12:50:14.000000 abst-1.9.7/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 12:50:14.000000 abst-1.9.7/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:50:25.000000 abst-1.9.7/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:50:25.687347 abst-1.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 12:50:14.000000 abst-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:50:25.687347 abst-1.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 12:50:14.000000 abst-1.9.7/tests/test_sample_dict.py
```

### Comparing `abst-1.9.6/LICENSE.md` & `abst-1.9.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/PKG-INFO` & `abst-1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.6
+Version: 1.9.7
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.6/README.md` & `abst-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.7/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/bastion_support/oci_bastion.py` & `abst-1.9.7/abst/bastion_support/oci_bastion.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,21 @@
                 f" '{response}'")
             self.current_status = "creating bastion session failed"
             return
         else:
             self.current_status = "creating bastion session succeeded"
             rich.print(
                 f"Created Session with id '{bid}' on Bastion {self.get_print_name()} "
-                f"'{response['data']['bastion-name']}'")
+                f"'{response['bastion_name']}'")
 
         rich.print("Auto resolving target details from response")
         host = creds["host"]
-        target_details = response["target-resource-details"]
-        ip = target_details["target-resource-private-ip-address"]
-        port = target_details["target-resource-port"]
+        target_details = response["target_resource_details"]
+        ip = target_details["target_resource_private_ip_address"]
+        port = target_details["target_resource_port"]
 
         self.current_status = "waiting for session init"
         self.wait_for_prepared()
 
         sleep(1)  # Precaution init delay
 
         self.current_status = "digging tunnel"
```

### Comparing `abst-1.9.6/abst/cfg_func.py` & `abst-1.9.7/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/config.py` & `abst-1.9.7/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/dialogs.py` & `abst-1.9.7/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/main.py` & `abst-1.9.7/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/notifier/version_notifier.py` & `abst-1.9.7/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/tools.py` & `abst-1.9.7/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst/wrappers.py` & `abst-1.9.7/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/abst.egg-info/PKG-INFO` & `abst-1.9.7/abst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.6
+Version: 1.9.7
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.6/abst.egg-info/SOURCES.txt` & `abst-1.9.7/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.6/setup.py` & `abst-1.9.7/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/abst-1.9.5.tar.gz` & `tmp/abst-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.5.tar", last modified: Tue Apr 25 11:56:21 2023, max compression
+gzip compressed data, was "abst-1.9.6.tar", last modified: Fri May 26 12:27:44 2023, max compression
```

## Comparing `abst-1.9.5.tar` & `abst-1.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 11:56:10.000000 abst-1.9.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-25 11:56:21.188225 abst-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-25 11:56:10.000000 abst-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 11:56:10.000000 abst-1.9.5/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-25 11:56:10.000000 abst-1.9.5/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-25 11:56:10.000000 abst-1.9.5/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 11:56:10.000000 abst-1.9.5/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-25 11:56:10.000000 abst-1.9.5/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-04-25 11:56:10.000000 abst-1.9.5/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:10.000000 abst-1.9.5/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 11:56:10.000000 abst-1.9.5/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-25 11:56:10.000000 abst-1.9.5/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-25 11:56:10.000000 abst-1.9.5/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 11:56:21.000000 abst-1.9.5/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 11:56:21.188225 abst-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-25 11:56:10.000000 abst-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 11:56:21.188225 abst-1.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 11:56:10.000000 abst-1.9.5/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 12:27:27.000000 abst-1.9.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:27:44.376497 abst-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 12:27:27.000000 abst-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 12:27:27.000000 abst-1.9.6/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-05-26 12:27:27.000000 abst-1.9.6/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 12:27:27.000000 abst-1.9.6/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 12:27:27.000000 abst-1.9.6/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 12:27:27.000000 abst-1.9.6/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18720 2023-05-26 12:27:27.000000 abst-1.9.6/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:27.000000 abst-1.9.6/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-26 12:27:27.000000 abst-1.9.6/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 12:27:27.000000 abst-1.9.6/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 12:27:27.000000 abst-1.9.6/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:27:44.000000 abst-1.9.6/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:27:44.376497 abst-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 12:27:27.000000 abst-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:27:44.376497 abst-1.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 12:27:27.000000 abst-1.9.6/tests/test_sample_dict.py
```

### Comparing `abst-1.9.5/LICENSE.md` & `abst-1.9.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/PKG-INFO` & `abst-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.5
+Version: 1.9.6
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.5/README.md` & `abst-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.6/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/bastion_support/oci_bastion.py` & `abst-1.9.6/abst/bastion_support/oci_bastion.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
         if Bastion.stopped:
             return
         public_key = get_public_key(ssh_path)
         sess_details = oci.bastion.models.CreateSessionDetails(bastion_id=bastion_id,
                                                                target_resource_details=oci.bastion.models.CreateManagedSshSessionTargetResourceDetails(
                                                                    session_type="MANAGED_SSH",
                                                                    target_resource_id=resource_id,
-                                                                   target_os_username=os_username),
+                                                                   target_resource_operating_system_user_name=os_username),
                                                                key_details=oci.bastion.models.PublicKeyDetails(
                                                                    public_key_content=public_key),
                                                                display_name=name,
                                                                key_type="PUB",
                                                                session_ttl_in_seconds=ttl)
         config = oci.config.from_file()
         req = oci.bastion.BastionClient(config).create_session(sess_details)
```

### Comparing `abst-1.9.5/abst/cfg_func.py` & `abst-1.9.6/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/config.py` & `abst-1.9.6/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/dialogs.py` & `abst-1.9.6/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/main.py` & `abst-1.9.6/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/notifier/version_notifier.py` & `abst-1.9.6/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/tools.py` & `abst-1.9.6/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst/wrappers.py` & `abst-1.9.6/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/abst.egg-info/PKG-INFO` & `abst-1.9.6/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.5
+Version: 1.9.6
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.5/abst.egg-info/SOURCES.txt` & `abst-1.9.6/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.5/setup.py` & `abst-1.9.6/setup.py`

 * *Files identical despite different names*


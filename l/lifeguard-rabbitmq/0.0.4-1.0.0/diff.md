# Comparing `tmp/lifeguard-rabbitmq-0.0.4.tar.gz` & `tmp/lifeguard-rabbitmq-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-rabbitmq-0.0.4.tar", last modified: Thu Jun 17 11:56:46 2021, max compression
+gzip compressed data, was "lifeguard-rabbitmq-1.0.0.tar", last modified: Fri May 26 12:08:09 2023, max compression
```

## Comparing `lifeguard-rabbitmq-0.0.4.tar` & `lifeguard-rabbitmq-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/rabbitmq/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-06-17 11:56:46.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      462 2021-06-17 11:56:46.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-17 11:56:46.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-06-17 11:56:46.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-06-17 11:56:46.000000 lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-17 11:56:46.477724 lifeguard-rabbitmq-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-06-17 11:56:26.000000 lifeguard-rabbitmq-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/rabbitmq/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-26 12:08:08.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 12:08:08.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:08:08.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 12:08:08.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 12:08:08.000000 lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 12:08:09.015653 lifeguard-rabbitmq-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 12:07:19.000000 lifeguard-rabbitmq-1.0.0/setup.py
```

### Comparing `lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/__init__.py` & `lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/context.py` & `lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/rabbitmq/admin.py` & `lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/rabbitmq/admin.py`

 * *Files identical despite different names*

### Comparing `lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/settings.py` & `lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-rabbitmq-0.0.4/lifeguard_rabbitmq/validations.py` & `lifeguard-rabbitmq-1.0.0/lifeguard_rabbitmq/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,17 @@
 
     for rabbitmq_admin_instance in options["queues"]:
         queues = options["queues"][rabbitmq_admin_instance]
 
         status = change_status(
             status, __check_consumers(rabbitmq_admin_instance, queues, details)
         )
-    return ValidationResponse("consumers_running_validation", status, details)
+    return ValidationResponse(
+        status, details, validation_name="consumers_running_validation"
+    )
 
 
 def messages_increasing_validation():
     """
     Validates message incresing for a queue
     """
 
@@ -116,8 +118,10 @@
     for rabbitmq_admin_instance in options["queues"]:
         queues = options["queues"][rabbitmq_admin_instance]
 
         status = change_status(
             status, __check_message_increasing(rabbitmq_admin_instance, queues, details)
         )
 
-    return ValidationResponse("messages_increasing_validation", status, details)
+    return ValidationResponse(
+        status, details, validation_name="messages_increasing_validation"
+    )
```


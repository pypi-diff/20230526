# Comparing `tmp/lifeguard-peewee-0.0.1.tar.gz` & `tmp/lifeguard-peewee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-peewee-0.0.1.tar", last modified: Mon Oct  4 10:27:34 2021, max compression
+gzip compressed data, was "lifeguard-peewee-0.0.2.tar", last modified: Fri May 26 20:36:36 2023, max compression
```

## Comparing `lifeguard-peewee-0.0.1.tar` & `lifeguard-peewee-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:27:34.215485 lifeguard-peewee-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-10-04 10:27:34.215485 lifeguard-peewee-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:27:34.215485 lifeguard-peewee-0.0.1/lifeguard_peewee/
--rw-r--r--   0 runner    (1001) docker     (121)      648 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/lifeguard_peewee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/lifeguard_peewee/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/lifeguard_peewee/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/lifeguard_peewee/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/lifeguard_peewee/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:27:34.215485 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-10-04 10:27:34.000000 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2021-10-04 10:27:34.000000 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 10:27:34.000000 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-04 10:27:34.000000 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-04 10:27:34.000000 lifeguard-peewee-0.0.1/lifeguard_peewee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-04 10:27:34.215485 lifeguard-peewee-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      503 2021-10-04 10:27:03.000000 lifeguard-peewee-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:36:36.481187 lifeguard-peewee-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 20:36:36.481187 lifeguard-peewee-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:36:36.477187 lifeguard-peewee-0.0.2/lifeguard_peewee/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/lifeguard_peewee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/lifeguard_peewee/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/lifeguard_peewee/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/lifeguard_peewee/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/lifeguard_peewee/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:36:36.477187 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 20:36:36.000000 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 20:36:36.000000 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:36:36.000000 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:36:36.000000 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:36:36.000000 lifeguard-peewee-0.0.2/lifeguard_peewee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:36:36.481187 lifeguard-peewee-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-26 20:36:10.000000 lifeguard-peewee-0.0.2/setup.py
```

### Comparing `lifeguard-peewee-0.0.1/lifeguard_peewee/__init__.py` & `lifeguard-peewee-0.0.2/lifeguard_peewee/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-peewee-0.0.1/lifeguard_peewee/context.py` & `lifeguard-peewee-0.0.2/lifeguard_peewee/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-peewee-0.0.1/lifeguard_peewee/models.py` & `lifeguard-peewee-0.0.2/lifeguard_peewee/models.py`

 * *Files identical despite different names*

### Comparing `lifeguard-peewee-0.0.1/lifeguard_peewee/repositories.py` & `lifeguard-peewee-0.0.2/lifeguard_peewee/repositories.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         save_or_update(
             ValidationModel,
             (ValidationModel.validation_name == validation_result.validation_name),
             {
                 "validation_name": validation_result.validation_name,
                 "status": validation_result.status,
                 "details": json.dumps(validation_result.details),
-                "settings": json.dumps(validation_result.settings),
+                "settings": json.dumps(validation_result.settings or {}),
                 "last_execution": validation_result.last_execution,
             },
         )
 
     def fetch_last_validation_result(self, validation_name):
         result = ValidationModel.get(ValidationModel.validation_name == validation_name)
         if result:
@@ -51,47 +51,49 @@
         for result in ValidationModel.select():
             results.append(self.__convert_to_validation(result))
 
         return results
 
     def __convert_to_validation(self, validation_document):
         return ValidationResponse(
-            validation_document["validation_name"],
-            validation_document["status"],
-            json.loads(validation_document["details"]),
-            json.loads(validation_document["settings"]),
-            last_execution=validation_document["last_execution"],
+            validation_document.status,
+            json.loads(validation_document.details),
+            json.loads(validation_document.settings),
+            last_execution=validation_document.last_execution,
+            validation_name=validation_document.validation_name,
         )
 
 
 class PeeweeNotificationRepository:
     """
     Implementation of NotificationRepository with Peewee
     """
 
     def save_last_notification_for_a_validation(self, notification):
         save_or_update(
             NotificationModel,
             (NotificationModel.validation_name == notification.validation_name),
             {
                 "validation_name": notification.validation_name,
-                "thread_ids": notification.thread_ids,
+                "thread_ids": json.dumps(notification.thread_ids),
                 "is_opened": notification.is_opened,
                 "options": json.dumps(notification.options),
                 "last_notification": notification.last_notification,
             },
         )
 
     def fetch_last_notification_for_a_validation(self, validation_name):
         result = (
             NotificationModel.select()
             .where(NotificationModel.validation_name == validation_name)
             .first()
         )
         if result:
             last_notification_status = NotificationStatus(
-                validation_name, result["thread_ids"], json.loads(result["options"])
+                validation_name,
+                json.loads(result["thread_ids"]),
+                json.loads(result["options"]),
             )
             last_notification_status.last_notification = result["last_notification"]
             last_notification_status.is_opened = result["is_opened"]
             return last_notification_status
         return None
```

### Comparing `lifeguard-peewee-0.0.1/lifeguard_peewee/settings.py` & `lifeguard-peewee-0.0.2/lifeguard_peewee/settings.py`

 * *Files identical despite different names*


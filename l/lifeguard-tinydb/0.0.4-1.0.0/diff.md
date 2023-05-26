# Comparing `tmp/lifeguard-tinydb-0.0.4.tar.gz` & `tmp/lifeguard-tinydb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-tinydb-0.0.4.tar", last modified: Thu Sep  1 11:47:58 2022, max compression
+gzip compressed data, was "lifeguard-tinydb-1.0.0.tar", last modified: Fri May 26 20:08:48 2023, max compression
```

## Comparing `lifeguard-tinydb-0.0.4.tar` & `lifeguard-tinydb-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 11:47:58.687712 lifeguard-tinydb-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-01 11:47:58.687712 lifeguard-tinydb-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-01 11:47:41.000000 lifeguard-tinydb-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 11:47:58.683712 lifeguard-tinydb-0.0.4/lifeguard_tinydb/
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-09-01 11:47:41.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-09-01 11:47:41.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-01 11:47:41.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 11:47:58.687712 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-01 11:47:58.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-09-01 11:47:58.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 11:47:58.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-01 11:47:58.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-01 11:47:58.000000 lifeguard-tinydb-0.0.4/lifeguard_tinydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-01 11:47:58.687712 lifeguard-tinydb-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-01 11:47:41.000000 lifeguard-tinydb-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/lifeguard_tinydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/setup.py
```

### Comparing `lifeguard-tinydb-0.0.4/lifeguard_tinydb/__init__.py` & `lifeguard-tinydb-1.0.0/lifeguard_tinydb/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-tinydb-0.0.4/lifeguard_tinydb/repositories.py` & `lifeguard-tinydb-1.0.0/lifeguard_tinydb/repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,32 +67,31 @@
     def __convert_to_validation(self, entry):
         last_execution = entry["last_execution"]
 
         if last_execution:
             last_execution = datetime.strptime(last_execution, DATE_FORMAT)
 
         return ValidationResponse(
-            entry["validation_name"],
             entry["status"],
             entry["details"],
             entry["settings"],
             last_execution=last_execution,
+            validation_name=entry["validation_name"],
         )
 
     def __get_key(self, validation_name):
         query = Query()
         return query.validation_name == validation_name
 
 
 class TinyDBNotificationRepository:
     def __init__(self):
         self.table = DATABASE.table("notifications")
 
     def save_last_notification_for_a_validation(self, notification):
-
         data = {
             "validation_name": notification.validation_name,
             "thread_ids": notification.thread_ids,
             "is_opened": notification.is_opened,
             "options": notification.options,
             "last_notification": None,
         }
```


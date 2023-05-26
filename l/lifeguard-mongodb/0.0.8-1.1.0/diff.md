# Comparing `tmp/lifeguard-mongodb-0.0.8.tar.gz` & `tmp/lifeguard-mongodb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-mongodb-0.0.8.tar", last modified: Mon Jan  3 11:34:26 2022, max compression
+gzip compressed data, was "lifeguard-mongodb-1.1.0.tar", last modified: Fri May 26 15:18:12 2023, max compression
```

## Comparing `lifeguard-mongodb-0.0.8.tar` & `lifeguard-mongodb-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 11:34:26.951189 lifeguard-mongodb-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-01-03 11:34:26.951189 lifeguard-mongodb-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-01-03 11:33:56.000000 lifeguard-mongodb-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 11:34:26.951189 lifeguard-mongodb-0.0.8/lifeguard_mongodb/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-01-03 11:33:56.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-01-03 11:33:56.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb/repositories.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-01-03 11:33:56.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 11:34:26.951189 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-01-03 11:34:26.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-01-03 11:34:26.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 11:34:26.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-03 11:34:26.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-03 11:34:26.000000 lifeguard-mongodb-0.0.8/lifeguard_mongodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 11:34:26.951189 lifeguard-mongodb-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-01-03 11:33:56.000000 lifeguard-mongodb-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/lifeguard_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/setup.py
```

### Comparing `lifeguard-mongodb-0.0.8/lifeguard_mongodb/__init__.py` & `lifeguard-mongodb-1.1.0/lifeguard_mongodb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Lifeguard integration with MongoDB
 """
 from lifeguard.repositories import declare_implementation
 
-from lifeguard_mongodb.repositories import (MongoDBNotificationRepository,
-                                            MongoDBValidationRepository)
+from lifeguard_mongodb.repositories import (
+    MongoDBHistoryRepository,
+    MongoDBNotificationRepository,
+    MongoDBValidationRepository,
+)
 
 
 class LifeguardMongoDBPlugin:
     def __init__(self, lifeguard_context):
         self.lifeguard_context = lifeguard_context
+        declare_implementation("history", MongoDBHistoryRepository)
         declare_implementation("notification", MongoDBNotificationRepository)
         declare_implementation("validation", MongoDBValidationRepository)
 
 
 def init(lifeguard_context):
     LifeguardMongoDBPlugin(lifeguard_context)
```

### Comparing `lifeguard-mongodb-0.0.8/lifeguard_mongodb/repositories.py` & `lifeguard-mongodb-1.1.0/lifeguard_mongodb/repositories.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Implementation of repositories using MongoDB
 """
-from lifeguard.notifications import NotificationStatus
+from lifeguard.notifications import NotificationStatus, NotificationOccurrence
 from lifeguard.validations import ValidationResponse
-from pymongo import MongoClient
+from pymongo import MongoClient, DESCENDING
 
 from lifeguard_mongodb.settings import LIFEGUARD_MONGODB_DATABASE, LIFEGUARD_MONGODB_URL
 
 CLIENT = MongoClient(LIFEGUARD_MONGODB_URL)
 DATABASE = CLIENT[LIFEGUARD_MONGODB_DATABASE]
 
 
@@ -20,14 +20,55 @@
     """
     if collection.count_documents(query):
         collection.update_many(query, {"$set": data})
     else:
         collection.insert_one(data)
 
 
+class MongoDBHistoryRepository:
+    def __init__(self):
+        self.collection = DATABASE.history
+
+    def append_notification(self, notification_occurrence):
+        self.collection.insert_one(
+            {
+                "validation_name": notification_occurrence.validation_name,
+                "details": notification_occurrence.details,
+                "status": notification_occurrence.status,
+                "notification_type": notification_occurrence.notification_type,
+                "created_at": notification_occurrence.created_at,
+            }
+        )
+
+    def fetch_notifications(self, start_interval, end_interval, filters, page, limit):
+        filters.update({"created_at": {"$gte": start_interval, "$lte": end_interval}})
+
+        query = self.collection.find(filters)
+
+        if page and limit:
+            query = query.limit(limit).skip((page - 1) * limit)
+
+        query = query.sort("created_at", DESCENDING)
+
+        return [self.__convert_to_occurrence(entry) for entry in query]
+
+    def count_notifications(self, start_interval, end_interval, filters):
+        filters.update({"created_at": {"$gte": start_interval, "$lte": end_interval}})
+        return self.collection.count_documents(filters)
+
+    def __convert_to_occurrence(self, entry):
+        return NotificationOccurrence(
+            validation_name=entry["validation_name"],
+            details=entry["details"],
+            status=entry["status"],
+            notification_type=entry["notification_type"],
+            created_at=entry["created_at"],
+        )
+
+
 class MongoDBValidationRepository:
     def __init__(self):
         self.collection = DATABASE.validations
 
     def save_validation_result(self, validation_result):
         save_or_update(
             self.collection,
@@ -52,19 +93,19 @@
         for result in self.collection.find():
             results.append(self.__convert_to_validation(result))
 
         return results
 
     def __convert_to_validation(self, validation_document):
         return ValidationResponse(
-            validation_document["validation_name"],
             validation_document["status"],
             validation_document["details"],
             validation_document["settings"],
             last_execution=validation_document["last_execution"],
+            validation_name=validation_document["validation_name"],
         )
 
 
 class MongoDBNotificationRepository:
     def __init__(self):
         self.collection = DATABASE.notifications
```

### Comparing `lifeguard-mongodb-0.0.8/lifeguard_mongodb/settings.py` & `lifeguard-mongodb-1.1.0/lifeguard_mongodb/settings.py`

 * *Files identical despite different names*


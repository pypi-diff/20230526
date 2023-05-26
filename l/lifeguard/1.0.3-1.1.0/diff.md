# Comparing `tmp/lifeguard-1.0.3.tar.gz` & `tmp/lifeguard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-1.0.3.tar", last modified: Fri May 26 13:14:58 2023, max compression
+gzip compressed data, was "lifeguard-1.1.0.tar", last modified: Fri May 26 13:55:35 2023, max compression
```

## Comparing `lifeguard-1.0.3.tar` & `lifeguard-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.931215 lifeguard-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-26 13:14:58.931215 lifeguard-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-26 13:14:44.000000 lifeguard-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.923215 lifeguard-1.0.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2790 2023-05-26 13:14:44.000000 lifeguard-1.0.3/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.923215 lifeguard-1.0.3/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.927215 lifeguard-1.0.3/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/actions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.927215 lifeguard-1.0.3/lifeguard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/controllers/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-26 13:14:44.000000 lifeguard-1.0.3/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.927215 lifeguard-1.0.3/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-26 13:14:58.000000 lifeguard-1.0.3/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 13:14:58.000000 lifeguard-1.0.3/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:14:58.000000 lifeguard-1.0.3/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 13:14:58.000000 lifeguard-1.0.3/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 13:14:58.000000 lifeguard-1.0.3/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 13:14:58.931215 lifeguard-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 13:14:44.000000 lifeguard-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.927215 lifeguard-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.931215 lifeguard-1.0.3/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/actions/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.931215 lifeguard-1.0.3/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/controllers/test_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:58.931215 lifeguard-1.0.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-26 13:14:44.000000 lifeguard-1.0.3/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 13:55:35.184851 lifeguard-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-26 13:55:24.000000 lifeguard-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.180851 lifeguard-1.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-05-26 13:55:24.000000 lifeguard-1.1.0/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 13:55:35.184851 lifeguard-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 13:55:24.000000 lifeguard-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_validations.py
```

### Comparing `lifeguard-1.0.3/PKG-INFO` & `lifeguard-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.0.3
+Version: 1.1.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -109,21 +109,25 @@
 
 This file should be in the `controllers` directory and should ends with `_controller.py`.
 
 ### Init Lifeguard
 
 Execute: `lifeguard`
 
+To init only web server: `lifeguard --no-scheduler`
+
+To init only scheduler: `lifeguard --no-server`
+
 ### Settings
 
 To see all settings avaiable run command:
 
 `lifeguard -d`
 
-## Builtin Endpoints 
+## Builtin Endpoints
 
 ### Recover Status
 
 __To get global status and all validations.__
 
 `GET /lifeguard/status/complete`
```

### Comparing `lifeguard-1.0.3/README.md` & `lifeguard-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -93,21 +93,25 @@
 
 This file should be in the `controllers` directory and should ends with `_controller.py`.
 
 ### Init Lifeguard
 
 Execute: `lifeguard`
 
+To init only web server: `lifeguard --no-scheduler`
+
+To init only scheduler: `lifeguard --no-server`
+
 ### Settings
 
 To see all settings avaiable run command:
 
 `lifeguard -d`
 
-## Builtin Endpoints 
+## Builtin Endpoints
 
 ### Recover Status
 
 __To get global status and all validations.__
 
 `GET /lifeguard/status/complete`
```

### Comparing `lifeguard-1.0.3/bin/lifeguard` & `lifeguard-1.1.0/bin/lifeguard`

 * *Files 9% similar despite different names*

```diff
@@ -29,16 +29,19 @@
 
 
 def number_of_workers():
     return (multiprocessing.cpu_count() * 2) + 1
 
 
 # Scheduler
-def scheduler():
-    _thread.start_new_thread(start_scheduler, ())
+def scheduler(start_in_thread):
+    if start_in_thread:
+        _thread.start_new_thread(start_scheduler, ())
+    else:
+        start_scheduler()
 
 
 # Server
 class StandaloneApplication(gunicorn.app.base.BaseApplication):
     def __init__(self, app, options=None):
         self.options = options or {}
         self.application = app
@@ -92,15 +95,16 @@
     setup(LIFEGUARD_CONTEXT)
 
     if args.settings:
         display_settings()
         sys.exit(0)
 
     if not args.no_scheduler:
-        scheduler()
+        start_in_thread = not args.no_server
+        scheduler(start_in_thread)
 
     if not args.no_server:
         from lifeguard.server import APP
 
         StandaloneApplication(
             APP,
             {
```

### Comparing `lifeguard-1.0.3/lifeguard/__init__.py` & `lifeguard-1.1.0/lifeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/actions/email.py` & `lifeguard-1.1.0/lifeguard/actions/email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/actions/notifications.py` & `lifeguard-1.1.0/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/auth.py` & `lifeguard-1.1.0/lifeguard/auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/context.py` & `lifeguard-1.1.0/lifeguard/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/controllers/__init__.py` & `lifeguard-1.1.0/lifeguard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/controllers/assets.py` & `lifeguard-1.1.0/lifeguard/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/http_client.py` & `lifeguard-1.1.0/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/logger.py` & `lifeguard-1.1.0/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/notifications.py` & `lifeguard-1.1.0/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/repositories.py` & `lifeguard-1.1.0/lifeguard/repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/scheduler.py` & `lifeguard-1.1.0/lifeguard/scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/server.py` & `lifeguard-1.1.0/lifeguard/server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/settings.py` & `lifeguard-1.1.0/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard/validations.py` & `lifeguard-1.1.0/lifeguard/validations.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/lifeguard.egg-info/PKG-INFO` & `lifeguard-1.1.0/lifeguard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.0.3
+Version: 1.1.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -109,21 +109,25 @@
 
 This file should be in the `controllers` directory and should ends with `_controller.py`.
 
 ### Init Lifeguard
 
 Execute: `lifeguard`
 
+To init only web server: `lifeguard --no-scheduler`
+
+To init only scheduler: `lifeguard --no-server`
+
 ### Settings
 
 To see all settings avaiable run command:
 
 `lifeguard -d`
 
-## Builtin Endpoints 
+## Builtin Endpoints
 
 ### Recover Status
 
 __To get global status and all validations.__
 
 `GET /lifeguard/status/complete`
```

### Comparing `lifeguard-1.0.3/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.1.0/lifeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/setup.py` & `lifeguard-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard",
-    version="1.0.3",
+    version="1.1.0",
     url="https://github.com/LifeguardSystem/lifeguard",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=["bin/lifeguard"],
     include_package_data=True,
     description="Application to monitor your systems and give you the security to sleep peacefully at night",
```

### Comparing `lifeguard-1.0.3/tests/actions/test_database.py` & `lifeguard-1.1.0/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/actions/test_email.py` & `lifeguard-1.1.0/tests/actions/test_email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/actions/test_notification.py` & `lifeguard-1.1.0/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/controllers/test_assets.py` & `lifeguard-1.1.0/tests/controllers/test_assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_auth.py` & `lifeguard-1.1.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_bootstrap.py` & `lifeguard-1.1.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_controllers.py` & `lifeguard-1.1.0/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_http_client.py` & `lifeguard-1.1.0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_lifeguard_core.py` & `lifeguard-1.1.0/tests/test_lifeguard_core.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_notifications.py` & `lifeguard-1.1.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_repositories.py` & `lifeguard-1.1.0/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_scheduler.py` & `lifeguard-1.1.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_server.py` & `lifeguard-1.1.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_settings.py` & `lifeguard-1.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.0.3/tests/test_validations.py` & `lifeguard-1.1.0/tests/test_validations.py`

 * *Files identical despite different names*


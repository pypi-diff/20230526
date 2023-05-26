# Comparing `tmp/metasdk-1.5.2.tar.gz` & `tmp/metasdk-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasdk-1.5.2.tar", last modified: Fri Oct 28 15:18:35 2022, max compression
+gzip compressed data, was "metasdk-1.6.0.tar", last modified: Fri May 26 15:59:41 2023, max compression
```

## Comparing `metasdk-1.5.2.tar` & `metasdk-1.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.371543 metasdk-1.5.2/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1074 2022-09-16 07:43:27.000000 metasdk-1.5.2/LICENSE
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-09-16 07:43:27.000000 metasdk-1.5.2/MANIFEST.in
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2096 2022-10-28 15:18:35.371543 metasdk-1.5.2/PKG-INFO
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1804 2022-09-16 07:43:27.000000 metasdk-1.5.2/README.md
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.368543 metasdk-1.5.2/metasdk/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)    16139 2022-10-12 13:23:13.000000 metasdk-1.5.2/metasdk/__init__.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      190 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/__state.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     3803 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/apiclient.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     6152 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/event_bus.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     3523 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/exceptions.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      102 2022-10-28 12:42:11.000000 metasdk-1.5.2/metasdk/info.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1815 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/internal.py
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.369542 metasdk-1.5.2/metasdk/logger/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     6374 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/logger/__init__.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1862 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/logger/bulk_logger.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     3477 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/logger/logger.py
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.371543 metasdk-1.5.2/metasdk/services/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     8667 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/ApiProxyService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      634 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/CacheService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     5086 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/DbQueryService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2922 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/DbService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1355 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/DevService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1066 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/ExportService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2563 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/ExternalSystemService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     4414 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/FeedService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1939 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/IssueService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     5785 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/LockService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1394 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/MailService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1936 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/MediaService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1362 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/MetaqlService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      968 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/ObjectLogService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2554 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/SettingsService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     8698 2022-10-28 12:42:11.000000 metasdk-1.5.2/metasdk/services/StarterService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      691 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/UserManagementService.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1157 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/services/__init__.py
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.371543 metasdk-1.5.2/metasdk/tools/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/tools/__init__.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1064 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/tools/extract_event_handlers.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2252 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/utils.py
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2051 2022-09-16 07:43:27.000000 metasdk-1.5.2/metasdk/worker.py
-drwxr-xr-x   0 anton_fedora  (1000) anton_fedora  (1000)        0 2022-10-28 15:18:35.368543 metasdk-1.5.2/metasdk.egg-info/
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     2096 2022-10-28 15:18:35.000000 metasdk-1.5.2/metasdk.egg-info/PKG-INFO
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1140 2022-10-28 15:18:35.000000 metasdk-1.5.2/metasdk.egg-info/SOURCES.txt
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        1 2022-10-28 15:18:35.000000 metasdk-1.5.2/metasdk.egg-info/dependency_links.txt
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      170 2022-10-28 15:18:35.000000 metasdk-1.5.2/metasdk.egg-info/requires.txt
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)        8 2022-10-28 15:18:35.000000 metasdk-1.5.2/metasdk.egg-info/top_level.txt
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)      205 2022-10-28 15:18:35.371543 metasdk-1.5.2/setup.cfg
--rw-r--r--   0 anton_fedora  (1000) anton_fedora  (1000)     1193 2022-09-16 07:43:27.000000 metasdk-1.5.2/setup.py
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.207190 metasdk-1.6.0/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1074 2022-08-26 13:49:22.000000 metasdk-1.6.0/LICENSE
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2022-08-26 13:49:22.000000 metasdk-1.6.0/MANIFEST.in
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2096 2023-05-26 15:59:41.207254 metasdk-1.6.0/PKG-INFO
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1804 2022-08-26 13:49:22.000000 metasdk-1.6.0/README.md
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.202357 metasdk-1.6.0/metasdk/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)    16137 2023-05-26 15:16:00.000000 metasdk-1.6.0/metasdk/__init__.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      190 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/__state.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     3803 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/apiclient.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     6152 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/event_bus.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     3523 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/exceptions.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      102 2023-05-26 15:16:00.000000 metasdk-1.6.0/metasdk/info.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1815 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/internal.py
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.203451 metasdk-1.6.0/metasdk/logger/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     6374 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/logger/__init__.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1862 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/logger/bulk_logger.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     3477 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/logger/logger.py
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.206769 metasdk-1.6.0/metasdk/services/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     8667 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/ApiProxyService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      634 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/CacheService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     5086 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/DbQueryService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2922 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/DbService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1355 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/DevService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1066 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/ExportService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2563 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/ExternalSystemService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     4414 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/FeedService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1939 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/IssueService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     5785 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/LockService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1394 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/MailService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1936 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/MediaService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1362 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/MetaqlService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      968 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/ObjectLogService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2554 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/SettingsService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     8698 2023-05-26 15:16:00.000000 metasdk-1.6.0/metasdk/services/StarterService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      691 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/UserManagementService.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1157 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/services/__init__.py
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.207041 metasdk-1.6.0/metasdk/tools/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/tools/__init__.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1064 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/tools/extract_event_handlers.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2252 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/utils.py
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2051 2022-08-26 13:49:22.000000 metasdk-1.6.0/metasdk/worker.py
+drwxr-xr-x   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        0 2023-05-26 15:59:41.202950 metasdk-1.6.0/metasdk.egg-info/
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     2096 2023-05-26 15:59:41.000000 metasdk-1.6.0/metasdk.egg-info/PKG-INFO
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1140 2023-05-26 15:59:41.000000 metasdk-1.6.0/metasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        1 2023-05-26 15:59:41.000000 metasdk-1.6.0/metasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      170 2023-05-26 15:59:41.000000 metasdk-1.6.0/metasdk.egg-info/requires.txt
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)        8 2023-05-26 15:59:41.000000 metasdk-1.6.0/metasdk.egg-info/top_level.txt
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)      205 2023-05-26 15:59:41.207518 metasdk-1.6.0/setup.cfg
+-rw-r--r--   0 user50   (796914239) REALWEBAD\Domain Users (416692438)     1193 2022-08-26 13:49:22.000000 metasdk-1.6.0/setup.py
```

### Comparing `metasdk-1.5.2/LICENSE` & `metasdk-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/PKG-INFO` & `metasdk-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.5.2
+Version: 1.6.0
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metasdk-1.5.2/README.md` & `metasdk-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/__init__.py` & `metasdk-1.6.0/metasdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         self.redis_url = os.environ.get("REDIS_URL", redis_url or "s1.meta.vmc.loc:6379:1")
         self.meta_url = os.environ.get("META_URL", meta_url or "http://apimeta.devision.io")
         self.api_proxy_url = os.environ.get("API_PROXY_URL", api_proxy_url or "https://apiproxy.apis.garpun.com")
 
         if debug and not starter_api_url:
             starter_api_url = DEV_STARTER_STUB_URL
-        self.starter_api_url = os.environ.get("STARTER_URL", starter_api_url or "http://s2.meta.vmc.loc:28341")
+        self.starter_api_url = os.environ.get("STARTER_URL", starter_api_url or "http://starter_url_not_set")
 
         if service_id:
             self.log.warning("Параметр service_id скоро будет удален из MetaApp")
 
         gcloud_log_host_port = os.environ.get("GCLOUD_LOG_HOST_PORT", gcloud_log_host_port or "n3.adp.vmc.loc:31891")
         service_ns = os.environ.get('SERVICE_NAMESPACE', "appscript")  # для ns в логах и для префикса Dispatcher
         service_id = os.environ.get('SERVICE_ID', "local_debug_serivce")
```

### Comparing `metasdk-1.5.2/metasdk/apiclient.py` & `metasdk-1.6.0/metasdk/apiclient.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/event_bus.py` & `metasdk-1.6.0/metasdk/event_bus.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/exceptions.py` & `metasdk-1.6.0/metasdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/internal.py` & `metasdk-1.6.0/metasdk/internal.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/logger/__init__.py` & `metasdk-1.6.0/metasdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/logger/bulk_logger.py` & `metasdk-1.6.0/metasdk/logger/bulk_logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/logger/logger.py` & `metasdk-1.6.0/metasdk/logger/logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/ApiProxyService.py` & `metasdk-1.6.0/metasdk/services/ApiProxyService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/CacheService.py` & `metasdk-1.6.0/metasdk/services/CacheService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/DbQueryService.py` & `metasdk-1.6.0/metasdk/services/DbQueryService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/DbService.py` & `metasdk-1.6.0/metasdk/services/DbService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/DevService.py` & `metasdk-1.6.0/metasdk/services/DevService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/ExportService.py` & `metasdk-1.6.0/metasdk/services/ExportService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/ExternalSystemService.py` & `metasdk-1.6.0/metasdk/services/ExternalSystemService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/FeedService.py` & `metasdk-1.6.0/metasdk/services/FeedService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/IssueService.py` & `metasdk-1.6.0/metasdk/services/IssueService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/LockService.py` & `metasdk-1.6.0/metasdk/services/LockService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/MailService.py` & `metasdk-1.6.0/metasdk/services/MailService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/MediaService.py` & `metasdk-1.6.0/metasdk/services/MediaService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/MetaqlService.py` & `metasdk-1.6.0/metasdk/services/MetaqlService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/ObjectLogService.py` & `metasdk-1.6.0/metasdk/services/ObjectLogService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/SettingsService.py` & `metasdk-1.6.0/metasdk/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/StarterService.py` & `metasdk-1.6.0/metasdk/services/StarterService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/UserManagementService.py` & `metasdk-1.6.0/metasdk/services/UserManagementService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/services/__init__.py` & `metasdk-1.6.0/metasdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/tools/extract_event_handlers.py` & `metasdk-1.6.0/metasdk/tools/extract_event_handlers.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/utils.py` & `metasdk-1.6.0/metasdk/utils.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk/worker.py` & `metasdk-1.6.0/metasdk/worker.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/metasdk.egg-info/PKG-INFO` & `metasdk-1.6.0/metasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.5.2
+Version: 1.6.0
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metasdk-1.5.2/metasdk.egg-info/SOURCES.txt` & `metasdk-1.6.0/metasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metasdk-1.5.2/setup.py` & `metasdk-1.6.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/recnetpy-0.1.46.tar.gz` & `tmp/recnetpy-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recnetpy-0.1.46.tar", last modified: Sun Dec  4 22:09:40 2022, max compression
+gzip compressed data, was "recnetpy-0.1.47.tar", last modified: Fri May 26 13:33:58 2023, max compression
```

## Comparing `recnetpy-0.1.46.tar` & `recnetpy-0.1.47.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.789094 recnetpy-0.1.46/
--rw-rw-rw-   0        0        0     1140 2022-10-05 19:19:27.000000 recnetpy-0.1.46/LICENSE
--rw-rw-rw-   0        0        0     3242 2022-12-04 22:09:40.788096 recnetpy-0.1.46/PKG-INFO
--rw-rw-rw-   0        0        0     2672 2022-10-26 14:57:00.000000 recnetpy-0.1.46/README.md
--rw-rw-rw-   0        0        0      715 2022-12-04 22:09:05.000000 recnetpy-0.1.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-04 22:09:40.789094 recnetpy-0.1.46/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.382674 recnetpy-0.1.46/src/
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.403127 recnetpy-0.1.46/src/recnetpy/
--rw-rw-rw-   0        0        0       26 2022-10-05 15:38:18.000000 recnetpy-0.1.46/src/recnetpy/__init__.py
--rw-rw-rw-   0        0        0     1550 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/client.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.551729 recnetpy-0.1.46/src/recnetpy/dataclasses/
--rw-rw-rw-   0        0        0      534 2022-10-09 18:26:54.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/__init__.py
--rw-rw-rw-   0        0        0    10007 2022-11-23 17:45:44.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/account.py
--rw-rw-rw-   0        0        0     1368 2022-10-28 11:56:21.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/base.py
--rw-rw-rw-   0        0        0     1011 2022-10-24 17:50:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/comment.py
--rw-rw-rw-   0        0        0     7806 2022-11-29 11:45:10.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/event.py
--rw-rw-rw-   0        0        0     1300 2022-11-04 16:30:04.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/event_response.py
--rw-rw-rw-   0        0        0     9314 2022-10-28 11:57:18.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/image.py
--rw-rw-rw-   0        0        0     7413 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/invention.py
--rw-rw-rw-   0        0        0     1371 2022-10-24 17:50:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/invention_version.py
--rw-rw-rw-   0        0        0      740 2022-10-24 17:50:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/loading_screen.py
--rw-rw-rw-   0        0        0      694 2022-10-24 17:50:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/progression.py
--rw-rw-rw-   0        0        0      821 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/promo_external_content.py
--rw-rw-rw-   0        0        0     1679 2022-10-26 17:18:50.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/role.py
--rw-rw-rw-   0        0        0    10867 2022-11-26 10:07:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/room.py
--rw-rw-rw-   0        0        0      852 2022-10-24 17:50:45.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/score.py
--rw-rw-rw-   0        0        0     2177 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/subroom.py
--rw-rw-rw-   0        0        0      701 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/dataclasses/tag.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.629520 recnetpy-0.1.46/src/recnetpy/managers/
--rw-rw-rw-   0        0        0      252 2022-10-05 11:49:19.000000 recnetpy-0.1.46/src/recnetpy/managers/__init__.py
--rw-rw-rw-   0        0        0     4170 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/managers/account_manager.py
--rw-rw-rw-   0        0        0     2035 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/managers/base_manager.py
--rw-rw-rw-   0        0        0     5380 2022-12-01 14:03:41.000000 recnetpy-0.1.46/src/recnetpy/managers/event_manager.py
--rw-rw-rw-   0        0        0     7463 2022-11-09 18:40:47.000000 recnetpy-0.1.46/src/recnetpy/managers/image_manager.py
--rw-rw-rw-   0        0        0     3578 2022-11-25 18:16:37.000000 recnetpy-0.1.46/src/recnetpy/managers/invention_manager.py
--rw-rw-rw-   0        0        0     7202 2022-10-26 13:35:46.000000 recnetpy-0.1.46/src/recnetpy/managers/room_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.670411 recnetpy-0.1.46/src/recnetpy/misc/
--rw-rw-rw-   0        0        0      169 2022-10-05 11:01:10.000000 recnetpy-0.1.46/src/recnetpy/misc/__init__.py
--rw-rw-rw-   0        0        0    10958 2022-10-12 16:38:44.000000 recnetpy-0.1.46/src/recnetpy/misc/api_responses.py
--rw-rw-rw-   0        0        0      589 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/misc/bitmask_decode.py
--rw-rw-rw-   0        0        0      124 2022-10-05 11:42:58.000000 recnetpy-0.1.46/src/recnetpy/misc/constants.py
--rw-rw-rw-   0        0        0      458 2022-10-24 17:57:53.000000 recnetpy-0.1.46/src/recnetpy/misc/date_to_unix.py
--rw-rw-rw-   0        0        0      245 2022-10-05 11:01:01.000000 recnetpy-0.1.46/src/recnetpy/misc/stringify_bulk.py
--rw-rw-rw-   0        0        0      959 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/misc/variable_class.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.707313 recnetpy-0.1.46/src/recnetpy/rest/
--rw-rw-rw-   0        0        0       71 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.757180 recnetpy-0.1.46/src/recnetpy/rest/async_threads/
--rw-rw-rw-   0        0        0       83 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/async_threads/__init__.py
--rw-rw-rw-   0        0        0     1244 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/async_threads/async_thread.py
--rw-rw-rw-   0        0        0     1875 2022-10-09 18:26:54.000000 recnetpy-0.1.46/src/recnetpy/rest/async_threads/async_thread_pool.py
--rw-rw-rw-   0        0        0     1588 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/async_threads/thread_task.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.787099 recnetpy-0.1.46/src/recnetpy/rest/exceptions/
--rw-rw-rw-   0        0        0      159 2022-11-09 18:39:50.000000 recnetpy-0.1.46/src/recnetpy/rest/exceptions/__init__.py
--rw-rw-rw-   0        0        0      213 2022-10-05 10:46:08.000000 recnetpy-0.1.46/src/recnetpy/rest/exceptions/bad_request.py
--rw-rw-rw-   0        0        0      474 2022-10-02 19:24:27.000000 recnetpy-0.1.46/src/recnetpy/rest/exceptions/http_error.py
--rw-rw-rw-   0        0        0      257 2022-10-05 10:45:56.000000 recnetpy-0.1.46/src/recnetpy/rest/exceptions/internal_server_error.py
--rw-rw-rw-   0        0        0      252 2022-10-02 19:12:12.000000 recnetpy-0.1.46/src/recnetpy/rest/exceptions/not_found.py
--rw-rw-rw-   0        0        0     2092 2022-11-09 18:39:44.000000 recnetpy-0.1.46/src/recnetpy/rest/http_client.py
--rw-rw-rw-   0        0        0     2632 2022-11-29 11:48:51.000000 recnetpy-0.1.46/src/recnetpy/rest/request.py
--rw-rw-rw-   0        0        0      397 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/response.py
--rw-rw-rw-   0        0        0     1809 2022-11-26 10:47:49.000000 recnetpy-0.1.46/src/recnetpy/rest/route_builder.py
--rw-rw-rw-   0        0        0     2411 2022-10-02 09:57:14.000000 recnetpy-0.1.46/src/recnetpy/rest/route_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-04 22:09:40.427062 recnetpy-0.1.46/src/recnetpy.egg-info/
--rw-rw-rw-   0        0        0     3242 2022-12-04 22:09:40.000000 recnetpy-0.1.46/src/recnetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2022-12-04 22:09:40.000000 recnetpy-0.1.46/src/recnetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-04 22:09:40.000000 recnetpy-0.1.46/src/recnetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-12-04 22:09:40.000000 recnetpy-0.1.46/src/recnetpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-04 22:09:40.000000 recnetpy-0.1.46/src/recnetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.314626 recnetpy-0.1.47/
+-rw-rw-rw-   0        0        0     1140 2023-05-26 12:49:51.000000 recnetpy-0.1.47/LICENSE
+-rw-rw-rw-   0        0        0     3242 2023-05-26 13:33:58.313629 recnetpy-0.1.47/PKG-INFO
+-rw-rw-rw-   0        0        0     2672 2023-05-26 12:49:51.000000 recnetpy-0.1.47/README.md
+-rw-rw-rw-   0        0        0      715 2023-05-26 13:30:34.000000 recnetpy-0.1.47/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 13:33:58.314626 recnetpy-0.1.47/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.232336 recnetpy-0.1.47/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.242311 recnetpy-0.1.47/src/recnetpy/
+-rw-rw-rw-   0        0        0       26 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/client.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.280718 recnetpy-0.1.47/src/recnetpy/dataclasses/
+-rw-rw-rw-   0        0        0      534 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/__init__.py
+-rw-rw-rw-   0        0        0    10007 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/account.py
+-rw-rw-rw-   0        0        0     1368 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/base.py
+-rw-rw-rw-   0        0        0     1011 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/comment.py
+-rw-rw-rw-   0        0        0     7806 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/event.py
+-rw-rw-rw-   0        0        0     1300 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/event_response.py
+-rw-rw-rw-   0        0        0     9314 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/image.py
+-rw-rw-rw-   0        0        0     7413 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/invention.py
+-rw-rw-rw-   0        0        0     1371 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/invention_version.py
+-rw-rw-rw-   0        0        0      740 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/loading_screen.py
+-rw-rw-rw-   0        0        0      694 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/progression.py
+-rw-rw-rw-   0        0        0      821 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/promo_external_content.py
+-rw-rw-rw-   0        0        0     1679 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/role.py
+-rw-rw-rw-   0        0        0    11138 2023-05-26 13:30:17.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/room.py
+-rw-rw-rw-   0        0        0      852 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/score.py
+-rw-rw-rw-   0        0        0     2177 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/subroom.py
+-rw-rw-rw-   0        0        0      701 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/dataclasses/tag.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.287698 recnetpy-0.1.47/src/recnetpy/managers/
+-rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/__init__.py
+-rw-rw-rw-   0        0        0     4170 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/account_manager.py
+-rw-rw-rw-   0        0        0     2035 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/base_manager.py
+-rw-rw-rw-   0        0        0     5380 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/event_manager.py
+-rw-rw-rw-   0        0        0     7463 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/image_manager.py
+-rw-rw-rw-   0        0        0     3578 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/invention_manager.py
+-rw-rw-rw-   0        0        0     7202 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/managers/room_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.298669 recnetpy-0.1.47/src/recnetpy/misc/
+-rw-rw-rw-   0        0        0      169 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/__init__.py
+-rw-rw-rw-   0        0        0    10958 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/api_responses.py
+-rw-rw-rw-   0        0        0      589 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/bitmask_decode.py
+-rw-rw-rw-   0        0        0      124 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/constants.py
+-rw-rw-rw-   0        0        0      458 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/date_to_unix.py
+-rw-rw-rw-   0        0        0      245 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/stringify_bulk.py
+-rw-rw-rw-   0        0        0      959 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/misc/variable_class.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.304653 recnetpy-0.1.47/src/recnetpy/rest/
+-rw-rw-rw-   0        0        0       71 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.308643 recnetpy-0.1.47/src/recnetpy/rest/async_threads/
+-rw-rw-rw-   0        0        0       83 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/async_threads/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/async_threads/async_thread.py
+-rw-rw-rw-   0        0        0     1875 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/async_threads/async_thread_pool.py
+-rw-rw-rw-   0        0        0     1588 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/async_threads/thread_task.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.312631 recnetpy-0.1.47/src/recnetpy/rest/exceptions/
+-rw-rw-rw-   0        0        0      159 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/exceptions/bad_request.py
+-rw-rw-rw-   0        0        0      474 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/exceptions/http_error.py
+-rw-rw-rw-   0        0        0      257 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/exceptions/internal_server_error.py
+-rw-rw-rw-   0        0        0      252 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/exceptions/not_found.py
+-rw-rw-rw-   0        0        0     2092 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/http_client.py
+-rw-rw-rw-   0        0        0     2632 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/request.py
+-rw-rw-rw-   0        0        0      397 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/response.py
+-rw-rw-rw-   0        0        0     1809 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/route_builder.py
+-rw-rw-rw-   0        0        0     2411 2023-05-26 12:49:51.000000 recnetpy-0.1.47/src/recnetpy/rest/route_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:33:58.259771 recnetpy-0.1.47/src/recnetpy.egg-info/
+-rw-rw-rw-   0        0        0     3242 2023-05-26 13:33:58.000000 recnetpy-0.1.47/src/recnetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-05-26 13:33:58.000000 recnetpy-0.1.47/src/recnetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 13:33:58.000000 recnetpy-0.1.47/src/recnetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-26 13:33:58.000000 recnetpy-0.1.47/src/recnetpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 13:33:58.000000 recnetpy-0.1.47/src/recnetpy.egg-info/top_level.txt
```

### Comparing `recnetpy-0.1.46/LICENSE` & `recnetpy-0.1.47/LICENSE`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/PKG-INFO` & `recnetpy-0.1.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recnetpy
-Version: 0.1.46
+Version: 0.1.47
 Summary: RecNetPy is an API wrapper built in Python for pulling data from RecNet.
 Author: RecNetBot Development
 Project-URL: Homepage, https://github.com/RecNetBot-Development/RecNetPy
 Project-URL: Bug Tracker, https://github.com/RecNetBot-Development/RecNetPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `recnetpy-0.1.46/README.md` & `recnetpy-0.1.47/README.md`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/pyproject.toml` & `recnetpy-0.1.47/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "recnetpy"
-version = "0.1.46"
+version = "0.1.47"
 authors = [
     { name="RecNetBot Development"}
 ]
 description = "RecNetPy is an API wrapper built in Python for pulling data from RecNet."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `recnetpy-0.1.46/src/recnetpy/client.py` & `recnetpy-0.1.47/src/recnetpy/client.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/__init__.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/account.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/account.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/base.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/base.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/comment.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/comment.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/event.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         cached result, if this function has been already called.
 
         :param take: The number of results to return.
         :param skip: The number of results to skip.
         :param force: If true, fetches new data.
         :return: A list of images.
         """
-        if self.images in None or force:
+        if self.images is None or force:
             self.images = await self.client.images.during_event(self.id, take = take, skip = skip)
         return self.images
 
     async def get_creator_player(self, force: bool = False) -> 'Account':
         """
         Fetches the creator of this event. Returns a
         cached result, if this function has been already called.
```

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/event_response.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/event_response.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/image.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/image.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/invention.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/invention.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/invention_version.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/invention_version.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/loading_screen.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/loading_screen.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/progression.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/progression.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/promo_external_content.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/promo_external_content.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/role.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/role.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/room.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,9 +226,20 @@
         accounts: Dict[int, Account] = {}
         for role in roles:
             account = self.client.accounts.create_dataclass(role.account_id)
             role.account = account
             accounts[role.account_id] = account
         data: 'Response[List[AccountResponse]]' = await self.rec_net.accounts.account.bulk.make_request('post', body = {"id": accounts.keys()})
         for data_response in data.data: accounts.get(data_response['accountId']).patch_data(data_response)
+
+        # Search for deleted accounts
+        deleted = []
+        for i in self.roles:
+            if not hasattr(i.account, "username"):
+                deleted.append(i)
+
+        # Eradicate them
+        for i in deleted:
+            self.roles.remove(i)
+
         return self.roles
```

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/score.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/score.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/subroom.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/subroom.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/dataclasses/tag.py` & `recnetpy-0.1.47/src/recnetpy/dataclasses/tag.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/account_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/base_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/event_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/image_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/image_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/invention_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/invention_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/managers/room_manager.py` & `recnetpy-0.1.47/src/recnetpy/managers/room_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/misc/api_responses.py` & `recnetpy-0.1.47/src/recnetpy/misc/api_responses.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/misc/bitmask_decode.py` & `recnetpy-0.1.47/src/recnetpy/misc/bitmask_decode.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/misc/variable_class.py` & `recnetpy-0.1.47/src/recnetpy/misc/variable_class.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/async_threads/async_thread.py` & `recnetpy-0.1.47/src/recnetpy/rest/async_threads/async_thread.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/async_threads/async_thread_pool.py` & `recnetpy-0.1.47/src/recnetpy/rest/async_threads/async_thread_pool.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/async_threads/thread_task.py` & `recnetpy-0.1.47/src/recnetpy/rest/async_threads/thread_task.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/http_client.py` & `recnetpy-0.1.47/src/recnetpy/rest/http_client.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/request.py` & `recnetpy-0.1.47/src/recnetpy/rest/request.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/route_builder.py` & `recnetpy-0.1.47/src/recnetpy/rest/route_builder.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy/rest/route_manager.py` & `recnetpy-0.1.47/src/recnetpy/rest/route_manager.py`

 * *Files identical despite different names*

### Comparing `recnetpy-0.1.46/src/recnetpy.egg-info/PKG-INFO` & `recnetpy-0.1.47/src/recnetpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recnetpy
-Version: 0.1.46
+Version: 0.1.47
 Summary: RecNetPy is an API wrapper built in Python for pulling data from RecNet.
 Author: RecNetBot Development
 Project-URL: Homepage, https://github.com/RecNetBot-Development/RecNetPy
 Project-URL: Bug Tracker, https://github.com/RecNetBot-Development/RecNetPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `recnetpy-0.1.46/src/recnetpy.egg-info/SOURCES.txt` & `recnetpy-0.1.47/src/recnetpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/preemo_worker_sdk-0.5.2.tar.gz` & `tmp/preemo_worker_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preemo_worker_sdk-0.5.2.tar", max compression
+gzip compressed data, was "preemo_worker_sdk-0.6.0.tar", max compression
```

## Comparing `preemo_worker_sdk-0.5.2.tar` & `preemo_worker_sdk-0.6.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.5.2/LICENSE
--rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.5.2/README.md
--rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.5.2/preemo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057207 preemo_worker_sdk-0.5.2/preemo/gen/__init__.py
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057418 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/__init__.py
--rw-r--r--   0        0        0     4333 2023-04-25 19:46:41.903033 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
--rw-r--r--   0        0        0     7285 2023-04-25 19:46:42.071630 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     3035 2023-04-25 19:46:41.903159 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.py
--rw-r--r--   0        0        0     6629 2023-04-25 19:46:42.078426 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
--rw-r--r--   0        0        0     2642 2023-04-25 19:46:41.903266 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.py
--rw-r--r--   0        0        0     4134 2023-04-25 19:46:42.084193 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi
--rw-r--r--   0        0        0     2837 2023-04-25 19:46:41.903373 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
--rw-r--r--   0        0        0     5106 2023-04-25 19:46:42.090178 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
--rw-r--r--   0        0        0     4502 2023-04-25 19:46:41.903470 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
--rw-r--r--   0        0        0     7767 2023-04-25 19:46:42.099799 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-25 19:46:41.903560 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.py
--rw-r--r--   0        0        0     5686 2023-04-25 19:46:42.109202 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
--rw-r--r--   0        0        0     4409 2023-04-25 19:46:41.903662 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
--rw-r--r--   0        0        0     7699 2023-04-25 19:46:42.117663 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
--rw-r--r--   0        0        0     1382 2023-04-25 19:46:41.903764 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.py
--rw-r--r--   0        0        0     1811 2023-04-25 19:46:42.125765 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.pyi
--rw-r--r--   0        0        0     1665 2023-04-25 19:46:41.903852 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.py
--rw-r--r--   0        0        0     3019 2023-04-25 19:46:42.133597 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.pyi
--rw-r--r--   0        0        0     1128 2023-04-25 19:46:41.903952 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.py
--rw-r--r--   0        0        0     1515 2023-04-25 19:46:42.148610 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.pyi
--rw-r--r--   0        0        0     1403 2023-04-25 19:46:41.904045 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.py
--rw-r--r--   0        0        0     1721 2023-04-25 19:46:42.158689 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/register_function_pb2.pyi
--rw-r--r--   0        0        0     1130 2023-05-01 17:44:07.185317 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.py
--rw-r--r--   0        0        0      816 2023-05-01 17:44:07.185506 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
--rw-r--r--   0        0        0     1085 2023-04-25 19:46:41.904240 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.py
--rw-r--r--   0        0        0      786 2023-04-25 19:46:42.174637 preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.057965 preemo_worker_sdk-0.5.2/preemo/gen/models/__init__.py
--rw-r--r--   0        0        0     1104 2023-04-25 19:46:41.904364 preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.py
--rw-r--r--   0        0        0     1129 2023-04-25 19:46:42.181218 preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.pyi
--rw-r--r--   0        0        0     1135 2023-04-25 19:46:41.904467 preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.py
--rw-r--r--   0        0        0     1624 2023-04-25 19:46:42.189956 preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.pyi
--rw-r--r--   0        0        0     1174 2023-04-25 19:46:41.904568 preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.py
--rw-r--r--   0        0        0     1396 2023-04-25 19:46:42.196623 preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-25 19:46:42.058182 preemo_worker_sdk-0.5.2/preemo/gen/services/__init__.py
--rw-r--r--   0        0        0     4369 2023-04-25 19:46:42.046773 preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.py
--rw-r--r--   0        0        0     1302 2023-04-25 19:46:42.206915 preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.pyi
--rw-r--r--   0        0        0    21861 2023-04-25 19:46:42.047102 preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.py
--rw-r--r--   0        0        0     6536 2023-04-25 19:46:42.216498 preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.5.2/preemo/py.typed
--rw-r--r--   0        0        0     2500 2023-05-01 17:44:07.185692 preemo_worker_sdk-0.5.2/preemo/worker/__init__.py
--rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.5.2/preemo/worker/__init__.pyi
--rw-r--r--   0        0        0    13624 2023-05-02 18:39:31.234171 preemo_worker_sdk-0.5.2/preemo/worker/_artifact_manager.py
--rw-r--r--   0        0        0     1959 2023-05-01 17:44:07.186566 preemo_worker_sdk-0.5.2/preemo/worker/_env_manager.py
--rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.5.2/preemo/worker/_function_registry.py
--rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.5.2/preemo/worker/_messaging_client.py
--rw-r--r--   0        0        0     1394 2023-05-01 17:44:07.186878 preemo_worker_sdk-0.5.2/preemo/worker/_sdk_server.py
--rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.5.2/preemo/worker/_sdk_service.py
--rw-r--r--   0        0        0     1286 2023-04-25 19:43:44.759473 preemo_worker_sdk-0.5.2/preemo/worker/_types.py
--rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.5.2/preemo/worker/_validation.py
--rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.5.2/preemo/worker/_worker_client.py
--rw-r--r--   0        0        0     1852 2023-05-02 21:07:16.127981 preemo_worker_sdk-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3985 2023-05-26 16:30:50.161867 preemo_worker_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.6.0/preemo/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-26 16:12:16.075370 preemo_worker_sdk-0.6.0/preemo/gen/__init__.py
+-rw-r--r--   0        0        0      306 2023-05-26 16:12:16.075578 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/__init__.py
+-rw-r--r--   0        0        0     4333 2023-05-26 16:12:15.906172 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7285 2023-05-26 16:12:16.085185 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     3035 2023-05-26 16:12:15.906316 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_create_artifact_pb2.py
+-rw-r--r--   0        0        0     6629 2023-05-26 16:12:16.093587 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
+-rw-r--r--   0        0        0     2642 2023-05-26 16:12:15.906430 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_execute_function_pb2.py
+-rw-r--r--   0        0        0     4134 2023-05-26 16:12:16.102272 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi
+-rw-r--r--   0        0        0     2837 2023-05-26 16:12:15.906547 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
+-rw-r--r--   0        0        0     5106 2023-05-26 16:12:16.109769 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4502 2023-05-26 16:12:15.906655 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
+-rw-r--r--   0        0        0     7767 2023-05-26 16:12:16.118325 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-05-26 16:12:15.906781 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_pb2.py
+-rw-r--r--   0        0        0     5686 2023-05-26 16:12:16.126573 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4409 2023-05-26 16:12:15.906888 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
+-rw-r--r--   0        0        0     7699 2023-05-26 16:12:16.132809 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
+-rw-r--r--   0        0        0     1382 2023-05-26 16:12:15.907003 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/check_function_pb2.py
+-rw-r--r--   0        0        0     1811 2023-05-26 16:12:16.142045 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/check_function_pb2.pyi
+-rw-r--r--   0        0        0     1665 2023-05-26 16:12:15.907130 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/execute_function_pb2.py
+-rw-r--r--   0        0        0     3019 2023-05-26 16:12:16.147458 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/execute_function_pb2.pyi
+-rw-r--r--   0        0        0     1128 2023-05-26 16:12:15.907263 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/header_pb2.py
+-rw-r--r--   0        0        0     1515 2023-05-26 16:12:16.154092 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/header_pb2.pyi
+-rw-r--r--   0        0        0     2654 2023-05-26 16:30:50.162835 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/register_function_pb2.py
+-rw-r--r--   0        0        0     8694 2023-05-26 16:30:50.163017 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/register_function_pb2.pyi
+-rw-r--r--   0        0        0     1130 2023-05-26 16:12:15.907509 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/sdk_server_ready_pb2.py
+-rw-r--r--   0        0        0      816 2023-05-26 16:12:16.175241 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
+-rw-r--r--   0        0        0     1085 2023-05-26 16:12:15.907617 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/terminate_pb2.py
+-rw-r--r--   0        0        0      786 2023-05-26 16:12:16.191467 preemo_worker_sdk-0.6.0/preemo/gen/endpoints/terminate_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-05-26 16:12:16.076144 preemo_worker_sdk-0.6.0/preemo/gen/models/__init__.py
+-rw-r--r--   0        0        0     1104 2023-05-26 16:12:15.907771 preemo_worker_sdk-0.6.0/preemo/gen/models/artifact_type_pb2.py
+-rw-r--r--   0        0        0     1129 2023-05-26 16:12:16.206768 preemo_worker_sdk-0.6.0/preemo/gen/models/artifact_type_pb2.pyi
+-rw-r--r--   0        0        0     1135 2023-05-26 16:12:15.907881 preemo_worker_sdk-0.6.0/preemo/gen/models/registered_function_pb2.py
+-rw-r--r--   0        0        0     1624 2023-05-26 16:12:16.214033 preemo_worker_sdk-0.6.0/preemo/gen/models/registered_function_pb2.pyi
+-rw-r--r--   0        0        0     1174 2023-05-26 16:12:15.907996 preemo_worker_sdk-0.6.0/preemo/gen/models/value_pb2.py
+-rw-r--r--   0        0        0     1508 2023-05-26 16:30:50.163241 preemo_worker_sdk-0.6.0/preemo/gen/models/value_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-05-26 16:12:16.076417 preemo_worker_sdk-0.6.0/preemo/gen/services/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-26 16:12:16.059393 preemo_worker_sdk-0.6.0/preemo/gen/services/sdk_pb2_grpc.py
+-rw-r--r--   0        0        0     1302 2023-05-26 16:12:16.230948 preemo_worker_sdk-0.6.0/preemo/gen/services/sdk_pb2_grpc.pyi
+-rw-r--r--   0        0        0    21861 2023-05-26 16:12:16.059578 preemo_worker_sdk-0.6.0/preemo/gen/services/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     6536 2023-05-26 16:12:16.241641 preemo_worker_sdk-0.6.0/preemo/gen/services/worker_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.6.0/preemo/py.typed
+-rw-r--r--   0        0        0     2500 2023-05-01 17:44:07.185692 preemo_worker_sdk-0.6.0/preemo/worker/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-26 16:30:50.163435 preemo_worker_sdk-0.6.0/preemo/worker/__init__.pyi
+-rw-r--r--   0        0        0    13397 2023-05-25 18:07:08.307281 preemo_worker_sdk-0.6.0/preemo/worker/_artifact_manager.py
+-rw-r--r--   0        0        0     1053 2023-05-26 16:30:50.163704 preemo_worker_sdk-0.6.0/preemo/worker/_bytes.py
+-rw-r--r--   0        0        0     1959 2023-05-17 17:20:06.344682 preemo_worker_sdk-0.6.0/preemo/worker/_env_manager.py
+-rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.6.0/preemo/worker/_function_registry.py
+-rw-r--r--   0        0        0    11315 2023-05-17 17:20:06.345067 preemo_worker_sdk-0.6.0/preemo/worker/_messaging_client.py
+-rw-r--r--   0        0        0     1394 2023-05-01 17:44:07.186878 preemo_worker_sdk-0.6.0/preemo/worker/_sdk_server.py
+-rw-r--r--   0        0        0     3619 2023-05-25 21:19:52.423163 preemo_worker_sdk-0.6.0/preemo/worker/_sdk_service.py
+-rw-r--r--   0        0        0     1286 2023-05-18 23:53:20.250327 preemo_worker_sdk-0.6.0/preemo/worker/_types.py
+-rw-r--r--   0        0        0      740 2023-05-26 16:30:50.163992 preemo_worker_sdk-0.6.0/preemo/worker/_validation.py
+-rw-r--r--   0        0        0    10345 2023-05-26 16:30:50.164325 preemo_worker_sdk-0.6.0/preemo/worker/_worker_client.py
+-rw-r--r--   0        0        0     1852 2023-05-26 16:31:29.165000 preemo_worker_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.6.0/PKG-INFO
```

### Comparing `preemo_worker_sdk-0.5.2/LICENSE` & `preemo_worker_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_create_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_create_artifact_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_execute_function_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/check_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/check_function_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/check_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/execute_function_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/header_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/header_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/header_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/sdk_server_ready_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/sdk_server_ready_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/terminate_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/endpoints/terminate_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/endpoints/terminate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/models/artifact_type_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/artifact_type_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/models/artifact_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/models/registered_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/registered_function_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/models/registered_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.py` & `preemo_worker_sdk-0.6.0/preemo/gen/models/value_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/models/value_pb2.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/models/value_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class Value(google.protobuf.message.Message):
+    """TODO(adrian@preemo.io, 06/01/2023): move this to an ArtifactId message with an optional string value"""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NULL_VALUE_FIELD_NUMBER: builtins.int
     ARTIFACT_ID_FIELD_NUMBER: builtins.int
     null_value: google.protobuf.struct_pb2.NullValue.ValueType
     artifact_id: builtins.str
     """Unique identifier for a file stored in the cloud."""
```

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.py` & `preemo_worker_sdk-0.6.0/preemo/gen/services/sdk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/services/sdk_pb2_grpc.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/services/sdk_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.py` & `preemo_worker_sdk-0.6.0/preemo/gen/services/worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/gen/services/worker_pb2_grpc.pyi` & `preemo_worker_sdk-0.6.0/preemo/gen/services/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/__init__.py` & `preemo_worker_sdk-0.6.0/preemo/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_artifact_manager.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_artifact_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import concurrent.futures
 import enum
 import gzip
 import math
 import os
-from typing import Dict, List, Protocol, runtime_checkable
+from typing import Dict, List, NewType, Protocol, runtime_checkable
 
 import requests
 from pydantic import StrictInt
 
 from preemo.gen.endpoints.batch_allocate_artifact_part_pb2 import (
     AllocateArtifactPartConfig,
     AllocateArtifactPartConfigMetadata,
@@ -37,19 +37,17 @@
 )
 from preemo.gen.models.artifact_type_pb2 import (
     ARTIFACT_TYPE_PARAMS,
     ARTIFACT_TYPE_RESULT,
 )
 from preemo.worker._env_manager import EnvManager
 from preemo.worker._messaging_client import IMessagingClient
-from preemo.worker._types import ImmutableModel, StringValue
+from preemo.worker._types import ImmutableModel
 
-
-class ArtifactId(StringValue):
-    pass
+ArtifactId = NewType("ArtifactId", str)
 
 
 class Artifact(ImmutableModel):
     id: ArtifactId
     part_size_threshold: StrictInt
 
 
@@ -99,15 +97,15 @@
                 data=gzip.compress(content),
                 headers={
                     "Content-Encoding": "gzip",
                     "Content-Type": "application/octet-stream",
                 },
             )
 
-            # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
+            # TODO(adrian@preemo.io, 06/15/2023): should retry if it fails
             if not response.ok:
                 raise Exception(f"unexpected response while uploading: {response}")
 
     def _read_content(self, *, url: str) -> bytes:
         if EnvManager.is_development:
             # treat url as file path
             with open(url, "rb") as fin:
@@ -117,15 +115,15 @@
                 url=url,
                 headers={
                     "Accept-Encoding": "gzip",
                     "Content-Type": "application/octet-stream",
                 },
             )
 
-            # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
+            # TODO(adrian@preemo.io, 06/15/2023): should retry if it fails
             if not response.ok:
                 raise Exception(f"unexpected response while downloading: {response}")
 
             return response.content
 
     def _create_artifacts(
         self,
@@ -145,15 +143,15 @@
         }
         response = self._messaging_client.batch_create_artifact(
             BatchCreateArtifactRequest(configs_by_index=configs_by_index)
         )
 
         return [
             Artifact(
-                id=ArtifactId(value=result.artifact_id),
+                id=ArtifactId(result.artifact_id),
                 part_size_threshold=result.part_size_threshold,
             )
             for _, result in sorted(
                 response.results_by_index.items(), key=lambda x: x[0]
             )
         ]
 
@@ -167,61 +165,55 @@
     def create_artifacts(
         self, *, contents: List[bytes], type_: ArtifactType
     ) -> List[ArtifactId]:
         artifacts = self._create_artifacts(count=len(contents), type_=type_)
         if len(artifacts) != len(contents):
             raise Exception("expected artifacts and contents lengths to be equal")
 
-        allocate_configs_by_artifact_id_value: Dict[
-            str, AllocateArtifactPartConfig
-        ] = {}
-        upload_configs_by_artifact_id_value: Dict[str, GetArtifactUploadUrlConfig] = {}
+        allocate_configs_by_artifact_id: Dict[str, AllocateArtifactPartConfig] = {}
+        upload_configs_by_artifact_id: Dict[str, GetArtifactUploadUrlConfig] = {}
         for artifact, content in zip(artifacts, contents):
             part_count = ArtifactManager._calculate_part_count(
                 content_length=len(content),
                 part_size_threshold=artifact.part_size_threshold,
             )
 
-            allocate_configs_by_artifact_id_value[
-                artifact.id.value
-            ] = AllocateArtifactPartConfig(
+            allocate_configs_by_artifact_id[artifact.id] = AllocateArtifactPartConfig(
                 metadatas_by_part_number={
                     part_number: AllocateArtifactPartConfigMetadata()
                     for part_number in range(part_count)
                 }
             )
 
-            upload_configs_by_artifact_id_value[
-                artifact.id.value
-            ] = GetArtifactUploadUrlConfig(
+            upload_configs_by_artifact_id[artifact.id] = GetArtifactUploadUrlConfig(
                 metadatas_by_part_number={
                     part_number: GetArtifactUploadUrlConfigMetadata()
                     for part_number in range(part_count)
                 }
             )
 
         self._messaging_client.batch_allocate_artifact_part(
             BatchAllocateArtifactPartRequest(
-                configs_by_artifact_id=allocate_configs_by_artifact_id_value
+                configs_by_artifact_id=allocate_configs_by_artifact_id
             )
         )
 
         get_url_response = self._messaging_client.batch_get_artifact_upload_url(
             BatchGetArtifactUploadUrlRequest(
-                configs_by_artifact_id=upload_configs_by_artifact_id_value
+                configs_by_artifact_id=upload_configs_by_artifact_id
             )
         )
 
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=EnvManager.max_upload_threads
         ) as executor:
             futures = []
             for artifact, content in zip(artifacts, contents):
                 content_view = memoryview(content)
-                result = get_url_response.results_by_artifact_id[artifact.id.value]
+                result = get_url_response.results_by_artifact_id[artifact.id]
 
                 for part_number, metadata in result.metadatas_by_part_number.items():
                     start_index = part_number * artifact.part_size_threshold
                     part_content = content_view[
                         start_index : start_index + artifact.part_size_threshold
                     ]
 
@@ -229,15 +221,15 @@
                         executor.submit(
                             self._write_content,
                             content=part_content,
                             url=metadata.signed_url,
                         )
                     )
 
-            # TODO(adrian@preemo.io, 04/15/2023): add exception handling
+            # TODO(adrian@preemo.io, 06/15/2023): add exception handling
             done, not_done = concurrent.futures.wait(
                 futures, return_when=concurrent.futures.ALL_COMPLETED
             )
 
             if len(not_done) != 0:
                 raise Exception("expected incomplete future set to be empty")
 
@@ -247,15 +239,15 @@
             for future in done:
                 # this will raise any exceptions raised in the thread
                 future.result()
 
         self._messaging_client.batch_finalize_artifact(
             BatchFinalizeArtifactRequest(
                 configs_by_artifact_id={
-                    artifact.id.value: FinalizeArtifactConfig(
+                    artifact.id: FinalizeArtifactConfig(
                         total_size=len(content),
                         part_count=ArtifactManager._calculate_part_count(
                             content_length=len(content),
                             part_size_threshold=artifact.part_size_threshold,
                         ),
                     )
                     for artifact, content in zip(artifacts, contents)
@@ -272,57 +264,56 @@
 
         return contents[0]
 
     def get_artifacts(self, *, artifact_ids: List[ArtifactId]) -> List[bytes]:
         get_artifact_response = self._messaging_client.batch_get_artifact(
             BatchGetArtifactRequest(
                 configs_by_artifact_id={
-                    artifact_id.value: GetArtifactConfig()
-                    for artifact_id in artifact_ids
+                    artifact_id: GetArtifactConfig() for artifact_id in artifact_ids
                 }
             )
         )
 
-        configs_by_artifact_id_value = {
-            artifact_id_value: GetArtifactDownloadUrlConfig(
+        configs_by_artifact_id = {
+            artifact_id: GetArtifactDownloadUrlConfig(
                 metadatas_by_part_number={
                     part_number: GetArtifactDownloadUrlConfigMetadata()
                     for part_number in range(result.part_count)
                 }
             )
-            for artifact_id_value, result in get_artifact_response.results_by_artifact_id.items()
+            for artifact_id, result in get_artifact_response.results_by_artifact_id.items()
         }
         get_url_response = self._messaging_client.batch_get_artifact_download_url(
             BatchGetArtifactDownloadUrlRequest(
-                configs_by_artifact_id=configs_by_artifact_id_value
+                configs_by_artifact_id=configs_by_artifact_id
             )
         )
 
         with concurrent.futures.ThreadPoolExecutor(
             max_workers=EnvManager.max_download_threads
         ) as executor:
             futures_by_artifact_id_and_part_number: Dict[
                 ArtifactId, Dict[int, concurrent.futures.Future]
             ] = {}
             for (
-                artifact_id_value,
+                artifact_id,
                 artifact_part_result,
             ) in get_url_response.results_by_artifact_id.items():
                 futures_by_part_number: Dict[int, concurrent.futures.Future] = {}
                 for (
                     part_number,
                     metadata,
                 ) in artifact_part_result.metadatas_by_part_number.items():
                     futures_by_part_number[part_number] = executor.submit(
                         self._read_content,
                         url=metadata.signed_url,
                     )
 
                 futures_by_artifact_id_and_part_number[
-                    ArtifactId(value=artifact_id_value)
+                    ArtifactId(artifact_id)
                 ] = futures_by_part_number
 
             futures = [
                 future
                 for futures_by_part_number in futures_by_artifact_id_and_part_number.values()
                 for future in futures_by_part_number.values()
             ]
@@ -339,18 +330,18 @@
 
             results: List[bytes] = []
             for artifact_id in artifact_ids:
                 futures_by_part_number = futures_by_artifact_id_and_part_number[
                     artifact_id
                 ]
                 get_artifact_result = get_artifact_response.results_by_artifact_id[
-                    artifact_id.value
+                    artifact_id
                 ]
 
-                # TODO(adrian@preemo.io, 04/20/2023): Consider other options for constructing the byte result,
+                # TODO(adrian@preemo.io, 06/20/2023): Consider other options for constructing the byte result,
                 # such as a memory-mapped file or BytesIO
                 result = bytearray()
                 for part_number, future in sorted(
                     futures_by_part_number.items(), key=lambda x: x[0]
                 ):
                     content = future.result()
 
@@ -362,11 +353,11 @@
                             )
 
                     result.extend(content)
 
                 if len(result) != get_artifact_result.total_size:
                     raise Exception("expected result object size to equal total_size")
 
-                # TODO(adrian@preemo.io, 04/20/2023): do i need to convert to bytes here? Is bytearray just masquerading as bytes?
+                # TODO(adrian@preemo.io, 06/20/2023): do i need to convert to bytes here? Is bytearray just masquerading as bytes?
                 results.append(result)
 
         return results
```

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_env_manager.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_env_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     value = os.getenv(key=name)
     if value is None or len(value) == 0:
         return None
 
     return value
 
 
-# TODO(adrian@preemo.io, 04/24/2023): test this
+# TODO(adrian@preemo.io, 05/24/2023): test this
 def _get_optional_int_env(name: str) -> Optional[int]:
     value = _get_string_env(name)
     if value is None:
         return None
 
     try:
         return int(value)
```

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_function_registry.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_function_registry.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_messaging_client.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_messaging_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self, request: SdkServerReadyRequest
     ) -> SdkServerReadyResponse:
         pass
 
 
 class MessagingClient:
     def __init__(self, *, worker_server_url: str) -> None:
-        # TODO(adrian@preemo.io, 03/25/2023): investigate whether it makes sense to use secure_channel instead
+        # TODO(adrian@preemo.io, 06/25/2023): investigate whether it makes sense to use secure_channel instead
         self._channel = grpc.insecure_channel(target=worker_server_url)
         self._worker_service = WorkerServiceStub(self._channel)
 
         self._initiate(HeaderRequest(version=__version__))
 
     def _initiate(self, request: HeaderRequest) -> HeaderResponse:
         return self._worker_service.Initiate(request)
```

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_sdk_server.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_sdk_server.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_sdk_service.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_sdk_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from preemo.gen.models.value_pb2 import Value
 from preemo.gen.services.sdk_pb2_grpc import SdkServiceServicer
 from preemo.worker._artifact_manager import ArtifactId, ArtifactType, IArtifactManager
 from preemo.worker._function_registry import FunctionRegistry
 from preemo.worker._types import assert_never
 
 
+# TODO(adrian@preemo.io, 05/11/2023): add logging
 class SdkService(SdkServiceServicer):
     @staticmethod
     def _validate_execute_function_request(
         request: ExecuteFunctionRequest, context: grpc.ServicerContext
     ) -> None:
         if not request.HasField("function_to_execute"):
             context.abort(
@@ -55,15 +56,15 @@
             raise Exception("expected value to have kind")
 
         if kind == "null_value":
             return None
 
         if kind == "artifact_id":
             return self._artifact_manager.get_artifact(
-                artifact_id=ArtifactId(value=value.artifact_id)
+                artifact_id=ArtifactId(value.artifact_id)
             )
 
         assert_never(kind)
 
     def ExecuteFunction(
         self, request: ExecuteFunctionRequest, context: grpc.ServicerContext
     ) -> ExecuteFunctionResponse:
@@ -83,19 +84,19 @@
             result = func()
         else:
             result = func(parameter_value)
 
         if result is None:
             result_value = Value(null_value=NULL_VALUE)
         else:
-            # TODO(adrian@preemo.io, 04/04/2023): validate that result is bytes?
+            # TODO(adrian@preemo.io, 06/04/2023): validate that result is bytes?
             result_artifact_id = self._artifact_manager.create_artifact(
                 content=result, type_=ArtifactType.RESULT
             )
-            result_value = Value(artifact_id=result_artifact_id.value)
+            result_value = Value(artifact_id=result_artifact_id)
 
         return ExecuteFunctionResponse(result=result_value)
 
     def Terminate(
         self, request: TerminateRequest, context: grpc.ServicerContext
     ) -> TerminateResponse:
         self._terminate_server()
```

### Comparing `preemo_worker_sdk-0.5.2/preemo/worker/_types.py` & `preemo_worker_sdk-0.6.0/preemo/worker/_types.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.5.2/pyproject.toml` & `preemo_worker_sdk-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preemo_worker_sdk"
-version = "0.5.2"
+version = "0.6.0"
 description = ""
 license = "MIT"
 authors = [
   "Forrest Moret <forrest@preemo.io>",
   "Adrian Miguel <adrian@preemo.io>",
 ]
 readme = "README.md"
@@ -15,15 +15,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 packages = [
   { include = "preemo" },
 ]
 
-# TODO(adrian@preemo.io, 05/01/2023): Push these versions as low as possible to make it easier for users to meet the requirements
+# TODO(adrian@preemo.io, 06/01/2023): Push these versions as low as possible to make it easier for users to meet the requirements
 [tool.poetry.dependencies]
 grpcio = "^1.51.3"
 protobuf = "^4.21.12"
 pydantic = "^1.10.6"
 python = "^3.8.13"
 requests = "^2.28.2"
 
@@ -31,15 +31,15 @@
 autoflake = "2.0.1"
 black = "22.3.0"
 build = "0.10.0"
 flake8 = "6.0.0"
 grpc-stubs = "1.24.12"
 grpcio-tools = "1.51.3"
 isort = "5.10.1"
-mypy = "1.0.0"
+mypy = "1.3.0"
 mypy-protobuf = "3.4.0"
 pep8-naming = "0.13.0"
 pytest = "7.2.1"
 twine = "4.0.2"
 types-protobuf = "4.21.0.4"
 types-requests = "2.28.11.17"
```

### Comparing `preemo_worker_sdk-0.5.2/PKG-INFO` & `preemo_worker_sdk-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: preemo-worker-sdk
-Version: 0.5.2
+Version: 0.6.0
 Summary: 
 Home-page: https://www.preemo.io/
 License: MIT
 Author: Forrest Moret
 Author-email: forrest@preemo.io
 Requires-Python: >=3.8.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: grpcio (>=1.51.3,<2.0.0)
 Requires-Dist: protobuf (>=4.21.12,<5.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/Preemo-Inc/worker-sdk
 Description-Content-Type: text/markdown
 
@@ -53,15 +52,61 @@
 ```python
 @register
 def do_something(params: str):
     # registers with name do_something in the global namespace
     ...
 ```
 
-At the moment, only functions that take 0 or 1 bytes arguments will work. These functions should also either return `None` or bytes.
+At the moment, only functions that take 0 or 1 `bytes` arguments will work. These functions should also either return `None` or `bytes`.
+
+#### Resource Requirements
+
+If your function has particular resource requirements, you should specify those during registration.
+
+For example, if your function needs 4 cpu cores to run effectively, you can pass a configuration object.
+
+```python
+from preemo.worker import register
+
+@register(name="some_name", namespace="dev", cpu_cores=4)
+def do_something(params: bytes):
+    ...
+```
+
+You can specify the memory and/or storage requirments in either Mebibytes (`MiB`) or Gibibytes (`GiB`).
+
+```python
+from preemo.worker import register
+
+@register(name="some_name", namespace="dev", memory={ "MiB": 100 }, storage={ "GiB": 10 })
+def do_something(params: bytes):
+    ...
+```
+
+If you need GPUs to effectively run your function, you may pass the specific model to use.
+
+```python
+from preemo.worker import register
+
+@register(name="some_name", namespace="dev", gpu_model="nvidia-tesla-k80")
+def do_something(params: bytes):
+    ...
+```
+
+Along with a gpu model, you may pass a number of gpu devices needed.
+
+```python
+from preemo.worker import register
+
+@register(name="some_name", namespace="dev", gpu_model="nvidia-tesla-k80", gpu_count=2)
+def do_something(params: bytes):
+    ...
+```
+
+<!-- TODO(adrian@preemo.io, 06/01/2023): Include a list of supported gpu models -->
 
 ### Execute Function
 
 In order to execute a function that you have previously registered with Preemo workers, you can use `get_function`.
 
 ```python
 from preemo.worker import get_function
```


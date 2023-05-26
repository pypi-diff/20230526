# Comparing `tmp/alibabacloud_pai-dlc20201203-1.2.5.tar.gz` & `tmp/alibabacloud_pai-dlc20201203-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.5.tar", last modified: Thu Mar 23 03:45:30 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.6.tar", last modified: Fri May 26 02:14:31 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203-1.2.5.tar` & `alibabacloud_pai-dlc20201203-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/
--rw-r--r--   0 root         (0) root         (0)      661 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72862 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   190516 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2023-03-23 03:45:30.000000 alibabacloud_pai-dlc20201203-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      750 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73550 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   196320 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/ChangeLog.md` & `alibabacloud_pai-dlc20201203-1.2.6/ChangeLog.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-03-23 Version: 1.2.5
+- Change the type of RequestId to string in GetJobEvents API.
+
 2023-01-04 Version: 1.2.4
 - Support images from private docker registry.
 
 2022-12-13 Version: 1.2.3
 - CreateJob supports params SuccessPolicy.
 
 2022-07-26 Version: 1.2.1
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/LICENSE` & `alibabacloud_pai-dlc20201203-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203
-Version: 1.2.5
+Version: 1.2.6
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/README-CN.md` & `alibabacloud_pai-dlc20201203-1.2.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/README.md` & `alibabacloud_pai-dlc20201203-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,19 +518,25 @@
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.delete_tensorboard_with_options_async(tensorboard_id, request, headers, runtime)
 
     def get_job_with_options(
         self,
         job_id: str,
+        request: pai_dlc_20201203_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_dlc_20201203_models.GetJobResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.need_detail):
+            query['NeedDetail'] = request.need_detail
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJob',
             version='2020-12-03',
             protocol='HTTPS',
             pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}',
             method='GET',
@@ -543,19 +549,25 @@
             pai_dlc_20201203_models.GetJobResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def get_job_with_options_async(
         self,
         job_id: str,
+        request: pai_dlc_20201203_models.GetJobRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_dlc_20201203_models.GetJobResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.need_detail):
+            query['NeedDetail'] = request.need_detail
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetJob',
             version='2020-12-03',
             protocol='HTTPS',
             pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}',
             method='GET',
@@ -568,26 +580,28 @@
             pai_dlc_20201203_models.GetJobResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_job(
         self,
         job_id: str,
+        request: pai_dlc_20201203_models.GetJobRequest,
     ) -> pai_dlc_20201203_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_job_with_options(job_id, headers, runtime)
+        return self.get_job_with_options(job_id, request, headers, runtime)
 
     async def get_job_async(
         self,
         job_id: str,
+        request: pai_dlc_20201203_models.GetJobRequest,
     ) -> pai_dlc_20201203_models.GetJobResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.get_job_with_options_async(job_id, headers, runtime)
+        return await self.get_job_with_options_async(job_id, request, headers, runtime)
 
     def get_job_events_with_options(
         self,
         job_id: str,
         request: pai_dlc_20201203_models.GetJobEventsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1152,69 +1152,117 @@
 
 
 class JobElasticSpec(TeaModel):
     def __init__(
         self,
         aimaster_docker_image: str = None,
         aimaster_type: str = None,
+        edpmax_parallelism: int = None,
+        edpmin_parallelism: int = None,
+        elastic_strategy: str = None,
         enable_aimaster: bool = None,
+        enable_edp: bool = None,
         enable_elastic_training: bool = None,
+        enable_ps_job_elastic_ps: bool = None,
         enable_ps_job_elastic_worker: bool = None,
+        enable_ps_resource_estimate: bool = None,
         max_parallelism: int = None,
         min_parallelism: int = None,
+        psmax_parallelism: int = None,
+        psmin_parallelism: int = None,
     ):
         self.aimaster_docker_image = aimaster_docker_image
         self.aimaster_type = aimaster_type
+        self.edpmax_parallelism = edpmax_parallelism
+        self.edpmin_parallelism = edpmin_parallelism
+        self.elastic_strategy = elastic_strategy
         self.enable_aimaster = enable_aimaster
+        self.enable_edp = enable_edp
         self.enable_elastic_training = enable_elastic_training
+        self.enable_ps_job_elastic_ps = enable_ps_job_elastic_ps
         self.enable_ps_job_elastic_worker = enable_ps_job_elastic_worker
+        self.enable_ps_resource_estimate = enable_ps_resource_estimate
         self.max_parallelism = max_parallelism
         self.min_parallelism = min_parallelism
+        self.psmax_parallelism = psmax_parallelism
+        self.psmin_parallelism = psmin_parallelism
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.aimaster_docker_image is not None:
             result['AIMasterDockerImage'] = self.aimaster_docker_image
         if self.aimaster_type is not None:
             result['AIMasterType'] = self.aimaster_type
+        if self.edpmax_parallelism is not None:
+            result['EDPMaxParallelism'] = self.edpmax_parallelism
+        if self.edpmin_parallelism is not None:
+            result['EDPMinParallelism'] = self.edpmin_parallelism
+        if self.elastic_strategy is not None:
+            result['ElasticStrategy'] = self.elastic_strategy
         if self.enable_aimaster is not None:
             result['EnableAIMaster'] = self.enable_aimaster
+        if self.enable_edp is not None:
+            result['EnableEDP'] = self.enable_edp
         if self.enable_elastic_training is not None:
             result['EnableElasticTraining'] = self.enable_elastic_training
+        if self.enable_ps_job_elastic_ps is not None:
+            result['EnablePsJobElasticPS'] = self.enable_ps_job_elastic_ps
         if self.enable_ps_job_elastic_worker is not None:
             result['EnablePsJobElasticWorker'] = self.enable_ps_job_elastic_worker
+        if self.enable_ps_resource_estimate is not None:
+            result['EnablePsResourceEstimate'] = self.enable_ps_resource_estimate
         if self.max_parallelism is not None:
             result['MaxParallelism'] = self.max_parallelism
         if self.min_parallelism is not None:
             result['MinParallelism'] = self.min_parallelism
+        if self.psmax_parallelism is not None:
+            result['PSMaxParallelism'] = self.psmax_parallelism
+        if self.psmin_parallelism is not None:
+            result['PSMinParallelism'] = self.psmin_parallelism
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AIMasterDockerImage') is not None:
             self.aimaster_docker_image = m.get('AIMasterDockerImage')
         if m.get('AIMasterType') is not None:
             self.aimaster_type = m.get('AIMasterType')
+        if m.get('EDPMaxParallelism') is not None:
+            self.edpmax_parallelism = m.get('EDPMaxParallelism')
+        if m.get('EDPMinParallelism') is not None:
+            self.edpmin_parallelism = m.get('EDPMinParallelism')
+        if m.get('ElasticStrategy') is not None:
+            self.elastic_strategy = m.get('ElasticStrategy')
         if m.get('EnableAIMaster') is not None:
             self.enable_aimaster = m.get('EnableAIMaster')
+        if m.get('EnableEDP') is not None:
+            self.enable_edp = m.get('EnableEDP')
         if m.get('EnableElasticTraining') is not None:
             self.enable_elastic_training = m.get('EnableElasticTraining')
+        if m.get('EnablePsJobElasticPS') is not None:
+            self.enable_ps_job_elastic_ps = m.get('EnablePsJobElasticPS')
         if m.get('EnablePsJobElasticWorker') is not None:
             self.enable_ps_job_elastic_worker = m.get('EnablePsJobElasticWorker')
+        if m.get('EnablePsResourceEstimate') is not None:
+            self.enable_ps_resource_estimate = m.get('EnablePsResourceEstimate')
         if m.get('MaxParallelism') is not None:
             self.max_parallelism = m.get('MaxParallelism')
         if m.get('MinParallelism') is not None:
             self.min_parallelism = m.get('MinParallelism')
+        if m.get('PSMaxParallelism') is not None:
+            self.psmax_parallelism = m.get('PSMaxParallelism')
+        if m.get('PSMinParallelism') is not None:
+            self.psmin_parallelism = m.get('PSMinParallelism')
         return self
 
 
 class JobItemCodeSource(TeaModel):
     def __init__(
         self,
         branch: str = None,
@@ -1840,14 +1888,97 @@
                 temp_model = Metric()
                 self.metrics.append(temp_model.from_map(k))
         if m.get('NodeName') is not None:
             self.node_name = m.get('NodeName')
         return self
 
 
+class PodItem(TeaModel):
+    def __init__(
+        self,
+        gmt_create_time: str = None,
+        gmt_finish_time: str = None,
+        gmt_start_time: str = None,
+        history_pods: List['PodItem'] = None,
+        ip: str = None,
+        pod_id: str = None,
+        pod_uid: str = None,
+        status: str = None,
+        type: str = None,
+    ):
+        self.gmt_create_time = gmt_create_time
+        self.gmt_finish_time = gmt_finish_time
+        self.gmt_start_time = gmt_start_time
+        self.history_pods = history_pods
+        self.ip = ip
+        self.pod_id = pod_id
+        self.pod_uid = pod_uid
+        self.status = status
+        self.type = type
+
+    def validate(self):
+        if self.history_pods:
+            for k in self.history_pods:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.gmt_create_time is not None:
+            result['GmtCreateTime'] = self.gmt_create_time
+        if self.gmt_finish_time is not None:
+            result['GmtFinishTime'] = self.gmt_finish_time
+        if self.gmt_start_time is not None:
+            result['GmtStartTime'] = self.gmt_start_time
+        result['HistoryPods'] = []
+        if self.history_pods is not None:
+            for k in self.history_pods:
+                result['HistoryPods'].append(k.to_map() if k else None)
+        if self.ip is not None:
+            result['Ip'] = self.ip
+        if self.pod_id is not None:
+            result['PodId'] = self.pod_id
+        if self.pod_uid is not None:
+            result['PodUid'] = self.pod_uid
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.type is not None:
+            result['Type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GmtCreateTime') is not None:
+            self.gmt_create_time = m.get('GmtCreateTime')
+        if m.get('GmtFinishTime') is not None:
+            self.gmt_finish_time = m.get('GmtFinishTime')
+        if m.get('GmtStartTime') is not None:
+            self.gmt_start_time = m.get('GmtStartTime')
+        self.history_pods = []
+        if m.get('HistoryPods') is not None:
+            for k in m.get('HistoryPods'):
+                temp_model = PodItem()
+                self.history_pods.append(temp_model.from_map(k))
+        if m.get('Ip') is not None:
+            self.ip = m.get('Ip')
+        if m.get('PodId') is not None:
+            self.pod_id = m.get('PodId')
+        if m.get('PodUid') is not None:
+            self.pod_uid = m.get('PodUid')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Type') is not None:
+            self.type = m.get('Type')
+        return self
+
+
 class PodMetric(TeaModel):
     def __init__(
         self,
         metrics: List[Metric] = None,
         pod_id: str = None,
     ):
         self.metrics = metrics
@@ -2948,19 +3079,17 @@
     def __init__(
         self,
         data_source_id: str = None,
         job_id: str = None,
         request_id: str = None,
         tensorboard_id: str = None,
     ):
-        # DataSourceId
         self.data_source_id = data_source_id
         self.job_id = job_id
         self.request_id = request_id
-        # Tensorboard id
         self.tensorboard_id = tensorboard_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3142,15 +3271,14 @@
 class DeleteTensorboardResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tensorboard_id: str = None,
     ):
         self.request_id = request_id
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3213,14 +3341,41 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteTensorboardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetJobRequest(TeaModel):
+    def __init__(
+        self,
+        need_detail: bool = None,
+    ):
+        self.need_detail = need_detail
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.need_detail is not None:
+            result['NeedDetail'] = self.need_detail
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NeedDetail') is not None:
+            self.need_detail = m.get('NeedDetail')
+        return self
+
+
 class GetJobResponseBodyCodeSource(TeaModel):
     def __init__(
         self,
         branch: str = None,
         code_source_id: str = None,
         commit: str = None,
         mount_path: str = None,
@@ -3308,19 +3463,16 @@
         status: str = None,
         sub_status: str = None,
         type: str = None,
     ):
         self.gmt_create_time = gmt_create_time
         self.gmt_finish_time = gmt_finish_time
         self.gmt_start_time = gmt_start_time
-        # Pod Ip
         self.ip = ip
-        # Pod Id
         self.pod_id = pod_id
-        # Pod UId
         self.pod_uid = pod_uid
         self.resource_type = resource_type
         self.status = status
         self.sub_status = sub_status
         self.type = type
 
     def validate(self):
@@ -3396,15 +3548,14 @@
     ):
         self.gmt_create_time = gmt_create_time
         self.gmt_finish_time = gmt_finish_time
         self.gmt_start_time = gmt_start_time
         self.history_pods = history_pods
         self.ip = ip
         self.pod_id = pod_id
-        # Pod UId
         self.pod_uid = pod_uid
         self.resource_type = resource_type
         self.status = status
         self.sub_status = sub_status
         self.type = type
 
     def validate(self):
@@ -4337,15 +4488,14 @@
 
 class GetTensorboardRequest(TeaModel):
     def __init__(
         self,
         jod_id: str = None,
         workspace_id: str = None,
     ):
-        # JodId
         self.jod_id = jod_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4920,25 +5070,23 @@
         status: str = None,
         tensorboard_id: str = None,
         verbose: bool = None,
         workspace_id: str = None,
     ):
         self.display_name = display_name
         self.end_time = end_time
-        # JobId
         self.job_id = job_id
         self.order = order
         self.page_number = page_number
         self.page_size = page_size
         self.sort_by = sort_by
         self.source_id = source_id
         self.source_type = source_type
         self.start_time = start_time
         self.status = status
-        # TensorboardId
         self.tensorboard_id = tensorboard_id
         self.verbose = verbose
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -5132,15 +5280,14 @@
 class StartTensorboardResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tensorboard_id: str = None,
     ):
         self.request_id = request_id
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5314,15 +5461,14 @@
 class StopTensorboardResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tensorboard_id: str = None,
     ):
         self.request_id = request_id
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5529,15 +5675,14 @@
 class UpdateTensorboardResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         tensorboard_id: str = None,
     ):
         self.request_id = request_id
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203
-Version: 1.2.5
+Version: 1.2.6
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.5/setup.py` & `alibabacloud_pai-dlc20201203-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203.
 
-Created on 23/03/2023
+Created on 26/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python"
```


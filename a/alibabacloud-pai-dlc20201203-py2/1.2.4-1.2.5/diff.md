# Comparing `tmp/alibabacloud_pai-dlc20201203_py2-1.2.4.tar.gz` & `tmp/alibabacloud_pai-dlc20201203_py2-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.4.tar", last modified: Thu Mar 23 03:44:57 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.5.tar", last modified: Fri May 26 02:14:13 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4.tar` & `alibabacloud_pai-dlc20201203_py2-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/
--rw-r--r--   0 root         (0) root         (0)      541 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33143 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   190376 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2023-03-23 03:44:57.000000 alibabacloud_pai-dlc20201203_py2-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33393 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   196179 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/ChangeLog.md` & `alibabacloud_pai-dlc20201203_py2-1.2.5/ChangeLog.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-03-23 Version: 1.2.4
+- Change the type of RequestId to string in GetJobEvents API.
+
 2022-12-13 Version: 1.2.3
 - CreateJob supports params SuccessPolicy.
 
 2022-07-26 Version: 1.2.1
 - Support to automatically fill in endpoint according to region.
 
 2022-07-26 Version: 1.2.0
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/LICENSE` & `alibabacloud_pai-dlc20201203_py2-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203_py2
-Version: 1.2.4
+Version: 1.2.5
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/README-CN.md` & `alibabacloud_pai-dlc20201203_py2-1.2.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/README.md` & `alibabacloud_pai-dlc20201203_py2-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,17 +258,22 @@
         )
 
     def delete_tensorboard(self, tensorboard_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.delete_tensorboard_with_options(tensorboard_id, request, headers, runtime)
 
-    def get_job_with_options(self, job_id, headers, runtime):
+    def get_job_with_options(self, job_id, request, headers, runtime):
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
             pathname='/api/v1/jobs/%s' % TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(job_id)),
             method='GET',
@@ -278,18 +283,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             pai_dlc_20201203_models.GetJobResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_job(self, job_id):
+    def get_job(self, job_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.get_job_with_options(job_id, headers, runtime)
+        return self.get_job_with_options(job_id, request, headers, runtime)
 
     def get_job_events_with_options(self, job_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.max_events_num):
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -974,65 +974,107 @@
             self.gmt_create_time = m.get('GmtCreateTime')
         if m.get('JobId') is not None:
             self.job_id = m.get('JobId')
         return self
 
 
 class JobElasticSpec(TeaModel):
-    def __init__(self, aimaster_docker_image=None, aimaster_type=None, enable_aimaster=None,
-                 enable_elastic_training=None, enable_ps_job_elastic_worker=None, max_parallelism=None, min_parallelism=None):
+    def __init__(self, aimaster_docker_image=None, aimaster_type=None, edpmax_parallelism=None,
+                 edpmin_parallelism=None, elastic_strategy=None, enable_aimaster=None, enable_edp=None, enable_elastic_training=None,
+                 enable_ps_job_elastic_ps=None, enable_ps_job_elastic_worker=None, enable_ps_resource_estimate=None, max_parallelism=None,
+                 min_parallelism=None, psmax_parallelism=None, psmin_parallelism=None):
         self.aimaster_docker_image = aimaster_docker_image  # type: str
         self.aimaster_type = aimaster_type  # type: str
+        self.edpmax_parallelism = edpmax_parallelism  # type: int
+        self.edpmin_parallelism = edpmin_parallelism  # type: int
+        self.elastic_strategy = elastic_strategy  # type: str
         self.enable_aimaster = enable_aimaster  # type: bool
+        self.enable_edp = enable_edp  # type: bool
         self.enable_elastic_training = enable_elastic_training  # type: bool
+        self.enable_ps_job_elastic_ps = enable_ps_job_elastic_ps  # type: bool
         self.enable_ps_job_elastic_worker = enable_ps_job_elastic_worker  # type: bool
+        self.enable_ps_resource_estimate = enable_ps_resource_estimate  # type: bool
         self.max_parallelism = max_parallelism  # type: int
         self.min_parallelism = min_parallelism  # type: int
+        self.psmax_parallelism = psmax_parallelism  # type: int
+        self.psmin_parallelism = psmin_parallelism  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(JobElasticSpec, self).to_map()
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
 
     def from_map(self, m=None):
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
     def __init__(self, branch=None, code_source_id=None, commit=None, mount_path=None):
         self.branch = branch  # type: str
         self.code_source_id = code_source_id  # type: str
@@ -1537,14 +1579,87 @@
                 temp_model = Metric()
                 self.metrics.append(temp_model.from_map(k))
         if m.get('NodeName') is not None:
             self.node_name = m.get('NodeName')
         return self
 
 
+class PodItem(TeaModel):
+    def __init__(self, gmt_create_time=None, gmt_finish_time=None, gmt_start_time=None, history_pods=None, ip=None,
+                 pod_id=None, pod_uid=None, status=None, type=None):
+        self.gmt_create_time = gmt_create_time  # type: str
+        self.gmt_finish_time = gmt_finish_time  # type: str
+        self.gmt_start_time = gmt_start_time  # type: str
+        self.history_pods = history_pods  # type: list[PodItem]
+        self.ip = ip  # type: str
+        self.pod_id = pod_id  # type: str
+        self.pod_uid = pod_uid  # type: str
+        self.status = status  # type: str
+        self.type = type  # type: str
+
+    def validate(self):
+        if self.history_pods:
+            for k in self.history_pods:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(PodItem, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, metrics=None, pod_id=None):
         self.metrics = metrics  # type: list[Metric]
         self.pod_id = pod_id  # type: str
 
     def validate(self):
         if self.metrics:
@@ -2580,19 +2695,17 @@
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class CreateTensorboardResponseBody(TeaModel):
     def __init__(self, data_source_id=None, job_id=None, request_id=None, tensorboard_id=None):
-        # DataSourceId
         self.data_source_id = data_source_id  # type: str
         self.job_id = job_id  # type: str
         self.request_id = request_id  # type: str
-        # Tensorboard id
         self.tensorboard_id = tensorboard_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateTensorboardResponseBody, self).to_map()
@@ -2753,15 +2866,14 @@
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class DeleteTensorboardResponseBody(TeaModel):
     def __init__(self, request_id=None, tensorboard_id=None):
         self.request_id = request_id  # type: str
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteTensorboardResponseBody, self).to_map()
@@ -2819,14 +2931,38 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteTensorboardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetJobRequest(TeaModel):
+    def __init__(self, need_detail=None):
+        self.need_detail = need_detail  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetJobRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.need_detail is not None:
+            result['NeedDetail'] = self.need_detail
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NeedDetail') is not None:
+            self.need_detail = m.get('NeedDetail')
+        return self
+
+
 class GetJobResponseBodyCodeSource(TeaModel):
     def __init__(self, branch=None, code_source_id=None, commit=None, mount_path=None):
         self.branch = branch  # type: str
         self.code_source_id = code_source_id  # type: str
         self.commit = commit  # type: str
         self.mount_path = mount_path  # type: str
 
@@ -2893,19 +3029,16 @@
 
 class GetJobResponseBodyPodsHistoryPods(TeaModel):
     def __init__(self, gmt_create_time=None, gmt_finish_time=None, gmt_start_time=None, ip=None, pod_id=None,
                  pod_uid=None, resource_type=None, status=None, sub_status=None, type=None):
         self.gmt_create_time = gmt_create_time  # type: str
         self.gmt_finish_time = gmt_finish_time  # type: str
         self.gmt_start_time = gmt_start_time  # type: str
-        # Pod Ip
         self.ip = ip  # type: str
-        # Pod Id
         self.pod_id = pod_id  # type: str
-        # Pod UId
         self.pod_uid = pod_uid  # type: str
         self.resource_type = resource_type  # type: str
         self.status = status  # type: str
         self.sub_status = sub_status  # type: str
         self.type = type  # type: str
 
     def validate(self):
@@ -2969,15 +3102,14 @@
                  pod_id=None, pod_uid=None, resource_type=None, status=None, sub_status=None, type=None):
         self.gmt_create_time = gmt_create_time  # type: str
         self.gmt_finish_time = gmt_finish_time  # type: str
         self.gmt_start_time = gmt_start_time  # type: str
         self.history_pods = history_pods  # type: list[GetJobResponseBodyPodsHistoryPods]
         self.ip = ip  # type: str
         self.pod_id = pod_id  # type: str
-        # Pod UId
         self.pod_uid = pod_uid  # type: str
         self.resource_type = resource_type  # type: str
         self.status = status  # type: str
         self.sub_status = sub_status  # type: str
         self.type = type  # type: str
 
     def validate(self):
@@ -3801,15 +3933,14 @@
             temp_model = GetPodLogsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetTensorboardRequest(TeaModel):
     def __init__(self, jod_id=None, workspace_id=None):
-        # JodId
         self.jod_id = jod_id  # type: str
         self.workspace_id = workspace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4303,25 +4434,23 @@
 
 class ListTensorboardsRequest(TeaModel):
     def __init__(self, display_name=None, end_time=None, job_id=None, order=None, page_number=None, page_size=None,
                  sort_by=None, source_id=None, source_type=None, start_time=None, status=None, tensorboard_id=None,
                  verbose=None, workspace_id=None):
         self.display_name = display_name  # type: str
         self.end_time = end_time  # type: str
-        # JobId
         self.job_id = job_id  # type: str
         self.order = order  # type: str
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: int
         self.sort_by = sort_by  # type: str
         self.source_id = source_id  # type: str
         self.source_type = source_type  # type: str
         self.start_time = start_time  # type: str
         self.status = status  # type: str
-        # TensorboardId
         self.tensorboard_id = tensorboard_id  # type: str
         self.verbose = verbose  # type: bool
         self.workspace_id = workspace_id  # type: str
 
     def validate(self):
         pass
 
@@ -4498,15 +4627,14 @@
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class StartTensorboardResponseBody(TeaModel):
     def __init__(self, request_id=None, tensorboard_id=None):
         self.request_id = request_id  # type: str
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StartTensorboardResponseBody, self).to_map()
@@ -4659,15 +4787,14 @@
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class StopTensorboardResponseBody(TeaModel):
     def __init__(self, request_id=None, tensorboard_id=None):
         self.request_id = request_id  # type: str
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(StopTensorboardResponseBody, self).to_map()
@@ -4849,15 +4976,14 @@
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class UpdateTensorboardResponseBody(TeaModel):
     def __init__(self, request_id=None, tensorboard_id=None):
         self.request_id = request_id  # type: str
-        # Tensorboad Id
         self.tensorboard_id = tensorboard_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateTensorboardResponseBody, self).to_map()
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203-py2
-Version: 1.2.4
+Version: 1.2.5
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.4/setup.py` & `alibabacloud_pai-dlc20201203_py2-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203_py2.
 
-Created on 23/03/2023
+Created on 26/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python2"
```


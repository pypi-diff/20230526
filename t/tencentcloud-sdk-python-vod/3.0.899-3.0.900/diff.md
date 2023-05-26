# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.899.tar", last modified: Thu May 25 00:41:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.900.tar", last modified: Fri May 26 02:31:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.899.tar` & `tencentcloud-sdk-python-vod-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1185339 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:41:01.000000 tencentcloud-sdk-python-vod-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   177071 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1201061 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:31:54.000000 tencentcloud-sdk-python-vod-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/README.rst` & `tencentcloud-sdk-python-vod-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/vod_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateEnhanceMediaTemplate(self, request):
+        """创建音画质重生模板。
+
+        :param request: Request instance for CreateEnhanceMediaTemplate.
+        :type request: :class:`tencentcloud.vod.v20180717.models.CreateEnhanceMediaTemplateRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.CreateEnhanceMediaTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateEnhanceMediaTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateEnhanceMediaTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateHeadTailTemplate(self, request):
         """创建片头片尾模板。
 
         :param request: Request instance for CreateHeadTailTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.CreateHeadTailTemplateRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.CreateHeadTailTemplateResponse`
 
@@ -834,14 +857,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteEnhanceMediaTemplate(self, request):
+        """删除音画质重生模板。
+
+        :param request: Request instance for DeleteEnhanceMediaTemplate.
+        :type request: :class:`tencentcloud.vod.v20180717.models.DeleteEnhanceMediaTemplateRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.DeleteEnhanceMediaTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteEnhanceMediaTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteEnhanceMediaTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteHeadTailTemplate(self, request):
         """删除片头片尾模板。
 
         :param request: Request instance for DeleteHeadTailTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.DeleteHeadTailTemplateRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.DeleteHeadTailTemplateResponse`
 
@@ -1583,14 +1629,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeEnhanceMediaTemplates(self, request):
+        """获取音画质重生模板列表。
+
+        :param request: Request instance for DescribeEnhanceMediaTemplates.
+        :type request: :class:`tencentcloud.vod.v20180717.models.DescribeEnhanceMediaTemplatesRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.DescribeEnhanceMediaTemplatesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeEnhanceMediaTemplates", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeEnhanceMediaTemplatesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeEventConfig(self, request):
         """腾讯云点播为客户提供了媒体上传、媒体管理、媒体处理等等服务，在这些服务执行过程或执行结束时，腾讯云点播也提供各种对应的事件通知，方便开发者感知服务处理状态，并做下一步的业务操作。
 
         开发者可以通过本接口来查询当前配置事件通知的接收方式、接收地址以及哪些事件开启了接收回调通知。
 
         默认接口请求频率限制：100次/秒。
 
@@ -2378,14 +2447,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def EnhanceMediaByTemplate(self, request):
+        """使用模板发起音画质重生。
+
+        :param request: Request instance for EnhanceMediaByTemplate.
+        :type request: :class:`tencentcloud.vod.v20180717.models.EnhanceMediaByTemplateRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.EnhanceMediaByTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EnhanceMediaByTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.EnhanceMediaByTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ExecuteFunction(self, request):
         """本接口仅用于定制开发的特殊场景，除非云点播客服人员主动告知您需要使用本接口，其它情况请勿调用。
 
         :param request: Request instance for ExecuteFunction.
         :type request: :class:`tencentcloud.vod.v20180717.models.ExecuteFunctionRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.ExecuteFunctionResponse`
 
@@ -2679,14 +2771,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyEnhanceMediaTemplate(self, request):
+        """修改音画质重生模板。
+
+        :param request: Request instance for ModifyEnhanceMediaTemplate.
+        :type request: :class:`tencentcloud.vod.v20180717.models.ModifyEnhanceMediaTemplateRequest`
+        :rtype: :class:`tencentcloud.vod.v20180717.models.ModifyEnhanceMediaTemplateResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyEnhanceMediaTemplate", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyEnhanceMediaTemplateResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyEventConfig(self, request):
         """腾讯云点播为客户提供了媒体上传、媒体管理、媒体处理等等服务，在这些服务执行过程或执行结束时，腾讯云点播也提供各种对应的事件通知，方便开发者感知服务处理状态，并做下一步的业务操作。
 
         开发者可以通过调用本接口来实现：
         - 设置接收回调通知的类型，目前有[ HTTP 回调通知](https://cloud.tencent.com/document/product/266/33779) 和 [基于消息队列的可靠通知](https://cloud.tencent.com/document/product/266/33779) 两种类型。
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.899/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.900/tencentcloud/vod/v20180717/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6752,14 +6752,109 @@
 
 
     def _deserialize(self, params):
         self.Definition = params.get("Definition")
         self.RequestId = params.get("RequestId")
 
 
+class CreateEnhanceMediaTemplateRequest(AbstractModel):
+    """CreateEnhanceMediaTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Container: 输出文件封装格式，可选值：mp4、flv、hls。
+        :type Container: str
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        :param Name: 音画质重生模板名称，长度限制：64 个字符。
+        :type Name: str
+        :param Comment: 模板描述信息，长度限制：256 个字符。
+        :type Comment: str
+        :param RebuildVideoInfo: 音画质重生视频控制控制信息。
+        :type RebuildVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildVideoInfo`
+        :param RebuildAudioInfo: 音画质重生音频控制控制信息。
+        :type RebuildAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildAudioInfo`
+        :param TargetVideoInfo: 输出目标视频控制信息。
+        :type TargetVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetVideoStream`
+        :param TargetAudioInfo: 输出目标音频控制信息。
+        :type TargetAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetAudioStream`
+        :param RemoveVideo: 是否去除视频数据，可选值：
+<li>0：保留</li>
+<li>1：去除</li>
+默认值 0。
+        :type RemoveVideo: int
+        :param RemoveAudio: 是否去除音频数据，可选值：
+<li>0：保留</li>
+<li>1：去除</li>
+默认值 0。
+        :type RemoveAudio: int
+        """
+        self.Container = None
+        self.SubAppId = None
+        self.Name = None
+        self.Comment = None
+        self.RebuildVideoInfo = None
+        self.RebuildAudioInfo = None
+        self.TargetVideoInfo = None
+        self.TargetAudioInfo = None
+        self.RemoveVideo = None
+        self.RemoveAudio = None
+
+
+    def _deserialize(self, params):
+        self.Container = params.get("Container")
+        self.SubAppId = params.get("SubAppId")
+        self.Name = params.get("Name")
+        self.Comment = params.get("Comment")
+        if params.get("RebuildVideoInfo") is not None:
+            self.RebuildVideoInfo = RebuildVideoInfo()
+            self.RebuildVideoInfo._deserialize(params.get("RebuildVideoInfo"))
+        if params.get("RebuildAudioInfo") is not None:
+            self.RebuildAudioInfo = RebuildAudioInfo()
+            self.RebuildAudioInfo._deserialize(params.get("RebuildAudioInfo"))
+        if params.get("TargetVideoInfo") is not None:
+            self.TargetVideoInfo = RebuildMediaTargetVideoStream()
+            self.TargetVideoInfo._deserialize(params.get("TargetVideoInfo"))
+        if params.get("TargetAudioInfo") is not None:
+            self.TargetAudioInfo = RebuildMediaTargetAudioStream()
+            self.TargetAudioInfo._deserialize(params.get("TargetAudioInfo"))
+        self.RemoveVideo = params.get("RemoveVideo")
+        self.RemoveAudio = params.get("RemoveAudio")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateEnhanceMediaTemplateResponse(AbstractModel):
+    """CreateEnhanceMediaTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Definition: 音画质重生模板 ID。
+        :type Definition: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Definition = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Definition = params.get("Definition")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateHeadTailTemplateRequest(AbstractModel):
     """CreateHeadTailTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8476,14 +8571,59 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteEnhanceMediaTemplateRequest(AbstractModel):
+    """DeleteEnhanceMediaTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Definition: 音画质重生模板号。
+        :type Definition: int
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        """
+        self.Definition = None
+        self.SubAppId = None
+
+
+    def _deserialize(self, params):
+        self.Definition = params.get("Definition")
+        self.SubAppId = params.get("SubAppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteEnhanceMediaTemplateResponse(AbstractModel):
+    """DeleteEnhanceMediaTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteHeadTailTemplateRequest(AbstractModel):
     """DeleteHeadTailTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -10262,14 +10402,86 @@
     def _deserialize(self, params):
         if params.get("SDMCInfo") is not None:
             self.SDMCInfo = SDMCDrmKeyProviderInfo()
             self.SDMCInfo._deserialize(params.get("SDMCInfo"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeEnhanceMediaTemplatesRequest(AbstractModel):
+    """DescribeEnhanceMediaTemplates请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        :param Definitions: 音画质重生模板列表。长度限制：100。
+        :type Definitions: list of int
+        :param Type: 模板类型过滤条件，可选值：
+<li>Preset：系统预置模板；</li>
+<li>Custom：用户自定义模板。</li>
+        :type Type: str
+        :param Offset: 分页偏移量，默认值：0。
+        :type Offset: int
+        :param Limit: 返回记录条数，默认值：10，最大值：100。
+        :type Limit: int
+        """
+        self.SubAppId = None
+        self.Definitions = None
+        self.Type = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.SubAppId = params.get("SubAppId")
+        self.Definitions = params.get("Definitions")
+        self.Type = params.get("Type")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeEnhanceMediaTemplatesResponse(AbstractModel):
+    """DescribeEnhanceMediaTemplates返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 符合过滤条件的记录总数。
+        :type TotalCount: int
+        :param RebuildMediaTemplateSet: 音画质重生模板详情列表。
+        :type RebuildMediaTemplateSet: list of RebuildMediaTemplate
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.RebuildMediaTemplateSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("RebuildMediaTemplateSet") is not None:
+            self.RebuildMediaTemplateSet = []
+            for item in params.get("RebuildMediaTemplateSet"):
+                obj = RebuildMediaTemplate()
+                obj._deserialize(item)
+                self.RebuildMediaTemplateSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeEventConfigRequest(AbstractModel):
     """DescribeEventConfig请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13347,14 +13559,97 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class EnhanceMediaByTemplateRequest(AbstractModel):
+    """EnhanceMediaByTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileId: 媒体文件 ID。
+        :type FileId: str
+        :param Definition: 音画质重生模板 ID。
+        :type Definition: int
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        :param StartTimeOffset: 起始偏移时间，单位：秒，不填表示从视频开始截取。
+        :type StartTimeOffset: float
+        :param EndTimeOffset: 结束偏移时间，单位：秒，不填表示截取到视频末尾。
+        :type EndTimeOffset: float
+        :param OutputConfig: 音画质重生后的文件配置。
+        :type OutputConfig: :class:`tencentcloud.vod.v20180717.models.RebuildMediaOutputConfig`
+        :param SessionId: 用于去重的识别码，如果三天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长 50 个字符，不带或者带空字符串表示不做去重。
+        :type SessionId: str
+        :param SessionContext: 来源上下文，用于透传用户请求信息，任务流状态变更回调将返回该字段值，最长 1000 个字符。
+        :type SessionContext: str
+        :param TasksPriority: 任务的优先级，数值越大优先级越高，取值范围是 -10 到 10，不填代表 0。
+        :type TasksPriority: int
+        :param ExtInfo: 保留字段，特殊用途时使用。
+        :type ExtInfo: str
+        """
+        self.FileId = None
+        self.Definition = None
+        self.SubAppId = None
+        self.StartTimeOffset = None
+        self.EndTimeOffset = None
+        self.OutputConfig = None
+        self.SessionId = None
+        self.SessionContext = None
+        self.TasksPriority = None
+        self.ExtInfo = None
+
+
+    def _deserialize(self, params):
+        self.FileId = params.get("FileId")
+        self.Definition = params.get("Definition")
+        self.SubAppId = params.get("SubAppId")
+        self.StartTimeOffset = params.get("StartTimeOffset")
+        self.EndTimeOffset = params.get("EndTimeOffset")
+        if params.get("OutputConfig") is not None:
+            self.OutputConfig = RebuildMediaOutputConfig()
+            self.OutputConfig._deserialize(params.get("OutputConfig"))
+        self.SessionId = params.get("SessionId")
+        self.SessionContext = params.get("SessionContext")
+        self.TasksPriority = params.get("TasksPriority")
+        self.ExtInfo = params.get("ExtInfo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EnhanceMediaByTemplateResponse(AbstractModel):
+    """EnhanceMediaByTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 音画质重生的任务 ID，可以通过该 ID 查询音画质重生任务的状态。
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class EventContent(AbstractModel):
     """事件通知内容，其中，TranscodeCompleteEvent、ConcatCompleteEvent、ClipCompleteEvent、CreateImageSpriteCompleteEvent、SnapshotByTimeOffsetCompleteEvent 为兼容 2017 版接口发起任务的事件通知。
 
     """
 
     def __init__(self):
         r"""
@@ -18385,14 +18680,109 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyEnhanceMediaTemplateRequest(AbstractModel):
+    """ModifyEnhanceMediaTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Definition: 音画质重生模板号。
+        :type Definition: int
+        :param SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
+        :type SubAppId: int
+        :param Name: 音画质重生模板名称，长度限制：64 个字符。
+        :type Name: str
+        :param Comment: 模板描述信息，长度限制：256 个字符。
+        :type Comment: str
+        :param RebuildVideoInfo: 音画质重生视频控制控制信息。
+        :type RebuildVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildVideoInfo`
+        :param RebuildAudioInfo: 音画质重生音频控制控制信息。
+        :type RebuildAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildAudioInfo`
+        :param TargetVideoInfo: 输出目标视频控制信息。
+        :type TargetVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetVideoStream`
+        :param TargetAudioInfo: 输出目标音频控制信息。
+        :type TargetAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetAudioStream`
+        :param Container: 输出文件封装格式，可选值：mp4、flv、hls。
+        :type Container: str
+        :param RemoveVideo: 是否去除视频数据，可选值：
+<li>0：保留</li>
+<li>1：去除</li>
+默认值 0。
+        :type RemoveVideo: int
+        :param RemoveAudio: 是否去除音频数据，可选值：
+<li>0：保留</li>
+<li>1：去除</li>
+默认值 0。
+        :type RemoveAudio: int
+        """
+        self.Definition = None
+        self.SubAppId = None
+        self.Name = None
+        self.Comment = None
+        self.RebuildVideoInfo = None
+        self.RebuildAudioInfo = None
+        self.TargetVideoInfo = None
+        self.TargetAudioInfo = None
+        self.Container = None
+        self.RemoveVideo = None
+        self.RemoveAudio = None
+
+
+    def _deserialize(self, params):
+        self.Definition = params.get("Definition")
+        self.SubAppId = params.get("SubAppId")
+        self.Name = params.get("Name")
+        self.Comment = params.get("Comment")
+        if params.get("RebuildVideoInfo") is not None:
+            self.RebuildVideoInfo = RebuildVideoInfo()
+            self.RebuildVideoInfo._deserialize(params.get("RebuildVideoInfo"))
+        if params.get("RebuildAudioInfo") is not None:
+            self.RebuildAudioInfo = RebuildAudioInfo()
+            self.RebuildAudioInfo._deserialize(params.get("RebuildAudioInfo"))
+        if params.get("TargetVideoInfo") is not None:
+            self.TargetVideoInfo = RebuildMediaTargetVideoStream()
+            self.TargetVideoInfo._deserialize(params.get("TargetVideoInfo"))
+        if params.get("TargetAudioInfo") is not None:
+            self.TargetAudioInfo = RebuildMediaTargetAudioStream()
+            self.TargetAudioInfo._deserialize(params.get("TargetAudioInfo"))
+        self.Container = params.get("Container")
+        self.RemoveVideo = params.get("RemoveVideo")
+        self.RemoveAudio = params.get("RemoveAudio")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyEnhanceMediaTemplateResponse(AbstractModel):
+    """ModifyEnhanceMediaTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.900/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.899'
+__version__ = '3.0.900'
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.900/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.900/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.899/setup.py` & `tencentcloud-sdk-python-vod-3.0.900/setup.py`

 * *Files identical despite different names*


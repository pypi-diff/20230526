# Comparing `tmp/tencentcloud-sdk-python-asr-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-asr-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.899.tar", last modified: Thu May 25 00:16:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-asr-3.0.900.tar", last modified: Fri May 26 02:10:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-asr-3.0.899.tar` & `tencentcloud-sdk-python-asr-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    24780 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)     6520 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64128 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:16:41.000000 tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    25038 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64128 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:10:06.000000 tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-asr-3.0.899/README.rst` & `tencentcloud-sdk-python-asr-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/asr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateRecTask(self, request):
         """本接口服务对时长5小时以内的录音文件进行识别，异步返回识别全部结果。
         • 支持中文普通话、英语、粤语、日语、越南语、马来语、印度尼西亚语、菲律宾语、葡萄牙语、土耳其语、上海话、四川话、武汉话、贵阳话、昆明话、西安话、郑州话、太原话、兰州话、银川话、西宁话、南京话、合肥话、南昌话、长沙话、苏州话、杭州话、济南话、天津话、石家庄话、黑龙江话、吉林话、辽宁话。
         • 支持wav、mp3、m4a、flv、mp4、wma、3gp、amr、aac、ogg-opus、flac格式。
-        • 支持语音 URL 和本地语音文件两种请求方式。语音 URL 的音频时长不能长于5小时，文件大小不超过1GB。本地语音文件调用不能大于5MB。
+        • 支持语音 URL 和本地语音文件两种请求方式。语音 URL 的音频时长不能长于5小时，文件大小不超过1GB。本地语音文件调用不能大于5MB。推荐使用 [ 腾讯云COS](https://cloud.tencent.com/document/product/436/38484) 来存储&生成URL提交任务，无外网&流量下行费用，节约成本、提升任务速度。(COS桶权限需要设置公有读私有写，或URL设置外部可访问)
         • 提交录音文件识别请求后，在3小时内完成识别（大多数情况下1小时音频约3分钟以内完成识别，半小时内发送超过1000小时录音或者2万条识别任务的除外），识别结果在服务端可保存7天。
         • 支持回调或轮询的方式获取结果，结果获取请参考[ 录音文件识别结果查询](https://cloud.tencent.com/document/product/1093/37822)。
         •   生成字幕场景可设置参数ResTextFormat为3，解析ResultDetail结构生成字幕，可参考 [生成字幕最佳实践](https://cloud.tencent.com/document/product/1093/84291)。
         •   签名方法参考 [公共参数](https://cloud.tencent.com/document/api/1093/35640) 中签名方法v3。
         • 默认接口请求频率限制：20次/秒，如您有提高请求频率限制的需求，请提[工单](https://console.cloud.tencent.com/workorder/category)进行咨询。
 
         :param request: Request instance for CreateRecTask.
```

### Comparing `tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.899/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-asr-3.0.900/tencentcloud/asr/v20190614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-asr-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-asr-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-asr-3.0.899/setup.py` & `tencentcloud-sdk-python-asr-3.0.900/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-asr-3.0.899/tencentcloud_sdk_python_asr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-asr-3.0.900/tencentcloud_sdk_python_asr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-asr
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Asr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


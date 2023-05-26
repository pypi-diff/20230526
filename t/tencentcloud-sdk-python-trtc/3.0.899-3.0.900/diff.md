# Comparing `tmp/tencentcloud-sdk-python-trtc-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-trtc-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.899.tar", last modified: Thu May 25 00:40:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trtc-3.0.900.tar", last modified: Fri May 26 02:31:04 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trtc-3.0.899.tar` & `tencentcloud-sdk-python-trtc-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)     9679 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198994 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)    58535 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/trtc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:40:04.000000 tencentcloud-sdk-python-trtc-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)     9679 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198994 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)    58535 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/trtc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:31:04.000000 tencentcloud-sdk-python-trtc-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/README.rst` & `tencentcloud-sdk-python-trtc-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     _apiVersion = '2019-07-22'
     _endpoint = 'trtc.tencentcloudapi.com'
     _service = 'trtc'
 
 
     def CreateCloudRecording(self, request):
         """接口说明：
-        启动云端录制功能，完成房间内的音视频录制，并上传到指定的云存储。您可以通过此 API 接口把TRTC 房间中的每一路音视频流做单独的录制有或者多路视频画面混流一路。
+        启动云端录制功能，完成房间内的音视频录制，并上传到指定的云存储。您可以通过此 API 接口把TRTC 房间中的每一路音视频流做单独的录制又或者多路视频画面混流一路。
 
         您可以通过此接口实现如下目标：
         * 指定订阅流参数（RecordParams）来指定需要录制的主播的黑名单或者白名单。
         * 指定第三方存储的参数（StorageParams）来指定上传到您希望的云存储，目前支持云点播VOD和对象存储COS
         * 指定混流模式下的音视频转码详细参数（MixTranscodeParams），包括视频分辨率、视频码率、视频帧率、以及声音质量等
         * 指定混流模式各路画面的位置和布局或者也可以指定自动模板的方式来配置。
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trtc-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.900/tencentcloud_sdk_python_trtc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-trtc-3.0.900/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trtc
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Trtc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trtc-3.0.899/setup.py` & `tencentcloud-sdk-python-trtc-3.0.900/setup.py`

 * *Files identical despite different names*


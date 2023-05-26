# Comparing `tmp/tencentcloud-sdk-python-tmt-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-tmt-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.899.tar", last modified: Thu May 25 00:39:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.900.tar", last modified: Fri May 26 02:30:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tmt-3.0.899.tar` & `tencentcloud-sdk-python-tmt-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)     3585 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9401 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)    33942 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:39:31.000000 tencentcloud-sdk-python-tmt-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:39:32.000000 tencentcloud-sdk-python-tmt-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9401 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    33942 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:30:34.000000 tencentcloud-sdk-python-tmt-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:30:35.000000 tencentcloud-sdk-python-tmt-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/README.rst` & `tencentcloud-sdk-python-tmt-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
 # 音频分片长度超过限制，请保证分片长度小于8s。
 UNSUPPORTEDOPERATION_AUDIODURATIONEXCEED = 'UnsupportedOperation.AudioDurationExceed'
 
-# 单次请求text超过长度限制，请保证单次请求⻓度低于2000。
+# 单次请求text超过长度限制。
 UNSUPPORTEDOPERATION_TEXTTOOLONG = 'UnsupportedOperation.TextTooLong'
 
 # 不支持的目标语言，请参照语言列表。
 UNSUPPORTEDOPERATION_UNSUPPORTEDTARGETLANGUAGE = 'UnsupportedOperation.UnSupportedTargetLanguage'
 
 # 不支持的语言，请参照语言列表。
 UNSUPPORTEDOPERATION_UNSUPPORTEDLANGUAGE = 'UnsupportedOperation.UnsupportedLanguage'
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-tmt-3.0.900/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.900/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.900/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.899/setup.py` & `tencentcloud-sdk-python-tmt-3.0.900/setup.py`

 * *Files identical despite different names*


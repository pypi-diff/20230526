# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.899.tar", last modified: Thu May 25 00:32:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.900.tar", last modified: Fri May 26 02:24:22 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.899.tar` & `tencentcloud-sdk-python-ocr-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113845 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   507696 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:32:51.000000 tencentcloud-sdk-python-ocr-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113845 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   508075 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/README.rst` & `tencentcloud-sdk-python-ocr-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 # 引擎识别超时。
 FAILEDOPERATION_ENGINERECOGNIZETIMEOUT = 'FailedOperation.EngineRecognizeTimeout'
 
 # 身份证信息不合法（身份证号、姓名字段校验非法等）。
 FAILEDOPERATION_IDCARDINFOILLEGAL = 'FailedOperation.IdCardInfoIllegal'
 
+# 图片分辨率过小或身份证在原图中的占比过小
+FAILEDOPERATION_IDCARDTOOSMALL = 'FailedOperation.IdCardTooSmall'
+
 # 银行卡信息非法。
 FAILEDOPERATION_ILLEGALBANKCARDERROR = 'FailedOperation.IllegalBankCardError'
 
 # 图片模糊。
 FAILEDOPERATION_IMAGEBLUR = 'FailedOperation.ImageBlur'
 
 # 图片解码失败。
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,14 +616,18 @@
 注：告警码可以同时存在多个
         :type RecognizeWarnCode: list of int
         :param RecognizeWarnMsg: 告警码说明：
 OCR_WARNING_TYPE_NOT_MATCH 非营业执照
 WARN_COPY_CARD 黑白复印件告警
 注：告警信息可以同时存在多个
         :type RecognizeWarnMsg: list of str
+        :param IsDuplication: 是否为副本。1为是，-1为不是。
+        :type IsDuplication: int
+        :param RegistrationDate: 登记日期
+        :type RegistrationDate: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.RegNum = None
         self.Name = None
         self.Capital = None
         self.Person = None
@@ -631,14 +635,16 @@
         self.Business = None
         self.Type = None
         self.Period = None
         self.ComposingForm = None
         self.SetDate = None
         self.RecognizeWarnCode = None
         self.RecognizeWarnMsg = None
+        self.IsDuplication = None
+        self.RegistrationDate = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RegNum = params.get("RegNum")
         self.Name = params.get("Name")
         self.Capital = params.get("Capital")
@@ -647,14 +653,16 @@
         self.Business = params.get("Business")
         self.Type = params.get("Type")
         self.Period = params.get("Period")
         self.ComposingForm = params.get("ComposingForm")
         self.SetDate = params.get("SetDate")
         self.RecognizeWarnCode = params.get("RecognizeWarnCode")
         self.RecognizeWarnMsg = params.get("RecognizeWarnMsg")
+        self.IsDuplication = params.get("IsDuplication")
+        self.RegistrationDate = params.get("RegistrationDate")
         self.RequestId = params.get("RequestId")
 
 
 class BizLicenseVerifyResult(AbstractModel):
     """验真接口
 
     """
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.900/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.899/setup.py` & `tencentcloud-sdk-python-ocr-3.0.900/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/tencentcloud-sdk-python-ame-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-ame-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.899.tar", last modified: Thu May 25 00:15:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.900.tar", last modified: Fri May 26 02:09:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ame-3.0.899.tar` & `tencentcloud-sdk-python-ame-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/
--rw-r--r--   0 root         (0) root         (0)    29455 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/ame_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126346 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:15:47.000000 tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/
+-rw-r--r--   0 root         (0) root         (0)    29455 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/ame_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126602 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:09:11.000000 tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ame-3.0.899/README.rst` & `tencentcloud-sdk-python-ame-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/ame_client.py` & `tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/ame_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/errorcodes.py` & `tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.899/tencentcloud/ame/v20190916/models.py` & `tencentcloud-sdk-python-ame-3.0.900/tencentcloud/ame/v20190916/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3569,30 +3569,37 @@
         :param PrivateMapKey: 进房钥匙，若需要权限控制请携带该参数。
  [privateMapKey 权限设置](/document/product/647/32240) 
         :type PrivateMapKey: str
         :param Role: 用户角色，目前支持两种角色：
 <li>anchor：主播</li>
 <li>audience：观众</li>
         :type Role: str
+        :param RoomIdType: TRTC房间号的类型：
+<li>Integer：数字类型</li>
+<li> String：字符串类型</li>
+默认为：Integer 。
+        :type RoomIdType: str
         """
         self.Sign = None
         self.RoomId = None
         self.SdkAppId = None
         self.UserId = None
         self.PrivateMapKey = None
         self.Role = None
+        self.RoomIdType = None
 
 
     def _deserialize(self, params):
         self.Sign = params.get("Sign")
         self.RoomId = params.get("RoomId")
         self.SdkAppId = params.get("SdkAppId")
         self.UserId = params.get("UserId")
         self.PrivateMapKey = params.get("PrivateMapKey")
         self.Role = params.get("Role")
+        self.RoomIdType = params.get("RoomIdType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ame-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ame-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ame-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ame-3.0.899/setup.py` & `tencentcloud-sdk-python-ame-3.0.900/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.899/tencentcloud_sdk_python_ame.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.900/tencentcloud_sdk_python_ame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


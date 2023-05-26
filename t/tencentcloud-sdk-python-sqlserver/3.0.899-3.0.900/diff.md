# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.899.tar", last modified: Thu May 25 00:35:07 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.900.tar", last modified: Fri May 26 02:26:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.899.tar` & `tencentcloud-sdk-python-sqlserver-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      755 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   106575 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   349080 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-05-25 00:35:06.000000 tencentcloud-sdk-python-sqlserver-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:35:07.000000 tencentcloud-sdk-python-sqlserver-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   106575 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   349517 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:26:33.000000 tencentcloud-sdk-python-sqlserver-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1165,23 +1165,33 @@
 
     """
 
     def __init__(self):
         r"""
         :param DealName: 订单名称
         :type DealName: str
+        :param FlowId: 流程ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FlowId: int
+        :param InstanceIdSet: 实例ID集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceIdSet: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DealName = None
+        self.FlowId = None
+        self.InstanceIdSet = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DealName = params.get("DealName")
+        self.FlowId = params.get("FlowId")
+        self.InstanceIdSet = params.get("InstanceIdSet")
         self.RequestId = params.get("RequestId")
 
 
 class CreateBusinessIntelligenceFileRequest(AbstractModel):
     """CreateBusinessIntelligenceFile请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.900/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.900/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.899/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.900/setup.py`

 * *Files identical despite different names*


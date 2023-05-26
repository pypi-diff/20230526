# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.899.tar", last modified: Thu May 25 00:26:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.900.tar", last modified: Fri May 26 02:18:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.899.tar` & `tencentcloud-sdk-python-ess-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223633 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:26:39.000000 tencentcloud-sdk-python-ess-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223871 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.899/README.rst` & `tencentcloud-sdk-python-ess-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.899/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4138,34 +4138,39 @@
         :type CreatedOn: int
         :param FlowMessage: 拒签或者取消的原因描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowMessage: str
         :param Creator:  合同发起人userId
 注意：此字段可能返回 null，表示取不到有效值。
         :type Creator: str
+        :param Deadline: 合同过期时间，时间戳，单位秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Deadline: int
         """
         self.FlowId = None
         self.FlowName = None
         self.FlowDescription = None
         self.FlowType = None
         self.FlowStatus = None
         self.CreatedOn = None
         self.FlowMessage = None
         self.Creator = None
+        self.Deadline = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.FlowName = params.get("FlowName")
         self.FlowDescription = params.get("FlowDescription")
         self.FlowType = params.get("FlowType")
         self.FlowStatus = params.get("FlowStatus")
         self.CreatedOn = params.get("CreatedOn")
         self.FlowMessage = params.get("FlowMessage")
         self.Creator = params.get("Creator")
+        self.Deadline = params.get("Deadline")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.899/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.899/setup.py` & `tencentcloud-sdk-python-ess-3.0.900/setup.py`

 * *Files identical despite different names*


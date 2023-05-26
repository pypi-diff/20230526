# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.899.tar", last modified: Thu May 25 00:23:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.900.tar", last modified: Fri May 26 02:15:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.899.tar` & `tencentcloud-sdk-python-cvm-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42926 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   430169 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:23:37.000000 tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119300 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42926 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   430455 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:15:37.000000 tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/README.rst` & `tencentcloud-sdk-python-cvm-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,15 +747,15 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceTypeConfigs(self, request):
         """本接口 (DescribeInstanceTypeConfigs) 用于查询实例机型配置。
 
-        * 可以根据`zone`、`instance-family`来查询实例机型配置。过滤条件详见过滤器[`Filter`](https://cloud.tencent.com/document/api/213/15753#Filter)。
+        * 可以根据`zone`、`instance-family`、`instance-type`来查询实例机型配置。过滤条件详见过滤器[`Filter`](https://cloud.tencent.com/document/api/213/15753#Filter)。
         * 如果参数为空，返回指定地域的所有实例机型配置。
 
         :param request: Request instance for DescribeInstanceTypeConfigs.
         :type request: :class:`tencentcloud.cvm.v20170312.models.DescribeInstanceTypeConfigsRequest`
         :rtype: :class:`tencentcloud.cvm.v20170312.models.DescribeInstanceTypeConfigsResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2364,14 +2364,16 @@
 
     def __init__(self):
         r"""
         :param Filters: <li><strong>zone</strong></li>
 <p style="padding-left: 30px;">按照【<strong>可用区</strong>】进行过滤。可用区形如：ap-guangzhou-1。</p><p style="padding-left: 30px;">类型：String</p><p style="padding-left: 30px;">必选：否</p><p style="padding-left: 30px;">可选项：<a href="https://cloud.tencent.com/document/product/213/6091">可用区列表</a></p>
 <li><strong>instance-family</strong></li>
 <p style="padding-left: 30px;">按照【<strong>实例机型系列</strong>】进行过滤。实例机型系列形如：S1、I1、M1等。</p><p style="padding-left: 30px;">类型：String</p><p style="padding-left: 30px;">必选：否</p>
+<li><strong>instance-type</strong></li>
+<p style="padding-left: 30px;">按照【<strong>实例类型</strong>】进行过滤。实例类型形如：S5.12XLARGE128、S5.12XLARGE96等。</p><p style="padding-left: 30px;">类型：String</p><p style="padding-left: 30px;">必选：否</p>
 每次请求的`Filters`的上限为10，`Filter.Values`的上限为1。
         :type Filters: list of Filter
         """
         self.Filters = None
 
 
     def _deserialize(self, params):
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.900/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/setup.py` & `tencentcloud-sdk-python-cvm-3.0.900/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.899/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.900/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


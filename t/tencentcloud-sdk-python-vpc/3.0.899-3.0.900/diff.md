# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.899.tar", last modified: Thu May 25 00:41:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.900.tar", last modified: Fri May 26 02:32:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.899.tar` & `tencentcloud-sdk-python-vpc-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332279 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851611 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:41:09.000000 tencentcloud-sdk-python-vpc-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332331 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851805 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:32:01.000000 tencentcloud-sdk-python-vpc-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.900/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/README.rst` & `tencentcloud-sdk-python-vpc-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4538,15 +4538,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeVpnGatewaySslServers(self, request):
-        """查询SSL-VPN SERVER 列表信息
+        """本接口（DescribeVpnGatewaySslServers）用于查询SSL-VPN SERVER 列表信息。
 
         :param request: Request instance for DescribeVpnGatewaySslServers.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewaySslServersRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeVpnGatewaySslServersResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,28 +81,33 @@
         :type VpnGatewayIdSslAccessPolicyId: str
         :param ForAllClient: 是否对所有用户都生效。1 生效 0不生效
         :type ForAllClient: int
         :param UserGroupIds: 用户组ID
         :type UserGroupIds: list of str
         :param UpdateTime: 更新时间
         :type UpdateTime: str
+        :param Remark: Remark
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Remark: str
         """
         self.TargetCidr = None
         self.VpnGatewayIdSslAccessPolicyId = None
         self.ForAllClient = None
         self.UserGroupIds = None
         self.UpdateTime = None
+        self.Remark = None
 
 
     def _deserialize(self, params):
         self.TargetCidr = params.get("TargetCidr")
         self.VpnGatewayIdSslAccessPolicyId = params.get("VpnGatewayIdSslAccessPolicyId")
         self.ForAllClient = params.get("ForAllClient")
         self.UserGroupIds = params.get("UserGroupIds")
         self.UpdateTime = params.get("UpdateTime")
+        self.Remark = params.get("Remark")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13115,26 +13120,26 @@
 class DescribeVpnGatewaySslServersRequest(AbstractModel):
     """DescribeVpnGatewaySslServers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Offset: 偏移量
+        :param Offset: 偏移量。
         :type Offset: int
-        :param Limit: 请求对象个数
+        :param Limit: 请求对象个数。
         :type Limit: int
         :param SslVpnServerIds: SSL-VPN-SERVER实例ID。形如：vpngwSslServer-12345678。每次请求的实例的上限为100。参数不支持同时指定SslVpnServerIds和Filters。
         :type SslVpnServerIds: list of str
         :param Filters: 过滤条件，参数不支持同时指定SslVpnServerIds和Filters。
-<li>vpc-id - String - （过滤条件）VPC实例ID形如：vpc-f49l6u0z。</li>
-<li>vpn-gateway-id - String - （过滤条件）VPN实例ID形如：vpngw-5aluhh9t。</li>
+<li>vpc-id - String - （过滤条件）VPC实例ID，形如：vpc-f49l6u0z。</li>
+<li>vpn-gateway-id - String - （过滤条件）VPN实例ID，形如：vpngw-5aluhh9t。</li>
 <li>vpn-gateway-name - String - （过滤条件）VPN实例名称。</li>
 <li>ssl-vpn-server-name - String - （过滤条件）SSL-VPN-SERVER实例名称。</li>
-<li>ssl-vpn-server-id - String - （过滤条件）SSL-VPN-SERVER实例ID形如：vpngwSslServer-123456。</li>
+<li>ssl-vpn-server-id - String - （过滤条件）SSL-VPN-SERVER实例ID，形如：vpns-xxx。</li>
         :type Filters: list of FilterObject
         :param IsVpnPortal: vpn门户使用。 默认Flase
         :type IsVpnPortal: bool
         """
         self.Offset = None
         self.Limit = None
         self.SslVpnServerIds = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.900/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.899/setup.py` & `tencentcloud-sdk-python-vpc-3.0.900/setup.py`

 * *Files identical despite different names*


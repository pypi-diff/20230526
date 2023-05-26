# Comparing `tmp/tencentcloud-sdk-python-scf-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-scf-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.899.tar", last modified: Thu May 25 00:34:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-scf-3.0.900.tar", last modified: Fri May 26 02:25:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-scf-3.0.899.tar` & `tencentcloud-sdk-python-scf-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    42711 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)    31630 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191703 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:34:14.000000 tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)    31630 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191703 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:25:44.000000 tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-scf-3.0.899/README.rst` & `tencentcloud-sdk-python-scf-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.899/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-scf-3.0.900/tencentcloud/scf/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-scf-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-scf-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.900/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-scf-3.0.899/setup.py` & `tencentcloud-sdk-python-scf-3.0.900/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-scf-3.0.899/tencentcloud_sdk_python_scf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-scf-3.0.900/tencentcloud_sdk_python_scf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-scf
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Scf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.899.tar", last modified: Thu May 25 00:41:50 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.900.tar", last modified: Fri May 26 02:32:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.899.tar` & `tencentcloud-sdk-python-yinsuda-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72966 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)    15889 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/yinsuda_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-25 00:41:49.000000 tencentcloud-sdk-python-yinsuda-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:41:50.000000 tencentcloud-sdk-python-yinsuda-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72966 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)    15889 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:32:38.000000 tencentcloud-sdk-python-yinsuda-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.900/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.899/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.900/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.899.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.899.tar", last modified: Thu May 25 00:19:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.900.tar", last modified: Fri May 26 02:12:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.899.tar` & `tencentcloud-sdk-python-cdb-3.0.900.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   150608 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   526122 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-25 00:19:25.000000 tencentcloud-sdk-python-cdb-3.0.899/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   150608 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526122 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:12:50.000000 tencentcloud-sdk-python-cdb-3.0.900/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/README.rst` & `tencentcloud-sdk-python-cdb-3.0.900/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/cdb/v20170320/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.900/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.900/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.899
+Version: 3.0.900
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.899/setup.py` & `tencentcloud-sdk-python-cdb-3.0.900/setup.py`

 * *Files identical despite different names*

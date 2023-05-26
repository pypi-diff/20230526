# Comparing `tmp/splunktalib-3.0.3.tar.gz` & `tmp/splunktalib-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunktalib-3.0.3.tar", max compression
+gzip compressed data, was "splunktalib-3.0.4.tar", max compression
```

## Comparing `splunktalib-3.0.3.tar` & `splunktalib-3.0.4.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0    11342 2023-02-03 13:05:56.285388 splunktalib-3.0.3/LICENSE
--rw-r--r--   0        0        0     1089 2023-02-03 13:06:36.265318 splunktalib-3.0.3/pyproject.toml
--rw-r--r--   0        0        0      598 2023-02-03 13:06:36.261318 splunktalib-3.0.3/splunktalib/__init__.py
--rw-r--r--   0        0        0      575 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/__init__.py
--rw-r--r--   0        0        0      594 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/consts.py
--rw-r--r--   0        0        0     4951 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/log.py
--rw-r--r--   0        0        0     1599 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/pattern.py
--rw-r--r--   0        0        0     3922 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/util.py
--rw-r--r--   0        0        0     2251 2023-02-03 13:05:56.285388 splunktalib-3.0.3/splunktalib/common/xml_dom_parser.py
--rw-r--r--   0        0        0      575 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/concurrent/__init__.py
--rw-r--r--   0        0        0     3497 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/concurrent/concurrent_executor.py
--rw-r--r--   0        0        0     2247 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/concurrent/process_pool.py
--rw-r--r--   0        0        0    10691 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/concurrent/thread_pool.py
--rw-r--r--   0        0        0      575 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/__init__.py
--rw-r--r--   0        0        0     6088 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/conf_endpoints.py
--rw-r--r--   0        0        0     9206 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/conf_manager.py
--rw-r--r--   0        0        0     7195 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/data_input_endpoints.py
--rw-r--r--   0        0        0     3467 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/property_endpoints.py
--rw-r--r--   0        0        0     1796 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/request.py
--rw-r--r--   0        0        0     6892 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/conf_manager/ta_conf_manager.py
--rw-r--r--   0        0        0    12871 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/credentials.py
--rw-r--r--   0        0        0     5830 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/event_writer.py
--rw-r--r--   0        0        0     2358 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/file_monitor.py
--rw-r--r--   0        0        0     7444 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/kv_client.py
--rw-r--r--   0        0        0     5207 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/modinput.py
--rw-r--r--   0        0        0     2586 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/orphan_process_monitor.py
--rw-r--r--   0        0        0     3001 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/rest.py
--rw-r--r--   0        0        0      575 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/schedule/__init__.py
--rw-r--r--   0        0        0     3065 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/schedule/job.py
--rw-r--r--   0        0        0     4637 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/schedule/scheduler.py
--rw-r--r--   0        0        0      667 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/setting.conf
--rw-r--r--   0        0        0     2336 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/splunk_cluster.py
--rw-r--r--   0        0        0     1906 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/splunk_platform.py
--rw-r--r--   0        0        0     9147 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/state_store.py
--rw-r--r--   0        0        0     2617 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/timer.py
--rw-r--r--   0        0        0     4779 2023-02-03 13:05:56.289389 splunktalib-3.0.3/splunktalib/timer_queue.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 splunktalib-3.0.3/setup.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 splunktalib-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-26 12:30:49.211469 splunktalib-3.0.4/LICENSE
+-rw-r--r--   0        0        0     1104 2023-05-26 12:31:21.624237 splunktalib-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0      598 2023-05-26 12:31:21.620237 splunktalib-3.0.4/splunktalib/__init__.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/__init__.py
+-rw-r--r--   0        0        0      594 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/consts.py
+-rw-r--r--   0        0        0     4951 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/log.py
+-rw-r--r--   0        0        0     1599 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/pattern.py
+-rw-r--r--   0        0        0     3922 2023-05-26 12:30:49.211469 splunktalib-3.0.4/splunktalib/common/util.py
+-rw-r--r--   0        0        0     2251 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/common/xml_dom_parser.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/__init__.py
+-rw-r--r--   0        0        0     3497 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/concurrent_executor.py
+-rw-r--r--   0        0        0     2247 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/process_pool.py
+-rw-r--r--   0        0        0    10691 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/concurrent/thread_pool.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/__init__.py
+-rw-r--r--   0        0        0     6088 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/conf_endpoints.py
+-rw-r--r--   0        0        0     9206 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/conf_manager.py
+-rw-r--r--   0        0        0     7195 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/data_input_endpoints.py
+-rw-r--r--   0        0        0     3467 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/property_endpoints.py
+-rw-r--r--   0        0        0     1796 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/request.py
+-rw-r--r--   0        0        0     6892 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/conf_manager/ta_conf_manager.py
+-rw-r--r--   0        0        0    12871 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/credentials.py
+-rw-r--r--   0        0        0     5830 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/event_writer.py
+-rw-r--r--   0        0        0     2358 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/file_monitor.py
+-rw-r--r--   0        0        0     7444 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/kv_client.py
+-rw-r--r--   0        0        0     5207 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/modinput.py
+-rw-r--r--   0        0        0     2586 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/orphan_process_monitor.py
+-rw-r--r--   0        0        0     3001 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/rest.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/job.py
+-rw-r--r--   0        0        0     4637 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/schedule/scheduler.py
+-rw-r--r--   0        0        0      667 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/setting.conf
+-rw-r--r--   0        0        0     2336 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/splunk_cluster.py
+-rw-r--r--   0        0        0     1906 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/splunk_platform.py
+-rw-r--r--   0        0        0     9147 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/state_store.py
+-rw-r--r--   0        0        0     2617 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/timer.py
+-rw-r--r--   0        0        0     4779 2023-05-26 12:30:49.215469 splunktalib-3.0.4/splunktalib/timer_queue.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 splunktalib-3.0.4/PKG-INFO
```

### Comparing `splunktalib-3.0.3/LICENSE` & `splunktalib-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/pyproject.toml` & `splunktalib-3.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "splunktalib"
-version = "3.0.3"
+version = "3.0.4"
 description = "Supporting library for Splunk Add-ons"
 authors = ["rfaircloth-splunk <rfaircloth@splunk.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/splunk/addonfactory-ta-library-python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 sortedcontainers = "^2"
 defusedxml = "^0"
-requests = "^2.26.0"
+requests = "^2.31.0"
+urllib3 = "<2"
 
 [tool.poetry.dev-dependencies]
 
 
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `splunktalib-3.0.3/splunktalib/__init__.py` & `splunktalib-3.0.4/splunktalib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "3.0.3"
+__version__ = "3.0.4"
```

### Comparing `splunktalib-3.0.3/splunktalib/common/__init__.py` & `splunktalib-3.0.4/splunktalib/common/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/common/consts.py` & `splunktalib-3.0.4/splunktalib/common/consts.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/common/log.py` & `splunktalib-3.0.4/splunktalib/common/log.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/common/pattern.py` & `splunktalib-3.0.4/splunktalib/common/pattern.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/common/util.py` & `splunktalib-3.0.4/splunktalib/common/util.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/common/xml_dom_parser.py` & `splunktalib-3.0.4/splunktalib/common/xml_dom_parser.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/concurrent/__init__.py` & `splunktalib-3.0.4/splunktalib/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/concurrent/concurrent_executor.py` & `splunktalib-3.0.4/splunktalib/concurrent/concurrent_executor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/concurrent/process_pool.py` & `splunktalib-3.0.4/splunktalib/concurrent/process_pool.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/concurrent/thread_pool.py` & `splunktalib-3.0.4/splunktalib/concurrent/thread_pool.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/__init__.py` & `splunktalib-3.0.4/splunktalib/conf_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/conf_endpoints.py` & `splunktalib-3.0.4/splunktalib/conf_manager/conf_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/conf_manager.py` & `splunktalib-3.0.4/splunktalib/conf_manager/conf_manager.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/data_input_endpoints.py` & `splunktalib-3.0.4/splunktalib/conf_manager/data_input_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/property_endpoints.py` & `splunktalib-3.0.4/splunktalib/conf_manager/property_endpoints.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/request.py` & `splunktalib-3.0.4/splunktalib/conf_manager/request.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/conf_manager/ta_conf_manager.py` & `splunktalib-3.0.4/splunktalib/conf_manager/ta_conf_manager.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/credentials.py` & `splunktalib-3.0.4/splunktalib/credentials.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/event_writer.py` & `splunktalib-3.0.4/splunktalib/event_writer.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/file_monitor.py` & `splunktalib-3.0.4/splunktalib/file_monitor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/kv_client.py` & `splunktalib-3.0.4/splunktalib/kv_client.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/modinput.py` & `splunktalib-3.0.4/splunktalib/modinput.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/orphan_process_monitor.py` & `splunktalib-3.0.4/splunktalib/orphan_process_monitor.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/rest.py` & `splunktalib-3.0.4/splunktalib/rest.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/schedule/__init__.py` & `splunktalib-3.0.4/splunktalib/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/schedule/job.py` & `splunktalib-3.0.4/splunktalib/schedule/job.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/schedule/scheduler.py` & `splunktalib-3.0.4/splunktalib/schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/setting.conf` & `splunktalib-3.0.4/splunktalib/setting.conf`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/splunk_cluster.py` & `splunktalib-3.0.4/splunktalib/splunk_cluster.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/splunk_platform.py` & `splunktalib-3.0.4/splunktalib/splunk_platform.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/state_store.py` & `splunktalib-3.0.4/splunktalib/state_store.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/timer.py` & `splunktalib-3.0.4/splunktalib/timer.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/splunktalib/timer_queue.py` & `splunktalib-3.0.4/splunktalib/timer_queue.py`

 * *Files identical despite different names*

### Comparing `splunktalib-3.0.3/PKG-INFO` & `splunktalib-3.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: splunktalib
-Version: 3.0.3
+Version: 3.0.4
 Summary: Supporting library for Splunk Add-ons
 Home-page: https://github.com/splunk/addonfactory-ta-library-python
 License: Apache-2.0
 Author: rfaircloth-splunk
 Author-email: rfaircloth@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: defusedxml (>=0,<1)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sortedcontainers (>=2,<3)
+Requires-Dist: urllib3 (<2)
 Project-URL: Repository, https://github.com/splunk/addonfactory-ta-library-python
```


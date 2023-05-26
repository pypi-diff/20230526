# Comparing `tmp/splunktaucclib-6.0.8.tar.gz` & `tmp/splunktaucclib-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splunktaucclib-6.0.8.tar", max compression
+gzip compressed data, was "splunktaucclib-6.0.9.tar", max compression
```

## Comparing `splunktaucclib-6.0.8.tar` & `splunktaucclib-6.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11341 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/LICENSE
--rw-r--r--   0        0        0     1097 2023-05-18 12:36:58.458221 splunktaucclib-6.0.8/pyproject.toml
--rw-r--r--   0        0        0      598 2023-05-18 12:36:58.454220 splunktaucclib-6.0.8/splunktaucclib/__init__.py
--rw-r--r--   0        0        0     6826 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/alert_actions_base.py
--rw-r--r--   0        0        0    24625 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/cim_actions.py
--rw-r--r--   0        0        0     1625 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/common/__init__.py
--rw-r--r--   0        0        0     1607 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/common/log.py
--rw-r--r--   0        0        0    14532 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/config.py
--rw-r--r--   0        0        0      575 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/data_collection/__init__.py
--rw-r--r--   0        0        0     2423 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_checkpoint_manager.py
--rw-r--r--   0        0        0     8905 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_config.py
--rw-r--r--   0        0        0     1360 2023-05-18 12:36:11.370415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_consts.py
--rw-r--r--   0        0        0     3084 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_client.py
--rw-r--r--   0        0        0     7196 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_collector.py
--rw-r--r--   0        0        0     5505 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_loader.py
--rw-r--r--   0        0        0     5215 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_helper.py
--rw-r--r--   0        0        0     6617 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_mod_input.py
--rw-r--r--   0        0        0     2187 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/global_config/__init__.py
--rw-r--r--   0        0        0    12211 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/global_config/configuration.py
--rw-r--r--   0        0        0     2354 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/global_config/schema.py
--rw-r--r--   0        0        0      575 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/modinput_wrapper/__init__.py
--rw-r--r--   0        0        0    22729 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/modinput_wrapper/base_modinput.py
--rw-r--r--   0        0        0      622 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/__init__.py
--rw-r--r--   0        0        0     6452 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/admin_external.py
--rw-r--r--   0        0        0    24305 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/base.py
--rw-r--r--   0        0        0     1499 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/base_hook_mixin.py
--rw-r--r--   0        0        0     5783 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/cred_mgmt.py
--rw-r--r--   0        0        0    16618 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/credentials.py
--rw-r--r--   0        0        0     6857 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/datainput.py
--rw-r--r--   0        0        0     2122 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/eai.py
--rw-r--r--   0        0        0     4331 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/__init__.py
--rw-r--r--   0        0        0     8368 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/converter.py
--rw-r--r--   0        0        0     2103 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/field.py
--rw-r--r--   0        0        0    13158 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/validator.py
--rw-r--r--   0        0        0      913 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/entity.py
--rw-r--r--   0        0        0     1526 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/error.py
--rw-r--r--   0        0        0     5743 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/error_ctl.py
--rw-r--r--   0        0        0    13772 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/handler.py
--rw-r--r--   0        0        0     5916 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/multimodel.py
--rw-r--r--   0        0        0     2952 2023-05-18 12:36:11.374415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/normaliser.py
--rw-r--r--   0        0        0     6854 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/poster.py
--rw-r--r--   0        0        0     1115 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/schema.py
--rw-r--r--   0        0        0     5023 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/teardown.py
--rw-r--r--   0        0        0     4461 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/util.py
--rw-r--r--   0        0        0     9160 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/rest_handler/validator.py
--rw-r--r--   0        0        0      575 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/rest_helper.py
--rw-r--r--   0        0        0     7768 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/rest_migration.py
--rw-r--r--   0        0        0    13882 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/setup_util.py
--rw-r--r--   0        0        0     1152 2023-05-18 12:36:11.378415 splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/utility.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 splunktaucclib-6.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/LICENSE
+-rw-r--r--   0        0        0     1092 2023-05-26 12:40:30.068767 splunktaucclib-6.0.9/pyproject.toml
+-rw-r--r--   0        0        0      598 2023-05-26 12:40:30.064767 splunktaucclib-6.0.9/splunktaucclib/__init__.py
+-rw-r--r--   0        0        0     6826 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/alert_actions_base.py
+-rw-r--r--   0        0        0    24625 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/cim_actions.py
+-rw-r--r--   0        0        0     1625 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/common/__init__.py
+-rw-r--r--   0        0        0     1607 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/common/log.py
+-rw-r--r--   0        0        0    14532 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/config.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/__init__.py
+-rw-r--r--   0        0        0     2423 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_checkpoint_manager.py
+-rw-r--r--   0        0        0     8905 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_config.py
+-rw-r--r--   0        0        0     1360 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_consts.py
+-rw-r--r--   0        0        0     3084 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_client.py
+-rw-r--r--   0        0        0     7196 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_collector.py
+-rw-r--r--   0        0        0     5505 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_loader.py
+-rw-r--r--   0        0        0     5215 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_helper.py
+-rw-r--r--   0        0        0     6617 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_mod_input.py
+-rw-r--r--   0        0        0     2187 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/global_config/__init__.py
+-rw-r--r--   0        0        0    12211 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/global_config/configuration.py
+-rw-r--r--   0        0        0     2354 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/global_config/schema.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/modinput_wrapper/__init__.py
+-rw-r--r--   0        0        0    22729 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/modinput_wrapper/base_modinput.py
+-rw-r--r--   0        0        0      622 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/__init__.py
+-rw-r--r--   0        0        0     6452 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/admin_external.py
+-rw-r--r--   0        0        0    24305 2023-05-26 12:39:58.840896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/base.py
+-rw-r--r--   0        0        0     1499 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/base_hook_mixin.py
+-rw-r--r--   0        0        0     5783 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/cred_mgmt.py
+-rw-r--r--   0        0        0    16618 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/credentials.py
+-rw-r--r--   0        0        0     6857 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/datainput.py
+-rw-r--r--   0        0        0     2122 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/eai.py
+-rw-r--r--   0        0        0     4331 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/__init__.py
+-rw-r--r--   0        0        0     8368 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/converter.py
+-rw-r--r--   0        0        0     2103 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/field.py
+-rw-r--r--   0        0        0    13158 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/validator.py
+-rw-r--r--   0        0        0      913 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/entity.py
+-rw-r--r--   0        0        0     1526 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/error.py
+-rw-r--r--   0        0        0     5743 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/error_ctl.py
+-rw-r--r--   0        0        0    13772 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/handler.py
+-rw-r--r--   0        0        0     5916 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/multimodel.py
+-rw-r--r--   0        0        0     2952 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/normaliser.py
+-rw-r--r--   0        0        0     6854 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/poster.py
+-rw-r--r--   0        0        0     1115 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/schema.py
+-rw-r--r--   0        0        0     5023 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/teardown.py
+-rw-r--r--   0        0        0     4461 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/util.py
+-rw-r--r--   0        0        0     9160 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/rest_handler/validator.py
+-rw-r--r--   0        0        0      575 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/rest_helper.py
+-rw-r--r--   0        0        0     7768 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/rest_migration.py
+-rw-r--r--   0        0        0    13882 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/setup_util.py
+-rw-r--r--   0        0        0     1152 2023-05-26 12:39:58.844896 splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/utility.py
+-rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 splunktaucclib-6.0.9/PKG-INFO
```

### Comparing `splunktaucclib-6.0.8/LICENSE` & `splunktaucclib-6.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/pyproject.toml` & `splunktaucclib-6.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "splunktaucclib"
-version = "6.0.8"
+version = "6.0.9"
 description = ""
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-splunktalib = "^3.0.0"
-requests = "^2.26.0"
+splunktalib = "^3.0.4"
+requests = "^2.31.0"
+urllib3 = "<2"
 PySocks = "^1.7.1"
 splunk-sdk = ">=1.6.18"
-solnlib = "^4.7.0"
+solnlib = "^4.11.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
-splunk-add-on-ucc-framework = "^5.24.0"
-requests = "^2.28.1"
+splunk-add-on-ucc-framework = "^5.27.1"
 splunk-packaging-toolkit = "^1.0.1"
 
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `splunktaucclib-6.0.8/splunktaucclib/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "6.0.8"
+__version__ = "6.0.9"
```

### Comparing `splunktaucclib-6.0.8/splunktaucclib/alert_actions_base.py` & `splunktaucclib-6.0.9/splunktaucclib/alert_actions_base.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/cim_actions.py` & `splunktaucclib-6.0.9/splunktaucclib/cim_actions.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/common/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/common/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/common/log.py` & `splunktaucclib-6.0.9/splunktaucclib/common/log.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/config.py` & `splunktaucclib-6.0.9/splunktaucclib/config.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_checkpoint_manager.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_config.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_config.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_consts.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_consts.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_client.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_client.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_collector.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_collector.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_data_loader.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_data_loader.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_helper.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_helper.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/data_collection/ta_mod_input.py` & `splunktaucclib-6.0.9/splunktaucclib/data_collection/ta_mod_input.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/global_config/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/global_config/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/global_config/configuration.py` & `splunktaucclib-6.0.9/splunktaucclib/global_config/configuration.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/global_config/schema.py` & `splunktaucclib-6.0.9/splunktaucclib/global_config/schema.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/modinput_wrapper/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/modinput_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/modinput_wrapper/base_modinput.py` & `splunktaucclib-6.0.9/splunktaucclib/modinput_wrapper/base_modinput.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/admin_external.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/admin_external.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/base.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/base.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/base_hook_mixin.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/base_hook_mixin.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/cred_mgmt.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/cred_mgmt.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/credentials.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/credentials.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/datainput.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/datainput.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/eai.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/eai.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/converter.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/converter.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/field.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/field.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/endpoint/validator.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/endpoint/validator.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/entity.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/entity.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/error.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/error.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/error_ctl.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/error_ctl.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/handler.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/handler.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/multimodel.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/multimodel.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/normaliser.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/normaliser.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/poster.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/poster.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/schema.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/schema.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/teardown.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/teardown.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/util.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/util.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/rest_handler/validator.py` & `splunktaucclib-6.0.9/splunktaucclib/rest_handler/validator.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/__init__.py` & `splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/__init__.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/rest_helper.py` & `splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/rest_helper.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/rest_migration.py` & `splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/rest_migration.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/setup_util.py` & `splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/setup_util.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/splunktaucclib/splunk_aoblib/utility.py` & `splunktaucclib-6.0.9/splunktaucclib/splunk_aoblib/utility.py`

 * *Files identical despite different names*

### Comparing `splunktaucclib-6.0.8/PKG-INFO` & `splunktaucclib-6.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: splunktaucclib
-Version: 6.0.8
+Version: 6.0.9
 Summary: 
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PySocks (>=1.7.1,<2.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: solnlib (>=4.7.0,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: solnlib (>=4.11.2,<5.0.0)
 Requires-Dist: splunk-sdk (>=1.6.18)
-Requires-Dist: splunktalib (>=3.0.0,<4.0.0)
+Requires-Dist: splunktalib (>=3.0.4,<4.0.0)
+Requires-Dist: urllib3 (<2)
```


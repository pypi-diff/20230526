# Comparing `tmp/cognite_extractor_utils-4.3.1.tar.gz` & `tmp/cognite_extractor_utils-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-4.3.1.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-5.0.0.tar", max compression
```

## Comparing `cognite_extractor_utils-4.3.1.tar` & `cognite_extractor_utils-5.0.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0    10173 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/LICENSE
--rw-r--r--   0        0        0     4091 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/README.md
--rw-r--r--   0        0        0      739 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0     3954 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/authentication.py
--rw-r--r--   0        0        0    15891 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/base.py
--rw-r--r--   0        0        0    32146 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/configtools.py
--rw-r--r--   0        0        0     1061 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0     4528 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/extraction_pipelines.py
--rw-r--r--   0        0        0     1003 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/logging_prometheus.py
--rw-r--r--   0        0        0    14598 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1005 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0     2853 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/retry.py
--rw-r--r--   0        0        0    17450 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     2083 2023-04-18 12:01:04.716326 cognite_extractor_utils-4.3.1/cognite/extractorutils/throttle.py
--rw-r--r--   0        0        0    54282 2023-04-18 12:01:04.720326 cognite_extractor_utils-4.3.1/cognite/extractorutils/uploader.py
--rw-r--r--   0        0        0     7404 2023-04-18 12:01:04.720326 cognite_extractor_utils-4.3.1/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-04-18 12:01:04.720326 cognite_extractor_utils-4.3.1/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0     5588 2023-04-18 12:01:04.720326 cognite_extractor_utils-4.3.1/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2073 2023-04-18 12:01:04.720326 cognite_extractor_utils-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     5494 1970-01-01 00:00:00.000000 cognite_extractor_utils-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/LICENSE
+-rw-r--r--   0        0        0     4091 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/README.md
+-rw-r--r--   0        0        0      739 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    15990 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     2861 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4294 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    18506 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0     9188 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1061 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    14604 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1005 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    17449 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3054 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5239 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3865 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5292 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    11351 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6888 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    25071 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7404 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    13352 2023-05-26 07:07:57.875121 cognite_extractor_utils-5.0.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     1650 2023-05-26 07:07:57.879121 cognite_extractor_utils-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.0.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-4.3.1/LICENSE` & `cognite_extractor_utils-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/README.md` & `cognite_extractor_utils-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "4.3.1"
+__version__ = "5.0.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/base.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,50 +8,44 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import argparse
 import logging
 import os
 import sys
-import traceback
 from dataclasses import is_dataclass
 from enum import Enum
 from threading import Event, Thread
 from types import TracebackType
 from typing import Any, Callable, Dict, Generic, Optional, Type, TypeVar
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import ExtractionPipeline, ExtractionPipelineRun
 from dotenv import find_dotenv, load_dotenv
 
-from cognite.extractorutils.configtools import (
-    BaseConfig,
-    ConfigResolver,
-    CustomConfigClass,
-    StateStoreConfig,
-    _BaseConfig,
-    load_yaml,
-)
+from cognite.extractorutils.configtools import BaseConfig, ConfigResolver, StateStoreConfig
 from cognite.extractorutils.exceptions import InvalidConfigError
 from cognite.extractorutils.metrics import BaseMetrics
 from cognite.extractorutils.statestore import AbstractStateStore, LocalStateStore, NoStateStore
 from cognite.extractorutils.util import set_event_on_interrupt
 
 
 class ReloadConfigAction(Enum):
     DO_NOTHING = 1
     REPLACE_ATTRIBUTE = 2
     SHUTDOWN = 3
     CALLBACK = 4
 
 
+CustomConfigClass = TypeVar("CustomConfigClass", bound=BaseConfig)
+
+
 class Extractor(Generic[CustomConfigClass]):
     """
     Base class for extractors.
 
     When used as a context manager, the Extractor class will parse command line arguments, load a configuration file,
     set up everything needed for the extractor to run, and call the ``run_handle``. If the extractor raises an
     exception, the exception will be handled by the Extractor class and logged and reported as an error.
@@ -208,15 +202,17 @@
         """
         Called on a successful exit of the extractor
         """
         if self.extraction_pipeline:
             self.logger.info("Reporting new successful run")
             self.cognite_client.extraction_pipelines.runs.create(
                 ExtractionPipelineRun(
-                    external_id=self.extraction_pipeline.external_id, status="success", message="Successful shutdown"
+                    extpipe_external_id=self.extraction_pipeline.external_id,
+                    status="success",
+                    message="Successful shutdown",
                 )
             )
 
     def _report_error(self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: TracebackType) -> None:
         """
         Called on an unsuccessful exit of the extractor
 
@@ -228,15 +224,15 @@
         self.logger.error("Unexpected error during extraction", exc_info=exc_val)
         if self.extraction_pipeline:
             message = f"{exc_type.__name__}: {str(exc_val)}"[:1000]
 
             self.logger.info(f"Reporting new failed run: {message}")
             self.cognite_client.extraction_pipelines.runs.create(
                 ExtractionPipelineRun(
-                    external_id=self.extraction_pipeline.external_id, status="failure", message=message
+                    extpipe_external_id=self.extraction_pipeline.external_id, status="failure", message=message
                 )
             )
 
     def __enter__(self) -> "Extractor":
         """
         Configures and initializes the global logger, cognite client, loads config file, state store, etc.
 
@@ -288,29 +284,31 @@
             while not self.cancellation_token.is_set():
                 self.cancellation_token.wait(self.heartbeat_waiting_time)
 
                 if not self.cancellation_token.is_set():
                     self.logger.info("Reporting new heartbeat")
                     try:
                         self.cognite_client.extraction_pipelines.runs.create(
-                            ExtractionPipelineRun(external_id=self.extraction_pipeline.external_id, status="seen")
+                            ExtractionPipelineRun(
+                                extpipe_external_id=self.extraction_pipeline.external_id, status="seen"
+                            )
                         )
                     except Exception:
                         self.logger.exception("Failed to report heartbeat")
 
         if self.extraction_pipeline:
             self.logger.info("Starting heartbeat loop")
             Thread(target=heartbeat_loop, name="HeartbeatLoop", daemon=True).start()
         else:
             self.logger.info("No extraction pipeline configured")
 
         if self.extraction_pipeline and self.continuous_extractor:
             self.cognite_client.extraction_pipelines.runs.create(
                 ExtractionPipelineRun(
-                    external_id=self.extraction_pipeline.external_id,
+                    extpipe_external_id=self.extraction_pipeline.external_id,
                     status="success",
                     message=f"New startup of {self.name}",
                 )
             )
 
         self.started = True
         return self
```

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,9 +392,9 @@
             if type(metric) == Metric and metric.type in ["gauge", "counter"]:
                 if len(metric.samples) == 0:
                     continue
 
                 external_id = self.external_id_prefix + metric.name
                 datapoints.append({"externalId": external_id, "datapoints": [(timestamp, metric.samples[0].value)]})
 
-        self.cdf_client.datapoints.insert_multiple(datapoints)
+        self.cdf_client.time_series.data.insert_multiple(datapoints)
         self.logger.debug("Pushed metrics to CDF tenant '%s'", self._cdf_project)
```

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/statestore.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 from cognite.client import CogniteClient
 from cognite.client.exceptions import CogniteAPIError
 from requests.exceptions import ConnectionError
 
 from cognite.extractorutils.uploader import DataPointList
 
 from ._inner_util import _DecimalDecoder, _DecimalEncoder, _resolve_log_level
-from .retry import retry
+from .util import retry
 
 RETRY_BACKOFF_FACTOR = 1.5
 RETRY_MAX_DELAY = 15
 RETRY_DELAY = 5
 RETRIES = 10
```

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-5.0.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-4.3.1/pyproject.toml` & `cognite_extractor_utils-5.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "4.3.1"
+version = "5.0.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -21,48 +21,29 @@
 multi_line_output=3            # corresponds to -m  flag
 include_trailing_comma=true    # corresponds to -tc flag
 skip_glob = '^((?!py$).)*$'    # this makes sort all Python files
 known_third_party = ["arrow", "cryptography", "dacite", "decorator", "dotenv", "more_itertools", "parameterized", "prometheus_client", "psutil", "pytest", "requests", "yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-cognite-sdk = ">=5.8, <6"
+cognite-sdk = ">=6.0, <7"
 prometheus-client = ">0.7.0, <=1.0.0"
 arrow = "^1.0.0"
 pyyaml = ">=5.3.0, <7"
 dacite = "^1.6.0"
 psutil = "^5.7.0"
 decorator = "^5.1.1"
 more-itertools = "^9.0.0"
 typing-extensions = ">=3.7.4, <5"
 python-dotenv = "^1.0.0"
-cognite-sdk-experimental = {version = "^0.110.0", optional = true}
 jq = [{version = "^1.3.0", platform = "macos"}, {version = "^1.3.0", platform = "linux"}]
 
 [tool.poetry.extras]
 experimental = ["cognite-sdk-experimental"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-isolated_build = true
-envlist = py38
-[testenv]
-setenv =
-    COGNITE_API_KEY={env:COGNITE_API_KEY}
-    COGNITE_BASE_URL={env:COGNITE_BASE_URL}
-    COGNITE_PROJECT={env:COGNITE_PROJECT}
-deps =
-    pytest
-    pytest-cov
-commands =
-    coverage run --source cognite.extractorutils -m pytest -v tests
-    coverage xml
-"""
-
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 mypy = "*"
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 sphinx = "^6.0.0"
```

### Comparing `cognite_extractor_utils-4.3.1/PKG-INFO` & `cognite_extractor_utils-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 4.3.1
+Version: 5.0.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: experimental
 Requires-Dist: arrow (>=1.0.0,<2.0.0)
-Requires-Dist: cognite-sdk (>=5.8,<6)
-Requires-Dist: cognite-sdk-experimental (>=0.110.0,<0.111.0) ; extra == "experimental"
+Requires-Dist: cognite-sdk (>=6.0,<7)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "linux"
 Requires-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "macos"
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
```

#### html2text {}

```diff
@@ -1,31 +1,29 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 4.3.1 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.0.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: experimental Requires-Dist: arrow
-(>=1.0.0,<2.0.0) Requires-Dist: cognite-sdk (>=5.8,<6) Requires-Dist: cognite-
-sdk-experimental (>=0.110.0,<0.111.0) ; extra == "experimental" Requires-Dist:
-dacite (>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-
-Dist: jq (>=1.3.0,<2.0.0) ; sys_platform == "linux" Requires-Dist: jq
-(>=1.3.0,<2.0.0) ; sys_platform == "macos" Requires-Dist: more-itertools
-(>=9.0.0,<10.0.0) Requires-Dist: prometheus-client (>0.7.0,<=1.0.0) Requires-
-Dist: psutil (>=5.7.0,<6.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: pyyaml (>=5.3.0,<7) Requires-Dist: typing-extensions
-(>=3.7.4,<5) Project-URL: Repository, https://github.com/cognitedata/python-
-extractor-utils Description-Content-Type: text/markdown [Cognite_logo] Cognite
-Python `extractor-utils` ================================ [![Build Status]
-(https://github.com/cognitedata/python-extractor-utils/workflows/release/
-badge.svg)](https://github.com/cognitedata/python-extractor-utils/actions) [!
-[Documentation Status](https://readthedocs.com/projects/cognite-extractor-
-utils/badge/
+(>=1.0.0,<2.0.0) Requires-Dist: cognite-sdk (>=6.0,<7) Requires-Dist: dacite
+(>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-Dist: jq
+(>=1.3.0,<2.0.0) ; sys_platform == "linux" Requires-Dist: jq (>=1.3.0,<2.0.0) ;
+sys_platform == "macos" Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
+Requires-Dist: prometheus-client (>0.7.0,<=1.0.0) Requires-Dist: psutil
+(>=5.7.0,<6.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
+pyyaml (>=5.3.0,<7) Requires-Dist: typing-extensions (>=3.7.4,<5) Project-URL:
+Repository, https://github.com/cognitedata/python-extractor-utils Description-
+Content-Type: text/markdown [Cognite_logo] Cognite Python `extractor-utils`
+================================ [![Build Status](https://github.com/
+cognitedata/python-extractor-utils/workflows/release/badge.svg)](https://
+github.com/cognitedata/python-extractor-utils/actions) [![Documentation Status]
+(https://readthedocs.com/projects/cognite-extractor-utils/badge/
 ?version=latest&token=a9bab88214cbf624706005f6a71bbd77964efc910f8e527c7b3d75edc016397c)]
 (https://cognite-extractor-utils.readthedocs-hosted.com/en/latest/
 ?badge=latest) [![codecov](https://codecov.io/gh/cognitedata/python-extractor-
 utils/branch/master/graph/badge.svg?token=7AmVCpAh7I)](https://codecov.io/gh/
 cognitedata/python-extractor-utils) [![PyPI version](https://badge.fury.io/py/
 cognite-extractor-utils.svg)](https://pypi.org/project/cognite-extractor-utils)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cognite-
```


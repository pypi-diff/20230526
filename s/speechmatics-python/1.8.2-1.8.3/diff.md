# Comparing `tmp/speechmatics-python-1.8.2.tar.gz` & `tmp/speechmatics-python-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechmatics-python-1.8.2.tar", last modified: Thu May 18 18:45:48 2023, max compression
+gzip compressed data, was "speechmatics-python-1.8.3.tar", last modified: Fri May 26 12:06:28 2023, max compression
```

## Comparing `speechmatics-python-1.8.2.tar` & `speechmatics-python-1.8.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.550819 speechmatics-python-1.8.2/speechmatics/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/batch_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28866 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/speechmatics/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/speechmatics_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 18:45:48.000000 speechmatics-python-1.8.2/speechmatics_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:48.554819 speechmatics-python-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/mock_rt_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_cli_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-18 18:45:37.000000 speechmatics-python-1.8.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-05-26 12:06:28.611637 speechmatics-python-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 12:06:28.611637 speechmatics-python-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/speechmatics/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14238 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/batch_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27404 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/speechmatics/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/speechmatics_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 12:06:28.000000 speechmatics-python-1.8.3/speechmatics_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:28.607637 speechmatics-python-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/mock_rt_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_cli_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-26 12:06:13.000000 speechmatics-python-1.8.3/tests/utils.py
```

### Comparing `speechmatics-python-1.8.2/CHANGELOG.md` & `speechmatics-python-1.8.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.8.3]
+
+### Added
+
+- Pass sdk information to batch and rt requests
+- Add support for providing just auth_token ConnectionSettings
+- Use default URLs + .toml config in python sdk
+
+### Fixed
+
+- Fixed an issue in the batch client where jobs with fetch_url were not able to be submitted
+- Fixed reading translation config from config file
+
 ## [1.8.2]
 
 ### Fixed
 
 - TranscriptionConfig.enable_partials defaults to False
 
 ## [1.8.1]
```

### Comparing `speechmatics-python-1.8.2/LICENSE.txt` & `speechmatics-python-1.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/setup.py` & `speechmatics-python-1.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/speechmatics/adapters.py` & `speechmatics-python-1.8.3/speechmatics/adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/speechmatics/batch_client.py` & `speechmatics-python-1.8.3/speechmatics/batch_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,85 +2,127 @@
 """
 Wrapper library to interface with Speechmatics ASR batch v2 API.
 """
 
 import json
 import logging
 import os
+from pathlib import Path
 import time
-from typing import Any, Dict, Tuple, Union, List
+from typing import Any, Dict, List, Tuple, Union
 
 import httpx
 from polling2 import poll
 
-from speechmatics.exceptions import (
-    TranscriptionError,
-    JobNotFoundException,
-)
-from speechmatics.models import ConnectionSettings, BatchTranscriptionConfig
+from speechmatics.exceptions import JobNotFoundException, TranscriptionError
+from speechmatics.helpers import get_version
+from speechmatics.models import BatchTranscriptionConfig, ConnectionSettings, UsageMode
 
 LOGGER = logging.getLogger(__name__)
 
 # If the logging level is set to DEBUG then websockets logs very verbosely,
 # including a hex dump of every message being sent. Setting the websockets
 # logger at INFO level specifically prevents this spam.
 logging.getLogger("websockets.protocol").setLevel(logging.INFO)
 
 POLLING_DURATION = 15
 
 
+class _ForceMultipartDict(dict):
+    """Creates a dictionary that evaluates to True, even if empty.
+    Used in submit_job() to force proper multipart encoding when fetch_data is used.
+    See https://github.com/encode/httpx/discussions/2399 (link to psf/requests#1081) for details.
+    """
+
+    def __bool__(self):
+        return True
+
+
+class HttpClient(httpx.Client):
+    """Wrapper class around httpx.Client that adds the sm-sdk query parameter to request urls"""
+
+    def __init__(self, *args, **kwargs):
+        self._from_cli = False
+        if "from_cli" in kwargs:
+            self._from_cli = kwargs["from_cli"]
+            kwargs.pop("from_cli")
+        super().__init__(*args, **kwargs)
+
+    def build_request(self, method: str, url, *args, **kwargs):
+        cli = "-cli" if self._from_cli is True else ""
+        version = get_version()
+        url = httpx.URL(url)
+        url = url.copy_merge_params({"sm-sdk": f"python{cli}-{version}"})
+        return super().build_request(method, url, *args, **kwargs)
+
+
 class BatchClient:
     """Client class for Speechmatics Batch ASR REST API.
 
     This client may be used directly but must be closed afterwards, e.g.::
 
-        settings = ConnectionSettings(url="https://{api}/v2",
-        auth_token="{token}")
-        client = BatchClient(settings)
+        client = BatchClient(auth_token)
         client.connect()
         list_of_jobs = client.list_jobs()
         client.close()
 
     It may also be used as a context manager, which handles opening and
     closing the connection for you, e.g.::
 
         with BatchClient(settings) as client:
             list_of_jobs = client.list_jobs()
 
     """
 
-    def __init__(self, connection_settings: ConnectionSettings):
-        """Constructor method.
-
-        :param connection_settings: Connection settings for API
-        :type connection_settings: speechmatics.models.ConnectionSettings.
-        """
-        if connection_settings.url[-1] == "/":
-            connection_settings.url = connection_settings.url[:-1]
-
-        if not connection_settings.url.endswith("/v2"):
-            connection_settings.url = "/".join([connection_settings.url, "v2"])
+    def __init__(
+        self,
+        connection_settings_or_auth_token: Union[str, ConnectionSettings, None] = None,
+        from_cli=False,
+    ):
+        """
+        Args:
+            connection_settings_or_auth_token (Union[str, ConnectionSettings, None], optional)
+                If `str`,, assumes auth_token passed and default URL being used
+                If `None`, attempts using auth_token from config.
+                Defaults to `None`
+            from_clie (bool)
+        """
+        if not isinstance(connection_settings_or_auth_token, ConnectionSettings):
+            self.connection_settings = ConnectionSettings.create(
+                UsageMode.Batch, connection_settings_or_auth_token
+            )
+        else:
+            self.connection_settings = connection_settings_or_auth_token
+            self.connection_settings.set_missing_values_from_config(UsageMode.Batch)
+        if self.connection_settings.url[-1] == "/":
+            self.connection_settings.url = self.connection_settings.url[:-1]
+        if not self.connection_settings.url.endswith("/v2"):
+            self.connection_settings.url = "/".join(
+                [self.connection_settings.url, "v2"]
+            )
 
-        self.connection_settings = connection_settings
+        self.connection_settings = self.connection_settings
         self.transcription_config = None
 
         self.default_headers = {
             "Authorization": f"Bearer {self.connection_settings.auth_token}",
             "Accept-Charset": "utf-8",
         }
         self.api_client = None
+        self._from_cli = from_cli
 
     def connect(self):
         """Create a connection to a Speechmatics Transcription REST endpoint"""
-        self.api_client = httpx.Client(
+        self.api_client = HttpClient(
             base_url=self.connection_settings.url,
             timeout=None,
             headers=self.default_headers,
             http2=True,
             verify=self.connection_settings.ssl_context,
+            from_cli=self._from_cli,
         )
         return self
 
     def __enter__(self):
         return self.connect()
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -129,56 +171,72 @@
         :returns: List of jobs
         :rtype: List[Dict[str, Any]]
         """
         return self.send_request("GET", "jobs").json()["jobs"]
 
     def submit_job(
         self,
-        audio: Union[Tuple[str, bytes], str, os.PathLike],
+        audio: Union[Tuple[str, bytes], str, os.PathLike, None],
         transcription_config: Union[
             Dict[str, Any], BatchTranscriptionConfig, str, os.PathLike
         ],
     ) -> str:
         """
         Submits audio and config for transcription.
 
-        :param audio: Audio file path or tuple of filename and bytes
-        :type audio: os.Pathlike | str | Tuple[str, bytes]
+        :param audio: Audio file path or tuple of filename and bytes, or None if using fetch_url
+            NOTE: You must expliticly pass audio=None if providing a fetch_url in the config
+        :type audio: os.Pathlike | str | Tuple[str, bytes] | None
 
         :param transcription_config: Configuration for the transcription.
         :type transcription_config:
             Dict[str, Any] | speechmatics.models.BatchTranscriptionConfig | str
 
         :returns: Job ID
         :rtype: str
 
         :raises httpx.HTTPError: For any request errors, httpx exceptions are raised.
         """
+
+        # Handle getting config into a dict
         if isinstance(transcription_config, (str or os.PathLike)):
-            config_json = json.dumps(self._from_file(transcription_config, "json"))
+            with Path(transcription_config).expanduser().open(
+                mode="rt", encoding="utf-8"
+            ) as file:
+                config_dict = json.load(file)
         elif isinstance(transcription_config, BatchTranscriptionConfig):
-            config_json = transcription_config.as_config()
+            config_dict = json.loads(transcription_config.as_config())
         elif isinstance(transcription_config, dict):
-            config_json = json.dumps(transcription_config)
+            config_dict = transcription_config
         else:
             raise ValueError(
                 """Job configuration must be a BatchTranscriptionConfig object,
                 a filepath as a string or Path object, or a dict"""
             )
-        config_data = {"config": config_json.encode("utf-8")}
 
-        if isinstance(audio, (str, os.PathLike)):
-            audio_data = self._from_file(audio, "binary")
-        elif isinstance(audio, tuple):
+        # If audio=None, fetch_data must be specified
+        if audio and "fetch_data" in config_dict:
+            raise ValueError("Only one of audio or fetch_data can be set at a time")
+        if not audio and "fetch_data" in config_dict:
+            audio_data = None
+        elif isinstance(audio, (str, os.PathLike)):
+            with Path(audio).expanduser().open("rb") as file:
+                audio_data = os.path.basename(file.name), file.read()
+        elif isinstance(audio, tuple) and "fetch_data" not in config_dict:
             audio_data = audio
         else:
-            raise ValueError(
-                "Audio must be a filepath or a tuple of" "(filename, bytes)"
-            )
-        audio_file = {"data_file": audio_data}
+            raise ValueError("Audio must be a filepath or a tuple of (filename, bytes)")
+
+        # httpx seems to expect an un-nested json, throws a type error otherwise.
+        config_data = {"config": json.dumps(config_dict, ensure_ascii=False)}
+
+        if audio_data:
+            audio_file = {"data_file": audio_data}
+        else:
+            audio_file = _ForceMultipartDict()
 
         response = self.send_request("POST", "jobs", data=config_data, files=audio_file)
         return response.json()["id"]
 
     def get_job_result(
         self,
         job_id: str,
@@ -301,15 +359,14 @@
         :rtype: Union[str, Dict[str, Any]]
 
         :raises JobNotFoundException : When a job_id is not found.
         :raises httpx.HTTPError: For any request other than 404, httpx exceptions are raised.
         """
 
         def _poll_for_status() -> bool:
-
             job_status = self.check_job_status(job_id)["job"]["status"]
             if job_status == "done":
                 return True
             if job_status == "running":
                 LOGGER.info(
                     "Job ID %s still running, polling again in %s seconds.",
                     job_id,
@@ -319,34 +376,18 @@
             raise TranscriptionError(f"{job_id} status {job_status}")
 
         status = self.check_job_status(job_id)
 
         if status["job"]["status"] == "done":
             return self.get_job_result(job_id, transcription_format)
 
-        min_rtf = 0.25
+        min_rtf = 0.10
         duration = status["job"]["duration"]
         LOGGER.info(
             "Waiting %i sec to begin polling for completion.", round(duration * min_rtf)
         )
         # Wait until the min. processing time has passed before polling.
         time.sleep(duration * min_rtf)
 
         LOGGER.info("Starting poll.")
         poll(_poll_for_status, step=POLLING_DURATION, timeout=3600)
         return self.get_job_result(job_id, transcription_format)
-
-    # pylint:disable=no-self-use
-    # pylint:disable=inconsistent-return-statements
-    def _from_file(
-        self, path: Union[str, os.PathLike], filetype: str
-    ) -> Union[Dict[Any, Any], Tuple[str, bytes]]:
-        """Retrieve data from a file.
-        For filetype=="json", returns a dict
-        For filetype=="binary", returns a tuple of (filename, data)
-        """
-        if filetype == "json":
-            with open(path, mode="rt", encoding="utf-8") as file:
-                return json.load(file)
-        elif filetype == "binary":
-            with open(path, mode="rb") as file:
-                return os.path.basename(file.name), file.read()
```

### Comparing `speechmatics-python-1.8.2/speechmatics/cli.py` & `speechmatics-python-1.8.3/speechmatics/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,49 +5,41 @@
 """
 
 import json
 import logging
 import os
 import ssl
 import sys
-from socket import gaierror
-
 from dataclasses import dataclass
-from typing import List, Dict, Union, Tuple, Any
+from socket import gaierror
+from typing import List
 
-import toml
 import httpx
+import toml
 from websockets.exceptions import WebSocketException
 
 import speechmatics.adapters
-from speechmatics.helpers import _process_status_errors
-from speechmatics.client import WebsocketClient
 from speechmatics.batch_client import BatchClient
-from speechmatics.exceptions import (
-    TranscriptionError,
-    JobNotFoundException,
-)
+from speechmatics.cli_parser import parse_args
+from speechmatics.client import WebsocketClient
+from speechmatics.config import read_config_from_home
+from speechmatics.constants import BATCH_SELF_SERVICE_URL, RT_SELF_SERVICE_URL
+from speechmatics.exceptions import JobNotFoundException, TranscriptionError
+from speechmatics.helpers import _process_status_errors
 from speechmatics.models import (
-    TranscriptionConfig,
     AudioSettings,
+    BatchLanguageIdentificationConfig,
+    BatchSpeakerDiarizationConfig,
+    BatchTranscriptionConfig,
     ClientMessageType,
-    ServerMessageType,
     ConnectionSettings,
-    BatchTranscriptionConfig,
-    BatchSpeakerDiarizationConfig,
     RTSpeakerDiarizationConfig,
     RTTranslationConfig,
-    BatchLanguageIdentificationConfig,
-)
-from speechmatics.cli_parser import (
-    parse_args,
-)
-from speechmatics.constants import (
-    BATCH_SELF_SERVICE_URL,
-    RT_SELF_SERVICE_URL,
+    ServerMessageType,
+    TranscriptionConfig,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 
 def print_symbol(symbol):
     """
@@ -139,42 +131,28 @@
     :return: Settings for the WebSocket connection.
     :rtype: speechmatics.models.ConnectionSettings
     """
     auth_token = args.get("auth_token")
     generate_temp_token = args.get("generate_temp_token")
     url = args.get("url")
 
-    home_directory = os.path.expanduser("~")
-    if os.path.exists(f"{home_directory}/.speechmatics/config"):
-        cli_config = {"default": {}}
-        with open(
-            f"{home_directory}/.speechmatics/config", "r", encoding="UTF-8"
-        ) as file:
-            cli_config = toml.load(file)
-        profile = args.get("profile", "default")
-        if profile not in cli_config:
-            raise SystemExit(
-                f"Cannot unset config for profile {profile}. Profile does not exist."
-            )
-        if "auth_token" in cli_config[profile] and auth_token is None:
-            auth_token = cli_config[profile].get("auth_token")
-        if "generate_temp_token" in cli_config[profile]:
-            generate_temp_token = cli_config[profile].get("generate_temp_token")
-        if (
-            url is None
-            and args.get("mode") == "batch"
-            and "batch_url" in cli_config[profile]
-        ):
-            url = cli_config[profile].get("batch_url")
+    stored_config = read_config_from_home(args.get("profile", "default"))
+    if stored_config is not None:
+        if auth_token is None and stored_config.get("auth_token") is not None:
+            auth_token = stored_config["auth_token"]
         if (
-            url is None
-            and args.get("mode") == "rt"
-            and "realtime_url" in cli_config[profile]
+            generate_temp_token is None
+            and stored_config.get("generate_temp_token") is not None
         ):
-            url = cli_config[profile].get("realtime_url")
+            generate_temp_token = stored_config["generate_temp_token"]
+
+        if url is None and args.get("mode") == "batch" and "batch_url" in stored_config:
+            url = stored_config.get("batch_url")
+        if url is None and args.get("mode") == "rt" and "realtime_url" in stored_config:
+            url = stored_config.get("realtime_url")
 
     if url is None:
         if args.get("mode") == "batch":
             url = BATCH_SELF_SERVICE_URL
         else:
             url = f"{RT_SELF_SERVICE_URL}/{lang}"
 
@@ -282,21 +260,29 @@
 
     if args.get("speaker_diarization_sensitivity") is not None:
         speaker_sensitivity = args.get("speaker_diarization_sensitivity")
         config["speaker_diarization_config"] = BatchSpeakerDiarizationConfig(
             speaker_sensitivity=speaker_sensitivity
         )
 
-    if args.get("translation_target_languages") is not None:
-        translation_target_languages = args.get("translation_target_languages")
-        enable_partials = args.get("enable_partials", False) or args.get(
-            "enable_translation_partials", False
+    translation_config = config.get("translation_config", {})
+    args_target_languages = args.get("translation_target_languages")
+    if translation_config or args_target_languages:
+        enable_partials = (
+            args.get("enable_partials", False)
+            or args.get("enable_translation_partials", False)
+            or translation_config.get("enable_partials", False)
+        )
+        target_languages = (
+            args_target_languages.split(",")
+            if args_target_languages
+            else translation_config.get("target_languages")
         )
         config["translation_config"] = RTTranslationConfig(
-            target_languages=translation_target_languages.split(","),
+            target_languages=target_languages,
             enable_partials=enable_partials,
         )
 
     if args.get("langid_expected_languages") is not None:
         langid_expected_languages = args.get("langid_expected_languages")
         config["language_identification_config"] = BatchLanguageIdentificationConfig(
             expected_languages=langid_expected_languages.split(",")
@@ -488,50 +474,14 @@
     if language in {"ja", "cmn"}:
         separator = ""
     else:
         separator = " "
     return separator.join(words)
 
 
-def submit_job_and_wait(
-    connection_settings: ConnectionSettings,
-    audio: Union[Tuple[str, bytes], str, os.PathLike],
-    transcription_config: Union[
-        Dict[str, Any], BatchTranscriptionConfig, str, os.PathLike
-    ],
-    transcription_format: str = "txt",
-) -> str:
-    """
-    Submit a job, waiting for response.
-    This is the ``batch transcribe`` command.
-
-    :param connection_settings: Settings for API connection.
-    :type connection_settings: speechmatics.models.ConnectionSettings
-
-    :param audio: Audio file path or tuple of filename and bytes
-    :type audio: os.Pathlike | str | Tuple[str, bytes]
-
-    :param transcription_config: Configuration for the transcription.
-    :type transcription_config:
-        Dict[str, Any] | speechmatics.models.BatchTranscriptionConfig | str
-
-    :param transcription_format: Format of transcript. Defaults to txt.
-        Valid options are json-v2, txt, srt. json is accepted as an
-        alias for json-v2.
-    :type format: str
-
-    :return: transcript in txt format
-    :rtype: str
-    """
-    with BatchClient(connection_settings) as client:
-        job_id = client.submit_job(audio, transcription_config)
-        print(f"Job submission successful. ID: {job_id} . Waiting for completion")
-        return client.wait_for_completion(job_id, transcription_format)
-
-
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-statements
 def main(args=None):
     """
     Main entrypoint.
 
     :param args: command-line arguments; defaults to None in which
@@ -619,15 +569,15 @@
     if settings.url.lower().startswith("ws://") and args["ssl_mode"] != "none":
         raise SystemExit(
             f"ssl_mode '{args['ssl_mode']}' is incompatible with"
             "protocol 'ws'. Use 'wss' instead."
         )
     if settings.url.lower().startswith("wss://") and args["ssl_mode"] == "none":
         raise SystemExit(
-            "ssl_mode 'none' is incompatible with protocol 'wss'." "Use 'ws' instead."
+            "ssl_mode 'none' is incompatible with protocol 'wss'. Use 'ws' instead."
         )
 
     transcripts = Transcripts(text="", json=[])
     add_printing_handlers(
         api,
         transcripts,
         enable_partials=args["enable_partials"],
@@ -638,15 +588,15 @@
         print_json=args["print_json"],
         translation_config=transcription_config.translation_config,
     )
 
     def run(stream):
         try:
             api.run_synchronously(
-                stream, transcription_config, get_audio_settings(args)
+                stream, transcription_config, get_audio_settings(args), from_cli=True
             )
         except KeyboardInterrupt:
             # Gracefully handle Ctrl-C, else we get a huge stack-trace.
             LOGGER.warning("Keyboard interrupt received.")
 
     if args["files"][0] == "-":
         run(sys.stdin.buffer)
@@ -659,24 +609,25 @@
 def batch_main(args):
     """Main dispatch for "batch" command set
 
     :param args: arguments from parse_args()
     :type args: argparse.Namespace
     """
     command = args["command"]
-    with BatchClient(get_connection_settings(args)) as batch_client:
+    with BatchClient(get_connection_settings(args), from_cli=True) as batch_client:
         if command == "transcribe":
             for filename in args["files"]:
                 print(f"Processing {filename}\n==========")
-                result = submit_job_and_wait(
-                    connection_settings=get_connection_settings(args),
-                    audio=filename,
-                    transcription_config=get_transcription_config(args),
-                    transcription_format=args["output_format"],
+                job_id = batch_client.submit_job(
+                    filename, get_transcription_config(args)
+                )
+                print(
+                    f"Job submission successful. ID: {job_id} . Waiting for completion"
                 )
+                result = batch_client.wait_for_completion(job_id, args["output_format"])
                 if args["output_format"] in ["json", "json-v2"]:
                     print(json.dumps(result, ensure_ascii=False))
                 else:
                     print(result)
                 print(f"==========\n{filename} completed!\n==========")
         elif command == "submit":
             for filename in args["files"]:
```

### Comparing `speechmatics-python-1.8.2/speechmatics/cli_parser.py` & `speechmatics-python-1.8.3/speechmatics/cli_parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # (c) 2022, Cantab Research Ltd.
 """
 Parsers used by the CLI to handle CLI arguments
 """
 import argparse
-from urllib.parse import urlparse
 import logging
+from urllib.parse import urlparse
 
 LOGGER = logging.getLogger(__name__)
 
 
 def additional_vocab_item(to_parse):
     """
     Parses a single item of additional vocab. Used in conjunction with the
```

### Comparing `speechmatics-python-1.8.2/speechmatics/client.py` & `speechmatics-python-1.8.3/speechmatics/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,34 @@
 """
 
 import asyncio
 import copy
 import json
 import logging
 import os
+from typing import Union
+from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
-import websockets
 import httpx
+import websockets
 
 from speechmatics.exceptions import (
     EndOfTranscriptException,
     ForceEndSession,
     TranscriptionError,
 )
-from speechmatics.models import ClientMessageType, ServerMessageType
-from speechmatics.helpers import json_utf8, read_in_chunks
-
+from speechmatics.helpers import get_version, json_utf8, read_in_chunks
+from speechmatics.models import (
+    AudioSettings,
+    ClientMessageType,
+    ConnectionSettings,
+    ServerMessageType,
+    TranscriptionConfig,
+    UsageMode,
+)
 
 LOGGER = logging.getLogger(__name__)
 
 # If the logging level is set to DEBUG then websockets logs very verbosely,
 # including a hex dump of every message being sent. Setting the websockets
 # logger at INFO level specifically prevents this spam.
 logging.getLogger("websockets.protocol").setLevel(logging.INFO)
@@ -41,16 +49,31 @@
     :param connection_settings: Settings for the WebSocket connection,
         including the URL of the server.
     :type connection_settings: speechmatics.models.ConnectionSettings
     """
 
     # pylint: disable=too-many-instance-attributes
 
-    def __init__(self, connection_settings):
-        self.connection_settings = connection_settings
+    def __init__(
+        self,
+        connection_settings_or_auth_token: Union[str, ConnectionSettings, None] = None,
+    ):
+        """
+        Args:
+            connection_settings_or_auth_token (Union[str, ConnectionSettings, None], optional): Defaults to None.
+                If `str`,, assumes auth_token passed and default URL being used
+                If `None`, attempts using auth_token from config.
+        """
+        if not isinstance(connection_settings_or_auth_token, ConnectionSettings):
+            self.connection_settings = ConnectionSettings.create(
+                UsageMode.RealTime, connection_settings_or_auth_token
+            )
+        else:
+            self.connection_settings = connection_settings_or_auth_token
+            self.connection_settings.set_missing_values_from_config(UsageMode.RealTime)
         self.websocket = None
         self.transcription_config = None
         self.translation_config = None
 
         self.event_handlers = {x: [] for x in ServerMessageType}
         self.middlewares = {x: [] for x in ClientMessageType}
 
@@ -379,15 +402,21 @@
             task.cancel()
 
         for task in done:
             exc = task.exception()
             if exc and not isinstance(exc, (EndOfTranscriptException, ForceEndSession)):
                 raise exc
 
-    async def run(self, stream, transcription_config, audio_settings):
+    async def run(
+        self,
+        stream,
+        transcription_config: TranscriptionConfig,
+        audio_settings=AudioSettings(),
+        from_cli=False,
+    ):
         """
         Begin a new recognition session.
         This will run asynchronously. Most callers may prefer to use
         :py:meth:`run_synchronously` which will block until the session is
         finished.
 
         :param stream: File-like object which an audio stream can be read from.
@@ -395,14 +424,17 @@
 
         :param transcription_config: Configuration for the transcription.
         :type transcription_config: speechmatics.models.TranscriptionConfig
 
         :param audio_settings: Configuration for the audio stream.
         :type audio_settings: speechmatics.models.AudioSettings
 
+        :param from_cli: Indicates whether the caller is the command-line interface or not.
+        :type from_cli: bool
+
         :raises Exception: Can raise any exception returned by the
             consumer/producer tasks.
         """
         self.transcription_config = transcription_config
         self.translation_config = transcription_config.translation_config
         self.seq_no = 0
         self._language_pack_info = None
@@ -419,17 +451,33 @@
             self.connection_settings.generate_temp_token
             and self.connection_settings.auth_token is not None
         ):
             temp_token = await _get_temp_token(self.connection_settings.auth_token)
             token = f"Bearer {temp_token}"
             extra_headers["Authorization"] = token
 
+        url = self.connection_settings.url
+        if not url.endswith(self.transcription_config.language):
+            if url.endswith("/"):
+                url += self.transcription_config.language
+            else:
+                url += f"/{self.transcription_config.language}"
+
+        # Extend connection url with sdk version information
+        cli = "-cli" if from_cli is True else ""
+        version = get_version()
+        parsed_url = urlparse(url)
+        query_params = dict(parse_qsl(parsed_url.query))
+        query_params["sm-sdk"] = f"python{cli}-{version}"
+        updated_query = urlencode(query_params)
+        updated_url = urlunparse(parsed_url._replace(query=updated_query))
+
         try:
             async with websockets.connect(  # pylint: disable=no-member
-                self.connection_settings.url,
+                updated_url,
                 ssl=self.connection_settings.ssl_context,
                 ping_timeout=self.connection_settings.ping_timeout_seconds,
                 # Don't limit the max. size of incoming messages
                 max_size=None,
                 extra_headers=extra_headers,
             ) as self.websocket:
                 await self._communicate(stream, audio_settings)
@@ -456,17 +504,18 @@
         asyncio.run(asyncio.wait_for(self.run(*args, **kwargs), timeout=timeout))
 
 
 async def _get_temp_token(api_key):
     """
     Used to get a temporary token from management platform api for SaaS users
     """
+    version = get_version()
     mp_api_url = os.getenv("SM_MANAGEMENT_PLATFORM_URL", "https://mp.speechmatics.com")
     endpoint = mp_api_url + "/v1/api_keys"
-    params = {"type": "rt"}
+    params = {"type": "rt", "sm-sdk": f"python-{version}"}
     body = {"ttl": 60}
     headers = {"Authorization": f"Bearer {api_key}", "Content-Type": "application/json"}
     # pylint: disable=no-member
     response = httpx.post(endpoint, json=body, params=params, headers=headers)
     response.raise_for_status()
     response.read()
     key_object = response.json()
```

### Comparing `speechmatics-python-1.8.2/speechmatics/exceptions.py` & `speechmatics-python-1.8.3/speechmatics/exceptions.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/speechmatics/helpers.py` & `speechmatics-python-1.8.3/speechmatics/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # (c) 2020, Cantab Research Ltd.
 """
 Helper functions used by the library.
 """
 
 import asyncio
 import concurrent.futures
-import json
 import inspect
+import json
+import os
 import sys
 
+import pkg_resources
+
 
 def del_none(dictionary):
     """
     Recursively delete from the dictionary all entries which values are None.
     This function changes the input parameter in place.
 
     :param dictionary: input dictionary
@@ -68,14 +71,35 @@
                 )
 
         if not audio_chunk:
             break
         yield audio_chunk
 
 
+def get_version() -> str:
+    """
+    Reads the version number from the package or from VERSION file in case
+    the package information is not found.
+
+    :return: the library version
+    :rtype: str
+    """
+    try:
+        version = pkg_resources.get_distribution("speechmatics-python").version
+    except pkg_resources.DistributionNotFound:
+        # The library is not running from the distributed package
+        # Get the version from the VERSION file
+        base_path = os.path.abspath(os.path.dirname(__file__))
+        version_path = os.path.join(base_path, "..", "VERSION")
+        with open(version_path, "r", encoding="utf-8") as version_file:
+            version = version_file.read().strip()
+
+    return version
+
+
 def _process_status_errors(error):
     """
     Takes an httpx.HTTPSStatusError and prints in a useful format for CLI
 
     :param error: the status error produced by the server for a request
     :type error: httpx.HTTPStatusError
```

### Comparing `speechmatics-python-1.8.2/speechmatics/models.py` & `speechmatics-python-1.8.3/speechmatics/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # (c) 2020, Cantab Research Ltd.
 """
 Data models and message types used by the library.
 """
 
 import json
 import ssl
-
 from dataclasses import asdict, dataclass, field, fields
 from enum import Enum
-
 from typing import Any, Dict, List, Optional
 
+from speechmatics.config import CONFIG_PATH, read_config_from_home
+from speechmatics.constants import BATCH_SELF_SERVICE_URL, RT_SELF_SERVICE_URL
+
 
 @dataclass
 class FetchData:
     """Batch: Optional configuration for fetching file for transcription."""
 
     url: str
     """URL to fetch"""
@@ -301,14 +302,20 @@
         return {
             "type": "raw",
             "encoding": self.encoding,
             "sample_rate": self.sample_rate,
         }
 
 
+class UsageMode(str, Enum):
+    # pylint: disable=invalid-name
+    Batch = "batch"
+    RealTime = "rt"
+
+
 @dataclass
 class ConnectionSettings:
     """Defines connection parameters."""
 
     url: str
     """Websocket server endpoint."""
 
@@ -320,22 +327,71 @@
 
     semaphore_timeout_seconds: float = 120
     """Semaphore timeout in seconds."""
 
     ping_timeout_seconds: float = 60
     """Ping-pong timeout in seconds."""
 
-    auth_token: str = None
-    """auth token to authenticate a customer.
-    This auth token is only applicable for RT-SaaS."""
+    auth_token: Optional[str] = None
+    """auth token to authenticate a customer."""
 
     generate_temp_token: Optional[bool] = False
     """Automatically generate a temporary token for authentication.
     Non-enterprise customers must set this to True. Enterprise customers should set this to False."""
 
+    def set_missing_values_from_config(self, mode: UsageMode):
+        stored_config = read_config_from_home()
+        if self.url is None or self.url == "":
+            url_key = "realtime_url" if mode == UsageMode.RealTime else "batch_url"
+            if stored_config and url_key in stored_config:
+                self.url = stored_config[url_key]
+            else:
+                raise ValueError(f"No URL provided or set in {CONFIG_PATH}")
+        if self.auth_token is None or self.auth_token == "":
+            if stored_config and stored_config.get("auth_token"):
+                self.auth_token = stored_config["auth_token"]
+
+    @classmethod
+    def create(cls, mode: UsageMode, auth_token: Optional[str] = None):
+        stored_config = read_config_from_home()
+        default_url = (
+            RT_SELF_SERVICE_URL
+            if mode == UsageMode.RealTime
+            else BATCH_SELF_SERVICE_URL
+        )
+        url_key = "realtime_url" if mode == UsageMode.RealTime else "batch_url"
+        if stored_config and url_key in stored_config:
+            url = stored_config[url_key]
+        else:
+            url = default_url
+        if auth_token is not None:
+            return ConnectionSettings(
+                url=url,
+                auth_token=auth_token,
+                generate_temp_token=True,
+            )
+        if stored_config and stored_config.get("auth_token"):
+            url = stored_config.get(url_key, default_url)
+            return ConnectionSettings(
+                url,
+                auth_token=stored_config["auth_token"],
+                generate_temp_token=stored_config.get("generate_temp_token", True),
+            )
+        raise ValueError(f"No acces token provided or set in {CONFIG_PATH}")
+
+
+@dataclass
+class RTConnectionSettings(ConnectionSettings):
+    url = f"{RT_SELF_SERVICE_URL}/en"
+
+
+@dataclass
+class BatchConnectionSettings(ConnectionSettings):
+    url = BATCH_SELF_SERVICE_URL
+
 
 class ClientMessageType(str, Enum):
     # pylint: disable=invalid-name
     """Real-time: Defines various messages sent from client to server."""
 
     StartRecognition = "StartRecognition"
     """Initiates a recognition job based on configuration set previously."""
```

### Comparing `speechmatics-python-1.8.2/speechmatics_python.egg-info/SOURCES.txt` & `speechmatics-python-1.8.3/speechmatics_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 setup.py
 speechmatics/__init__.py
 speechmatics/adapters.py
 speechmatics/batch_client.py
 speechmatics/cli.py
 speechmatics/cli_parser.py
 speechmatics/client.py
+speechmatics/config.py
 speechmatics/constants.py
 speechmatics/exceptions.py
 speechmatics/helpers.py
 speechmatics/models.py
 speechmatics_python.egg-info/PKG-INFO
 speechmatics_python.egg-info/SOURCES.txt
 speechmatics_python.egg-info/dependency_links.txt
```

### Comparing `speechmatics-python-1.8.2/tests/conftest.py` & `speechmatics-python-1.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/tests/mock_rt_server.py` & `speechmatics-python-1.8.3/tests/mock_rt_server.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/tests/test_adapters.py` & `speechmatics-python-1.8.3/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/tests/test_cli.py` & `speechmatics-python-1.8.3/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     ],
 )
 def test_cli_arg_parse_with_file(args, values):
     common_transcribe_args = ["--auth-token=xyz", "--url=example", "fake_file.wav"]
     test_args = args + common_transcribe_args
     actual_values = vars(cli.parse_args(args=test_args))
 
-    for (key, val) in values.items():
+    for key, val in values.items():
         assert actual_values[key] == val, f"Expected {actual_values} to match {values}"
 
 
 @pytest.mark.parametrize(
     "args, values",
     [
         (
@@ -275,15 +275,15 @@
     ],
 )
 def test_cli_arg_parse_transcribe_url(args, values):
     connection_args = ["--auth-token=xyz"]
     test_args = args + connection_args + ["fake_file.wav"]
     actual_values = vars(cli.parse_args(args=test_args))
 
-    for (key, val) in values.items():
+    for key, val in values.items():
         assert actual_values[key] == val
 
 
 @pytest.mark.parametrize(
     "args, values",
     [
         (
@@ -318,15 +318,15 @@
     ],
 )
 def test_cli_list_arg_parse_without_file(args, values):
     required_args = ["--url=example", "--auth-token=xyz"]
     test_args = args + required_args
     actual_values = vars(cli.parse_args(args=test_args))
 
-    for (key, val) in values.items():
+    for key, val in values.items():
         assert actual_values[key] == val
 
 
 def test_parse_additional_vocab(tmp_path, mocker):
     vocab_file = tmp_path / "vocab.json"
     vocab_file.write_text('["Speechmatics", "gnocchi"]')
     assert cli.parse_additional_vocab(vocab_file) == (["Speechmatics", "gnocchi"])
@@ -447,15 +447,15 @@
     cli.main(vars(cli.parse_args(args)))
     mock_server.wait_for_clean_disconnects()
 
     assert mock_server.clients_connected_count == 1
     assert mock_server.clients_disconnected_count == 1
     assert mock_server.messages_received
     assert mock_server.messages_sent
-    assert mock_server.path == "/v2"
+    assert mock_server.path.startswith("/v2")
 
 
 def test_rt_main_with_temp_token_option(mock_server):
     args = [
         "-vv",
         "rt",
         "transcribe",
@@ -468,15 +468,15 @@
     cli.main(vars(cli.parse_args(args)))
     mock_server.wait_for_clean_disconnects()
 
     assert mock_server.clients_connected_count == 1
     assert mock_server.clients_disconnected_count == 1
     assert mock_server.messages_received
     assert mock_server.messages_sent
-    assert mock_server.path == "/v2"
+    assert mock_server.path.startswith("/v2")
 
 
 def test_rt_main_with_toml_config(mock_server):
     args = [
         "config",
         "set",
         "--auth-token=faketoken",
@@ -494,15 +494,15 @@
     cli.main(vars(cli.parse_args(args)))
     mock_server.wait_for_clean_disconnects()
     print(mock_server.messages_received)
     assert mock_server.clients_connected_count == 1
     assert mock_server.clients_disconnected_count == 1
     assert mock_server.messages_received
     assert mock_server.messages_sent
-    assert mock_server.path == "/v2"
+    assert mock_server.path.startswith("/v2")
 
 
 def test_rt_main_with_all_options(mock_server, tmp_path):
     vocab_file = tmp_path / "vocab.json"
     vocab_file.write_text(
         '["jabberwock", {"content": "brillig", "sounds_like": ["brillick"]}]'
     )
@@ -618,28 +618,33 @@
 
     assert msg["audio_format"]["type"] == "file"
     assert len(msg["audio_format"]) == 1
     assert msg["transcription_config"]["language"] == "xy"
     assert msg["transcription_config"]["domain"] == "fake"
     assert msg["transcription_config"]["enable_entities"] is True
     assert msg["transcription_config"].get("operating_point") is None
+    assert msg["translation_config"] is not None
+    assert msg["translation_config"]["enable_partials"] is False
+    assert msg["translation_config"]["target_languages"] == ["es"]
 
 
 def test_rt_main_with_config_file_cmdline_override(mock_server):
     audio_path = path_to_test_resource("ch.wav")
     config_path = path_to_test_resource("transcription_config.json")
 
     args = [
         "rt",
         "transcribe",
         "--ssl-mode=insecure",
         "--url",
         mock_server.url,
         "--config-file",
         config_path,
+        "--translation-langs=fr",
+        "--enable-translation-partials",
         "--auth-token=xyz",
         "--lang=yz",
         "--output-locale=en-US",
         "--domain=different",
         "--operating-point=enhanced",
         "--speaker-change-sensitivity",
         "0.8",
@@ -661,14 +666,17 @@
     assert len(msg["audio_format"]) == 1
     assert msg["transcription_config"]["language"] == "yz"
     assert msg["transcription_config"]["domain"] == "different"
     assert msg["transcription_config"]["enable_entities"] is True
     assert msg["transcription_config"]["output_locale"] == "en-US"
     assert msg["transcription_config"]["speaker_change_sensitivity"] == 0.8
     assert msg["transcription_config"]["operating_point"] == "enhanced"
+    assert msg["translation_config"] is not None
+    assert msg["translation_config"]["enable_partials"] is True
+    assert msg["translation_config"]["target_languages"] == ["fr"]
 
 
 @pytest.mark.parametrize(
     "args, values",
     (
         (
             ["config", "set", "--auth-token=faketoken", "--generate-temp-token"],
@@ -677,18 +685,17 @@
         (
             ["config", "unset", "--auth-token", "--generate-temp-token"],
             {"auth_token": True, "generate_temp_token": True},
         ),
     ),
 )
 def test_cli_argparse_config(args, values):
-
     actual_values = vars(cli.parse_args(args=args))
 
-    for (key, val) in values.items():
+    for key, val in values.items():
         assert actual_values[key] == val
 
 
 @pytest.mark.parametrize(
     "args",
     (
         {
@@ -714,15 +721,15 @@
     except Exception:  # pylint: disable=broad-except
         assert False
     home_dir = os.path.expanduser("~")
     cli_config = {}
     with open(f"{home_dir}/.speechmatics/config", "r", encoding="UTF-8") as file:
         cli_config = toml.load(file)
     profile = args.get("profile", "default")
-    for (key, val) in args.items():
+    for key, val in args.items():
         if key != "profile":
             assert cli_config[profile][key] == val
 
     unset_args = {"command": "unset", "profile": profile}
     for key in ["auth_token", "generate_temp_token", "realtime_url", "batch_url"]:
         if key in args:
             unset_args[key] = True
@@ -733,15 +740,15 @@
         cli.config_main(unset_args)
     except Exception:  # pylint: disable=broad-except
         assert False
     home_dir = os.path.expanduser("~")
     with open(f"{home_dir}/.speechmatics/config", "r", encoding="UTF-8") as file:
         cli_config = toml.load(file)
 
-    for (key, val) in args.items():
+    for key, val in args.items():
         if key != "profile":
             assert key not in cli_config[profile]
 
 
 def test_default_urls_connection_config():
     rt_args = {"mode": "rt"}
     settings = cli.get_connection_settings(rt_args, lang="es")
```

### Comparing `speechmatics-python-1.8.2/tests/test_cli_handlers.py` & `speechmatics-python-1.8.3/tests/test_cli_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,14 @@
 def check_printing_handlers(
     mocker,
     capsys,
     transcript,
     expected_transcript_txt,
     speaker_change_token,
 ):
-
     api = mocker.MagicMock()
     api.get_language_pack_info = mocker.MagicMock(return_value={"word_delimiter": " "})
     transcripts = cli.Transcripts(text="", json=[])
 
     cli.add_printing_handlers(
         api, transcripts, speaker_change_token=speaker_change_token
     )
```

### Comparing `speechmatics-python-1.8.2/tests/test_client.py` & `speechmatics-python-1.8.3/tests/test_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from speechmatics.exceptions import ForceEndSession
 from speechmatics.models import (
     ConnectionSettings,
     ServerMessageType,
     ClientMessageType,
     RTSpeakerDiarizationConfig,
     BatchTranscriptionConfig,
+    TranscriptionConfig,
 )
 
 from tests.utils import path_to_test_resource, default_ws_client_setup
 
 
 def test_json_utf8():
     @client.json_utf8
@@ -94,15 +95,15 @@
     with open(path_to_test_resource("ch.wav"), "rb") as audio_stream:
         ws_client.run_synchronously(audio_stream, transcription_config, audio_settings)
     mock_server.wait_for_clean_disconnects()
 
     # Each handler should have been called once for every message
     # received from the server
     server_message_counts = Counter(msg["message"] for msg in mock_server.messages_sent)
-    for (msg_name, count) in server_message_counts.items():
+    for msg_name, count in server_message_counts.items():
         assert msg_name and handlers[msg_name].call_count == count
 
     # The 'all' handler should have been called for every message.
     assert all_handler.call_count == len(mock_server.messages_sent)
 
 
 def test_middlewares_called(mock_server, mocker):
@@ -137,15 +138,15 @@
 
     # Each handler should have been called once for every message
     # sent from the client
     client_message_counts = Counter(
         msg["message"] if isinstance(msg, dict) else "AddAudio"
         for msg in mock_server.messages_received
     )
-    for (msg_name, count) in client_message_counts.items():
+    for msg_name, count in client_message_counts.items():
         assert msg_name and middlewares[msg_name].call_count == count
 
     # The change to the language made by the middleware above
     # should have been received
     assert (
         mock_server.find_start_recognition_message()["transcription_config"]["language"]
         == "ja"
@@ -309,15 +310,17 @@
         yield None  # pylint: disable=unreachable
 
     mock_logger_error_method = MagicMock()
 
     with patch("websockets.connect", mock_connect):
         with patch.object(client.LOGGER, "error", mock_logger_error_method):
             try:
-                ws_client.run_synchronously(MagicMock(), MagicMock(), MagicMock())
+                ws_client.run_synchronously(
+                    MagicMock(), TranscriptionConfig(language="en"), MagicMock()
+                )
             except ConnectionResetError as exc:
                 assert exc is not None
 
 
 @pytest.mark.asyncio
 async def test__buffer_semaphore():
     """Test the WebsocketClient internal BoundedSemaphore."""
@@ -572,14 +575,92 @@
 
         actual_transcript = batch_client.wait_for_completion(
             job_id, transcription_format="txt"
         )
         assert transcript.decode("utf-8") == actual_transcript
 
 
+def test_client_apikey_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "realtime_url": "http://rt-example.com",
+        },
+    )
+    sm_client = client.WebsocketClient("fake_api_key")
+    assert "fake_api_key" == sm_client.connection_settings.auth_token
+    assert "http://rt-example.com" == sm_client.connection_settings.url
+    assert sm_client.connection_settings.generate_temp_token
+
+
+def test_client_empty_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "realtime_url": "http://rt-example.com",
+            "auth_token": "home_token",
+            "generate_temp_token": True,
+        },
+    )
+    sm_client = client.WebsocketClient()
+    assert "http://rt-example.com" == sm_client.connection_settings.url
+    assert "home_token" == sm_client.connection_settings.auth_token
+    assert sm_client.connection_settings.generate_temp_token
+
+
+def test_client_url_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "auth_token": "home_token",
+        },
+    )
+    sm_client = client.WebsocketClient(ConnectionSettings("http://rt-example.com"))
+    assert "home_token" == sm_client.connection_settings.auth_token
+
+
+def test_batch_client_empty_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "batch_url": "http://batch-example.com/v2",
+            "auth_token": "home_token",
+            "generate_temp_token": True,
+        },
+    )
+    with BatchClient() as batch_client:
+        assert "http://batch-example.com/v2" == batch_client.connection_settings.url
+        assert "home_token" == batch_client.connection_settings.auth_token
+        assert batch_client.connection_settings.generate_temp_token
+
+
+def test_batch_client_url_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "auth_token": "home_token",
+        },
+    )
+    with BatchClient() as batch_client:
+        assert "home_token" == batch_client.connection_settings.auth_token
+
+
+def test_batch_client_api_key_constructor(mocker):
+    mocker.patch(
+        "speechmatics.models.read_config_from_home",
+        return_value={
+            "batch_url": "http://batch-example.com/v2",
+        },
+    )
+    with BatchClient("home_token") as batch_client:
+        assert "http://batch-example.com/v2" == batch_client.connection_settings.url
+        assert "home_token" == batch_client.connection_settings.auth_token
+        assert batch_client.connection_settings.generate_temp_token
+
+
 def deepcopy_state(obj):
     """
     Return a deepcopy of the __dict__ (or state) of an object but ignore
     the keys that cause trouble when trying to copy.deepcopy them.
     """
     state = vars(obj)
     state_copy = {}
```

### Comparing `speechmatics-python-1.8.2/tests/test_models.py` & `speechmatics-python-1.8.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `speechmatics-python-1.8.2/tests/utils.py` & `speechmatics-python-1.8.3/tests/utils.py`

 * *Files identical despite different names*


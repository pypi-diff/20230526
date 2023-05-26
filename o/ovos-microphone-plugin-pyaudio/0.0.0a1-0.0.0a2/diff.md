# Comparing `tmp/ovos-microphone-plugin-pyaudio-0.0.0a1.tar.gz` & `tmp/ovos-microphone-plugin-pyaudio-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-microphone-plugin-pyaudio-0.0.0a1.tar", last modified: Wed May 17 19:44:45 2023, max compression
+gzip compressed data, was "ovos-microphone-plugin-pyaudio-0.0.0a2.tar", last modified: Fri May 26 19:03:01 2023, max compression
```

## Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1.tar` & `ovos-microphone-plugin-pyaudio-0.0.0a2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:45.443364 ovos-microphone-plugin-pyaudio-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-17 19:44:39.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 19:44:39.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 19:44:45.443364 ovos-microphone-plugin-pyaudio-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 19:44:39.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:45.443364 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio/
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-17 19:44:39.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 19:44:41.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:44:45.443364 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:44:45.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:44:45.443364 ovos-microphone-plugin-pyaudio-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-17 19:44:39.000000 ovos-microphone-plugin-pyaudio-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:03:01.598935 ovos-microphone-plugin-pyaudio-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-26 19:02:53.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 19:02:53.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 19:03:01.598935 ovos-microphone-plugin-pyaudio-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 19:02:53.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:03:01.598935 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-26 19:02:53.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 19:02:56.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:03:01.598935 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:03:01.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:03:01.598935 ovos-microphone-plugin-pyaudio-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3148 2023-05-26 19:02:53.000000 ovos-microphone-plugin-pyaudio-0.0.0a2/setup.py
```

### Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1/LICENSE` & `ovos-microphone-plugin-pyaudio-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1/PKG-INFO` & `ovos-microphone-plugin-pyaudio-0.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-pyaudio
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A pyaudio microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-pyaudio
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone pyaudio
```

### Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio/__init__.py` & `ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 from threading import Thread
 from typing import Optional
 
 import pyaudio
 from ovos_plugin_manager.templates.microphone import Microphone
 from ovos_utils.log import LOG
 from speech_recognition import Microphone as _Mic
+from ovos_config import Configuration
 
 
 @dataclass
 class PyAudioMicrophone(Microphone):
-    device: str = "default"
+    device: str = Configuration().get("listener", {}).get("device") or "default"
     period_size: int = 1024
     timeout: float = 5.0
     multiplier: float = 1.0
     full_chunk = bytes()
     _thread: Optional[Thread] = None
     _queue: "Queue[Optional[bytes]]" = field(default_factory=Queue)
     _is_running: bool = False
```

### Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1/ovos_microphone_plugin_pyaudio.egg-info/PKG-INFO` & `ovos-microphone-plugin-pyaudio-0.0.0a2/ovos_microphone_plugin_pyaudio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-pyaudio
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A pyaudio microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-pyaudio
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone pyaudio
```

### Comparing `ovos-microphone-plugin-pyaudio-0.0.0a1/setup.py` & `ovos-microphone-plugin-pyaudio-0.0.0a2/setup.py`

 * *Files identical despite different names*


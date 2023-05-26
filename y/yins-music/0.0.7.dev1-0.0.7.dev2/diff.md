# Comparing `tmp/yins-music-0.0.7.dev1.tar.gz` & `tmp/yins-music-0.0.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yins-music-0.0.7.dev1.tar", last modified: Fri May 26 01:48:30 2023, max compression
+gzip compressed data, was "yins-music-0.0.7.dev2.tar", last modified: Fri May 26 05:43:06 2023, max compression
```

## Comparing `yins-music-0.0.7.dev1.tar` & `yins-music-0.0.7.dev2.tar`

### file list

```diff
@@ -1,13 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/yins_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/group_call_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/group_call_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/implementation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/base_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_discarded_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_participant_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/update_group_call_participants_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/update_group_call_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/fipper_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/telethon_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto_client_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/yins_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/top_level.txt
```

### Comparing `yins-music-0.0.7.dev1/LICENSE` & `yins-music-0.0.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.7.dev1/PKG-INFO` & `yins-music-0.0.7.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.7.dev1
+Version: 0.0.7.dev2
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev1 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev2 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.7.dev1/README.md` & `yins-music-0.0.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `yins-music-0.0.7.dev1/setup.py` & `yins-music-0.0.7.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import re
 
 from setuptools import setup, find_packages
 
 base_path = path.abspath(path.dirname(__file__))
 packages = find_packages()
 
-with open(path.join(base_path, 'pytgcalls/pytgcalls/__init__.py'), encoding='utf-8') as f:
+with open(path.join(base_path, 'pytgcalls/__init__.py'), encoding='utf-8') as f:
     version = re.findall(r"__version__ = '(.+)'", f.read())[0]
 
 with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='yins-music',
```

### Comparing `yins-music-0.0.7.dev1/yins_music.egg-info/PKG-INFO` & `yins-music-0.0.7.dev2/yins_music.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yins-music
-Version: 0.0.7.dev1
+Version: 0.0.7.dev2
 Summary: a library connecting the tgcalls Python binding with MTProto
 Home-page: https://github.com/MarshalX/tgcalls
 Author: AyiinXd
 Author-email: ayiinxd0307@gmail.com
 License: LGPLv3
 Project-URL: Documentation, https://tgcalls.org/
 Project-URL: Telegram Channel, https://t.me/tgcallslib
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev1 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev2 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```


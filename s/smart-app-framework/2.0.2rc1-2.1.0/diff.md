# Comparing `tmp/smart_app_framework-2.0.2rc1-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 306562 bytes, number of entries: 334
+Zip file size: 306540 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -326,11 +326,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10830 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.2rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.0.2rc1.dist-info/RECORD
-334 files, 985923 bytes uncompressed, 253780 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10819 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32366 b- defN 16-Jan-01 00:00 smart_app_framework-2.1.0.dist-info/RECORD
+334 files, 985903 bytes uncompressed, 253776 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -987,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.0.2rc1.dist-info/METADATA
+Filename: smart_app_framework-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.0.2rc1.dist-info/WHEEL
+Filename: smart_app_framework-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.0.2rc1.dist-info/RECORD
+Filename: smart_app_framework-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `smart_app_framework-2.0.2rc1.dist-info/METADATA` & `smart_app_framework-2.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.0.2rc1
+Version: 2.1.0
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: Jinja2 (==3.0.3)
 Requires-Dist: PyYAML (==5.3)
 Requires-Dist: Twisted (==22.8.0)
 Requires-Dist: aiohttp (==3.8.4)
 Requires-Dist: boto (==2.49.0)
 Requires-Dist: cachetools (==5.3.0)
 Requires-Dist: confluent_kafka (==1.9.2) ; python_version < "3.11"
-Requires-Dist: confluent_kafka (==2.0.2) ; python_full_version >= "3.11.0" and python_full_version < "3.12.0"
+Requires-Dist: confluent_kafka (==2.0.2) ; python_version >= "3.11.dev0" and python_version < "3.12.dev0"
 Requires-Dist: croniter (==1.3.7)
 Requires-Dist: dill (==0.3.6)
 Requires-Dist: freezegun (==1.1.0)
 Requires-Dist: ics (==0.6)
 Requires-Dist: incremental (==21.3.0)
 Requires-Dist: keras (==2.12.0) ; extra == "ml"
 Requires-Dist: lxml (==4.9.2)
@@ -37,15 +37,15 @@
 Requires-Dist: pymorphy2 (==0.8)
 Requires-Dist: pymorphy2_dicts (==2.4.393442.3710985)
 Requires-Dist: python-dateutil (==2.7.3)
 Requires-Dist: python-json-logger (==0.1.11)
 Requires-Dist: requests (==2.22.0)
 Requires-Dist: rusenttokenize (==0.0.5)
 Requires-Dist: scikit-learn (==1.1.2) ; (python_version < "3.11") and (extra == "ml")
-Requires-Dist: scikit-learn (==1.2.0) ; (python_full_version >= "3.11.0" and python_full_version < "3.12.0") and (extra == "ml")
+Requires-Dist: scikit-learn (==1.2.0) ; (python_version >= "3.11.dev0" and python_version < "3.12.dev0") and (extra == "ml")
 Requires-Dist: setuptools (==62.3.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tensorflow (==2.12.0) ; (sys_platform == "darwin" and platform_machine == "x86_64") and (extra == "ml")
 Requires-Dist: tensorflow (==2.12.0) ; (sys_platform == "linux" and platform_machine == "x86_64") and (extra == "ml")
 Requires-Dist: tensorflow-aarch64 (==2.12.0) ; (sys_platform == "linux" and platform_machine == "aarch64") and (extra == "ml")
 Requires-Dist: tensorflow-macos (==2.12.0) ; (sys_platform == "darwin" and platform_machine == "arm64") and (extra == "ml")
 Requires-Dist: timeout-decorator (==0.4.1)
```

## Comparing `smart_app_framework-2.0.2rc1.dist-info/RECORD` & `smart_app_framework-2.1.0.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -325,10 +325,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=bC7tdYW480irANhxaFxiKgnAsvmz-luf52WSu7ZjnIU,3385
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.0.2rc1.dist-info/METADATA,sha256=BygaYqSx6kjHhjJTwmJLBenxnvARzfMAxvZyN3_XwdA,10830
-smart_app_framework-2.0.2rc1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-smart_app_framework-2.0.2rc1.dist-info/RECORD,,
+smart_app_framework-2.1.0.dist-info/METADATA,sha256=fnCTVaNZ8FX0HB1KM8-OvK6qd1Yn-BfTSrwgDs0PL4o,10819
+smart_app_framework-2.1.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+smart_app_framework-2.1.0.dist-info/RECORD,,
```


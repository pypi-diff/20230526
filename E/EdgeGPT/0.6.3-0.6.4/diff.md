# Comparing `tmp/EdgeGPT-0.6.3.tar.gz` & `tmp/EdgeGPT-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.6.3.tar", last modified: Wed May 24 16:31:19 2023, max compression
+gzip compressed data, was "EdgeGPT-0.6.4.tar", last modified: Thu May 25 12:55:38 2023, max compression
```

## Comparing `EdgeGPT-0.6.3.tar` & `EdgeGPT-0.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:31:19.596595 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 16:31:19.000000 EdgeGPT-0.6.3/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-24 16:30:49.000000 EdgeGPT-0.6.3/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:55:38.281982 EdgeGPT-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 12:55:05.000000 EdgeGPT-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-25 12:55:38.281982 EdgeGPT-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 12:55:38.281982 EdgeGPT-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-25 12:55:05.000000 EdgeGPT-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:55:38.281982 EdgeGPT-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:55:38.281982 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 12:55:38.000000 EdgeGPT-0.6.4/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38046 2023-05-25 12:55:05.000000 EdgeGPT-0.6.4/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 12:55:05.000000 EdgeGPT-0.6.4/src/ImageGen.py
```

### Comparing `EdgeGPT-0.6.3/LICENSE` & `EdgeGPT-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.3/PKG-INFO` & `EdgeGPT-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.3
+Version: 0.6.4
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.3 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.4 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.3/README.md` & `EdgeGPT-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.6.3/setup.py` & `EdgeGPT-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.6.3",
+    version="0.6.4",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.6.3/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.6.4/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.6.3
+Version: 0.6.4
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.3 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.6.4 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.6.3/src/EdgeGPT.py` & `EdgeGPT-0.6.4/src/EdgeGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,15 +505,15 @@
         await self.wss.send_str(_append_identifier(self.request.struct))
         final = False
         draw = False
         resp_txt = ""
         result_text = ""
         resp_txt_no_link = ""
         while not final:
-            msg = await self.wss.receive()
+            msg = await self.wss.receive(timeout=10)
             objects = msg.data.split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
@@ -588,15 +588,15 @@
                         )
                     final = True
                     await self.close()
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send_str(_append_identifier({"protocol": "json", "version": 1}))
-        await self.wss.receive()
+        await self.wss.receive(timeout=10)
 
     async def close(self) -> None:
         """
         Close the connection
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
@@ -692,15 +692,15 @@
 
     async def reset(self) -> None:
         """
         Reset the conversation
         """
         await self.close()
         self.chat_hub = _ChatHub(
-            await _Conversation.create(self.proxy),
+            await _Conversation.create(self.proxy, cookies=self.chat_hub.cookies),
             proxy=self.proxy,
             cookies=self.chat_hub.cookies,
         )
 
 
 async def _get_input_async(
     session: PromptSession = None,
```


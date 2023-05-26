# Comparing `tmp/toui-2.4.1.tar.gz` & `tmp/toui-2.4.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.4.1.tar", last modified: Tue May 23 17:58:46 2023, max compression
+gzip compressed data, was "toui-2.4.2b0.tar", last modified: Fri May 26 03:55:20 2023, max compression
```

## Comparing `toui-2.4.1.tar` & `toui-2.4.2b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.531751 toui-2.4.1/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.1/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-23 17:58:46.531751 toui-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.464317 toui-2.4.1/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.1/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.1/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.1/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.472786 toui-2.4.1/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.1/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-23 17:58:46.531751 toui-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.514953 toui-2.4.1/toui/
--rw-rw-rw-   0        0        0      266 2023-05-23 16:57:01.000000 toui-2.4.1/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.1/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.4.1/toui/_helpers.py
--rw-rw-rw-   0        0        0    10611 2023-05-23 15:20:04.000000 toui-2.4.1/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6452 2023-05-23 15:20:31.000000 toui-2.4.1/toui/_signals.py
--rw-rw-rw-   0        0        0    30744 2023-05-23 16:55:16.000000 toui-2.4.1/toui/apps.py
--rw-rw-rw-   0        0        0    22886 2023-05-23 15:17:02.000000 toui-2.4.1/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.1/toui/exceptions.py
--rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.1/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.1/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:58:46.531751 toui-2.4.1/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 17:58:46.000000 toui-2.4.1/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.516293 toui-2.4.2b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.4.2b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.4.2b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3235 2023-05-26 03:55:20.515293 toui-2.4.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2860 2023-05-24 15:31:01.000000 toui-2.4.2b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.258611 toui-2.4.2b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.4.2b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.263611 toui-2.4.2b0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.4.2b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-26 03:55:20.516293 toui-2.4.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-23 17:57:05.000000 toui-2.4.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.494293 toui-2.4.2b0/toui/
+-rw-rw-rw-   0        0        0      271 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-23 15:00:55.000000 toui-2.4.2b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10863 2023-05-26 03:45:07.000000 toui-2.4.2b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2023-05-26 03:42:45.000000 toui-2.4.2b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    31491 2023-05-26 03:32:16.000000 toui-2.4.2b0/toui/apps.py
+-rw-rw-rw-   0        0        0    22886 2023-05-24 15:46:55.000000 toui-2.4.2b0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.4.2b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    18047 2023-05-23 16:30:18.000000 toui-2.4.2b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.4.2b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:55:20.513292 toui-2.4.2b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3235 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-26 03:55:20.000000 toui-2.4.2b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-26 03:55:19.000000 toui-2.4.2b0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.4.1/LICENSE` & `toui-2.4.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/PKG-INFO` & `toui-2.4.2b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.4.1
+Version: 2.4.2b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![ToUI Image](images/logo.png)
 
+![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
+![Latest version](https://img.shields.io/pypi/v/toui)
+![Docs](https://img.shields.io/readthedocs/toui)
+
 # Overview
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
```

### Comparing `toui-2.4.1/README.md` & `toui-2.4.2b0/toui.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+Metadata-Version: 2.1
+Name: toui
+Version: 2.4.2b0
+Summary: Creates user interfaces (websites and desktop apps) from HTML easily
+Author: Mubarak Almehairbi
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![ToUI Image](images/logo.png)
 
+![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
+![Latest version](https://img.shields.io/pypi/v/toui)
+![Docs](https://img.shields.io/readthedocs/toui)
+
 # Overview
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
```

### Comparing `toui-2.4.1/examples/advanced_example_1_toui_blueprint.py` & `toui-2.4.2b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/examples/example_1_simple_website.py` & `toui-2.4.2b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/examples/example_2_simple_desktop_app.py` & `toui-2.4.2b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/examples/example_3_updating_page.py` & `toui-2.4.2b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/examples/example_4_function_with_arg.py` & `toui-2.4.2b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/examples/example_5_user_variables.py` & `toui-2.4.2b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/images/logo.png` & `toui-2.4.2b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/setup.py` & `toui-2.4.2b0/setup.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/toui/_helpers.py` & `toui-2.4.2b0/toui/_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,8 +51,14 @@
 def obj_converter(obj):
     if obj is True:
         return 'true'
     if obj is False:
         return 'false'
     if obj is None:
         return 'null'
-    return obj
+    return obj
+
+def show_debug(bool=True):
+    if bool:
+        logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(logging.INFO)
```

### Comparing `toui-2.4.1/toui/_javascript_templates.py` & `toui-2.4.2b0/toui/_javascript_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 const newKey = parseInt(lastKey) + 1
             }
             _touiFiles[newKey.toString()] = file
             fileJSON['file-id'] = newKey.toString()
             files.push(fileJSON)
         }
     }
-    var jsonString = JSON.stringify({data: files, type: "files"})
+    var jsonString = JSON.stringify({data: files, type: "files", "msg-num": kwargs["msg-num"]})
     var dataSent = _send(jsonString)
     return dataSent
 }
 
 async function _saveFile(kwargs) {
     var fileId = kwargs['file-id']
     var file = _touiFiles[fileId]
@@ -160,35 +160,37 @@
             const content = new Uint8Array(buffer)
             const lengthPerPart = 16000
             const charsLength = content.length
             for (var i = 0; i < charsLength; i += lengthPerPart) {
                 var smallerContent = [...content.slice(i, i + lengthPerPart)]
                 var jsonString = JSON.stringify({type: "save files",
                                                   data: smallerContent,
-                                                  end: false})
+                                                  end: false,
+                                                  "msg-num": kwargs["msg-num"]})
                 var dataSent = _send(jsonString)
             }
-            var jsonString = JSON.stringify({type: "save files", data: [],
+            var jsonString = JSON.stringify({type: "save files", data: [], "msg-num": kwargs["msg-num"],
                                               end: true})
             var dataSent = _send(jsonString)
         }
         reader.readAsArrayBuffer(file)
     } else {
         reader.onload = function () {
             const content = reader.result
             const lengthPerPart = 16000
             const charsLength = content.length
             for (var i = 0; i < charsLength; i += lengthPerPart) {
                 var smallerContent = content.substring(i, i + lengthPerPart)
                 var jsonString = JSON.stringify({type: "save files",
                                                   data: smallerContent,
+                                                  "msg-num": kwargs["msg-num"],
                                                   end: false})
                 var dataSent = _send(jsonString)
             }
-            var jsonString = JSON.stringify({type: "save files", data: "",
+            var jsonString = JSON.stringify({type: "save files", data: "", "msg-num": kwargs["msg-num"],
                                               end: true})
             var dataSent = _send(jsonString)
         }
         reader.readAsText(file)
     }
 }
```

### Comparing `toui-2.4.1/toui/_signals.py` & `toui-2.4.2b0/toui/_signals.py`

 * *Files 21% similar despite different names*

```diff
@@ -54,24 +54,42 @@
                 signal = method(**kwargs)
                 if signal:
                     return self._send(signal)
                 else:
                     return
 
     def _send(self, signal):
+        msg_num = self.ws.msg_num = self.ws.msg_num + 1
+        signal['kwargs']['msg-num'] = msg_num
         self.ws.send(json.dumps(signal))
         debug(f"SENT: {signal}")
         if self.return_type == "js":
-            data_from_js = self.ws.receive()
-            debug(f"DATA RECEIVED")
-            data_validation = self.object._app._validate_data(data_from_js)
-            if not data_validation:
-                info("Data validation returns `False`. The data will not be used.")
-                return
-            data_dict = json.loads(data_from_js)
+            valid_message = False
+            while not valid_message:
+                data_from_js = self.ws.receive()
+                debug(f"DATA RECEIVED")
+                data_validation = self.object._app._validate_data(data_from_js)
+                if not data_validation:
+                    info("Data validation returns `False`. The data will not be used.")
+                    return
+                data_dict = json.loads(data_from_js)
+                if data_dict.get("msg-num") == msg_num:
+                    valid_message = True
+                else:
+                    if data_dict.get("type") == "page":
+                        debug("Adding to pending pages")
+                        self.ws.pending_pages.append(data_dict)
+                    else:
+                        self.ws.pending_messages[data_dict.get("msg-num")] = data_dict
+                    debug(f"Non-matching message number: {data_dict.get('msg-num')}, checking for other messages..")
+                    if msg_num in self.ws.pending_messages:
+                        data_dict = self.ws.pending_messages.pop(msg_num)
+                        valid_message = True
+                debug("Could not find message number")
+            debug(f"Message number: {msg_num} found")
             debug(f"RECEIVED DATA KEYS: {list(data_dict.keys())}")
             if data_dict['type'] == "files":
                 files = []
                 for file_dict in data_dict['data']:
                     files.append(File(file_dict, signal, self.object._app, file_dict['file-id'], ws=self.ws))
                 return files
             return data_dict['data']
@@ -129,32 +147,58 @@
     def __iter__(self):
         js_func = "_saveFile"
         js_args = []
         js_kwargs = {}
         js_kwargs['file-id'] = self._id
         js_kwargs['binary'] = self.is_binary
         signal = {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
+
+        msg_num = self._ws.msg_num = self._ws.msg_num + 1
+        signal['kwargs']['msg-num'] = msg_num
         self._ws.send(json.dumps(signal))
         debug(f"SENT: {signal}")
         while True:
-            data_from_js = self._ws.receive()
-            data_validation = self._app._validate_data(data_from_js)
-            if not data_validation:
-                info("Data validation returns `False`. The data will not be used.")
-                return
-            data_dict = json.loads(data_from_js)
+            data_dict = self._get_valid_message(msg_num)
+            if data_dict is None:
+                break
             data = data_dict['data']
             if self.is_binary:
                 data = bytearray(data)
             yield data
             if data_dict['end'] == True:
                 break
 
     def __repr__(self):
         return f"<File {self.name}>"
+    
+    def _get_valid_message(self, msg_num):
+        valid_message = False
+        data_dict = None
+        while not valid_message:
+            data_from_js = self._ws.receive()
+            debug(f"DATA RECEIVED")
+            data_validation = self._app._validate_data(data_from_js)
+            if not data_validation:
+                info("Data validation returns `False`. The data will not be used.")
+                return
+            data_dict = json.loads(data_from_js)
+            if data_dict.get("msg-num") == msg_num:
+                valid_message = True
+            else:
+                if data_dict.get("type") == "page":
+                    debug("Adding to pending pages")
+                    self._ws.pending_pages.append(data_dict)
+                else:
+                    self._ws.pending_messages[data_dict.get("msg-num")] = data_dict
+                debug(f"Non-matching message number: {data_dict.get('msg-num')}, checking for other messages..")
+                if msg_num in self._ws.pending_messages:
+                    data_dict = self._ws.pending_messages.pop(msg_num)
+                    valid_message = True
+        debug(f"Message number: {msg_num} found")
+        return data_dict
 
     def save(self, stream):
         """
         Saves the contents of the file to a stream.
 
         Parameters
         ----------
```

### Comparing `toui-2.4.1/toui/apps.py` & `toui-2.4.2b0/toui/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,51 +617,65 @@
     def _communicate(self, ws):
         """This is a private function."""
         validation = self._validate_ws(ws)
         if not validation:
             info("WebSocket validation returns `False`. No data should be sent or received.")
             return
         info(f'WebSocket connected: {ws.connected}')
+        ws.msg_num = 0
+        ws.pending_messages = {}
+        ws.pending_pages = []
         while True:
-            data_from_js = ws.receive()
-            data_validation = self._validate_data(data_from_js)
-            if not data_validation:
-                info("Data validation returns `False`. The data will not be used.")
-                continue
-            s = time.time()
-            self._session_check()
-            data_dict = json.loads(data_from_js)
-            func = data_dict['func']
-            args = data_dict['args']
-            url = data_dict['url']
-            new_html = data_dict['html']
-            new_page = Page(url=url)
-            new_page.from_str(new_html)
-            new_page._app = self
-            new_page._signal_mode = True
-            new_page._ws = ws
-            new_page._inherit_functions()
-            selector_to_element = data_dict['selector-to-element']
-            if selector_to_element:
-                for index, arg in enumerate(args):
-                    if type(arg) is dict:
-                        if arg.get('type') == "element":
-                            args[index] = new_page.get_element_from_selector(arg['selector'])
-            if "uid" in data_dict:
-                new_page._uid = data_dict['uid']
-            session['user page'] = new_page
-            try:
-                if new_page._func_exists(func):
-                    new_page._call_func(func, *args)
-                del session['user page']
-            except Exception as e:
-                del session['user page']
-                raise e
-            e = time.time()
-            debug(f"TIME: {e - s}s")
+            valid_message = False
+            while not valid_message:
+                data_from_js = ws.receive()
+                data_validation = self._validate_data(data_from_js)
+                if not data_validation:
+                    info("Data validation returns `False`. The data will not be used.")
+                    continue
+                s = time.time()
+                data_dict = json.loads(data_from_js)
+                if data_dict.get("type") == "page":
+                    ws.pending_pages.append(data_dict)
+                    valid_message = True
+            while True:
+                debug(f"Pages Before: {len(ws.pending_pages)}")
+                if len(ws.pending_pages) == 0:
+                    break
+                data_dict = ws.pending_pages.pop(0)
+                debug(f"Pages After: {len(ws.pending_pages)}")
+                self._session_check()
+                func = data_dict['func']
+                args = data_dict['args']
+                url = data_dict['url']
+                new_html = data_dict['html']
+                new_page = Page(url=url)
+                new_page.from_str(new_html)
+                new_page._app = self
+                new_page._signal_mode = True
+                new_page._ws = ws
+                new_page._inherit_functions()
+                selector_to_element = data_dict['selector-to-element']
+                if selector_to_element:
+                    for index, arg in enumerate(args):
+                        if type(arg) is dict:
+                            if arg.get('type') == "element":
+                                args[index] = new_page.get_element_from_selector(arg['selector'])
+                if "uid" in data_dict:
+                    new_page._uid = data_dict['uid']
+                session['user page'] = new_page
+                try:
+                    if new_page._func_exists(func):
+                        new_page._call_func(func, *args)
+                    del session['user page']
+                except Exception as e:
+                    del session['user page']
+                    raise e
+                e = time.time()
+                debug(f"TIME: {e - s}s")
 
     def _confirm_user_database_created(self):
         if self._user_cls is None:
             raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database`.")
 
     def _load_user(self, user_id):
         return self._user_cls.query.filter_by(id=int(user_id)).first()
@@ -944,15 +958,15 @@
     >>> app = get_global_app()
 
     """
     global _global_app
     _global_app = app
 
 
-def get_global_app():
+def get_global_app() -> _App:
     """
     Gets the shared app object.
 
     See :py:meth:`set_global_app`.
     """
     return _global_app
```

### Comparing `toui-2.4.1/toui/elements.py` & `toui-2.4.2b0/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/toui/pages.py` & `toui-2.4.2b0/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/toui/structure.py` & `toui-2.4.2b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.4.1/toui.egg-info/PKG-INFO` & `toui-2.4.2b0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-Metadata-Version: 2.1
-Name: toui
-Version: 2.4.1
-Summary: Creates user interfaces (websites and desktop apps) from HTML easily
-Author: Mubarak Almehairbi
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![ToUI Image](images/logo.png)
 
+![License](https://img.shields.io/github/license/mubarakalmehairbi/ToUI)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/toui)
+![Latest version](https://img.shields.io/pypi/v/toui)
+![Docs](https://img.shields.io/readthedocs/toui)
+
 # Overview
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
```

### Comparing `toui-2.4.1/toui.egg-info/SOURCES.txt` & `toui-2.4.2b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*


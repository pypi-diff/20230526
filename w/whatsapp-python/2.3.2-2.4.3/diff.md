# Comparing `tmp/whatsapp-python-2.3.2.tar.gz` & `tmp/whatsapp-python-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-python-2.3.2.tar", last modified: Sun Apr 30 08:30:20 2023, max compression
+gzip compressed data, was "whatsapp-python-2.4.3.tar", last modified: Fri May 26 16:32:05 2023, max compression
```

## Comparing `whatsapp-python-2.3.2.tar` & `whatsapp-python-2.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/whatsapp/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-04-30 08:30:19.000000 whatsapp-python-2.3.2/whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:30:20.913652 whatsapp-python-2.3.2/whatsapp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 08:30:20.000000 whatsapp-python-2.3.2/whatsapp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-05-26 16:32:04.000000 whatsapp-python-2.4.3/whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:32:05.630838 whatsapp-python-2.4.3/whatsapp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 16:32:05.000000 whatsapp-python-2.4.3/whatsapp_python.egg-info/top_level.txt
```

### Comparing `whatsapp-python-2.3.2/LICENSE` & `whatsapp-python-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-python-2.3.2/PKG-INFO` & `whatsapp-python-2.4.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.3.2
+Version: 2.4.3
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -23,48 +23,57 @@
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
-Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
+Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
+
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
 ## Supported features
 
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
 
-## Switching from `Neurotech-HQ/heyoo`
-Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+## Documentation
+
+The documentation for the is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
+
+## Costs of the API
 
+While using third-party API providers of the WhatsApp API may have some monthly fees, using the WhatsApp API provided directly by Facebook is way cheaper. 
+The first 1000 chats created are free, then there is a pay-as-you-go fee that is paid for each conversation started.
+
+All the prices are available in the [**WhatsApp API docs**](https://developers.facebook.com/docs/whatsapp/pricing)
+
+## Switching from `Neurotech-HQ/heyoo`
+Any version >1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+Any version <=1.1.2 is fully compatible with the original `heyoo` library and doesn't include any breaking change.
 You can ignore this warning if it's your first time using the library.
 
 
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
-Note: docs for version 1.1.2 are available in the [wiki dedicated page](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
+Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
 
 
-## Documentation
-
-The documentation for the is available in the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
 
 
 ## Issues
 
-If you are facing any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/filipporomani/whatsapp/issues)
+If you are facing any issues or have any questions, please open an issue on the [**GitHub repository**](https://github.com/filipporomani/whatsapp/issues)
 
 ## Contributing
 
-This is an opensource project published under the ```MIT License```. Please refer to the [LICENSE](LICENSE) file.
+This is an opensource project published under the ```MIT License```: [**LICENSE**](LICENSE).
 
 ## References
 
 1. [WhatsApp Cloud API official documentation](https://developers.facebook.com/docs/whatsapp/cloud-api/)
```

### Comparing `whatsapp-python-2.3.2/setup.py` & `whatsapp-python-2.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="whatsapp-python",
-    version="2.3.2",
+    version="2.4.3",
     description="Opensource Python wrapper to WhatsApp Cloud API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/filipporomani/whatsapp",
     author="Filippo Romani",
     author_email="mail@filipporomani.it",
     license="MIT",
```

### Comparing `whatsapp-python-2.3.2/whatsapp/__init__.py` & `whatsapp-python-2.4.3/whatsapp/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Unofficial Python wrapper for the WhatsApp Cloud API.
 """
 from __future__ import annotations
 
 import requests
 from json import dumps
 import logging
+from flask import Flask, request, Response
+
 
 # Setup logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 class WhatsApp(object):
     """ "
@@ -23,15 +25,15 @@
         Args:
             token[str]: Token for the WhatsApp cloud API obtained from the Facebook developer portal
             phone_number_id[str]: Phone number id for the WhatsApp cloud API obtained from the developer portal
             logger[bool]: Whether to enable logging or not (default: True)
         """
 
         # Check if the version is up to date
-        self.VERSION = "2.3.3"
+        self.VERSION = "2.4.3"
         latest = str(requests.get(
             "https://pypi.org/pypi/whatsapp-python/json").json()["info"]["version"])
         if self.VERSION != latest:
             version_int = int(self.VERSION.replace(".", ""))
             latest_int = int(latest.replace(".", ""))
             # this is to avoid the case where the version is 1.0.10 and the latest is 1.0.2 (possible if user is using the github version)
             if version_int < latest_int:
@@ -158,8 +160,49 @@
             except:
                 pass
 
         self.instance = instance
         self.url = self.instance.url
         self.headers = self.instance.headers
 
-    from ext._message import send, reply, mark_as_read
+    from ext._message import send, reply, mark_as_read
+
+
+
+
+class Hook(object):
+
+    def __init__(self, instance: WhatsApp = None, host: str = "localhost", port: int = 8080, verify_token: str = "", handler: function = None):
+        self.instance = instance
+        self.host = host
+        self.port = port
+        self.token = verify_token
+        self.app = Flask(__name__)
+        self.handler = handler
+    
+        @self.app.get("/")
+        def verify_token():
+            if request.args.get("hub.verify_token") == self.token:
+                logging.info("Verified webhook")
+                challenge = request.args.get("hub.challenge")
+                return str(challenge)
+            logging.error("Webhook Verification failed")
+            return "Invalid verification token"
+
+
+        @self.app.post("/")
+        def hook():
+            # Handle Webhook Subscriptions
+            data = request.get_json()
+            if data is None:
+                return Response(status=200)
+            logging.info("Received webhook data: %s", data)
+            changed_field = self.instance.changed_field(data)
+            if changed_field == "messages":
+                new_message = self.instance.is_message(data)
+                if new_message:
+                    msg = Message(instance=self.instance, data=data)
+                    self.handler(msg)
+            return "OK", 200
+
+    def run(self):
+        self.app.run(host=self.host, port=self.port)
```

### Comparing `whatsapp-python-2.3.2/whatsapp_python.egg-info/PKG-INFO` & `whatsapp-python-2.4.3/whatsapp_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-python
-Version: 2.3.2
+Version: 2.4.3
 Summary: Opensource Python wrapper to WhatsApp Cloud API
 Home-page: https://github.com/filipporomani/whatsapp
 Author: Filippo Romani
 Author-email: mail@filipporomani.it
 License: MIT
 Keywords: whatsapp,whatsapp-libary,WhatsApp Cloud API Wrapper,PyWhatsApp,WhatsApp API in Python
 Classifier: Development Status :: 4 - Beta
@@ -23,48 +23,57 @@
 # [whatsapp-python](https://pypi.org/project/whatsapp-python/)
 
 ![Made in Italy](https://img.shields.io/badge/made%20in-italy-008751.svg?style=flat-square)
 [![Downloads](https://pepy.tech/badge/whatsapp-python)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/month)](https://pepy.tech/project/whatsapp-python)
 [![Downloads](https://pepy.tech/badge/whatsapp-python/week)](https://pepy.tech/project/whatsapp-python)
 
-Unofficial Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api)
+Free, open-source Python wrapper for the [WhatsApp Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api).
+
 Forked from [Neurotech-HQ/heyoo](https://github.com/Neurotech-HQ/heyoo)
 
 ## Supported features
 
 1. Sending messages
 2. Marking messages as read
 3. Sending Media (images, audio, video and documents)
 4. Sending location
 5. Sending interactive buttons
 6. Sending template messages
 7. Parsing messages and media received
 
-## Switching from `Neurotech-HQ/heyoo`
-Any version newer than 1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+## Documentation
+
+The documentation for the is available in the [**wiki**](https://github.com/filipporomani/whatsapp/wiki)
+
+## Costs of the API
 
+While using third-party API providers of the WhatsApp API may have some monthly fees, using the WhatsApp API provided directly by Facebook is way cheaper. 
+The first 1000 chats created are free, then there is a pay-as-you-go fee that is paid for each conversation started.
+
+All the prices are available in the [**WhatsApp API docs**](https://developers.facebook.com/docs/whatsapp/pricing)
+
+## Switching from `Neurotech-HQ/heyoo`
+Any version >1.1.2 is incompatible with the original `heyoo` library! Be careful updating! Read the docs first!
+Any version <=1.1.2 is fully compatible with the original `heyoo` library and doesn't include any breaking change.
 You can ignore this warning if it's your first time using the library.
 
 
 Switching from heyoo to whatsapp-python doesn't require any change for versions up to 1.1.2: just uninstall the old, install the new and change the import name from `heyoo` to `whatsapp`.
 For version which are GREATER THEN 1.1.2, messages have became objects, so you need to change your code to use the new methods.
 
-Note: docs for version 1.1.2 are available in the [wiki dedicated page](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
+Note: docs for version 1.1.2 are available in the [**dedicated wiki page**](https://github.com/filipporomani/whatsapp/wiki/v1.1.2)
 
 
-## Documentation
-
-The documentation for the is available in the [wiki section](https://github.com/filipporomani/whatsapp/wiki)
 
 
 ## Issues
 
-If you are facing any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/filipporomani/whatsapp/issues)
+If you are facing any issues or have any questions, please open an issue on the [**GitHub repository**](https://github.com/filipporomani/whatsapp/issues)
 
 ## Contributing
 
-This is an opensource project published under the ```MIT License```. Please refer to the [LICENSE](LICENSE) file.
+This is an opensource project published under the ```MIT License```: [**LICENSE**](LICENSE).
 
 ## References
 
 1. [WhatsApp Cloud API official documentation](https://developers.facebook.com/docs/whatsapp/cloud-api/)
```


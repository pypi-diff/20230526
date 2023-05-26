# Comparing `tmp/GoogleBard-1.1.1.tar.gz` & `tmp/GoogleBard-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-1.1.1.tar", last modified: Thu May 25 07:04:25 2023, max compression
+gzip compressed data, was "GoogleBard-1.1.2.tar", last modified: Fri May 26 00:41:21 2023, max compression
```

## Comparing `GoogleBard-1.1.1.tar` & `GoogleBard-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:25.224626 GoogleBard-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 07:03:58.000000 GoogleBard-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-25 07:04:25.224626 GoogleBard-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 07:03:58.000000 GoogleBard-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:04:25.224626 GoogleBard-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 07:03:58.000000 GoogleBard-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:25.224626 GoogleBard-1.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-05-25 07:03:58.000000 GoogleBard-1.1.1/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:04:25.224626 GoogleBard-1.1.1/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-25 07:04:25.000000 GoogleBard-1.1.1/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 07:04:25.000000 GoogleBard-1.1.1/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:04:25.000000 GoogleBard-1.1.1/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 07:04:25.000000 GoogleBard-1.1.1/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 07:04:25.000000 GoogleBard-1.1.1/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-26 00:40:53.000000 GoogleBard-1.1.2/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:41:21.049971 GoogleBard-1.1.2/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 00:41:21.000000 GoogleBard-1.1.2/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-1.1.1/LICENSE` & `GoogleBard-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.1/PKG-INFO` & `GoogleBard-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.1
+Version: 1.1.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleBard-1.1.1/README.md` & `GoogleBard-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `GoogleBard-1.1.1/setup.py` & `GoogleBard-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="1.1.1",
+    version="1.1.2",
     license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
```

### Comparing `GoogleBard-1.1.1/src/Bard.py` & `GoogleBard-1.1.2/src/Bard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-"""
-Reverse engineering of Google Bard
-"""
 import argparse
 import json
 import os
 import random
 import re
-import string
 import sys
-
+import string
 import requests
-from prompt_toolkit import prompt
-from prompt_toolkit import PromptSession
+from prompt_toolkit import prompt, PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.console import Console
 from rich.markdown import Markdown
 
@@ -51,58 +46,79 @@
 class Chatbot:
     """
     A class to interact with Google Bard.
     Parameters
         session_id: str
             The __Secure-1PSID cookie.
         proxy: str
+        timeout: int
+            Request timeout in seconds.
+        session: requests.Session
+            Requests session object.
     """
 
     __slots__ = [
         "headers",
         "_reqid",
         "SNlM0e",
         "conversation_id",
         "response_id",
         "choice_id",
+        "proxy",
+        "session_id",
         "session",
+        "timeout",
     ]
 
-    def __init__(self, session_id: str, proxy: str = None):
+    def __init__(
+        self,
+        session_id: str,
+        proxy: dict = None,
+        timeout: int = 20,
+        session: requests.Session = None,
+    ):
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
         }
         self._reqid = int("".join(random.choices(string.digits, k=4)))
+        self.proxy = proxy
         self.conversation_id = ""
         self.response_id = ""
         self.choice_id = ""
-        self.session = requests.Session()
-        if proxy:
-            self.session.proxies.update(
-                {
-                    "http": proxy,
-                    "https": proxy,
-                },
-            )
+        self.session_id = session_id
+        self.session = session or requests.Session()
         self.session.headers = headers
         self.session.cookies.set("__Secure-1PSID", session_id)
         self.SNlM0e = self.__get_snlm0e()
+        self.timeout = timeout
 
     def __get_snlm0e(self):
-        resp = self.session.get(url="https://bard.google.com/", timeout=10)
         # Find "SNlM0e":"<ID>"
+        if not self.session_id or self.session_id[-1] != ".":
+            raise Exception(
+                "__Secure-1PSID value must end with a single dot. Enter correct __Secure-1PSID value."
+            )
+        resp = self.session.get(
+            "https://bard.google.com/", timeout=10, proxies=self.proxy
+        )
         if resp.status_code != 200:
-            raise Exception("Could not get Google Bard")
-        SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
-        return SNlM0e
+            raise Exception(
+                f"Response code not 200. Response Status is {resp.status_code}"
+            )
+        SNlM0e = re.search(r"SNlM0e\":\"(.*?)\"", resp.text)
+        if not SNlM0e:
+            raise Exception(
+                "SNlM0e value not found in response. Check __Secure-1PSID value."
+            )
+        return SNlM0e.group(1)
 
     def ask(self, message: str) -> dict:
         """
         Send a message to Google Bard and return the response.
         :param message: The message to send to Google Bard.
         :return: A dict containing the response from Google Bard.
         """
@@ -119,23 +135,21 @@
             None,
             [self.conversation_id, self.response_id, self.choice_id],
         ]
         data = {
             "f.req": json.dumps([None, json.dumps(message_struct)]),
             "at": self.SNlM0e,
         }
-
-        # do the request!
         resp = self.session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
-            timeout=120,
+            timeout=self.timeout,
+            proxies=self.proxy,
         )
-
         chat_data = json.loads(resp.content.splitlines()[3])[0][2]
         if not chat_data:
             return {"content": f"Google Bard encountered an error: {resp.content}."}
         json_chat_data = json.loads(chat_data)
         images = set()
         if len(json_chat_data) >= 3:
             if len(json_chat_data[4][0]) >= 4:
@@ -172,15 +186,15 @@
         if not session:
             print("BARD_SESSION environment variable not set.")
             sys.exit(1)
         chatbot = Chatbot(session)
         # Join arguments into a single string
         MESSAGE = " ".join(sys.argv[1:])
         response = chatbot.ask(MESSAGE)
-        console.print(Markdown((response["content"])))
+        console.print(Markdown(response["content"]))
         console.print(response["images"] if response["images"] else "")
         sys.exit(0)
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--session",
         help="__Secure-1PSID cookie.",
         type=str,
```

### Comparing `GoogleBard-1.1.1/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-1.1.2/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 1.1.1
+Version: 1.1.2
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
```


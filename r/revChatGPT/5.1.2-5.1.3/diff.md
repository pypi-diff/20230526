# Comparing `tmp/revChatGPT-5.1.2.tar.gz` & `tmp/revChatGPT-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.1.2.tar", last modified: Wed May 24 18:17:38 2023, max compression
+gzip compressed data, was "revChatGPT-5.1.3.tar", last modified: Fri May 26 01:10:59 2023, max compression
```

## Comparing `revChatGPT-5.1.2.tar` & `revChatGPT-5.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    50854 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 18:17:38.000000 revChatGPT-5.1.2/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:17:38.921970 revChatGPT-5.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-24 18:17:09.000000 revChatGPT-5.1.2/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    50929 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 01:10:59.000000 revChatGPT-5.1.3/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:10:59.566065 revChatGPT-5.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-26 01:10:08.000000 revChatGPT-5.1.3/tests/test_recipient.py
```

### Comparing `revChatGPT-5.1.2/LICENSE` & `revChatGPT-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/PKG-INFO` & `revChatGPT-5.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.1.2
+Version: 5.1.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,16 +26,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained.
-
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
```

### Comparing `revChatGPT-5.1.2/README.md` & `revChatGPT-5.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained.
-
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
```

### Comparing `revChatGPT-5.1.2/setup.py` & `revChatGPT-5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.1.2",
+    version="5.1.3",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.1.2/src/revChatGPT/V1.py` & `revChatGPT-5.1.3/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://ai.fakeopen.com/api/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
 
 bcolors = t.Colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
@@ -160,16 +160,16 @@
                     "http://": config["proxy"],
                     "https://": config["proxy"],
                 }
                 self.session = AsyncClient(proxies=proxies)  # type: ignore
             else:
                 self.session.proxies.update(proxies)
 
-        self.conversation_id = conversation_id
-        self.parent_id = parent_id
+        self.conversation_id = conversation_id or config.get("conversation_id", None)
+        self.parent_id = parent_id or config.get("parent_id", None)
         self.conversation_mapping = {}
         self.conversation_id_prev_queue = []
         self.parent_id_prev_queue = []
         self.lazy_loading = lazy_loading
         self.base_url = base_url or BASE_URL
         self.recipients = RecipientManager()
```

### Comparing `revChatGPT-5.1.2/src/revChatGPT/V3.py` & `revChatGPT-5.1.3/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/__init__.py` & `revChatGPT-5.1.3/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/__main__.py` & `revChatGPT-5.1.3/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.1.3/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/recipient.py` & `revChatGPT-5.1.3/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/typings.py` & `revChatGPT-5.1.3/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT/utils.py` & `revChatGPT-5.1.3/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.1.2/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.1.3/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.1.2
+Version: 5.1.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,16 +26,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-Status: Working but unmaintained.
-
 [![](https://github.com/acheong08/ChatGPT/blob/main/docs/view.gif?raw=true)](https://pypi.python.org/pypi/revChatGPT)
 
 # Installation
 
 ```
 python -m pip install --upgrade revChatGPT
 ```
```

### Comparing `revChatGPT-5.1.2/tests/test_recipient.py` & `revChatGPT-5.1.3/tests/test_recipient.py`

 * *Files identical despite different names*


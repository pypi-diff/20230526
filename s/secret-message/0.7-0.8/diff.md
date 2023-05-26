# Comparing `tmp/secret_message-0.7.tar.gz` & `tmp/secret_message-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.7.tar", last modified: Wed May 24 18:27:11 2023, max compression
+gzip compressed data, was "secret_message-0.8.tar", last modified: Fri May 26 07:00:31 2023, max compression
```

## Comparing `secret_message-0.7.tar` & `secret_message-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 18:27:11.448382 secret_message-0.7/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.7/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-24 18:27:11.438382 secret_message-0.7/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2335 2023-05-23 06:45:28.000000 secret_message-0.7/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 18:27:11.368382 secret_message-0.7/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1804 2023-05-24 18:26:32.000000 secret_message-0.7/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-24 18:27:11.418382 secret_message-0.7/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2713 2023-05-24 18:27:11.000000 secret_message-0.7/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-24 18:27:11.000000 secret_message-0.7/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-24 18:27:11.000000 secret_message-0.7/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-24 18:27:11.000000 secret_message-0.7/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-24 18:27:11.448382 secret_message-0.7/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     2881 2023-05-24 18:26:36.000000 secret_message-0.7/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:31.093956 secret_message-0.8/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.8/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     2897 2023-05-26 07:00:31.003956 secret_message-0.8/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2519 2023-05-26 06:58:49.000000 secret_message-0.8/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:30.863956 secret_message-0.8/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1804 2023-05-24 18:26:32.000000 secret_message-0.8/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:30.983956 secret_message-0.8/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2897 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-26 07:00:31.093956 secret_message-0.8/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     3065 2023-05-26 06:58:07.000000 secret_message-0.8/setup.py
```

### Comparing `secret_message-0.7/LICENSE.txt` & `secret_message-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.7/PKG-INFO` & `secret_message-0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-Metadata-Version: 2.1
-Name: secret_message
-Version: 0.7
-Summary: Create and share a Message Secretly.
-Author: E Lusifa Taehyung
-Author-email: purplebird7613@gmail.com
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
 # Secret-Message 
-[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&style=plastic)](https://pypi.org/project/secret-message/)
+[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
+
+[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
-pip install secretmessage
+pip install secret-message
 ```
 
 ## Import the package
 ```python
-import secretmessage
+import secret_message
 
 # ------OR------
 
-#from secretmessage import create,show,history
+#from secret_message import create,show,history
 ```
 
 ## Create a Message:
 ```python
-import secretmessage as message 
+import secret_message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -59,15 +48,15 @@
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 ```
 
 ## Show/Read Message
 ```python
-import secretmessage as message
+import secret_message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -81,15 +70,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```python
-import secretmessage as message
+import secret_message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 ```
@@ -105,9 +94,7 @@
   	   "web_msg_link": "<YOUR_MESSAGE_LINK_FOR_WEB>",
   	   "api_msg_link": "<YOUR_MESSAGE_LINK_FOR_API_CALL>" 
   	},
   	........,
   ]
 }
 ```
-
-
```

### Comparing `secret_message-0.7/secret_message/__init__.py` & `secret_message-0.8/secret_message/__init__.py`

 * *Files identical despite different names*

### Comparing `secret_message-0.7/secret_message.egg-info/PKG-INFO` & `secret_message-0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-Metadata-Version: 2.1
-Name: secret-message
-Version: 0.7
-Summary: Create and share a Message Secretly.
-Author: E Lusifa Taehyung
-Author-email: purplebird7613@gmail.com
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
+import setuptools
 
+description = """
 # Secret-Message 
-[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&style=plastic)](https://pypi.org/project/secret-message/)
+[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
+
+[![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
-pip install secretmessage
+pip install secret-message
 ```
 
 ## Import the package
 ```python
-import secretmessage
+import secret_message
 
 # ------OR------
 
-#from secretmessage import create,show,history
+#from secret_message import create,show,history
 ```
 
 ## Create a Message:
 ```python
-import secretmessage as message 
+import secret_message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -59,15 +51,15 @@
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 ```
 
 ## Show/Read Message
 ```python
-import secretmessage as message
+import secret_message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -81,15 +73,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```python
-import secretmessage as message
+import secret_message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 ```
 1. Username - Just add your name as username(No registration stuff is required.)
 ```
@@ -107,7 +99,39 @@
   	},
   	........,
   ]
 }
 ```
 
 
+"""          
+
+setuptools.setup(
+
+	name = 'secret_message', 
+
+	version = '0.8',
+
+	author = "E Lusifa Taehyung",
+
+	author_email = "purplebird7613@gmail.com",
+
+	description = "Create and share a Message Secretly.",
+	
+	long_description = description,
+	
+    long_description_content_type = 'text/markdown',
+  
+	
+	packages = setuptools.find_packages(),
+ 
+	classifiers = [
+
+    "Programming Language :: Python",
+
+    "License :: OSI Approved :: MIT License",
+
+    "Operating System :: OS Independent",
+
+    ],
+
+)
```


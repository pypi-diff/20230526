# Comparing `tmp/secret_message-0.8.tar.gz` & `tmp/secret_message-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.8.tar", last modified: Fri May 26 07:00:31 2023, max compression
+gzip compressed data, was "secret_message-0.9.tar", last modified: Fri May 26 07:27:13 2023, max compression
```

## Comparing `secret_message-0.8.tar` & `secret_message-0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:31.093956 secret_message-0.8/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.8/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2897 2023-05-26 07:00:31.003956 secret_message-0.8/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2519 2023-05-26 06:58:49.000000 secret_message-0.8/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:30.863956 secret_message-0.8/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1804 2023-05-24 18:26:32.000000 secret_message-0.8/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:00:30.983956 secret_message-0.8/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2897 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-26 07:00:30.000000 secret_message-0.8/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-26 07:00:31.093956 secret_message-0.8/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     3065 2023-05-26 06:58:07.000000 secret_message-0.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:27:13.483956 secret_message-0.9/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.9/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     3080 2023-05-26 07:27:13.473956 secret_message-0.9/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2702 2023-05-26 07:26:21.000000 secret_message-0.9/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:27:13.393956 secret_message-0.9/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1804 2023-05-24 18:26:32.000000 secret_message-0.9/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-26 07:27:13.453956 secret_message-0.9/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     3080 2023-05-26 07:27:12.000000 secret_message-0.9/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-26 07:27:13.000000 secret_message-0.9/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-26 07:27:12.000000 secret_message-0.9/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-26 07:27:12.000000 secret_message-0.9/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-26 07:27:13.483956 secret_message-0.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     3248 2023-05-26 07:26:36.000000 secret_message-0.9/setup.py
```

### Comparing `secret_message-0.8/LICENSE.txt` & `secret_message-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.8/PKG-INFO` & `secret_message-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: secret_message
-Version: 0.8
+Version: 0.9
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Secret-Message 
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
 
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/PurpleBird7613/secret_msg?color=inactive&label=GitHub)](https://github.com/PurpleBird7613/secret_msg)
+
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
 pip install secret-message
```

### Comparing `secret_message-0.8/README.md` & `secret_message-0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Secret-Message 
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
 
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/PurpleBird7613/secret_msg?color=inactive&label=GitHub)](https://github.com/PurpleBird7613/secret_msg)
+
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
 pip install secret-message
```

### Comparing `secret_message-0.8/secret_message/__init__.py` & `secret_message-0.9/secret_message/__init__.py`

 * *Files identical despite different names*

### Comparing `secret_message-0.8/secret_message.egg-info/PKG-INFO` & `secret_message-0.9/secret_message.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: secret-message
-Version: 0.8
+Version: 0.9
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # Secret-Message 
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
 
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/PurpleBird7613/secret_msg?color=inactive&label=GitHub)](https://github.com/PurpleBird7613/secret_msg)
+
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
 pip install secret-message
```

### Comparing `secret_message-0.8/setup.py` & `secret_message-0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import setuptools
 
 description = """
 # Secret-Message 
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blueviolet&label=Web-version%20&logo=appveyor&style=plastic)](https://secret-msg.onrender.com/)
 
+[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/PurpleBird7613/secret_msg?color=inactive&label=GitHub)](https://github.com/PurpleBird7613/secret_msg)
+
 [![PyPI](https://img.shields.io/pypi/v/secret-message?color=blue&label=python-package&style=plastic)](https://pypi.org/project/secret-message/)
 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```python
 pip install secret-message
@@ -105,15 +107,15 @@
 
 """          
 
 setuptools.setup(
 
 	name = 'secret_message', 
 
-	version = '0.8',
+	version = '0.9',
 
 	author = "E Lusifa Taehyung",
 
 	author_email = "purplebird7613@gmail.com",
 
 	description = "Create and share a Message Secretly.",
```


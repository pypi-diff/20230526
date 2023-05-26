# Comparing `tmp/corby-0.0.9.tar.gz` & `tmp/corby-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.0.9.tar", last modified: Thu May 25 11:24:59 2023, max compression
+gzip compressed data, was "corby-0.1.1.tar", last modified: Fri May 26 15:08:01 2023, max compression
```

## Comparing `corby-0.0.9.tar` & `corby-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.033194 corby-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 11:24:42.000000 corby-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 11:24:59.033194 corby-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 11:24:42.000000 corby-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 11:24:42.000000 corby-0.0.9/corby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 11:24:42.000000 corby-0.0.9/corby/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.033194 corby-0.0.9/corby/generator/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 11:24:42.000000 corby-0.0.9/corby/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:24:59.033194 corby-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 11:24:42.000000 corby-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 15:07:43.000000 corby-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 15:08:01.203511 corby-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-26 15:07:43.000000 corby-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:07:43.000000 corby-0.1.1/corby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:07:43.000000 corby-0.1.1/corby/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/corby/generator/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/base_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/corby/generator/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/notebook/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-26 15:07:43.000000 corby-0.1.1/corby/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:08:01.203511 corby-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-26 15:07:43.000000 corby-0.1.1/setup.py
```

### Comparing `corby-0.0.9/LICENSE` & `corby-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corby-0.0.9/PKG-INFO` & `corby-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.0.9
+Version: 0.1.1
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,15 +14,17 @@
 
 ![pypi](https://github.com/JoseHervas/corby/actions/workflows/publish.yml/badge.svg) ![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) [![Downloads](https://static.pepy.tech/badge/corby)](https://pepy.tech/project/corby) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
 
 ## 🚀 Quick Install
 
 ```bash
 pip install corby
-alias corby="python -m corby"
+
+# check your installation
+corby -v
 ```
 
 ## 🤔 What is this?
 
 AI applications are awesome, but... who has time to go through all the settings, configurations and the hell of folder structuring? 😫
 
 **Corby** is a tool that bootstraps the skeleton of your AI applications so you don't have spend a ton of time preparing the configurations.
```

### Comparing `corby-0.0.9/README.md` & `corby-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 ![pypi](https://github.com/JoseHervas/corby/actions/workflows/publish.yml/badge.svg) ![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) [![Downloads](https://static.pepy.tech/badge/corby)](https://pepy.tech/project/corby) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
 
 ## 🚀 Quick Install
 
 ```bash
 pip install corby
-alias corby="python -m corby"
+
+# check your installation
+corby -v
 ```
 
 ## 🤔 What is this?
 
 AI applications are awesome, but... who has time to go through all the settings, configurations and the hell of folder structuring? 😫
 
 **Corby** is a tool that bootstraps the skeleton of your AI applications so you don't have spend a ton of time preparing the configurations.
```

### Comparing `corby-0.0.9/corby/generator/chatbot/index.py` & `corby-0.1.1/corby/generator/chatbot/index.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 """Dispatches the action to the corresponding chatbot generator"""
 
 import inquirer
 from .cli import CliChatbotGenerator
+from .telegram import TelegramChatbotGenerator
+from .web import WebChatbotGenerator
 
 def create_chatbot():
-    """Ask the user for the chatbot's name and interface and create it"""
+    """Ask the user for the chatbot's name and interface and
+    dispatches the action to the corresponding chatbot generator"""
     questions = [
         inquirer.Text("name", message="Name of your chatbot:"),
-        inquirer.List("interface", message="Choose your chatbot's interface:", choices=["CLI"]),
+        inquirer.List(
+            "interface", 
+            message="Choose your chatbot's interface:",
+            choices=["CLI", "Telegram", "Web"]
+        ),
     ]
     answers = inquirer.prompt(questions)
     if answers["interface"] == "CLI":
         generator = CliChatbotGenerator()
-        generator.create_cli_chatbot(answers["name"])
+        generator.create_chatbot(answers["name"])
+    elif answers["interface"] == "Telegram":
+        generator = TelegramChatbotGenerator()
+        generator.create_chatbot(answers["name"])
+    elif answers["interface"] == "Web":
+        generator = WebChatbotGenerator()
+        generator.create_chatbot(answers["name"])
```

### Comparing `corby-0.0.9/corby/index.py` & `corby-0.1.1/corby/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Main CLI entrypoint for Corby"""
 
 import argparse
 from string import Template
 from .generator.chatbot.index import create_chatbot
+from .generator.notebook.index import create_notebook
 
-__version__ = "0.0.9"
+__version__ = "0.1.1"
 
 # We'll include more features in the future
 available_actions = ['new']
 
 available_entities = ['chatbot', 'notebook']
 
 parser = argparse.ArgumentParser(
@@ -27,13 +28,13 @@
 args = parser.parse_args()
 
 def main():
     """Dispatches the action to the corresponding manager"""
     if args.action:
         if args.action == 'new':
             if args.entity == 'notebook':
-                print("Sorry, the notebook generator is not yet available 😥")
+                create_notebook()
             elif args.entity == 'chatbot':
                 create_chatbot()
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `corby-0.0.9/corby.egg-info/PKG-INFO` & `corby-0.1.1/corby.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.0.9
+Version: 0.1.1
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -14,15 +14,17 @@
 
 ![pypi](https://github.com/JoseHervas/corby/actions/workflows/publish.yml/badge.svg) ![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) [![Downloads](https://static.pepy.tech/badge/corby)](https://pepy.tech/project/corby) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
 
 ## 🚀 Quick Install
 
 ```bash
 pip install corby
-alias corby="python -m corby"
+
+# check your installation
+corby -v
 ```
 
 ## 🤔 What is this?
 
 AI applications are awesome, but... who has time to go through all the settings, configurations and the hell of folder structuring? 😫
 
 **Corby** is a tool that bootstraps the skeleton of your AI applications so you don't have spend a ton of time preparing the configurations.
```

### Comparing `corby-0.0.9/setup.py` & `corby-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 '''Pypi setup file for corby'''
 
 from setuptools import setup, find_packages
 
 setup(
     name="corby",
-    version="0.0.9",
+    version="0.1.1",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     # pylint: disable=consider-using-with
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
     packages=find_packages(),
+    entry_points={
+        'console_scripts': [
+            'corby = corby.__main__:main',
+        ],
+    },
     install_requires=[
         "inquirer",
         "jinja2",
         "gitpython",
     ],
 )
```


# Comparing `tmp/gptty-0.2.6.tar.gz` & `tmp/gptty-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptty-0.2.6.tar", last modified: Mon May 15 19:14:45 2023, max compression
+gzip compressed data, was "gptty-0.2.7.tar", last modified: Thu May 25 22:17:34 2023, max compression
```

## Comparing `gptty-0.2.6.tar` & `gptty-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.792317 gptty-0.2.6/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1073 2023-03-19 16:18:57.000000 gptty-0.2.6/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-04-05 23:32:19.000000 gptty-0.2.6/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)    12097 2023-05-15 19:14:45.792317 gptty-0.2.6/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)    11674 2023-05-14 21:20:17.000000 gptty-0.2.6/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/assets/
--rw-rw-r--   0 sig       (1000) sig       (1000)    90232 2023-03-20 03:21:49.000000 gptty-0.2.6/assets/context_example.png
--rw-rw-r--   0 sig       (1000) sig       (1000)   125593 2023-03-29 18:54:23.000000 gptty-0.2.6/assets/error_troubleshooting_example.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    83079 2023-03-31 16:52:10.000000 gptty-0.2.6/assets/json_example.png
--rw-rw-r--   0 sig       (1000) sig       (1000)   170440 2023-03-27 23:01:52.000000 gptty-0.2.6/assets/question_chain_example.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    53244 2023-03-30 21:07:16.000000 gptty-0.2.6/assets/verbosity_example.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/gptty/
--rw-rw-r--   0 sig       (1000) sig       (1000)      269 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/__init__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     8533 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/__main__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     3415 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/config.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     9363 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/context.py
--rw-rw-r--   0 sig       (1000) sig       (1000)    18316 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/gptty.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     4154 2023-05-15 19:14:04.000000 gptty-0.2.6/gptty/tagging.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/gptty.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)    12097 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      552 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/entry_points.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)      119 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        6 2023-05-15 19:14:45.000000 gptty-0.2.6/gptty.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)      118 2023-04-02 01:10:59.000000 gptty-0.2.6/requirements.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-05-15 19:14:45.792317 gptty-0.2.6/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)      835 2023-05-15 19:14:04.000000 gptty-0.2.6/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-15 19:14:45.788317 gptty-0.2.6/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     2047 2023-05-14 21:23:21.000000 gptty-0.2.6/tests/test_config.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     5149 2023-04-04 21:44:31.000000 gptty-0.2.6/tests/test_context.py
--rw-rw-r--   0 sig       (1000) sig       (1000)     1036 2023-03-29 19:43:35.000000 gptty-0.2.6/tests/test_tagging.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-25 22:17:34.166716 gptty-0.2.7/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1073 2023-03-19 16:18:57.000000 gptty-0.2.7/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-04-05 23:32:19.000000 gptty-0.2.7/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)    13753 2023-05-25 22:17:34.166716 gptty-0.2.7/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)    13329 2023-05-25 14:15:52.000000 gptty-0.2.7/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-25 22:17:34.166716 gptty-0.2.7/assets/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    90232 2023-03-20 03:21:49.000000 gptty-0.2.7/assets/context_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)   125593 2023-03-29 18:54:23.000000 gptty-0.2.7/assets/error_troubleshooting_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    83079 2023-03-31 16:52:10.000000 gptty-0.2.7/assets/json_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)   170440 2023-03-27 23:01:52.000000 gptty-0.2.7/assets/question_chain_example.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    53244 2023-03-30 21:07:16.000000 gptty-0.2.7/assets/verbosity_example.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-25 22:17:34.166716 gptty-0.2.7/gptty/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    13992 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     8533 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/__main__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3415 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/config.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     9363 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/context.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)    18316 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/gptty.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4154 2023-05-25 22:16:56.000000 gptty-0.2.7/gptty/tagging.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-25 22:17:34.166716 gptty-0.2.7/gptty.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    13753 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      552 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       46 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/entry_points.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)      119 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        6 2023-05-25 22:17:34.000000 gptty-0.2.7/gptty.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)      118 2023-04-02 01:10:59.000000 gptty-0.2.7/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-05-25 22:17:34.166716 gptty-0.2.7/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)      835 2023-05-25 22:16:56.000000 gptty-0.2.7/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-05-25 22:17:34.166716 gptty-0.2.7/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2047 2023-05-14 21:23:21.000000 gptty-0.2.7/tests/test_config.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     5149 2023-04-04 21:44:31.000000 gptty-0.2.7/tests/test_context.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1036 2023-03-29 19:43:35.000000 gptty-0.2.7/tests/test_tagging.py
```

### Comparing `gptty-0.2.6/LICENSE` & `gptty-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/PKG-INFO` & `gptty-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptty
-Version: 0.2.6
+Version: 0.2.7
 Summary: Chat GPT wrapper in your TTY 
 Home-page: https://github.com/signebedi/gptty
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -114,15 +114,15 @@
 | :context[a:b] | Display the context history, optionally specifying a range a and b. *Under development*   |
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
-api_key: SOME_CONFIG_HERE
+api_key: SOME_KEY_HERE
 org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
@@ -218,7 +218,43 @@
 You can send each question from the `questions.txt` file to the `gptty query` command using the following bash one-liner:
 
 ```bash
 xargs -d '\n' -I {} gptty query --question "{}" < questions.txt
 ```
 
 ![question chain example](assets/question_chain_example.png)
+
+
+## UniversalCompletion
+
+The UniversalCompletion class provides a unified interface for interacting with OpenAI's language models, (mostly) abstracting away the specifics of whether the application is using the Completion or ChatCompletion mode. The main idea is to facilitate the creation, configuration, and management of the language models. Here is some example usage.
+
+```python
+>>> from gptty import UniversalCompletion
+>>> g = UniversalCompletion(api_key="sk-SOME_CHARS_HERE", org_id="org-SOME_CHARS_HERE")
+>>> g.connect()
+>>> g.set_model('gpt-3.5-turbo')
+>>> g.validate_model_type(g.model)
+'v1/chat/completions'
+>>> g.fetch_response(prompt=[{"role": "user", "content": "What is an abstraction?"}])
+<OpenAIObject chat.completion id=chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ at 0x7fc2ls949e21> JSON: {
+  "choices": [
+    {
+      "finish_reason": "stop",
+      "index": 0,
+      "message": {
+        "content": "An abstraction is a simplified representation of a complex system or concept. It involves focusing on the most important aspects of the system or concept and ignoring the details that are not relevant to the current context. Abstractions are used in many fields, including computer science, mathematics, and philosophy, to help people understand complex ideas and systems. They can be represented in various forms, such as diagrams, models, or algorithms.",
+        "role": "assistant"
+      }
+    }
+  ],
+  "created": 1684990000,
+  "id": "chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ",
+  "model": "gpt-3.5-turbo-0301",
+  "object": "chat.completion",
+  "usage": {
+    "completion_tokens": 82,
+    "prompt_tokens": 13,
+    "total_tokens": 95
+  }
+}
+```
```

### Comparing `gptty-0.2.6/README.md` & `gptty-0.2.7/gptty.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gptty
+Version: 0.2.7
+Summary: Chat GPT wrapper in your TTY 
+Home-page: https://github.com/signebedi/gptty
+Author: Sig Janoska-Bedi
+Author-email: signe@atreeus.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gptty
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/gptty.svg)](https://pypi.python.org/pypi/gptty)
 [![Downloads](https://static.pepy.tech/badge/gptty)](https://pepy.tech/project/gptty)
 [![gptty tests](https://github.com/signebedi/gptty/workflows/tests/badge.svg)](https://github.com/signebedi/gptty/actions)
 
@@ -100,15 +114,15 @@
 | :context[a:b] | Display the context history, optionally specifying a range a and b. *Under development*   |
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
-api_key: SOME_CONFIG_HERE
+api_key: SOME_KEY_HERE
 org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
@@ -204,7 +218,43 @@
 You can send each question from the `questions.txt` file to the `gptty query` command using the following bash one-liner:
 
 ```bash
 xargs -d '\n' -I {} gptty query --question "{}" < questions.txt
 ```
 
 ![question chain example](assets/question_chain_example.png)
+
+
+## UniversalCompletion
+
+The UniversalCompletion class provides a unified interface for interacting with OpenAI's language models, (mostly) abstracting away the specifics of whether the application is using the Completion or ChatCompletion mode. The main idea is to facilitate the creation, configuration, and management of the language models. Here is some example usage.
+
+```python
+>>> from gptty import UniversalCompletion
+>>> g = UniversalCompletion(api_key="sk-SOME_CHARS_HERE", org_id="org-SOME_CHARS_HERE")
+>>> g.connect()
+>>> g.set_model('gpt-3.5-turbo')
+>>> g.validate_model_type(g.model)
+'v1/chat/completions'
+>>> g.fetch_response(prompt=[{"role": "user", "content": "What is an abstraction?"}])
+<OpenAIObject chat.completion id=chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ at 0x7fc2ls949e21> JSON: {
+  "choices": [
+    {
+      "finish_reason": "stop",
+      "index": 0,
+      "message": {
+        "content": "An abstraction is a simplified representation of a complex system or concept. It involves focusing on the most important aspects of the system or concept and ignoring the details that are not relevant to the current context. Abstractions are used in many fields, including computer science, mathematics, and philosophy, to help people understand complex ideas and systems. They can be represented in various forms, such as diagrams, models, or algorithms.",
+        "role": "assistant"
+      }
+    }
+  ],
+  "created": 1684990000,
+  "id": "chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ",
+  "model": "gpt-3.5-turbo-0301",
+  "object": "chat.completion",
+  "usage": {
+    "completion_tokens": 82,
+    "prompt_tokens": 13,
+    "total_tokens": 95
+  }
+}
+```
```

### Comparing `gptty-0.2.6/assets/context_example.png` & `gptty-0.2.7/assets/context_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/assets/error_troubleshooting_example.png` & `gptty-0.2.7/assets/error_troubleshooting_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/assets/json_example.png` & `gptty-0.2.7/assets/json_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/assets/question_chain_example.png` & `gptty-0.2.7/assets/question_chain_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/assets/verbosity_example.png` & `gptty-0.2.7/assets/verbosity_example.png`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/gptty/__main__.py` & `gptty-0.2.7/gptty/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 gptty: context-preserving chatGPT CLI wrapper
 
 """
 
 __name__ = "gptty"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 # general packages
 import click
 import os
```

### Comparing `gptty-0.2.6/gptty/config.py` & `gptty-0.2.7/gptty/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "gptty.config"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import configparser
 
 # parse config data
```

### Comparing `gptty-0.2.6/gptty/context.py` & `gptty-0.2.7/gptty/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "gptty.context"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 
 import click
 import tiktoken
```

### Comparing `gptty-0.2.6/gptty/gptty.py` & `gptty-0.2.7/gptty/gptty.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "gptty.gptty"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import click
 import openai
 import pandas as pd
```

### Comparing `gptty-0.2.6/gptty/tagging.py` & `gptty-0.2.7/gptty/tagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 __name__ = "gptty.tagging"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi"]
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __license__ = "MIT"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 # def old_get_tag_from_text(user_input, replacement_string='-'):
 
 #     # Initialize the tag and remaining text variables
```

### Comparing `gptty-0.2.6/gptty.egg-info/PKG-INFO` & `gptty-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gptty
-Version: 0.2.6
-Summary: Chat GPT wrapper in your TTY 
-Home-page: https://github.com/signebedi/gptty
-Author: Sig Janoska-Bedi
-Author-email: signe@atreeus.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gptty
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/signebedi/gptty/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/gptty.svg)](https://pypi.python.org/pypi/gptty)
 [![Downloads](https://static.pepy.tech/badge/gptty)](https://pepy.tech/project/gptty)
 [![gptty tests](https://github.com/signebedi/gptty/workflows/tests/badge.svg)](https://github.com/signebedi/gptty/actions)
 
@@ -114,15 +100,15 @@
 | :context[a:b] | Display the context history, optionally specifying a range a and b. *Under development*   |
 
 To use a command, simply type it into the command prompt and press Enter. For example, use the following command to display the current configuration settings in the terminal:
 
 ```
 > :configs
 
-api_key: SOME_CONFIG_HERE
+api_key: SOME_KEY_HERE
 org_id: org-SOME_CHARS_HERE
 your_name: question
 gpt_name: response
 output_file: output.txt
 model: text-davinci-003
 temperature: 0.0
 max_tokens: 250
@@ -218,7 +204,43 @@
 You can send each question from the `questions.txt` file to the `gptty query` command using the following bash one-liner:
 
 ```bash
 xargs -d '\n' -I {} gptty query --question "{}" < questions.txt
 ```
 
 ![question chain example](assets/question_chain_example.png)
+
+
+## UniversalCompletion
+
+The UniversalCompletion class provides a unified interface for interacting with OpenAI's language models, (mostly) abstracting away the specifics of whether the application is using the Completion or ChatCompletion mode. The main idea is to facilitate the creation, configuration, and management of the language models. Here is some example usage.
+
+```python
+>>> from gptty import UniversalCompletion
+>>> g = UniversalCompletion(api_key="sk-SOME_CHARS_HERE", org_id="org-SOME_CHARS_HERE")
+>>> g.connect()
+>>> g.set_model('gpt-3.5-turbo')
+>>> g.validate_model_type(g.model)
+'v1/chat/completions'
+>>> g.fetch_response(prompt=[{"role": "user", "content": "What is an abstraction?"}])
+<OpenAIObject chat.completion id=chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ at 0x7fc2ls949e21> JSON: {
+  "choices": [
+    {
+      "finish_reason": "stop",
+      "index": 0,
+      "message": {
+        "content": "An abstraction is a simplified representation of a complex system or concept. It involves focusing on the most important aspects of the system or concept and ignoring the details that are not relevant to the current context. Abstractions are used in many fields, including computer science, mathematics, and philosophy, to help people understand complex ideas and systems. They can be represented in various forms, such as diagrams, models, or algorithms.",
+        "role": "assistant"
+      }
+    }
+  ],
+  "created": 1684990000,
+  "id": "chatcmpl-7JxBPjmne2lsd9s2uqy3GasdlXQCZ",
+  "model": "gpt-3.5-turbo-0301",
+  "object": "chat.completion",
+  "usage": {
+    "completion_tokens": 82,
+    "prompt_tokens": 13,
+    "total_tokens": 95
+  }
+}
+```
```

### Comparing `gptty-0.2.6/gptty.egg-info/SOURCES.txt` & `gptty-0.2.7/gptty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/setup.py` & `gptty-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     DESCRIPTION = f.read()
 
 with open('requirements.txt') as f:
     REQUIRED = f.read().splitlines()
 
 setup(
     name='gptty',
-    version="0.2.6",
+    version="0.2.7",
     description='Chat GPT wrapper in your TTY ',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     long_description=DESCRIPTION, 
     long_description_content_type='text/markdown',
     url="https://github.com/signebedi/gptty",
     packages=['gptty'],
```

### Comparing `gptty-0.2.6/tests/test_config.py` & `gptty-0.2.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/tests/test_context.py` & `gptty-0.2.7/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `gptty-0.2.6/tests/test_tagging.py` & `gptty-0.2.7/tests/test_tagging.py`

 * *Files identical despite different names*


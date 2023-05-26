# Comparing `tmp/openthaigpt-0.1.0.tar.gz` & `tmp/openthaigpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openthaigpt-0.1.0.tar", last modified: Sun Apr 23 17:03:39 2023, max compression
+gzip compressed data, was "openthaigpt-0.1.1.tar", last modified: Fri May 26 15:45:33 2023, max compression
```

## Comparing `openthaigpt-0.1.0.tar` & `openthaigpt-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,27 @@
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069864 openthaigpt-0.1.0/
--rw-r--r--   0 kv         (501) staff       (20)      130 2023-03-11 07:31:58.000000 openthaigpt-0.1.0/AUTHORS.md
--rw-r--r--   0 kv         (501) staff       (20)     3406 2023-03-11 07:32:57.000000 openthaigpt-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 kv         (501) staff       (20)      428 2023-04-23 17:01:09.000000 openthaigpt-0.1.0/HISTORY.md
--rw-r--r--   0 kv         (501) staff       (20)      595 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/LICENSE
--rw-r--r--   0 kv         (501) staff       (20)      257 2023-03-11 07:31:36.000000 openthaigpt-0.1.0/MANIFEST.in
--rw-r--r--   0 kv         (501) staff       (20)     3909 2023-04-23 17:03:39.069923 openthaigpt-0.1.0/PKG-INFO
--rw-r--r--   0 kv         (501) staff       (20)     2360 2023-04-23 17:01:09.000000 openthaigpt-0.1.0/README.md
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.068089 openthaigpt-0.1.0/docs/
--rw-r--r--   0 kv         (501) staff       (20)      612 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/Makefile
--rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:31:16.000000 openthaigpt-0.1.0/docs/authors.rst
--rwxr-xr-x   0 kv         (501) staff       (20)     4862 2023-03-11 07:31:10.000000 openthaigpt-0.1.0/docs/conf.py
--rw-r--r--   0 kv         (501) staff       (20)       32 2023-03-11 07:31:04.000000 openthaigpt-0.1.0/docs/contributing.rst
--rw-r--r--   0 kv         (501) staff       (20)       27 2023-03-11 07:30:55.000000 openthaigpt-0.1.0/docs/history.rst
--rw-r--r--   0 kv         (501) staff       (20)      308 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/index.rst
--rw-r--r--   0 kv         (501) staff       (20)     1142 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/installation.rst
--rw-r--r--   0 kv         (501) staff       (20)      809 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/make.bat
--rw-r--r--   0 kv         (501) staff       (20)       26 2023-03-11 07:30:59.000000 openthaigpt-0.1.0/docs/readme.rst
--rw-r--r--   0 kv         (501) staff       (20)       77 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/docs/usage.rst
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.068448 openthaigpt-0.1.0/openthaigpt/
--rw-r--r--   0 kv         (501) staff       (20)      199 2023-04-23 17:03:21.000000 openthaigpt-0.1.0/openthaigpt/__init__.py
--rw-r--r--   0 kv         (501) staff       (20)     2540 2023-04-23 16:50:59.000000 openthaigpt-0.1.0/openthaigpt/openthaigpt_module.py
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069481 openthaigpt-0.1.0/openthaigpt.egg-info/
--rw-r--r--   0 kv         (501) staff       (20)     3909 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/PKG-INFO
--rw-r--r--   0 kv         (501) staff       (20)      561 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/SOURCES.txt
--rw-r--r--   0 kv         (501) staff       (20)        1 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/dependency_links.txt
--rw-r--r--   0 kv         (501) staff       (20)        1 2023-02-28 01:42:10.000000 openthaigpt-0.1.0/openthaigpt.egg-info/not-zip-safe
--rw-r--r--   0 kv         (501) staff       (20)       56 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/requires.txt
--rw-r--r--   0 kv         (501) staff       (20)       12 2023-04-23 17:03:39.000000 openthaigpt-0.1.0/openthaigpt.egg-info/top_level.txt
--rw-r--r--   0 kv         (501) staff       (20)      383 2023-04-23 17:03:39.070150 openthaigpt-0.1.0/setup.cfg
--rw-r--r--   0 kv         (501) staff       (20)     1776 2023-04-23 17:03:11.000000 openthaigpt-0.1.0/setup.py
-drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-04-23 17:03:39.069736 openthaigpt-0.1.0/tests/
--rw-r--r--   0 kv         (501) staff       (20)       41 2023-02-28 01:06:54.000000 openthaigpt-0.1.0/tests/__init__.py
--rw-r--r--   0 kv         (501) staff       (20)      548 2023-04-23 17:03:01.000000 openthaigpt-0.1.0/tests/test_openthaigpt.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-05-26 15:45:33.722405 openthaigpt-0.1.1/
+-rw-r--r--   0 kv         (501) staff       (20)      130 2023-03-11 07:31:58.000000 openthaigpt-0.1.1/AUTHORS.md
+-rw-r--r--   0 kv         (501) staff       (20)     3406 2023-03-11 07:32:57.000000 openthaigpt-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 kv         (501) staff       (20)      575 2023-05-26 14:38:04.000000 openthaigpt-0.1.1/HISTORY.md
+-rw-r--r--   0 kv         (501) staff       (20)      595 2023-02-28 01:06:54.000000 openthaigpt-0.1.1/LICENSE
+-rw-r--r--   0 kv         (501) staff       (20)      257 2023-03-11 07:31:36.000000 openthaigpt-0.1.1/MANIFEST.in
+-rw-r--r--   0 kv         (501) staff       (20)     5818 2023-05-26 15:45:33.722648 openthaigpt-0.1.1/PKG-INFO
+-rw-r--r--   0 kv         (501) staff       (20)     4122 2023-05-26 14:34:27.000000 openthaigpt-0.1.1/README.md
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-05-26 15:45:33.719687 openthaigpt-0.1.1/docs/
+-rw-r--r--   0 kv         (501) staff       (20)      612 2023-02-28 01:06:54.000000 openthaigpt-0.1.1/docs/Makefile
+-rwxr-xr-x   0 kv         (501) staff       (20)     4862 2023-03-11 07:31:10.000000 openthaigpt-0.1.1/docs/conf.py
+-rw-r--r--   0 kv         (501) staff       (20)      809 2023-02-28 01:06:54.000000 openthaigpt-0.1.1/docs/make.bat
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-05-26 15:45:33.720413 openthaigpt-0.1.1/openthaigpt/
+-rw-r--r--   0 kv         (501) staff       (20)      199 2023-05-26 14:29:36.000000 openthaigpt-0.1.1/openthaigpt/__init__.py
+-rw-r--r--   0 kv         (501) staff       (20)     5861 2023-05-26 15:45:19.000000 openthaigpt-0.1.1/openthaigpt/openthaigpt_module.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-05-26 15:45:33.721534 openthaigpt-0.1.1/openthaigpt.egg-info/
+-rw-r--r--   0 kv         (501) staff       (20)     5818 2023-05-26 15:45:33.000000 openthaigpt-0.1.1/openthaigpt.egg-info/PKG-INFO
+-rw-r--r--   0 kv         (501) staff       (20)      437 2023-05-26 15:45:33.000000 openthaigpt-0.1.1/openthaigpt.egg-info/SOURCES.txt
+-rw-r--r--   0 kv         (501) staff       (20)        1 2023-05-26 15:45:33.000000 openthaigpt-0.1.1/openthaigpt.egg-info/dependency_links.txt
+-rw-r--r--   0 kv         (501) staff       (20)        1 2023-05-26 14:36:47.000000 openthaigpt-0.1.1/openthaigpt.egg-info/not-zip-safe
+-rw-r--r--   0 kv         (501) staff       (20)       56 2023-05-26 15:45:33.000000 openthaigpt-0.1.1/openthaigpt.egg-info/requires.txt
+-rw-r--r--   0 kv         (501) staff       (20)       12 2023-05-26 15:45:33.000000 openthaigpt-0.1.1/openthaigpt.egg-info/top_level.txt
+-rw-r--r--   0 kv         (501) staff       (20)      383 2023-05-26 15:45:33.723034 openthaigpt-0.1.1/setup.cfg
+-rw-r--r--   0 kv         (501) staff       (20)     1776 2023-05-26 14:34:08.000000 openthaigpt-0.1.1/setup.py
+drwxr-xr-x   0 kv         (501) staff       (20)        0 2023-05-26 15:45:33.722133 openthaigpt-0.1.1/tests/
+-rw-r--r--   0 kv         (501) staff       (20)       41 2023-02-28 01:06:54.000000 openthaigpt-0.1.1/tests/__init__.py
+-rw-r--r--   0 kv         (501) staff       (20)      548 2023-04-23 17:03:01.000000 openthaigpt-0.1.1/tests/test_openthaigpt.py
```

### Comparing `openthaigpt-0.1.0/CONTRIBUTING.md` & `openthaigpt-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.1.0/LICENSE` & `openthaigpt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.1.0/PKG-INFO` & `openthaigpt-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,104 @@
-Metadata-Version: 2.1
-Name: openthaigpt
-Version: 0.1.0
-Summary: OpenThaiGPT focuses on developing a Thai Chatbot system to have capabilities equivalent to ChatGPT, as well as being able to connect to external systems and be able to retrieve data flexibly. Easily expandable and customizable and developed into Free open source software for everyone.
-Home-page: https://github.com/OpenThaiGPT/openthaigpt
-Author: Kobkrit Viriyayudhakorn
-Author-email: kobkrit@iapp.co.th
-License: Apache Software License 2.0
-Keywords: openthaigpt
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Natural Language :: Thai
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 # OpenThaiGPT
 
 [![](https://img.shields.io/pypi/v/openthaigpt.svg)](https://pypi.python.org/pypi/openthaigpt) [![](https://pyup.io/repos/github/OpenThaiGPT/openthaigpt/shield.svg)](https://pyup.io/repos/github/OpenThaiGPT/openthaigpt/)
 
 OpenThaiGPT focuses on developing a Thai Chatbot system to have capabilities equivalent to ChatGPT, as well as being able to connect to external systems and be able to retrieve data flexibly. Easily expandable and customizable and developed into Free open source software for everyone.
 
 * Free software: Apache Software License 2.0
 * Project Homepage: https://openthaigpt.aieat.or.th
-* Documentation: https://openthaigpt.readthedocs.io.
+* Documentation: https://openthaigpt.readthedocs.io
+
+## Versions
 
-## Features
+- OpenThaiGPT chat inference library (this repository): version 0.1.1
+
+- Released models
+    * kobkrit/openthaigpt-0.1.0-beta
+      - Pretraining Model: Facebook Llama (7 billion params)
+      - Dataset: 200,000 Various Translated Instruction Dataset 
+      - RLHF: None
+      - Minimium Requirement: Nvidia T4 16GB
+
+    * kobkrit/openthaigpt-0.1.0-alpha
+      - Pretraining Model: ByT5-XL (3.74 billion params)
+      - Dataset: 50,000 Thai SelfInstruct 
+      - RLHF: None
+      - Minimium Requirement: Nvidia A100 40GB
+
+    * kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4
+      - Pretraining Model: GPT-2 Thai-base
+      - InstructDataset: 300,000 Pantip + 5,000 Wiki QA => 12,920 Thai InstructGPT
+      - RLHF: None
+      - Minimium Requirement: CPU or Nvidia GTX 1060 6GB
+
+    * kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.3
+      - Pretraining Model: GPT-2 Thai-base
+      - InstructDataset: 300,000 Pantip + 5,000 Wiki QA => 7,000 Thai InstructGPT
+      - RLHF: None
+      - Minimium Requirement: CPU or Nvidia GTX 1060 6GB
+
+    * kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.2
+      - Pretraining Model: GPT-2 Thai-base
+      - InstructDataset: 7,000 Thai InstructGPT
+      - RLHF: None
+      - Minimium Requirement: CPU or Nvidia GTX 1060 6GB
+
+    * kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.1
+      - Pretraining Model: GPT-2 Thai-base
+      - InstructDataset: 298,678 QA Pairs getting from 70,000 Pantip katoos + Wikipedia QA by iApp
+      - RLHF: None
+      - Minimium Requirement: CPU or Nvidia GTX 1060 6GB
 
-* You can now select the model_name as follows:
-* kobkrit/openthaigpt-0.1.0-alpha
-* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4
-* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.3
-* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.2
-* kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.1
 
 ## Installation
 Python>=3.6
 
 ### CPU-Only
 ``$ pip install openthaigpt torch --extra-index-url https://download.pytorch.org/whl/cpu``
 
-### GPU
+### With GPU
 
 CUDA 11.6
 ``$ pip install openthaigpt torch --extra-index-url https://download.pytorch.org/whl/cu116``
 
 CUDA 11.7
 ``$ pip install openthaigpt torch``
 
-## Usage
+## Using 0.1.0-beta model
 ```
 import openthaigpt
 
-print(openthaigpt.generate("Q: อยากลดความอ้วนทำไง\n\nA:"))
-print(openthaigpt.zero("การลดน้ำหนักเป็นเรื่องที่ต้องพิจารณาอย่างละเอียดและรอบคอบเพื่อให้ได้ผลลัพธ์ที่ดีและมีประสิทธิภาพมากที่สุด"))
+print(openthaigpt.generate(instruction="แปลภาษาอังกฤษเป็นภาษาไทย", input="We want to reduce weight.", model_name = "kobkrit/openthaigpt-0.1.0-beta", min_length=50, max_length=300, top_p=0.75, top_k=40, num_beams=1, no_repeat_ngram_size=0, temperature=0.1, early_stopping=True, load_8bit=False))
 ```
 
 ## Using 0.1.0-alpha model
 ```
 import openthaigpt
 
 print(openthaigpt.generate(instruction="แปลภาษาอังกฤษเป็นภาษาไทย", input="We want to reduce weight.", model_name = "kobkrit/openthaigpt-0.1.0-alpha", min_length=50, max_length=300,  top_k=20, num_beams=5, no_repeat_ngram_size=20, temperature=1, early_stopping=True))
 ```
 
-## Collaboration By
+
+## Usage 0.0.1-0.0.4 model
+```
+import openthaigpt
+
+print(openthaigpt.generate("Q: อยากลดความอ้วนทำไง\n\nA:", model_name = "kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4"))
+print(openthaigpt.zero("การลดน้ำหนักเป็นเรื่องที่ต้องพิจารณาอย่างละเอียดและรอบคอบเพื่อให้ได้ผลลัพธ์ที่ดีและมีประสิทธิภาพมากที่สุด"))
+```
+
+## Sponsored by
+* Pantip.com
+* ThaiSC
+
+## Collaborated By
 * Artificial Intelligence Entrepreneur Association of Thailand (AIEAT)
 * Artificial Intelligence Association of Thailand (AIAT)
 
 ## Supported By
 * NECTEC
 * iApp Technology
-* Pantip
 * NVIDIA
 * Microsoft
 * Mahidol University
 * Gitbook
-
-# History
-
-0.1.0 (2023-04-23)
-
-* Update Model to Version 0.1.0-alpha (https://huggingface.co/kobkrit/openthaigpt-0.1.0-alpha)
-
-0.0.9 - 0.0.10 (2023-03-19)
-
-* Release OpenThaiGPT Zero
-
-0.0.8 (2023-03-12)
-
-* Update Readme
-
-0.0.7 (2023-03-12)
-
-* Update Model to Version 0.0.4 (https://huggingface.co/kobkrit/openthaigpt-gpt2-instructgpt-poc-0.0.4)
-
-0.0.6 (2023-03-05)
-
-* Update README
-
-0.0.5 (2023-02-28)
-
-* First release on PyPI.
```

### Comparing `openthaigpt-0.1.0/docs/Makefile` & `openthaigpt-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.1.0/docs/conf.py` & `openthaigpt-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.1.0/docs/make.bat` & `openthaigpt-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `openthaigpt-0.1.0/setup.py` & `openthaigpt-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     include_package_data=True,
     keywords='openthaigpt',
     name='openthaigpt',
     packages=find_packages(include=['openthaigpt', 'openthaigpt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/OpenThaiGPT/openthaigpt',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `openthaigpt-0.1.0/tests/test_openthaigpt.py` & `openthaigpt-0.1.1/tests/test_openthaigpt.py`

 * *Files identical despite different names*


# Comparing `tmp/py_bugs_open_ai-0.1.1.tar.gz` & `tmp/py_bugs_open_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_bugs_open_ai-0.1.1.tar", last modified: Tue May 23 21:24:46 2023, max compression
+gzip compressed data, was "py_bugs_open_ai-0.1.2.tar", last modified: Fri May 26 18:32:08 2023, max compression
```

## Comparing `py_bugs_open_ai-0.1.1.tar` & `py_bugs_open_ai-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/py_bugs_open_ai/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/open_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/open_ai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai/py_bugs_open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 21:24:46.000000 py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 21:24:46.533336 py_bugs_open_ai-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 21:24:37.000000 py_bugs_open_ai-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/py_bugs_open_ai/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/open_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/open_ai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai/py_bugs_open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 18:32:08.000000 py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-26 18:32:08.414562 py_bugs_open_ai-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-26 18:31:52.000000 py_bugs_open_ai-0.1.2/setup_constants.py
```

### Comparing `py_bugs_open_ai-0.1.1/LICENSE` & `py_bugs_open_ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/PKG-INFO` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_bugs_open_ai
-Version: 0.1.1
+Name: py-bugs-open-ai
+Version: 0.1.2
 Summary: A utility to help use OpenAI to find bugs in large projects or git diffs in python code.  Makes heavy use of caching to save time/money
 Home-page: https://github.com/valmikirao/py_bugs_open_ai
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: GNU General Public License v3
 Keywords: py_bugs_open_ai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,14 +23,16 @@
 # Python Bugs OpenAI
 
 ![version](https://img.shields.io/pypi/v/py_bugs_open_ai)
 ![python versions](https://img.shields.io/pypi/pyversions/py_bugs_open_ai)
 ![build](https://img.shields.io/github/actions/workflow/status/valmikirao/py_bugs_open_ai/push-workflow.yml?branch=master)
 
 * Free software: GNU General Public License v3
+* Note for Python 3.8 and MacOS: I can't get this to work on my local machine with this combination, but it seems to
+ work in ubuntu, so I'm keeping this as working for Python 3.8
 
 A utility to help use OpenAI to find bugs in large projects or git diffs in python code.  Makes heavy use of caching to save time/money
 
 # Table of Contents
 
 1. [Installation](#Installation)
 2. [Usage](#Usage)
```

### Comparing `py_bugs_open_ai-0.1.1/README.md` & `py_bugs_open_ai-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Python Bugs OpenAI
 
 ![version](https://img.shields.io/pypi/v/py_bugs_open_ai)
 ![python versions](https://img.shields.io/pypi/pyversions/py_bugs_open_ai)
 ![build](https://img.shields.io/github/actions/workflow/status/valmikirao/py_bugs_open_ai/push-workflow.yml?branch=master)
 
 * Free software: GNU General Public License v3
+* Note for Python 3.8 and MacOS: I can't get this to work on my local machine with this combination, but it seems to
+ work in ubuntu, so I'm keeping this as working for Python 3.8
 
 A utility to help use OpenAI to find bugs in large projects or git diffs in python code.  Makes heavy use of caching to save time/money
 
 # Table of Contents
 
 1. [Installation](#Installation)
 2. [Usage](#Usage)
```

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/cli.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/cli.py`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/constants.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import importlib
 import os
-import sys
 from typing import Final
 
 DEFAULT_MODEL: Final[str] = 'gpt-3.5-turbo'
 DEFAULT_MAX_CHUNK_SIZE: Final[int] = 500
 OPEN_AI_API_KEY: Final[str] = 'OPEN_AI_API_KEY'
 _home = os.environ.get('HOME', os.path.join(os.path.abspath(os.sep), 'etc'))
 DEFAULT_CACHE: Final[str] = os.path.join(_home, '.pybugsai', 'cache')
@@ -19,36 +17,24 @@
 ERROR_OUT: Final[str] = '\033[91merror\033[0m'  # red "error"
 WARN_OUT: Final[str] = '\033[93mwarning\033[0m'  # yellow "warning"
 OK_OUT: Final[str] = '\033[92mok\033[0m'  # green "ok"
 SKIP_OUT: Final[str] = '\033[93mskip\033[0m'  # yellow "skip"
 NOT_IN_DIFF_OUT: Final[str] = '\033[93mnot in diff\033[0m'  # yellow "skip"
 EMBEDDINGS_REQUEST_CHUNK_SIZE: Final[int] = 1000
 DEFAULT_EMBEDDINGS_MODEL = 'text-embedding-ada-002'
+SHORT_DESCRIPTION: Final[str] = 'A utility to help use OpenAI to find bugs in large projects or git diffs in python' \
+                                ' code.  Makes heavy use of caching to save time/money'
+LICENSE: Final[str] = 'GNU General Public License v3'
+CLI_NAME: Final[str] = 'pybugsai'
+VERSION: Final[str] = '0.1.2'
+AUTHOR: Final[str] = 'Valmiki Rao'
+AUTHOR_EMAIL: Final[str] = 'valmikirao@gmail.com'
 
 
 def get_root_dir() -> str:
     abs_file = os.path.abspath(__file__)
     dirname = os.path.dirname(abs_file)
     root_dir, _ = os.path.split(dirname)
     return root_dir
 
 
 ROOT_DIR: Final[str] = get_root_dir()
-
-
-def get_setup_constants_module():
-    setup_constants_path = os.path.join(ROOT_DIR, 'setup_constants.py')
-    spec = importlib.util.spec_from_file_location("setup_constants", setup_constants_path)
-    module = importlib.util.module_from_spec(spec)
-    sys.modules["setup_constants"] = module
-    spec.loader.exec_module(module)
-    return module
-
-
-setup_constants = get_setup_constants_module()
-
-SHORT_DESCRIPTION: Final[str] = setup_constants.SHORT_DESCRIPTION
-LICENSE: Final[str] = setup_constants.LICENSE
-CLI_NAME: Final[str] = setup_constants.CLI_NAME
-VERSION: Final[str] = setup_constants.VERSION
-AUTHOR: Final[str] = setup_constants.AUTHOR
-AUTHOR_EMAIL: Final[str] = setup_constants.AUTHOR_EMAIL
```

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/diff.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/diff.py`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/models/open_ai.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/models/open_ai.py`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/open_ai_client.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/open_ai_client.py`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai/py_bugs_open_ai.py` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai/py_bugs_open_ai.py`

 * *Files identical despite different names*

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/PKG-INFO` & `py_bugs_open_ai-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-bugs-open-ai
-Version: 0.1.1
+Name: py_bugs_open_ai
+Version: 0.1.2
 Summary: A utility to help use OpenAI to find bugs in large projects or git diffs in python code.  Makes heavy use of caching to save time/money
 Home-page: https://github.com/valmikirao/py_bugs_open_ai
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: GNU General Public License v3
 Keywords: py_bugs_open_ai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,14 +23,16 @@
 # Python Bugs OpenAI
 
 ![version](https://img.shields.io/pypi/v/py_bugs_open_ai)
 ![python versions](https://img.shields.io/pypi/pyversions/py_bugs_open_ai)
 ![build](https://img.shields.io/github/actions/workflow/status/valmikirao/py_bugs_open_ai/push-workflow.yml?branch=master)
 
 * Free software: GNU General Public License v3
+* Note for Python 3.8 and MacOS: I can't get this to work on my local machine with this combination, but it seems to
+ work in ubuntu, so I'm keeping this as working for Python 3.8
 
 A utility to help use OpenAI to find bugs in large projects or git diffs in python code.  Makes heavy use of caching to save time/money
 
 # Table of Contents
 
 1. [Installation](#Installation)
 2. [Usage](#Usage)
```

### Comparing `py_bugs_open_ai-0.1.1/py_bugs_open_ai.egg-info/SOURCES.txt` & `py_bugs_open_ai-0.1.2/py_bugs_open_ai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+setup_constants.py
 py_bugs_open_ai/__init__.py
 py_bugs_open_ai/cli.py
 py_bugs_open_ai/constants.py
 py_bugs_open_ai/diff.py
 py_bugs_open_ai/open_ai_client.py
 py_bugs_open_ai/py_bugs_open_ai.py
 py_bugs_open_ai.egg-info/PKG-INFO
```

### Comparing `py_bugs_open_ai-0.1.1/setup.py` & `py_bugs_open_ai-0.1.2/setup.py`

 * *Files identical despite different names*


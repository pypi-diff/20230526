# Comparing `tmp/freeGPT-1.1.2.tar.gz` & `tmp/freeGPT-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-o5talkyl\freeGPT-1.1.2.tar", last modified: Fri May 26 12:49:19 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-4bhwh_th\freeGPT-1.1.3.tar", last modified: Fri May 26 13:20:15 2023, max compression
```

## Comparing `freeGPT-1.1.2.tar` & `freeGPT-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.106953 freeGPT-1.1.2/
--rw-rw-rw-   0        0        0    35149 2023-05-26 12:48:24.000000 freeGPT-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-26 12:48:24.000000 freeGPT-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2958 2023-05-26 12:49:19.104966 freeGPT-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-26 12:48:24.000000 freeGPT-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.097951 freeGPT-1.1.2/freeGPT/
--rw-rw-rw-   0        0        0     1868 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.102966 freeGPT-1.1.2/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5177 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.103952 freeGPT-1.1.2/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6915 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.102966 freeGPT-1.1.2/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     2958 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 12:49:19.107966 freeGPT-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-05-26 12:48:24.000000 freeGPT-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/
+-rw-rw-rw-   0        0        0    35149 2023-05-26 13:18:55.000000 freeGPT-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-26 13:18:55.000000 freeGPT-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2958 2023-05-26 13:20:15.886983 freeGPT-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-26 13:18:55.000000 freeGPT-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.871358 freeGPT-1.1.3/freeGPT/
+-rw-rw-rw-   0        0        0     1868 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5181 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6915 2023-05-26 13:18:55.000000 freeGPT-1.1.3/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 13:20:15.886983 freeGPT-1.1.3/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     2958 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 13:20:15.000000 freeGPT-1.1.3/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 13:20:15.886983 freeGPT-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-05-26 13:18:55.000000 freeGPT-1.1.3/setup.py
```

### Comparing `freeGPT-1.1.2/LICENSE` & `freeGPT-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.2/PKG-INFO` & `freeGPT-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.2
+Version: 1.1.3
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.1.2/README.md` & `freeGPT-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.2/freeGPT/__init__.py` & `freeGPT-1.1.3/freeGPT/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt4
 
 __author__ = "Ruu3f"
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
 
     GPT3 = "gpt3"
```

### Comparing `freeGPT-1.1.2/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.3/freeGPT/gpt3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, re, json
 
 try:
     from tls_client import Session
 except:
     os.system("pip install tls_client --no-cache-dir")
 from uuid import uuid4
-from pydantic import BaseMaodel
+from pydantic import BaseModel
 from fake_useragent import UserAgent
 from typing import Optional, List, Dict, Any
 
 
 class Completion:
     """A class that provides methods for creating completion requests."""
 
@@ -20,15 +20,15 @@
         count: int = 10,
         safe_search: str = "Moderate",
         on_shopping_page: bool = False,
         mkt: str = "",
         response_filter: str = "WebPages,Translations,TimeZone,Computation,RelatedSearches",
         domain: str = "youchat",
         query_trace_id: str = None,
-        chat: list = None,
+        chat: List[str] = None,
         include_links: bool = False,
         detailed: bool = False,
         proxy: Optional[str] = None,
     ) -> dict:
         """
         Creates a completion request.
```

### Comparing `freeGPT-1.1.2/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.3/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.2/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.3/freeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.2
+Version: 1.1.3
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.1.2/setup.py` & `freeGPT-1.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.2",
+    version="1.1.3",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```


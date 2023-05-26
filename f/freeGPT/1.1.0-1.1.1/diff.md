# Comparing `tmp/freeGPT-1.1.0.tar.gz` & `tmp/freeGPT-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-fhwkn9co\freeGPT-1.1.0.tar", last modified: Thu May 25 17:45:34 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-r66mluya\freeGPT-1.1.1.tar", last modified: Fri May 26 12:39:28 2023, max compression
```

## Comparing `freeGPT-1.1.0.tar` & `freeGPT-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.641065 freeGPT-1.1.0/
--rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:45:34.641065 freeGPT-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/
--rw-rw-rw-   0        0        0     1336 2023-05-25 17:39:20.000000 freeGPT-1.1.0/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2208 2023-05-25 17:41:54.000000 freeGPT-1.1.0/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt3web/
--rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt3web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT/gpt4web/
--rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.1.0/freeGPT/gpt4web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 17:45:34.625460 freeGPT-1.1.0/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 17:45:34.000000 freeGPT-1.1.0/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 17:45:34.641065 freeGPT-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-05-25 17:38:18.000000 freeGPT-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/
+-rw-rw-rw-   0        0        0    35149 2023-05-26 12:31:10.000000 freeGPT-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-26 12:31:10.000000 freeGPT-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2948 2023-05-26 12:39:28.888371 freeGPT-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1943 2023-05-26 12:31:10.000000 freeGPT-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.872747 freeGPT-1.1.1/freeGPT/
+-rw-rw-rw-   0        0        0     1867 2023-05-26 12:38:52.000000 freeGPT-1.1.1/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5177 2023-05-26 12:31:10.000000 freeGPT-1.1.1/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6915 2023-05-26 12:31:10.000000 freeGPT-1.1.1/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     2948 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:39:28.888371 freeGPT-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-05-26 12:34:57.000000 freeGPT-1.1.1/setup.py
```

### Comparing `freeGPT-1.1.0/LICENSE` & `freeGPT-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.0/PKG-INFO` & `freeGPT-1.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.0
+Version: 1.1.1
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -29,51 +29,52 @@
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
-| gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3web           | [you.com](https://you.com)               |
-| gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
+| gpt3              | [you.com](https://you.com)               |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [x] Add a internet search model for GPT-3 & GPT-4
+- [x] Make GPT-3 & GPT-4 models with web access.
 - [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
+from freeGPT import gpt3
 
-prompt = input("👦 > ")
-resp = gpt3.Completion.create(prompt=prompt)
-print(f"🤖 > {resp.text}")
+while True:
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt)
+    print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
+# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
+from freeGPT import gpt4
 
-token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
-prompt = input("👦 > ")
-resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
-print(f"🤖 > {resp.text}")
+while True:
+    token = Account.create(logging=True)
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt, token=token)
+    print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.0/README.md` & `freeGPT-1.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,51 +7,52 @@
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
-| gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3web           | [you.com](https://you.com)               |
-| gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
+| gpt3              | [you.com](https://you.com)               |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [x] Add a internet search model for GPT-3 & GPT-4
+- [x] Make GPT-3 & GPT-4 models with web access.
 - [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
+from freeGPT import gpt3
 
-prompt = input("👦 > ")
-resp = gpt3.Completion.create(prompt=prompt)
-print(f"🤖 > {resp.text}")
+while True:
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt)
+    print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
+# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
+from freeGPT import gpt4
 
-token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
-prompt = input("👦 > ")
-resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
-print(f"🤖 > {resp.text}")
+while True:
+    token = Account.create(logging=True)
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt, token=token)
+    print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.0/freeGPT/gpt3web/__init__.py` & `freeGPT-1.1.1/freeGPT/gpt3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, re, json
 
 try:
     from tls_client import Session
 except:
     os.system("pip install tls_client --no-cache-dir")
 from uuid import uuid4
-from pydantic import BaseModel
+from pydantic import BaseMaodel
 from fake_useragent import UserAgent
 from typing import Optional, List, Dict, Any
 
 
 class Completion:
     """A class that provides methods for creating completion requests."""
```

### Comparing `freeGPT-1.1.0/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.1/freeGPT.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.0
+Version: 1.1.1
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -29,51 +29,52 @@
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
-| gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3web           | [you.com](https://you.com)               |
-| gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
+| gpt3              | [you.com](https://you.com)               |
+| gpt4              | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
-- [x] Add a internet search model for GPT-3 & GPT-4
+- [x] Make GPT-3 & GPT-4 models with web access.
 - [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
+from freeGPT import gpt3
 
-prompt = input("👦 > ")
-resp = gpt3.Completion.create(prompt=prompt)
-print(f"🤖 > {resp.text}")
+while True:
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt)
+    print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
+# Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
+from freeGPT import gpt4
 
-token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
-prompt = input("👦 > ")
-resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
-print(f"🤖 > {resp.text}")
+while True:
+    token = Account.create(logging=True)
+    prompt = input("👦 > ")
+    resp = Completion.create(prompt=prompt, token=token)
+    print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.0/setup.py` & `freeGPT-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.0",
+    version="1.1.1",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```


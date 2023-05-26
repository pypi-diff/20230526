# Comparing `tmp/freeGPT-1.1.1.tar.gz` & `tmp/freeGPT-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-r66mluya\freeGPT-1.1.1.tar", last modified: Fri May 26 12:39:28 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-o5talkyl\freeGPT-1.1.2.tar", last modified: Fri May 26 12:49:19 2023, max compression
```

## Comparing `freeGPT-1.1.1.tar` & `freeGPT-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/
--rw-rw-rw-   0        0        0    35149 2023-05-26 12:31:10.000000 freeGPT-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-26 12:31:10.000000 freeGPT-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2948 2023-05-26 12:39:28.888371 freeGPT-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1943 2023-05-26 12:31:10.000000 freeGPT-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.872747 freeGPT-1.1.1/freeGPT/
--rw-rw-rw-   0        0        0     1867 2023-05-26 12:38:52.000000 freeGPT-1.1.1/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5177 2023-05-26 12:31:10.000000 freeGPT-1.1.1/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     6915 2023-05-26 12:31:10.000000 freeGPT-1.1.1/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:39:28.888371 freeGPT-1.1.1/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     2948 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 12:39:28.000000 freeGPT-1.1.1/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 12:39:28.888371 freeGPT-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1416 2023-05-26 12:34:57.000000 freeGPT-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.106953 freeGPT-1.1.2/
+-rw-rw-rw-   0        0        0    35149 2023-05-26 12:48:24.000000 freeGPT-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-26 12:48:24.000000 freeGPT-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2958 2023-05-26 12:49:19.104966 freeGPT-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-05-26 12:48:24.000000 freeGPT-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.097951 freeGPT-1.1.2/freeGPT/
+-rw-rw-rw-   0        0        0     1868 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.102966 freeGPT-1.1.2/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     5177 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.103952 freeGPT-1.1.2/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     6915 2023-05-26 12:48:24.000000 freeGPT-1.1.2/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:49:19.102966 freeGPT-1.1.2/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     2958 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 12:49:19.000000 freeGPT-1.1.2/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:49:19.107966 freeGPT-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2023-05-26 12:48:24.000000 freeGPT-1.1.2/setup.py
```

### Comparing `freeGPT-1.1.1/LICENSE` & `freeGPT-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.1/PKG-INFO` & `freeGPT-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.1
+Version: 1.1.2
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -55,26 +55,26 @@
 #### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt)
+    resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt, token=token)
+    resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.1/README.md` & `freeGPT-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 #### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt)
+    resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt, token=token)
+    resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.1/freeGPT/__init__.py` & `freeGPT-1.1.2/freeGPT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from freeGPT import gpt3, gpt4
 
 __author__ = "Ruu3f"
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __all__ = ["Provider", "Completion"]
 
 
 class Provider(Enum):
     """Enum class representing the available GPT providers."""
 
     GPT3 = "gpt3"
@@ -60,8 +60,8 @@
 
         Args:
             prompt (str): The prompt text for completion.
 
         Returns:
             str: The generated completion text.
         """
-        return gpt4.Completion.create(prompt=prompt).text
+        return gpt4.Completion.create(prompt=prompt).text
```

### Comparing `freeGPT-1.1.1/freeGPT/gpt3/__init__.py` & `freeGPT-1.1.2/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.1/freeGPT/gpt4/__init__.py` & `freeGPT-1.1.2/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.1/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.1.2/freeGPT.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.1
+Version: 1.1.2
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -55,26 +55,26 @@
 #### GPT-3:
 
 ```python
 from freeGPT import gpt3
 
 while True:
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt)
+    resp = gpt3.Completion.create(prompt=prompt)
     print(f"🤖 > {resp['text']}")
 ```
 #### GPT-4:
 
 ```python
 # Uhh, sorry but gpt4 is kinda broken currently, will maybe get fixed in the next update.
 from freeGPT import gpt4
 
 while True:
     token = Account.create(logging=True)
     prompt = input("👦 > ")
-    resp = Completion.create(prompt=prompt, token=token)
+    resp = gpt4.Completion.create(prompt=prompt, token=token)
     print(f"🤖 > {resp.text}")
 ```
 
 ## Star History:
 [![Star History Chart](https://api.star-history.com/svg?repos=Ruu3f/freeGPT&type=Date)](https://github.com/Ruu3f/freeGPT/stargazers)
```

### Comparing `freeGPT-1.1.1/setup.py` & `freeGPT-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.1",
+    version="1.1.2",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```


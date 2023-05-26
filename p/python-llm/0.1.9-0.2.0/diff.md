# Comparing `tmp/python-llm-0.1.9.tar.gz` & `tmp/python-llm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-llm-0.1.9.tar", last modified: Sun May 21 16:31:29 2023, max compression
+gzip compressed data, was "python-llm-0.2.0.tar", last modified: Fri May 26 13:45:56 2023, max compression
```

## Comparing `python-llm-0.1.9.tar` & `python-llm-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.318094 python-llm-0.1.9/
--rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.1.9/LICENSE
--rw-r--r--   0 danielgross   (501) staff       (20)       24 2023-05-21 11:54:44.000000 python-llm-0.1.9/MANIFEST.in
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 16:31:29.317988 python-llm-0.1.9/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.1.9/README.md
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.316157 python-llm-0.1.9/llm/
--rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.1.9/llm/__init__.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.316466 python-llm-0.1.9/llm/api/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.1.9/llm/api/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2493 2023-05-21 16:00:40.000000 python-llm-0.1.9/llm/api/anthropicapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3262 2023-05-21 16:19:37.000000 python-llm-0.1.9/llm/api/openaiapi.py
--rw-r--r--   0 danielgross   (501) staff       (20)     4686 2023-05-21 15:27:54.000000 python-llm-0.1.9/llm/main.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.316792 python-llm-0.1.9/llm/utils/
--rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.1.9/llm/utils/__init__.py
--rw-r--r--   0 danielgross   (501) staff       (20)     3200 2023-05-20 11:56:01.000000 python-llm-0.1.9/llm/utils/apikeys.py
--rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.1.9/llm/utils/parsing.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.317510 python-llm-0.1.9/python_llm.egg-info/
--rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-21 16:31:29.000000 python-llm-0.1.9/python_llm.egg-info/PKG-INFO
--rw-r--r--   0 danielgross   (501) staff       (20)      453 2023-05-21 16:31:29.000000 python-llm-0.1.9/python_llm.egg-info/SOURCES.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-21 16:31:29.000000 python-llm-0.1.9/python_llm.egg-info/dependency_links.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      533 2023-05-21 16:31:29.000000 python-llm-0.1.9/python_llm.egg-info/requires.txt
--rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-21 16:31:29.000000 python-llm-0.1.9/python_llm.egg-info/top_level.txt
--rw-r--r--   0 danielgross   (501) staff       (20)      533 2023-05-21 15:29:28.000000 python-llm-0.1.9/requirements.txt
--rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-21 16:31:29.318126 python-llm-0.1.9/setup.cfg
--rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-21 16:31:09.000000 python-llm-0.1.9/setup.py
-drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-21 16:31:29.317845 python-llm-0.1.9/tests/
--rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.1.9/tests/test_anthropic.py
--rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.1.9/tests/test_multi_stream.py
--rw-r--r--   0 danielgross   (501) staff       (20)     4761 2023-05-21 15:57:30.000000 python-llm-0.1.9/tests/test_openai.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.373018 python-llm-0.2.0/
+-rw-r--r--   0 danielgross   (501) staff       (20)     1069 2023-03-30 14:06:17.000000 python-llm-0.2.0/LICENSE
+-rw-r--r--   0 danielgross   (501) staff       (20)       24 2023-05-21 11:54:44.000000 python-llm-0.2.0/MANIFEST.in
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-26 13:45:56.372880 python-llm-0.2.0/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)     2342 2023-05-20 19:12:04.000000 python-llm-0.2.0/README.md
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.370420 python-llm-0.2.0/llm/
+-rw-r--r--   0 danielgross   (501) staff       (20)       81 2023-05-20 15:11:39.000000 python-llm-0.2.0/llm/__init__.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.370831 python-llm-0.2.0/llm/api/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-03-29 19:17:50.000000 python-llm-0.2.0/llm/api/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2493 2023-05-21 16:00:40.000000 python-llm-0.2.0/llm/api/anthropicapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3259 2023-05-26 13:43:35.000000 python-llm-0.2.0/llm/api/openaiapi.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     4686 2023-05-21 15:27:54.000000 python-llm-0.2.0/llm/main.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.371240 python-llm-0.2.0/llm/utils/
+-rw-r--r--   0 danielgross   (501) staff       (20)        0 2023-05-20 11:50:33.000000 python-llm-0.2.0/llm/utils/__init__.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     3236 2023-05-26 13:43:11.000000 python-llm-0.2.0/llm/utils/apikeys.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     2441 2023-05-20 19:38:17.000000 python-llm-0.2.0/llm/utils/parsing.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.372218 python-llm-0.2.0/python_llm.egg-info/
+-rw-r--r--   0 danielgross   (501) staff       (20)     2619 2023-05-26 13:45:56.000000 python-llm-0.2.0/python_llm.egg-info/PKG-INFO
+-rw-r--r--   0 danielgross   (501) staff       (20)      453 2023-05-26 13:45:56.000000 python-llm-0.2.0/python_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        1 2023-05-26 13:45:56.000000 python-llm-0.2.0/python_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      533 2023-05-26 13:45:56.000000 python-llm-0.2.0/python_llm.egg-info/requires.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)        4 2023-05-26 13:45:56.000000 python-llm-0.2.0/python_llm.egg-info/top_level.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)      533 2023-05-21 15:29:28.000000 python-llm-0.2.0/requirements.txt
+-rw-r--r--   0 danielgross   (501) staff       (20)       38 2023-05-26 13:45:56.373067 python-llm-0.2.0/setup.cfg
+-rw-r--r--   0 danielgross   (501) staff       (20)      650 2023-05-26 13:45:42.000000 python-llm-0.2.0/setup.py
+drwxr-xr-x   0 danielgross   (501) staff       (20)        0 2023-05-26 13:45:56.372681 python-llm-0.2.0/tests/
+-rw-r--r--   0 danielgross   (501) staff       (20)     3407 2023-05-20 19:49:17.000000 python-llm-0.2.0/tests/test_anthropic.py
+-rw-r--r--   0 danielgross   (501) staff       (20)      945 2023-05-20 19:51:00.000000 python-llm-0.2.0/tests/test_multi_stream.py
+-rw-r--r--   0 danielgross   (501) staff       (20)     4761 2023-05-21 15:57:30.000000 python-llm-0.2.0/tests/test_openai.py
```

### Comparing `python-llm-0.1.9/LICENSE` & `python-llm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/PKG-INFO` & `python-llm-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.9
+Version: 0.2.0
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.9/README.md` & `python-llm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/llm/api/anthropicapi.py` & `python-llm-0.2.0/llm/api/anthropicapi.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/llm/api/openaiapi.py` & `python-llm-0.2.0/llm/api/openaiapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return enc.decode(tokens)
     return text
 
 
 def complete(prompt, engine, prompt_overflow=None, **kwargs):
     """Complete text using the OpenAI API."""
     if prompt_overflow == "trim":
-        logging.debug(f"Trimming overflow for {engine}")
+        logger.debug(f"Trimming overflow for {engine}")
         prompt = _trim_overflow(prompt, engine)
 
     if engine.startswith("gpt-3.5") or engine.startswith("gpt-4"):
         return chat(structure_chat([prompt]), engine=engine, **kwargs)
     logger.debug(f"Completing with {engine} using prompt: {prompt}")
     return openai.Completion.create(
         engine=engine,
@@ -50,15 +50,15 @@
         **kwargs
     ).choices[0].text
 
 
 def chat(messages, engine, system=None, prompt_overflow=None, **kwargs):
     """Chat with the OpenAI API."""
     if prompt_overflow == "trim":
-        logging.debug(f"Trimming overflow for {engine}")
+        logger.debug(f"Trimming overflow for {engine}")
         # TODO For now, just trim the last message.
         messages[-1]['content'] = _trim_overflow(
             messages[-1]['content'], engine)
 
     if engine.startswith("text-"):
         raise ValueError(
             f"Cannot issue a ChatCompletion with engine {engine}.")
@@ -72,15 +72,15 @@
     )
     return response.choices[0].message.content
 
 
 async def stream_chat(messages, engine, system=None, prompt_overflow=None, **kwargs):
     """Chat with the OpenAI API."""
     if prompt_overflow == "trim":
-        logging.debug(f"Trimming overflow for {engine}")
+        logger.debug(f"Trimming overflow for {engine}")
         # TODO For now, just trim the last message.
         messages[-1]['content'] = _trim_overflow(
             messages[-1]['content'], engine)
 
     if system is not None:
         messages = [{"role": "system", "content": system}] + messages
     logger.debug(f"Chatting with {engine} using messages: {messages}")
```

### Comparing `python-llm-0.1.9/llm/main.py` & `python-llm-0.2.0/llm/main.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/llm/utils/apikeys.py` & `python-llm-0.2.0/llm/utils/apikeys.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 py_llm_dir = os.path.join(os.path.expanduser('~'), ".python-llm")
 env_path = os.path.join(py_llm_dir, "apikeys.env")
 
 # Supported apis and memory
 supported_apis = ["openai", "anthropic"]
 api_keys = {}
 
+logger = logging.getLogger(__name__)
+
 
 # --- public interface ---
 
 def configure_api_keys(*args, **kwargs) -> None:
     """Configure the API keys. Call me like this:
     - llm.set_api_keys(openai="sk-...")
     - llm.set_api_keys("path/to/api_keys.json")
@@ -48,15 +50,15 @@
     _sync_keys_with_apis()
 
 
 def load_keys_from_cache() -> int:
     """Load API keys from the disk cache."""
     load_dotenv(env_path)  # from cache to os environment
     num_keys = _load_keys_from_env()  #  load keys from os env
-    logging.debug(f"Loaded {num_keys} api keys from cache"
+    logger.debug(f"Loaded {num_keys} api keys from cache"
                   if num_keys else "api keys env cache does not exist")
 
 
 # --- private related to key management ---
 
 def _update_keys_memory(keys: dict) -> None:
     """Update the API keys memory."""
@@ -70,15 +72,15 @@
         if api not in supported_apis:
             raise ValueError(f"API {api} not supported.")
 
 
 def _sync_keys_with_apis() -> None:
     """Update the API keys from the environment."""
     import openai
-    logging.debug(f"Setting OpenAI API key to {api_keys.get('openai')}")
+    logger.debug(f"Setting OpenAI API key to {api_keys.get('openai')}")
     openai.api_key = api_keys.get("openai")
 
 
 # --- private related to key cache ---
 
 def _save_keys_to_cache(filepath: str = env_path) -> None:
     """Save API keys to the disk cache."""
```

### Comparing `python-llm-0.1.9/llm/utils/parsing.py` & `python-llm-0.2.0/llm/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/python_llm.egg-info/PKG-INFO` & `python-llm-0.2.0/python_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-llm
-Version: 0.1.9
+Version: 0.2.0
 Summary: An LLM wrapper for Humans
 Home-page: https://github.com/danielgross/python-llm
 Author: Daniel Gross
 Author-email: d@dcgross.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-llm-0.1.9/python_llm.egg-info/requires.txt` & `python-llm-0.2.0/python_llm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/requirements.txt` & `python-llm-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/setup.py` & `python-llm-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='python-llm',
-    version='0.1.9',
+    version='0.2.0',
     author='Daniel Gross',
     author_email='d@dcgross.com',
     description='An LLM wrapper for Humans',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(include=['llm', 'llm.*']),
     url="https://github.com/danielgross/python-llm",
```

### Comparing `python-llm-0.1.9/tests/test_anthropic.py` & `python-llm-0.2.0/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/tests/test_multi_stream.py` & `python-llm-0.2.0/tests/test_multi_stream.py`

 * *Files identical despite different names*

### Comparing `python-llm-0.1.9/tests/test_openai.py` & `python-llm-0.2.0/tests/test_openai.py`

 * *Files identical despite different names*


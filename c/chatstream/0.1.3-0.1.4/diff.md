# Comparing `tmp/chatstream-0.1.3.tar.gz` & `tmp/chatstream-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatstream-0.1.3.tar", last modified: Mon May 22 04:54:09 2023, max compression
+gzip compressed data, was "chatstream-0.1.4.tar", last modified: Fri May 26 02:36:51 2023, max compression
```

## Comparing `chatstream-0.1.3.tar` & `chatstream-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.835131 chatstream-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.769747 chatstream-0.1.3/ChatStream.egg-info/
--rw-rw-rw-   0        0        0     7337 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 04:54:09.000000 chatstream-0.1.3/ChatStream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     7337 2023-05-22 04:54:09.835131 chatstream-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6485 2023-05-22 04:52:49.000000 chatstream-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.828133 chatstream-0.1.3/chatstream/
--rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/__init__.py
--rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_core.py
--rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_process.py
--rw-rw-rw-   0        0        0     2644 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/chat_process_mock.py
--rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.3/chatstream/chat_prompt.py
--rw-rw-rw-   0        0        0    20904 2023-05-22 00:16:49.000000 chatstream-0.1.3/chatstream/chat_stream.py
--rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/mock_response_example_text.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:54:09.834129 chatstream-0.1.3/chatstream/request_handler/
--rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/request_handler.py
--rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/request_handler/simple_session_request_handler.py
--rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/sampling_utils.py
--rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.3/chatstream/util_request_id.py
--rw-rw-rw-   0        0        0       42 2023-05-22 04:54:09.835131 chatstream-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-05-22 04:53:08.000000 chatstream-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.025482 chatstream-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.014081 chatstream-0.1.4/ChatStream.egg-info/
+-rw-rw-rw-   0        0        0     7337 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 02:36:50.000000 chatstream-0.1.4/ChatStream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11356 2023-05-21 23:57:09.000000 chatstream-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7337 2023-05-26 02:36:51.024483 chatstream-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6485 2023-05-22 04:52:49.000000 chatstream-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.021482 chatstream-0.1.4/chatstream/
+-rw-rw-rw-   0        0        0      168 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/__init__.py
+-rw-rw-rw-   0        0        0     8430 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/chat_core.py
+-rw-rw-rw-   0        0        0     8648 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/chat_process.py
+-rw-rw-rw-   0        0        0     2907 2023-05-26 02:27:29.000000 chatstream-0.1.4/chatstream/chat_process_mock.py
+-rw-rw-rw-   0        0        0     6416 2023-05-22 01:34:57.000000 chatstream-0.1.4/chatstream/chat_prompt.py
+-rw-rw-rw-   0        0        0    20900 2023-05-26 02:24:23.000000 chatstream-0.1.4/chatstream/chat_stream.py
+-rw-rw-rw-   0        0        0     3146 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/mock_response_example_text.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:51.024483 chatstream-0.1.4/chatstream/request_handler/
+-rw-rw-rw-   0        0        0        0 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/request_handler.py
+-rw-rw-rw-   0        0        0     4916 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/request_handler/simple_session_request_handler.py
+-rw-rw-rw-   0        0        0     3356 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/sampling_utils.py
+-rw-rw-rw-   0        0        0      803 2023-05-21 23:57:09.000000 chatstream-0.1.4/chatstream/util_request_id.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 02:36:51.025482 chatstream-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-05-26 02:33:07.000000 chatstream-0.1.4/setup.py
```

### Comparing `chatstream-0.1.3/ChatStream.egg-info/PKG-INFO` & `chatstream-0.1.4/ChatStream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chatstream-0.1.3/ChatStream.egg-info/SOURCES.txt` & `chatstream-0.1.4/ChatStream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/LICENSE` & `chatstream-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/PKG-INFO` & `chatstream-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstream
-Version: 0.1.3
+Version: 0.1.4
 Summary: Streaming chat server building blocks for FastAPI/Starlette
 Home-page: https://github.com/riversun/ChatStream
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `chatstream-0.1.3/README.md` & `chatstream-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/chat_core.py` & `chatstream-0.1.4/chatstream/chat_core.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/chat_process.py` & `chatstream-0.1.4/chatstream/chat_process.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/chat_process_mock.py` & `chatstream-0.1.4/chatstream/chat_process_mock.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,36 +23,42 @@
             if chat_prompt.is_chat_mode_enabled():
                 stop_strs = chat_prompt.get_stop_strs()
             else:
                 stop_strs = None
 
             self.params["stop_strs"] = stop_strs
 
-            if self.params.get("mock_type") == "round":
+            time_per_token_sec = self.params.get("time_per_token_sec", 0.1)
+            initial_wait_sec = self.params.get("initial_wait_sec", 0)
+
+
+            if self.params.get("type") == "round":
                 line = sample_text_array[(chat_prompt.get_turn() - 1) % len(
                     sample_text_array)]
             else:
                 line = sample_text_long
 
             tokens = line.split(' ')
             resp_text = ""
 
             prev = ""
             for index, updated_text in enumerate(tokens):
                 if index == 0:
                     resp_text += updated_text
+                    if initial_wait_sec>0:
+                        await asyncio.sleep(initial_wait_sec)
                 else:
                     resp_text += " " + updated_text
 
                 updated_text = resp_text[len(prev):]
                 pos = "mid"
                 if index == 0:
                     pos = "begin"
 
-                await asyncio.sleep(0.1)  # わずかな遅延を発生させ、逐次返信となるようにする
+                await asyncio.sleep(time_per_token_sec)  # わずかな遅延を発生させ、逐次返信となるようにする
 
                 # 出力タイプごとに出しわける
                 if otype == "updated_text":
                     yield updated_text
                 elif otype == "response_text":
                     yield resp_text
                 else:
```

### Comparing `chatstream-0.1.3/chatstream/chat_prompt.py` & `chatstream-0.1.4/chatstream/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/chat_stream.py` & `chatstream-0.1.4/chatstream/chat_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                  # The number of simultaneous executions for sentence generation tasks in the pre-trained language model
                  max_queue_size: int = 5,
                  # The maximum queue size for sentence generation tasks in the pre-trained language model
                  too_many_request_as_http_error=False,
                  # True: When a 'Too many requests' situation occurs, it returns the status as 429
                  use_mock_response=False,
                  # True: Returns fixed phrases for testing. As it doesn't need to load the model, it starts up immediately
-                 mock_type="round",  # "round" / "long" - The type of phrases to return when use_mock_response=True
+                 mock_params={type:"round"},  # "round" / "long" - The type of phrases to return when use_mock_response=True
                  chat_prompt_clazz=None,
                  # Specifies the class that manages the prompts sent to the language model. Inherit from AbstractChatPrompt and implement a class that generates chat prompts according to the etiquette of each model
                  max_new_tokens=256,  # The maximum size of the newly generated tokens
                  context_len=1024,  # The size of the context (in terms of the number of tokens)
                  temperature=1.0,  # The temperature value for randomness in prediction
                  top_k=50,  # Value of top K for sampling
                  top_p=1.0,  # Value of top P for sampling
@@ -95,15 +95,15 @@
         self.processing_queue = asyncio.Queue(maxsize=num_of_concurrent_executions)
 
         # コンソールチャット使用時のシングルユーザー用の ChatPrompt
         self.chat_prompt_for_single_user_on_console = None
 
         if use_mock_response:
             self.chat_generator = ChatGeneratorMock(model=None, tokenizer=None, device=None,
-                                                    params={"mock_type": mock_type})
+                                                    params=mock_params)
         else:
             self.chat_generator = ChatGenerator(model, tokenizer, device, chat_params)
 
         # request_handler にパラメータをセット
         request_handler.chat_generator = self.chat_generator
         request_handler.chat_prompt_clazz = self.chat_prompt_clazz
```

### Comparing `chatstream-0.1.3/chatstream/mock_response_example_text.py` & `chatstream-0.1.4/chatstream/mock_response_example_text.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/request_handler/request_handler.py` & `chatstream-0.1.4/chatstream/request_handler/request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/request_handler/simple_session_request_handler.py` & `chatstream-0.1.4/chatstream/request_handler/simple_session_request_handler.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/sampling_utils.py` & `chatstream-0.1.4/chatstream/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/chatstream/util_request_id.py` & `chatstream-0.1.4/chatstream/util_request_id.py`

 * *Files identical despite different names*

### Comparing `chatstream-0.1.3/setup.py` & `chatstream-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chatstream",
-    version="0.1.3",
+    version="0.1.4",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="Streaming chat server building blocks for FastAPI/Starlette",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/ChatStream",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
```


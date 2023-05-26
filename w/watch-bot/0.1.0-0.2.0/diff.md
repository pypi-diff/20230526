# Comparing `tmp/watch-bot-0.1.0.tar.gz` & `tmp/watch-bot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-bot-0.1.0.tar", last modified: Fri May 26 15:50:45 2023, max compression
+gzip compressed data, was "watch-bot-0.2.0.tar", last modified: Fri May 26 15:59:06 2023, max compression
```

## Comparing `watch-bot-0.1.0.tar` & `watch-bot-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.159767 watch-bot-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.147767 watch-bot-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.155767 watch-bot-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-26 15:50:22.000000 watch-bot-0.1.0/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 15:50:22.000000 watch-bot-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-26 15:50:22.000000 watch-bot-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.155767 watch-bot-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 15:50:22.000000 watch-bot-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-26 15:50:22.000000 watch-bot-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:50:22.000000 watch-bot-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 15:50:45.159767 watch-bot-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-26 15:50:22.000000 watch-bot-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 15:50:22.000000 watch-bot-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 15:50:22.000000 watch-bot-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:50:45.159767 watch-bot-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.151767 watch-bot-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.155767 watch-bot-0.1.0/src/watch_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 15:50:22.000000 watch-bot-0.1.0/src/watch_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-26 15:50:22.000000 watch-bot-0.1.0/src/watch_bot/_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 15:50:22.000000 watch-bot-0.1.0/src/watch_bot/_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 15:50:22.000000 watch-bot-0.1.0/src/watch_bot/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 15:50:22.000000 watch-bot-0.1.0/src/watch_bot/prompt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.159767 watch-bot-0.1.0/src/watch_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 15:50:45.000000 watch-bot-0.1.0/src/watch_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-26 15:50:45.000000 watch-bot-0.1.0/src/watch_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:50:45.000000 watch-bot-0.1.0/src/watch_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 15:50:45.000000 watch-bot-0.1.0/src/watch_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:50:45.000000 watch-bot-0.1.0/src/watch_bot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.159767 watch-bot-0.1.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:50:45.159767 watch-bot-0.1.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/data/hack_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/data/hack_prompt_answer.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 15:50:22.000000 watch-bot-0.1.0/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.558635 watch-bot-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-26 15:58:45.000000 watch-bot-0.2.0/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 15:58:45.000000 watch-bot-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-26 15:58:45.000000 watch-bot-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 15:58:45.000000 watch-bot-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-26 15:58:45.000000 watch-bot-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:58:45.000000 watch-bot-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 15:59:06.558635 watch-bot-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-26 15:58:45.000000 watch-bot-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 15:58:45.000000 watch-bot-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 15:58:45.000000 watch-bot-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:59:06.558635 watch-bot-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/src/watch_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 15:58:45.000000 watch-bot-0.2.0/src/watch_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-26 15:58:45.000000 watch-bot-0.2.0/src/watch_bot/_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 15:58:45.000000 watch-bot-0.2.0/src/watch_bot/_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-26 15:58:45.000000 watch-bot-0.2.0/src/watch_bot/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 15:58:45.000000 watch-bot-0.2.0/src/watch_bot/prompt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.554635 watch-bot-0.2.0/src/watch_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 15:59:06.000000 watch-bot-0.2.0/src/watch_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-26 15:59:06.000000 watch-bot-0.2.0/src/watch_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:59:06.000000 watch-bot-0.2.0/src/watch_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 15:59:06.000000 watch-bot-0.2.0/src/watch_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:59:06.000000 watch-bot-0.2.0/src/watch_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.558635 watch-bot-0.2.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:59:06.558635 watch-bot-0.2.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/data/hack_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/data/hack_prompt_answer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 15:58:45.000000 watch-bot-0.2.0/test/test_response.py
```

### Comparing `watch-bot-0.1.0/.github/workflows/actions.yml` & `watch-bot-0.2.0/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/.pre-commit-config.yaml` & `watch-bot-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/LICENSE` & `watch-bot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/PKG-INFO` & `watch-bot-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watch-bot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Implementation of the watchbot, to control the behaviour of a LLM-based chatbot
 Author-email: Francesco Calcavecchia <francesco086@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco086@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `watch-bot-0.1.0/README.md` & `watch-bot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/pyproject.toml` & `watch-bot-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/src/watch_bot/_bot.py` & `watch-bot-0.2.0/src/watch_bot/_bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class WatchBot:
     def __init__(self, engine: str, chatbot_instructions: str) -> None:
         self._engine = engine
         self._chatbot_instructions = chatbot_instructions
 
-    def check_dialog(self, dialog: Dialog) -> WatchBotResponse:
+    def verify(self, dialog: Dialog) -> WatchBotResponse:
         answer = self._ask_gpt_if_dialog_is_suspicious(dialog=dialog)
         if "yes" in answer[:5].lower():
             return WatchBotResponse(should_stop=True, reason=answer)
         elif "no" in answer[:5].lower():
             return WatchBotResponse(should_stop=False, reason="")
         else:
             raise ValueError(f"Unexpected answer: {answer}")
```

### Comparing `watch-bot-0.1.0/src/watch_bot/_dialog.py` & `watch-bot-0.2.0/src/watch_bot/_dialog.py`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/src/watch_bot/prompt.template` & `watch-bot-0.2.0/src/watch_bot/prompt.template`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/src/watch_bot.egg-info/PKG-INFO` & `watch-bot-0.2.0/src/watch_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watch-bot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Implementation of the watchbot, to control the behaviour of a LLM-based chatbot
 Author-email: Francesco Calcavecchia <francesco086@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco086@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `watch-bot-0.1.0/src/watch_bot.egg-info/SOURCES.txt` & `watch-bot-0.2.0/src/watch_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/test/data/hack_prompt.txt` & `watch-bot-0.2.0/test/data/hack_prompt.txt`

 * *Files identical despite different names*

### Comparing `watch-bot-0.1.0/test/test_bot.py` & `watch-bot-0.2.0/test/test_bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,32 @@
         )
         self.bot = WatchBot(engine=os.environ["OPENAI_ENGINE"], chatbot_instructions=self.chatbot_instructions)
         openai.api_type = os.environ["OPENAI_API_TYPE"]
         openai.api_version = os.environ["OPENAI_API_VERSION"]
         openai.api_base = os.environ["OPENAI_API_BASE"]
         openai.api_key = os.environ["OPENAI_API_KEY"]
 
-    def test_instance_with_defaults_has_check_dialog_method(self) -> None:
-        self.assertTrue(hasattr(self.bot, "check_dialog"))
+    def test_instance_with_defaults_has_verify_method(self) -> None:
+        self.assertTrue(hasattr(self.bot, "verify"))
 
     def test_build_prompt(self) -> None:
         self.assertTrue(
             '"User": "Hi"\n"Chatbot": "Hello"' in self.bot.build_prompt(dialog=Dialog(messages=["Hi", "Hello"]))
         )
 
     def test_build_prompt_when_messages_contain_double_quotation_mark(self) -> None:
         self.assertTrue(
             '"User": "\'Hi\'"\n"Chatbot": "\'Hello\'"'
             in self.bot.build_prompt(dialog=Dialog(messages=['"Hi"', '"Hello"']))
         )
 
     def test_check_regular_dialog_returns_should_not_stop(self) -> None:
         dialog = Dialog(messages=["Hi", "Hello"])
-        response = self.bot.check_dialog(dialog=dialog)
+        response = self.bot.verify(dialog=dialog)
         self.assertFalse(response.should_stop)
         self.assertEqual(len(response.reason), 0)
 
     def test_check_dialog_with_hack_attack_returns_should_not_stop(self) -> None:
         dialog = Dialog(messages=[read_hack_prompt(), read_hack_prompt_answer()])
-        response = self.bot.check_dialog(dialog=dialog)
+        response = self.bot.verify(dialog=dialog)
         self.assertTrue(response.should_stop)
         self.assertGreater(len(response.reason), 0)
```

### Comparing `watch-bot-0.1.0/test/test_dialog.py` & `watch-bot-0.2.0/test/test_dialog.py`

 * *Files identical despite different names*


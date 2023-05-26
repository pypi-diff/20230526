# Comparing `tmp/oobabot_plugin-0.1.8.tar.gz` & `tmp/oobabot_plugin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot_plugin-0.1.8.tar", max compression
+gzip compressed data, was "oobabot_plugin-0.1.9.tar", max compression
```

## Comparing `oobabot_plugin-0.1.8.tar` & `oobabot_plugin-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-05-21 10:32:26.331669 oobabot_plugin-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2023-05-23 04:56:48.491563 oobabot_plugin-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-23 04:56:48.491490 oobabot_plugin-0.1.8/oobabot_plugin/__init__.py
--rw-r--r--   0        0        0     9455 2023-05-24 00:34:54.207825 oobabot_plugin-0.1.8/oobabot_plugin/controller.py
--rw-r--r--   0        0        0     9027 2023-05-23 20:26:32.725432 oobabot_plugin-0.1.8/oobabot_plugin/input_handlers.py
--rw-r--r--   0        0        0     3145 2023-05-24 00:45:21.798444 oobabot_plugin-0.1.8/oobabot_plugin/install.py
--rw-r--r--   0        0        0      806 2023-05-23 19:56:31.876256 oobabot_plugin-0.1.8/oobabot_plugin/instructions.md
--rw-r--r--   0        0        0     8596 2023-05-24 00:34:43.876076 oobabot_plugin-0.1.8/oobabot_plugin/layout.py
--rw-r--r--   0        0        0     1223 2023-05-23 20:40:18.813416 oobabot_plugin-0.1.8/oobabot_plugin/oobabot_log.css
--rw-r--r--   0        0        0      275 2023-05-23 19:56:48.214517 oobabot_plugin-0.1.8/oobabot_plugin/oobabot_log.js
--rw-r--r--   0        0        0     2691 2023-05-24 00:33:56.561216 oobabot_plugin-0.1.8/oobabot_plugin/script.py
--rw-r--r--   0        0        0     4109 2023-05-23 22:32:41.125243 oobabot_plugin-0.1.8/oobabot_plugin/strings.py
--rw-r--r--   0        0        0     5376 2023-05-24 00:34:46.048481 oobabot_plugin-0.1.8/oobabot_plugin/worker.py
--rw-r--r--   0        0        0     1185 2023-05-24 00:37:21.125548 oobabot_plugin-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 oobabot_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-23 18:45:53.519115 oobabot_plugin-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1951 2023-05-24 06:06:57.334971 oobabot_plugin-0.1.9/README.md
+-rw-r--r--   0        0        0     1181 2023-05-26 18:44:59.392017 oobabot_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-24 16:52:38.642666 oobabot_plugin-0.1.9/src/oobabot_plugin/__init__.py
+-rw-r--r--   0        0        0   920346 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/ace.js
+-rw-r--r--   0        0        0    12073 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_mode_yaml.js
+-rw-r--r--   0        0        0     1572 2023-05-26 18:39:06.122009 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_oobabot.js
+-rw-r--r--   0        0        0     3509 2023-05-26 18:42:31.352014 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_github.js
+-rw-r--r--   0        0        0     3800 2023-05-26 18:42:31.352014 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_github_dark.js
+-rw-r--r--   0        0        0     3511 2023-05-26 18:39:02.492009 oobabot_plugin-0.1.9/src/oobabot_plugin/ace_theme_twilight.js
+-rw-r--r--   0        0        0     7676 2023-05-26 18:40:18.922011 oobabot_plugin-0.1.9/src/oobabot_plugin/bootstrap.py
+-rw-r--r--   0        0        0    16913 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/controller.py
+-rw-r--r--   0        0        0      172 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/editor.html
+-rw-r--r--   0        0        0     9903 2023-05-25 16:33:44.756742 oobabot_plugin-0.1.9/src/oobabot_plugin/input_handlers.py
+-rw-r--r--   0        0        0     3305 2023-05-25 16:33:44.756742 oobabot_plugin-0.1.9/src/oobabot_plugin/install.py
+-rw-r--r--   0        0        0      806 2023-05-23 19:32:11.169051 oobabot_plugin-0.1.9/src/oobabot_plugin/instructions.md
+-rw-r--r--   0        0        0    13529 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/layout.py
+-rw-r--r--   0        0        0     2935 2023-05-26 18:42:15.202013 oobabot_plugin-0.1.9/src/oobabot_plugin/oobabot_log.css
+-rw-r--r--   0        0        0     1144 2023-05-24 17:50:51.222742 oobabot_plugin-0.1.9/src/oobabot_plugin/script.py
+-rw-r--r--   0        0        0      783 2023-05-26 18:41:48.302013 oobabot_plugin-0.1.9/src/oobabot_plugin/server.py
+-rw-r--r--   0        0        0     4728 2023-05-26 18:42:11.702013 oobabot_plugin-0.1.9/src/oobabot_plugin/strings.py
+-rw-r--r--   0        0        0     8509 2023-05-26 15:19:23.951748 oobabot_plugin-0.1.9/src/oobabot_plugin/worker.py
+-rw-r--r--   0        0        0     2699 1970-01-01 00:00:00.000000 oobabot_plugin-0.1.9/PKG-INFO
```

### Comparing `oobabot_plugin-0.1.8/LICENSE` & `oobabot_plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.8/oobabot_plugin/input_handlers.py` & `oobabot_plugin-0.1.9/src/oobabot_plugin/input_handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -103,59 +103,76 @@
         settings_group: oobabot.overengineered_settings_parser.ConfigSettingGroup,
         setting_name: str,
         fn_get_character_list: typing.Callable[[], typing.List[str]],
     ):
         super().__init__(component, settings_group, setting_name)
         self.fn_get_character_list = fn_get_character_list
 
-    def _character_name_to_filepath(self, character: str) -> str:
+    @classmethod
+    def character_name_to_filepath(cls, character: str) -> str:
         # this is how it's done in chat.py... there's no method to
         # call, so just do the same thing here
         filename = ""
         for extension in ["yml", "yaml", "json"]:
-            filepath = pathlib.Path(f"{self.FOLDER}/{character}.{extension}")
+            filepath = pathlib.Path(f"{cls.FOLDER}/{character}.{extension}")
             if filepath.exists():
                 filename = str(filepath.resolve())
         return filename
 
     def write_to_settings(self, new_value: str) -> None:
-        filename = self._character_name_to_filepath(new_value)
+        filename = self.character_name_to_filepath(new_value)
         super().write_to_settings(filename)
 
-    def read_from_settings(self) -> str:
-        # turning the path back into the character name just means
-        # removing the folder and extension... but case may have been
-        # lost, so we'll need to match it against the list of available
-        # options.
-        # also, the file may no longer exist, in that case we'll just
-        # return the empty string
-        filename = super().read_from_settings()
+    @classmethod
+    def filename_to_character_name(
+        cls,
+        filename: str,
+        fn_get_character_list: typing.Callable[[], typing.List[str]],
+    ) -> str:
         if not filename:
             return ""
         path = pathlib.Path(str(filename))
         if not path.exists():
             return ""
-        characters = self.fn_get_character_list()
+        characters = fn_get_character_list()
         for character in characters:
             if character.lower() == path.stem.lower():
                 return character
         return ""
 
+    def read_from_settings(self) -> str:
+        # turning the path back into the character name just means
+        # removing the folder and extension... but case may have been
+        # lost, so we'll need to match it against the list of available
+        # options.
+        # also, the file may no longer exist, in that case we'll just
+        # return the empty string
+        filename = super().read_from_settings()
+        return self.filename_to_character_name(
+            str(filename),
+            self.fn_get_character_list,
+        )
+
     def update_component_from_event(self, new_value: str) -> dict:
         self.write_to_settings(new_value)
         result = self.component.update(
             value=self.read_from_settings(),
             choices=self.fn_get_character_list(),
         )
         return result
 
     def init_component_from_setting(self):
         def init_component():
+            # when initializing the component, we need to
+            # return "None" for an empty character name.
+            character_name = self.read_from_settings()
+            if not character_name:
+                character_name = "None"
             return self.component.update(
-                value=self.read_from_settings(),
+                value=character_name,
                 interactive=True,
                 choices=self.fn_get_character_list(),
             )
 
         self.component.attach_load_event(
             init_component,
             None,
@@ -164,22 +181,31 @@
 
 class ListComponentToSetting(SimpleComponentToSetting):
     """
     A specific implementation of SimpleComponentToSetting that
     handles settings that are lists of strings.
     """
 
+    @classmethod
+    def list_to_string(cls, word_list: typing.List[str]) -> str:
+        word_list = [str(word).strip() for word in word_list]
+        return ", ".join(word_list)
+
+    @classmethod
+    def string_to_list(cls, word_string: str) -> typing.List[str]:
+        word_list = [word.strip() for word in word_string.split(",")]
+        return [word for word in word_list if word]
+
     def write_to_settings(self, new_value: str) -> None:
-        words = [word.strip() for word in new_value.split(",")]
+        words = self.string_to_list(new_value)
         self.settings_group.set(self.setting_name, words)
 
     def read_from_settings(self) -> str:
         word_list = self.settings_group.get_list(self.setting_name)
-        word_list = [str(word).strip() for word in word_list]
-        return ", ".join(word_list)
+        return self.list_to_string(word_list)  # type: ignore
 
 
 class ResponseRadioComponentToSetting(ComponentToSetting):
     """
     A specific implementation of ComponentToSetting that
     handles the radio button group for how we split
     responses into messages.  There are currently 3
```

### Comparing `oobabot_plugin-0.1.8/oobabot_plugin/install.py` & `oobabot_plugin-0.1.9/src/oobabot_plugin/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import argparse
 import importlib.resources
 import os
 import shutil
 import sys
 
+from oobabot_plugin import server
+
 
 def ensure_in_oobabooga_dir(cwd: str) -> None:
     if os.path.isdir(cwd + "/extensions"):
         return
 
     print(
         "This script must be run from the root directory of an oobabooga install.",
@@ -88,14 +90,18 @@
     parser = argparse.ArgumentParser(
         description="Install or uninstall the oobabot plugin.",
         epilog="This script must be run from the root directory of "
         + "an oobabooga install.",
     )
     subparsers = parser.add_subparsers()
 
+    subparsers.add_parser("server", help="Run our standalone web server.").set_defaults(
+        func=server.web_main
+    )
+
     subparsers.add_parser("install", help="Install the oobabot plugin.").set_defaults(
         func=do_install
     )
 
     subparsers.add_parser(
         "uninstall", help="Uninstall the oobabot plugin."
     ).set_defaults(func=do_uninstall)
```

### Comparing `oobabot_plugin-0.1.8/oobabot_plugin/instructions.md` & `oobabot_plugin-0.1.9/src/oobabot_plugin/instructions.md`

 * *Files identical despite different names*

### Comparing `oobabot_plugin-0.1.8/oobabot_plugin/strings.py` & `oobabot_plugin-0.1.9/src/oobabot_plugin/strings.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,21 +39,38 @@
 
 
 def get_css() -> str:
     return resource("oobabot_log.css")
 
 
 def get_js() -> str:
-    return resource("oobabot_log.js")
+    custom_js = resource("ace.js")
+    custom_js += resource("ace_theme_github.js")
+    custom_js += resource("ace_theme_github_dark.js")
+    custom_js += resource("ace_mode_yaml.js")
+    custom_js += resource("ace_oobabot.js")
+    return custom_js
 
 
 def token_is_plausible(token: str) -> bool:
     return len(token.strip()) >= TOKEN_LEN_CHARS
 
 
+def format_yaml_for_html(yaml: str) -> str:
+    template = resource("editor.html")
+    # replace {{OOBABOT-CONFIG-YML}} with yaml
+    return template.replace("{{OOBABOT-CONFIG-YML}}", yaml)
+
+
+def format_save_result(yaml_error: typing.Optional[str]) -> str:
+    if yaml_error:
+        return "❌ **Error**: " + yaml_error
+    return "✔️ **Saved**"
+
+
 def make_link_from_token(
     token: str,
     fn_calc_invite_url: typing.Optional[typing.Callable[[str], str]],
 ) -> str:
     if not token or not fn_calc_invite_url:
         return "A link will appear here once you have set your Discord token."
     link = fn_calc_invite_url(token)
@@ -82,28 +99,31 @@
             fn_generate_invite_url,
         )
     if new_token:
         return prefix
     return "A link will appear here once you have set your Discord token."
 
 
-def get_available_characters():
+CHARACTER_NONE = "None"
+
+
+def get_available_characters() -> typing.List[str]:
     """
     This is a list of all files in the ./characters folder whose
     extension is .json, .yaml, or .yml
 
     The list is then sorted alphabetically, and 'None' is added to
     the start.
     """
     characters = []
     for extension in ["yml", "yaml", "json"]:
         for filepath in pathlib.Path("characters").glob(f"*.{extension}"):
             characters.append(filepath.stem)
     characters.sort()
-    characters.insert(0, "None")
+    characters.insert(0, CHARACTER_NONE)
     return characters
 
 
 def repair_logging() -> typing.Optional[logging.Logger]:
     ##################################
     # so, logging_colors.py, rather than using the logging module's built-in
     # formatter, is monkey-patching the logging module's StreamHandler.emit.
```

### Comparing `oobabot_plugin-0.1.8/pyproject.toml` & `oobabot_plugin-0.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "oobabot-plugin"
-version = "0.1.8"
-description = "A plugin to oobabooga's text-generation-webui supporting AI-driven Discord bots."
+version = "0.1.9"
+description = "A Discord bot plugin to oobabooga's text-generation-webui, based on oobabot."
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot-plugin"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-oobabot = "^0.1.8"
+oobabot = "^0.1.9"
 gradio = "^3.31.0"
 
+[tool.poetry.scripts]
+oobabot-plugin = 'oobabot_plugin.install:main'
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.flakeheaven]
 format = "grouped"
 max-line-length = 88
@@ -42,10 +45,7 @@
 py-version = '3.8.1'
 j = 8
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 88
 disable = "C0116,R0902,R0903,R0912,R0913,R0914,W0511,W0621"
 include-naming-hint = true
-
-[tool.poetry.scripts]
-oobabot-plugin = 'oobabot_plugin.install:main'
```


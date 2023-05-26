# Comparing `tmp/oobabot-0.1.8.tar.gz` & `tmp/oobabot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.8.tar", max compression
+gzip compressed data, was "oobabot-0.1.9.tar", max compression
```

## Comparing `oobabot-0.1.8.tar` & `oobabot-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-05-03 00:11:59.534663 oobabot-0.1.8/LICENSE
--rw-r--r--   0        0        0    15491 2023-05-24 01:57:57.638210 oobabot-0.1.8/README.md
--rw-r--r--   0        0        0     1222 2023-05-22 15:16:17.945097 oobabot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-19 20:38:41.345994 oobabot-0.1.8/src/oobabot/__init__.py
--rw-r--r--   0        0        0      121 2023-05-18 18:14:55.125650 oobabot-0.1.8/src/oobabot/__main__.py
--rw-r--r--   0        0        0     6457 2023-05-22 15:03:15.709636 oobabot-0.1.8/src/oobabot/bot_commands.py
--rw-r--r--   0        0        0     6873 2023-05-22 15:03:19.938322 oobabot-0.1.8/src/oobabot/decide_to_respond.py
--rw-r--r--   0        0        0    29147 2023-05-22 15:12:32.817542 oobabot-0.1.8/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     6906 2023-05-22 13:58:48.609231 oobabot-0.1.8/src/oobabot/discord_utils.py
--rw-r--r--   0        0        0     8405 2023-05-23 05:48:45.666973 oobabot-0.1.8/src/oobabot/fancy_logger.py
--rw-r--r--   0        0        0     3106 2023-05-18 18:20:12.856052 oobabot-0.1.8/src/oobabot/http_client.py
--rw-r--r--   0        0        0    13406 2023-05-22 14:46:56.313942 oobabot-0.1.8/src/oobabot/image_generator.py
--rw-r--r--   0        0        0    10159 2023-05-23 05:48:45.668106 oobabot-0.1.8/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0    13626 2023-05-24 00:48:55.123541 oobabot-0.1.8/src/oobabot/oobabot.py
--rw-r--r--   0        0        0    12812 2023-05-23 05:48:45.669521 oobabot-0.1.8/src/oobabot/overengineered_settings_parser.py
--rw-r--r--   0        0        0     4353 2023-05-21 10:37:28.483174 oobabot-0.1.8/src/oobabot/persona.py
--rw-r--r--   0        0        0     7774 2023-05-23 05:48:45.670867 oobabot-0.1.8/src/oobabot/prompt_generator.py
--rw-r--r--   0        0        0     3243 2023-05-18 18:22:10.143873 oobabot-0.1.8/src/oobabot/repetition_tracker.py
--rw-r--r--   0        0        0     6736 2023-05-22 14:11:01.702461 oobabot-0.1.8/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     9758 2023-05-21 10:37:28.483908 oobabot-0.1.8/src/oobabot/sd_client.py
--rw-r--r--   0        0        0    30229 2023-05-23 05:48:45.672008 oobabot-0.1.8/src/oobabot/settings.py
--rw-r--r--   0        0        0    10906 2023-05-19 17:11:29.625366 oobabot-0.1.8/src/oobabot/templates.py
--rw-r--r--   0        0        0     1481 2023-05-18 17:46:10.237360 oobabot-0.1.8/src/oobabot/types.py
--rw-r--r--   0        0        0    16328 1970-01-01 00:00:00.000000 oobabot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.9/LICENSE
+-rw-r--r--   0        0        0    15491 2023-05-24 05:41:27.585006 oobabot-0.1.9/README.md
+-rw-r--r--   0        0        0     1222 2023-05-26 15:58:27.461799 oobabot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-26 15:58:34.741799 oobabot-0.1.9/src/oobabot/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     6457 2023-05-26 15:20:56.341750 oobabot-0.1.9/src/oobabot/bot_commands.py
+-rw-r--r--   0        0        0     7616 2023-05-25 21:00:13.017091 oobabot-0.1.9/src/oobabot/decide_to_respond.py
+-rw-r--r--   0        0        0    29410 2023-05-25 21:00:13.017091 oobabot-0.1.9/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     6991 2023-05-25 16:33:50.006742 oobabot-0.1.9/src/oobabot/discord_utils.py
+-rw-r--r--   0        0        0     8993 2023-05-26 15:20:56.341750 oobabot-0.1.9/src/oobabot/fancy_logger.py
+-rw-r--r--   0        0        0     3106 2023-05-22 16:17:18.271389 oobabot-0.1.9/src/oobabot/http_client.py
+-rw-r--r--   0        0        0    13406 2023-05-22 16:25:27.421377 oobabot-0.1.9/src/oobabot/image_generator.py
+-rw-r--r--   0        0        0    10297 2023-05-25 16:33:50.006742 oobabot-0.1.9/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0    13851 2023-05-26 15:21:06.401750 oobabot-0.1.9/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0    13391 2023-05-26 15:21:06.401750 oobabot-0.1.9/src/oobabot/overengineered_settings_parser.py
+-rw-r--r--   0        0        0     4353 2023-05-22 16:16:39.311390 oobabot-0.1.9/src/oobabot/persona.py
+-rw-r--r--   0        0        0     7774 2023-05-22 23:19:07.950798 oobabot-0.1.9/src/oobabot/prompt_generator.py
+-rw-r--r--   0        0        0     3243 2023-05-20 20:44:28.735288 oobabot-0.1.9/src/oobabot/repetition_tracker.py
+-rw-r--r--   0        0        0     6736 2023-05-22 16:25:27.421377 oobabot-0.1.9/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     9758 2023-05-20 20:33:38.965441 oobabot-0.1.9/src/oobabot/sd_client.py
+-rw-r--r--   0        0        0    26244 2023-05-26 15:36:23.871770 oobabot-0.1.9/src/oobabot/settings.py
+-rw-r--r--   0        0        0    10906 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/templates.py
+-rw-r--r--   0        0        0     1481 2023-05-20 20:17:19.345668 oobabot-0.1.9/src/oobabot/types.py
+-rw-r--r--   0        0        0    16328 1970-01-01 00:00:00.000000 oobabot-0.1.9/PKG-INFO
```

### Comparing `oobabot-0.1.8/LICENSE` & `oobabot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/README.md` & `oobabot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/pyproject.toml` & `oobabot-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
```

### Comparing `oobabot-0.1.8/src/oobabot/bot_commands.py` & `oobabot-0.1.9/src/oobabot/bot_commands.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/decide_to_respond.py` & `oobabot-0.1.9/src/oobabot/decide_to_respond.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,22 +15,31 @@
     """
     A dictionary that keeps track of the last time we were mentioned
     in a channel.
 
     This uses the timestamp on the message, not the local system's
     RTC.  The advantage of this is that if messages are delayed,
     we'll only respond to ones that were actually sent within the
-    appropriate time window.
+    appropriate time window.  It also makes it easier to test.
     """
 
-    def __init__(self, cache_timeout: float):
+    def __init__(self, cache_timeout: float, unsolicited_channel_cap: int):
         self.cache_timeout = cache_timeout
+        self.unsolicited_channel_cap = unsolicited_channel_cap
 
     def purge_outdated(self, latest_timestamp: float) -> None:
         oldest_time_to_keep = latest_timestamp - self.cache_timeout
+
+        if self.unsolicited_channel_cap > 0:
+            # find the n-th largest timestamp
+            if self.unsolicited_channel_cap < len(self):
+                nth_largest_timestamp = sorted(self.values())[
+                    -self.unsolicited_channel_cap
+                ]
+                oldest_time_to_keep = max(oldest_time_to_keep, nth_largest_timestamp)
         purged = {
             channel_id: response_time
             for channel_id, response_time in self.items()
             if response_time >= oldest_time_to_keep
         }
         self.clear()
         self.update(purged)
@@ -57,15 +66,19 @@
     ):
         self.ignore_dms = discord_settings["ignore_dms"]
         self.interrobang_bonus = interrobang_bonus
         self.persona = persona
         self.time_vs_response_chance = time_vs_response_chance
 
         last_reply_cache_timeout = max(time for time, _ in time_vs_response_chance)
-        self.last_reply_times = LastReplyTimes(last_reply_cache_timeout)
+        unsolicited_channel_cap = discord_settings["unsolicited_channel_cap"]
+        self.last_reply_times = LastReplyTimes(
+            last_reply_cache_timeout,
+            unsolicited_channel_cap,
+        )
 
     def is_directly_mentioned(
         self, our_user_id: int, message: types.GenericMessage
     ) -> bool:
         """
         Returns True if the message is a direct message to us, or if it
         mentions us by @name or wakeword.
@@ -189,7 +202,10 @@
                 return (True, False)
 
         # ignore anything else
         return (False, False)
 
     def log_mention(self, channel_id: int, send_timestamp: float) -> None:
         self.last_reply_times.log_mention(channel_id, send_timestamp)
+
+    def get_unsolicited_channel_cap(self) -> int:
+        return self.last_reply_times.unsolicited_channel_cap
```

### Comparing `oobabot-0.1.8/src/oobabot/discord_bot.py` & `oobabot-0.1.9/src/oobabot/discord_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,22 @@
             "History: %d lines ", self.prompt_generator.history_lines
         )
 
         fancy_logger.get().debug(
             "Stop markers: %s", ", ".join(self.stop_markers) or "<none>"
         )
 
+        # log unsolicited_channel_cap
+        cap = self.decide_to_respond.get_unsolicited_channel_cap()
+        cap = str(cap) if cap > 0 else "<unlimited>"
+        fancy_logger.get().debug(
+            "Unsolicited channel cap: %s",
+            cap,
+        )
+
         str_wakewords = (
             ", ".join(self.persona.wakewords) if self.persona.wakewords else "<none>"
         )
         fancy_logger.get().debug("Wakewords: %s", str_wakewords)
 
         self.ooba_client.on_ready()
```

### Comparing `oobabot-0.1.8/src/oobabot/discord_utils.py` & `oobabot-0.1.9/src/oobabot/discord_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,7 +207,11 @@
         add_reactions=True,
     ).value
 
     return (
         "https://discord.com/api/oauth2/authorize?client_id="
         + f"{ai_user_id}&permissions={permissions}&scope=bot"
     )
+
+
+def setup_logging(**kwargs: typing.Any):
+    discord.utils.setup_logging(**kwargs)
```

### Comparing `oobabot-0.1.8/src/oobabot/fancy_logger.py` & `oobabot-0.1.9/src/oobabot/fancy_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 """
 
 import html
 import logging
 import textwrap
 import typing
 
+from oobabot import discord_utils
+
 FOREGROUND_COLORS = {
     "black": 30,
     "red": 31,
     "green": 32,
     "yellow": 33,
     "blue": 34,
     "magenta": 35,
     "cyan": 36,
     "white": 37,
 }
 
+BACKGROUND_COLORS = {k: v + 10 for k, v in FOREGROUND_COLORS.items()}
+
 HTML_HEADER = textwrap.dedent(
     """
     <!DOCTYPE html>
     <html lang="en">
     <head>
     <meta charset="utf-8">
     <title>oobabot logs</title>
@@ -49,26 +53,31 @@
     <body><div class="oobabot-log">
     """
 )
 HTML_RECORD_SEPARATOR = "\n<br>"
 HTML_FOOTER = "</div></body></html>"
 
 
-def apply_color_console(color: str, text: str) -> str:
-    return f"\033[{FOREGROUND_COLORS[color]}m{text}\033[0m"
+def apply_color_console(color: str, text: str, bg_color: str = "black") -> str:
+    return (
+        f"\033[{FOREGROUND_COLORS[color]};{BACKGROUND_COLORS[bg_color]}m{text}\033[0m"
+    )
 
 
 def apply_color_html(color: str, text: str) -> str:
     return f"<span class='oobabot-{color}'>{text}</span>"
 
 
 def make_coloring_book(
     fn_apply_color: typing.Callable[[str, str], str]
 ) -> typing.Dict[int, str]:
-    prefix = f'{fn_apply_color("yellow", "%(asctime)s")} %(levelname)s '
+    prefix = (
+        f'{fn_apply_color("yellow", "%(asctime)s")}'
+        + f'{fn_apply_color("white", " %(levelname)5s ")}'
+    )
     msg = "%(message)s"
     return {
         logging.DEBUG: prefix + fn_apply_color("cyan", msg),
         logging.INFO: prefix + fn_apply_color("white", msg),
         logging.WARNING: prefix + fn_apply_color("yellow", msg),
         logging.ERROR: prefix + fn_apply_color("red", msg),
         logging.CRITICAL: prefix + fn_apply_color("red", msg),
@@ -144,14 +153,25 @@
         console_handler.setFormatter(
             ColorfulLoggingFormatter(
                 coloring_book=make_coloring_book(apply_color_console),
             )
         )
         logger.addHandler(console_handler)
 
+        discord_utils.setup_logging(
+            handler=logging.StreamHandler(),
+            level=logging.INFO,
+            formatter=ColorfulLoggingFormatter(
+                coloring_book=make_coloring_book(
+                    lambda a, b: apply_color_console(a, b, "magenta")
+                ),
+            ),
+            root=False,
+        )
+
     recent_logs.setLevel(level)
     recent_logs.setFormatter(
         ColorfulLoggingFormatter(
             coloring_book=make_coloring_book(apply_color_html),
             fn_format_message=do_escape,
         )
     )
```

### Comparing `oobabot-0.1.8/src/oobabot/http_client.py` & `oobabot-0.1.9/src/oobabot/http_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/image_generator.py` & `oobabot-0.1.9/src/oobabot/image_generator.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/ooba_client.py` & `oobabot-0.1.9/src/oobabot/ooba_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import re
 import time
 import typing
 
 import aiohttp
 import pysbd
+import pysbd.utils
 
 from oobabot import fancy_logger
 from oobabot import http_client
 
 
 class MessageSplitter(abc.ABC):
     """
@@ -93,15 +94,17 @@
     """
 
     def __init__(self):
         super().__init__()
         self.segmenter = pysbd.Segmenter(language="en", clean=False, char_span=True)
 
     def partition(self, unseen: str) -> typing.Generator[str, None, None]:
-        segments = self.segmenter.segment(unseen)
+        segments: typing.List[pysbd.utils.TextSpan] = self.segmenter.segment(
+            unseen
+        )  # type: ignore -- type is determined by char_span=True above
 
         # any remaining non-sentence things will be in the last element
         # of the list.  Don't print that yet.  At the very worst, we'll
         # print it when the END_OF_INPUT signal is reached.
         for sentence_w_char_spans in segments[:-1]:
             # sentence_w_char_spans is a class with the following fields:
             #  - sent: str, sentence text
```

### Comparing `oobabot-0.1.8/src/oobabot/oobabot.py` & `oobabot-0.1.9/src/oobabot/oobabot.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,18 @@
 
             if self.settings.general_settings.get("help"):
                 self.settings.print_help()
                 return
 
             if self.settings.general_settings.get("generate_config"):
                 self.settings.write_to_stream(out_stream=sys.stdout)
+                if sys.stdout.isatty():
+                    print(self.settings.META_INSTRUCTION, file=sys.stderr)
+                else:
+                    print("# oobabot: config.yml output successfully", file=sys.stderr)
                 return
 
             if not self.settings.discord_settings.get("discord_token"):
                 msg = (
                     f"Please set the '{self.settings.DISCORD_TOKEN_ENV_VAR}' "
                     + "environment variable to your bot's discord token."
                 )
```

### Comparing `oobabot-0.1.8/src/oobabot/overengineered_settings_parser.py` & `oobabot-0.1.9/src/oobabot/overengineered_settings_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 load_from_dict - sets defaults, then loads from a dictionary only.
 load_from_yaml - sets defaults, then loads from YAML only.
 write_to_file - writes the given config as YAML to the given file.
 write_to_stream - writes the given config as YAML to the given stream.
 """
 
 import argparse
+import pathlib
 import textwrap
 import typing
 
 import ruamel.yaml as ryaml
+import ruamel.yaml.error as ryaml_error
 
 import oobabot
 
 YAML_WIDTH = 88
 DIVIDER = "# " * (YAML_WIDTH >> 1)
 INDENT_UNIT = 2
 
@@ -285,27 +287,46 @@
     def get_all(self) -> typing.Dict[str, SettingValueType]:
         return {name: setting.get() for (name, setting) in self.settings.items()}.copy()
 
 
 def load_from_yaml(
     filename: str,
     setting_groups: typing.List["ConfigSettingGroup"],
-) -> None:
+) -> typing.Optional[str]:
     """
     Load settings from a YAML file only
+
+    Returns None if successful, or an error message if not
     """
     try:
         with open(filename, "r", encoding="utf-8") as file:
-            yaml = ryaml.YAML(typ="safe")
-            yaml_settings = yaml.load(file)
-            for group in setting_groups:
-                group.set_values_from_yaml(yaml_settings)
+            return load_from_yaml_stream(file, setting_groups)
 
     except (FileNotFoundError, IsADirectoryError):
-        pass
+        return "File not found"
+
+
+def load_from_yaml_stream(
+    stream: typing.Union[pathlib.Path, ryaml.StreamTextType],
+    setting_groups: typing.List["ConfigSettingGroup"],
+) -> typing.Optional[str]:
+    """
+    Load settings from a YAML string only
+
+    Returns None if successful, or an error message if not
+    """
+    try:
+        yaml = ryaml.YAML(typ="safe")
+        yaml_settings = yaml.load(stream)
+    except ryaml_error.MarkedYAMLError as err:
+        return str(err)
+
+    for group in setting_groups:
+        group.set_values_from_yaml(yaml_settings)
+    return None
 
 
 def load_from_cli(
     args,
     setting_groups: typing.List["ConfigSettingGroup"],
 ) -> argparse.ArgumentParser:
     """
```

### Comparing `oobabot-0.1.8/src/oobabot/persona.py` & `oobabot-0.1.9/src/oobabot/persona.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/prompt_generator.py` & `oobabot-0.1.9/src/oobabot/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/repetition_tracker.py` & `oobabot-0.1.9/src/oobabot/repetition_tracker.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/response_stats.py` & `oobabot-0.1.9/src/oobabot/response_stats.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/sd_client.py` & `oobabot-0.1.9/src/oobabot/sd_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/settings.py` & `oobabot-0.1.9/src/oobabot/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,30 @@
         a setting group for settings related to the stable diffusion API
 
     - general_settings:
         a setting group for settings that are not included in the config file
 """
 import os
 import shutil
-import sys
 import textwrap
 import typing
 
 from oobabot import templates
 import oobabot.overengineered_settings_parser as oesp
 
 
 def _console_wrapped(message):
     width = shutil.get_terminal_size().columns
     return "\n".join(textwrap.wrap(message, width))
 
 
 def _make_template_comment(
-    name: str,
     tokens_desc_tuple: typing.Tuple[typing.List[templates.TemplateToken], str, bool],
 ) -> typing.List[str]:
     return [
-        f"Path to a file containing the {name} template.",
         tokens_desc_tuple[1],
         ".",
         f"Allowed tokens: {', '.join([str(t) for t in tokens_desc_tuple[0]])}",
         ".",
     ]
 
 
@@ -403,28 +400,51 @@
                         """
                     )
                 ],
                 include_in_argparse=False,
             )
         )
         self.discord_settings.add_setting(
-            oesp.ConfigSetting[bool](
+            oesp.ConfigSetting[int](
                 name="stream_responses",
                 default=False,
                 description_lines=[
                     textwrap.dedent(
                         """
                         FEATURE PREVIEW: Stream responses into a single message
                         as they are generated.
                         Note: may be janky
                         """
                     )
                 ],
             )
         )
+        self.discord_settings.add_setting(
+            oesp.ConfigSetting[int](
+                name="unsolicited_channel_cap",
+                default=3,
+                description_lines=[
+                    textwrap.dedent(
+                        """
+                        FEATURE PREVIEW: Adds a limit to the number of channels
+                        the bot will post unsolicited messages in at the same
+                        time.  This is to prevent the bot from being too noisy
+                        in large servers.
+
+                        When set, only the most recent N channels the bot has
+                        been summoned in will have a chance of receiving an
+                        unsolicited message.  The bot will still respond to
+                        @-mentions and wake words in any channel it can access.
+
+                        Set to 0 to disable this feature.
+                        """
+                    )
+                ],
+            )
+        )
 
         ###########################################################
         # Oobabooga Settings
 
         self.oobabooga_settings = oesp.ConfigSettingGroup("Oobabooga")
         self.setting_groups.append(self.oobabooga_settings)
 
@@ -593,152 +613,19 @@
         for template, tokens_desc_tuple in templates.TemplateStore.TEMPLATES.items():
             _, _, is_ai_prompt = tokens_desc_tuple
 
             self.template_settings.add_setting(
                 oesp.ConfigSetting[str](
                     name=str(template),
                     default=templates.TemplateStore.DEFAULT_TEMPLATES[template],
-                    description_lines=_make_template_comment(
-                        str(template), tokens_desc_tuple
-                    ),
+                    description_lines=_make_template_comment(tokens_desc_tuple),
                     include_in_yaml=is_ai_prompt,
                 )
             )
 
-        self._add_deprecated_settings()
-
-    def _add_deprecated_settings(self) -> None:
-        ###########################################################
-        # Deprecated Settings
-        # These used to be part of the Stable Diffusion section,
-        # but now are covered in the stable_diffusion->request_params
-        # section of the config.yml file.
-        #
-        # These are still here for backwards compatibility, but
-        # will be removed in a future release.
-        #
-        # They're being moved since they're redundant with the
-        # request_params values, and it's confusing to have those
-        # set in two separate places.
-        #
-        # The settings won't be written to the config.yaml template,
-        # as they're already covered in the request_params section.
-
-        def set_sd_parm(param: str, value: oesp.SettingValueType):
-            if not value:
-                return
-            setting = self.stable_diffusion_settings.get_setting("request_params")
-
-            # get returns a copy of the settings dict, so we need to
-            # push it back after we make a change
-            setting_dict = setting.get()
-            setting_dict[param] = value
-            setting.set_value(setting_dict)
-
-        self.deprecated_settings = oesp.ConfigSettingGroup(
-            "Deprecated Settings",
-            include_in_yaml=False,
-            description="These settings are deprecated and will be removed in "
-            + "a future release.  Please set them with config.yml instead.",
-        )
-        self.setting_groups.append(self.deprecated_settings)
-
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[int](
-                name="diffusion_steps",
-                default=0,
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Number of diffusion steps to take when generating an image.
-                        """
-                    )
-                ],
-                fn_on_set=lambda x: set_sd_parm("steps", int(x)),
-            )
-        )
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[int](
-                name="image_height",
-                default=0,
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Size of images to generate.  This is the height of the image
-                        in pixels.
-                        """
-                    )
-                ],
-                fn_on_set=lambda x: set_sd_parm("height", int(x)),
-            )
-        )
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[int](
-                name="image_width",
-                default=0,
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Size of images to generate.  This is the width of the image
-                        in pixels.
-                        """
-                    )
-                ],
-                fn_on_set=lambda x: set_sd_parm("width", int(x)),
-            )
-        )
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[str](
-                name="stable_diffusion_sampler",
-                default="",
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Sampler to use when generating images.  If not specified,
-                        the one set on the AUTOMATIC1111 server will be used.
-                        """
-                    )
-                ],
-                cli_args=["--stable-diffusion-sampler", "--sd-sampler"],
-                fn_on_set=lambda x: set_sd_parm("sampler", str(x)),
-            )
-        )
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[str](
-                name="sd_negative_prompt",
-                default="",
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Negative prompt to use when generating images.  This will
-                        discourage Stable Diffusion from generating images with the
-                        specified content.  By default, this is set to follow
-                        Discord's TOS.
-                        """
-                    )
-                ],
-                fn_on_set=lambda x: set_sd_parm("negative_prompt", str(x)),
-            )
-        )
-        self.deprecated_settings.add_setting(
-            oesp.ConfigSetting[str](
-                name="sd_negative_prompt_nsfw",
-                default="",
-                description_lines=[
-                    textwrap.dedent(
-                        """
-                        Negative prompt to use when generating images in a channel
-                        marked as 'Age-Restricted'.
-                        """
-                    )
-                ],
-                fn_on_set=lambda x: set_sd_parm("negative_prompt_nsfw", str(x)),
-            )
-        )
-
     META_INSTRUCTION = (
         "\n\n"
         + "# " * 30
         + textwrap.dedent(
             """
             # Please save this output into ./config.yml
             # edit it to your liking, then run the bot again.
@@ -747,18 +634,14 @@
             #       oobabot
             """
         )
     )
 
     def write_to_stream(self, out_stream) -> None:
         oesp.write_to_stream(self.setting_groups, out_stream)
-        if sys.stdout.isatty():
-            print(self.META_INSTRUCTION, file=sys.stderr)
-        else:
-            print("# oobabot: config.yml output successfully", file=sys.stderr)
 
     def write_to_file(self, filename: str) -> None:
         oesp.write_to_file(self.setting_groups, filename)
 
     def _filename_from_args(self, args: typing.List[str]) -> str:
         """
         Get the configuration filename from the command line arguments.
@@ -774,14 +657,27 @@
                 # find the element after config_flag in args
                 try:
                     return args[args.index(config_flag) + 1]
                 except (ValueError, IndexError):
                     continue
         return config_setting.default
 
+    def load_from_yaml_stream(self, stream: typing.TextIO) -> typing.Optional[str]:
+        """
+        Load the config from a YAML stream.
+
+        params:
+            stream: stream to load the config from
+
+        returns:
+            None if the config was loaded successfully, otherwise a string
+            containing an error message.
+        """
+        return oesp.load_from_yaml_stream(stream, setting_groups=self.setting_groups)
+
     def load(
         self,
         cli_args: typing.List[str],
         config_file: typing.Optional[str] = None,
     ) -> None:
         """
         Load the config from the command line arguments and config file.
```

### Comparing `oobabot-0.1.8/src/oobabot/templates.py` & `oobabot-0.1.9/src/oobabot/templates.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/src/oobabot/types.py` & `oobabot-0.1.9/src/oobabot/types.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.8/PKG-INFO` & `oobabot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
 Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/nonebot-plugin-alconna-0.5.1.tar.gz` & `tmp/nonebot-plugin-alconna-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.5.1.tar", last modified: Sun May 21 13:31:02 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.6.0.tar", last modified: Fri May 26 08:54:56 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.5.1.tar` & `nonebot-plugin-alconna-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.5.1/LICENSE
--rw-r--r--   0        0        0     1135 2023-05-21 13:28:49.813097 nonebot-plugin-alconna-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.5.1/README.md
--rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2405 2023-05-18 15:49:32.019141 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1231 2023-05-18 15:49:32.003141 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1448 2023-05-11 15:34:24.694684 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3819 2023-05-18 16:17:32.686671 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8912 2023-05-21 13:23:07.447971 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1135 2023-05-26 08:51:03.270110 nonebot-plugin-alconna-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.6.0/README.md
+-rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2405 2023-05-18 15:49:32.019141 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1231 2023-05-18 15:49:32.003141 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-26 08:51:03.247079 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-26 08:51:03.151926 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     9020 2023-05-26 08:51:03.217077 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.6.0/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.5.1/LICENSE` & `nonebot-plugin-alconna-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/pyproject.toml` & `nonebot-plugin-alconna-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.5.1"
+version = "0.6.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
-    "arclet-alconna<2.0.0, >=1.7.6",
+    "arclet-alconna<2.0.0, >=1.7.7",
     "arclet-alconna-tools<0.7.0, >=0.6.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
```

### Comparing `nonebot-plugin-alconna-0.5.1/README.md` & `nonebot-plugin-alconna-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Generic, TypeVar, Optional, TypedDict
 from typing_extensions import NotRequired
 
-from arclet.alconna import Arparma, Empty
+from arclet.alconna import Arparma, Empty, Alconna
 from arclet.alconna.duplication import Duplication
 
 T = TypeVar("T")
 T_Duplication = TypeVar("T_Duplication", bound=Duplication)
 
 
 @dataclass
@@ -42,14 +42,15 @@
 
     def __repr__(self):
         return f"Query({self.path}, {self.result})"
 
 
 @dataclass(frozen=True)
 class CommandResult:
+    source: Alconna
     result: Arparma
     output: Optional[str] = field(default=None)
 
     @property
     def matched(self) -> bool:
         return self.result.matched
```

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Type, TypeVar, overload, Any, Callable
 from typing_extensions import Annotated
 
 from arclet.alconna import Arparma, Duplication, Empty
-from arclet.alconna.duplication import generate_duplication
+from arclet.alconna.builtin import generate_duplication
 from nonebot.internal.matcher import Matcher as Matcher
 from nonebot.internal.params import Depends as Depends
 from nonebot.typing import T_State
 
 from .consts import ALCONNA_RESULT
 from .model import CommandResult, Match, Query, T
 
@@ -62,16 +62,17 @@
 @overload
 def AlconnaDuplication(__t: Type[T_Duplication]) -> T_Duplication:
     ...
 
 
 def AlconnaDuplication(__t: Optional[Type[T_Duplication]] = None) -> Duplication:
     def _alconna_match(state: T_State) -> Duplication:
-        arp = _alconna_result(state).result
-        return __t(arp) if __t else generate_duplication(arp)
+        res = _alconna_result(state)
+        gt = __t or generate_duplication(res.source)
+        return gt(res.result)
 
     return Depends(_alconna_match, use_cache=False)
 
 
 AlcResult = Annotated[CommandResult, AlconnaResult()]
 AlcMatches = Annotated[Arparma, AlconnaMatches()]
```

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,22 +178,24 @@
         except (NotImplementedError, ValueError):
             return False
         with output_manager.capture(self.command.name) as cap:
             output_manager.set_action(lambda x: x, self.command.name)
             try:
                 arp = await self.handle(bot, event, msg)
             except Exception as e:
-                arp = Arparma(self.command.path, msg, False, error_info=repr(e))
+                arp = Arparma(self.command.path, msg, False, error_info=e)
             may_help_text: Optional[str] = cap.get("output", None)
         if not arp.matched and not may_help_text and self.skip:
             return False
+        if not may_help_text and arp.error_info:
+            may_help_text = repr(arp.error_info)
         if self.auto_send and may_help_text:
             await bot.send(event, await self._convert(may_help_text, event, arp))
             return False
-        state[ALCONNA_RESULT] = CommandResult(arp, may_help_text)
+        state[ALCONNA_RESULT] = CommandResult(self.command, arp, may_help_text)
         return True
 
     async def _convert(self, text: str, event: Event, arp: Arparma) -> Message:
         _t = (
             str(arp.error_info)
             if isinstance(arp.error_info, SpecialOptionTriggered)
             else "help"
```

### Comparing `nonebot-plugin-alconna-0.5.1/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/typings.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.5.1/PKG-INFO` & `nonebot-plugin-alconna-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.5.1
+Version: 0.6.0
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
```


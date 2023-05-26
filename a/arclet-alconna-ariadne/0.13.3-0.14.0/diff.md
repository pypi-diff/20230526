# Comparing `tmp/arclet-alconna-ariadne-0.13.3.tar.gz` & `tmp/arclet-alconna-ariadne-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ariadne-0.13.3.tar", last modified: Sun May 21 12:31:36 2023, max compression
+gzip compressed data, was "arclet-alconna-ariadne-0.14.0.tar", last modified: Fri May 26 10:13:38 2023, max compression
```

## Comparing `arclet-alconna-ariadne-0.13.3.tar` & `arclet-alconna-ariadne-0.14.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.3/LICENSE
--rw-r--r--   0        0        0     6165 2023-05-21 12:31:01.630026 arclet-alconna-ariadne-0.13.3/pyproject.toml
--rw-r--r--   0        0        0     7402 2023-05-10 15:25:33.392236 arclet-alconna-ariadne-0.13.3/README.md
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.3/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     6239 2023-05-21 06:45:27.744563 arclet-alconna-ariadne-0.13.3/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.3/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.14.0/LICENSE
+-rw-r--r--   0        0        0     6165 2023-05-26 10:11:22.219776 arclet-alconna-ariadne-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet-alconna-ariadne-0.14.0/README.md
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     4725 2023-05-26 09:57:30.809955 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.14.0/PKG-INFO
```

### Comparing `arclet-alconna-ariadne-0.13.3/LICENSE` & `arclet-alconna-ariadne-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.3/pyproject.toml` & `arclet-alconna-ariadne-0.14.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.13.3"
+version = "0.14.0"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -55,32 +55,32 @@
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.13.3"
+version = "0.14.0"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
     "graia",
     "arclet",
     "ariadne",
 ]
 dependencies = [
-    "arclet-alconna<2.0.0, >=1.7.6",
+    "arclet-alconna<2.0.0, >=1.7.7",
     "arclet-alconna-tools<0.7.0, >=0.6.0",
     "tarina>=0.3.3",
-    "nepattern<0.6.0, >=0.5.6",
+    "nepattern<0.6.0, >=0.5.8",
     "creart-graia>=0.1.5",
     "creart>=0.2.1",
     "graia-amnesia>=0.5.0",
     "graia-broadcast>=0.18.2",
     "graia-saya>=0.0.17",
     "launart>=0.5.0",
 ]
@@ -107,20 +107,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.3, >= 0.13.3",
+    "arclet-alconna-graia<0.14.0, >= 0.14.0",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.13.3"
+version = "0.14.0"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -148,20 +148,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.3, >= 0.13.3",
+    "arclet-alconna-graia<0.14.0, >= 0.14.0",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.13.3"
+version = "0.14.0"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -190,20 +190,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.3, >= 0.13.3",
+    "arclet-alconna-graia<0.14.0, >= 0.14.0",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.13.3"
+version = "0.14.0"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet-alconna-ariadne-0.13.3/README.md` & `arclet-alconna-ariadne-0.14.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 ### 单文件
 
 ariadne:
 
 ```python
 from arclet.alconna import Args
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult
 from arclet.alconna.graia.service import AlconnaGraiaService
 import arclet.alconna.ariadne
 ...
 manager = Launart(...)
 manager.add_service(AlconnaGraiaService())
 app = Ariadne(...)
 
@@ -88,27 +88,27 @@
 
 @app.broadcast.receiver(
     GroupMessage,
     dispatchers=[AlconnaDispatcher(alc, send_flag='stay')]
 )
 async def test2(
     group: Group,
-    result: AlconnaProperty[GroupMessage],
+    result: CommandResult[GroupMessage],
     sth: Match[str]
 ):
     print("sign:", result.result)
     print("sender:", group)
     print("match", sth.available, sth.result)
 ```
 
 avilla:
 
 ```python
 from arclet.alconna import Args
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult
 from arclet.alconna.graia.service import AlconnaGraiaService
 import arclet.alconna.avilla
 ...
 broadcast = create(Broadcast)
 manager = Launart(...)
 manager.add_service(AlconnaGraiaService())
 avilla = Avilla(...)
@@ -118,36 +118,36 @@
 
 @broadcast.receiver(
     MessageReceived,
     dispatchers=[AlconnaDispatcher(alc, send_flag='stay')]
 )
 async def test2(
     context: Context,
-    result: AlconnaProperty[MessageReceived],
+    result: CommandResult[MessageReceived],
     sth: Match[str]
 ):
     print("sign:", result.result)
     print("sender:", context.scene)
     print("match", sth.available, sth.result)
 ```
 
 ### 使用 Saya
 
 in module.py:
 ```python
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty, AlconnaSchema
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult, AlconnaSchema
 from arclet.alconna import Args
 ...
 channel = Channel.current()
 
 alc = Alconna("!jrrp", Args["sth", str, 1123])
 
 @channel.use(AlconnaSchema(AlconnaDispatcher(alc)))
 @channel.use(ListenerSchema([...]))
-async def test2(result: AlconnaProperty[...], sth: Match[str]):
+async def test2(result: CommandResult[...], sth: Match[str]):
     print("sign:", result.result)
     print("match", sth.available, sth.result)
 
 
 ```
 
 in main.py:
@@ -233,15 +233,15 @@
 ```
 
 `command`: 使用的 Alconna 指令
 
 `send_flag`: 解析期间输出信息的发送方式
 - reply: 直接发送给指令发送者
 - post: 以事件通过 Broadcast 广播
-- stay: 存入 AlconnaProperty 传递给事件处理器
+- stay: 存入 CommandResult 传递给事件处理器
 
 `skip_for_unmatch`: 解析失败时是否跳过, 否则错误信息按 send_flag 处理
 
 `comp_session`: 补全会话配置, 不传入则不启用补全会话
 
 `message_converter`: send_flag 为 reply 时 输出信息的预处理器
```

### Comparing `arclet-alconna-ariadne-0.13.3/src/arclet/alconna/ariadne/adapter.py` & `arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
-from contextlib import suppress
 from typing import Any, Callable, Union
 
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from graia.ariadne.app import Ariadne
-from graia.ariadne.dispatcher import ContextDispatcher
 from graia.ariadne.event.message import FriendMessage, GroupMessage, MessageEvent
 from graia.ariadne.message.chain import MessageChain
 from graia.ariadne.message.element import At, Plain, Source, File, Quote
 from graia.ariadne.model import Friend, Member, Client, Stranger
-from graia.ariadne.util import resolve_dispatchers_mixin
 from graia.ariadne.util.interrupt import FunctionWaiter
+from graia.broadcast import BaseDispatcher
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.interrupt import Waiter
 from graia.broadcast.utilles import run_always_await
 
 from arclet.alconna import Arparma, argv_config, set_default_argv_type
 
-from ..graia import AlconnaProperty, AlconnaSchema
+from ..graia.model import CommandResult, TConvert
 from ..graia.adapter import AlconnaGraiaAdapter
 from ..graia.argv import BaseMessageChainArgv
-from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
+from ..graia.dispatcher import AlconnaDispatcher
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda _, x: MessageChain([Plain(x)])
 Sender = Union[Friend, Member, Stranger, Client]
 
 
 class AlconnaAriadneAdapter(AlconnaGraiaAdapter[MessageEvent]):
@@ -42,56 +40,32 @@
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain("Unknown"))
 
     def source_id(self, source: MessageEvent | None = None) -> str:
         return str(source.source.id) if source else "_"
 
     async def send(
         self,
-        dispatcher: AlconnaDispatcher,
+        converter: TConvert,
         result: Arparma[MessageChain],
         output_text: str | None = None,
         source: MessageEvent | None = None,
     ) -> None:
         app: Ariadne = Ariadne.current()
         help_message: MessageChain = await run_always_await(
-            dispatcher.converter,
+            converter,
             str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
             output_text,
         )
         if isinstance(source, GroupMessage):
             await app.send_group_message(source.sender.group, help_message)
         else:
             await app.send_message(source.sender, help_message)  # type: ignore
 
-    async def property(
-        self,
-        dispatcher: AlconnaDispatcher,
-        result: Arparma[MessageChain],
-        output_text: str | None = None,
-        source: MessageEvent | None = None,
-    ) -> AlconnaProperty[MessageEvent]:
-        if not isinstance(source, MessageEvent) or (result.matched or not output_text):
-            return AlconnaProperty(result, None, source)
-        if dispatcher.send_flag == "stay":
-            return AlconnaProperty(result, output_text, source)
-        if dispatcher.send_flag == "reply":
-            await self.send(dispatcher, result, output_text, source)
-        elif dispatcher.send_flag == "post":
-            with suppress(LookupError):
-                interface = DispatcherInterface.ctx.get()
-                dispatchers = resolve_dispatchers_mixin([source.Dispatcher, ContextDispatcher]) + [
-                    self.Dispatcher(dispatcher.command, output_text, source)
-                ]
-                for listener in interface.broadcast.default_listener_generator(AlconnaOutputMessage):
-                    await interface.broadcast.Executor(listener, dispatchers)
-                    listener.oplog.clear()
-        return AlconnaProperty(result, None, source)
-
     def fetch_name(self, path: str) -> Depend:
-        async def __wrapper__(app: Ariadne, result: AlconnaProperty):
+        async def __wrapper__(app: Ariadne, result: CommandResult):
             event = result.source
             arp = result.result
             if t := arp.all_matched_args.get(path, None):
                 return t.representation or (await app.get_user_profile(t.target)).nickname if isinstance(t, At) else t
             elif isinstance(event.sender, Friend):
                 return event.sender.nickname
             else:
@@ -110,28 +84,31 @@
                     return True
             if isinstance(match, At) and match.target == app.account:
                 return True
             raise ExecutionStop
 
         return Depend(__wrapper__)
 
-    def alcommand(
-        self, dispatcher: AlconnaDispatcher, guild: bool, private: bool, private_name: str, guild_name: str
-    ) -> Callable[[Callable, dict[str, Any]], AlconnaSchema]:
-        def wrapper(func: Callable, buffer: dict[str, Any]):
-            events = []
-            if guild:
-                events.append(GroupMessage)
-            if private:
-                events.append(FriendMessage)
-            buffer.setdefault("dispatchers", []).append(dispatcher)
-            listen(*events)(func)  # noqa
-            return AlconnaSchema(dispatcher.command)
-
-        return wrapper
+    def handle_listen(
+        self,
+        func: Callable,
+        buffer: dict[str, Any],
+        dispatcher: BaseDispatcher,
+        guild: bool,
+        private: bool,
+        private_name: str,
+        guild_name: str
+    ) -> None:
+        events = []
+        if guild:
+            events.append(GroupMessage)
+        if private:
+            events.append(FriendMessage)
+        buffer.setdefault("dispatchers", []).append(dispatcher)
+        listen(*events)(func)
 
 
 class AriadneMessageChainArgv(BaseMessageChainArgv):
     ...
 
 
 set_default_argv_type(AriadneMessageChainArgv)
```

### Comparing `arclet-alconna-ariadne-0.13.3/src/arclet/alconna/ariadne/typings.py` & `arclet-alconna-ariadne-0.14.0/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.3/PKG-INFO` & `arclet-alconna-ariadne-0.14.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.13.3
+Version: 0.14.0
 Summary: Support Alconna to GraiaProject/Ariadne
 License: AGPL-3.0
 Keywords: alconna,graia,arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -89,15 +89,15 @@
 
 ### 单文件
 
 ariadne:
 
 ```python
 from arclet.alconna import Args
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult
 from arclet.alconna.graia.service import AlconnaGraiaService
 import arclet.alconna.ariadne
 ...
 manager = Launart(...)
 manager.add_service(AlconnaGraiaService())
 app = Ariadne(...)
 
@@ -106,27 +106,27 @@
 
 @app.broadcast.receiver(
     GroupMessage,
     dispatchers=[AlconnaDispatcher(alc, send_flag='stay')]
 )
 async def test2(
     group: Group,
-    result: AlconnaProperty[GroupMessage],
+    result: CommandResult[GroupMessage],
     sth: Match[str]
 ):
     print("sign:", result.result)
     print("sender:", group)
     print("match", sth.available, sth.result)
 ```
 
 avilla:
 
 ```python
 from arclet.alconna import Args
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult
 from arclet.alconna.graia.service import AlconnaGraiaService
 import arclet.alconna.avilla
 ...
 broadcast = create(Broadcast)
 manager = Launart(...)
 manager.add_service(AlconnaGraiaService())
 avilla = Avilla(...)
@@ -136,36 +136,36 @@
 
 @broadcast.receiver(
     MessageReceived,
     dispatchers=[AlconnaDispatcher(alc, send_flag='stay')]
 )
 async def test2(
     context: Context,
-    result: AlconnaProperty[MessageReceived],
+    result: CommandResult[MessageReceived],
     sth: Match[str]
 ):
     print("sign:", result.result)
     print("sender:", context.scene)
     print("match", sth.available, sth.result)
 ```
 
 ### 使用 Saya
 
 in module.py:
 ```python
-from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, AlconnaProperty, AlconnaSchema
+from arclet.alconna.graia import Alconna, AlconnaDispatcher, Match, CommandResult, AlconnaSchema
 from arclet.alconna import Args
 ...
 channel = Channel.current()
 
 alc = Alconna("!jrrp", Args["sth", str, 1123])
 
 @channel.use(AlconnaSchema(AlconnaDispatcher(alc)))
 @channel.use(ListenerSchema([...]))
-async def test2(result: AlconnaProperty[...], sth: Match[str]):
+async def test2(result: CommandResult[...], sth: Match[str]):
     print("sign:", result.result)
     print("match", sth.available, sth.result)
 
 
 ```
 
 in main.py:
@@ -251,15 +251,15 @@
 ```
 
 `command`: 使用的 Alconna 指令
 
 `send_flag`: 解析期间输出信息的发送方式
 - reply: 直接发送给指令发送者
 - post: 以事件通过 Broadcast 广播
-- stay: 存入 AlconnaProperty 传递给事件处理器
+- stay: 存入 CommandResult 传递给事件处理器
 
 `skip_for_unmatch`: 解析失败时是否跳过, 否则错误信息按 send_flag 处理
 
 `comp_session`: 补全会话配置, 不传入则不启用补全会话
 
 `message_converter`: send_flag 为 reply 时 输出信息的预处理器
```


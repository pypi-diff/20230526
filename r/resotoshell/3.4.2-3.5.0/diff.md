# Comparing `tmp/resotoshell-3.4.2.tar.gz` & `tmp/resotoshell-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.4.2.tar", last modified: Wed May 10 12:23:03 2023, max compression
+gzip compressed data, was "resotoshell-3.5.0.tar", last modified: Fri May 26 18:25:25 2023, max compression
```

## Comparing `resotoshell-3.4.2.tar` & `resotoshell-3.5.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:20:33.000000 resotoshell-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-10 12:23:03.671552 resotoshell-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-10 12:20:33.000000 resotoshell-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:20:33.000000 resotoshell-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.667552 resotoshell-3.4.2/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:23:03.671552 resotoshell-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-10 12:20:33.000000 resotoshell-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-10 12:20:33.000000 resotoshell-3.4.2/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-10 12:20:33.000000 resotoshell-3.4.2/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:43.000000 resotoshell-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-26 18:25:25.456874 resotoshell-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-26 18:21:43.000000 resotoshell-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 18:21:43.000000 resotoshell-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.452874 resotoshell-3.5.0/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35784 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 18:25:25.456874 resotoshell-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 18:21:43.000000 resotoshell-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_protected_files.py
```

### Comparing `resotoshell-3.4.2/PKG-INFO` & `resotoshell-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.4.2
+Version: 3.5.0
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.4.2/README.md` & `resotoshell-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.2/resotoshell/__main__.py` & `resotoshell-3.5.0/resotoshell/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import asyncio
 import os
 import sys
 from argparse import Namespace
 from datetime import datetime
 from signal import SIGTERM
 from threading import Event
-from typing import Callable
 
 from prompt_toolkit.formatted_text import FormattedText
 from resotoclient.async_client import ResotoClient
 from rich.console import Console
 
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.core import resotocore, add_args as core_add_args, wait_for_resotocore
 from resotolib.core.ca import TLSData
 from resotolib.jwt import add_args as jwt_add_args
 from resotolib.logger import log, setup_logger, add_args as logging_add_args
+from resotoshell import authorized_client
 from resotoshell.promptsession import PromptSession, core_metadata
-from resotoshell.shell import Shell
+from resotoshell.shell import Shell, ShutdownShellError
 
 
 async def main_async() -> None:
     resotolib.proc.parent_pid = os.getpid()
     setup_logger("resotoshell", json_format=False)
     arg_parser = ArgumentParser(description="resoto shell", env_args_prefix="RESOTOSHELL_")
     core_add_args(arg_parser)
@@ -35,24 +35,19 @@
     try:
         wait_for_resotocore(resotocore.http_uri, timeout=args.resotocore_wait)
     except TimeoutError:
         log.fatal(f"resotocore is not online at {resotocore.http_uri}")
         sys.exit(1)
     resotolib.proc.initializer()
 
-    client = ResotoClient(
-        url=resotocore.http_uri,
-        psk=args.psk,
-        custom_ca_cert_path=args.ca_cert,
-        verify=args.verify_certs,
-    )
+    client = await authorized_client.new_client(args)
 
     async def check_system_info() -> None:
         try:
-            async for line in client.cli_execute("system info"):
+            async for _ in client.cli_execute("system info"):
                 break
         except Exception as e:
             log.error(f"resotocore is not accessible: {e}")
             raise e
 
     try:
         await client.start()
@@ -62,14 +57,17 @@
         sys.exit(1)
     if args.stdin or not sys.stdin.isatty():
         await handle_from_stdin(client)
     else:
         cmds, kinds, props = await core_metadata(client)
         session = PromptSession(cmds=cmds, kinds=kinds, props=props)
         await repl(client, args, session)
+
+    # update the eventually changed auth token
+    await authorized_client.update_auth_header(client)
     await client.shutdown()
 
 
 async def repl(client: ResotoClient, args: Namespace, session: PromptSession) -> None:
     shutdown_event = Event()
     shell = Shell(client, True, detect_color_system(args))
     log.debug("Starting interactive session")
@@ -89,15 +87,15 @@
                     continue
                 if command == "quit":
                     shutdown_event.set()
                     continue
                 await shell.handle_command(command)
             except KeyboardInterrupt:
                 pass
-            except EOFError:
+            except (EOFError, ShutdownShellError):
                 shutdown_event.set()
             except (RuntimeError, ValueError) as e:
                 log.error(e)
             except Exception:
                 log.exception("Caught unhandled exception while processing CLI command")
     finally:
         if event_listener:
@@ -154,23 +152,14 @@
         }
         cs = lookup.get(Console().color_system, "standard")
         log.debug(f"Detected color system is: {cs}")
         return cs
 
 
 def add_args(arg_parser: ArgumentParser) -> None:
-    def is_file(message: str) -> Callable[[str], str]:
-        def check_file(path: str) -> str:
-            if os.path.isfile(path):
-                return path
-            else:
-                raise AttributeError(f"{message}: path {path} is not a directory!")
-
-        return check_file
-
     arg_parser.add_argument(
         "--resotocore-section",
         help="All queries are interpreted with this section name. If not set, the server default is used.",
         dest="resotocore_section",
     )
     arg_parser.add_argument(
         "--resotocore-graph",
```

### Comparing `resotoshell-3.4.2/resotoshell/promptsession.py` & `resotoshell-3.5.0/resotoshell/promptsession.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,15 @@
             option_group_defined = False
             if group := ag.arg.option_group if ag else None:
                 option_group_defined = any(
                     a.arg.name in parts for a in self.args.values() if a.arg.option_group == group
                 )
 
             # if we come here: this is a valid completion
-            return False if already_defined or another_value_defined or option_group_defined else True
+            return not (already_defined or another_value_defined or option_group_defined)
 
         # either there is no option or an option has been started
         if adapted_stripped == "" or start_arg:
             last_doc = Document(
                 last,
                 cursor_position=document.cursor_position - (len(document.text) - len(last)),
             )
```

### Comparing `resotoshell-3.4.2/resotoshell/protected_files.py` & `resotoshell-3.5.0/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.2/resotoshell/shell.py` & `resotoshell-3.5.0/resotoshell/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     "standard": ColorDepth.DEPTH_8_BIT,
     "eight_bit": ColorDepth.DEPTH_8_BIT,
     "truecolor": ColorDepth.DEPTH_24_BIT,
     "legacy_windows": ColorDepth.DEPTH_4_BIT,
 }
 
 
+class ShutdownShellError(Exception):
+    pass
+
+
 class Shell:
     def __init__(
         self,
         client: ResotoClient,
         tty: bool,
         color_system: str,
         graph: Optional[str] = None,
@@ -82,14 +86,17 @@
                             command=command,
                             files=to_upload,
                             graph=self.graph,
                             section=self.section,
                             headers=headers,
                         )
                         await handle_response(mp, True)
+                    elif response.status_code == 401:
+                        self.stderr("Session invalid. Please restart and login again.")
+                        raise ShutdownShellError()
                     else:
                         log.debug(f"HTTP error, code: {response.status_code}")
                         self.stderr(await response.text())
                         return
 
         try:
             received_response = await self.client.cli_execute_raw(
@@ -103,14 +110,16 @@
         except ConnectionError:
             err = (
                 "Error: Could not communicate with resotocore"
                 f" at {urlsplit(self.client.resotocore_url).netloc}."
                 " Is it up and reachable?"
             )
             self.stderr(err)
+        except ShutdownShellError:
+            raise
         except Exception as ex:
             self.stderr(f"Error performing command: `{command}`\nReason: {ex}")
 
     async def handle_result(
         self,
         response: Union[HttpResponse, aiohttp.BodyPartReader, aiohttp.MultipartReader],
         first: bool = True,
```

### Comparing `resotoshell-3.4.2/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.5.0/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.4.2
+Version: 3.5.0
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.4.2/setup.py` & `resotoshell-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.2/test/test_promptsession.py` & `resotoshell-3.5.0/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.2/test/test_protected_files.py` & `resotoshell-3.5.0/test/test_protected_files.py`

 * *Files identical despite different names*


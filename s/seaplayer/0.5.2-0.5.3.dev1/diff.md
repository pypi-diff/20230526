# Comparing `tmp/seaplayer-0.5.2.tar.gz` & `tmp/seaplayer-0.5.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.2.tar", max compression
+gzip compressed data, was "seaplayer-0.5.3.dev1.tar", max compression
```

## Comparing `seaplayer-0.5.2.tar` & `seaplayer-0.5.3.dev1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.2/LICENSE
--rw-r--r--   0        0        0     1722 2023-05-26 18:01:01.483976 seaplayer-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.2/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.2/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.2/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.2/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.2/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.2/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.2/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.2/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1236 2023-05-26 17:54:46.502092 seaplayer-0.5.2/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-25 19:18:33.271766 seaplayer-0.5.2/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-25 19:18:12.427286 seaplayer-0.5.2/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     4310 2023-05-26 17:59:54.881739 seaplayer-0.5.2/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      390 2023-05-26 17:56:14.784901 seaplayer-0.5.2/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 17:51:53.658632 seaplayer-0.5.2/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      817 2023-05-26 16:11:34.702097 seaplayer-0.5.2/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:07:48.169014 seaplayer-0.5.2/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     7967 2023-05-26 17:54:30.962481 seaplayer-0.5.2/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 16:40:30.212986 seaplayer-0.5.2/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.2/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.2/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.2/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    19615 2023-05-26 14:21:54.328149 seaplayer-0.5.2/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1463 2023-05-26 17:53:46.300187 seaplayer-0.5.2/seaplayer/units.py
--rw-r--r--   0        0        0     2831 1970-01-01 00:00:00.000000 seaplayer-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.3.dev1/LICENSE
+-rw-r--r--   0        0        0     1727 2023-05-26 20:39:52.670544 seaplayer-0.5.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.3.dev1/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.3.dev1/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev1/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.3.dev1/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.3.dev1/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev1/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.3.dev1/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.3.dev1/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev1/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.3.dev1/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev1/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.3.dev1/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.3.dev1/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.3.dev1/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1236 2023-05-26 18:16:55.015726 seaplayer-0.5.3.dev1/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.3.dev1/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.3.dev1/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.3.dev1/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     4980 2023-05-26 20:35:00.054615 seaplayer-0.5.3.dev1/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.3.dev1/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.3.dev1/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.3.dev1/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 19:49:05.778773 seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     7967 2023-05-26 18:16:55.019724 seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev1/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.3.dev1/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.3.dev1/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    19615 2023-05-26 18:16:55.021730 seaplayer-0.5.3.dev1/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.3.dev1/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1468 2023-05-26 20:40:03.758787 seaplayer-0.5.3.dev1/seaplayer/units.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.3.dev1/PKG-INFO
```

### Comparing `seaplayer-0.5.2/LICENSE` & `seaplayer-0.5.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/pyproject.toml` & `seaplayer-0.5.3.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.2"
+version = "0.5.3.dev1"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
```

### Comparing `seaplayer-0.5.2/README.md` & `seaplayer-0.5.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.3.dev1/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/codecs/Any.py` & `seaplayer-0.5.3.dev1/seaplayer/codecs/Any.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.3.dev1/seaplayer/codecs/MIDI.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/codecs/WAV.py` & `seaplayer-0.5.3.dev1/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/codeсbase.py` & `seaplayer-0.5.3.dev1/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/config.py` & `seaplayer-0.5.3.dev1/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/css/objects.css` & `seaplayer-0.5.3.dev1/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/css/seaplayer.css` & `seaplayer-0.5.3.dev1/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/functions.py` & `seaplayer-0.5.3.dev1/seaplayer/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/modules/colorizer.py` & `seaplayer-0.5.3.dev1/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/Configurate.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/Image.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/Input.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/Log.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/MusicList.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/Notification.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.3.dev1/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.3.dev1/seaplayer/plug/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import os
 import click
+import shutil
 from rich.console import Console
+from rich.live import Live
 # > Local Import's
 from .exceptions import *
-from ...units import PLUGINS_CONFIG_PATH
+from .vars import CREATE_DEFAULT_CODE
+from ...units import PLUGINS_CONFIG_PATH, PLUGINS_DIRPATH
 from ..pluginbase import PluginInfo
 from ..pluginloader import PluginLoaderConfigManager
 from .functions import (
     init_config,
     is_config_inited,
     get_plugins_info,
     raise_exception,
     is_plugin_dirpath
 )
 
-# ! Vars
+# ! Init
 console = Console()
 plugin_config = PluginLoaderConfigManager(PLUGINS_CONFIG_PATH)
 
-CREATE_DEFAULT_CODE = """\
-from seaplayer.plug import PluginBase
-
-class Plugin(PluginBase):
-    pass
-
-plugin_main = Plugin
-"""
-
 # ! Commands
 @click.command("enable", help="Enabling plugin.")
 @click.argument("plugin_name_id")
 def enabling(plugin_name_id: str):
     if plugin_config.exists_plugin_by_name_id(plugin_name_id):
         plugin_config.enable_plugin_by_name_id(plugin_name_id)
         console.print(f"[yellow]The {repr(plugin_name_id)} plug-in is [green]enabled[/green].[/yellow]")
@@ -90,19 +84,15 @@
     type=str, default=None
 )
 @click.option(
     "--recreate", "recreate",
     help="Ignores if there is already a plugin in the folder and overwrites it.",
     is_flag=True, default=False
 )
-def creating(
-    dirpath: str,
-    recreate: bool,
-    **kwargs: str
-):
+def creating(dirpath: str, recreate: bool, **kwargs: str):
     dirpath = os.path.abspath(dirpath)
     try:
         if (not is_plugin_dirpath(dirpath)) or recreate:
             info = PluginInfo(**kwargs)
             
             with open(os.path.join(dirpath, "info.json"), "w", encoding="utf-8") as file:
                 file.write(info.json())
@@ -111,14 +101,30 @@
             
             console.print("[yellow]The plugin directory has been [green]created[/green].[/yellow]")
         else:
             raise_exception(console, IsPluginDirectoryError, dirpath)
     except:
         console.print_exception()
 
+@click.command("load", help="Load the plugin into the SeaPlayer plugins directory.")
+@click.argument("dirpath", type=click.Path(True, False))
+def loading(dirpath: str):
+    dirpath = os.path.abspath(dirpath)
+    if is_plugin_dirpath(dirpath):
+        with Live("[yellow]Loading...[/yellow]", console=console) as l:
+            shutil.copytree(
+                dirpath,
+                os.path.join(PLUGINS_DIRPATH, os.path.basename(dirpath)),
+                dirs_exist_ok=True
+            )
+            init_config()
+            l.update("[yellow]Plugin [green]loaded[/green]![/yellow]", refresh=True)
+    else:
+        raise_exception(console, IsNotPluginDirectoryError, dirpath)
+
 # ! Main Group
 @click.group
 @click.option(
     "--init-config", "initialization_config",
     help="Forced (re)initialisation of the config.",
     is_flag=True, default=False
 )
@@ -127,7 +133,8 @@
         init_config()
 
 # ! Main Group Bind Commands
 main.add_command(enabling)
 main.add_command(disabling)
 main.add_command(listing)
 main.add_command(creating)
+main.add_command(loading)
```

### Comparing `seaplayer-0.5.2/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.3.dev1/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.3.dev1/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.3.dev1/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/screens/Configurate.py` & `seaplayer-0.5.3.dev1/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/screens/Unknown.py` & `seaplayer-0.5.3.dev1/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/seaplayer.py` & `seaplayer-0.5.3.dev1/seaplayer/seaplayer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/types/Convert.py` & `seaplayer-0.5.3.dev1/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/types/MusicList.py` & `seaplayer-0.5.3.dev1/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.2/seaplayer/units.py` & `seaplayer-0.5.3.dev1/seaplayer/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.2"
+__version__ = "0.5.3.dev1"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.2/PKG-INFO` & `seaplayer-0.5.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.2
+Version: 0.5.3.dev1
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
```


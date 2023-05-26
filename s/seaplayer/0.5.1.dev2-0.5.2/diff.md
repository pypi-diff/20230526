# Comparing `tmp/seaplayer-0.5.1.dev2.tar.gz` & `tmp/seaplayer-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.1.dev2.tar", max compression
+gzip compressed data, was "seaplayer-0.5.2.tar", max compression
```

## Comparing `seaplayer-0.5.1.dev2.tar` & `seaplayer-0.5.2.tar`

### file list

```diff
@@ -1,45 +1,51 @@
--rw-r--r--   0        0        0     1064 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/LICENSE
--rw-r--r--   0        0        0     1304 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/README.md
--rw-r--r--   0        0        0     1450 2023-05-24 20:48:50.932426 seaplayer-0.5.1.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__init__.py
--rw-r--r--   0        0        0      331 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0     2415 2023-05-24 19:25:42.492196 seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      459 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2860 2023-05-24 19:26:44.687111 seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      455 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      457 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      574 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0      254 2023-05-24 15:00:37.735912 seaplayer-0.5.1.dev2/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     1859 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6031 2023-05-24 19:05:33.708654 seaplayer-0.5.1.dev2/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1491 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/objects.css
--rw-r--r--   0        0        0      555 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      260 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      374 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1367 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     1975 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0     1022 2023-05-24 15:31:52.607550 seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     2938 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1094 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Input.py
--rw-r--r--   0        0        0      950 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5430 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      759 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1240 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0      316 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0       85 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      730 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     6978 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2100 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0     9316 2023-05-24 20:38:01.064915 seaplayer-0.5.1.dev2/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0      982 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0       83 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0    18891 2023-05-24 20:28:20.713484 seaplayer-0.5.1.dev2/seaplayer/seaplayer.py
--rw-r--r--   0        0        0     2547 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1553 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0       63 2023-05-24 14:13:35.295929 seaplayer-0.5.1.dev2/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1407 2023-05-24 20:49:18.523757 seaplayer-0.5.1.dev2/seaplayer/units.py
--rw-r--r--   0        0        0     2653 1970-01-01 00:00:00.000000 seaplayer-0.5.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1722 2023-05-26 18:01:01.483976 seaplayer-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.2/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.2/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.2/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.2/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.2/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.2/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.2/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.2/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.2/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2036 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.2/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.2/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.2/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.2/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1236 2023-05-26 17:54:46.502092 seaplayer-0.5.2/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5562 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.2/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-25 19:18:33.271766 seaplayer-0.5.2/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-25 19:18:12.427286 seaplayer-0.5.2/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     4310 2023-05-26 17:59:54.881739 seaplayer-0.5.2/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      390 2023-05-26 17:56:14.784901 seaplayer-0.5.2/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 17:51:53.658632 seaplayer-0.5.2/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      817 2023-05-26 16:11:34.702097 seaplayer-0.5.2/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:07:48.169014 seaplayer-0.5.2/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     7967 2023-05-26 17:54:30.962481 seaplayer-0.5.2/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 16:40:30.212986 seaplayer-0.5.2/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.2/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.2/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.2/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    19615 2023-05-26 14:21:54.328149 seaplayer-0.5.2/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       64 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.2/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1463 2023-05-26 17:53:46.300187 seaplayer-0.5.2/seaplayer/units.py
+-rw-r--r--   0        0        0     2831 1970-01-01 00:00:00.000000 seaplayer-0.5.2/PKG-INFO
```

### Comparing `seaplayer-0.5.1.dev2/LICENSE` & `seaplayer-0.5.2/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Romanin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Romanin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `seaplayer-0.5.1.dev2/README.md` & `seaplayer-0.5.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<div id="header" align="center">
-    <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
-</div>
-<div id="header" align="center"><h1>SeaPlayer</h1></div>
-
-## Descriptions
-SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` and `FLAC` files.
-
-## Install
-
-
-1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
-2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
-3.  ```
-    pip install --upgrade seaplayer
-    ```
-
-### For MIDI playback
-***If you have Windows*** you can skip this part as ***Windows*** has a default decoder for `MIDI` and ***does not need to be installed***.
-
-
-***For Linux or MacOS users:***
-
-You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
-
-## Using
-```shell
-python -m seaplayer # Method for `downloaded repository` or `installed via pip`
-```
-
-![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
-![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
+<div id="header" align="center">
+    <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
+</div>
+<div id="header" align="center"><h1>SeaPlayer</h1></div>
+
+## Descriptions
+SeaPlayer is a player that works in the terminal. Works with `MP3`, `OGG`, `WAV`, `MIDI` and `FLAC` files.
+
+## Install
+
+
+1. You can use [Release](https://github.com/romanin-rf/sea-player/releases)
+2. ***Download clone repository*** install the dependencies from `requirements.txt` and run via [Python](https://www.python.org).
+3.  ```
+    pip install --upgrade seaplayer
+    ```
+
+### For MIDI playback
+***If you have Windows*** you can skip this part as ***Windows*** has a default decoder for `MIDI` and ***does not need to be installed***.
+
+
+***For Linux or MacOS users:***
+
+You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
+
+## Using
+```shell
+python -m seaplayer # Method for `downloaded repository` or `installed via pip`
+```
+
+![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
+![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
```

### Comparing `seaplayer-0.5.1.dev2/pyproject.toml` & `seaplayer-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-[tool.poetry]
-name = "SeaPlayer"
-version = "0.5.1.dev2"
-description = "SeaPlayer is a player that works in the terminal."
-repository = "https://github.com/romanin-rf/SeaPlayer"
-authors = ["Romanin <semina054@gmail.com>"]
-keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
-license = "MIT"
-readme = "README.md"
-classifiers = [
-    "Environment :: Console",
-    "Operating System :: Microsoft :: Windows :: Windows 10",
-    "Operating System :: Microsoft :: Windows :: Windows 11",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
-]
-packages = [{ include = "seaplayer" }]
-include = [
-    "seaplayer/modules/__init__.py",
-    "seaplayer/modules/colorizer.py",
-    "seaplayer/assets/image-not-found.png",
-    "seaplayer/css/configurate.css",
-    "seaplayer/css/objects.css",
-    "seaplayer/css/seaplayer.css",
-    "seaplayer/css/unknown.css"
-]
-
-[tool.poetry.scripts]
-seaplayer = "seaplayer.__main__:run"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pillow = "^9.5.0"
-aiofiles = "^23.1.0"
-rich = ">=13.3.5"
-mutagen = "1.45.1"
-textual = ">=0.25.0"
-playsoundsimple-py = "0.7.0"
-properties-py = "1.1.0"
-typing-inspect = "^0.8.0"
-ripix = ">=2.2.3"
-platformdirs = "^3.5.1"
-pydantic = "^1.10.7"
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "SeaPlayer"
+version = "0.5.2"
+description = "SeaPlayer is a player that works in the terminal."
+repository = "https://github.com/romanin-rf/SeaPlayer"
+authors = ["Romanin <semina054@gmail.com>"]
+keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
+license = "MIT"
+readme = "README.md"
+classifiers = [
+    "Environment :: Console",
+    "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Operating System :: Microsoft :: Windows :: Windows 11",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: MacOS",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
+]
+packages = [{ include = "seaplayer" }]
+include = [
+    "seaplayer/modules/__init__.py",
+    "seaplayer/modules/colorizer.py",
+    "seaplayer/assets/image-not-found.png",
+    "seaplayer/css/configurate.css",
+    "seaplayer/css/objects.css",
+    "seaplayer/css/seaplayer.css",
+    "seaplayer/css/unknown.css"
+]
+
+[tool.poetry.scripts]
+seaplayer = "seaplayer.__main__:run"
+seaplug = "seaplayer.plug.__main__:run"
+
+[tool.poetry.dependencies]
+python = "^3.9,<3.12"
+pillow = "^9.5.0"
+aiofiles = "^23.1.0"
+rich = ">=13.3.5"
+mutagen = "1.45.1"
+textual = ">=0.25.0"
+playsoundsimple-py = "0.7.0"
+properties-py = "1.1.0"
+typing-inspect = "^0.8.0"
+ripix = ">=2.2.3"
+platformdirs = "^3.5.1"
+pydantic = "^1.10.7"
+poetry = {version = "^1.5.0", optional = true}
+pyinstaller = {version = "^5.11.0", optional = true}
+click = "^8.1.3"
+
+[tool.poetry.extras]
+build = ["poetry", "pyinstaller"]
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.2/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.1.dev2/seaplayer/codecs/Any.py` & `seaplayer-0.5.2/seaplayer/codecs/Any.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import os
-import hashlib
-import aiofiles
-# > Sound Works
-from playsoundsimple import Sound
-# > Typing
-from typing import Optional
-# > Local Imports
-from ..codeсbase import CodecBase
-
-
-class AnyCodec(CodecBase):
-    codec_name: str = "Any"
-    
-    # ! Initialized
-    def __init__(self, path: str, sound_device_id: Optional[int]=None, **kwargs) -> None:
-        self.name = os.path.abspath(path)
-        self._sound = Sound(self.name, device_id=sound_device_id)
-    
-    def __sha1__(self, buffer_size: int) -> str:
-        sha1 = hashlib.sha1()
-        with open(self.name, "rb") as file:
-            while True:
-                data = file.read(buffer_size)
-                if not data: break
-                sha1.update(data)
-        return sha1.hexdigest()
-    
-    async def __aio_sha1__(self, buffer_size: int) -> str:
-        sha1 = hashlib.sha1()
-        async with aiofiles.open(self.name, "rb") as file:
-            while True:
-                data = await file.read(buffer_size)
-                if not data: break
-                sha1.update(data)
-        return sha1.hexdigest()
-    
-    # ! Info
-    @property
-    def duration(self) -> float: return self._sound.duration
-    @property
-    def channels(self) -> int: return self._sound.channels
-    @property
-    def samplerate(self) -> int: return self._sound.samplerate
-    @property
-    def bitrate(self) -> int: return self._sound.bitrate
-    
-    # ! Playback Info
-    @property
-    def playing(self) -> bool: return self._sound.playing
-    @property
-    def paused(self) -> bool: return self._sound.paused
-    
-    # ! Sound Info
-    @property
-    def title(self) -> Optional[str]: return self._sound.title
-    @property
-    def artist(self) -> Optional[str]: return self._sound.artist
-    @property
-    def album(self) -> Optional[str]: return self._sound.album
-    @property
-    def icon_data(self) -> Optional[bytes]: return self._sound.icon_data
-    
-    # ! Functions
-    def play(self) -> None: self._sound.play()
-    def stop(self) -> None: self._sound.stop()
-    def pause(self) -> None: self._sound.pause()
-    def unpause(self) -> None: self._sound.unpause()
-    def get_volume(self) -> float: return self._sound.get_volume()
-    def set_volume(self, value: float) -> None: self._sound.set_volume(value)
-    def get_pos(self) -> float: return self._sound.get_pos()
+import os
+import hashlib
+import aiofiles
+# > Sound Works
+from playsoundsimple import Sound
+# > Typing
+from typing import Optional
+# > Local Imports
+from ..codeсbase import CodecBase
+
+
+class AnyCodec(CodecBase):
+    codec_name: str = "Any"
+    
+    # ! Initialized
+    def __init__(self, path: str, sound_device_id: Optional[int]=None, **kwargs) -> None:
+        self.name = os.path.abspath(path)
+        self._sound = Sound(self.name, device_id=sound_device_id)
+    
+    def __sha1__(self, buffer_size: int) -> str:
+        sha1 = hashlib.sha1()
+        with open(self.name, "rb") as file:
+            while True:
+                data = file.read(buffer_size)
+                if not data: break
+                sha1.update(data)
+        return sha1.hexdigest()
+    
+    async def __aio_sha1__(self, buffer_size: int) -> str:
+        sha1 = hashlib.sha1()
+        async with aiofiles.open(self.name, "rb") as file:
+            while True:
+                data = await file.read(buffer_size)
+                if not data: break
+                sha1.update(data)
+        return sha1.hexdigest()
+    
+    # ! Info
+    @property
+    def duration(self) -> float: return self._sound.duration
+    @property
+    def channels(self) -> int: return self._sound.channels
+    @property
+    def samplerate(self) -> int: return self._sound.samplerate
+    @property
+    def bitrate(self) -> int: return self._sound.bitrate
+    
+    # ! Playback Info
+    @property
+    def playing(self) -> bool: return self._sound.playing
+    @property
+    def paused(self) -> bool: return self._sound.paused
+    
+    # ! Sound Info
+    @property
+    def title(self) -> Optional[str]: return self._sound.title
+    @property
+    def artist(self) -> Optional[str]: return self._sound.artist
+    @property
+    def album(self) -> Optional[str]: return self._sound.album
+    @property
+    def icon_data(self) -> Optional[bytes]: return self._sound.icon_data
+    
+    # ! Functions
+    def play(self) -> None: self._sound.play()
+    def stop(self) -> None: self._sound.stop()
+    def pause(self) -> None: self._sound.pause()
+    def unpause(self) -> None: self._sound.unpause()
+    def get_volume(self) -> float: return self._sound.get_volume()
+    def set_volume(self, value: float) -> None: self._sound.set_volume(value)
+    def get_pos(self) -> float: return self._sound.get_pos()
     def set_pos(self, value: float) -> None: self._sound.set_pos(value)
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.2/seaplayer/codecs/MIDI.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import os
-import asyncio
-import aiofiles
-import subprocess
-from tempfile import mkstemp
-# > Sound Works
-from playsoundsimple import Sound
-from playsoundsimple.units import SOUND_FONTS_PATH, FLUID_SYNTH_PATH
-from playsoundsimple.exceptions import FileTypeError
-from playsoundsimple.player import SoundFP, get_sound_filepath
-# > Typing Import
-from typing import Optional
-# > Local Imports
-from .Any import AnyCodec
-
-
-# ! Codec Types
-class MIDISound(Sound):
-    async def aio_from_midi(
-        fp: SoundFP,
-        sound_fonts_path: Optional[str]=None,
-        **kwargs
-    ):
-        path, is_temp = get_sound_filepath(fp, filetype=".midi")
-        sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
-        if path is None: raise FileTypeError(fp)
-        npath = mkstemp(suffix=".wav")[1]
-        
-        process = await asyncio.create_subprocess_exec(
-            FLUID_SYNTH_PATH, "-ni", sound_fonts_path, path, "-F", npath, "-q",
-            stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-        )
-        await process.wait()
-        
-        if is_temp:
-            try: os.remove(path)
-            except: pass
-        
-        return Sound(npath, **{"is_temp": True, **kwargs})
-    
-    def from_midi(
-        fp: SoundFP,
-        sound_fonts_path: Optional[str]=None,
-        **kwargs
-    ):
-        path, is_temp = get_sound_filepath(fp, filetype=".midi")
-        sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
-        if path is None: raise FileTypeError(fp)
-        npath = mkstemp(suffix=".wav")[1]
-        
-        subprocess.call(
-            [FLUID_SYNTH_PATH, "-ni", sound_fonts_path, path, "-F", npath, "-q"],
-            stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
-        )
-        
-        if is_temp:
-            try: os.remove(path)
-            except: pass
-        
-        return Sound(npath, **{"is_temp": True, **kwargs})
-
-# ! Codec
-class MIDICodec(AnyCodec):
-    codec_name: str = "MIDI"
-    
-    # ! Testing
-    @staticmethod
-    def is_this_codec(path: str) -> bool:
-        with open(path, 'rb') as file:
-            return file.read(4) == b"MThd"
-    
-    @staticmethod
-    async def aio_is_this_codec(path: str) -> bool:
-        async with aiofiles.open(path, 'rb') as file:
-            return await file.read(4) == b"MThd"
-    
-    # ! Initialized
-    def __init__(self, path: str, aio_init: bool=False, sound_device_id: Optional[int]=None, **kwargs) -> None:
-        self.name = os.path.abspath(path)
-        if not aio_init:
-            self._sound = MIDISound.from_midi(self.name, device_id=sound_device_id, **kwargs)
-    
-    @staticmethod
-    async def __aio_init__(path: str, sound_device_id: Optional[int]=None, **kwargs):
-        self = MIDICodec(path, aio_init=True)
-        self._sound = await MIDISound.aio_from_midi(self.name, device_id=sound_device_id, **kwargs)
+import os
+import asyncio
+import aiofiles
+import subprocess
+from tempfile import mkstemp
+# > Sound Works
+from playsoundsimple import Sound
+from playsoundsimple.units import SOUND_FONTS_PATH, FLUID_SYNTH_PATH
+from playsoundsimple.exceptions import FileTypeError
+from playsoundsimple.player import SoundFP, get_sound_filepath
+# > Typing Import
+from typing import Optional
+# > Local Imports
+from .Any import AnyCodec
+
+
+# ! Codec Types
+class MIDISound(Sound):
+    async def aio_from_midi(
+        fp: SoundFP,
+        sound_fonts_path: Optional[str]=None,
+        **kwargs
+    ):
+        path, is_temp = get_sound_filepath(fp, filetype=".midi")
+        sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
+        if path is None: raise FileTypeError(fp)
+        npath = mkstemp(suffix=".wav")[1]
+        
+        process = await asyncio.create_subprocess_exec(
+            FLUID_SYNTH_PATH, "-ni", sound_fonts_path, path, "-F", npath, "-q",
+            stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        )
+        await process.wait()
+        
+        if is_temp:
+            try: os.remove(path)
+            except: pass
+        
+        return Sound(npath, **{"is_temp": True, **kwargs})
+    
+    def from_midi(
+        fp: SoundFP,
+        sound_fonts_path: Optional[str]=None,
+        **kwargs
+    ):
+        path, is_temp = get_sound_filepath(fp, filetype=".midi")
+        sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
+        if path is None: raise FileTypeError(fp)
+        npath = mkstemp(suffix=".wav")[1]
+        
+        subprocess.call(
+            [FLUID_SYNTH_PATH, "-ni", sound_fonts_path, path, "-F", npath, "-q"],
+            stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+        )
+        
+        if is_temp:
+            try: os.remove(path)
+            except: pass
+        
+        return Sound(npath, **{"is_temp": True, **kwargs})
+
+# ! Codec
+class MIDICodec(AnyCodec):
+    codec_name: str = "MIDI"
+    
+    # ! Testing
+    @staticmethod
+    def is_this_codec(path: str) -> bool:
+        with open(path, 'rb') as file:
+            return file.read(4) == b"MThd"
+    
+    @staticmethod
+    async def aio_is_this_codec(path: str) -> bool:
+        async with aiofiles.open(path, 'rb') as file:
+            return await file.read(4) == b"MThd"
+    
+    # ! Initialized
+    def __init__(self, path: str, aio_init: bool=False, sound_device_id: Optional[int]=None, **kwargs) -> None:
+        self.name = os.path.abspath(path)
+        if not aio_init:
+            self._sound = MIDISound.from_midi(self.name, device_id=sound_device_id, **kwargs)
+    
+    @staticmethod
+    async def __aio_init__(path: str, sound_device_id: Optional[int]=None, **kwargs):
+        self = MIDICodec(path, aio_init=True)
+        self._sound = await MIDISound.aio_from_midi(self.name, device_id=sound_device_id, **kwargs)
         return self
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/codeсbase.py` & `seaplayer-0.5.2/seaplayer/codeсbase.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from typing import Optional
-
-# ! Functions
-def formater(**kwargs) -> str:
-    return ", ".join([f"{key}={repr(value)}" for key, value in kwargs.items()])
-
-# ! Codecs Base
-class CodecBase:
-    # * Codec Info
-    codec_name: str = "None"
-    
-    # * Info
-    name: str
-    duration: float
-    channels: int
-    samplerate: int
-    bitrate: int
-    
-    # * Sound Info
-    title: Optional[str]
-    artist: Optional[str]
-    album: Optional[str]
-    icon_data: Optional[bytes]
-    
-    # * Playback Info
-    playing: bool
-    paused: bool
-    
-    # ! Initializing Functions
-    def __init__(self, path: str, **kwargs) -> None: ...
-    #async def __aio_init__(self, path: str, **kwargs) -> None: ...
-    def __repr__(self):
-        return \
-            "{0}({1})".format(
-                self.__class__.__name__,
-                formater(
-                    name=self.name,
-                    duration=self.duration,
-                    channels=self.channels,
-                    samplerate=self.samplerate,
-                    bitrate=self.bitrate,
-                    title=self.title,
-                    artist=self.artist,
-                    album=self.album
-                )
-            )
-    
-    def __sha1__(self, buffer_size: int) -> str: ...
-    async def __aio_sha1__(self, buffer_size: int) -> str: ...
-    
-    # ! Testing Functions
-    @staticmethod
-    def is_this_codec(path: str) -> bool: return False
-    @staticmethod
-    async def aio_is_this_codec(path: str) -> bool: return False
-    
-    # ! Playback Functions
-    def play(self) -> None: ...
-    def stop(self) -> None: ...
-    def pause(self) -> None: ...
-    def unpause(self) -> None: ...
-    def get_volume(self) -> float: return 1.0
-    def set_volume(self, value: float) -> None: ...
-    def get_pos(self) -> float: return 0.0
-    def set_pos(self, value: float) -> None: ...
+from typing import Optional
+
+# ! Functions
+def formater(**kwargs) -> str:
+    return ", ".join([f"{key}={repr(value)}" for key, value in kwargs.items()])
+
+# ! Codecs Base
+class CodecBase:
+    # * Codec Info
+    codec_name: str = "None"
+    
+    # * Info
+    name: str
+    duration: float
+    channels: int
+    samplerate: int
+    bitrate: int
+    
+    # * Sound Info
+    title: Optional[str]
+    artist: Optional[str]
+    album: Optional[str]
+    icon_data: Optional[bytes]
+    
+    # * Playback Info
+    playing: bool
+    paused: bool
+    
+    # ! Initializing Functions
+    def __init__(self, path: str, **kwargs) -> None: ...
+    #async def __aio_init__(self, path: str, **kwargs) -> None: ...
+    def __repr__(self):
+        return \
+            "{0}({1})".format(
+                self.__class__.__name__,
+                formater(
+                    name=self.name,
+                    duration=self.duration,
+                    channels=self.channels,
+                    samplerate=self.samplerate,
+                    bitrate=self.bitrate,
+                    title=self.title,
+                    artist=self.artist,
+                    album=self.album
+                )
+            )
+    
+    def __sha1__(self, buffer_size: int) -> str: ...
+    async def __aio_sha1__(self, buffer_size: int) -> str: ...
+    
+    # ! Testing Functions
+    @staticmethod
+    def is_this_codec(path: str) -> bool: return False
+    @staticmethod
+    async def aio_is_this_codec(path: str) -> bool: return False
+    
+    # ! Playback Functions
+    def play(self) -> None: ...
+    def stop(self) -> None: ...
+    def pause(self) -> None: ...
+    def unpause(self) -> None: ...
+    def get_volume(self) -> float: return 1.0
+    def set_volume(self, value: float) -> None: ...
+    def get_pos(self) -> float: return 0.0
+    def set_pos(self, value: float) -> None: ...
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/config.py` & `seaplayer-0.5.2/seaplayer/config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import properties
-from pathlib import Path
-from typing import Dict, Any, Optional, TypeVar, Union, Literal
-
-T = TypeVar("T")
-
-DEFAULT_CONFIG_DATA = {
-    "sound": {
-        "sound_font_path": None,                # * Optional[str]
-        "output_sound_device_id": None,         # * Optional[int]
-    },
-    "image": {
-        "image_update_method": "sync",          # * Literal["sync", "async"]
-        "image_resample_method": "bilinear",    # * Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]
-    },
-    "playback": {
-        "volume_change_percent": 0.05,
-        "rewind_count_seconds": 5,
-        "max_volume_percent": 2.0
-    },
-    "playlist": {
-        "recursive_search": False
-    },
-    "keys": {
-        "quit": "q,й",
-        "rewind_forward": "*",
-        "rewind_back": "/",
-        "volume_up": "+",
-        "volume_down": "-"
-    },
-    "debag": {
-        "log_menu_enable": False
-    }
-}
-
-class SeaPlayerConfig:
-    @staticmethod
-    def dump(filepath: Path, data: Dict[str, Any]) -> None:
-        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
-            properties.dump_tree(data, file)
-    
-    @staticmethod
-    def load(filepath: Path, default: Dict[str, Any]) -> Dict[str, Any]:
-        with open(filepath, "r", encoding="utf-8", errors="ignore") as file:
-            try: return properties.load_tree(file)
-            except: pass
-        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
-            properties.dump_tree(default, file)
-        return default
-    
-    def refresh(self) -> None: self.dump(self.filepath, self.config)
-    
-    def __init__(
-        self,
-        filepath: str,
-        *,
-        default_data: Dict[str, Any]=DEFAULT_CONFIG_DATA
-    ) -> None:
-        self.filepath = Path(filepath)
-        self.default_data = default_data
-        if self.filepath.exists():
-            self.config = self.load(self.filepath, self.default_data)
-            config_temp = self.default_data.copy()
-            config_temp.update(self.config)
-            self.config = config_temp.copy()
-            del config_temp
-        else:
-            self.config = default_data.copy()
-        self.refresh()
-    
-    @staticmethod
-    def tevey(key_path: str, *, sep: str=".") -> str:
-        return "".join([f"[{repr(key)}]" for key in key_path.split(sep)])
-    def get(self, key: str, default: T=None) -> Union[Any, T]:
-        try: return eval(f"self.config{self.tevey(key)}")
-        except: return default
-    def set(self, key: str, value: Any) -> None:
-        try: exec(f"self.config{self.tevey(key)} = value") ; self.refresh()
-        except: pass
-    
-    # ! Sound
-    @property
-    def sound_font_path(self) -> Optional[str]: return self.get("sound.sound_font_path")
-    @sound_font_path.setter
-    def sound_font_path(self, value: Optional[str]): self.set("sound.sound_font_path", value)
-    
-    @property
-    def output_sound_device_id(self) -> Optional[int]: return self.get("sound.output_sound_device_id")
-    @output_sound_device_id.setter
-    def output_sound_device_id(self, value: Optional[int]): self.set("sound.output_sound_device_id", value)
-    
-    # ! Image
-    @property
-    def image_update_method(self) -> Literal["sync", "async"]: return self.get("image.image_update_method")
-    @image_update_method.setter
-    def image_update_method(self, value: Literal["sync", "async"]): self.set("image.image_update_method", value)
-    
-    @property
-    def image_resample_method(self) -> Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]:
-        return self.get("image.image_resample_method")
-    @image_resample_method.setter
-    def image_resample_method(self, value: Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]):
-        self.set("image.image_resample_method", value)
-    
-    # ! Playback
-    @property
-    def volume_change_percent(self) -> float: return self.get("playback.volume_change_percent")
-    @volume_change_percent.setter
-    def volume_change_percent(self, value: float): self.set("playback.volume_change_percent", value)
-    
-    @property
-    def rewind_count_seconds(self) -> int: return self.get("playback.rewind_count_seconds")
-    @rewind_count_seconds.setter
-    def rewind_count_seconds(self, value: int): self.set("playback.rewind_count_seconds", value)
-    
-    @property
-    def max_volume_percent(self) -> float: return self.get("playback.max_volume_percent")
-    @max_volume_percent.setter
-    def max_volume_percent(self, value: float): self.set("playback.max_volume_percent", value)
-    
-    # ! Playlist
-    @property
-    def recursive_search(self) -> bool: return self.get("playlist.recursive_search")
-    @recursive_search.setter
-    def recursive_search(self, value: bool): self.set("playlist.recursive_search", value)
-    
-    # ! Keys
-    @property
-    def key_quit(self) -> str: return self.get("keys.quit")
-    @key_quit.setter
-    def key_quit(self, value: str): self.set("keys.quit", value)
-    
-    @property
-    def key_rewind_forward(self) -> str: return self.get("keys.rewind_forward")
-    @key_rewind_forward.setter
-    def key_rewind_forward(self, value: str): self.set("keys.rewind_forward", value)
-    
-    @property
-    def key_rewind_back(self) -> str: return self.get("keys.rewind_back")
-    @key_rewind_back.setter
-    def key_rewind_back(self, value: str): self.set("keys.rewind_back", value)
-    
-    @property
-    def key_volume_up(self) -> str: return self.get("keys.volume_up")
-    @key_volume_up.setter
-    def key_volume_up(self, value: str): self.set("keys.volume_up", value)
-    
-    @property
-    def key_volume_down(self) -> str: return self.get("keys.volume_down")
-    @key_volume_down.setter
-    def key_volume_down(self, value: str): self.set("keys.volume_down", value)
-    
-    # ! Debag
-    @property
-    def log_menu_enable(self) -> bool: return self.get("debag.log_menu_enable")
-    @log_menu_enable.setter
-    def log_menu_enable(self, value: bool): self.set("debag.log_menu_enable", value)
+import properties
+from pathlib import Path
+from typing import Dict, Any, Optional, TypeVar, Union, Literal
+
+T = TypeVar("T")
+
+DEFAULT_CONFIG_DATA = {
+    "sound": {
+        "sound_font_path": None,                # * Optional[str]
+        "output_sound_device_id": None,         # * Optional[int]
+    },
+    "image": {
+        "image_update_method": "sync",          # * Literal["sync", "async"]
+        "image_resample_method": "bilinear",    # * Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]
+    },
+    "playback": {
+        "volume_change_percent": 0.05,
+        "rewind_count_seconds": 5,
+        "max_volume_percent": 2.0
+    },
+    "playlist": {
+        "recursive_search": False
+    },
+    "keys": {
+        "quit": "q,й",
+        "rewind_forward": "*",
+        "rewind_back": "/",
+        "volume_up": "+",
+        "volume_down": "-"
+    },
+    "debag": {
+        "log_menu_enable": False
+    }
+}
+
+class SeaPlayerConfig:
+    @staticmethod
+    def dump(filepath: Path, data: Dict[str, Any]) -> None:
+        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
+            properties.dump_tree(data, file)
+    
+    @staticmethod
+    def load(filepath: Path, default: Dict[str, Any]) -> Dict[str, Any]:
+        with open(filepath, "r", encoding="utf-8", errors="ignore") as file:
+            try: return properties.load_tree(file)
+            except: pass
+        with open(filepath, "w", encoding="utf-8", errors="ignore") as file:
+            properties.dump_tree(default, file)
+        return default
+    
+    def refresh(self) -> None: self.dump(self.filepath, self.config)
+    
+    def __init__(
+        self,
+        filepath: str,
+        *,
+        default_data: Dict[str, Any]=DEFAULT_CONFIG_DATA
+    ) -> None:
+        self.filepath = Path(filepath)
+        self.default_data = default_data
+        if self.filepath.exists():
+            self.config = self.load(self.filepath, self.default_data)
+            config_temp = self.default_data.copy()
+            config_temp.update(self.config)
+            self.config = config_temp.copy()
+            del config_temp
+        else:
+            self.config = default_data.copy()
+        self.refresh()
+    
+    @staticmethod
+    def tevey(key_path: str, *, sep: str=".") -> str:
+        return "".join([f"[{repr(key)}]" for key in key_path.split(sep)])
+    def get(self, key: str, default: T=None) -> Union[Any, T]:
+        try: return eval(f"self.config{self.tevey(key)}")
+        except: return default
+    def set(self, key: str, value: Any) -> None:
+        try: exec(f"self.config{self.tevey(key)} = value") ; self.refresh()
+        except: pass
+    
+    # ! Sound
+    @property
+    def sound_font_path(self) -> Optional[str]: return self.get("sound.sound_font_path")
+    @sound_font_path.setter
+    def sound_font_path(self, value: Optional[str]): self.set("sound.sound_font_path", value)
+    
+    @property
+    def output_sound_device_id(self) -> Optional[int]: return self.get("sound.output_sound_device_id")
+    @output_sound_device_id.setter
+    def output_sound_device_id(self, value: Optional[int]): self.set("sound.output_sound_device_id", value)
+    
+    # ! Image
+    @property
+    def image_update_method(self) -> Literal["sync", "async"]: return self.get("image.image_update_method")
+    @image_update_method.setter
+    def image_update_method(self, value: Literal["sync", "async"]): self.set("image.image_update_method", value)
+    
+    @property
+    def image_resample_method(self) -> Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]:
+        return self.get("image.image_resample_method")
+    @image_resample_method.setter
+    def image_resample_method(self, value: Literal["nearest", "bilinear", "bicubic", "lanczos", "hamming", "box"]):
+        self.set("image.image_resample_method", value)
+    
+    # ! Playback
+    @property
+    def volume_change_percent(self) -> float: return self.get("playback.volume_change_percent")
+    @volume_change_percent.setter
+    def volume_change_percent(self, value: float): self.set("playback.volume_change_percent", value)
+    
+    @property
+    def rewind_count_seconds(self) -> int: return self.get("playback.rewind_count_seconds")
+    @rewind_count_seconds.setter
+    def rewind_count_seconds(self, value: int): self.set("playback.rewind_count_seconds", value)
+    
+    @property
+    def max_volume_percent(self) -> float: return self.get("playback.max_volume_percent")
+    @max_volume_percent.setter
+    def max_volume_percent(self, value: float): self.set("playback.max_volume_percent", value)
+    
+    # ! Playlist
+    @property
+    def recursive_search(self) -> bool: return self.get("playlist.recursive_search")
+    @recursive_search.setter
+    def recursive_search(self, value: bool): self.set("playlist.recursive_search", value)
+    
+    # ! Keys
+    @property
+    def key_quit(self) -> str: return self.get("keys.quit")
+    @key_quit.setter
+    def key_quit(self, value: str): self.set("keys.quit", value)
+    
+    @property
+    def key_rewind_forward(self) -> str: return self.get("keys.rewind_forward")
+    @key_rewind_forward.setter
+    def key_rewind_forward(self, value: str): self.set("keys.rewind_forward", value)
+    
+    @property
+    def key_rewind_back(self) -> str: return self.get("keys.rewind_back")
+    @key_rewind_back.setter
+    def key_rewind_back(self, value: str): self.set("keys.rewind_back", value)
+    
+    @property
+    def key_volume_up(self) -> str: return self.get("keys.volume_up")
+    @key_volume_up.setter
+    def key_volume_up(self, value: str): self.set("keys.volume_up", value)
+    
+    @property
+    def key_volume_down(self) -> str: return self.get("keys.volume_down")
+    @key_volume_down.setter
+    def key_volume_down(self, value: str): self.set("keys.volume_down", value)
+    
+    # ! Debag
+    @property
+    def log_menu_enable(self) -> bool: return self.get("debag.log_menu_enable")
+    @log_menu_enable.setter
+    def log_menu_enable(self, value: bool): self.set("debag.log_menu_enable", value)
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/css/seaplayer.css` & `seaplayer-0.5.2/seaplayer/css/seaplayer.css`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-/* ! Main Screen */
-#_default  {
-    layout: horizontal;
-}
-
-.screen-box {
-    border: solid cornflowerblue;
-    width: 1fr;
-    height: 100%;
-}
-
-.test-box-border {
-    border: solid cadetblue;
-}
-
-/* ! Play Screen */
-.player-visual-panel {
-    border: solid cadetblue;
-    height: 1fr;
-}
-
-.player-contol-panel {
-    border: solid cadetblue;
-    height: 7;
-}
-
-.box-buttons-sound-control {
-    height: 3;
-}
-
-.button-sound-control {
-    width: 1fr;
-}
-
-.music-selected-label {
-    width: 1fr;
-    height: 1;
-    align: center middle;
-    text-align: center;
-}
+/* ! Main Screen */
+#_default  {
+    layout: horizontal;
+}
+
+.screen-box {
+    border: solid cornflowerblue;
+    width: 1fr;
+    height: 100%;
+}
+
+.test-box-border {
+    border: solid cadetblue;
+}
+
+/* ! Play Screen */
+.player-visual-panel {
+    border: solid cadetblue;
+    height: 1fr;
+}
+
+.player-contol-panel {
+    border: solid cadetblue;
+    height: 7;
+}
+
+.box-buttons-sound-control {
+    height: 3;
+}
+
+.button-sound-control {
+    width: 1fr;
+}
+
+.music-selected-label {
+    width: 1fr;
+    height: 1;
+    align: center middle;
+    text-align: center;
+}
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/functions.py` & `seaplayer-0.5.2/seaplayer/functions.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-import asyncio
-import aiofiles
-from io import BytesIO
-# > Image Works
-from PIL import Image
-# > Typing
-from typing import Literal, Tuple, Optional, Iterable, TypeVar
-# > Local Imports
-from .codeсbase import CodecBase
-
-# ! Types
-T = TypeVar("T")
-
-# ! Async Functions
-async def aiter(it: Iterable[T]):
-    for i in it:
-        await asyncio.sleep(0)
-        yield i
-
-async def get_bar_status() -> Tuple[str, Optional[float], Optional[float]]: return "", None, None
-
-async def aio_is_midi_file(filepath: str):
-    async with aiofiles.open(filepath, 'rb') as file:
-        return await file.read(4) == b"MThd"
-
-# ! Exceptions Rich
-def rich_exception(exc: Exception) -> str:
-    return f"[red]{exc.__class__.__name__}[/red]: {exc.__str__()}"
-
-# ! Functions
-def check_status(sound: CodecBase) -> Literal["Stoped", "Playing", "Paused"]:
-    if sound.playing:
-        if sound.paused: return "Paused"
-        else: return "Playing"
-    return "Stoped"
-
-def get_sound_basename(sound: CodecBase) -> str:
-    if sound.title is not None:
-        if sound.artist is not None:
-            return f"{sound.artist} - {sound.title}"
-        return f"{sound.title}"
-    try: return f"{os.path.basename(sound.name)}"
-    except: return sound.name
-
-def image_from_bytes(data: Optional[bytes]) -> Optional[Image.Image]:
+import os
+import asyncio
+import aiofiles
+from io import BytesIO
+# > Image Works
+from PIL import Image
+# > Typing
+from typing import Literal, Tuple, Optional, Iterable, TypeVar
+# > Local Imports
+from .codeсbase import CodecBase
+
+# ! Types
+T = TypeVar("T")
+
+# ! Async Functions
+async def aiter(it: Iterable[T]):
+    for i in it:
+        await asyncio.sleep(0)
+        yield i
+
+async def get_bar_status() -> Tuple[str, Optional[float], Optional[float]]: return "", None, None
+
+async def aio_is_midi_file(filepath: str):
+    async with aiofiles.open(filepath, 'rb') as file:
+        return await file.read(4) == b"MThd"
+
+# ! Exceptions Rich
+def rich_exception(exc: Exception) -> str:
+    return f"[red]{exc.__class__.__name__}[/red]: {exc.__str__()}"
+
+# ! Functions
+def check_status(sound: CodecBase) -> Literal["Stoped", "Playing", "Paused"]:
+    if sound.playing:
+        if sound.paused: return "Paused"
+        else: return "Playing"
+    return "Stoped"
+
+def get_sound_basename(sound: CodecBase) -> str:
+    if sound.title is not None:
+        if sound.artist is not None:
+            return f"{sound.artist} - {sound.title}"
+        return f"{sound.title}"
+    try: return f"{os.path.basename(sound.name)}"
+    except: return sound.name
+
+def image_from_bytes(data: Optional[bytes]) -> Optional[Image.Image]:
     if data is not None: return Image.open(BytesIO(data))
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/modules/colorizer.py` & `seaplayer-0.5.2/seaplayer/modules/colorizer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Dict
-from typing_inspect import (
-    is_optional_type,
-    is_union_type,
-    is_literal_type,
-    is_tuple_type,
-    get_args,
-    get_origin
-)
-
-# ! Vars
-REPLACE_TYPES = {
-    "str": "[green]str[/]",
-    "bool": "[green]bool[/]",
-    "int": "[green]int[/]",
-    "float": "[green]float[/]",
-    "bytes": "[green]bytes[/]",
-    "bytearray": "[green]bytearray[/]",
-    "complex": "[green]complex[/]",
-    "list": "[green]list[/]",
-    "tuple": "[green]tuple[/]",
-    "dict": "[green]dict[/]",
-    "None": "[cyan]None[/]",
-    "Tuple": "[green]Tuple[/]",
-    "Dict": "[green]Dict[/]",
-    "List": "[green]List[/]",
-    "Any": "[white]Any[/]",
-    "Literal": "[green]Literal[/]",
-    "['": "[[yellow]'",
-    ", '": ", [yellow]'",
-    "']": "'[/]]",
-    "', ": "'[/], "
-}
-
-# ! Other Functions
-def is_list_type(tp) -> bool: return get_origin(tp) == list
-def is_dict_type(tp) -> bool: return get_origin(tp) == dict
-def replaces(string: str, replacement: Dict[str, str]) -> str:
-    for _old, _new in replacement.items(): string = string.replace(_old, _new)
-    return string
-
-# ! Functions
-def pullyper(tp: type) -> str:
-    if tp is None: return "None"
-    elif is_optional_type(tp):
-       return f"{pullyper(get_args(tp)[0])} | None"
-    elif is_union_type(tp):
-        return " | ".join(pullyper(arg) for arg in get_args(tp))
-    elif is_literal_type(tp):
-        return f"Literal[{', '.join(repr(arg) for arg in get_args(tp))}]"
-    elif is_tuple_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"Tuple[{', '.join(pullyper(arg) for arg in args)}]"
-        return "Tuple"
-    elif is_list_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"List[{pullyper(args[0])}]"
-        return "List"
-    elif is_dict_type(tp):
-        if len(args:=get_args(tp)) > 0: return f"Dict[{', '.join(pullyper(arg) for arg in args)}]"
-        return "Dict"
-    return tp.__name__
-
+from typing import Dict
+from typing_inspect import (
+    is_optional_type,
+    is_union_type,
+    is_literal_type,
+    is_tuple_type,
+    get_args,
+    get_origin
+)
+
+# ! Vars
+REPLACE_TYPES = {
+    "str": "[green]str[/]",
+    "bool": "[green]bool[/]",
+    "int": "[green]int[/]",
+    "float": "[green]float[/]",
+    "bytes": "[green]bytes[/]",
+    "bytearray": "[green]bytearray[/]",
+    "complex": "[green]complex[/]",
+    "list": "[green]list[/]",
+    "tuple": "[green]tuple[/]",
+    "dict": "[green]dict[/]",
+    "None": "[cyan]None[/]",
+    "Tuple": "[green]Tuple[/]",
+    "Dict": "[green]Dict[/]",
+    "List": "[green]List[/]",
+    "Any": "[white]Any[/]",
+    "Literal": "[green]Literal[/]",
+    "['": "[[yellow]'",
+    ", '": ", [yellow]'",
+    "']": "'[/]]",
+    "', ": "'[/], "
+}
+
+# ! Other Functions
+def is_list_type(tp) -> bool: return get_origin(tp) == list
+def is_dict_type(tp) -> bool: return get_origin(tp) == dict
+def replaces(string: str, replacement: Dict[str, str]) -> str:
+    for _old, _new in replacement.items(): string = string.replace(_old, _new)
+    return string
+
+# ! Functions
+def pullyper(tp: type) -> str:
+    if tp is None: return "None"
+    elif is_optional_type(tp):
+       return f"{pullyper(get_args(tp)[0])} | None"
+    elif is_union_type(tp):
+        return " | ".join(pullyper(arg) for arg in get_args(tp))
+    elif is_literal_type(tp):
+        return f"Literal[{', '.join(repr(arg) for arg in get_args(tp))}]"
+    elif is_tuple_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"Tuple[{', '.join(pullyper(arg) for arg in args)}]"
+        return "Tuple"
+    elif is_list_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"List[{pullyper(args[0])}]"
+        return "List"
+    elif is_dict_type(tp):
+        if len(args:=get_args(tp)) > 0: return f"Dict[{', '.join(pullyper(arg) for arg in args)}]"
+        return "Dict"
+    return tp.__name__
+
 def richefication(tp: type) -> str: return replaces(pullyper(tp), REPLACE_TYPES)
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/objects/Configurate.py` & `seaplayer-0.5.2/seaplayer/objects/Configurate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from textual.containers import ScrollableContainer, Container
-# > Typing
-from typing import Optional, Union
-
-
-class ConfigurateListItem(Container):
-    def __init__(
-        self,
-        *children,
-        title: str="",
-        desc: str="",
-        width: Union[int, str]="1fr",
-        height: Union[int, str]="1fr",
-        **kwargs
-    ):
-        kwargs["classes"] = "configurate-list-view-item"
-        super().__init__(*children, **kwargs)
-        self.border_title = title
-        self.border_subtitle = desc
-        self.styles.width = width
-        self.styles.height = height
-    
-    async def updating(self, title: Optional[str]="", desc: Optional[str]="") -> None:
-        if title is not None: self.border_title = title
-        if desc is not None: self.border_subtitle = desc
-
-class ConfigurateList(ScrollableContainer):
-    def __init__(self, *children, **kwargs):
-        kwargs["classes"] = "configurate-list-view"
-        super().__init__(*children, **kwargs)
+from textual.containers import ScrollableContainer, Container
+# > Typing
+from typing import Optional, Union
+
+
+class ConfigurateListItem(Container):
+    def __init__(
+        self,
+        *children,
+        title: str="",
+        desc: str="",
+        width: Union[int, str]="1fr",
+        height: Union[int, str]="1fr",
+        **kwargs
+    ):
+        kwargs["classes"] = "configurate-list-view-item"
+        super().__init__(*children, **kwargs)
+        self.border_title = title
+        self.border_subtitle = desc
+        self.styles.width = width
+        self.styles.height = height
+    
+    async def updating(self, title: Optional[str]="", desc: Optional[str]="") -> None:
+        if title is not None: self.border_title = title
+        if desc is not None: self.border_subtitle = desc
+
+class ConfigurateList(ScrollableContainer):
+    def __init__(self, *children, **kwargs):
+        kwargs["classes"] = "configurate-list-view"
+        super().__init__(*children, **kwargs)
         self.border_title = "Configurate"
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/objects/Input.py` & `seaplayer-0.5.2/seaplayer/objects/Input.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from textual.widgets import Input
-# > Typing
-from typing import Optional, Tuple, Any
-
-# ! InputFiles functions
-async def _conv(value: str) -> Tuple[bool, Optional[Any]]: return True, value
-async def _submit(input: Input, value: Any) -> None: ...
-def _update_placeholder() -> Optional[str]: ...
-
-# ! InputField class
-class InputField(Input):
-    def __init__(
-        self,
-        conv=_conv,
-        submit=_submit,
-        update_placeholder=_update_placeholder,
-        **kwargs
-    ) -> None:
-        super().__init__(**kwargs)
-        self._conv = conv
-        self._submit = submit
-        self._update_placeholder = update_placeholder
-        if (placeholder:=self._update_placeholder()) is not None:
-            self.placeholder = placeholder
-    
-    async def action_submit(self):
-        value = self.value
-        self.value = ""
-        if value.replace(" ", "") != "":
-            ok, c_value = await self._conv(value)
-            if ok: await self._submit(self, c_value)
-        if (placeholder:=self._update_placeholder()) is not None:
+from textual.widgets import Input
+# > Typing
+from typing import Optional, Tuple, Any
+
+# ! InputFiles functions
+async def _conv(value: str) -> Tuple[bool, Optional[Any]]: return True, value
+async def _submit(input: Input, value: Any) -> None: ...
+def _update_placeholder() -> Optional[str]: ...
+
+# ! InputField class
+class InputField(Input):
+    def __init__(
+        self,
+        conv=_conv,
+        submit=_submit,
+        update_placeholder=_update_placeholder,
+        **kwargs
+    ) -> None:
+        super().__init__(**kwargs)
+        self._conv = conv
+        self._submit = submit
+        self._update_placeholder = update_placeholder
+        if (placeholder:=self._update_placeholder()) is not None:
+            self.placeholder = placeholder
+    
+    async def action_submit(self):
+        value = self.value
+        self.value = ""
+        if value.replace(" ", "") != "":
+            ok, c_value = await self._conv(value)
+            if ok: await self._submit(self, c_value)
+        if (placeholder:=self._update_placeholder()) is not None:
             self.placeholder = placeholder
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/objects/MusicList.py` & `seaplayer-0.5.2/seaplayer/objects/MusicList.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from textual.widgets import Label, ListItem, ListView
-# > Typing
-from typing import Optional
-# > Local Import's
-from ..types import MusicList
-from ..codeсbase import CodecBase
-from ..functions import get_sound_basename, aiter
-
-
-class MusicListViewItem(ListItem):
-    def __init__(
-        self,
-        title: str="",
-        first_subtitle: str="",
-        second_subtitle: str="",
-        sound_uuid: Optional[str]=None
-    ) -> None:
-        super().__init__(classes="music-list-view-item")
-        self.title_label = Label(title, classes="music-list-view-item-title-label")
-        self.first_subtitle_label = Label(f" {first_subtitle}", classes="music-list-view-item-subtitle-label")
-        self.second_subtitle_label = Label(f" {second_subtitle}", classes="music-list-view-item-subtitle-label")
-        self.sound_uuid = sound_uuid
-        
-        self.compose_add_child(self.title_label)
-        self.compose_add_child(self.first_subtitle_label)
-        self.compose_add_child(self.second_subtitle_label)
-    
-    async def update_labels(
-        self,
-        title: Optional[str]=None,
-        first_subtitle: Optional[str]=None,
-        second_subtitle: Optional[str]=None,
-    ) -> None:
-        if title is not None: self.title_label.update(title)
-        if first_subtitle is not None: self.first_subtitle_label.update(title)
-        if second_subtitle is not None: self.second_subtitle_label.update(title)
-
-class MusicListView(ListView):
-    def __init__(self, **kwargs) -> None:
-        kwargs["classes"] = "music-list-view"
-        super().__init__(**kwargs)
-        self.music_list: MusicList = MusicList()
-    
-    def add_sound(self, sound: CodecBase) -> str:
-        sound_uuid = self.music_list.add(sound)
-        self.append(
-            MusicListViewItem(
-                f"{get_sound_basename(sound)}",
-                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
-                    duration=round(sound.duration),
-                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
-                    samplerate=round(sound.samplerate),
-                    bitrate=round(sound.bitrate / 1000)
-                ),
-                sound.name,
-                sound_uuid
-            )
-        )
-        return sound_uuid
-    
-    def get_sound(self, sound_uuid: str) -> Optional[CodecBase]: return self.music_list.get(sound_uuid)
-    
-    async def aio_add_sound(self, sound: CodecBase):
-        sound_uuid = await self.music_list.aio_add(sound)
-        await self.append(
-            MusicListViewItem(
-                f"{get_sound_basename(sound)}",
-                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps, {codec_name}".format(
-                    duration=round(sound.duration),
-                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
-                    samplerate=round(sound.samplerate),
-                    bitrate=round(sound.bitrate / 1000),
-                    codec_name=sound.codec_name
-                ),
-                sound.name,
-                sound_uuid
-            )
-        )
-        return sound_uuid
-    
-    def get_items_count(self) -> int: return len(self.children)
-    def exists_item_index(self, index: int) -> bool: return 0 >= index < self.get_items_count()
-    def get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
-        item: MusicListViewItem
-        for idx, item in enumerate(self.children):
-            if item.sound_uuid == sound_uuid:
-                return idx
-    
-    def get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
-        try: return self.children[index]
-        except:
-            try: return self.children[0]
-            except: pass
-    
-    def get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
-        if (index:=self.get_item_index_from_sound_uuid(sound_uuid)) is not None:
-            if (mli:=self.get_item_from_index(index+1)) is not None:
-                return mli.sound_uuid
-    
-    def select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
-        try:
-            super()._on_list_item__child_clicked(
-                ListItem._ChildClicked(
-                    self.children[self.get_item_index_from_sound_uuid(sound_uuid)]
-                )
-            )
-        except: pass
-    
-    async def aio_get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
-        try: return self.children[index]
-        except:
-            try: return self.children[0]
-            except: pass
-    
-    async def aio_get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
-        item: MusicListViewItem
-        async for idx, item in aiter(enumerate(self.children)):
-            if item.sound_uuid == sound_uuid:
-                return idx
-    
-    async def aio_get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
-        if (index:=await self.aio_get_item_index_from_sound_uuid(sound_uuid)) is not None:
-            if (mli:=await self.aio_get_item_from_index(index+1)) is not None:
-                return mli.sound_uuid
-    
-    async def aio_select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
-        try:
-            super()._on_list_item__child_clicked(
-                ListItem._ChildClicked(
-                    self.children[await self.aio_get_item_index_from_sound_uuid(sound_uuid)]
-                )
-            )
+from textual.widgets import Label, ListItem, ListView
+# > Typing
+from typing import Optional
+# > Local Import's
+from ..types import MusicList
+from ..codeсbase import CodecBase
+from ..functions import get_sound_basename, aiter
+
+
+class MusicListViewItem(ListItem):
+    def __init__(
+        self,
+        title: str="",
+        first_subtitle: str="",
+        second_subtitle: str="",
+        sound_uuid: Optional[str]=None
+    ) -> None:
+        super().__init__(classes="music-list-view-item")
+        self.title_label = Label(title, classes="music-list-view-item-title-label")
+        self.first_subtitle_label = Label(f" {first_subtitle}", classes="music-list-view-item-subtitle-label")
+        self.second_subtitle_label = Label(f" {second_subtitle}", classes="music-list-view-item-subtitle-label")
+        self.sound_uuid = sound_uuid
+        
+        self.compose_add_child(self.title_label)
+        self.compose_add_child(self.first_subtitle_label)
+        self.compose_add_child(self.second_subtitle_label)
+    
+    async def update_labels(
+        self,
+        title: Optional[str]=None,
+        first_subtitle: Optional[str]=None,
+        second_subtitle: Optional[str]=None,
+    ) -> None:
+        if title is not None: self.title_label.update(title)
+        if first_subtitle is not None: self.first_subtitle_label.update(title)
+        if second_subtitle is not None: self.second_subtitle_label.update(title)
+
+class MusicListView(ListView):
+    def __init__(self, **kwargs) -> None:
+        kwargs["classes"] = "music-list-view"
+        super().__init__(**kwargs)
+        self.music_list: MusicList = MusicList()
+    
+    def add_sound(self, sound: CodecBase) -> str:
+        sound_uuid = self.music_list.add(sound)
+        self.append(
+            MusicListViewItem(
+                f"{get_sound_basename(sound)}",
+                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps".format(
+                    duration=round(sound.duration),
+                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
+                    samplerate=round(sound.samplerate),
+                    bitrate=round(sound.bitrate / 1000)
+                ),
+                sound.name,
+                sound_uuid
+            )
+        )
+        return sound_uuid
+    
+    def get_sound(self, sound_uuid: str) -> Optional[CodecBase]: return self.music_list.get(sound_uuid)
+    
+    async def aio_add_sound(self, sound: CodecBase):
+        sound_uuid = await self.music_list.aio_add(sound)
+        await self.append(
+            MusicListViewItem(
+                f"{get_sound_basename(sound)}",
+                "{duration} sec, {channel_mode}, {samplerate} Hz, {bitrate} kbps, {codec_name}".format(
+                    duration=round(sound.duration),
+                    channel_mode="Mono" if sound.channels <= 1 else "Stereo",
+                    samplerate=round(sound.samplerate),
+                    bitrate=round(sound.bitrate / 1000),
+                    codec_name=sound.codec_name
+                ),
+                sound.name,
+                sound_uuid
+            )
+        )
+        return sound_uuid
+    
+    def get_items_count(self) -> int: return len(self.children)
+    def exists_item_index(self, index: int) -> bool: return 0 >= index < self.get_items_count()
+    def get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
+        item: MusicListViewItem
+        for idx, item in enumerate(self.children):
+            if item.sound_uuid == sound_uuid:
+                return idx
+    
+    def get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
+        try: return self.children[index]
+        except:
+            try: return self.children[0]
+            except: pass
+    
+    def get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
+        if (index:=self.get_item_index_from_sound_uuid(sound_uuid)) is not None:
+            if (mli:=self.get_item_from_index(index+1)) is not None:
+                return mli.sound_uuid
+    
+    def select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
+        try:
+            super()._on_list_item__child_clicked(
+                ListItem._ChildClicked(
+                    self.children[self.get_item_index_from_sound_uuid(sound_uuid)]
+                )
+            )
+        except: pass
+    
+    async def aio_get_item_from_index(self, index: int) -> Optional[MusicListViewItem]:
+        try: return self.children[index]
+        except:
+            try: return self.children[0]
+            except: pass
+    
+    async def aio_get_item_index_from_sound_uuid(self, sound_uuid: str) -> Optional[int]:
+        item: MusicListViewItem
+        async for idx, item in aiter(enumerate(self.children)):
+            if item.sound_uuid == sound_uuid:
+                return idx
+    
+    async def aio_get_next_sound_uuid(self, sound_uuid: str) -> Optional[str]:
+        if (index:=await self.aio_get_item_index_from_sound_uuid(sound_uuid)) is not None:
+            if (mli:=await self.aio_get_item_from_index(index+1)) is not None:
+                return mli.sound_uuid
+    
+    async def aio_select_list_item_from_sound_uuid(self, sound_uuid: str) -> None:
+        try:
+            super()._on_list_item__child_clicked(
+                ListItem._ChildClicked(
+                    self.children[await self.aio_get_item_index_from_sound_uuid(sound_uuid)]
+                )
+            )
         except: pass
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.2/seaplayer/plug/pluginbase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from pydantic import BaseModel
-# > Local Import's
-from typing import Optional
-
-# ! Plugin Info Class
-class PluginInfo(BaseModel):
-    name: str
-    name_id: str
-    version: str
-    author: str
-    description: Optional[str]=None
-    url: Optional[str]=None
-
-# ! Plugin Base Class
-class PluginBase:
-    def __init__(self, app, pl, info) -> None:
-        self.app = app
-        self.pl = pl
-        self.info = info
-    
-
-    def on_init(self): pass
-    def on_run(self): pass
-    async def on_compose(self): pass
-    async def on_quit(self): pass
+from pydantic import BaseModel
+# > Local Import's
+from typing import Optional
+
+# ! Plugin Info Class
+class PluginInfo(BaseModel):
+    name: str
+    name_id: str
+    version: str
+    author: str
+    description: Optional[str]=None
+    url: Optional[str]=None
+
+# ! Plugin Base Class
+class PluginBase:
+    def __init_repr__(self) -> str:
+        return f"[green]{self.info.name}[/] ({repr(self.info.name_id)}) [cyan]v{self.info.version}[/cyan] [yellow]is initialized[/yellow]!"
+    
+    def __init__(self, app, pl, info: PluginInfo) -> None:
+        self.app = app
+        self.pl = pl
+        self.info = info
+        
+        self.app.info(self.__init_repr__())
+
+    def on_init(self): pass
+    def on_run(self): pass
+    async def on_compose(self): pass
+    async def on_quit(self): pass
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.2/seaplayer/plug/pluginloader.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,86 @@
-from pathlib import Path
-from pydantic import BaseModel
-# > Typing
-from types import ModuleType
-from typing import (
-    Any,
-    Dict,
-    List,
-    Type,
-    Tuple,
-    Union,
-    Optional,
-    Generator, 
-    AsyncGenerator
-)
-# > Local Import's
-from .pluginbase import PluginBase, PluginInfo
-from ..seaplayer import SeaPlayer
-
-# ! Types
-class PluginModuleType(ModuleType):
-    plugin_main: Type[PluginBase]
-
-# ! Functions
-def get_module_info(path: str) -> Tuple[str, str]: ...
-def load_module(path: str) -> PluginModuleType: ...
-def plugin_from_module(app: SeaPlayer, pl: PluginLoader, info: PluginInfo, module: PluginModuleType) -> PluginBase: ...
-
-# ! Plugin Loader Config
-class PluginLoaderConfigModel(BaseModel):
-    plugins_enable: Dict[str, bool] = {}
-
-class PluginLoaderConfigManager:
-    filepath: Path
-    config: PluginLoaderConfigModel
-    
-    @staticmethod
-    def dump(path: str, data: PluginLoaderConfigModel) -> None: ...
-    @staticmethod
-    def load(path: str, default_data: Dict[str, Any]) -> PluginLoaderConfigModel: ...
-    def refresh(self) -> None: ...
-
-    def __init__(self, path: str) -> None: ...
-
-    def exists_plugin(self, info: PluginInfo) -> bool: ...
-    def add_plugin(self, info: PluginInfo) -> None: ...
-    def is_enable_plugin(self, info: PluginInfo) -> bool: ...
-
-# ! Plugin Loader Class
-class PluginLoader:
-    app: SeaPlayer
-    plugins_dirpath: Path
-    plugins_config_path: Path
-    on_plugins: List[PluginBase]
-    off_plugins: List[PluginInfo]
-    error_plugins: List[Tuple[str, str]]
-
-    def __init__(
-        self,
-        app: SeaPlayer,
-        plugins_dirpath: Optional[Union[str, Path]]=None,
-        plugins_config_path: Optional[Union[str, Path]]=None,
-        *args,
-        **kwargs
-    ) -> None:
-        ...
-    
-    async def aio_search_plugins_paths(self) -> AsyncGenerator[Tuple[str, str]]: ...
-    def search_plugins_paths(self) -> Generator[Tuple[str, str], Any, None]: ...
-
-    def on_init(self) -> None: ...
-    def on_run(self) -> None: ...
-    async def on_compose(self) -> None: ...
-    async def on_quit(self) -> None: ...
-    
+from pathlib import Path
+from pydantic import BaseModel
+# > Typing
+from types import ModuleType
+from typing import (
+    Any,
+    Dict,
+    List,
+    Type,
+    Tuple,
+    Union,
+    Optional,
+    Generator, 
+    AsyncGenerator
+)
+# > Local Import's
+from .pluginbase import PluginBase, PluginInfo
+from ..seaplayer import SeaPlayer
+
+# ! Types
+class PluginModuleType(ModuleType):
+    plugin_main: Type[PluginBase]
+
+INFO_FILE_PATH = str
+INIT_FILE_PATH = str
+
+# ! Functions
+def get_module_info(path: str) -> Tuple[str, str]: ...
+def load_module(path: str) -> PluginModuleType: ...
+def plugin_from_module(app: SeaPlayer, pl: PluginLoader, info: PluginInfo, module: PluginModuleType) -> PluginBase: ...
+
+# ! Plugin Loader Config
+class PluginLoaderConfigModel(BaseModel):
+    plugins_enable: Dict[str, bool] = {}
+
+class PluginLoaderConfigManager:
+    filepath: Path
+    config: PluginLoaderConfigModel
+    
+    @staticmethod
+    def dump(path: str, data: PluginLoaderConfigModel) -> None: ...
+    @staticmethod
+    def load(path: str, default_data: Dict[str, Any]) -> PluginLoaderConfigModel: ...
+    def refresh(self) -> None: ...
+
+    def __init__(self, path: str) -> None: ...
+
+    def exists_plugin(self, info: PluginInfo) -> bool: ...
+    def exists_plugin_by_name_id(self, name_id: str) -> bool: ...
+    def add_plugin(self, info: PluginInfo) -> None: ...
+    def is_enable_plugin(self, info: PluginInfo) -> bool: ...
+    def disable_plugin(self, info: PluginInfo) -> None: ...
+    def disable_plugin_by_name_id(self, name_id: str) -> None: ...
+    def enable_plugin(self, info: PluginInfo) -> None: ...
+    def enable_plugin_by_name_id(self, name_id: str) -> None: ...
+
+# ! Plugin Loader Class
+class PluginLoader:
+    app: SeaPlayer
+    plugins_dirpath: Path
+    plugins_config_path: Path
+    on_plugins: List[PluginBase]
+    off_plugins: List[PluginInfo]
+    error_plugins: List[Tuple[str, str]]
+
+    def __init__(
+        self,
+        app: SeaPlayer,
+        plugins_dirpath: Optional[Union[str, Path]]=None,
+        plugins_config_path: Optional[Union[str, Path]]=None,
+        *args,
+        **kwargs
+    ) -> None:
+        ...
+    
+    @staticmethod
+    async def aio_search_plugins_paths() -> AsyncGenerator[Tuple[INFO_FILE_PATH, INIT_FILE_PATH]]: ...
+    @staticmethod
+    def search_plugins_paths() -> Generator[Tuple[INFO_FILE_PATH, INIT_FILE_PATH], Any, None]: ...
+    @staticmethod
+    def load_plugin_info(path: str) -> PluginInfo: ...
+    
+    def on_init(self) -> None: ...
+    def on_run(self) -> None: ...
+    async def on_compose(self) -> None: ...
+    async def on_quit(self) -> None: ...
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/screens/Unknown.py` & `seaplayer-0.5.2/seaplayer/screens/Unknown.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import base64
-import platform
-# > Graphics
-from textual.app import ComposeResult
-from textual.screen import Screen
-from textual.widgets import Static
-
-# ! Constants
-TEXT = b'CkFuIGVycm9yIGhhcyBvY2N1cnJlZC4gVG8gY29udGludWU6CgpQcmVzcyBFbnRlciB0byByZXR1cm4gdG8ge3N5c3RlbX0sIG9yCgpQcmVzcyBDVFJMK0FMVCtERUwgdG8gcmVzdGFydCB5b3VyIGNvbXB1dGVyLiBJZiB5b3UgZG8gdGhpcywKeW91IHdpbGwgbG9zZSBhbnkgdW5zYXZlZCBpbmZvcm1hdGlvbiBpbiBhbGwgb3BlbiBhcHBsaWNhdGlvbnMuCgpFcnJvcjogMEUgOiAwMTZGIDogQkZGOUIzRDQK'
-TEXT = base64.b64decode(TEXT).decode(errors="ignore").format(system=platform.system())
-UNKNOWN_OPEN_KEY = base64.b64decode(b"Yg==").decode(errors="ignore")
-
-# ! Main Class
-class Unknown(Screen):
-    """This Unknown screen."""
-    BINDINGS = [("escape", "app.pop_screen", "Back")]
-
-    def compose(self) -> ComposeResult:
-        yield Static(f" {platform.system()} ", id="unknown-title")
-        yield Static(TEXT)
+import base64
+import platform
+# > Graphics
+from textual.app import ComposeResult
+from textual.screen import Screen
+from textual.widgets import Static
+
+# ! Constants
+TEXT = b'CkFuIGVycm9yIGhhcyBvY2N1cnJlZC4gVG8gY29udGludWU6CgpQcmVzcyBFbnRlciB0byByZXR1cm4gdG8ge3N5c3RlbX0sIG9yCgpQcmVzcyBDVFJMK0FMVCtERUwgdG8gcmVzdGFydCB5b3VyIGNvbXB1dGVyLiBJZiB5b3UgZG8gdGhpcywKeW91IHdpbGwgbG9zZSBhbnkgdW5zYXZlZCBpbmZvcm1hdGlvbiBpbiBhbGwgb3BlbiBhcHBsaWNhdGlvbnMuCgpFcnJvcjogMEUgOiAwMTZGIDogQkZGOUIzRDQK'
+TEXT = base64.b64decode(TEXT).decode(errors="ignore").format(system=platform.system())
+UNKNOWN_OPEN_KEY = base64.b64decode(b"Yg==").decode(errors="ignore")
+
+# ! Main Class
+class Unknown(Screen):
+    """This Unknown screen."""
+    BINDINGS = [("escape", "app.pop_screen", "Back")]
+
+    def compose(self) -> ComposeResult:
+        yield Static(f" {platform.system()} ", id="unknown-title")
+        yield Static(TEXT)
         yield Static("Press any key to continue [blink]_[/]", id="unknown-any-key")
```

### Comparing `seaplayer-0.5.1.dev2/seaplayer/types/MusicList.py` & `seaplayer-0.5.2/seaplayer/types/MusicList.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-
-
-# > Typing
-from typing import Optional, Dict
-# > Local Import's
-from ..codeсbase import CodecBase
-
-
-class MusicList:
-    @staticmethod
-    def get_file_sha1(sound: CodecBase, buffer_size: int=65536) -> str: return sound.__sha1__(buffer_size)
-    
-    @staticmethod
-    async def aio_get_file_sha1(sound: CodecBase, buffer_size: int=65536) -> str: return await sound.__aio_sha1__(buffer_size)
-    
-    def __init__(self, **child_sounds: CodecBase) -> None:
-        self.sounds: Dict[str, CodecBase] = {}
-        for key in child_sounds:
-            if isinstance(child_sounds[key], CodecBase):
-                self.sounds[key] = child_sounds[key]
-    
-    def exists(self, sound_uuid: str) -> bool: return sound_uuid in self.sounds.keys()
-    def get(self, sound_uuid: str) -> Optional[CodecBase]: return self.sounds.get(sound_uuid)
-    def add(self, sound: CodecBase) -> str:
-        self.sounds[(sound_uuid:=self.get_file_sha1(sound))] = sound
-        return sound_uuid
-    def exists_sha1(self, sound: CodecBase) -> bool:
-        return self.get_file_sha1(sound) in self.sounds.keys()
-    
-    async def aio_exists(self, sound_uuid: str): return sound_uuid in self.sounds.keys()
-    async def aio_get(self, sound_uuid: str): return self.sounds.get(sound_uuid)
-    async def aio_add(self, sound: CodecBase):
-        self.sounds[(sound_uuid:=await self.aio_get_file_sha1(sound))] = sound
-        return sound_uuid
-    async def aio_exists_sha1(self, sound: CodecBase) -> bool:
-        return await self.aio_get_file_sha1(sound) in self.sounds.keys()
+
+
+# > Typing
+from typing import Optional, Dict
+# > Local Import's
+from ..codeсbase import CodecBase
+
+
+class MusicList:
+    @staticmethod
+    def get_file_sha1(sound: CodecBase, buffer_size: int=65536) -> str: return sound.__sha1__(buffer_size)
+    
+    @staticmethod
+    async def aio_get_file_sha1(sound: CodecBase, buffer_size: int=65536) -> str: return await sound.__aio_sha1__(buffer_size)
+    
+    def __init__(self, **child_sounds: CodecBase) -> None:
+        self.sounds: Dict[str, CodecBase] = {}
+        for key in child_sounds:
+            if isinstance(child_sounds[key], CodecBase):
+                self.sounds[key] = child_sounds[key]
+    
+    def exists(self, sound_uuid: str) -> bool: return sound_uuid in self.sounds.keys()
+    def get(self, sound_uuid: str) -> Optional[CodecBase]: return self.sounds.get(sound_uuid)
+    def add(self, sound: CodecBase) -> str:
+        self.sounds[(sound_uuid:=self.get_file_sha1(sound))] = sound
+        return sound_uuid
+    def exists_sha1(self, sound: CodecBase) -> bool:
+        return self.get_file_sha1(sound) in self.sounds.keys()
+    
+    async def aio_exists(self, sound_uuid: str): return sound_uuid in self.sounds.keys()
+    async def aio_get(self, sound_uuid: str): return self.sounds.get(sound_uuid)
+    async def aio_add(self, sound: CodecBase):
+        self.sounds[(sound_uuid:=await self.aio_get_file_sha1(sound))] = sound
+        return sound_uuid
+    async def aio_exists_sha1(self, sound: CodecBase) -> bool:
+        return await self.aio_get_file_sha1(sound) in self.sounds.keys()
```

### Comparing `seaplayer-0.5.1.dev2/PKG-INFO` & `seaplayer-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.1.dev2
+Version: 0.5.2
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: build
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: mutagen (==1.45.1)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: platformdirs (>=3.5.1,<4.0.0)
 Requires-Dist: playsoundsimple-py (==0.7.0)
+Requires-Dist: poetry (>=1.5.0,<2.0.0) ; extra == "build"
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyinstaller (>=5.11.0,<6.0.0) ; extra == "build"
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
 Requires-Dist: textual (>=0.25.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
```


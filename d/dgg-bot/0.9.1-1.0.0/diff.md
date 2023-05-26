# Comparing `tmp/dgg-bot-0.9.1.tar.gz` & `tmp/dgg-bot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgg-bot-0.9.1.tar", last modified: Wed Feb 15 11:08:53 2023, max compression
+gzip compressed data, was "dgg-bot-1.0.0.tar", last modified: Fri May 26 14:20:52 2023, max compression
```

## Comparing `dgg-bot-0.9.1.tar` & `dgg-bot-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.812425 dgg-bot-0.9.1/
--rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     3565 2023-02-15 11:08:53.812425 dgg-bot-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     2811 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.789426 dgg-bot-0.9.1/dgg_bot.egg-info/
--rw-rw-rw-   0        0        0     3565 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-15 11:08:53.000000 dgg-bot-0.9.1/dgg_bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.807428 dgg-bot-0.9.1/dggbot/
--rw-rw-rw-   0        0        0      206 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/__init__.py
--rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-0.9.1/dggbot/_logging.py
--rw-rw-rw-   0        0        0     3208 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/dggbot/bot.py
--rw-rw-rw-   0        0        0    13851 2023-02-14 14:09:09.000000 dgg-bot-0.9.1/dggbot/chat.py
--rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-0.9.1/dggbot/errors.py
--rw-rw-rw-   0        0        0      607 2023-02-08 17:15:19.000000 dgg-bot-0.9.1/dggbot/event.py
--rw-rw-rw-   0        0        0      339 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/funcs.py
-drwxrwxrwx   0        0        0        0 2023-02-15 11:08:53.811425 dgg-bot-0.9.1/dggbot/live/
--rw-rw-rw-   0        0        0     3551 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/live/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-01-11 16:43:22.000000 dgg-bot-0.9.1/dggbot/live/message.py
--rw-rw-rw-   0        0        0     1569 2023-02-10 14:03:33.000000 dgg-bot-0.9.1/dggbot/message.py
--rw-rw-rw-   0        0        0      197 2023-01-11 16:43:21.000000 dgg-bot-0.9.1/dggbot/user.py
--rw-rw-rw-   0        0        0     1017 2023-02-15 10:52:35.000000 dgg-bot-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       26 2023-02-10 14:04:45.000000 dgg-bot-0.9.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 11:08:53.813425 dgg-bot-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-02-15 10:38:12.000000 dgg-bot-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.726970 dgg-bot-1.0.0/
+-rw-rw-rw-   0        0        0     1081 2022-09-09 16:56:19.000000 dgg-bot-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3886 2023-05-26 14:20:52.725970 dgg-bot-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2023-05-26 14:19:48.000000 dgg-bot-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.690970 dgg-bot-1.0.0/dgg_bot.egg-info/
+-rw-rw-rw-   0        0        0     3886 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 14:20:52.000000 dgg-bot-1.0.0/dgg_bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.716971 dgg-bot-1.0.0/dggbot/
+-rw-rw-rw-   0        0        0      329 2023-05-26 14:15:08.000000 dgg-bot-1.0.0/dggbot/__init__.py
+-rw-rw-rw-   0        0        0      504 2022-09-11 20:38:19.000000 dgg-bot-1.0.0/dggbot/_logging.py
+-rw-rw-rw-   0        0        0     4141 2023-04-03 11:05:30.000000 dgg-bot-1.0.0/dggbot/bot.py
+-rw-rw-rw-   0        0        0     7756 2023-05-26 13:57:58.000000 dgg-bot-1.0.0/dggbot/chat.py
+-rw-rw-rw-   0        0        0      497 2023-01-15 02:17:22.000000 dgg-bot-1.0.0/dggbot/errors.py
+-rw-rw-rw-   0        0        0      622 2023-05-26 13:06:27.000000 dgg-bot-1.0.0/dggbot/event.py
+-rw-rw-rw-   0        0        0      863 2023-05-26 13:12:01.000000 dgg-bot-1.0.0/dggbot/flairs.py
+-rw-rw-rw-   0        0        0      339 2023-03-13 02:12:12.000000 dgg-bot-1.0.0/dggbot/funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.721970 dgg-bot-1.0.0/dggbot/live/
+-rw-rw-rw-   0        0        0     1770 2023-04-28 01:20:01.000000 dgg-bot-1.0.0/dggbot/live/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-05-22 18:25:49.000000 dgg-bot-1.0.0/dggbot/live/message.py
+-rw-rw-rw-   0        0        0     3892 2023-05-26 14:03:51.000000 dgg-bot-1.0.0/dggbot/message.py
+-rw-rw-rw-   0        0        0      151 2023-05-26 11:13:39.000000 dgg-bot-1.0.0/dggbot/user.py
+-rw-rw-rw-   0        0        0     2578 2023-05-26 10:38:55.000000 dgg-bot-1.0.0/dggbot/wsbase.py
+-rw-rw-rw-   0        0        0     1221 2023-05-26 14:19:48.000000 dgg-bot-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       41 2023-05-26 14:11:03.000000 dgg-bot-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:20:52.726970 dgg-bot-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 14:20:52.724969 dgg-bot-1.0.0/tests/
+-rw-rw-rw-   0        0        0      357 2023-05-26 13:31:13.000000 dgg-bot-1.0.0/tests/testtest.py
```

### Comparing `dgg-bot-0.9.1/LICENSE` & `dgg-bot-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgg-bot-0.9.1/PKG-INFO` & `dgg-bot-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 0.9.1
-Summary: A library for making a bot in Destiny.gg chat.
-Home-page: https://github.com/Fritz-02/dgg-bot/
+Version: 1.0.0
+Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 DGG-bot
 =======
 
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
 
-A library for making a bot in Destiny.gg chat.
+A library for connecting to and making a bot in Destiny.gg chat.
 
 Installing
 ----------
 
 **Python 3.9 or higher is required** (version 0.5.0 and above, Python 3.8+ for versions below)
 
 .. code:: sh
@@ -109,23 +109,30 @@
 
 
 Connecting to alternative DGG environments.
 
 .. code-block:: python
 
     from dggbot import DGGBot
-    import time
 
     bot = DGGBot(
         owner="Owner",
         prefix="$",
-        wss="wss://chat.omniliberal.dev/ws",
         sid="SID",
         rememberme="REMEMBERME",
+        config={
+            {
+                "wss": "wss://chat.omniliberal.dev/ws",
+                "wss-origin": "https://www.omniliberal.dev",
+                "baseurl": "https://www.omniliberal.dev",
+                "endpoints": {"user": "/api/chat/me", "userinfo": "/api/userinfo"},
+                "flairs": "https://cdn.omniliberal.dev/flairs/flairs.json",
+            }
+        },
     )
 
     @bot.event()
     def on_msg(msg):
         print(msg)
 
     if __name__ == "__main__":
-         bot.run_forever(origin="https://www.omniliberal.dev")
+        bot.run_forever()
```

### Comparing `dgg-bot-0.9.1/README.rst` & `dgg-bot-1.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
 
-A library for making a bot in Destiny.gg chat.
+A library for connecting to and making a bot in Destiny.gg chat.
 
 Installing
 ----------
 
 **Python 3.9 or higher is required** (version 0.5.0 and above, Python 3.8+ for versions below)
 
 .. code:: sh
@@ -89,23 +89,30 @@
 
 
 Connecting to alternative DGG environments.
 
 .. code-block:: python
 
     from dggbot import DGGBot
-    import time
 
     bot = DGGBot(
         owner="Owner",
         prefix="$",
-        wss="wss://chat.omniliberal.dev/ws",
         sid="SID",
         rememberme="REMEMBERME",
+        config={
+            {
+                "wss": "wss://chat.omniliberal.dev/ws",
+                "wss-origin": "https://www.omniliberal.dev",
+                "baseurl": "https://www.omniliberal.dev",
+                "endpoints": {"user": "/api/chat/me", "userinfo": "/api/userinfo"},
+                "flairs": "https://cdn.omniliberal.dev/flairs/flairs.json",
+            }
+        },
     )
 
     @bot.event()
     def on_msg(msg):
         print(msg)
 
     if __name__ == "__main__":
-         bot.run_forever(origin="https://www.omniliberal.dev")
+        bot.run_forever()
```

### Comparing `dgg-bot-0.9.1/dgg_bot.egg-info/PKG-INFO` & `dgg-bot-1.0.0/dgg_bot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: dgg-bot
-Version: 0.9.1
-Summary: A library for making a bot in Destiny.gg chat.
-Home-page: https://github.com/Fritz-02/dgg-bot/
+Version: 1.0.0
+Summary: A library for connecting to and making a bot in Destiny.gg chat.
 Author: Fritz-02
 License: MIT
 Project-URL: Homepage, https://github.com/Fritz-02/dgg-bot/
 Project-URL: Bug Tracker, https://github.com/Fritz-02/dgg-bot/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: LICENSE
 
 DGG-bot
 =======
 
 .. image:: https://img.shields.io/pypi/v/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI version info
 .. image:: https://img.shields.io/pypi/pyversions/dgg-bot.svg
    :target: https://pypi.python.org/pypi/dgg-bot
    :alt: PyPI supported Python versions
 
-A library for making a bot in Destiny.gg chat.
+A library for connecting to and making a bot in Destiny.gg chat.
 
 Installing
 ----------
 
 **Python 3.9 or higher is required** (version 0.5.0 and above, Python 3.8+ for versions below)
 
 .. code:: sh
@@ -109,23 +109,30 @@
 
 
 Connecting to alternative DGG environments.
 
 .. code-block:: python
 
     from dggbot import DGGBot
-    import time
 
     bot = DGGBot(
         owner="Owner",
         prefix="$",
-        wss="wss://chat.omniliberal.dev/ws",
         sid="SID",
         rememberme="REMEMBERME",
+        config={
+            {
+                "wss": "wss://chat.omniliberal.dev/ws",
+                "wss-origin": "https://www.omniliberal.dev",
+                "baseurl": "https://www.omniliberal.dev",
+                "endpoints": {"user": "/api/chat/me", "userinfo": "/api/userinfo"},
+                "flairs": "https://cdn.omniliberal.dev/flairs/flairs.json",
+            }
+        },
     )
 
     @bot.event()
     def on_msg(msg):
         print(msg)
 
     if __name__ == "__main__":
-         bot.run_forever(origin="https://www.omniliberal.dev")
+        bot.run_forever()
```

### Comparing `dgg-bot-0.9.1/dggbot/event.py` & `dgg-bot-1.0.0/dggbot/event.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class EventType:
     BAN = "BAN"
     BROADCAST = "BROADCAST"
     ERROR = "ERR"
     JOIN = "JOIN"
+    ME = "ME"
     MESSAGE = "MSG"
     MUTE = "MUTE"
     NAMES = "NAMES"
     PIN = "PIN"
     POLLSTART = "POLLSTART"
     POLLSTOP = "POLLSTOP"
     PRIVMSG = "PRIVMSG"
```

### Comparing `dgg-bot-0.9.1/pyproject.toml` & `dgg-bot-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dgg-bot"
-version = "0.9.1"
 authors = [
     { name="Fritz-02"},
 ]
-description="A library for making a bot in Destiny.gg chat."
+description="A library for connecting to and making a bot in Destiny.gg chat."
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Communications :: Chat"
 ]
-dynamic = ["dependencies"]
+dynamic = ["dependencies", "version"]
 
 [project.urls]
 "Homepage" = "https://github.com/Fritz-02/dgg-bot/"
 "Bug Tracker" = "https://github.com/Fritz-02/dgg-bot/issues"
 
+[project.optional-dependencies]
+dev = ["black", "flake8"]
+
 [tool.black]
 line-length = 88
 target-version = ['py39']
 
 [tool.isort]
 profile = "black"
 py_version = 38
 line_length = 88
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
+version = {attr = "dggbot.VERSION"}
+
+[tool.setuptools.packages.find]
+include = ["dggbot*"]
+exclude = ["configs*"]
```


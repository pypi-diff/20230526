# Comparing `tmp/langchain_discord-0.0.3.tar.gz` & `tmp/langchain_discord-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_discord-0.0.3.tar", last modified: Fri May 26 14:54:30 2023, max compression
+gzip compressed data, was "langchain_discord-0.0.4.tar", last modified: Fri May 26 14:56:51 2023, max compression
```

## Comparing `langchain_discord-0.0.3.tar` & `langchain_discord-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:54:30.794806 langchain_discord-0.0.3/
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:54:30.793509 langchain_discord-0.0.3/.vscode/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.3/.vscode/settings.json
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.3/LICENSE.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 14:54:30.794990 langchain_discord-0.0.3/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.3/README.md
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:54:30.793816 langchain_discord-0.0.3/langchain_discord/
--rw-r--r--   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:50:09.000000 langchain_discord-0.0.3/langchain_discord/__init__.py
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1689 2023-05-26 14:42:53.000000 langchain_discord-0.0.3/langchain_discord/webhook.py
-drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:54:30.794641 langchain_discord-0.0.3/langchain_discord.egg-info/
--rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 14:54:30.000000 langchain_discord-0.0.3/langchain_discord.egg-info/PKG-INFO
--rw-r--r--   0 lennarddorst   (501) staff       (20)      340 2023-05-26 14:54:30.000000 langchain_discord-0.0.3/langchain_discord.egg-info/SOURCES.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-26 14:54:30.000000 langchain_discord-0.0.3/langchain_discord.egg-info/dependency_links.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-26 14:54:30.000000 langchain_discord-0.0.3/langchain_discord.egg-info/requires.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-26 14:54:30.000000 langchain_discord-0.0.3/langchain_discord.egg-info/top_level.txt
--rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-26 14:54:00.000000 langchain_discord-0.0.3/pyproject.toml
--rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-26 14:54:30.795385 langchain_discord-0.0.3/setup.cfg
--rw-r--r--   0 lennarddorst   (501) staff       (20)     1719 2023-05-26 14:53:53.000000 langchain_discord-0.0.3/setup.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:56:51.816778 langchain_discord-0.0.4/
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:56:51.815670 langchain_discord-0.0.4/.vscode/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      237 2023-05-24 19:54:14.000000 langchain_discord-0.0.4/.vscode/settings.json
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1065 2023-05-25 16:34:10.000000 langchain_discord-0.0.4/LICENSE.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 14:56:51.816958 langchain_discord-0.0.4/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       65 2023-05-25 11:43:21.000000 langchain_discord-0.0.4/README.md
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:56:51.815830 langchain_discord-0.0.4/langchain_discord/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1689 2023-05-26 14:42:53.000000 langchain_discord-0.0.4/langchain_discord/webhook.py
+drwxr-xr-x   0 lennarddorst   (501) staff       (20)        0 2023-05-26 14:56:51.816610 langchain_discord-0.0.4/langchain_discord.egg-info/
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      739 2023-05-26 14:56:51.000000 langchain_discord-0.0.4/langchain_discord.egg-info/PKG-INFO
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      310 2023-05-26 14:56:51.000000 langchain_discord-0.0.4/langchain_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)        1 2023-05-26 14:56:51.000000 langchain_discord-0.0.4/langchain_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       17 2023-05-26 14:56:51.000000 langchain_discord-0.0.4/langchain_discord.egg-info/requires.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       18 2023-05-26 14:56:51.000000 langchain_discord-0.0.4/langchain_discord.egg-info/top_level.txt
+-rw-r--r--   0 lennarddorst   (501) staff       (20)      478 2023-05-26 14:56:35.000000 langchain_discord-0.0.4/pyproject.toml
+-rw-r--r--   0 lennarddorst   (501) staff       (20)       79 2023-05-26 14:56:51.817358 langchain_discord-0.0.4/setup.cfg
+-rw-r--r--   0 lennarddorst   (501) staff       (20)     1720 2023-05-26 14:56:38.000000 langchain_discord-0.0.4/setup.py
```

### Comparing `langchain_discord-0.0.3/LICENSE.txt` & `langchain_discord-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_discord-0.0.3/PKG-INFO` & `langchain_discord-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_discord
-Version: 0.0.3
+Version: 0.0.4
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.3/langchain_discord/webhook.py` & `langchain_discord-0.0.4/langchain_discord/webhook.py`

 * *Files identical despite different names*

### Comparing `langchain_discord-0.0.3/langchain_discord.egg-info/PKG-INFO` & `langchain_discord-0.0.4/langchain_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-discord
-Version: 0.0.3
+Version: 0.0.4
 Summary: A list of tools for LangChain to power Discord (Webhooks, etc.).
 Home-page: https://github.com/0w9/langchain-discord
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Lennard Dorst
 Author-email: Lennard Dorst <lennardsolana@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/0w9/langchain-discord
```

### Comparing `langchain_discord-0.0.3/setup.py` & `langchain_discord-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'langchain_discord',         # How you named your package folder (MyLib)
   packages = ['langchain_discord'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.04',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This package offers some easy-to-use tools to integrate Discord into LangChain for agents.',   # Give a short description about your library
   author = 'Lennard Dorst',                   # Type in your name
   author_email = 'lennardsolana@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/0w9/langchain-discord',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['AI', 'LangChain', 'Discord'],   # Keywords that define your package best
```


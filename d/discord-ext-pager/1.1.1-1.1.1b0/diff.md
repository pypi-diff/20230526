# Comparing `tmp/discord-ext-pager-1.1.1.tar.gz` & `tmp/discord-ext-pager-1.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.1.1.tar", last modified: Fri May 26 17:09:52 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.1.1b0.tar", last modified: Wed May 24 01:14:45 2023, max compression
```

## Comparing `discord-ext-pager-1.1.1.tar` & `discord-ext-pager-1.1.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-26 17:09:40.000000 discord-ext-pager-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-26 17:09:40.000000 discord-ext-pager-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-26 17:09:40.000000 discord-ext-pager-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/src/discord/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/src/discord/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/src/discord/ext/pager/
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-05-26 17:09:40.000000 discord-ext-pager-1.1.1/src/discord/ext/pager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:09:52.402432 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-26 17:09:52.000000 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:09:52.000000 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:09:52.000000 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 17:09:52.000000 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 17:09:52.000000 discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.410966 discord-ext-pager-1.1.1b0/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-24 01:14:33.000000 discord-ext-pager-1.1.1b0/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 01:14:45.414966 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 01:14:45.000000 discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.1.1/LICENSE` & `discord-ext-pager-1.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.1.1/PKG-INFO` & `discord-ext-pager-1.1.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.1.1
+Version: 1.1.1b0
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `discord-ext-pager-1.1.1/README.md` & `discord-ext-pager-1.1.1b0/README.md`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.1.1/pyproject.toml` & `discord-ext-pager-1.1.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord-ext-pager-1.1.1/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.1.1b0/src/discord/ext/pager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Union,
     cast,
 )
 
 import discord
 from typing_extensions import TypeAlias
 
-__version__ = "1.1.1"
+__version__ = "1.1.1b"
 
 __all__ = (
     "PageOption",
     "PageSource",
     "ListPageSource",
     "AsyncIteratorPageSource",
     "StopAction",
```

### Comparing `discord-ext-pager-1.1.1/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.1.1b0/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-ext-pager
-Version: 1.1.1
+Version: 1.1.1b0
 Summary: A view-based paginator library for discord.py 2.0
 Author: thegamecracks
 Project-URL: Homepage, https://github.com/thegamecracks/discord-ext-pager
 Keywords: discord,discord.py,paginator,view
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```


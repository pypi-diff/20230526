# Comparing `tmp/lifeguard-telegram-0.0.4.tar.gz` & `tmp/lifeguard-telegram-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-telegram-0.0.4.tar", last modified: Tue Jul  6 17:42:30 2021, max compression
+gzip compressed data, was "lifeguard-telegram-1.0.0.tar", last modified: Fri May 26 14:56:04 2023, max compression
```

## Comparing `lifeguard-telegram-0.0.4.tar` & `lifeguard-telegram-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/lifeguard_telegram/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/lifeguard_telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/lifeguard_telegram/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/lifeguard_telegram/bot_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/lifeguard_telegram/bot_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/lifeguard_telegram/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-07-06 17:42:30.000000 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2021-07-06 17:42:30.000000 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-06 17:42:30.000000 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-07-06 17:42:30.000000 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-06 17:42:30.000000 lifeguard-telegram-0.0.4/lifeguard_telegram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-06 17:42:30.679113 lifeguard-telegram-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-07-06 17:42:06.000000 lifeguard-telegram-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/lifeguard_telegram/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 14:56:04.000000 lifeguard-telegram-1.0.0/lifeguard_telegram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:56:04.952862 lifeguard-telegram-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 14:55:43.000000 lifeguard-telegram-1.0.0/setup.py
```

### Comparing `lifeguard-telegram-0.0.4/lifeguard_telegram/__init__.py` & `lifeguard-telegram-1.0.0/lifeguard_telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-0.0.4/lifeguard_telegram/bot.py` & `lifeguard-telegram-1.0.0/lifeguard_telegram/bot.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-0.0.4/lifeguard_telegram/bot_handlers/builtin_bot_handler.py` & `lifeguard-telegram-1.0.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-0.0.4/lifeguard_telegram/settings.py` & `lifeguard-telegram-1.0.0/lifeguard_telegram/settings.py`

 * *Files identical despite different names*


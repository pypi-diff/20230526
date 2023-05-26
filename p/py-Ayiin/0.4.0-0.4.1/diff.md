# Comparing `tmp/py-Ayiin-0.4.0.tar.gz` & `tmp/py-Ayiin-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.0.tar", last modified: Thu May 25 13:12:34 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.1.tar", last modified: Fri May 26 06:49:17 2023, max compression
```

## Comparing `py-Ayiin-0.4.0.tar` & `py-Ayiin-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.312662 py-Ayiin-0.4.0/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.312662 py-Ayiin-0.4.0/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12526 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.316662 py-Ayiin-0.4.0/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.316662 py-Ayiin-0.4.0/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.316662 py-Ayiin-0.4.0/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.316662 py-Ayiin-0.4.0/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 13:12:34.000000 py-Ayiin-0.4.0/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-25 13:12:34.000000 py-Ayiin-0.4.0/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:12:34.000000 py-Ayiin-0.4.0/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 13:12:34.000000 py-Ayiin-0.4.0/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 13:12:34.000000 py-Ayiin-0.4.0/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:12:34.320662 py-Ayiin-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-25 13:12:22.000000 py-Ayiin-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.998320 py-Ayiin-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-26 06:49:16.998320 py-Ayiin-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.990320 py-Ayiin-0.4.1/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.990320 py-Ayiin-0.4.1/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12526 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:49:16.994320 py-Ayiin-0.4.1/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-26 06:49:16.000000 py-Ayiin-0.4.1/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-26 06:49:16.000000 py-Ayiin-0.4.1/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:49:16.000000 py-Ayiin-0.4.1/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 06:49:16.000000 py-Ayiin-0.4.1/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 06:49:16.000000 py-Ayiin-0.4.1/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:49:16.998320 py-Ayiin-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 06:49:07.000000 py-Ayiin-0.4.1/setup.py
```

### Comparing `py-Ayiin-0.4.0/LICENSE` & `py-Ayiin-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/NOTICE` & `py-Ayiin-0.4.1/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/PKG-INFO` & `py-Ayiin-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.0/README.md` & `py-Ayiin-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.1/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.1/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.1/pyAyiin/Clients/pytgcalls.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 
 import asyncio
 import os
 import yt_dlp
 
 from typing import Optional, Union
 
+from fipper import Client
 from fipper.types import Message
 from fipper.raw.functions.channels import GetFullChannel
 from fipper.raw.functions.messages import GetFullChat
 from fipper.raw.functions.phone import CreateGroupCall, DiscardGroupCall, EditGroupCallTitle
 from fipper.raw.types import InputGroupCall, InputPeerChannel, InputPeerChat
 
 from pytgcalls.exceptions import GroupCallNotFoundError
 
-from ..methods.queue import Queues, QUEUE
+from ..methods.queue import Queues
 
 from .client import *
 
 
 ACTIVE_CALLS, QUEUE = [], {}
 MSGID_CACHE, PLAY_ON = {}, {}
 CLIENTS = {}
```

### Comparing `py-Ayiin-0.4.0/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.1/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/__init__.py` & `py-Ayiin-0.4.1/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.4.0/pyAyiin/__main__.py` & `py-Ayiin-0.4.1/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/assistant.py` & `py-Ayiin-0.4.1/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/config.py` & `py-Ayiin-0.4.1/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.1/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.1/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.1/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.1/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.1/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.1/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.1/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.1/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.1/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.1/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.1/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.1/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/start.py` & `py-Ayiin-0.4.1/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.1/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.1/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.1/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.1/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/decorator.py` & `py-Ayiin-0.4.1/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/exceptions.py` & `py-Ayiin-0.4.1/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.1/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.1/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.1/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.1/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/func.py` & `py-Ayiin-0.4.1/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.1/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.1/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.1/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.1/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.1/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.1/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.1/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/pyAyiin/xd.py` & `py-Ayiin-0.4.1/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.1/py_Ayiin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.0/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.1/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.0/setup.py` & `py-Ayiin-0.4.1/setup.py`

 * *Files identical despite different names*


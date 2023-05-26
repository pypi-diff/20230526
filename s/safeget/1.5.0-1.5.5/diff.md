# Comparing `tmp/safeget-1.5.0.tar.gz` & `tmp/safeget-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeget-1.5.0.tar", last modified: Sun Nov 27 11:24:54 2022, max compression
+gzip compressed data, was "safeget-1.5.5.tar", last modified: Fri May 26 13:50:25 2023, max compression
```

## Comparing `safeget-1.5.0.tar` & `safeget-1.5.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.945075 safeget-1.5.0/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      594 2022-04-23 12:12:52.000000 safeget-1.5.0/LICENSE
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       28 2022-04-23 12:12:52.000000 safeget-1.5.0/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3868 2022-11-27 11:24:54.945075 safeget-1.5.0/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2538 2022-11-27 11:24:40.000000 safeget-1.5.0/README.md
-drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.945075 safeget-1.5.0/bin/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    45021 2022-11-27 11:24:54.000000 safeget-1.5.0/bin/safeget
-drwxr-sr-x   0 ramblin   (1000) ramblin   (1000)        0 2022-11-27 11:24:54.945075 safeget-1.5.0/safeget.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3868 2022-11-27 11:24:54.000000 safeget-1.5.0/safeget.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      174 2022-11-27 11:24:54.000000 safeget-1.5.0/safeget.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2022-11-27 11:24:54.000000 safeget-1.5.0/safeget.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        8 2022-11-27 11:24:54.000000 safeget-1.5.0/safeget.egg-info/top_level.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2022-11-27 11:24:54.945075 safeget-1.5.0/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1956 2022-11-27 11:24:54.000000 safeget-1.5.0/setup.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-26 13:50:25.426651 safeget-1.5.5/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2023-05-20 22:43:49.000000 safeget-1.5.5/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9619 2023-05-26 13:50:25.426651 safeget-1.5.5/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7279 2023-05-24 06:13:24.000000 safeget-1.5.5/README.md
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-26 13:50:25.422651 safeget-1.5.5/bin/
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    45027 2023-05-26 13:49:55.000000 safeget-1.5.5/bin/safeget
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-26 13:50:25.426651 safeget-1.5.5/safeget.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9619 2023-05-26 13:50:18.000000 safeget-1.5.5/safeget.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      197 2023-05-26 13:50:20.000000 safeget-1.5.5/safeget.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2023-05-26 13:50:18.000000 safeget-1.5.5/safeget.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       12 2023-05-26 13:50:18.000000 safeget-1.5.5/safeget.egg-info/top_level.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2023-05-26 13:50:25.426651 safeget-1.5.5/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1811 2023-05-26 13:49:55.000000 safeget-1.5.5/setup.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-26 13:50:25.426651 safeget-1.5.5/src/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2022-04-23 12:12:53.000000 safeget-1.5.5/src/__init__.py
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    45027 2023-05-26 08:58:34.000000 safeget-1.5.5/src/safeget.py
```

### Comparing `safeget-1.5.0/bin/safeget` & `safeget-1.5.5/bin/safeget`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 '''
     Safeget downloads and verifies files from online.
     It requires signed hashes, signed message, or a signature
     verified with a matching PGP key.
 
     If you would like a simple custom safeget for your app
     which embeds all the parameters usually passed on the
-    command line, contact support@denova.com. It's free.
+    command line, contact support@github.com/safeapps. It's free.
     Your users then run that simple small program to download
     and fully verify your app, without the hassles.
 
-    Learn more at https://denova.com/open/safeget/
-
     This is intentionally a single file to make it easier
     to verify safeget itself.
 
-    Copyright 2019-2022 DeNova
-    Last modified: 2022-11-23
+    Copyright 2019-2023 safeapps
+    Last modified: 2023-05-26
 '''
 
 import argparse
 import hashlib
 import json
 import os
 import platform
@@ -36,16 +34,16 @@
 from tempfile import mkdtemp
 from traceback import format_exc
 from urllib.error import HTTPError, URLError
 from urllib.parse import urlencode, urlparse
 from urllib.request import build_opener, urlopen, HTTPCookieProcessor, ProxyHandler, Request
 
 
-CURRENT_VERSION = '1.5.0'
-COPYRIGHT = 'Copyright 2019-2022 DeNova'
+CURRENT_VERSION = '1.5.5'
+COPYRIGHT = 'Copyright 2019-2023 safeapps'
 LICENSE = 'GPLv3'
 
 DEFAULT_TRIES = 20 # wget default
 # use standard text streams for stdin, stdout and stderr
 STD_TEXT_STREAMS = True
 TMP_DIR = mkdtemp(prefix='safeget.')
 
@@ -151,15 +149,15 @@
         details = f'\nSafeget {CURRENT_VERSION}\n{COPYRIGHT}\nLicense: {LICENSE}\n\n'
         notice(details)
 
 def more():
     ''' Let them know where to get more safeget commands. '''
 
     print('\n')
-    print('Find more safegets at https://denova.com/open/safeget/custom/')
+    print('Find more safegets at https://github.com/safeapps/open/safeget/custom/')
     print('\n')
 
 def notice(msg):
     ''' Print short notice message without newline. '''
 
     print(msg, end='', flush=True)
 
@@ -574,15 +572,15 @@
 def check_safeget_itself(host=None, target=None):
     '''
         Check safeget itself by checking the online
         database for original file size and hashes.
 
         The parameters are only passed for testing.
     '''
-    HEADERS = {'User-Agent': 'DeNova Safeget 1.0'}
+    HEADERS = {'User-Agent': 'solidlibs Safeget 1.0'}
 
     ok = True
     error_message = None
 
     full_api_url, encoded_params, opener = setup_safeget_check(host=host, target=target)
     request = Request(full_api_url, encoded_params, HEADERS)
 
@@ -619,15 +617,15 @@
 def setup_safeget_check(host=None, target=None):
     '''
         Set up to check safeget itself.
 
         The parameters are only passed for testing.
     '''
 
-    HOST = 'https://denova.com'
+    HOST = 'https://github.com/safeapps'
     API_URL = 'open/safeget/api/'
 
     if host is None:
         host = HOST
 
     if target is None:
         target = args.target
@@ -1227,20 +1225,20 @@
 
     return args
 
 def get_details_for_failure(url, attempts, reason):
     '''
         Get the details about the failure.
 
-        >>> url = 'https://denova.com/open/safecopy'
+        >>> url = 'https://github.com/safeapps/open/safecopy'
         >>> attempts = DEFAULT_TRIES
         >>> reason = '[Errno 53] Unable to reach server.'
         >>> message = get_details_for_failure(url, attempts, reason)
         Attempted to download 20 time(s)
-        >>> 'Unable to safely get https://denova.com/open/safecopy.\\n' in message
+        >>> 'Unable to safely get https://github.com/safeapps/open/safecopy.\\n' in message
         True
         >>> '\\tError: Unable to reach server.\\n' in message
         True
         >>> '\\tSuggestions: Check connections or try again later.' in message
         True
     '''
 
@@ -1336,18 +1334,18 @@
 
         >>> command_args = ['ls', '-l', gettempdir()]
         >>> kwargs = {}
         >>> get_run_args(*command_args, **kwargs)
         (['ls', '-l', '/tmp'], {})
 
         >>> # test command line with glob=False
-        >>> command_args = ['ls', '-l', f'{gettempdir()}/denova*']
+        >>> command_args = ['ls', '-l', f'{gettempdir()}/solidlibs*']
         >>> kwargs = {'glob': False}
         >>> get_run_args(*command_args, **kwargs)
-        (['ls', '-l', '/tmp/denova*'], {})
+        (['ls', '-l', '/tmp/solidlibs*'], {})
     '''
 
     if kwargs is None:
         kwargs = {}
 
     if 'glob' in kwargs:
         globbing = kwargs['glob']
```


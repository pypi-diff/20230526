# Comparing `tmp/eva4-repl-legacy-0.0.7.tar.gz` & `tmp/eva4-repl-legacy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva4-repl-legacy-0.0.7.tar", last modified: Fri Apr  1 19:02:28 2022, max compression
+gzip compressed data, was "eva4-repl-legacy-0.0.9.tar", last modified: Fri Apr  1 21:33:41 2022, max compression
```

## Comparing `eva4-repl-legacy-0.0.7.tar` & `eva4-repl-legacy-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/
--rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       46 2022-03-19 18:21:20.000000 eva4-repl-legacy-0.0.7/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       71 2022-03-22 22:13:22.000000 eva4-repl-legacy-0.0.7/bin/eva4-repl-legacy
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/eva4_repl_legacy/
--rw-r--r--   0 divisor   (1000) root         (0)    19703 2022-04-01 19:02:16.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 19:02:28.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      267 2022-04-01 19:02:28.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-01 19:02:28.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      112 2022-04-01 19:02:28.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       17 2022-04-01 19:02:28.000000 eva4-repl-legacy-0.0.7/eva4_repl_legacy.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-01 19:02:28.322616 eva4-repl-legacy-0.0.7/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1143 2022-04-01 19:02:16.000000 eva4-repl-legacy-0.0.7/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/
+-rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       46 2022-03-19 18:21:20.000000 eva4-repl-legacy-0.0.9/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.302387 eva4-repl-legacy-0.0.9/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       71 2022-03-22 22:13:22.000000 eva4-repl-legacy-0.0.9/bin/eva4-repl-legacy
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/eva4_repl_legacy/
+-rw-r--r--   0 divisor   (1000) root         (0)    19703 2022-04-01 21:33:39.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      509 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      267 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)      112 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       17 2022-04-01 21:33:41.000000 eva4-repl-legacy-0.0.9/eva4_repl_legacy.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2022-04-01 21:33:41.306388 eva4-repl-legacy-0.0.9/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1143 2022-04-01 21:33:39.000000 eva4-repl-legacy-0.0.9/setup.py
```

### Comparing `eva4-repl-legacy-0.0.7/eva4_repl_legacy/__init__.py` & `eva4-repl-legacy-0.0.9/eva4_repl_legacy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.7'
+__version__ = '0.0.9'
 
 import evaics.sdk as sdk
 from types import SimpleNamespace
 import psrt
 import threading
 import msgpack
 import time
```

### Comparing `eva4-repl-legacy-0.0.7/setup.py` & `eva4-repl-legacy-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.7'
+__version__ = '0.0.9'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva4-repl-legacy',
@@ -12,15 +12,15 @@
                  description='EVA ICS v4 legacy replication service',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/alttch/eva4',
                  packages=setuptools.find_packages(),
                  license='Apache License 2.0',
                  install_requires=[
-                     'cachetools>=4.11', 'elbus>=0.0.14', 'evaics>=0.0.7',
+                     'cachetools>=4.11', 'elbus>=0.0.14', 'evaics>=0.0.9',
                      'msgpack>=1.0.3', 'psrt>=0.0.18', 'pyaltt2>=0.0.116',
                      'pycryptodomex>=3.12.0'
                  ],
                  classifiers=('Programming Language :: Python :: 3',
                               'License :: OSI Approved :: MIT License',
                               'Topic :: Communications'),
                  scripts=['bin/eva4-repl-legacy'])
```


# Comparing `tmp/torchbones-1.0.1.tar.gz` & `tmp/torchbones-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.0.1.tar", last modified: Fri May 26 18:52:53 2023, max compression
+gzip compressed data, was "torchbones-1.0.3.tar", last modified: Fri May 26 19:21:54 2023, max compression
```

## Comparing `torchbones-1.0.1.tar` & `torchbones-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 18:52:53.379106 torchbones-1.0.1/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 18:52:53.379106 torchbones-1.0.1/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 18:52:53.379106 torchbones-1.0.1/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      470 2023-05-26 18:52:18.000000 torchbones-1.0.1/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 18:52:53.379106 torchbones-1.0.1/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 18:52:53.000000 torchbones-1.0.1/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      177 2023-05-26 18:52:53.000000 torchbones-1.0.1/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 18:52:53.000000 torchbones-1.0.1/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 18:52:53.000000 torchbones-1.0.1/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 18:52:53.000000 torchbones-1.0.1/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:21:54.685776 torchbones-1.0.3/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 19:21:54.685776 torchbones-1.0.3/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 19:21:54.696610 torchbones-1.0.3/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      441 2023-05-26 19:21:51.000000 torchbones-1.0.3/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:21:54.685776 torchbones-1.0.3/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:11:15.000000 torchbones-1.0.3/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    14981 2023-05-26 17:39:33.000000 torchbones-1.0.3/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:21:54.685776 torchbones-1.0.3/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 19:21:54.000000 torchbones-1.0.3/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-26 19:21:54.000000 torchbones-1.0.3/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 19:21:54.000000 torchbones-1.0.3/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 19:21:54.000000 torchbones-1.0.3/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-26 19:21:54.000000 torchbones-1.0.3/torchbones.egg-info/top_level.txt
```


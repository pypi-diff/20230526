# Comparing `tmp/packagetestbancolombia-0.1.tar.gz` & `tmp/packagetestbancolombia-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagetestbancolombia-0.1.tar", last modified: Tue May 23 20:57:33 2023, max compression
+gzip compressed data, was "packagetestbancolombia-1.0.2.tar", last modified: Fri May 26 08:50:49 2023, max compression
```

## Comparing `packagetestbancolombia-0.1.tar` & `packagetestbancolombia-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:57:33.641398 packagetestbancolombia-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 20:57:33.641398 packagetestbancolombia-0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:57:33.641398 packagetestbancolombia-0.1/packagetestbancolombia/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 20:57:22.000000 packagetestbancolombia-0.1/packagetestbancolombia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 20:57:22.000000 packagetestbancolombia-0.1/packagetestbancolombia/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:57:33.641398 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 20:57:33.000000 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-23 20:57:33.000000 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:57:33.000000 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:57:33.000000 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 20:57:33.000000 packagetestbancolombia-0.1/packagetestbancolombia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:57:33.641398 packagetestbancolombia-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 20:57:22.000000 packagetestbancolombia-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:49.808059 packagetestbancolombia-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 08:50:49.808059 packagetestbancolombia-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:49.808059 packagetestbancolombia-1.0.2/packagetestbancolombia/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 08:50:35.000000 packagetestbancolombia-1.0.2/packagetestbancolombia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:50:35.000000 packagetestbancolombia-1.0.2/packagetestbancolombia/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:49.808059 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 08:50:49.000000 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 08:50:49.000000 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:50:49.000000 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:50:49.000000 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 08:50:49.000000 packagetestbancolombia-1.0.2/packagetestbancolombia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:50:49.808059 packagetestbancolombia-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 08:50:35.000000 packagetestbancolombia-1.0.2/setup.py
```


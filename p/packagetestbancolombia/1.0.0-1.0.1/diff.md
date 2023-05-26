# Comparing `tmp/packagetestbancolombia-1.0.0.tar.gz` & `tmp/packagetestbancolombia-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagetestbancolombia-1.0.0.tar", last modified: Fri May 26 13:17:43 2023, max compression
+gzip compressed data, was "packagetestbancolombia-1.0.1.tar", last modified: Fri May 26 13:26:24 2023, max compression
```

## Comparing `packagetestbancolombia-1.0.0.tar` & `packagetestbancolombia-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:17:43.968760 packagetestbancolombia-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 13:17:43.968760 packagetestbancolombia-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:17:43.968760 packagetestbancolombia-1.0.0/packagetestbancolombia/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 13:17:29.000000 packagetestbancolombia-1.0.0/packagetestbancolombia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:17:29.000000 packagetestbancolombia-1.0.0/packagetestbancolombia/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:17:43.968760 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 13:17:43.000000 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 13:17:43.000000 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:17:43.000000 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:17:43.000000 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 13:17:43.000000 packagetestbancolombia-1.0.0/packagetestbancolombia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:17:43.968760 packagetestbancolombia-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 13:17:29.000000 packagetestbancolombia-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:26:24.787821 packagetestbancolombia-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 13:26:24.787821 packagetestbancolombia-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:26:24.787821 packagetestbancolombia-1.0.1/packagetestbancolombia/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 13:26:13.000000 packagetestbancolombia-1.0.1/packagetestbancolombia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:26:13.000000 packagetestbancolombia-1.0.1/packagetestbancolombia/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:26:24.787821 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 13:26:24.000000 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 13:26:24.000000 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:26:24.000000 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:26:24.000000 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 13:26:24.000000 packagetestbancolombia-1.0.1/packagetestbancolombia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:26:24.787821 packagetestbancolombia-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 13:26:13.000000 packagetestbancolombia-1.0.1/setup.py
```


# Comparing `tmp/silicron-0.0.1.tar.gz` & `tmp/silicron-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicron-0.0.1.tar", last modified: Tue May 23 08:36:34 2023, max compression
+gzip compressed data, was "silicron-0.0.2.tar", last modified: Fri May 26 07:42:54 2023, max compression
```

## Comparing `silicron-0.0.1.tar` & `silicron-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-23 08:36:34.655327 silicron-0.0.1/
--rw-r--r--   0 michael    (501) staff       (20)      217 2023-05-23 08:36:34.655193 silicron-0.0.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      311 2023-05-23 07:59:14.000000 silicron-0.0.1/README.md
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-23 08:36:34.655385 silicron-0.0.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      347 2023-05-23 08:26:48.000000 silicron-0.0.1/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-23 08:36:34.653938 silicron-0.0.1/silicron/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-23 08:36:26.000000 silicron-0.0.1/silicron/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      107 2023-05-23 08:23:26.000000 silicron-0.0.1/silicron/main.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-23 08:36:34.654710 silicron-0.0.1/silicron.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)      217 2023-05-23 08:36:34.000000 silicron-0.0.1/silicron.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      242 2023-05-23 08:36:34.000000 silicron-0.0.1/silicron.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-23 08:36:34.000000 silicron-0.0.1/silicron.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)        8 2023-05-23 08:36:34.000000 silicron-0.0.1/silicron.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2023-05-23 08:36:34.000000 silicron-0.0.1/silicron.egg-info/top_level.txt
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-23 08:36:34.654967 silicron-0.0.1/tmp/
--rw-r--r--   0 michael    (501) staff       (20)       26 2023-05-20 02:25:45.000000 silicron-0.0.1/tmp/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5403 2023-05-23 07:59:14.000000 silicron-0.0.1/tmp/api.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.317426 silicron-0.0.2/
+-rw-r--r--   0 michael    (501) staff       (20)      320 2023-05-26 07:42:54.317295 silicron-0.0.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1063 2023-05-26 07:37:06.000000 silicron-0.0.2/README.md
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-26 07:42:54.317479 silicron-0.0.2/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      558 2023-05-26 07:41:26.000000 silicron-0.0.2/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.316462 silicron-0.0.2/silicron/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-24 06:45:57.000000 silicron-0.0.2/silicron/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-05-26 07:42:39.000000 silicron-0.0.2/silicron/api.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-26 07:42:54.317079 silicron-0.0.2/silicron.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)      320 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      183 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)        9 2023-05-26 07:42:54.000000 silicron-0.0.2/silicron.egg-info/top_level.txt
```


# Comparing `tmp/intra42-0.1.0.tar.gz` & `tmp/intra42-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intra42-0.1.0.tar", last modified: Thu May 25 20:45:48 2023, max compression
+gzip compressed data, was "intra42-0.1.1.tar", last modified: Fri May 26 17:46:30 2023, max compression
```

## Comparing `intra42-0.1.0.tar` & `intra42-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-25 20:45:48.250723 intra42-0.1.0/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-25 20:45:48.250723 intra42-0.1.0/PKG-INFO
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-25 20:45:48.250723 intra42-0.1.0/intra42.egg-info/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-25 20:45:48.000000 intra42-0.1.0/intra42.egg-info/PKG-INFO
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-25 20:45:48.000000 intra42-0.1.0/intra42.egg-info/SOURCES.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-25 20:45:48.000000 intra42-0.1.0/intra42.egg-info/dependency_links.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-25 20:45:48.000000 intra42-0.1.0/intra42.egg-info/requires.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-25 20:45:48.000000 intra42-0.1.0/intra42.egg-info/top_level.txt
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-25 20:45:48.250723 intra42-0.1.0/intrascraper/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       47 2023-05-25 19:07:57.000000 intra42-0.1.0/intrascraper/__init__.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     1547 2023-05-25 19:07:17.000000 intra42-0.1.0/intrascraper/intrascraper.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-25 20:45:48.250723 intra42-0.1.0/setup.cfg
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      439 2023-05-25 20:45:18.000000 intra42-0.1.0/setup.py
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.087753 intra42-0.1.1/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-26 17:46:30.087753 intra42-0.1.1/PKG-INFO
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.083753 intra42-0.1.1/intra42.egg-info/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/PKG-INFO
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/SOURCES.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/dependency_links.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/requires.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/top_level.txt
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.087753 intra42-0.1.1/intrascraper/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      105 2023-05-26 17:24:40.000000 intra42-0.1.1/intrascraper/__init__.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5539 2023-05-26 17:34:19.000000 intra42-0.1.1/intrascraper/intrascraper.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-26 17:46:30.087753 intra42-0.1.1/setup.cfg
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-26 17:46:24.000000 intra42-0.1.1/setup.py
```


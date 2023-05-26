# Comparing `tmp/limpo-0.0.2.tar.gz` & `tmp/limpo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limpo-0.0.2.tar", last modified: Fri May 26 07:28:31 2023, max compression
+gzip compressed data, was "limpo-0.0.3.tar", last modified: Fri May 26 08:23:56 2023, max compression
```

## Comparing `limpo-0.0.2.tar` & `limpo-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 07:28:31.336884 limpo-0.0.2/
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      215 2023-05-26 07:28:31.336749 limpo-0.0.2/PKG-INFO
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        7 2023-05-25 09:50:15.000000 limpo-0.0.2/README.md
-drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 07:28:31.335917 limpo-0.0.2/limpo/
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)       12 2023-05-26 07:17:37.000000 limpo-0.0.2/limpo/__init__.py
-drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 07:28:31.336583 limpo-0.0.2/limpo.egg-info/
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      215 2023-05-26 07:28:31.000000 limpo-0.0.2/limpo.egg-info/PKG-INFO
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      152 2023-05-26 07:28:31.000000 limpo-0.0.2/limpo.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        1 2023-05-26 07:28:31.000000 limpo-0.0.2/limpo.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        6 2023-05-26 07:28:31.000000 limpo-0.0.2/limpo.egg-info/top_level.txt
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)       38 2023-05-26 07:28:31.336926 limpo-0.0.2/setup.cfg
--rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      479 2023-05-26 07:25:54.000000 limpo-0.0.2/setup.py
+drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 08:23:56.692862 limpo-0.0.3/
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)     1076 2023-05-26 07:40:32.000000 limpo-0.0.3/LICENSE.text
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      341 2023-05-26 08:23:56.692730 limpo-0.0.3/PKG-INFO
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        7 2023-05-25 09:50:15.000000 limpo-0.0.3/README.md
+drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 08:23:56.692041 limpo-0.0.3/limpo/
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)       30 2023-05-26 08:23:23.000000 limpo-0.0.3/limpo/__init__.py
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)     1409 2023-05-26 08:23:23.000000 limpo-0.0.3/limpo/limpo.py
+drwxr-xr-x   0 alexanderbrueck_p   (502) staff       (20)        0 2023-05-26 08:23:56.692550 limpo-0.0.3/limpo.egg-info/
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      341 2023-05-26 08:23:56.000000 limpo-0.0.3/limpo.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      180 2023-05-26 08:23:56.000000 limpo-0.0.3/limpo.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        1 2023-05-26 08:23:56.000000 limpo-0.0.3/limpo.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)        6 2023-05-26 08:23:56.000000 limpo-0.0.3/limpo.egg-info/top_level.txt
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)       38 2023-05-26 08:23:56.692905 limpo-0.0.3/setup.cfg
+-rw-r--r--   0 alexanderbrueck_p   (502) staff       (20)      604 2023-05-26 08:23:49.000000 limpo-0.0.3/setup.py
```


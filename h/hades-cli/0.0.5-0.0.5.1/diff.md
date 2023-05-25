# Comparing `tmp/hades-cli-0.0.5.tar.gz` & `tmp/hades-cli-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-cli-0.0.5.tar", last modified: Thu May 25 23:02:57 2023, max compression
+gzip compressed data, was "hades-cli-0.0.5.1.tar", last modified: Thu May 25 23:10:11 2023, max compression
```

## Comparing `hades-cli-0.0.5.tar` & `hades-cli-0.0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.935629 hades-cli-0.0.5/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 23:02:57.935462 hades-cli-0.0.5/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.931125 hades-cli-0.0.5/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.5/app/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.931631 hades-cli-0.0.5/app/handlers/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.5/app/handlers/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.932345 hades-cli-0.0.5/app/handlers/generate/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.5/app/handlers/generate/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.5/app/handlers/generate/backend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2526 2023-05-25 23:01:21.000000 hades-cli-0.0.5/app/handlers/generate/frontend.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.933892 hades-cli-0.0.5/app/resources/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.5/app/resources/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.5/app/resources/chakra.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.5/app/resources/redux.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.5/app/resources/router.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.5/app/resources/tailwind.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      718 2023-05-25 23:02:45.000000 hades-cli-0.0.5/app/start.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.5/app/utils.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:02:57.935202 hades-cli-0.0.5/hades_cli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:02:57.000000 hades-cli-0.0.5/hades_cli.egg-info/top_level.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:02:57.935690 hades-cli-0.0.5/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      557 2023-05-25 23:02:50.000000 hades-cli-0.0.5/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.744014 hades-cli-0.0.5.1/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      154 2023-05-25 23:10:11.743845 hades-cli-0.0.5.1/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.739279 hades-cli-0.0.5.1/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.5.1/app/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.739696 hades-cli-0.0.5.1/app/handlers/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.5.1/app/handlers/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.740320 hades-cli-0.0.5.1/app/handlers/generate/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.5.1/app/handlers/generate/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.5.1/app/handlers/generate/backend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2526 2023-05-25 23:01:21.000000 hades-cli-0.0.5.1/app/handlers/generate/frontend.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.742214 hades-cli-0.0.5.1/app/resources/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.5.1/app/resources/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.5.1/app/resources/chakra.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.5.1/app/resources/redux.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.5.1/app/resources/router.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.5.1/app/resources/tailwind.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      718 2023-05-25 23:02:45.000000 hades-cli-0.0.5.1/app/start.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.5.1/app/utils.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:10:11.743581 hades-cli-0.0.5.1/hades_cli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      154 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:10:11.000000 hades-cli-0.0.5.1/hades_cli.egg-info/top_level.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:10:11.744069 hades-cli-0.0.5.1/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      511 2023-05-25 23:10:05.000000 hades-cli-0.0.5.1/setup.py
```

### Comparing `hades-cli-0.0.5/app/handlers/generate/backend.py` & `hades-cli-0.0.5.1/app/handlers/generate/backend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/handlers/generate/frontend.py` & `hades-cli-0.0.5.1/app/handlers/generate/frontend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/resources/chakra.py` & `hades-cli-0.0.5.1/app/resources/chakra.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/resources/redux.py` & `hades-cli-0.0.5.1/app/resources/redux.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/resources/router.py` & `hades-cli-0.0.5.1/app/resources/router.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/resources/tailwind.py` & `hades-cli-0.0.5.1/app/resources/tailwind.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/app/start.py` & `hades-cli-0.0.5.1/app/start.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5/hades_cli.egg-info/requires.txt` & `hades-cli-0.0.5.1/hades_cli.egg-info/requires.txt`

 * *Files identical despite different names*


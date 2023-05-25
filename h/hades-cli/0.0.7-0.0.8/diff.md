# Comparing `tmp/hades-cli-0.0.7.tar.gz` & `tmp/hades-cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-cli-0.0.7.tar", last modified: Thu May 25 23:52:30 2023, max compression
+gzip compressed data, was "hades-cli-0.0.8.tar", last modified: Thu May 25 23:55:00 2023, max compression
```

## Comparing `hades-cli-0.0.7.tar` & `hades-cli-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.417146 hades-cli-0.0.7/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:52:30.416992 hades-cli-0.0.7/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.414390 hades-cli-0.0.7/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:25.000000 hades-cli-0.0.7/app/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.414550 hades-cli-0.0.7/app/handlers/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.7/app/handlers/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.414939 hades-cli-0.0.7/app/handlers/generate/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.7/app/handlers/generate/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.7/app/handlers/generate/backend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2614 2023-05-25 23:36:20.000000 hades-cli-0.0.7/app/handlers/generate/frontend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      736 2023-05-25 23:43:19.000000 hades-cli-0.0.7/app/main.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.415846 hades-cli-0.0.7/app/resources/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.7/app/resources/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.7/app/resources/chakra.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.7/app/resources/redux.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.7/app/resources/router.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.7/app/resources/tailwind.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.7/app/resources/utils.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:52:30.416786 hades-cli-0.0.7/hades_cli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      508 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       39 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:52:30.000000 hades-cli-0.0.7/hades_cli.egg-info/top_level.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:52:30.417200 hades-cli-0.0.7/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      507 2023-05-25 23:52:26.000000 hades-cli-0.0.7/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.663421 hades-cli-0.0.8/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:55:00.663266 hades-cli-0.0.8/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.660167 hades-cli-0.0.8/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:25.000000 hades-cli-0.0.8/app/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.660329 hades-cli-0.0.8/app/handlers/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.8/app/handlers/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.660910 hades-cli-0.0.8/app/handlers/generate/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.8/app/handlers/generate/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.8/app/handlers/generate/backend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2547 2023-05-25 23:54:14.000000 hades-cli-0.0.8/app/handlers/generate/frontend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      742 2023-05-25 23:54:40.000000 hades-cli-0.0.8/app/main.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.661831 hades-cli-0.0.8/app/resources/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.8/app/resources/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.8/app/resources/chakra.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.8/app/resources/redux.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.8/app/resources/router.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.8/app/resources/tailwind.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.8/app/resources/utils.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:55:00.663001 hades-cli-0.0.8/hades_cli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      508 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       39 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:55:00.000000 hades-cli-0.0.8/hades_cli.egg-info/top_level.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:55:00.663476 hades-cli-0.0.8/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      507 2023-05-25 23:54:53.000000 hades-cli-0.0.8/setup.py
```

### Comparing `hades-cli-0.0.7/app/handlers/generate/backend.py` & `hades-cli-0.0.8/app/handlers/generate/backend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.7/app/handlers/generate/frontend.py` & `hades-cli-0.0.8/app/handlers/generate/frontend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 from inquirer import prompt, Text, Confirm, List
 import boto3
 import sys
 
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "../..")))
 
-from resources.redux import Redux
-from resources.tailwind import Tailwind
-from resources.router import Router
-from resources.chakra import Chakra
+from app.resources.redux import Redux
+from app.resources.tailwind import Tailwind
+from app.resources.router import Router
+from app.resources.chakra import Chakra
 
 __ui_frameworks__ = [
     "none",
     "chakra-ui",
     "material-ui",
     "react-bootstrap",
     "react-md",
```

### Comparing `hades-cli-0.0.7/app/main.py` & `hades-cli-0.0.8/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
-from .handlers.generate.frontend import FrontendGenerator
-from .handlers.generate.backend import BackendGenerator
+from app.handlers.generate.frontend import FrontendGenerator
+from app.handlers.generate.backend import BackendGenerator
 import os
 import pyfiglet
 
 pyfiglet.print_figlet("Hades Toolkit")
 
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
```

### Comparing `hades-cli-0.0.7/app/resources/chakra.py` & `hades-cli-0.0.8/app/resources/chakra.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.7/app/resources/redux.py` & `hades-cli-0.0.8/app/resources/redux.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.7/app/resources/router.py` & `hades-cli-0.0.8/app/resources/router.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.7/app/resources/tailwind.py` & `hades-cli-0.0.8/app/resources/tailwind.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.7/hades_cli.egg-info/requires.txt` & `hades-cli-0.0.8/hades_cli.egg-info/requires.txt`

 * *Files identical despite different names*


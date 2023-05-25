# Comparing `tmp/hades-cli-0.0.5.2.tar.gz` & `tmp/hades-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-cli-0.0.5.2.tar", last modified: Thu May 25 23:20:36 2023, max compression
+gzip compressed data, was "hades-cli-0.0.6.tar", last modified: Thu May 25 23:21:50 2023, max compression
```

## Comparing `hades-cli-0.0.5.2.tar` & `hades-cli-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.088841 hades-cli-0.0.5.2/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      154 2023-05-25 23:20:36.088703 hades-cli-0.0.5.2/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.084365 hades-cli-0.0.5.2/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.5.2/app/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      718 2023-05-25 23:20:14.000000 hades-cli-0.0.5.2/app/application.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.084509 hades-cli-0.0.5.2/app/handlers/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.5.2/app/handlers/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.084901 hades-cli-0.0.5.2/app/handlers/generate/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.5.2/app/handlers/generate/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.5.2/app/handlers/generate/backend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2534 2023-05-25 23:19:50.000000 hades-cli-0.0.5.2/app/handlers/generate/frontend.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.087034 hades-cli-0.0.5.2/app/resources/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.5.2/app/resources/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.5.2/app/resources/chakra.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.5.2/app/resources/redux.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.5.2/app/resources/router.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.5.2/app/resources/tailwind.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.5.2/app/utils.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:20:36.088497 hades-cli-0.0.5.2/hades_cli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      154 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      505 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       46 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:20:36.000000 hades-cli-0.0.5.2/hades_cli.egg-info/top_level.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:20:36.088887 hades-cli-0.0.5.2/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      531 2023-05-25 23:20:08.000000 hades-cli-0.0.5.2/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.580245 hades-cli-0.0.6/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:21:50.580087 hades-cli-0.0.6/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.575755 hades-cli-0.0.6/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.6/app/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      716 2023-05-25 23:21:44.000000 hades-cli-0.0.6/app/application.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.576305 hades-cli-0.0.6/app/handlers/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.6/app/handlers/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.576924 hades-cli-0.0.6/app/handlers/generate/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.6/app/handlers/generate/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.6/app/handlers/generate/backend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2534 2023-05-25 23:19:50.000000 hades-cli-0.0.6/app/handlers/generate/frontend.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.578249 hades-cli-0.0.6/app/resources/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.6/app/resources/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.6/app/resources/chakra.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.6/app/resources/redux.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.6/app/resources/router.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.6/app/resources/tailwind.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.6/app/utils.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 23:21:50.579836 hades-cli-0.0.6/hades_cli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      152 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      505 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       46 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 23:21:50.000000 hades-cli-0.0.6/hades_cli.egg-info/top_level.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 23:21:50.580297 hades-cli-0.0.6/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      529 2023-05-25 23:21:38.000000 hades-cli-0.0.6/setup.py
```

### Comparing `hades-cli-0.0.5.2/app/application.py` & `hades-cli-0.0.6/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyfiglet
 
 pyfiglet.print_figlet("Hades Toolkit")
 
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
 
 @click.group()
-@click.version_option("0.0.5.3")
+@click.version_option("0.0.6")
 def cli():
     """The main entry point of the application"""
     pass
 
 
 @cli.group()
 def generate():
```

### Comparing `hades-cli-0.0.5.2/app/handlers/generate/backend.py` & `hades-cli-0.0.6/app/handlers/generate/backend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/app/handlers/generate/frontend.py` & `hades-cli-0.0.6/app/handlers/generate/frontend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/app/resources/chakra.py` & `hades-cli-0.0.6/app/resources/chakra.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/app/resources/redux.py` & `hades-cli-0.0.6/app/resources/redux.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/app/resources/router.py` & `hades-cli-0.0.6/app/resources/router.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/app/resources/tailwind.py` & `hades-cli-0.0.6/app/resources/tailwind.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/hades_cli.egg-info/requires.txt` & `hades-cli-0.0.6/hades_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.5.2/setup.py` & `hades-cli-0.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read()
 
 
 setup(
     name="hades-cli",
-    version="0.0.5.2",
+    version="0.0.6",
     packages=find_packages(),
     author="Wilson Mendoza",
     author_email="mreyeswilson@gmail.com",
     description="A CLI for generating projects",
     py_modules=["app"],
     include_dirs=["app"],
     install_requires=[requirements],
```


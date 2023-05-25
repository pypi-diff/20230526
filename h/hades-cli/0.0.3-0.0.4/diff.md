# Comparing `tmp/hades-cli-0.0.3.tar.gz` & `tmp/hades-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-cli-0.0.3.tar", last modified: Thu May 25 22:53:45 2023, max compression
+gzip compressed data, was "hades-cli-0.0.4.tar", last modified: Thu May 25 22:56:05 2023, max compression
```

## Comparing `hades-cli-0.0.3.tar` & `hades-cli-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.145211 hades-cli-0.0.3/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:53:45.145055 hades-cli-0.0.3/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.140503 hades-cli-0.0.3/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.3/app/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.140900 hades-cli-0.0.3/app/handlers/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.3/app/handlers/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.141636 hades-cli-0.0.3/app/handlers/generate/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.3/app/handlers/generate/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.3/app/handlers/generate/backend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2582 2023-05-25 22:13:57.000000 hades-cli-0.0.3/app/handlers/generate/frontend.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.143350 hades-cli-0.0.3/app/resources/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.3/app/resources/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.3/app/resources/chakra.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.3/app/resources/redux.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.3/app/resources/router.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.3/app/resources/tailwind.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      690 2023-05-25 22:33:50.000000 hades-cli-0.0.3/app/start.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.3/app/utils.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:53:45.144794 hades-cli-0.0.3/hades_cli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 22:53:45.000000 hades-cli-0.0.3/hades_cli.egg-info/top_level.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 22:53:45.145269 hades-cli-0.0.3/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      575 2023-05-25 22:53:42.000000 hades-cli-0.0.3/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.356441 hades-cli-0.0.4/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:56:05.356275 hades-cli-0.0.4/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.351595 hades-cli-0.0.4/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.4/app/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.352113 hades-cli-0.0.4/app/handlers/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.4/app/handlers/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.352799 hades-cli-0.0.4/app/handlers/generate/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.4/app/handlers/generate/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.4/app/handlers/generate/backend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2582 2023-05-25 22:13:57.000000 hades-cli-0.0.4/app/handlers/generate/frontend.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.354609 hades-cli-0.0.4/app/resources/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.4/app/resources/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.4/app/resources/chakra.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.4/app/resources/redux.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.4/app/resources/router.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.4/app/resources/tailwind.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      722 2023-05-25 22:55:56.000000 hades-cli-0.0.4/app/start.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.4/app/utils.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:56:05.355996 hades-cli-0.0.4/hades_cli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 22:56:05.000000 hades-cli-0.0.4/hades_cli.egg-info/top_level.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 22:56:05.356504 hades-cli-0.0.4/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      557 2023-05-25 22:55:59.000000 hades-cli-0.0.4/setup.py
```

### Comparing `hades-cli-0.0.3/app/handlers/generate/backend.py` & `hades-cli-0.0.4/app/handlers/generate/backend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/handlers/generate/frontend.py` & `hades-cli-0.0.4/app/handlers/generate/frontend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/resources/chakra.py` & `hades-cli-0.0.4/app/resources/chakra.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/resources/redux.py` & `hades-cli-0.0.4/app/resources/redux.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/resources/router.py` & `hades-cli-0.0.4/app/resources/router.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/resources/tailwind.py` & `hades-cli-0.0.4/app/resources/tailwind.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/app/start.py` & `hades-cli-0.0.4/app/start.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import click
 from app.handlers.generate.frontend import FrontendGenerator
 from app.handlers.generate.backend import BackendGenerator
 import os
 import pyfiglet
 
-pyfiglet.print_figlet("Hera Toolkit")
+pyfiglet.print_figlet("Hades Toolkit")
 
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
 
 @click.group()
+@click.version_option("0.0.4")
 def main():
     """The main entry point of the application"""
     pass
 
 
 @main.group()
 def generate():
```

### Comparing `hades-cli-0.0.3/hades_cli.egg-info/requires.txt` & `hades-cli-0.0.4/hades_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.3/setup.py` & `hades-cli-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 
 with open("requirements.txt") as f:
     requirements = f.read()
 
 
 setuptools.setup(
     name="hades-cli",
-    version="0.0.3",
+    version="0.0.4",
     author="Wilson Mendoza",
     author_email="mreyeswilson@gmail.com",
     description="A CLI for generating projects",
     url="https://github.com/mreyeswilson/mycli",
     packages=setuptools.find_packages(),
     install_requires=requirements,
-    entry_points={
-        "console_scripts": [
-            "hades = app.start:main",
-        ]
-    },
+    entry_points='''
+        [console_scripts]
+        hades=app.start:main
+    ''',
     include_dirs=["app"],
     py_modules=["app"],
     python_requires=">=3.8"
 )
```


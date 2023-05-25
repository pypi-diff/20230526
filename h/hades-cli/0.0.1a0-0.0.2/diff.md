# Comparing `tmp/hades-cli-0.0.1a0.tar.gz` & `tmp/hades-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-cli-0.0.1a0.tar", last modified: Thu May 25 22:49:30 2023, max compression
+gzip compressed data, was "hades-cli-0.0.2.tar", last modified: Thu May 25 22:50:22 2023, max compression
```

## Comparing `hades-cli-0.0.1a0.tar` & `hades-cli-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.435654 hades-cli-0.0.1a0/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      226 2023-05-25 22:49:30.435477 hades-cli-0.0.1a0/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.431274 hades-cli-0.0.1a0/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.1a0/app/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.431650 hades-cli-0.0.1a0/app/handlers/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.1a0/app/handlers/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.432355 hades-cli-0.0.1a0/app/handlers/generate/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.1a0/app/handlers/generate/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.1a0/app/handlers/generate/backend.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2582 2023-05-25 22:13:57.000000 hades-cli-0.0.1a0/app/handlers/generate/frontend.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.434010 hades-cli-0.0.1a0/app/resources/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.1a0/app/resources/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.1a0/app/resources/chakra.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.1a0/app/resources/redux.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.1a0/app/resources/router.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.1a0/app/resources/tailwind.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      690 2023-05-25 22:33:50.000000 hades-cli-0.0.1a0/app/start.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.1a0/app/utils.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:49:30.435206 hades-cli-0.0.1a0/hades_cli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      226 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 22:49:30.000000 hades-cli-0.0.1a0/hades_cli.egg-info/top_level.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 22:49:30.435731 hades-cli-0.0.1a0/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      557 2023-05-25 22:49:25.000000 hades-cli-0.0.1a0/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.444387 hades-cli-0.0.2/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:50:22.444229 hades-cli-0.0.2/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.439643 hades-cli-0.0.2/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:04.000000 hades-cli-0.0.2/app/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.440079 hades-cli-0.0.2/app/handlers/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 17:01:12.000000 hades-cli-0.0.2/app/handlers/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.440770 hades-cli-0.0.2/app/handlers/generate/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 16:39:27.000000 hades-cli-0.0.2/app/handlers/generate/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3625 2023-05-25 22:23:14.000000 hades-cli-0.0.2/app/handlers/generate/backend.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2582 2023-05-25 22:13:57.000000 hades-cli-0.0.2/app/handlers/generate/frontend.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.442524 hades-cli-0.0.2/app/resources/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:12:35.000000 hades-cli-0.0.2/app/resources/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1070 2023-05-25 22:04:01.000000 hades-cli-0.0.2/app/resources/chakra.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     2375 2023-05-25 22:01:56.000000 hades-cli-0.0.2/app/resources/redux.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     1320 2023-05-25 22:19:18.000000 hades-cli-0.0.2/app/resources/router.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      962 2023-05-25 21:49:31.000000 hades-cli-0.0.2/app/resources/tailwind.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      690 2023-05-25 22:33:50.000000 hades-cli-0.0.2/app/start.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      187 2023-05-25 16:09:20.000000 hades-cli-0.0.2/app/utils.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-25 22:50:22.443977 hades-cli-0.0.2/hades_cli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      224 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      499 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      631 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-25 22:50:22.000000 hades-cli-0.0.2/hades_cli.egg-info/top_level.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-25 22:50:22.444440 hades-cli-0.0.2/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      551 2023-05-25 22:50:20.000000 hades-cli-0.0.2/setup.py
```

### Comparing `hades-cli-0.0.1a0/app/handlers/generate/backend.py` & `hades-cli-0.0.2/app/handlers/generate/backend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/handlers/generate/frontend.py` & `hades-cli-0.0.2/app/handlers/generate/frontend.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/resources/chakra.py` & `hades-cli-0.0.2/app/resources/chakra.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/resources/redux.py` & `hades-cli-0.0.2/app/resources/redux.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/resources/router.py` & `hades-cli-0.0.2/app/resources/router.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/resources/tailwind.py` & `hades-cli-0.0.2/app/resources/tailwind.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/app/start.py` & `hades-cli-0.0.2/app/start.py`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/hades_cli.egg-info/requires.txt` & `hades-cli-0.0.2/hades_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hades-cli-0.0.1a0/setup.py` & `hades-cli-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read()
 
 
 setuptools.setup(
     name="hades-cli",
-    version="0.0.1-alpha",
+    version="0.0.2",
     author="Wilson Mendoza",
     author_email="mreyeswilson@gmail.com",
     description="A CLI for generating projects",
     url="https://github.com/mreyeswilson/mycli",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     entry_points={
```


# Comparing `tmp/webpy-framework-1.0.0.tar.gz` & `tmp/webpy-framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.0.0.tar", last modified: Fri May 26 17:18:34 2023, max compression
+gzip compressed data, was "webpy-framework-1.0.1.tar", last modified: Fri May 26 17:46:07 2023, max compression
```

## Comparing `webpy-framework-1.0.0.tar` & `webpy-framework-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:18:34.696544 webpy-framework-1.0.0/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3054 2023-05-26 17:18:34.695437 webpy-framework-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-05-26 17:11:21.000000 webpy-framework-1.0.0/README.md
--rw-rw-rw-   0        0        0      998 2023-05-26 17:18:17.000000 webpy-framework-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 17:18:34.697556 webpy-framework-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 17:18:34.676174 webpy-framework-1.0.0/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.0.0/webpy/__init__.py
--rw-rw-rw-   0        0        0     6043 2023-05-26 17:11:06.000000 webpy-framework-1.0.0/webpy/__main__.py
--rw-rw-rw-   0        0        0     1722 2023-05-26 17:08:09.000000 webpy-framework-1.0.0/webpy/fs_routes.py
--rw-rw-rw-   0        0        0       50 2023-04-23 19:16:48.000000 webpy-framework-1.0.0/webpy/pysite_semantic_tags.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:18:34.693161 webpy-framework-1.0.0/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     3054 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      142 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 17:18:34.000000 webpy-framework-1.0.0/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 17:46:07.903645 webpy-framework-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6100 2023-05-26 17:46:07.901622 webpy-framework-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4221 2023-05-26 17:45:42.000000 webpy-framework-1.0.1/README.md
+-rw-rw-rw-   0        0        0      998 2023-05-26 17:42:01.000000 webpy-framework-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:46:07.903645 webpy-framework-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 17:46:07.881139 webpy-framework-1.0.1/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.0.1/webpy/__init__.py
+-rw-rw-rw-   0        0        0     6043 2023-05-26 17:11:06.000000 webpy-framework-1.0.1/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1722 2023-05-26 17:08:09.000000 webpy-framework-1.0.1/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0       50 2023-04-23 19:16:48.000000 webpy-framework-1.0.1/webpy/pysite_semantic_tags.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:46:07.899251 webpy-framework-1.0.1/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6100 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      142 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 17:46:07.000000 webpy-framework-1.0.1/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.0.0/LICENSE` & `webpy-framework-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.0/pyproject.toml` & `webpy-framework-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.0.0"
+version = "1.0.1"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
@@ -21,15 +21,15 @@
 	"flask >= 2.2.2",
 	"dill >= 0.3.5.1",
 	"python-minifier >= 2.8.0",
 	"dill >= 0.3.6",
 	"flask-session >= 0.5.0",
 	"flask-sqlalchemy >= 3.0.0",
 	"py-domapi >= 1.0.0",
-	"pyx-pysite >= 1.0.0"
+	"pyx-pysite >= 1.0.1"
 
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
```

### Comparing `webpy-framework-1.0.0/webpy/__init__.py` & `webpy-framework-1.0.1/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.0/webpy/__main__.py` & `webpy-framework-1.0.1/webpy/__main__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.0.0/webpy/fs_routes.py` & `webpy-framework-1.0.1/webpy/fs_routes.py`

 * *Files identical despite different names*


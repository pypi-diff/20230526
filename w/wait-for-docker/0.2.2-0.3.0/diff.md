# Comparing `tmp/wait_for_docker-0.2.2.tar.gz` & `tmp/wait_for_docker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wait_for_docker-0.2.2.tar", max compression
+gzip compressed data, was "wait_for_docker-0.3.0.tar", max compression
```

## Comparing `wait_for_docker-0.2.2.tar` & `wait_for_docker-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      358 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/README.md
--rw-r--r--   0        0        0     1046 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/wait_for_docker/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/wait_for_docker/main.py
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 wait_for_docker-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-05-26 09:32:01.907689 wait_for_docker-0.3.0/README.md
+-rw-r--r--   0        0        0     1092 2023-05-26 09:32:01.907689 wait_for_docker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-26 09:32:01.907689 wait_for_docker-0.3.0/wait_for_docker/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-26 09:32:01.907689 wait_for_docker-0.3.0/wait_for_docker/main.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 wait_for_docker-0.3.0/PKG-INFO
```

### Comparing `wait_for_docker-0.2.2/pyproject.toml` & `wait_for_docker-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wait-for-docker"
-version = "0.2.2"
+version = "0.3.0"
 description = "A simple script to wait for Docker daemon to be active."
 license = "MIT"
 authors = ["Goto Hayato <habita.gh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gh640/wait-for-docker"
 keywords = ["docker"]
 classifiers = [
@@ -13,14 +13,15 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 docker = "^6.0.0"
 yaspin = "^2.0.0"
```

### Comparing `wait_for_docker-0.2.2/wait_for_docker/main.py` & `wait_for_docker-0.3.0/wait_for_docker/main.py`

 * *Files identical despite different names*

### Comparing `wait_for_docker-0.2.2/PKG-INFO` & `wait_for_docker-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wait-for-docker
-Version: 0.2.2
+Version: 0.3.0
 Summary: A simple script to wait for Docker daemon to be active.
 Home-page: https://github.com/gh640/wait-for-docker
 License: MIT
 Keywords: docker
 Author: Goto Hayato
 Author-email: habita.gh@gmail.com
 Requires-Python: >=3.7,<4.0
```


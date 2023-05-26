# Comparing `tmp/wait-for-docker-0.2.1.tar.gz` & `tmp/wait_for_docker-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wait-for-docker-0.2.1.tar", max compression
+gzip compressed data, was "wait_for_docker-0.2.2.tar", max compression
```

## Comparing `wait-for-docker-0.2.1.tar` & `wait_for_docker-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      358 2022-09-02 11:43:22.024711 wait-for-docker-0.2.1/README.md
--rw-r--r--   0        0        0     1046 2022-09-02 11:43:22.024711 wait-for-docker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-02 11:43:22.024711 wait-for-docker-0.2.1/wait_for_docker/__init__.py
--rw-r--r--   0        0        0     1053 2022-09-02 11:43:22.024711 wait-for-docker-0.2.1/wait_for_docker/main.py
--rw-r--r--   0        0        0     1215 2022-09-02 11:43:39.774244 wait-for-docker-0.2.1/setup.py
--rw-r--r--   0        0        0     1298 2022-09-02 11:43:39.774519 wait-for-docker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/README.md
+-rw-r--r--   0        0        0     1046 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/wait_for_docker/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-26 09:22:21.739515 wait_for_docker-0.2.2/wait_for_docker/main.py
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 wait_for_docker-0.2.2/PKG-INFO
```

### Comparing `wait-for-docker-0.2.1/pyproject.toml` & `wait_for_docker-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wait-for-docker"
-version = "0.2.1"
+version = "0.2.2"
 description = "A simple script to wait for Docker daemon to be active."
 license = "MIT"
 authors = ["Goto Hayato <habita.gh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/gh640/wait-for-docker"
 keywords = ["docker"]
 classifiers = [
```

### Comparing `wait-for-docker-0.2.1/wait_for_docker/main.py` & `wait_for_docker-0.2.2/wait_for_docker/main.py`

 * *Files identical despite different names*

### Comparing `wait-for-docker-0.2.1/PKG-INFO` & `wait_for_docker-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: wait-for-docker
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple script to wait for Docker daemon to be active.
 Home-page: https://github.com/gh640/wait-for-docker
 License: MIT
 Keywords: docker
 Author: Goto Hayato
 Author-email: habita.gh@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: yaspin (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/gh640/wait-for-docker
 Description-Content-Type: text/markdown
 
 A simple script `wait-for-docker` to wait for Docker daemon to be active.
```


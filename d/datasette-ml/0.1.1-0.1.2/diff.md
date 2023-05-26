# Comparing `tmp/datasette_ml-0.1.1.tar.gz` & `tmp/datasette_ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette_ml-0.1.1.tar", max compression
+gzip compressed data, was "datasette_ml-0.1.2.tar", max compression
```

## Comparing `datasette_ml-0.1.1.tar` & `datasette_ml-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/LICENSE
--rw-r--r--   0        0        0    10370 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/README.md
--rw-r--r--   0        0        0      632 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/datasette_ml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 15:14:46.825192 datasette_ml-0.1.1/datasette_ml/py.typed
--rw-r--r--   0        0        0     1337 2023-04-20 15:14:46.833192 datasette_ml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    11094 1970-01-01 00:00:00.000000 datasette_ml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 13:31:35.153230 datasette_ml-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10500 2023-05-26 13:31:35.153230 datasette_ml-0.1.2/README.md
+-rw-r--r--   0        0        0      632 2023-05-26 13:31:35.153230 datasette_ml-0.1.2/datasette_ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:31:35.153230 datasette_ml-0.1.2/datasette_ml/py.typed
+-rw-r--r--   0        0        0     1308 2023-05-26 13:31:35.161230 datasette_ml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11224 1970-01-01 00:00:00.000000 datasette_ml-0.1.2/PKG-INFO
```

### Comparing `datasette_ml-0.1.1/LICENSE` & `datasette_ml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette_ml-0.1.1/README.md` & `datasette_ml-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Datasette ML
 
 > Bringing Machine Learning models near your data, not the other way around!
 
 Datasette ML is a [Datasette](https://datasette.io) plugin providing an MLOps
 platform to train, evaluate and make predictions from machine learning models.
 
+All the underlying features are provided by [`sqlite-ml`](https://github.com/rclement/sqlite-ml).
+
 [![PyPI](https://img.shields.io/pypi/v/datasette-ml.svg)](https://pypi.org/project/datasette-ml/)
 [![CI/CD](https://github.com/rclement/datasette-ml/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/datasette-ml/actions/workflows/ci-cd.yml)
 [![Coverage Status](https://img.shields.io/codecov/c/github/rclement/datasette-ml)](https://codecov.io/gh/rclement/datasette-ml)
 [![License](https://img.shields.io/github/license/rclement/datasette-ml)](https://github.com/rclement/datasette-ml/blob/master/LICENSE)
 
 <!-- Try out a live demo at [https://datasette-ml-demo.vercel.app](https://datasette-ml-demo.vercel.app/-/dashboards) -->
 
@@ -293,14 +295,15 @@
 ```
 
 ## Inspiration
 
 All the things on the internet that have been inspiring this project:
 
 - [PostgresML](https://postgresml.org)
+- [MLFlow](https://mlflow.org)
 - [SQLite  Run-Time Loadable Extensions](https://www.sqlite.org/loadext.html)
 - [Alex Garcia's `sqlite-loadable-rs`](https://github.com/asg017/sqlite-loadable-rs)
 - [Alex Garcia's SQLite extensions](https://github.com/asg017)
 - [Alex Garcia, "Making SQLite extensions pip install-able"](https://observablehq.com/@asg017/making-sqlite-extensions-pip-install-able)
 - [Max Halford, "Online gradient descent written in SQL"](https://maxhalford.github.io/blog/ogd-in-sql/)
 - [Ricardo Anderegg, "Extending SQLite with Rust"](https://ricardoanderegg.com/posts/extending-sqlite-with-rust/)
```

### Comparing `datasette_ml-0.1.1/datasette_ml/__init__.py` & `datasette_ml-0.1.2/datasette_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `datasette_ml-0.1.1/pyproject.toml` & `datasette_ml-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [tool.poetry]
 name = "datasette-ml"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Datasette plugin providing an MLOps platform to train, eval and predict machine learning models"
 repository = "https://github.com/rclement/datasette-ml"
 authors = ["Romain Clement"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "datasette_ml"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 datasette = "*"
-sqlite-ml = "==0.1.1"
+sqlite-ml = "==0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.3.0"
-faker = "==18.4.0"
+faker = "==18.9.0"
 flake8 = "==6.0.0"
-importlib-metadata = "==6.5.0"
-mypy = "==1.2.0"
+mypy = "==1.3.0"
 pytest = "==7.3.1"
 pytest-asyncio = "==0.21.0"
-pytest-cov = "==4.0.0"
-sqlite-utils = "==3.30"
+pytest-cov = "==4.1.0"
+sqlite-utils = "==3.32.1"
 
 [tool.poetry.plugins."datasette"]
 "ml" = "datasette_ml"
 
 [tool.mypy]
 show_error_codes = "True"
 pretty = "True"
```

### Comparing `datasette_ml-0.1.1/PKG-INFO` & `datasette_ml-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: datasette-ml
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Datasette plugin providing an MLOps platform to train, eval and predict machine learning models
 Home-page: https://github.com/rclement/datasette-ml
 License: Apache License, Version 2.0
 Author: Romain Clement
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasette
-Requires-Dist: sqlite-ml (==0.1.1)
+Requires-Dist: sqlite-ml (==0.1.2)
 Project-URL: Repository, https://github.com/rclement/datasette-ml
 Description-Content-Type: text/markdown
 
 # Datasette ML
 
 > Bringing Machine Learning models near your data, not the other way around!
 
 Datasette ML is a [Datasette](https://datasette.io) plugin providing an MLOps
 platform to train, evaluate and make predictions from machine learning models.
 
+All the underlying features are provided by [`sqlite-ml`](https://github.com/rclement/sqlite-ml).
+
 [![PyPI](https://img.shields.io/pypi/v/datasette-ml.svg)](https://pypi.org/project/datasette-ml/)
 [![CI/CD](https://github.com/rclement/datasette-ml/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/rclement/datasette-ml/actions/workflows/ci-cd.yml)
 [![Coverage Status](https://img.shields.io/codecov/c/github/rclement/datasette-ml)](https://codecov.io/gh/rclement/datasette-ml)
 [![License](https://img.shields.io/github/license/rclement/datasette-ml)](https://github.com/rclement/datasette-ml/blob/master/LICENSE)
 
 <!-- Try out a live demo at [https://datasette-ml-demo.vercel.app](https://datasette-ml-demo.vercel.app/-/dashboards) -->
 
@@ -311,14 +313,15 @@
 ```
 
 ## Inspiration
 
 All the things on the internet that have been inspiring this project:
 
 - [PostgresML](https://postgresml.org)
+- [MLFlow](https://mlflow.org)
 - [SQLite  Run-Time Loadable Extensions](https://www.sqlite.org/loadext.html)
 - [Alex Garcia's `sqlite-loadable-rs`](https://github.com/asg017/sqlite-loadable-rs)
 - [Alex Garcia's SQLite extensions](https://github.com/asg017)
 - [Alex Garcia, "Making SQLite extensions pip install-able"](https://observablehq.com/@asg017/making-sqlite-extensions-pip-install-able)
 - [Max Halford, "Online gradient descent written in SQL"](https://maxhalford.github.io/blog/ogd-in-sql/)
 - [Ricardo Anderegg, "Extending SQLite with Rust"](https://ricardoanderegg.com/posts/extending-sqlite-with-rust/)
```


# Comparing `tmp/applovin_report-0.1.9.tar.gz` & `tmp/applovin_report-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applovin_report-0.1.9.tar", max compression
+gzip compressed data, was "applovin_report-0.2.0.tar", max compression
```

## Comparing `applovin_report-0.1.9.tar` & `applovin_report-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-24 11:28:36.620550 applovin_report-0.1.9/LICENSE
--rw-r--r--   0        0        0      782 2023-05-24 11:28:36.620550 applovin_report-0.1.9/README.md
--rw-r--r--   0        0        0      129 2023-05-24 11:28:36.620550 applovin_report-0.1.9/applovin_report/__init__.py
--rw-r--r--   0        0        0       19 2023-05-24 11:28:36.620550 applovin_report-0.1.9/applovin_report/app.py
--rw-r--r--   0        0        0     2502 2023-05-24 11:28:36.620550 applovin_report-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-24 11:28:36.620550 applovin_report-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-05-24 11:28:36.620550 applovin_report-0.1.9/tests/test_app.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 applovin_report-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-26 04:51:49.969633 applovin_report-0.2.0/LICENSE
+-rw-r--r--   0        0        0      762 2023-05-26 04:51:49.969633 applovin_report-0.2.0/README.md
+-rw-r--r--   0        0        0       94 2023-05-26 04:51:49.969633 applovin_report-0.2.0/applovin_report/__init__.py
+-rw-r--r--   0        0        0     4773 2023-05-26 04:51:49.969633 applovin_report-0.2.0/applovin_report/revenue_reporting_api.py
+-rw-r--r--   0        0        0     2589 2023-05-26 04:51:49.973633 applovin_report-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-26 04:51:49.973633 applovin_report-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-26 04:51:49.973633 applovin_report-0.2.0/tests/test_app.py
+-rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 applovin_report-0.2.0/PKG-INFO
```

### Comparing `applovin_report-0.1.9/LICENSE` & `applovin_report-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `applovin_report-0.1.9/pyproject.toml` & `applovin_report-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "applovin_report"
-version = "0.1.9"
+version = "0.2.0"
 homepage = "https://github.com/ikamedawn/applovin_report"
 description = "Applovin Report APIs wrapper."
 authors = ["Dawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
@@ -39,23 +39,26 @@
 twine = { version = "^4.0.2", optional = true }
 mkdocs-autorefs = { version = "^0.4.1", optional = true }
 pre-commit = { version = "^3.3.2", optional = true }
 toml = { version = "^0.10.2", optional = true }
 livereload = { version = "^2.6.3", optional = true }
 pyreadline = { version = "^2.1", optional = true }
 mike = { version = "^1.1.2", optional = true }
+requests = { version = "^2.31.0", optional = true }
+pandas = "^2.0.1"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
     "flake8-docstrings",
-    "pytest-cov"
+    "pytest-cov",
+    "requests"
 ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
 
 doc = [
     "mkdocs",
     "mkdocs-include-markdown-plugin",
@@ -73,15 +76,15 @@
 setuptools = "^67.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 88
+line-length = 121
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `applovin_report-0.1.9/PKG-INFO` & `applovin_report-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applovin-report
-Version: 0.1.9
+Version: 0.2.0
 Summary: Applovin Report APIs wrapper.
 Home-page: https://github.com/ikamedawn/applovin_report
 License: MIT
 Author: Dawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,19 +25,21 @@
 Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.4,<5.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=9.1.14,<10.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocstrings-python (>=1.0.0,<2.0.0) ; extra == "doc"
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pip (>=23.1.2,<24.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=3.3.2,<4.0.0) ; extra == "dev"
 Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "test"
+Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "test"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=4.5.1,<5.0.0) ; extra == "dev"
 Requires-Dist: twine (>=4.0.2,<5.0.0) ; extra == "dev"
 Requires-Dist: virtualenv (>=20.23.0,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # applovin-report
@@ -45,13 +47,12 @@
 [![release](https://img.shields.io/pypi/v/applovin_report.svg)](https://pypi.org/project/applovin-report/)
 [![docs](https://img.shields.io/website/https/ikamedawn.github.io/applovin_report/index.html.svg?label=docs&down_message=unavailable&up_message=available)](https://ikamedawn.github.io/applovin_report)
 [![develop](https://github.com/ikamedawn/applovin_report/actions/workflows/dev.yml/badge.svg)](https://github.com/ikamedawn/applovin_report/actions/workflows/dev.yml)
 [![main](https://github.com/ikamedawn/applovin_report/actions/workflows/release.yml/badge.svg)](https://github.com/ikamedawn/applovin_report/actions/workflows/release.yml)
 
 Applovin Report APIs wrapper
 
-* Documentation: <https://ikamedawn.github.io/applovin_report/>
-
 ## Features
 
-* TODO
+* Revenue Reporting API
+* More APIs are coming soon
```


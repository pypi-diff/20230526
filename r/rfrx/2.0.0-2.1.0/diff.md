# Comparing `tmp/rfrx-2.0.0.tar.gz` & `tmp/rfrx-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfrx-2.0.0.tar", max compression
+gzip compressed data, was "rfrx-2.1.0.tar", max compression
```

## Comparing `rfrx-2.0.0.tar` & `rfrx-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-05-26 08:19:07.771155 rfrx-2.0.0/LICENSE
--rw-r--r--   0        0        0     1832 2023-05-26 08:19:07.771155 rfrx-2.0.0/README.md
--rw-r--r--   0        0        0      852 2023-05-26 08:19:07.771155 rfrx-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/__init__.py
--rw-r--r--   0        0        0     2475 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/protronik.py
--rw-r--r--   0        0        0     4542 2023-05-26 08:19:07.771155 rfrx-2.0.0/rfrx/sbus.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 rfrx-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-05-26 11:54:06.325765 rfrx-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1970 2023-05-26 11:54:06.325765 rfrx-2.1.0/README.md
+-rw-r--r--   0        0        0     1003 2023-05-26 11:54:06.325765 rfrx-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-05-26 11:54:06.325765 rfrx-2.1.0/rfrx/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-26 11:54:06.325765 rfrx-2.1.0/rfrx/protronik.py
+-rw-r--r--   0        0        0     4542 2023-05-26 11:54:06.325765 rfrx-2.1.0/rfrx/sbus.py
+-rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 rfrx-2.1.0/PKG-INFO
```

### Comparing `rfrx-2.0.0/LICENSE` & `rfrx-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfrx-2.0.0/README.md` & `rfrx-2.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # rfrx
 
+[![Test](https://github.com/nim65s/rfrx/actions/workflows/test.yml/badge.svg)](https://github.com/nim65s/rfrx/actions/workflows/test.yml)
 [![Release](https://github.com/nim65s/rfrx/actions/workflows/release.yml/badge.svg)](https://github.com/nim65s/rfrx/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/rfrx.svg)](https://pypi.org/project/rfrx)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nim65s/rfrx/main.svg)](https://results.pre-commit.ci/latest/github/nim65s/rfrx/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 Receive RF frames from some remote controllers.
```

### Comparing `rfrx-2.0.0/pyproject.toml` & `rfrx-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,37 +4,42 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 authors = ["Guilhem Saurel <guilhem.saurel@laas.fr>"]
 description = "Receive RF frames from SBUS and Pro-Tronik PTR-6A v2"
-license = "BSD-2-Clauses"
+homepage = "https://github.com/nim65s/rfrx"
+license = "BSD-2-Clause"
 name = "rfrx"
 readme = "README.md"
-version = "2.0.0"
+version = "2.1.0"
 
 [tool.poetry.dependencies]
 pyserial = "^3.5"
 python = "^3.7"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+coverage = "^7.2.6"
 ipython = "^7"
 isort = "^5.11"
 pre-commit = "^2"
 ruff = "^0.0.270"
 
 [tool.poetry.scripts]
 protronik = "rfrx:ProTronikReader"
 sbus = "rfrx:SbusReader"
 
+[tool.poetry.urls]
+changelog = "https://github.com/nim65s/rfrx/blob/main/CHANGELOG.md"
+
 [tool.ruff]
 extend-ignore = ["D203", "D213"]
 extend-select = ["A", "B", "C", "COM", "D", "DJ", "EM", "EXE", "G", "N", "PTH", "RET", "RUF", "UP", "W", "YTT"]
 target-version = "py37"
 
 [tool.tomlsort]
 all = true
```

### Comparing `rfrx-2.0.0/rfrx/protronik.py` & `rfrx-2.1.0/rfrx/protronik.py`

 * *Files identical despite different names*

### Comparing `rfrx-2.0.0/rfrx/sbus.py` & `rfrx-2.1.0/rfrx/sbus.py`

 * *Files identical despite different names*

### Comparing `rfrx-2.0.0/PKG-INFO` & `rfrx-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: rfrx
-Version: 2.0.0
+Version: 2.1.0
 Summary: Receive RF frames from SBUS and Pro-Tronik PTR-6A v2
-License: BSD-2-Clauses
+Home-page: https://github.com/nim65s/rfrx
+License: BSD-2-Clause
 Author: Guilhem Saurel
 Author-email: guilhem.saurel@laas.fr
 Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyserial (>=3.5,<4.0)
+Project-URL: changelog, https://github.com/nim65s/rfrx/blob/main/CHANGELOG.md
 Description-Content-Type: text/markdown
 
 # rfrx
 
+[![Test](https://github.com/nim65s/rfrx/actions/workflows/test.yml/badge.svg)](https://github.com/nim65s/rfrx/actions/workflows/test.yml)
 [![Release](https://github.com/nim65s/rfrx/actions/workflows/release.yml/badge.svg)](https://github.com/nim65s/rfrx/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/rfrx.svg)](https://pypi.org/project/rfrx)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/nim65s/rfrx/main.svg)](https://results.pre-commit.ci/latest/github/nim65s/rfrx/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 Receive RF frames from some remote controllers.
```


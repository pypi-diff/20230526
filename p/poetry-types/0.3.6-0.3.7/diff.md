# Comparing `tmp/poetry_types-0.3.6.tar.gz` & `tmp/poetry_types-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_types-0.3.6.tar", max compression
+gzip compressed data, was "poetry_types-0.3.7.tar", max compression
```

## Comparing `poetry_types-0.3.6.tar` & `poetry_types-0.3.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-04-24 12:57:27.679500 poetry_types-0.3.6/LICENSE
--rw-r--r--   0        0        0     1475 2023-04-24 12:57:27.679500 poetry_types-0.3.6/README.md
--rw-r--r--   0        0        0      145 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/commands/__init__.py
--rw-r--r--   0        0        0      981 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/commands/add_types.py
--rw-r--r--   0        0        0     8414 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/commands/base.py
--rw-r--r--   0        0        0     1076 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/commands/remove_types.py
--rw-r--r--   0        0        0     2750 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/commands/update_types.py
--rw-r--r--   0        0        0      163 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/packages_map.py
--rw-r--r--   0        0        0      544 2023-04-24 12:57:27.679500 poetry_types-0.3.6/poetry_types/poetry_types.py
--rw-r--r--   0        0        0     1129 2023-04-24 12:57:27.679500 poetry_types-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 poetry_types-0.3.6/setup.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 poetry_types-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 20:31:35.621524 poetry_types-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1475 2023-05-26 20:31:35.621524 poetry_types-0.3.7/README.md
+-rw-r--r--   0        0        0      145 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/commands/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/commands/add_types.py
+-rw-r--r--   0        0        0     8414 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/commands/base.py
+-rw-r--r--   0        0        0     1076 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/commands/remove_types.py
+-rw-r--r--   0        0        0     2750 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/commands/update_types.py
+-rw-r--r--   0        0        0      163 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/packages_map.py
+-rw-r--r--   0        0        0      544 2023-05-26 20:31:35.621524 poetry_types-0.3.7/poetry_types/poetry_types.py
+-rw-r--r--   0        0        0     1152 2023-05-26 20:31:35.621524 poetry_types-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 poetry_types-0.3.7/setup.py
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 poetry_types-0.3.7/PKG-INFO
```

### Comparing `poetry_types-0.3.6/LICENSE` & `poetry_types-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/README.md` & `poetry_types-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/poetry_types/commands/add_types.py` & `poetry_types-0.3.7/poetry_types/commands/add_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/poetry_types/commands/base.py` & `poetry_types-0.3.7/poetry_types/commands/base.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/poetry_types/commands/remove_types.py` & `poetry_types-0.3.7/poetry_types/commands/remove_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/poetry_types/commands/update_types.py` & `poetry_types-0.3.7/poetry_types/commands/update_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/poetry_types/poetry_types.py` & `poetry_types-0.3.7/poetry_types/poetry_types.py`

 * *Files identical despite different names*

### Comparing `poetry_types-0.3.6/pyproject.toml` & `poetry_types-0.3.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "poetry-types"
-version = "0.3.6"
+version = "0.3.7"
 description = "A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command."
 authors = ["Jan Vollmer <jan@vllmr.dev>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/jvllmr/poetry-types"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Natural Language :: English",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 poetry = "^1.2"
+poetry-core = "<1.6.0"
 tomlkit = "^0.11.4"
 packaging = ">=21.3,<24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 tox = "^3.0 ||^4.0"
 black = "^22.6.0 || ^23.0.0"
```

### Comparing `poetry_types-0.3.6/setup.py` & `poetry_types-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 packages = \
 ['poetry_types', 'poetry_types.commands']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['packaging>=21.3,<24.0', 'poetry>=1.2,<2.0', 'tomlkit>=0.11.4,<0.12.0']
+['packaging>=21.3,<24.0',
+ 'poetry-core<1.6.0',
+ 'poetry>=1.2,<2.0',
+ 'tomlkit>=0.11.4,<0.12.0']
 
 entry_points = \
 {'poetry.application.plugin': ['poetry-types = '
                                'poetry_types.poetry_types:PoetryTypes']}
 
 setup_kwargs = {
     'name': 'poetry-types',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': 'A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command.',
     'long_description': '# poetry-types\n\n[![PyPI version](https://badge.fury.io/py/poetry-types.svg)](https://badge.fury.io/py/poetry-types)\n[![GitHub license](https://img.shields.io/github/license/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/blob/master/LICENSE)\n[![GitHub issues](https://img.shields.io/github/issues/jvllmr/poetry-types)](https://github.com/jvllmr/poetry-types/issues)\n![PyPI - Downloads](https://img.shields.io/pypi/dd/poetry-types)\n![Tests](https://github.com/jvllmr/poetry-types/actions/workflows/main.yml/badge.svg)\n\n## Description\n\nThis is a plugin to poetry for the upcoming poetry 1.2 plugin feature.\nIt installs/removes/updates typing stubs via following commands:\n\n- `poetry types add <package names>`\n- `poetry types remove <package names>`\n- `poetry types update <package names>`\n\n## Usage examples\n\n- `poetry types add SQLAlchemy` adds `types-SQLAlchemy` to your project\n- `poetry types update` adds `types-SQLAlchemy` if `SQLAlchemy` is present, but not `types-SQLAlchemy`\n- `poetry types update` removes `types-SQLAlchemy` if `types-SQLAlchemy` is present, but not `SQLAlchemy`\n\n## Installation\n\nRun `poetry self add poetry-types` for global install or run `poetry add -D poetry-types` to use this plugin with your project.\n\n## Usage with pre-commit\n\n```yaml\n- repo: https://github.com/jvllmr/poetry-types\n  rev: v0.3.5\n  hooks:\n    - id: poetry-types\n```\n\n### poetry-types has to be skipped with pre-commit.ci\n\n```yaml\nci:\n  skip: [poetry-types]\n```\n',
     'author': 'Jan Vollmer',
     'author_email': 'jan@vllmr.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jvllmr/poetry-types',
```

### Comparing `poetry_types-0.3.6/PKG-INFO` & `poetry_types-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-types
-Version: 0.3.6
+Version: 0.3.7
 Summary: A poetry plugin that adds/removes type stubs as dependencies like the mypy --install-types command.
 Home-page: https://github.com/jvllmr/poetry-types
 License: MIT
 Author: Jan Vollmer
 Author-email: jan@vllmr.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: packaging (>=21.3,<24.0)
 Requires-Dist: poetry (>=1.2,<2.0)
+Requires-Dist: poetry-core (<1.6.0)
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
 Project-URL: Repository, https://github.com/jvllmr/poetry-types
 Description-Content-Type: text/markdown
 
 # poetry-types
 
 [![PyPI version](https://badge.fury.io/py/poetry-types.svg)](https://badge.fury.io/py/poetry-types)
```


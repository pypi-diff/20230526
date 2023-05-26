# Comparing `tmp/clouding_server_manager-0.1.0.tar.gz` & `tmp/clouding_server_manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouding_server_manager-0.1.0.tar", max compression
+gzip compressed data, was "clouding_server_manager-1.0.0.tar", max compression
```

## Comparing `clouding_server_manager-0.1.0.tar` & `clouding_server_manager-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-0.1.0/LICENSE
--rw-r--r--   0        0        0     5850 2023-05-26 09:43:46.985516 clouding_server_manager-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-0.1.0/clouding_server_manager/__init__.py
--rw-r--r--   0        0        0      530 2023-05-26 09:45:27.506795 clouding_server_manager-0.1.0/clouding_server_manager/__main__.py
--rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-0.1.0/clouding_server_manager/commands.py
--rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-0.1.0/clouding_server_manager/constants.py
--rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-0.1.0/clouding_server_manager/helpers.py
--rw-r--r--   0        0        0      775 2023-05-26 09:30:00.012190 clouding_server_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6454 1970-01-01 00:00:00.000000 clouding_server_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5972 2023-05-26 10:21:40.385178 clouding_server_manager-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.0/clouding_server_manager/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.0/clouding_server_manager/__main__.py
+-rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.0/clouding_server_manager/commands.py
+-rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.0/clouding_server_manager/constants.py
+-rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.0/clouding_server_manager/helpers.py
+-rw-r--r--   0        0        0      851 2023-05-26 10:21:31.451727 clouding_server_manager-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.0/PKG-INFO
```

### Comparing `clouding_server_manager-0.1.0/LICENSE` & `clouding_server_manager-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-0.1.0/README.md` & `clouding_server_manager-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-0.1.0-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
@@ -74,14 +74,18 @@
     ```
     This will activate the virtual environment so that you can run the script.
 7. Enter your Clouding API key in the `.env` file. Check out `.env.sample` for an example. You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
 8. Run the script:
     ```bash
     python -m clouding_server_manager --help
     ```
+    or
+    ```bash
+    poetry run clouding-sm --help
+    ```
     This will display the help message and show you how to use the script.
 
 ## Installation with pip
 This is an alternative installation method that uses pip instead of Poetry. It might not work as expected, so it is recommended to use the Poetry installation method instead. To set up the project, follow these steps:
 1. Clone the repository:
     ```bash
     git clone https://github.com/dmarts05/clouding-server-manager
@@ -96,14 +100,18 @@
     ```
     You might need [pyenv](https://github.com/pyenv/pyenv) to install the Python version specified in the `requirements.txt` file.
 4. Enter your Clouding API key in the `.env` file. Check out `.env.sample` for an example. You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
 5. Run the script:
     ```bash
     python -m clouding_server_manager --help
     ```
+    or
+    ```bash
+    poetry run clouding-sm --help
+    ```
     This will display the help message and show you how to use the script.
 
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
```

### Comparing `clouding_server_manager-0.1.0/clouding_server_manager/commands.py` & `clouding_server_manager-1.0.0/clouding_server_manager/commands.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-0.1.0/clouding_server_manager/constants.py` & `clouding_server_manager-1.0.0/clouding_server_manager/constants.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-0.1.0/clouding_server_manager/helpers.py` & `clouding_server_manager-1.0.0/clouding_server_manager/helpers.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-0.1.0/pyproject.toml` & `clouding_server_manager-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "clouding-server-manager"
-version = "0.1.0"
+version = "1.0.0"
 description = "A Python project to easily manage Clouding servers from the command line."
 authors = ["dmarts05 <dmarts05@estudiantes.unileon.es>"]
 readme = "README.md"
 packages = [{include = "clouding_server_manager"}]
 
+[tool.poetry.scripts]
+clouding-sm = "clouding_server_manager.__main__:main"
+
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
 click = "^8.1.3"
 
-
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 types-requests = "^2.31.0.0"
```

### Comparing `clouding_server_manager-0.1.0/PKG-INFO` & `clouding_server_manager-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: clouding-server-manager
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python project to easily manage Clouding servers from the command line.
 Author: dmarts05
 Author-email: dmarts05@estudiantes.unileon.es
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-0.1.0-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
@@ -90,14 +90,18 @@
     ```
     This will activate the virtual environment so that you can run the script.
 7. Enter your Clouding API key in the `.env` file. Check out `.env.sample` for an example. You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
 8. Run the script:
     ```bash
     python -m clouding_server_manager --help
     ```
+    or
+    ```bash
+    poetry run clouding-sm --help
+    ```
     This will display the help message and show you how to use the script.
 
 ## Installation with pip
 This is an alternative installation method that uses pip instead of Poetry. It might not work as expected, so it is recommended to use the Poetry installation method instead. To set up the project, follow these steps:
 1. Clone the repository:
     ```bash
     git clone https://github.com/dmarts05/clouding-server-manager
@@ -112,14 +116,18 @@
     ```
     You might need [pyenv](https://github.com/pyenv/pyenv) to install the Python version specified in the `requirements.txt` file.
 4. Enter your Clouding API key in the `.env` file. Check out `.env.sample` for an example. You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
 5. Run the script:
     ```bash
     python -m clouding_server_manager --help
     ```
+    or
+    ```bash
+    poetry run clouding-sm --help
+    ```
     This will display the help message and show you how to use the script.
 
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
```


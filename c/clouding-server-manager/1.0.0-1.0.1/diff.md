# Comparing `tmp/clouding_server_manager-1.0.0.tar.gz` & `tmp/clouding_server_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouding_server_manager-1.0.0.tar", max compression
+gzip compressed data, was "clouding_server_manager-1.0.1.tar", max compression
```

## Comparing `clouding_server_manager-1.0.0.tar` & `clouding_server_manager-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.0/LICENSE
--rw-r--r--   0        0        0     5972 2023-05-26 10:21:40.385178 clouding_server_manager-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.0/clouding_server_manager/__init__.py
--rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.0/clouding_server_manager/__main__.py
--rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.0/clouding_server_manager/commands.py
--rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.0/clouding_server_manager/constants.py
--rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.0/clouding_server_manager/helpers.py
--rw-r--r--   0        0        0      851 2023-05-26 10:21:31.451727 clouding_server_manager-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6956 2023-05-26 10:29:34.188075 clouding_server_manager-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.1/clouding_server_manager/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.1/clouding_server_manager/__main__.py
+-rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.1/clouding_server_manager/commands.py
+-rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.1/clouding_server_manager/constants.py
+-rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.1/clouding_server_manager/helpers.py
+-rw-r--r--   0        0        0      851 2023-05-26 10:29:38.304795 clouding_server_manager-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.1/PKG-INFO
```

### Comparing `clouding_server_manager-1.0.0/LICENSE` & `clouding_server_manager-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.0/README.md` & `clouding_server_manager-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.1-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
 * [Examples](#examples)
 * [Installation with Poetry (recommended)](#installation-with-poetry-recommended)
 * [Installation with pip](#installation-with-pip)
+* [Installation as a PyPI package](#installation-as-a-pypi-package)
 * [Development Setup](#development-setup)
 * [Contributing](#contributing)
 * [License](#license)
 
 ## Features
 * Simple and easy to use command line interface.
 * List all the information about your Clouding servers and filter their fields so that you can see only the information you want.
@@ -106,14 +107,31 @@
     ```
     or
     ```bash
     poetry run clouding-sm --help
     ```
     This will display the help message and show you how to use the script.
 
+## Installation as a PyPI package
+This is an alternative installation method that uses pip to install the package from PyPI. It might not work as expected, so it is recommended to use the Poetry installation method instead. To set up the project, follow these steps:
+1. Install the package using pip:
+    ```bash
+    pip install clouding-server-manager
+    ```
+2. Configure the environment variable with `export` or by adding them to your `.bashrc` or `.zshrc` file:
+    ```bash
+    export CLOUDING_API_KEY="YOUR API KEY"
+    ```
+    You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
+2. Run the script:
+    ```bash
+    clouding-sm --help
+    ```
+    This will display the help message and show you how to use the script.
+
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
     ```
 2. Format the code:
```

### Comparing `clouding_server_manager-1.0.0/clouding_server_manager/__main__.py` & `clouding_server_manager-1.0.1/clouding_server_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.0/clouding_server_manager/commands.py` & `clouding_server_manager-1.0.1/clouding_server_manager/commands.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.0/clouding_server_manager/constants.py` & `clouding_server_manager-1.0.1/clouding_server_manager/constants.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.0/clouding_server_manager/helpers.py` & `clouding_server_manager-1.0.1/clouding_server_manager/helpers.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.0/pyproject.toml` & `clouding_server_manager-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clouding-server-manager"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python project to easily manage Clouding servers from the command line."
 authors = ["dmarts05 <dmarts05@estudiantes.unileon.es>"]
 readme = "README.md"
 packages = [{include = "clouding_server_manager"}]
 
 [tool.poetry.scripts]
 clouding-sm = "clouding_server_manager.__main__:main"
```

### Comparing `clouding_server_manager-1.0.0/PKG-INFO` & `clouding_server_manager-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: clouding-server-manager
-Version: 1.0.0
+Version: 1.0.1
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
-![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.1-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
 * [Examples](#examples)
 * [Installation with Poetry (recommended)](#installation-with-poetry-recommended)
 * [Installation with pip](#installation-with-pip)
+* [Installation as a PyPI package](#installation-as-a-pypi-package)
 * [Development Setup](#development-setup)
 * [Contributing](#contributing)
 * [License](#license)
 
 ## Features
 * Simple and easy to use command line interface.
 * List all the information about your Clouding servers and filter their fields so that you can see only the information you want.
@@ -122,14 +123,31 @@
     ```
     or
     ```bash
     poetry run clouding-sm --help
     ```
     This will display the help message and show you how to use the script.
 
+## Installation as a PyPI package
+This is an alternative installation method that uses pip to install the package from PyPI. It might not work as expected, so it is recommended to use the Poetry installation method instead. To set up the project, follow these steps:
+1. Install the package using pip:
+    ```bash
+    pip install clouding-server-manager
+    ```
+2. Configure the environment variable with `export` or by adding them to your `.bashrc` or `.zshrc` file:
+    ```bash
+    export CLOUDING_API_KEY="YOUR API KEY"
+    ```
+    You can find your Clouding API key in the API section of your Clouding account (as of now you need access to the beta version of the Clouding API). As an alternative, you can use --api-key or -k to specify your API key when running the script.
+2. Run the script:
+    ```bash
+    clouding-sm --help
+    ```
+    This will display the help message and show you how to use the script.
+
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
     ```
 2. Format the code:
```


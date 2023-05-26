# Comparing `tmp/dataverse_api-0.1.3.tar.gz` & `tmp/dataverse_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-0.1.3.tar", max compression
+gzip compressed data, was "dataverse_api-0.2.0.tar", max compression
```

## Comparing `dataverse_api-0.1.3.tar` & `dataverse_api-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       61 2023-05-12 18:28:06.104392 dataverse_api-0.1.3/dataverse_api/__init__.py
--rw-r--r--   0        0        0    17764 2023-05-12 18:40:36.006430 dataverse_api-0.1.3/dataverse_api/dataverse.py
--rw-r--r--   0        0        0     2428 2023-05-12 18:33:21.684230 dataverse_api-0.1.3/dataverse_api/schema.py
--rw-r--r--   0        0        0     2180 2023-05-12 18:01:04.757130 dataverse_api-0.1.3/dataverse_api/utils.py
--rw-r--r--   0        0        0     1093 2023-05-12 18:09:25.896155 dataverse_api-0.1.3/LICENSE
--rw-r--r--   0        0        0      756 2023-05-12 19:29:24.929473 dataverse_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2941 2023-05-12 19:21:52.771293 dataverse_api-0.1.3/README.md
--rw-r--r--   0        0        0     3556 1970-01-01 00:00:00.000000 dataverse_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-13 11:36:09.341892 dataverse_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3667 2023-05-26 19:09:30.479518 dataverse_api-0.2.0/README.md
+-rw-r--r--   0        0        0       60 2023-05-13 11:36:09.342484 dataverse_api-0.2.0/dataverse_api/__init__.py
+-rw-r--r--   0        0        0    25640 2023-05-26 19:09:53.063694 dataverse_api-0.2.0/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0     6283 2023-05-26 19:09:53.063896 dataverse_api-0.2.0/dataverse_api/utils.py
+-rw-r--r--   0        0        0      749 2023-05-26 19:14:31.431371 dataverse_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4365 1970-01-01 00:00:00.000000 dataverse_api-0.2.0/PKG-INFO
```

### Comparing `dataverse_api-0.1.3/LICENSE` & `dataverse_api-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Marcus Risanger
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Marcus Risanger
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dataverse_api-0.1.3/PKG-INFO` & `dataverse_api-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,21 @@
-Metadata-Version: 2.1
-Name: dataverse-api
-Version: 0.1.3
-Summary: Abstraction layer for interacting with Microsoft Dataverse in Python. Supports batch operations.
-Author: Marcus Risanger
-Author-email: 69350948+MarcusRisanger@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: msal (>=1.22.0,<2.0.0)
-Requires-Dist: msal-requests-auth (>=0.7.0,<0.8.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
-Description-Content-Type: text/markdown
+# `dataverse-api`
 
-
-`dataverse-api`
-================================
 [![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
 [![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 The `dataverse-api` package is an abstraction layer developed for allowing simple interaction with Microsoft Dataverse Web API.
 
-Overview
-================================
+# Overview
+
 The main goal of this project was to allow for simple upserts and inserts of data into Dataverse tables using simple and ubiquitous data structures, with use of batch requests to avoid frequent hits on the REST API. It is based on Python 3.9 to be compatible with current Python runtimes in Azure Functions.
 
+### Getting started
+
 Usage is fairly simple and assumes that a valid app registration for writing to Dataverse exists:
 
 ```
 import os
 from dataverse_api import DataverseClient
 
 app_id = os.environ["app_id"]
@@ -43,42 +27,49 @@
 
 client = DataverseClient(
     app_id=app_id,
     client_secret=client_secret,
     authority_url=authority_url,
     scopes=scopes,
     dynamics_url=url,
-    validate=True,
 )
-table = client.entity("xyz_my_table")
+
+table = client.entity(logical_name="xyz_my_table")
 
 data = [
     {"xyz_my_table_key": "Foo", "xyz_my_table_col": 1010},
     {"xyz_my_table_key": "Bar", "xyz_my_table_col": 1020},
 ]
 
 table.upsert(data)
 ```
 
+### Optional validation
+
+Instantiating a new `DataverseEntity` with `logical_name` triggers additional validation to take place, based on the EntityMetadata API endpoints. Upon instantiation, calls will be made to the API to fetch the `EntitySetName` used in API
+queries, together with column names and alternate key Attribute combinations.
+
+When validation is enabled, the client both checks that columns referred to in the data are valid according to the schema, and will automatically pick a suitable row ID for batch operations. While this is nice, it is mostly thought of as a debugging tool to develop scripts, since it carries the overhead of retrieving the information from the API. It is recommended to instantiate Entities by using the `entity_set_name` argument and specifying key columns in your data when preparing scripts for production.
+
 ## Development environment
 
 We use [poetry](https://python-poetry.org) to manage dependencies and to administrate virtual environments. To develop
 `dataverse-api`, follow the following steps to set up your local environment:
 
- 1. [Install poetry](https://python-poetry.org/docs/#installation) if you haven't already.
+1.  [Install poetry](https://python-poetry.org/docs/#installation) if you haven't already.
 
- 2. Clone repository:
+2.  Clone repository:
     ```
     $ git clone git@github.com:MarcusRisanger/dataverse-api.git
     ```
- 3. Move into the newly created local repository:
+3.  Move into the newly created local repository:
     ```
     $ cd dataverse-api
     ```
- 4. Create virtual environment and install dependencies:
+4.  Create virtual environment and install dependencies:
     ```
     $ poetry install
     ```
 
 ### Code requirements
 
 All code must pass [black](https://github.com/ambv/black) and [isort](https://github.com/timothycrosley/isort) style
@@ -90,12 +81,12 @@
 
 Each public method, class and module should have docstrings. Docstrings are written in the [Google
 style](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings).
 
 ### Testing
 
 To produce Coverage tests, run the following commands
+
 ```
 $ poetry run coverage run -m pytest
 $ poetry run coverage xml
 ```
-
```


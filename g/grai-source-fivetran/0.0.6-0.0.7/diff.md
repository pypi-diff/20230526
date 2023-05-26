# Comparing `tmp/grai_source_fivetran-0.0.6.tar.gz` & `tmp/grai_source_fivetran-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.6.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.7.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.6.tar` & `grai_source_fivetran-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,14 @@
--rw-r--r--   0        0        0      139 2023-05-19 10:56:28.943431 grai_source_fivetran-0.0.6/README.md
--rw-r--r--   0        0        0     1073 2023-05-19 10:56:36.009424 grai_source_fivetran-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      441 2023-05-19 09:16:42.851003 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/grai_source_fivetran.iml
--rw-r--r--   0        0        0     3706 2023-05-19 09:16:42.842120 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-05-19 09:16:42.863792 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      200 2023-05-19 09:16:42.860192 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/misc.xml
--rw-r--r--   0        0        0      292 2023-05-19 09:16:42.855186 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/modules.xml
--rw-r--r--   0        0        0     1676 2023-05-19 09:16:42.856457 grai_source_fivetran-0.0.6/src/grai_source_fivetran/.idea/workspace.xml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.6/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6644 2023-05-19 10:56:28.944032 grai_source_fivetran-0.0.6/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.6/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0      208 2023-04-10 14:43:24.094047 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0   304385 2023-04-10 14:43:24.142083 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/__pycache__/api_models.cpython-310.pyc
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    13390 2023-05-19 10:56:28.944303 grai_source_fivetran-0.0.6/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.6/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.6/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.6/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.6/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.6/setup.py
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-25 16:20:32.597515 grai_source_fivetran-0.0.7/README.md
+-rw-r--r--   0        0        0     1020 2023-05-26 19:11:57.309355 grai_source_fivetran-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.7/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     6644 2023-05-19 11:07:12.931545 grai_source_fivetran-0.0.7/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2111 2023-05-26 18:51:17.053006 grai_source_fivetran-0.0.7/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    13390 2023-05-26 18:52:58.771794 grai_source_fivetran-0.0.7/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.7/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.7/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.7/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.7/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.7/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.6/pyproject.toml` & `grai_source_fivetran-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
+
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
 grai-client = "^0.2.0"
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
-grai-schemas = "^0.1.10"
+grai-schemas = "^0.1.12"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 mypy = "^0.971"
 isort = "^5.12.0"
 pytest = "^7.2.0"
 pre-commit = "^3.0.4"
 types-requests = "^2.28.11.7"
-fastapi = "^0.88.0"
-fastapi-code-generator = "^0.3.6"
 faker = "^17.0.0"
 
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_source_fivetran"
```

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.6/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.7/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*


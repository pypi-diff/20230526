# Comparing `tmp/vanty-0.0.1.tar.gz` & `tmp/vanty-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanty-0.0.1.tar", max compression
+gzip compressed data, was "vanty-0.0.2.tar", max compression
```

## Comparing `vanty-0.0.1.tar` & `vanty-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.1/LICENSE
--rw-r--r--   0        0        0     1246 2023-05-26 17:56:09.814324 vanty-0.0.1/README.md
--rw-r--r--   0        0        0      619 2023-05-26 17:56:09.842967 vanty-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.1/vanty/__init__.py
--rw-r--r--   0        0        0       59 2022-11-14 22:54:03.784314 vanty-0.0.1/vanty/__main__.py
--rw-r--r--   0        0        0     2484 2023-05-26 16:00:32.565602 vanty-0.0.1/vanty/_client.py
--rw-r--r--   0        0        0     1223 2023-05-26 17:53:23.000293 vanty-0.0.1/vanty/auth.py
--rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.1/vanty/cli.py
--rw-r--r--   0        0        0     3652 2023-05-26 16:18:23.487417 vanty-0.0.1/vanty/config.py
--rw-r--r--   0        0        0     3464 2023-05-26 16:00:32.576812 vanty-0.0.1/vanty/dev.py
--rw-r--r--   0        0        0     1842 2023-05-26 16:00:32.579158 vanty-0.0.1/vanty/ops.py
--rw-r--r--   0        0        0      811 2023-05-26 17:53:22.962011 vanty-0.0.1/vanty/project.py
--rw-r--r--   0        0        0      948 2023-05-26 16:00:32.166597 vanty-0.0.1/vanty/schema.py
--rw-r--r--   0        0        0        0 2023-05-26 11:42:28.765792 vanty-0.0.1/vanty/tests/__init__.py
--rw-r--r--   0        0        0      802 2023-05-26 17:53:22.957434 vanty-0.0.1/vanty/tests/test_auth.py
--rw-r--r--   0        0        0      717 2023-05-26 17:53:22.640344 vanty-0.0.1/vanty/tests/test_client.py
--rw-r--r--   0        0        0        0 2023-05-26 11:54:18.738508 vanty-0.0.1/vanty/tests/test_config.py
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 vanty-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 15:47:21.194628 vanty-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1246 2023-05-26 17:56:09.814324 vanty-0.0.2/README.md
+-rw-r--r--   0        0        0      666 2023-05-26 17:58:31.045125 vanty-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 16:33:35.338956 vanty-0.0.2/vanty/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-14 22:54:03.784314 vanty-0.0.2/vanty/__main__.py
+-rw-r--r--   0        0        0     2484 2023-05-26 16:00:32.565602 vanty-0.0.2/vanty/_client.py
+-rw-r--r--   0        0        0     1223 2023-05-26 17:53:23.000293 vanty-0.0.2/vanty/auth.py
+-rw-r--r--   0        0        0      506 2023-05-26 17:53:23.021988 vanty-0.0.2/vanty/cli.py
+-rw-r--r--   0        0        0     3652 2023-05-26 16:18:23.487417 vanty-0.0.2/vanty/config.py
+-rw-r--r--   0        0        0     3464 2023-05-26 16:00:32.576812 vanty-0.0.2/vanty/dev.py
+-rw-r--r--   0        0        0     1842 2023-05-26 16:00:32.579158 vanty-0.0.2/vanty/ops.py
+-rw-r--r--   0        0        0      811 2023-05-26 17:53:22.962011 vanty-0.0.2/vanty/project.py
+-rw-r--r--   0        0        0      948 2023-05-26 16:00:32.166597 vanty-0.0.2/vanty/schema.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:42:28.765792 vanty-0.0.2/vanty/tests/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-26 17:53:22.957434 vanty-0.0.2/vanty/tests/test_auth.py
+-rw-r--r--   0        0        0      717 2023-05-26 17:53:22.640344 vanty-0.0.2/vanty/tests/test_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:54:18.738508 vanty-0.0.2/vanty/tests/test_config.py
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 vanty-0.0.2/PKG-INFO
```

### Comparing `vanty-0.0.1/LICENSE` & `vanty-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/README.md` & `vanty-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/pyproject.toml` & `vanty-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vanty"
-version = "0.0.1"
+version = "0.0.2"
 description = "CLI for installing and managing projects & applications from advantch.com"
 authors = ["Themba <themba@advantch.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [
     {include = "vanty"}
 ]
@@ -15,14 +15,17 @@
 honcho = "^1.1.0"
 django-environ = "^0.10.0"
 sh = "^2.0.4"
 toml = "^0.10.2"
 httpx = "^0.24.1"
 pydantic = "^1.10.8"
 
+[tool.poetry.scripts]
+vanty = "vanty.cli:app"
+
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 respx = "^0.20.1"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `vanty-0.0.1/vanty/_client.py` & `vanty-0.0.2/vanty/_client.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/auth.py` & `vanty-0.0.2/vanty/auth.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/config.py` & `vanty-0.0.2/vanty/config.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/dev.py` & `vanty-0.0.2/vanty/dev.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/ops.py` & `vanty-0.0.2/vanty/ops.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/project.py` & `vanty-0.0.2/vanty/project.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/schema.py` & `vanty-0.0.2/vanty/schema.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/tests/test_auth.py` & `vanty-0.0.2/vanty/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/vanty/tests/test_client.py` & `vanty-0.0.2/vanty/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vanty-0.0.1/PKG-INFO` & `vanty-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanty
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI for installing and managing projects & applications from advantch.com
 License: Apache
 Author: Themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


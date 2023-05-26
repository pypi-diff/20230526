# Comparing `tmp/logrich-0.7.0.tar.gz` & `tmp/logrich-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-0.7.0.tar", max compression
+gzip compressed data, was "logrich-0.7.1.tar", max compression
```

## Comparing `logrich-0.7.0.tar` & `logrich-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1184 2023-03-07 14:21:55.270867 logrich-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-03-07 14:21:55.270867 logrich-0.7.0/logrich/__init__.py
--rw-r--r--   0        0        0     1186 2023-03-07 14:21:55.270867 logrich-0.7.0/logrich/config.py
--rw-r--r--   0        0        0     2924 2023-03-07 14:21:55.270867 logrich-0.7.0/logrich/logger_.py
--rw-r--r--   0        0        0     4819 2023-03-07 14:21:55.274867 logrich-0.7.0/logrich/logger_assets.py
--rw-r--r--   0        0        0      904 2023-03-07 14:33:51.103056 logrich-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-0.7.1/README.md
+-rw-r--r--   0        0        0       29 2023-05-26 11:23:23.720683 logrich-0.7.1/logrich/__init__.py
+-rw-r--r--   0        0        0     2924 2023-03-25 11:37:39.181788 logrich-0.7.1/logrich/app.py
+-rw-r--r--   0        0        0     1192 2023-05-26 11:10:29.839735 logrich-0.7.1/logrich/config.py
+-rw-r--r--   0        0        0     4819 2023-05-26 11:25:52.964148 logrich-0.7.1/logrich/logger_assets.py
+-rw-r--r--   0        0        0      904 2023-05-26 11:29:53.615301 logrich-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 logrich-0.7.1/PKG-INFO
```

### Comparing `logrich-0.7.0/README.md` & `logrich-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `logrich-0.7.0/logrich/config.py` & `logrich-0.7.1/logrich/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Settings(BaseSettings):
     """
     Server config settings
     """
 
-    LOG_LEVEL: int = 5
+    LOG_LEVEL: int | str = 5
     # макисмальная длина текста чтобы разместить его на одной линии с уровнем лога
     MAX_WITH_LOG_OF_OBJ: int = 120
     # https://loguru.readthedocs.io/en/stable/resources/recipes.html#adapting-colors-and-format-of-logged-messages-dynamically
     # https://docs-python.ru/standart-library/modul-string-python/klass-template-modulja-string/
     # https://loguru.readthedocs.io/en/stable/api/logger.html#color
     # https://rich.readthedocs.io/en/stable/style.html
```

### Comparing `logrich-0.7.0/logrich/logger_.py` & `logrich-0.7.1/logrich/app.py`

 * *Files identical despite different names*

### Comparing `logrich-0.7.0/logrich/logger_assets.py` & `logrich-0.7.1/logrich/logger_assets.py`

 * *Files identical despite different names*

### Comparing `logrich-0.7.0/pyproject.toml` & `logrich-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "0.7.0"
+version = "0.7.1"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
```

### Comparing `logrich-0.7.0/PKG-INFO` & `logrich-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 0.7.0
+Version: 0.7.1
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```


# Comparing `tmp/sqlite_ml-0.1.1.tar.gz` & `tmp/sqlite_ml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite_ml-0.1.1.tar", max compression
+gzip compressed data, was "sqlite_ml-0.1.2.tar", max compression
```

## Comparing `sqlite_ml-0.1.1.tar` & `sqlite_ml-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/LICENSE
--rw-r--r--   0        0        0     2842 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/README.md
--rw-r--r--   0        0        0     1045 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/sqlite_ml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/sqlite_ml/py.typed
--rw-r--r--   0        0        0     2477 2023-04-20 14:52:38.994871 sqlite_ml-0.1.1/sqlite_ml/sql/schema.sql
--rw-r--r--   0        0        0    16409 2023-04-20 14:52:38.998871 sqlite_ml-0.1.1/sqlite_ml/sqml.py
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 sqlite_ml-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/LICENSE
+-rw-r--r--   0        0        0    11307 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/README.md
+-rw-r--r--   0        0        0     1047 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/sqlite_ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/sqlite_ml/py.typed
+-rw-r--r--   0        0        0     2477 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/sqlite_ml/sql/schema.sql
+-rw-r--r--   0        0        0    16454 2023-05-26 10:20:44.009261 sqlite_ml-0.1.2/sqlite_ml/sqml.py
+-rw-r--r--   0        0        0    11884 1970-01-01 00:00:00.000000 sqlite_ml-0.1.2/PKG-INFO
```

### Comparing `sqlite_ml-0.1.1/LICENSE` & `sqlite_ml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite_ml-0.1.1/pyproject.toml` & `sqlite_ml-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "sqlite-ml"
-version = "0.1.1"
+version = "0.1.2"
 description = "An SQLite extension for machine learning"
 authors = ["Romain Clement <contact@romain-clement.net>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 packages = [{include = "sqlite_ml"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 scikit-learn = "*"
 pandas = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.3.0"
-faker = "==18.4.0"
+faker = "==18.9.0"
 flake8 = "==6.0.0"
-mypy = "==1.2.0"
+mypy = "==1.3.0"
 pytest = "==7.3.1"
-pytest-cov = "==4.0.0"
-sqlite-utils = "==3.30"
+pytest-cov = "==4.1.0"
+sqlite-utils = "==3.32.1"
 
 [tool.mypy]
 show_error_codes = "True"
 pretty = "True"
 follow_imports = "silent"
 strict_optional = "True"
 warn_redundant_casts = "True"
```

### Comparing `sqlite_ml-0.1.1/sqlite_ml/sql/schema.sql` & `sqlite_ml-0.1.2/sqlite_ml/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `sqlite_ml-0.1.1/sqlite_ml/sqml.py` & `sqlite_ml-0.1.2/sqlite_ml/sqml.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,17 @@
             )
             model_metrics["recall"] = metrics.recall_score(
                 y_test, y_pred, average="weighted"
             )
         else:
             model_metrics["r2"] = metrics.r2_score(y_test, y_pred)
             model_metrics["mae"] = metrics.mean_absolute_error(y_test, y_pred)
-            model_metrics["rmse"] = metrics.mean_squared_error(y_test, y_pred)
+            model_metrics["rmse"] = metrics.mean_squared_error(
+                y_test, y_pred, squared=False
+            )
 
         serialized_model = pickle.dumps(estimator)
 
         with self.conn:
             model = self.conn.execute(
                 """
                 INSERT INTO sqml_models(run_id, library, data)
```


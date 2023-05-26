# Comparing `tmp/alembic_postgresql_enum-0.1.0.tar.gz` & `tmp/alembic_postgresql_enum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-0.1.0.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-0.1.1.tar", max compression
```

## Comparing `alembic_postgresql_enum-0.1.0.tar` & `alembic_postgresql_enum-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.0/LICENSE
--rw-r--r--   0        0        0     3833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.0/README.md
--rw-r--r--   0        0        0      423 2023-05-26 09:19:21.566710 alembic_postgresql_enum-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     4575 2023-05-26 08:19:49.157846 alembic_postgresql_enum-0.1.0/src/enum_alteration.py
--rw-r--r--   0        0        0     2145 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.0/src/enum_creation.py
--rw-r--r--   0        0        0     2833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.0/src/get_enum_data.py
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/README.md
+-rw-r--r--   0        0        0      423 2023-05-26 09:27:41.249844 alembic_postgresql_enum-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     4575 2023-05-26 08:19:49.157846 alembic_postgresql_enum-0.1.1/src/enum_alteration.py
+-rw-r--r--   0        0        0     2145 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/src/enum_creation.py
+-rw-r--r--   0        0        0     2833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/src/get_enum_data.py
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.1/PKG-INFO
```

### Comparing `alembic_postgresql_enum-0.1.0/LICENSE` & `alembic_postgresql_enum-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.0/README.md` & `alembic_postgresql_enum-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.0/src/enum_alteration.py` & `alembic_postgresql_enum-0.1.1/src/enum_alteration.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.0/src/enum_creation.py` & `alembic_postgresql_enum-0.1.1/src/enum_creation.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.0/src/get_enum_data.py` & `alembic_postgresql_enum-0.1.1/src/get_enum_data.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.0/PKG-INFO` & `alembic_postgresql_enum-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 0.1.0
+Version: 0.1.1
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


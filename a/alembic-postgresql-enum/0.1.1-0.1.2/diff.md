# Comparing `tmp/alembic_postgresql_enum-0.1.1.tar.gz` & `tmp/alembic_postgresql_enum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-0.1.1.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-0.1.2.tar", max compression
```

## Comparing `alembic_postgresql_enum-0.1.1.tar` & `alembic_postgresql_enum-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.1/LICENSE
--rw-r--r--   0        0        0     3833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/README.md
--rw-r--r--   0        0        0      423 2023-05-26 09:27:41.249844 alembic_postgresql_enum-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     4575 2023-05-26 08:19:49.157846 alembic_postgresql_enum-0.1.1/src/enum_alteration.py
--rw-r--r--   0        0        0     2145 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/src/enum_creation.py
--rw-r--r--   0        0        0     2833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.1/src/get_enum_data.py
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.2/README.md
+-rw-r--r--   0        0        0       60 2023-05-26 08:19:49.153846 alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/__init__.py
+-rw-r--r--   0        0        0     4575 2023-05-26 08:19:49.157846 alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/enum_alteration.py
+-rw-r--r--   0        0        0     2145 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/enum_creation.py
+-rw-r--r--   0        0        0     2833 2023-05-26 09:08:46.063634 alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/get_enum_data.py
+-rw-r--r--   0        0        0      812 2023-05-26 09:36:00.913393 alembic_postgresql_enum-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 alembic_postgresql_enum-0.1.2/PKG-INFO
```

### Comparing `alembic_postgresql_enum-0.1.1/LICENSE` & `alembic_postgresql_enum-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.1/README.md` & `alembic_postgresql_enum-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.1/src/enum_alteration.py` & `alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/enum_alteration.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.1/src/enum_creation.py` & `alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/enum_creation.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.1/src/get_enum_data.py` & `alembic_postgresql_enum-0.1.2/alembic_postgresql_enum/get_enum_data.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-0.1.1/PKG-INFO` & `alembic_postgresql_enum-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 0.1.1
+Version: 0.1.2
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.15,<3.0.0)
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
+Project-URL: Source code, https://github.com/RustyGuard/alembic-postgresql-enum
 Description-Content-Type: text/markdown
 
 # alembic-postgresql-enum
 Alembic autogenerate support for creation, alteration and deletion of enums
 
 Alembic will now automatically:
 - Create enums that currently are not in postgres schema
```


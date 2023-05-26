# Comparing `tmp/pyodb-0.1.1.tar.gz` & `tmp/pyodb-0.1.2.tar.gz`

## Comparing `pyodb-0.1.1.tar` & `pyodb-0.1.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyodb-0.1.1/.coveragerc
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pyodb-0.1.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 pyodb-0.1.1/MANIFEST.in
--rwxr-xr-x   0        0        0     2774 2020-02-02 00:00:00.000000 pyodb-0.1.1/environment.yaml
--rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyodb-0.1.1/performance.ipynb
--rwxr-xr-x   0        0        0      555 2020-02-02 00:00:00.000000 pyodb-0.1.1/requirements.txt
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyodb-0.1.1/tox.ini
--rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyodb-0.1.1/.github/workflows/python-package.yml
--rwxr-xr-x   0        0        0     2882 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/PyODBCacheExamples.md
--rwxr-xr-x   0        0        0     5905 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/PyODBExamples.md
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/conversion_example.puml
--rwxr-xr-x   0        0        0     7088 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/img/Logo.svg
--rwxr-xr-x   0        0        0    25699 2020-02-02 00:00:00.000000 pyodb-0.1.1/docs/img/conversion_example.svg
--rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyodb-0.1.1/scripts/activate.sh
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.1/scripts/deactivate.sh
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/__init__.py
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/__init__.py
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/_util.py
--rwxr-xr-x   0        0        0      855 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/error.py
--rwxr-xr-x   0        0        0    12732 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/pyodb.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/__init__.py
--rwxr-xr-x   0        0        0    12188 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/_base_schema.py
--rwxr-xr-x   0        0        0     1634 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/shard_schema.py
--rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/unified_schema.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/__init__.py
--rwxr-xr-x   0        0        0     9414 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_operators.py
--rwxr-xr-x   0        0        0    19128 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_sql_builders.py
--rwxr-xr-x   0        0        0     5006 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_table.py
--rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 pyodb-0.1.1/src/pyodb/schema/base/_type_defs.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/__init__.py
--rwxr-xr-x   0        0        0    10884 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/pyodb_test.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/util_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/__init__.py
--rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base_schema_test.py
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/shard_schema_test.py
--rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/unified_schema_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/__init__.py
--rwxr-xr-x   0        0        0     3388 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/operators_test.py
--rwxr-xr-x   0        0        0     7777 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/sql_builders_test.py
--rwxr-xr-x   0        0        0     1589 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/pyodb/schema/base/table_test.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/__init__.py
--rwxr-xr-x   0        0        0     2635 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/complex_models.py
--rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/high_complex_models.py
--rwxr-xr-x   0        0        0     4821 2020-02-02 00:00:00.000000 pyodb-0.1.1/test/test_models/primitive_models.py
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyodb-0.1.1/.gitignore
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyodb-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     8956 2020-02-02 00:00:00.000000 pyodb-0.1.1/README.md
--rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 pyodb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 pyodb-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 pyodb-0.1.2/.coveragerc
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pyodb-0.1.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 pyodb-0.1.2/MANIFEST.in
+-rwxr-xr-x   0        0        0     2776 2020-02-02 00:00:00.000000 pyodb-0.1.2/environment.yaml
+-rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 pyodb-0.1.2/performance.ipynb
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 pyodb-0.1.2/requirements.txt
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 pyodb-0.1.2/tox.ini
+-rwxr-xr-x   0        0        0     1221 2020-02-02 00:00:00.000000 pyodb-0.1.2/.github/workflows/python-package.yml
+-rwxr-xr-x   0        0        0     2882 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/PyODBCacheExamples.md
+-rwxr-xr-x   0        0        0     5905 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/PyODBExamples.md
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/conversion_example.puml
+-rwxr-xr-x   0        0        0     7088 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/img/Logo.svg
+-rwxr-xr-x   0        0        0    25699 2020-02-02 00:00:00.000000 pyodb-0.1.2/docs/img/conversion_example.svg
+-rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 pyodb-0.1.2/scripts/activate.sh
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 pyodb-0.1.2/scripts/deactivate.sh
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/__init__.py
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/__init__.py
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/_util.py
+-rwxr-xr-x   0        0        0      855 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/error.py
+-rwxr-xr-x   0        0        0    12732 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/pyodb.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0    12188 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/_base_schema.py
+-rwxr-xr-x   0        0        0     1634 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/shard_schema.py
+-rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/unified_schema.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     9414 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_operators.py
+-rwxr-xr-x   0        0        0    19128 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_sql_builders.py
+-rwxr-xr-x   0        0        0     5006 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_table.py
+-rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 pyodb-0.1.2/src/pyodb/schema/base/_type_defs.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/__init__.py
+-rwxr-xr-x   0        0        0    10884 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/pyodb_test.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/util_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/__init__.py
+-rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base_schema_test.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/shard_schema_test.py
+-rwxr-xr-x   0        0        0      669 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/unified_schema_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/__init__.py
+-rwxr-xr-x   0        0        0     3388 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/operators_test.py
+-rwxr-xr-x   0        0        0     7777 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/sql_builders_test.py
+-rwxr-xr-x   0        0        0     1589 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/pyodb/schema/base/table_test.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/__init__.py
+-rwxr-xr-x   0        0        0     2635 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/complex_models.py
+-rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/high_complex_models.py
+-rwxr-xr-x   0        0        0     4821 2020-02-02 00:00:00.000000 pyodb-0.1.2/test/test_models/primitive_models.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 pyodb-0.1.2/.gitignore
+-rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 pyodb-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     9337 2020-02-02 00:00:00.000000 pyodb-0.1.2/README.md
+-rwxr-xr-x   0        0        0     1889 2020-02-02 00:00:00.000000 pyodb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 pyodb-0.1.2/PKG-INFO
```

### Comparing `pyodb-0.1.1/.pre-commit-config.yaml` & `pyodb-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/environment.yaml` & `pyodb-0.1.2/environment.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -89,11 +89,11 @@
     - pyproject-hooks==1.0.0
     - pytest==7.2.2
     - pytest-cov==4.0.0
     - pyyaml==6.0
     - rich==13.3.2
     - ruff==0.0.257
     - snakeviz==2.1.1
-    - tornado==6.2
+    - tornado==6.3.2
     - tox==4.4.8
     - virtualenv==20.21.0
 prefix: /usr/miniconda3/envs/pyodb
```

### Comparing `pyodb-0.1.1/performance.ipynb` & `pyodb-0.1.2/performance.ipynb`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/requirements.txt` & `pyodb-0.1.2/requirements.txt`

 * *Files 23% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 pytest==7.2.2
 pytest-cov==4.0.0
 PyYAML==6.0
 rich==13.3.2
 ruff==0.0.257
 snakeviz==2.1.1
 tomli==2.0.1
-tornado==6.2
+tornado==6.3.2
 tox==4.4.8
 virtualenv==20.21.0
```

### Comparing `pyodb-0.1.1/.github/workflows/python-package.yml` & `pyodb-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/docs/PyODBCacheExamples.md` & `pyodb-0.1.2/docs/PyODBCacheExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/docs/PyODBExamples.md` & `pyodb-0.1.2/docs/PyODBExamples.md`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/docs/conversion_example.puml` & `pyodb-0.1.2/docs/conversion_example.puml`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/docs/img/Logo.svg` & `pyodb-0.1.2/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/docs/img/conversion_example.svg` & `pyodb-0.1.2/docs/img/conversion_example.svg`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/scripts/activate.sh` & `pyodb-0.1.2/scripts/activate.sh`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/scripts/deactivate.sh` & `pyodb-0.1.2/scripts/deactivate.sh`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/error.py` & `pyodb-0.1.2/src/pyodb/error.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/pyodb.py` & `pyodb-0.1.2/src/pyodb/pyodb.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/_base_schema.py` & `pyodb-0.1.2/src/pyodb/schema/_base_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/shard_schema.py` & `pyodb-0.1.2/src/pyodb/schema/shard_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/unified_schema.py` & `pyodb-0.1.2/src/pyodb/schema/unified_schema.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/base/_operators.py` & `pyodb-0.1.2/src/pyodb/schema/base/_operators.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/base/_sql_builders.py` & `pyodb-0.1.2/src/pyodb/schema/base/_sql_builders.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/base/_table.py` & `pyodb-0.1.2/src/pyodb/schema/base/_table.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/src/pyodb/schema/base/_type_defs.py` & `pyodb-0.1.2/src/pyodb/schema/base/_type_defs.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/pyodb_test.py` & `pyodb-0.1.2/test/pyodb/pyodb_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/base_schema_test.py` & `pyodb-0.1.2/test/pyodb/schema/base_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/shard_schema_test.py` & `pyodb-0.1.2/test/pyodb/schema/shard_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/unified_schema_test.py` & `pyodb-0.1.2/test/pyodb/schema/unified_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/base/operators_test.py` & `pyodb-0.1.2/test/pyodb/schema/base/operators_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/base/sql_builders_test.py` & `pyodb-0.1.2/test/pyodb/schema/base/sql_builders_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/pyodb/schema/base/table_test.py` & `pyodb-0.1.2/test/pyodb/schema/base/table_test.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/test_models/complex_models.py` & `pyodb-0.1.2/test/test_models/complex_models.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/test_models/high_complex_models.py` & `pyodb-0.1.2/test/test_models/high_complex_models.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/test/test_models/primitive_models.py` & `pyodb-0.1.2/test/test_models/primitive_models.py`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/.gitignore` & `pyodb-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/LICENSE` & `pyodb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodb-0.1.1/README.md` & `pyodb-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # PyODB
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/NeoSecundus/PyODB/python-package.yml)
 [![codecov](https://codecov.io/gh/NeoSecundus/PyODB/branch/main/graph/badge.svg?token=AEXOJTNDWZ)](https://codecov.io/gh/NeoSecundus/PyODB)
+![Open Issues](https://img.shields.io/github/issues-raw/NeoSecundus/PyODB)
+![Closed Issues](https://img.shields.io/github/issues-closed-raw/NeoSecundus/PyODB)
+![PyPI Version](https://img.shields.io/pypi/v/pyodb?color=%23a08)
+![Supported Python Versions](https://img.shields.io/badge/Python%20Versions-3.10+-48f)
+
+
+<img src="docs/img/Logo.svg" style="margin: auto; width: 20vh" />
 
 Python Object DataBase (PyODB) is a SQLite3 ORM library aiming to be as simple to use as possible.
 This library is supposed to be used for testing, in small projects, when wanting to export complex
 python data in a well structured format or for local inter-process data caching.
 
 **Basics:**
 
 - PyODB uses the python built-in SQLite3 implementation as database and has no external dependencies.
 - PyODB can take any (non-primitive) type you pass into it, extracts its members and creates a
-  database schema representing the type. Sub-types of the main type are also extracted recusively.
+  database schema representing the type. Sub-types of the main type are also extracted recursively.
 - Saves instances of known types into the database and loads them using basic filtering options.
 - Also provides a caching module 'PyODBCache' which may be used for inter-process data caching.
   > When using multiprocessing excessively race conditions may occur.
 - All data (cache & non-cache) can persist or be deleted upon closing of the process.
 
 1. [Setup](#setup)
 2. [Basic Usage](#basic-usage)
@@ -83,15 +90,15 @@
 Create a new instance - types are re-loaded from the database since persistent was set to True
 > This time, when the process exits, the data will be deleted because persistent is False by default
 
 ```python
 pyodb = PyODB()
 ```
 
-Now you can get a Selector instance wich is used to select and filter data loaded from the database.
+Now you can get a Selector instance which is used to select and filter data loaded from the database.
 
 ```python
 select = pyodb.select(MyType)
 
 ## filter loaded instances by some_number > 2
 select.gt(some_number = 2)
 
@@ -136,15 +143,15 @@
 ```
 
 As you can see loading and removing data is quite simple. Basic filtering is also possible in both
 select and delete.
 
 ### More in-depth examples
 
-Below are linkts to two documents containing more comprehensive examples of different functions.
+Below are links to two documents containing more comprehensive examples of different functions.
 They also contain best practices regarding performance and some possible error cases.
 
 For PyODB examples please refer to [PyODB examples](./docs/PyODBExamples.md)
 
 For PyODBCache examples please refer to [Caching examples](./docs/PyODBCacheExamples.md)
 
 ## Limitations
@@ -191,15 +198,15 @@
 
 ## How it works
 
 When a python class is added to the PyODB schema the classes are converted to SQL Tables and
 inserted into the database schema.
 
 > IMPORTANT: If a class changes between executions the table retains the old definition.
-> It is advisable to reset the database manually in case it was persistet.
+> It is advisable to reset the database manually in case it was persisted.
 
 The UML Diagram below shows what such a conversion looks like:
 
 ![Conversion Diagram](./docs/img/conversion_example.svg)
 
 ### Converting Primitive Types
 
@@ -221,15 +228,15 @@
 
 Henceforth Origin references the original class whose type is parsed into a SQL Table.
 
 #### Simple custom type
 
 When a simple custom type is contained by the Origin a table is created for the sub-type as
 well. The sub-type's table uses a `_parent_` column which references the `_id_` of the
-Origin and a `_parent_table_` column referenceing the type/table-name of the Origin.
+Origin and a `_parent_table_` column referencing the type/table-name of the Origin.
 
 When an Origin instance is inserted the sub-type instance is saved in it's own table. The table
 which the instance is saved in is then referenced by the Origin's sub-type column. As example:
 
 Here are the columns of an imaginary origin type:
 
 |Column Name| Type | Content |
@@ -251,15 +258,15 @@
 
 Collections and dicts can therefore not be loaded by other programs besides python unlike all other
 datatypes.
 
 ### Dynamic type definitions
 
 Dynamic type definitions (Union) of custom types can also be saved by PyODB.
-Only primitive datatypes must be unambigous.
+Only primitive datatypes must be unambiguous.
 
 The only exception is None. Data may always be defined with None as an option.
 
 **This is allowed:**
 
 ```python
 class Person:
```

### Comparing `pyodb-0.1.1/pyproject.toml` & `pyodb-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyodb"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Nikolas Teuschl", email="nikolas.teuschl@alpha-origin.biz" },
 ]
 description = "Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -14,22 +14,24 @@
 ]
 keywords = [
     "cache", "caching", "datacache",
     "orm", "database", "sqlite",
     "sqlite3",
 ]
 dependencies = []
+license = { file = "LICENSE" }
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project.urls]
 "Homepage" = "https://github.com/NeoSecundus/PyODB"
 "Bug Tracker" = "https://github.com/NeoSecundus/PyODB/issues"
+"Changelog" = "https://github.com/NeoSecundus/PyODB/blob/main/CHANGELOG.md"
 
 [tool.ruff]
 # Which types of errors to include
 select = [
     "F", # Pyflakes
     "E", # PyCodestyle Errors
     "W", # PyCodestyle Warnings
```

### Comparing `pyodb-0.1.1/PKG-INFO` & `pyodb-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,65 @@
 Metadata-Version: 2.1
 Name: pyodb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Object DataBase (PyODB) is an ORM library aiming to be as simple to use as possible.
 Project-URL: Homepage, https://github.com/NeoSecundus/PyODB
 Project-URL: Bug Tracker, https://github.com/NeoSecundus/PyODB/issues
+Project-URL: Changelog, https://github.com/NeoSecundus/PyODB/blob/main/CHANGELOG.md
 Author-email: Nikolas Teuschl <nikolas.teuschl@alpha-origin.biz>
+License: MIT License
+        
+        Copyright (c) 2023 Nikolas Teuschl
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Keywords: cache,caching,database,datacache,orm,sqlite,sqlite3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyODB
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/NeoSecundus/PyODB/python-package.yml)
 [![codecov](https://codecov.io/gh/NeoSecundus/PyODB/branch/main/graph/badge.svg?token=AEXOJTNDWZ)](https://codecov.io/gh/NeoSecundus/PyODB)
+![Open Issues](https://img.shields.io/github/issues-raw/NeoSecundus/PyODB)
+![Closed Issues](https://img.shields.io/github/issues-closed-raw/NeoSecundus/PyODB)
+![PyPI Version](https://img.shields.io/pypi/v/pyodb?color=%23a08)
+![Supported Python Versions](https://img.shields.io/badge/Python%20Versions-3.10+-48f)
+
+
+<img src="docs/img/Logo.svg" style="margin: auto; width: 20vh" />
 
 Python Object DataBase (PyODB) is a SQLite3 ORM library aiming to be as simple to use as possible.
 This library is supposed to be used for testing, in small projects, when wanting to export complex
 python data in a well structured format or for local inter-process data caching.
 
 **Basics:**
 
 - PyODB uses the python built-in SQLite3 implementation as database and has no external dependencies.
 - PyODB can take any (non-primitive) type you pass into it, extracts its members and creates a
-  database schema representing the type. Sub-types of the main type are also extracted recusively.
+  database schema representing the type. Sub-types of the main type are also extracted recursively.
 - Saves instances of known types into the database and loads them using basic filtering options.
 - Also provides a caching module 'PyODBCache' which may be used for inter-process data caching.
   > When using multiprocessing excessively race conditions may occur.
 - All data (cache & non-cache) can persist or be deleted upon closing of the process.
 
 1. [Setup](#setup)
 2. [Basic Usage](#basic-usage)
@@ -98,15 +127,15 @@
 Create a new instance - types are re-loaded from the database since persistent was set to True
 > This time, when the process exits, the data will be deleted because persistent is False by default
 
 ```python
 pyodb = PyODB()
 ```
 
-Now you can get a Selector instance wich is used to select and filter data loaded from the database.
+Now you can get a Selector instance which is used to select and filter data loaded from the database.
 
 ```python
 select = pyodb.select(MyType)
 
 ## filter loaded instances by some_number > 2
 select.gt(some_number = 2)
 
@@ -151,15 +180,15 @@
 ```
 
 As you can see loading and removing data is quite simple. Basic filtering is also possible in both
 select and delete.
 
 ### More in-depth examples
 
-Below are linkts to two documents containing more comprehensive examples of different functions.
+Below are links to two documents containing more comprehensive examples of different functions.
 They also contain best practices regarding performance and some possible error cases.
 
 For PyODB examples please refer to [PyODB examples](./docs/PyODBExamples.md)
 
 For PyODBCache examples please refer to [Caching examples](./docs/PyODBCacheExamples.md)
 
 ## Limitations
@@ -206,15 +235,15 @@
 
 ## How it works
 
 When a python class is added to the PyODB schema the classes are converted to SQL Tables and
 inserted into the database schema.
 
 > IMPORTANT: If a class changes between executions the table retains the old definition.
-> It is advisable to reset the database manually in case it was persistet.
+> It is advisable to reset the database manually in case it was persisted.
 
 The UML Diagram below shows what such a conversion looks like:
 
 ![Conversion Diagram](./docs/img/conversion_example.svg)
 
 ### Converting Primitive Types
 
@@ -236,15 +265,15 @@
 
 Henceforth Origin references the original class whose type is parsed into a SQL Table.
 
 #### Simple custom type
 
 When a simple custom type is contained by the Origin a table is created for the sub-type as
 well. The sub-type's table uses a `_parent_` column which references the `_id_` of the
-Origin and a `_parent_table_` column referenceing the type/table-name of the Origin.
+Origin and a `_parent_table_` column referencing the type/table-name of the Origin.
 
 When an Origin instance is inserted the sub-type instance is saved in it's own table. The table
 which the instance is saved in is then referenced by the Origin's sub-type column. As example:
 
 Here are the columns of an imaginary origin type:
 
 |Column Name| Type | Content |
@@ -266,15 +295,15 @@
 
 Collections and dicts can therefore not be loaded by other programs besides python unlike all other
 datatypes.
 
 ### Dynamic type definitions
 
 Dynamic type definitions (Union) of custom types can also be saved by PyODB.
-Only primitive datatypes must be unambigous.
+Only primitive datatypes must be unambiguous.
 
 The only exception is None. Data may always be defined with None as an option.
 
 **This is allowed:**
 
 ```python
 class Person:
```


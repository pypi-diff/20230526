# Comparing `tmp/flask-sqlacodegen-1.1.8.tar.gz` & `tmp/flask-sqlacodegen-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-sqlacodegen-1.1.8.tar", last modified: Sat Sep 12 19:07:45 2020, max compression
+gzip compressed data, was "flask-sqlacodegen-2.0.0.tar", last modified: Fri May 26 02:11:18 2023, max compression
```

## Comparing `flask-sqlacodegen-1.1.8.tar` & `flask-sqlacodegen-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2020-09-12 19:07:45.640410 flask-sqlacodegen-1.1.8/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1128 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/LICENSE
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       34 2020-09-12 18:49:48.000000 flask-sqlacodegen-1.1.8/MANIFEST.in
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     2893 2020-09-12 19:07:45.640410 flask-sqlacodegen-1.1.8/PKG-INFO
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1597 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/README.md
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2020-09-12 19:07:45.636410 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     2893 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/PKG-INFO
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      479 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/SOURCES.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/dependency_links.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       61 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/entry_points.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/not-zip-safe
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       33 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/requires.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       12 2020-09-12 19:07:45.000000 flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/top_level.txt
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      213 2020-09-12 19:07:45.640410 flask-sqlacodegen-1.1.8/setup.cfg
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     1957 2020-09-12 03:07:22.000000 flask-sqlacodegen-1.1.8/setup.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2020-09-12 19:07:45.636410 flask-sqlacodegen-1.1.8/sqlacodegen/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)       32 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/sqlacodegen/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)    30090 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/sqlacodegen/codegen.py
-drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2020-09-12 19:07:45.636410 flask-sqlacodegen-1.1.8/sqlacodegen/dialects/
--rw-rw-r--   0 kamil     (1000) kamil     (1000)        0 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/sqlacodegen/dialects/__init__.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      862 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/sqlacodegen/dialects/postgresql.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)     3157 2020-09-12 03:03:54.000000 flask-sqlacodegen-1.1.8/sqlacodegen/main.py
--rw-rw-r--   0 kamil     (1000) kamil     (1000)      435 2020-09-12 18:43:02.000000 flask-sqlacodegen-1.1.8/tox.ini
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2023-05-26 02:11:18.687259 flask-sqlacodegen-2.0.0/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1128 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/LICENSE
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       34 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/MANIFEST.in
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2749 2023-05-26 02:11:18.687259 flask-sqlacodegen-2.0.0/PKG-INFO
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     1570 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/README.md
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2023-05-26 02:11:18.687259 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2749 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/PKG-INFO
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      479 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/SOURCES.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/dependency_links.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       61 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/entry_points.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        1 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/not-zip-safe
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       31 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/requires.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       12 2023-05-26 02:11:18.000000 flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/top_level.txt
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      213 2023-05-26 02:11:18.691259 flask-sqlacodegen-2.0.0/setup.cfg
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     2105 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/setup.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2023-05-26 02:11:18.687259 flask-sqlacodegen-2.0.0/sqlacodegen/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)       32 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/sqlacodegen/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)    31073 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/sqlacodegen/codegen.py
+drwxrwxr-x   0 kamil     (1000) kamil     (1000)        0 2023-05-26 02:11:18.687259 flask-sqlacodegen-2.0.0/sqlacodegen/dialects/
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)        0 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/sqlacodegen/dialects/__init__.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      862 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/sqlacodegen/dialects/postgresql.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)     3479 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/sqlacodegen/main.py
+-rw-rw-r--   0 kamil     (1000) kamil     (1000)      435 2023-05-26 02:03:08.000000 flask-sqlacodegen-2.0.0/tox.ini
```

### Comparing `flask-sqlacodegen-1.1.8/LICENSE` & `flask-sqlacodegen-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-sqlacodegen-1.1.8/PKG-INFO` & `flask-sqlacodegen-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,14 @@
 Metadata-Version: 2.1
 Name: flask-sqlacodegen
-Version: 1.1.8
+Version: 2.0.0
 Summary: Automatic model code generator for SQLAlchemy with Flask support
 Home-page: UNKNOWN
 Author: Kamil Sindi
 License: MIT
-Description: # Flask sqlacodegen
-        
-        Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm. Based off of version 1.1.6.
-        
-        What's different:
-        
-        * Support for Flask-SQLAlchemy syntax using `--flask` option.
-        * Defaults to generating backrefs in relationships. `--nobackref` still included as option in case backrefs are not wanted. 
-        * Naming of backrefs is class name in snake_case (as opposed to CamelCase) and is pluralized if it's Many-to-One or Many-to-Many using [inflect](https://pypi.python.org/pypi/inflect).
-        * Primary joins are explicit.
-        * If column has a server_default set it to `FetchValue()` instead of trying to determine what that value is. Original code did not set the right server defaults in my setup.
-        * `--ignore-cols` ignores special columns when generating association tables. Original code requires all columns to be foreign keys in order to generate association table. Example: `--ignore-cols id,inserted,updated`.
-        * Uses the command `flask-sqlacodegen` instead of `sqlacodegen`.
-        * Added support for `--notables` to only generate model classes, even for association tables
-        
-        ## Install
-        
-        With pip:
-        ```sh
-        pip install flask-sqlacodegen
-        ```
-        
-        Without pip:
-        ```sh
-        git clone https://github.com/ksindi/flask-sqlacodegen.git
-        cd flask-sqlacodegen/
-        python setup.py install
-        ```
-        
-        For contributing:
-        ```sh
-        git clone https://github.com/ksindi/flask-sqlacodegen.git
-        python -m venv env
-        pip install -r requirements.txt
-        python -m sqlacodegen.main --flask --outfile models.py mysql+pymysql://<username>:<password>@<database-ip>:<port>/<database-name> [--tables <tablenames>] [--notables]
-        ```
 Keywords: sqlalchemy,sqlacodegen,flask
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Topic :: Database
@@ -54,8 +18,51 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask sqlacodegen
+
+Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm.
+
+What's different:
+
+* Support for Flask-SQLAlchemy syntax using `--flask` option.
+* Defaults to generating backrefs in relationships. `--nobackref` still included as option in case backrefs are not wanted. 
+* Naming of backrefs is class name in snake_case (as opposed to CamelCase) and is pluralized if it's Many-to-One or Many-to-Many using [inflect](https://pypi.python.org/pypi/inflect).
+* Primary joins are explicit.
+* If column has a server_default set it to `FetchValue()` instead of trying to determine what that value is. Original code did not set the right server defaults in my setup.
+* `--ignore-cols` ignores special columns when generating association tables. Original code requires all columns to be foreign keys in order to generate association table. Example: `--ignore-cols id,inserted,updated`.
+* Uses the command `flask-sqlacodegen` instead of `sqlacodegen`.
+* Added support for `--notables` to only generate model classes, even for association tables
+
+## Install
+
+With pip:
+```sh
+pip install flask-sqlacodegen
+```
+
+Without pip:
+```sh
+git clone https://github.com/ksindi/flask-sqlacodegen.git
+cd flask-sqlacodegen/
+python setup.py install
+```
+
+For contributing:
+```sh
+git clone https://github.com/ksindi/flask-sqlacodegen.git
+python -m venv env
+pip install -r requirements.txt
+python -m sqlacodegen.main --flask --outfile models.py mysql+pymysql://<username>:<password>@<database-ip>:<port>/<database-name> [--tables <tablenames>] [--notables]
+```
+
+
```

### Comparing `flask-sqlacodegen-1.1.8/README.md` & `flask-sqlacodegen-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Flask sqlacodegen
 
-Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm. Based off of version 1.1.6.
+Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm.
 
 What's different:
 
 * Support for Flask-SQLAlchemy syntax using `--flask` option.
 * Defaults to generating backrefs in relationships. `--nobackref` still included as option in case backrefs are not wanted. 
 * Naming of backrefs is class name in snake_case (as opposed to CamelCase) and is pluralized if it's Many-to-One or Many-to-Many using [inflect](https://pypi.python.org/pypi/inflect).
 * Primary joins are explicit.
@@ -29,8 +29,8 @@
 
 For contributing:
 ```sh
 git clone https://github.com/ksindi/flask-sqlacodegen.git
 python -m venv env
 pip install -r requirements.txt
 python -m sqlacodegen.main --flask --outfile models.py mysql+pymysql://<username>:<password>@<database-ip>:<port>/<database-name> [--tables <tablenames>] [--notables]
-```
+```
```

### Comparing `flask-sqlacodegen-1.1.8/flask_sqlacodegen.egg-info/PKG-INFO` & `flask-sqlacodegen-2.0.0/flask_sqlacodegen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,14 @@
 Metadata-Version: 2.1
 Name: flask-sqlacodegen
-Version: 1.1.8
+Version: 2.0.0
 Summary: Automatic model code generator for SQLAlchemy with Flask support
 Home-page: UNKNOWN
 Author: Kamil Sindi
 License: MIT
-Description: # Flask sqlacodegen
-        
-        Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm. Based off of version 1.1.6.
-        
-        What's different:
-        
-        * Support for Flask-SQLAlchemy syntax using `--flask` option.
-        * Defaults to generating backrefs in relationships. `--nobackref` still included as option in case backrefs are not wanted. 
-        * Naming of backrefs is class name in snake_case (as opposed to CamelCase) and is pluralized if it's Many-to-One or Many-to-Many using [inflect](https://pypi.python.org/pypi/inflect).
-        * Primary joins are explicit.
-        * If column has a server_default set it to `FetchValue()` instead of trying to determine what that value is. Original code did not set the right server defaults in my setup.
-        * `--ignore-cols` ignores special columns when generating association tables. Original code requires all columns to be foreign keys in order to generate association table. Example: `--ignore-cols id,inserted,updated`.
-        * Uses the command `flask-sqlacodegen` instead of `sqlacodegen`.
-        * Added support for `--notables` to only generate model classes, even for association tables
-        
-        ## Install
-        
-        With pip:
-        ```sh
-        pip install flask-sqlacodegen
-        ```
-        
-        Without pip:
-        ```sh
-        git clone https://github.com/ksindi/flask-sqlacodegen.git
-        cd flask-sqlacodegen/
-        python setup.py install
-        ```
-        
-        For contributing:
-        ```sh
-        git clone https://github.com/ksindi/flask-sqlacodegen.git
-        python -m venv env
-        pip install -r requirements.txt
-        python -m sqlacodegen.main --flask --outfile models.py mysql+pymysql://<username>:<password>@<database-ip>:<port>/<database-name> [--tables <tablenames>] [--notables]
-        ```
 Keywords: sqlalchemy,sqlacodegen,flask
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Topic :: Database
@@ -54,8 +18,51 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask sqlacodegen
+
+Fork of [sqlacodegen](https://pypi.python.org/pypi/sqlacodegen) by Alex Gronholm.
+
+What's different:
+
+* Support for Flask-SQLAlchemy syntax using `--flask` option.
+* Defaults to generating backrefs in relationships. `--nobackref` still included as option in case backrefs are not wanted. 
+* Naming of backrefs is class name in snake_case (as opposed to CamelCase) and is pluralized if it's Many-to-One or Many-to-Many using [inflect](https://pypi.python.org/pypi/inflect).
+* Primary joins are explicit.
+* If column has a server_default set it to `FetchValue()` instead of trying to determine what that value is. Original code did not set the right server defaults in my setup.
+* `--ignore-cols` ignores special columns when generating association tables. Original code requires all columns to be foreign keys in order to generate association table. Example: `--ignore-cols id,inserted,updated`.
+* Uses the command `flask-sqlacodegen` instead of `sqlacodegen`.
+* Added support for `--notables` to only generate model classes, even for association tables
+
+## Install
+
+With pip:
+```sh
+pip install flask-sqlacodegen
+```
+
+Without pip:
+```sh
+git clone https://github.com/ksindi/flask-sqlacodegen.git
+cd flask-sqlacodegen/
+python setup.py install
+```
+
+For contributing:
+```sh
+git clone https://github.com/ksindi/flask-sqlacodegen.git
+python -m venv env
+pip install -r requirements.txt
+python -m sqlacodegen.main --flask --outfile models.py mysql+pymysql://<username>:<password>@<database-ip>:<port>/<database-name> [--tables <tablenames>] [--notables]
+```
+
+
```

### Comparing `flask-sqlacodegen-1.1.8/setup.py` & `flask-sqlacodegen-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,21 +41,24 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords=['sqlalchemy', 'sqlacodegen', 'flask'],
     license='MIT',
     packages=find_packages(exclude=['tests']),
     install_requires=(
-        'SQLAlchemy >= 0.6.0',
-        'inflect >= 0.2.0'
+        "SQLAlchemy >= 2.0",
+        "inflect >= 4.0.0",
     ) + extra_requirements,
     tests_require=['pytest', 'pytest-pep8'],
     cmdclass={'test': PyTest},
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'flask-sqlacodegen=sqlacodegen.main:main'
```

### Comparing `flask-sqlacodegen-1.1.8/sqlacodegen/codegen.py` & `flask-sqlacodegen-2.0.0/sqlacodegen/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Contains the code generation logic and helper functions."""
 from __future__ import unicode_literals, division, print_function, absolute_import
 from collections import defaultdict
-from inspect import ArgSpec
 from keyword import iskeyword
 import inspect
 import sys
 import re
 
 from sqlalchemy import (Enum, ForeignKeyConstraint, PrimaryKeyConstraint, CheckConstraint, UniqueConstraint, Table,
                         Column)
@@ -21,20 +20,23 @@
     from sqlalchemy.sql.expression import text, _TextClause as TextClause
 
 _re_boolean_check_constraint = re.compile(r"(?:(?:.*?)\.)?(.*?) IN \(0, 1\)")
 _re_column_name = re.compile(r'(?:(["`]?)(?:.*)\1\.)?(["`]?)(.*)\2')
 _re_enum_check_constraint = re.compile(r"(?:(?:.*?)\.)?(.*?) IN \((.+)\)")
 _re_enum_item = re.compile(r"'(.*?)(?<!\\)'")
 _re_invalid_identifier = re.compile(r'[^a-zA-Z0-9_]' if sys.version_info[0] < 3 else r'(?u)\W')
+_re_invalid_relationship = re.compile(r'[^a-zA-Z0-9._()\[\]{}= \'",]')
 
 _re_first_cap = re.compile('(.)([A-Z][a-z]+)')
 _re_all_cap = re.compile('([a-z0-9])([A-Z])')
 
 _flask_prepend = 'db.'
 
+_dataclass = False
+
 
 class _DummyInflectEngine(object):
     def singular_noun(self, noun):
         return noun
     def plural_noun(self, noun):  # needed for backrefs
         import inflect
         inflect_engine = inflect.engine()
@@ -88,20 +90,20 @@
     c2 = set(c for c in table2.constraints if isinstance(c, ForeignKeyConstraint) and
              c.elements[0].column.table == table1)
     return c1.union(c2)
 
 
 def _getargspec_init(method):
     try:
-        return inspect.getargspec(method)
+        return inspect.getfullargspec(method)
     except TypeError:
         if method is object.__init__:
-            return ArgSpec(['self'], None, None, None)
+            return inspect.getfullargspec(lambda self: None)
         else:
-            return ArgSpec(['self'], 'args', 'kwargs', None)
+            return inspect.getfullargspec(lambda self, *args, **kwargs: None)
 
 
 def _render_column_type(coltype):
     args = []
     if isinstance(coltype, Enum):
         args.extend(repr(arg) for arg in coltype.enums)
         if coltype.name is not None:
@@ -308,23 +310,27 @@
 
         return text.rstrip('\n,') + '\n)'
 
 
 class ModelClass(Model):
     parent_name = 'Base'
 
-    def __init__(self, table, association_tables, inflect_engine, detect_joined):
+    def __init__(self, table, association_tables, inflect_engine, detect_joined, collector):
         super(ModelClass, self).__init__(table)
         self.name = self._tablename_to_classname(table.name, inflect_engine)
         self.children = []
         self.attributes = OrderedDict()
 
         # Assign attribute names for columns
         for column in table.columns:
             self._add_attribute(column.name, column)
+            if _dataclass:
+                if column.type.python_type.__module__ != 'builtins':
+                    collector.add_literal_import(column.type.python_type.__module__, column.type.python_type.__name__)
+            
 
         # Add many-to-one relationships
         pk_column_names = set(col.name for col in table.primary_key.columns)
         for constraint in sorted(table.constraints, key=_get_constraint_sort_key):
             if isinstance(constraint, ForeignKeyConstraint):
                 target_cls = self._tablename_to_classname(constraint.elements[0].column.table.name, inflect_engine)
                 if (detect_joined and self.parent_name == 'Base' and
@@ -363,15 +369,21 @@
         if any(isinstance(value, Relationship) for value in self.attributes.values()):
             collector.add_literal_import('sqlalchemy.orm', 'relationship')
 
         for child in self.children:
             child.add_imports(collector)
 
     def render(self):
+        global _dataclass        
+            
         text = 'class {0}({1}):\n'.format(self.name, self.parent_name)
+        
+        if _dataclass:
+            text = '@dataclass\n' + text
+            
         text += '    __tablename__ = {0!r}\n'.format(self.table.name)
 
         # Render constraints and indexes as __table_args__
         table_args = []
         for constraint in sorted(self.table.constraints, key=_get_constraint_sort_key):
             if isinstance(constraint, PrimaryKeyConstraint):
                 continue
@@ -398,14 +410,17 @@
             text += '    __table_args__ = (\n        {0}\n    )\n'.format(',\n        '.join(table_args))
 
         # Render columns
         text += '\n'
         for attr, column in self.attributes.items():
             if isinstance(column, Column):
                 show_name = attr != column.name
+                if _dataclass:                    
+                    text += '    ' + attr + ' : ' + column.type.python_type.__name__  + '\n'
+                
                 text += '    {0} = {1}\n'.format(attr, _render_column(column, show_name))
 
         # Render relationships
         if any(isinstance(value, Relationship) for value in self.attributes.values()):
             text += '\n'
         for attr, relationship in self.attributes.items():
             if isinstance(relationship, Relationship):
@@ -433,15 +448,16 @@
         if 'secondaryjoin' in self.kwargs:
             text += '\n        '
             delimiter, end = ',\n        ', '\n    )'
         else:
             delimiter, end = ', ', ')'
 
         args.extend([key + '=' + value for key, value in self.kwargs.items()])
-        return text + delimiter.join(args) + end
+        
+        return _re_invalid_relationship.sub('_', text + delimiter.join(args) + end)
 
     def make_backref(self, relationships, classes):
         backref = self.backref_name
         original_backref = backref
         # Check if backref already exists for relationship source_cls to target_cls and add suffix
         suffix = 0
         while (self.target_cls, backref) in [(x.target_cls, x.backref_name) for x in relationships]:
@@ -530,15 +546,15 @@
 
 class CodeGenerator(object):
     header = '# coding: utf-8'
     footer = ''
 
     def __init__(self, metadata, noindexes=False, noconstraints=False,
                  nojoined=False, noinflect=False, nobackrefs=False,
-                 flask=False, ignore_cols=None, noclasses=False, nocomments=False, notables=False):
+                 flask=False, ignore_cols=None, noclasses=False, nocomments=False, notables=False, dataclass=False):
         super(CodeGenerator, self).__init__()
 
         if noinflect:
             inflect_engine = _DummyInflectEngine()
         else:
             import inflect
             inflect_engine = inflect.engine()
@@ -548,14 +564,19 @@
         
         self.flask = flask
         if not self.flask:
             global _flask_prepend
             _flask_prepend = ''
 
         self.nocomments = nocomments
+        
+        self.dataclass = dataclass
+        if self.dataclass:
+            global _dataclass
+            _dataclass = True
 
         # Pick association tables from the metadata into their own set, don't process them normally
         links = defaultdict(lambda: [])
         association_tables = set()
         for table in metadata.tables.values():
             # Link tables have exactly two foreign key constraints and all columns are involved in them
             # except for special columns like id, inserted, and updated
@@ -606,21 +627,21 @@
                                 if not isinstance(table.c[colname].type, Enum):
                                     options = _re_enum_item.findall(items)
                                     table.c[colname].type = Enum(*options, native_enum=False)
                                 continue
 
             # Only generate classes when notables is set to True
             if notables:
-                model = ModelClass(table, links[table.name], inflect_engine, not nojoined)
+                model = ModelClass(table, links[table.name], inflect_engine, not nojoined, self.collector)
                 classes[model.name] = model
             elif not table.primary_key or table.name in association_tables or noclasses:
                 # Only form model classes for tables that have a primary key and are not association tables
                 model = ModelTable(table)
             elif not noclasses:
-                model = ModelClass(table, links[table.name], inflect_engine, not nojoined)
+                model = ModelClass(table, links[table.name], inflect_engine, not nojoined, self.collector)
                 classes[model.name] = model
 
             self.models.append(model)
 
             # collect imports for models only if flask is not specified
             if not self.flask:
                 model.add_imports(self.collector)
@@ -648,16 +669,21 @@
 
             for model in classes.values():
                 if model.parent_name == 'Base':
                     model.parent_name = parent_name
         else:
             self.collector.add_literal_import('sqlalchemy.ext.declarative', 'declarative_base')
             self.collector.add_literal_import('sqlalchemy', 'MetaData')
+            
+            
+        if self.dataclass:
+            self.collector.add_literal_import('dataclasses', 'dataclass')
 
     def render(self, outfile=sys.stdout):
+        
         print(self.header, file=outfile)
 
         # Render the collected imports
         print(self.collector.render() + '\n\n', file=outfile)
 
         if self.flask:
             print('db = SQLAlchemy()', file=outfile)
```

### Comparing `flask-sqlacodegen-1.1.8/sqlacodegen/dialects/postgresql.py` & `flask-sqlacodegen-2.0.0/sqlacodegen/dialects/postgresql.py`

 * *Files identical despite different names*

### Comparing `flask-sqlacodegen-1.1.8/sqlacodegen/main.py` & `flask-sqlacodegen-2.0.0/sqlacodegen/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,45 +22,50 @@
 
 
 def main():
     parser = argparse.ArgumentParser(description='Generates SQLAlchemy model code from an existing database.')
     parser.add_argument('url', nargs='?', help='SQLAlchemy url to the database')
     parser.add_argument('--version', action='store_true', help="print the version number and exit")
     parser.add_argument('--schema', help='load tables from an alternate schema')
+    parser.add_argument('--default-schema', help='default schema name for local schema object')
     parser.add_argument('--tables', help='tables to process (comma-separated, default: all)')
     parser.add_argument('--noviews', action='store_true', help="ignore views")
     parser.add_argument('--noindexes', action='store_true', help='ignore indexes')
     parser.add_argument('--noconstraints', action='store_true', help='ignore constraints')
     parser.add_argument('--nojoined', action='store_true', help="don't autodetect joined table inheritance")
     parser.add_argument('--noinflect', action='store_true', help="don't try to convert tables names to singular form")
     parser.add_argument('--noclasses', action='store_true', help="don't generate classes, only tables")
     parser.add_argument('--notables', action='store_true', help="don't generate tables, only classes")
     parser.add_argument('--outfile', help='file to write output to (default: stdout)')
     parser.add_argument('--nobackrefs', action='store_true', help="don't include backrefs")
     parser.add_argument('--flask', action='store_true', help="use Flask-SQLAlchemy columns")
     parser.add_argument('--ignore-cols', help="Don't check foreign key constraints on specified columns (comma-separated)")
     parser.add_argument('--nocomments', action='store_true', help="don't render column comments")
+    parser.add_argument('--dataclass', action='store_true', help="add dataclass decorators for JSON serialization")
     args = parser.parse_args()
 
     if args.version:
         print(sqlacodegen.version)
         return
     if not args.url:
         print('You must supply a url\n', file=sys.stderr)
         parser.print_help()
         return
+    default_schema = args.default_schema
+    if not default_schema:
+        default_schema = None  
 
     engine = create_engine(args.url)
     import_dialect_specificities(engine)
-    metadata = MetaData(engine)
+    metadata = MetaData()
     tables = args.tables.split(',') if args.tables else None
     ignore_cols = args.ignore_cols.split(',') if args.ignore_cols else None
     metadata.reflect(engine, args.schema, not args.noviews, tables)
     outfile = codecs.open(args.outfile, 'w', encoding='utf-8') if args.outfile else sys.stdout
     generator = CodeGenerator(metadata, args.noindexes, args.noconstraints,
                               args.nojoined, args.noinflect, args.nobackrefs,
-                              args.flask, ignore_cols, args.noclasses, args.nocomments, args.notables)
+                              args.flask, ignore_cols, args.noclasses, args.nocomments, args.notables, args.dataclass)
     generator.render(outfile)
 
 
 if __name__ == '__main__':
     main()
```


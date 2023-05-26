# Comparing `tmp/ardilla-0.2.0b0.tar.gz` & `tmp/ardilla-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.2.0b0.tar", last modified: Thu May 25 18:23:30 2023, max compression
+gzip compressed data, was "ardilla-0.2.1b0.tar", last modified: Fri May 26 03:01:09 2023, max compression
```

## Comparing `ardilla-0.2.0b0.tar` & `ardilla-0.2.1b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.856564 ardilla-0.2.0b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.2.0b0/LICENCE
--rw-rw-rw-   0        0        0     5298 2023-05-25 18:23:30.853564 ardilla-0.2.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     4396 2023-05-25 05:34:17.000000 ardilla-0.2.0b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.755033 ardilla-0.2.0b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.2.0b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     3537 2023-05-23 20:17:34.000000 ardilla-0.2.0b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.836562 ardilla-0.2.0b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.2.0b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.2.0b0/ardilla/asyncio/abc.py
--rw-rw-rw-   0        0        0     8082 2023-05-25 17:33:42.000000 ardilla-0.2.0b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     2398 2023-05-25 18:19:51.000000 ardilla-0.2.0b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     7762 2023-05-25 17:31:21.000000 ardilla-0.2.0b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     4983 2023-05-25 18:16:14.000000 ardilla-0.2.0b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.2.0b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.2.0b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.2.0b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2885 2023-05-25 17:39:33.000000 ardilla-0.2.0b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.2.0b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.2.0b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5181 2023-05-25 17:28:48.000000 ardilla-0.2.0b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.819551 ardilla-0.2.0b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     5298 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 18:23:30.000000 ardilla-0.2.0b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1215 2023-05-25 18:22:15.000000 ardilla-0.2.0b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 18:23:30.856564 ardilla-0.2.0b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-25 18:23:30.848563 ardilla-0.2.0b0/tests/
--rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.2.0b0/tests/test_async.py
--rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.2.0b0/tests/test_models.py
--rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.2.0b0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.099812 ardilla-0.2.1b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.2.1b0/LICENCE
+-rw-rw-rw-   0        0        0     5298 2023-05-26 03:01:09.097814 ardilla-0.2.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     4396 2023-05-25 05:34:17.000000 ardilla-0.2.1b0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.003809 ardilla-0.2.1b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.2.1b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     3537 2023-05-26 02:48:12.000000 ardilla-0.2.1b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.084811 ardilla-0.2.1b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.2.1b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-13 04:14:11.000000 ardilla-0.2.1b0/ardilla/asyncio/abc.py
+-rw-rw-rw-   0        0        0     8929 2023-05-26 02:57:48.000000 ardilla-0.2.1b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     2398 2023-05-25 18:19:51.000000 ardilla-0.2.1b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     8537 2023-05-26 02:56:48.000000 ardilla-0.2.1b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     4983 2023-05-25 18:16:14.000000 ardilla-0.2.1b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      316 2023-05-18 15:14:26.000000 ardilla-0.2.1b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.2.1b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.2.1b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2885 2023-05-25 17:39:33.000000 ardilla-0.2.1b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.2.1b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6456 2023-05-24 16:04:50.000000 ardilla-0.2.1b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     5181 2023-05-25 17:28:48.000000 ardilla-0.2.1b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.052814 ardilla-0.2.1b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     5298 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 03:01:08.000000 ardilla-0.2.1b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1216 2023-05-26 03:00:00.000000 ardilla-0.2.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 03:01:09.099812 ardilla-0.2.1b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 03:01:09.094814 ardilla-0.2.1b0/tests/
+-rw-rw-rw-   0        0        0     8304 2023-05-22 16:57:24.000000 ardilla-0.2.1b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     1909 2023-05-18 02:32:05.000000 ardilla-0.2.1b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     8383 2023-05-22 16:34:39.000000 ardilla-0.2.1b0/tests/test_sync.py
```

### Comparing `ardilla-0.2.0b0/LICENCE` & `ardilla-0.2.1b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/PKG-INFO` & `ardilla-0.2.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ardilla-0.2.0b0/README.md` & `ardilla-0.2.1b0/README.md`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/abc.py` & `ardilla-0.2.1b0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/asyncio/crud.py` & `ardilla-0.2.1b0/ardilla/asyncio/crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+from functools import wraps
 from typing import Literal, Generic, Optional, Union
 
 import aiosqlite
 from aiosqlite import Row
 
 from ..errors import QueryExecutionError
 from ..models import M
@@ -9,19 +11,33 @@
 from ..logging import log
 from ..schemas import SQLFieldType
 from .. import queries
 
 from .abc import AbstractAsyncEngine
 
 
+def async_verify_kws(coro):
+    """
+    Decorator for sync Crud methods to prevent
+    injection in the keys of the CRUD methods
+    """
+    @wraps(coro)
+    async def wrapper(self: AsyncCrud, *ags, **kws):
+        for key in kws:
+            if key not in self.Model.__fields__:
+                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
+        return await coro(self, *ags, **kws)
+    return wrapper
+
 class AsyncCrud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
     engine: AbstractAsyncEngine
 
+    @async_verify_kws
     async def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
         """Returns a row as an instance of the model if one is found or none
 
         Args:
             kws (SQLFieldType): The keyword arguments are passed as column names and values to
                 a select query
 
@@ -77,40 +93,43 @@
                 if returning and row:
                     return self._row2obj(row, cur.lastrowid)
             finally:
                 if cur is not None:
                     await cur.close()
                 await con.close()
 
+    @async_verify_kws
     async def insert(self, **kws: SQLFieldType) -> M:
         """
         Inserts a record into the database.
 
         Args:
             kws (SQLFieldType): the column names and values for the insertion query
 
         Returns:
             Returns the inserted row as an instance of the model
         Rises:
             ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
         """
         return await self._do_insert(False, True, **kws)
 
+    @async_verify_kws
     async def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
         """Inserts a record to the database with the keywords passed. It ignores conflicts.
 
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
 
         Returns:
             The newly created row as an instance of the model if there was no conflicts
         """
         return await self._do_insert(True, True, **kws)
 
+    @async_verify_kws
     async def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
         """Returns an object from the database with the spefied matching data
         Args:
             kws (SQLFieldType): the key value pairs will be used to query for an existing row
                 if no record is found then a new row will be inserted
         Returns:
             A tuple with two values, the object and a boolean indicating if the
@@ -118,15 +137,15 @@
         """
         created = False
         result = await self.get_or_none(**kws)
         if not result:
             result = await self.insert_or_ignore(**kws)
             created = True
         return result, created
-
+    
     async def get_all(self) -> list[M]:
         """Gets all objects from the database
         
         Returns:
             A list with all the rows in table as instances of the model
         """
         q = f"SELECT rowid, * FROM {self.tablename};"
@@ -151,14 +170,18 @@
             kws (SQLFieldType): the column names and values for the select query
 
             limit (Optional[int], optional): The number of items to return. Defaults to None.
 
         Returns:
             a list of rows matching the criteria as intences of the model
         """
+        for key in kws:
+            if key not in self.Model.__fields__:
+                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
+            
         q, vals = queries.for_get_many(
             self.Model, order_by=order_by, limit=limit, kws=kws
         )
         async with self.engine as con:
             async with con.execute(q, vals) as cur:
                 rows: list[Row] = await cur.fetchall()
                 return [self._row2obj(row) for row in rows]
```

### Comparing `ardilla-0.2.0b0/ardilla/asyncio/engine.py` & `ardilla-0.2.1b0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/crud.py` & `ardilla-0.2.1b0/ardilla/crud.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+from __future__ import annotations
+from functools import wraps
 import sqlite3
 from sqlite3 import Row
 from typing import Literal, Generic, Optional, Union
 
 from .abc import CrudABC, AbstractEngine
 from .models import M
 from .errors import QueryExecutionError
 from .logging import log
 from .schemas import SQLFieldType
 from . import queries
 
 
+def verify_kws(f):
+    """
+    Decorator for sync Crud methods to prevent
+    injection in the keys of the CRUD methods
+    """
+    @wraps(f)
+    def wrapper(self: Crud, *ags, **kws):
+        for key in kws:
+            if key not in self.Model.__fields__:
+                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
+        return f(self, *ags, **kws)
+    return wrapper
+
 class Crud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
     engine: AbstractEngine
 
     def _do_insert(
         self,
@@ -47,14 +62,15 @@
                 row = cur.fetchone()
                 con.commit()
                 if returning and row:
                     return self._row2obj(row, cur.lastrowid)
 
         return None
 
+    @verify_kws
     def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
         """Returns a row as an instance of the model if one is found or none
 
         Args:
             kws (SQLFieldType): The keyword arguments are passed as column names and values to 
                 a select query
             
@@ -74,14 +90,15 @@
             with ctxcur as cur:
                 cur.execute(q, vals)
                 row: Union[Row, None] = cur.fetchone()
                 if row:
                     return self._row2obj(row)
         return None
 
+    @verify_kws
     def insert(self, **kws: SQLFieldType) -> M:
         """Inserts a record into the database.
         
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
         
@@ -89,26 +106,29 @@
             Creates a new entry in the database and returns the object
             
         Rises:
             `ardilla.error.QueryExecutionError`: if there's a conflict when inserting the record
         """
         return self._do_insert(False, True, **kws)
 
+    @verify_kws
     def insert_or_ignore(self, **kws: SQLFieldType) -> Optional[M]:
         """Inserts a record to the database with the keywords passed. It ignores conflicts.
         
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
 
         Returns:
             The newly created row as an instance of the model if there was no conflicts
         """
         return self._do_insert(True, True, **kws)
 
+
+    @verify_kws
     def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
         """Returns an object from the database with the spefied matching data
         Args:
             kws (SQLFieldType): the key value pairs will be used to query for an existing row
                 if no record is found then a new row will be inserted
         Returns:
             A tuple with two values, the object and a boolean indicating if the 
@@ -143,14 +163,17 @@
             
             limit (Optional[int], optional): The number of items to return. Defaults to None.
             kws (SQLFieldType): The column names and values for the select query
 
         Returns:
             a list of rows matching the criteria as intences of the model
         """
+        for key in kws:
+            if key not in self.Model.__fields__:
+                raise KeyError(f'"{key}" is not a field of the "{self.Model.__name__}" and cannot be used in queries')
         q, vals = queries.for_get_many(self.Model, order_by=order_by, limit=limit, kws=kws)
         with self.engine as con:
             ctxcur = self.engine.cursor(con)
             with ctxcur as cur:
                 cur.execute(q, vals)
                 rows: list[Row] = cur.fetchall()
                 return [self._row2obj(row) for row in rows]
```

### Comparing `ardilla-0.2.0b0/ardilla/engine.py` & `ardilla-0.2.1b0/ardilla/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/fields.py` & `ardilla-0.2.1b0/ardilla/fields.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/models.py` & `ardilla-0.2.1b0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/ordering.py` & `ardilla-0.2.1b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/queries.py` & `ardilla-0.2.1b0/ardilla/queries.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla/schemas.py` & `ardilla-0.2.1b0/ardilla/schemas.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/ardilla.egg-info/PKG-INFO` & `ardilla-0.2.1b0/ardilla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ardilla-0.2.0b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.2.1b0/ardilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/pyproject.toml` & `ardilla-0.2.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.2.0-beta"
+version = "0.2.1-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
 
@@ -34,13 +34,13 @@
   "pytest==7.3.1", # testing
   "pytest-asyncio==0.21.0", # testing async
   "black==23.3.0", # formating
 ]
 docs = [
   "mkdocs==1.4.3",
   "jinja2<3.1.0",
-  "mkdocstrings[python]==0.21.2"
+  "mkdocstrings[python]==0.21.2",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

### Comparing `ardilla-0.2.0b0/tests/test_async.py` & `ardilla-0.2.1b0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/tests/test_models.py` & `ardilla-0.2.1b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.2.0b0/tests/test_sync.py` & `ardilla-0.2.1b0/tests/test_sync.py`

 * *Files identical despite different names*


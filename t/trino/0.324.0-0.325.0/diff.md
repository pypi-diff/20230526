# Comparing `tmp/trino-0.324.0.tar.gz` & `tmp/trino-0.325.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trino-0.324.0.tar", last modified: Mon May 15 13:47:40 2023, max compression
+gzip compressed data, was "trino-0.325.0.tar", last modified: Fri May 26 07:12:43 2023, max compression
```

## Comparing `trino-0.324.0.tar` & `trino-0.325.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-15 13:47:24.000000 trino-0.324.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 13:47:40.201059 trino-0.324.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-15 13:47:24.000000 trino-0.324.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 13:47:40.205060 trino-0.324.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3451 2023-05-15 13:47:24.000000 trino-0.324.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-15 13:47:28.000000 trino-0.324.0/trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-15 13:47:24.000000 trino-0.324.0/trino/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    46886 2023-05-15 13:47:24.000000 trino-0.324.0/trino/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-15 13:47:24.000000 trino-0.324.0/trino/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    22753 2023-05-15 13:47:24.000000 trino-0.324.0/trino/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-15 13:47:24.000000 trino-0.324.0/trino/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-15 13:47:24.000000 trino-0.324.0/trino/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-15 13:47:24.000000 trino-0.324.0/trino/sqlalchemy/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-15 13:47:24.000000 trino-0.324.0/trino/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:47:40.201059 trino-0.324.0/trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 13:47:40.000000 trino-0.324.0/trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 07:12:27.000000 trino-0.325.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 07:12:43.769862 trino-0.325.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-05-26 07:12:27.000000 trino-0.325.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-26 07:12:43.769862 trino-0.325.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-05-26 07:12:27.000000 trino-0.325.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.765862 trino-0.325.0/trino/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-26 07:12:30.000000 trino-0.325.0/trino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-26 07:12:27.000000 trino-0.325.0/trino/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46886 2023-05-26 07:12:27.000000 trino-0.325.0/trino/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-26 07:12:27.000000 trino-0.325.0/trino/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-05-26 07:12:27.000000 trino-0.325.0/trino/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-26 07:12:27.000000 trino-0.325.0/trino/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 07:12:27.000000 trino-0.325.0/trino/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/trino/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-26 07:12:27.000000 trino-0.325.0/trino/sqlalchemy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 07:12:27.000000 trino-0.325.0/trino/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:12:43.769862 trino-0.325.0/trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 07:12:43.000000 trino-0.325.0/trino.egg-info/top_level.txt
```

### Comparing `trino-0.324.0/LICENSE` & `trino-0.325.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/PKG-INFO` & `trino-0.325.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.324.0
+Version: 0.325.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.324.0/README.md` & `trino-0.325.0/README.md`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/setup.py` & `trino-0.325.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         "Topic :: Database :: Front-Ends",
     ],
     python_requires='>=3.7',
     install_requires=[
         "backports.zoneinfo;python_version<'3.9'",
         "python-dateutil",
         "pytz",
-        "requests",
+        # requests CVE https://github.com/advisories/GHSA-j8r2-6x86-q33q
+        "requests>=2.31.0",
         "tzlocal",
     ],
     extras_require={
         "all": all_require,
         "kerberos": kerberos_require,
         "sqlalchemy": sqlalchemy_require,
         "tests": tests_require,
```

### Comparing `trino-0.324.0/trino/__init__.py` & `trino-0.325.0/trino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
 __all__ = ['auth', 'dbapi', 'client', 'constants', 'exceptions', 'logging']
 
-__version__ = "0.324.0"
+__version__ = "0.325.0"
```

### Comparing `trino-0.324.0/trino/auth.py` & `trino-0.325.0/trino/auth.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/client.py` & `trino-0.325.0/trino/client.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/constants.py` & `trino-0.325.0/trino/constants.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/dbapi.py` & `trino-0.325.0/trino/dbapi.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 Fetch methods returns rows as a list of lists on purpose to let the caller
 decide to convert then to a list of tuples.
 """
 import binascii
 import datetime
 import math
 import uuid
+from collections import OrderedDict
 from decimal import Decimal
+from threading import Lock
+from time import time
 from typing import Any, Dict, List, NamedTuple, Optional  # NOQA for mypy types
 from urllib.parse import urlparse
 
 try:
     from zoneinfo import ZoneInfo
 except ModuleNotFoundError:
     from backports.zoneinfo import ZoneInfo
@@ -74,14 +77,49 @@
 apilevel = "2.0"
 threadsafety = 2
 paramstyle = "qmark"
 
 logger = trino.logging.get_logger(__name__)
 
 
+class TimeBoundLRUCache:
+    """A bounded LRU cache which expires entries after a configured number of seconds.
+    Note that expired entries will be evicted only on an attempted access (or through
+    the LRU policy)."""
+    def __init__(self, capacity: int, ttl_seconds: int):
+        self.capacity = capacity
+        self.ttl_seconds = ttl_seconds
+        self.cache = OrderedDict()
+        self.lock = Lock()
+
+    def get(self, key):
+        with self.lock:
+            if key not in self.cache:
+                return None
+            value, timestamp = self.cache[key]
+            if time() - timestamp > self.ttl_seconds:
+                self.cache.pop(key)
+                return None
+            self.cache.move_to_end(key)
+            return value
+
+    def put(self, key, value):
+        with self.lock:
+            self.cache[key] = value, time()
+            self.cache.move_to_end(key)
+            if len(self.cache) > self.capacity:
+                self.cache.popitem(last=False)
+
+    def __repr__(self):
+        return f"LRUCache(capacity: {self.capacity}, ttl: {self.ttl_seconds} seconds, {self.cache})"
+
+
+must_use_legacy_prepared_statements = TimeBoundLRUCache(1024, 3600)
+
+
 def connect(*args, **kwargs):
     """Constructor for creating a connection to the database.
 
     See class :py:class:`Connection` for arguments.
 
     :returns: a :py:class:`Connection` object.
     """
@@ -113,14 +151,15 @@
         max_attempts=constants.DEFAULT_MAX_ATTEMPTS,
         request_timeout=constants.DEFAULT_REQUEST_TIMEOUT,
         isolation_level=IsolationLevel.AUTOCOMMIT,
         verify=True,
         http_session=None,
         client_tags=None,
         legacy_primitive_types=False,
+        legacy_prepared_statements=None,
         roles=None,
         timezone=None,
     ):
         # Automatically assign http_schema, port based on hostname
         parsed_host = urlparse(host, allow_fragments=False)
 
         self.host = host if parsed_host.hostname is None else parsed_host.hostname + parsed_host.path
@@ -158,14 +197,15 @@
         self.request_timeout = request_timeout
         self.client_tags = client_tags
 
         self._isolation_level = isolation_level
         self._request = None
         self._transaction = None
         self.legacy_primitive_types = legacy_primitive_types
+        self.legacy_prepared_statements = legacy_prepared_statements
 
     @property
     def isolation_level(self):
         return self._isolation_level
 
     @property
     def transaction(self):
@@ -224,18 +264,37 @@
         if self.transaction is not None:
             request = self.transaction.request
         else:
             request = self._create_request()
         return Cursor(
             self,
             request,
-            # if legacy_primitive_types is not explicitly set in Cursor, take from Connection
+            # if legacy params are not explicitly set in Cursor, take them from Connection
             legacy_primitive_types if legacy_primitive_types is not None else self.legacy_primitive_types
         )
 
+    def _use_legacy_prepared_statements(self):
+        if self.legacy_prepared_statements is not None:
+            return self.legacy_prepared_statements
+
+        value = must_use_legacy_prepared_statements.get((self.host, self.port))
+        if value is None:
+            try:
+                query = trino.client.TrinoQuery(
+                    self._create_request(),
+                    query="EXECUTE IMMEDIATE 'SELECT 1'")
+                query.execute()
+            except Exception as e:
+                logger.warning(
+                    "EXECUTE IMMEDIATE not available for %s:%s; defaulting to legacy prepared statements (%s)",
+                    self.host, self.port, e)
+                value = True
+                must_use_legacy_prepared_statements.put((self.host, self.port), value)
+        return value
+
 
 class DescribeOutput(NamedTuple):
     name: str
     catalog: str
     schema: str
     table: str
     type: str
@@ -276,15 +335,19 @@
     """Database cursor.
 
     Cursors are not isolated, i.e., any changes done to the database by a
     cursor are immediately visible by other cursors or connections.
 
     """
 
-    def __init__(self, connection, request, legacy_primitive_types: bool = False):
+    def __init__(
+            self,
+            connection,
+            request,
+            legacy_primitive_types: bool = False):
         if not isinstance(connection, Connection):
             raise ValueError(
                 "connection must be a Connection object: {}".format(type(connection))
             )
         self._connection = connection
         self._request = request
 
@@ -387,14 +450,26 @@
         self,
         statement_name,
         params
     ):
         sql = 'EXECUTE ' + statement_name + ' USING ' + ','.join(map(self._format_prepared_param, params))
         return trino.client.TrinoQuery(self._request, query=sql, legacy_primitive_types=self._legacy_primitive_types)
 
+    def _execute_immediate_statement(self, statement: str, params):
+        """
+        Binds parameters and executes a statement in one call.
+
+        :param statement: sql to be executed.
+        :param params: parameters to be bound.
+        """
+        sql = "EXECUTE IMMEDIATE '" + statement.replace("'", "''") + \
+              "' USING " + ",".join(map(self._format_prepared_param, params))
+        return trino.client.TrinoQuery(
+            self.connection._create_request(), query=sql, legacy_primitive_types=self._legacy_primitive_types)
+
     def _format_prepared_param(self, param):
         """
         Formats parameters to be passed in an
         EXECUTE statement.
         """
         if param is None:
             return "NULL"
@@ -488,30 +563,34 @@
     def execute(self, operation, params=None):
         if params:
             assert isinstance(params, (list, tuple)), (
                 'params must be a list or tuple containing the query '
                 'parameter values'
             )
 
-            statement_name = self._generate_unique_statement_name()
-            self._prepare_statement(operation, statement_name)
-
-            try:
-                # Send execute statement and assign the return value to `results`
-                # as it will be returned by the function
-                self._query = self._execute_prepared_statement(
-                    statement_name, params
-                )
+            if self.connection._use_legacy_prepared_statements():
+                statement_name = self._generate_unique_statement_name()
+                self._prepare_statement(operation, statement_name)
+
+                try:
+                    # Send execute statement and assign the return value to `results`
+                    # as it will be returned by the function
+                    self._query = self._execute_prepared_statement(
+                        statement_name, params
+                    )
+                    self._iterator = iter(self._query.execute())
+                finally:
+                    # Send deallocate statement
+                    # At this point the query can be deallocated since it has already
+                    # been executed
+                    # TODO: Consider caching prepared statements if requested by caller
+                    self._deallocate_prepared_statement(statement_name)
+            else:
+                self._query = self._execute_immediate_statement(operation, params)
                 self._iterator = iter(self._query.execute())
-            finally:
-                # Send deallocate statement
-                # At this point the query can be deallocated since it has already
-                # been executed
-                # TODO: Consider caching prepared statements if requested by caller
-                self._deallocate_prepared_statement(statement_name)
 
         else:
             self._query = trino.client.TrinoQuery(self._request, query=operation,
                                                   legacy_primitive_types=self._legacy_primitive_types)
             self._iterator = iter(self._query.execute())
         return self
```

### Comparing `trino-0.324.0/trino/exceptions.py` & `trino-0.325.0/trino/exceptions.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/logging.py` & `trino-0.325.0/trino/logging.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/sqlalchemy/__init__.py` & `trino-0.325.0/trino/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/sqlalchemy/compiler.py` & `trino-0.325.0/trino/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/sqlalchemy/datatype.py` & `trino-0.325.0/trino/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/sqlalchemy/dialect.py` & `trino-0.325.0/trino/sqlalchemy/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,17 @@
 
         if "client_tags" in url.query:
             kwargs["client_tags"] = json.loads(unquote_plus(url.query["client_tags"]))
 
         if "legacy_primitive_types" in url.query:
             kwargs["legacy_primitive_types"] = json.loads(unquote_plus(url.query["legacy_primitive_types"]))
 
+        if "legacy_prepared_statements" in url.query:
+            kwargs["legacy_prepared_statements"] = unquote_plus(url.query["legacy_prepared_statements"])
+
         if "verify" in url.query:
             kwargs["verify"] = json.loads(unquote_plus(url.query["verify"]))
 
         if "roles" in url.query:
             kwargs["roles"] = json.loads(url.query["roles"])
 
         return args, kwargs
```

### Comparing `trino-0.324.0/trino/sqlalchemy/error.py` & `trino-0.325.0/trino/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino/sqlalchemy/util.py` & `trino-0.325.0/trino/sqlalchemy/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     schema: Optional[str] = None,
     source: Optional[str] = "trino-sqlalchemy",
     session_properties: Dict[str, str] = None,
     http_headers: Dict[str, Union[str, int]] = None,
     extra_credential: Optional[List[Tuple[str, str]]] = None,
     client_tags: Optional[List[str]] = None,
     legacy_primitive_types: Optional[bool] = None,
+    legacy_prepared_statements: Optional[bool] = None,
     access_token: Optional[str] = None,
     cert: Optional[str] = None,
     key: Optional[str] = None,
     verify: Optional[bool] = None,
     roles: Optional[Dict[str, str]] = None
 ) -> str:
     """
@@ -81,14 +82,17 @@
 
     if client_tags is not None:
         trino_url += f"&client_tags={quote_plus(json.dumps(client_tags))}"
 
     if legacy_primitive_types is not None:
         trino_url += f"&legacy_primitive_types={json.dumps(legacy_primitive_types)}"
 
+    if legacy_prepared_statements is not None:
+        trino_url += f"&legacy_prepared_statements={json.dumps(legacy_prepared_statements)}"
+
     if access_token is not None:
         trino_url += f"&access_token={quote_plus(access_token)}"
 
     if cert is not None:
         trino_url += f"&cert={quote_plus(cert)}"
 
     if key is not None:
```

### Comparing `trino-0.324.0/trino/transaction.py` & `trino-0.325.0/trino/transaction.py`

 * *Files identical despite different names*

### Comparing `trino-0.324.0/trino.egg-info/PKG-INFO` & `trino-0.325.0/trino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trino
-Version: 0.324.0
+Version: 0.325.0
 Summary: Client for the Trino distributed SQL Engine
 Home-page: https://github.com/trinodb/trino-python-client
 Author: Trino Team
 Author-email: python-client@trino.io
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trino-0.324.0/trino.egg-info/SOURCES.txt` & `trino-0.325.0/trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*


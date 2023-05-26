# Comparing `tmp/syncanyserver-0.0.1.tar.gz` & `tmp/syncanyserver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanyserver-0.0.1.tar", last modified: Fri May 12 09:56:21 2023, max compression
+gzip compressed data, was "syncanyserver-0.0.2.tar", last modified: Fri May 26 10:44:41 2023, max compression
```

## Comparing `syncanyserver-0.0.1.tar` & `syncanyserver-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:56:21.547690 syncanyserver-0.0.1/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.1/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-12 09:56:21.550691 syncanyserver-0.0.1/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.1/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-12 09:56:21.560690 syncanyserver-0.0.1/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2006 2023-05-12 08:09:59.000000 syncanyserver-0.0.1/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:56:21.214266 syncanyserver-0.0.1/syncanyserver/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-08 08:00:14.000000 syncanyserver-0.0.1/syncanyserver/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.1/syncanyserver/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1839 2023-05-12 08:53:07.000000 syncanyserver-0.0.1/syncanyserver/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    28582 2023-05-12 08:55:46.000000 syncanyserver-0.0.1/syncanyserver/server.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.1/syncanyserver/table.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2095 2023-05-12 08:39:46.000000 syncanyserver-0.0.1/syncanyserver/user.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:56:21.498671 syncanyserver-0.0.1/syncanyserver.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.1/syncanyserver.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      359 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-05-12 09:56:20.000000 syncanyserver-0.0.1/syncanyserver.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:41.128679 syncanyserver-0.0.2/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.2/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-26 10:44:41.130679 syncanyserver-0.0.2/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.2/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-26 10:44:41.140679 syncanyserver-0.0.2/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-26 07:24:05.000000 syncanyserver-0.0.2/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:40.750477 syncanyserver-0.0.2/syncanyserver/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-17 03:50:23.000000 syncanyserver-0.0.2/syncanyserver/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.2/syncanyserver/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.2/syncanyserver/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    31204 2023-05-26 09:48:39.000000 syncanyserver-0.0.2/syncanyserver/server.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.2/syncanyserver/table.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.2/syncanyserver/user.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:41.076686 syncanyserver-0.0.2/syncanyserver.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-05-26 10:44:40.000000 syncanyserver-0.0.2/syncanyserver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.2/syncanyserver.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/top_level.txt
```

### Comparing `syncanyserver-0.0.1/LICENSE` & `syncanyserver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.1/PKG-INFO` & `syncanyserver-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

### Comparing `syncanyserver-0.0.1/setup.py` & `syncanyserver-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.1"
+version = "0.0.2"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -33,16 +33,16 @@
     author='snower',
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
-        "sqlglot>=10.6.2",
-        "syncanysql>=0.1.3",
+        "sqlglot>=11.5.5,<12",
+        "syncanysql>=0.1.4",
         "mysql-mimic>=2.2.3"
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
         "openpyxl": ["openpyxl>=2.5.0"],
         "postgresql": ["psycopg2>=2.8.6"],
```

### Comparing `syncanyserver-0.0.1/syncanyserver/database.py` & `syncanyserver-0.0.2/syncanyserver/database.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.1/syncanyserver/main.py` & `syncanyserver-0.0.2/syncanyserver/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,21 +20,30 @@
         description="Simple and easy to use SQL scripts to build virtual database tables MySQL Server"
     )
     parser.add_argument('-b', "--bind", dest='bind', default="0.0.0.0", help='bind host (default: 0.0.0.0)')
     parser.add_argument('-p', "--port", dest='port', default=3306, type=int, help='bind port (default: 3306)')
     parser.add_argument('-c', "--config_path", dest='config_path', default=".", type=check_path,
                         help='The directory where the configuration file is located, '
                              'the default current directory (default: .)')
+    parser.add_argument('-U', "--username", dest='username', default="root", type=str,
+                        help='Login account name, invalid when configured with user.json'
+                             ' configuration file (default: root)')
+    parser.add_argument('-P', "--password", dest='password', default="", type=str,
+                        help='Login account password, invalid when configured with user.json'
+                             ' configuration file (default: )')
     parser.add_argument('-w', "--executor_max_workers", dest='executor_max_workers', default=5, type=int,
                         help='Maximum number of worker threads for ThreadPoolExecutor executing SQL '
                              'queries (default: 5)')
     parser.add_argument('-W', "--executor_wait_timeout", dest='executor_wait_timeout', default=120, type=int,
                         help='The maximum waiting seconds time before the SQL query task is submitted to '
                              'the ThreadPoolExecutor for execution (default: 120 seconds)')
     args = parser.parse_args()
+    if args.config_path:
+        os.chdir(os.path.abspath(args.config_path))
     asyncio.run(Server(args.bind, args.port, os.path.abspath(args.config_path),
+                       args.username, args.password,
                        args.executor_max_workers, args.executor_wait_timeout)
                 .serve_forever())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `syncanyserver-0.0.1/syncanyserver/server.py` & `syncanyserver-0.0.2/syncanyserver/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import sys
 import time
 from collections import defaultdict
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from sqlglot import expressions as sqlglot_expressions
 from mysql_mimic import Session, MysqlServer
+from mysql_mimic.errors import MysqlError, ErrorCode
+from mysql_mimic.intercept import expression_to_value
 from syncany.logger import get_logger
 from syncany.taskers.manager import TaskerManager
 from syncany.database.memory import MemoryDBCollection
 from syncanysql.compiler import Compiler
 from syncanysql.taskers.query import QueryTasker
 from syncanysql import ScriptEngine, Executor, ExecuterContext, SqlSegment, SqlParser, ExecuterError
 from syncanysql.parser import FileParser
@@ -137,14 +139,60 @@
                 if "show table status" in sql:
                     return [], ('Name', 'Engine', 'Version', 'Row_format', 'Rows', 'Avg_row_length', 'Data_length',
                                 'Max_data_length', 'Index_length', 'Data_free', 'Auto_increment', 'Create_time',
                                 'Update_time', 'Check_time', 'Collation', 'Checksum', 'Create_options', 'Comment')
                 return [], []
         return await super(ServerSession, self).handle_query(sql, attrs)
 
+    def _set_variable(self, setitem):
+        assignment = setitem.this
+        left = assignment.left
+
+        if isinstance(left, sqlglot_expressions.SessionParameter):
+            scope = left.text("kind") or "SESSION"
+            name = left.name
+        elif isinstance(left, sqlglot_expressions.Parameter):
+            scope = left.text("kind") or "GLOBAL"
+            name = left.name
+        else:
+            scope = setitem.text("kind") or "SESSION"
+            name = left.name
+
+        scope = scope.upper()
+        value = expression_to_value(assignment.right)
+
+        if scope in {"SESSION", "LOCAL"}:
+            self.variables.set(name, value)
+        if self.executer_context:
+            with self.executer_context as executer_context:
+                try:
+                    with executer_context.executor as executor:
+                        executor.run("session[%d-%d]" % (id(self), self.execute_index),
+                                     [SqlSegment("set " + str(setitem), 1)])
+                        exit_code = executor.execute()
+                        if exit_code is not None and exit_code != 0:
+                            raise ExecuterError(exit_code)
+                except Exception as e:
+                    raise MysqlError(str(e), code=ErrorCode.NOT_SUPPORTED_YET)
+        else:
+            raise MysqlError(
+                f"Cannot SET variable {name} with scope {scope}",
+                code=ErrorCode.NOT_SUPPORTED_YET,
+            )
+
+    async def _static_query_interceptor(self, expression):
+        try:
+            if isinstance(expression, sqlglot_expressions.Select) and \
+                    not any(expression.args.get(a)
+                            for a in set(sqlglot_expressions.Select.arg_types) - {"expressions", "limit", "hint"}):
+                return await self.query(expression, str(expression), {})
+            return None
+        except Exception:
+            return super(ServerSession, self)._static_query_interceptor(expression)
+
     async def query(self, expression, sql, attrs):
         if not isinstance(expression, (sqlglot_expressions.Insert, sqlglot_expressions.Delete,
                                        sqlglot_expressions.Select, sqlglot_expressions.Union)):
             if sql.lower().startswith("flush"):
                 await self.loop.run_in_executor(self.thread_pool_executor, self.identity_provider.load_users)
                 await self.loop.run_in_executor(self.thread_pool_executor, Database.scan_databases,
                                                 self.config_path, self.executer_context.engine, self.databases)
@@ -163,14 +211,23 @@
                               (time.time() - start_time) * 1000)
 
     def execute_query(self, expression, start_time):
         executor_wait_timeout = self.variables.values.get("wait_timeout") or self.executor_wait_timeout
         if start_time + int(executor_wait_timeout) <= time.time():
             raise TimeoutError("query execute wait timeout")
 
+        if expression.args.get("into"):
+            with self.executer_context as executer_context:
+                executer_context.session = self
+                try:
+                    executer_context.execute_expression(expression)
+                finally:
+                    executer_context.session = None
+            return [], []
+
         with self.executer_context.context(self) as executer_context:
             primary_tables = self.parse_primary_tables(expression, defaultdict(list))
             if primary_tables:
                 self.execute_tables(executer_context, primary_tables, self.parse_primary_variable_sqls(expression))
             joins_tables = self.parse_join_tables(expression, defaultdict(list))
             if joins_tables:
                 self.execute_tables(executer_context, joins_tables, self.parse_joins_variable_sqls(expression))
@@ -425,16 +482,18 @@
                 continue
             if self.has_column(child_expression):
                 return True
         return False
 
 
 class Server(MysqlServer):
-    def __init__(self, host=None, port=3306, config_path=".", executor_max_workers=5, executor_wait_timeout=120):
-        super(Server, self).__init__(session_factory=self.create_session, identity_provider=UserIdentityProvider())
+    def __init__(self, host=None, port=3306, config_path=".", username=None, password=None,
+                 executor_max_workers=5, executor_wait_timeout=120):
+        super(Server, self).__init__(session_factory=self.create_session,
+                                     identity_provider=UserIdentityProvider(config_path, username, password))
 
         self.host = host
         self.port = port
         self.config_path = config_path
         self.executor_max_workers = executor_max_workers
         self.executor_wait_timeout = executor_wait_timeout
         self.script_engine = None
```

### Comparing `syncanyserver-0.0.1/syncanyserver/table.py` & `syncanyserver-0.0.2/syncanyserver/table.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.1/syncanyserver/user.py` & `syncanyserver-0.0.2/syncanyserver/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 import os
 from syncany.logger import get_logger
 from mysql_mimic import IdentityProvider, NativePasswordAuthPlugin, User
 from syncany.taskers.config import load_config
 
 
 class UserIdentityProvider(IdentityProvider):
-    def __init__(self, config_path="."):
+    def __init__(self, config_path=".", username=None, password=None):
         self.config_path = config_path
+        self.username = username
+        self.password = password
         self.users = None
 
     def get_plugins(self):
         return [NativePasswordAuthPlugin()]
 
     async def get_user(self, username):
         if self.users is None:
@@ -49,9 +51,11 @@
                 config_users = config
             if not config_users:
                 continue
             for user in config_users:
                 if not isinstance(user, dict) or "username" not in user or "password" not in user:
                     continue
                 users[user["username"]] = user
+        if not users and self.username:
+            users[self.username] = {"username": self.username, "password": self.password}
         self.users = users
         get_logger().info("load users finish, users: %s", ",".join(list(users.keys())))
```

### Comparing `syncanyserver-0.0.1/syncanyserver.egg-info/PKG-INFO` & `syncanyserver-0.0.2/syncanyserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```


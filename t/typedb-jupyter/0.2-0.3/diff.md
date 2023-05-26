# Comparing `tmp/typedb-jupyter-0.2.tar.gz` & `tmp/typedb-jupyter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedb-jupyter-0.2.tar", last modified: Thu May  4 18:30:10 2023, max compression
+gzip compressed data, was "typedb-jupyter-0.3.tar", last modified: Fri May 26 10:19:04 2023, max compression
```

## Comparing `typedb-jupyter-0.2.tar` & `typedb-jupyter-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-04 18:30:10.461055 typedb-jupyter-0.2/
--rw-r--r--   0 jameswhiteside   (502) staff       (20)    32386 2023-04-20 13:54:26.000000 typedb-jupyter-0.2/LICENSE
--rw-r--r--   0 jameswhiteside   (502) staff       (20)    47015 2023-05-04 18:30:10.460697 typedb-jupyter-0.2/PKG-INFO
--rw-r--r--   0 jameswhiteside   (502) staff       (20)     8956 2023-05-04 18:25:40.000000 typedb-jupyter-0.2/README.md
--rw-r--r--   0 jameswhiteside   (502) staff       (20)      857 2023-05-04 17:52:51.000000 typedb-jupyter-0.2/pyproject.toml
--rw-r--r--   0 jameswhiteside   (502) staff       (20)       38 2023-05-04 18:30:10.461201 typedb-jupyter-0.2/setup.cfg
-drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-04 18:30:10.455617 typedb-jupyter-0.2/src/
-drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-04 18:30:10.458572 typedb-jupyter-0.2/src/tql/
--rw-r--r--   0 jameswhiteside   (502) staff       (20)      105 2023-05-04 18:23:01.000000 typedb-jupyter-0.2/src/tql/__init__.py
--rw-r--r--   0 jameswhiteside   (502) staff       (20)     4750 2023-05-04 18:06:15.000000 typedb-jupyter-0.2/src/tql/connection.py
--rw-r--r--   0 jameswhiteside   (502) staff       (20)       90 2023-04-20 13:54:26.000000 typedb-jupyter-0.2/src/tql/exception.py
--rw-r--r--   0 jameswhiteside   (502) staff       (20)     4845 2023-05-04 17:50:22.000000 typedb-jupyter-0.2/src/tql/magic.py
--rw-r--r--   0 jameswhiteside   (502) staff       (20)     7075 2023-05-04 17:36:07.000000 typedb-jupyter-0.2/src/tql/query.py
-drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-04 18:30:10.460173 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/
--rw-r--r--   0 jameswhiteside   (502) staff       (20)    47015 2023-05-04 18:30:10.000000 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 jameswhiteside   (502) staff       (20)      338 2023-05-04 18:30:10.000000 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 jameswhiteside   (502) staff       (20)        1 2023-05-04 18:30:10.000000 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 jameswhiteside   (502) staff       (20)       28 2023-05-04 18:30:10.000000 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/requires.txt
--rw-r--r--   0 jameswhiteside   (502) staff       (20)        4 2023-05-04 18:30:10.000000 typedb-jupyter-0.2/src/typedb_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-26 10:19:04.946062 typedb-jupyter-0.3/
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)    10172 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/LICENSE
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)    22533 2023-05-26 10:19:04.945399 typedb-jupyter-0.3/PKG-INFO
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)    10148 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/README.md
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)      933 2023-05-26 10:11:15.000000 typedb-jupyter-0.3/pyproject.toml
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)       38 2023-05-26 10:19:04.946217 typedb-jupyter-0.3/setup.cfg
+drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-26 10:19:04.940035 typedb-jupyter-0.3/src/
+drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-26 10:19:04.942681 typedb-jupyter-0.3/src/typedb_jupyter/
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)      986 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/src/typedb_jupyter/__init__.py
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)     5666 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/src/typedb_jupyter/connection.py
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)      911 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/src/typedb_jupyter/exception.py
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)     7839 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/src/typedb_jupyter/magic.py
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)    11703 2023-05-25 18:11:23.000000 typedb-jupyter-0.3/src/typedb_jupyter/query.py
+drwxr-xr-x   0 jameswhiteside   (502) staff       (20)        0 2023-05-26 10:19:04.944533 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)    22533 2023-05-26 10:19:04.000000 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)      393 2023-05-26 10:19:04.000000 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)        1 2023-05-26 10:19:04.000000 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)       28 2023-05-26 10:19:04.000000 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/requires.txt
+-rw-r--r--   0 jameswhiteside   (502) staff       (20)       15 2023-05-26 10:19:04.000000 typedb-jupyter-0.3/src/typedb_jupyter.egg-info/top_level.txt
```

### Comparing `typedb-jupyter-0.2/README.md` & `typedb-jupyter-0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,271 +1,280 @@
 # TypeDB Jupyter connector
 
-Runs TypeQL statements against a TypeDB database from a Jupyter notebook
-using the `%tql` IPython magic command.
+Runs TypeQL statements against a TypeDB database from a Jupyter notebook using the `%typedb` and `%typeql` IPython magic
+commands. Includes:
+- Full support for TypeDB Core and Cluster.
+- Ability to manage multiple concurrent connections.
+- Automatic session and transaction handling.
+- JSON-style output for all read queries.
+- Variable interpolation from the Jupyter namespace.
+- Query reading from supplied filepaths.
 
 ## Getting started
 
 Install this module with:
 
 ```
 pip install typedb-jupyter
 ```
 
 or your environment equivalent. Load the extension in Jupyter with:
 
 ```
-%load_ext tql
+%load_ext typedb_jupyter
 ```
 
 ## Connecting to TypeDB
 
 Establish a connection with:
 
 ```
-%tql -d <database name> [-a <server address>] [-n <connection name>]
+%typedb -d <database name> [-a <server address>] [-n <connection alias>]
 ```
 
 for example:
 
 ```
-In [1]: %tql -a 111.111.111.111:1729 -d database_1
+In [1]: %typedb -a 111.111.111.111:1729 -d database_1
 
 Out[1]: Opened connection: database_1@111.111.111.111:1729
 ```
 
 
 ```
-In [2]: %tql -a 222.222.222.222:1729 -d database_2 -n test_connection
+In [2]: %typedb -a 222.222.222.222:1729 -d database_2 -n test_connection
 
 Out[2]: Opened connection: test_connection (database_2@222.222.222.222:1729)
 ```
 
 
 ```
-In [3]: %tql -d database_local
+In [3]: %typedb -d database_local
 
 Out[3]: Opened connection: database_local@localhost:1729
 ```
 
-If no address is provided, the default `localhost:1729` will be used. If
-no connection name is provided, the connection will be assigned a name
-of the format `<database name>@<server address>`. If a connection with
-the server is established but no database with the name provided exists,
-a new database will be created with that name. Only one connection can
-be opened to each database at a time.
+If no address is provided, the default `localhost:1729` will be used. If no custom alias is provided, the connection
+will be assigned a default alias of the format `<database name>@<server address>`. Custom aliases can only include
+alphanumeric characters, hyphens, and underscores. If a connection with the server is established but no database with
+the name provided exists, a new database will be created with that name by default. Only one connection can be opened to
+each database at a time.
+
+For connecting to TypeDB Cluster, use:
+
+```
+%typedb -d <database name> -a <server address> -u <username> -p <password> -c <certificate path> [-n <connection alias>]
+```
 
 List established connections with:
 
 ```
-In [4]: %tql -l
+In [4]: %typedb -l
 
 Out[4]: Open connections:
    ...:    database_1@111.111.111.111:1729
    ...:    test_connection (database_2@222.222.222.222:1729)
    ...:  * database_local@localhost:1729
 ```
 
-An asterisk appears next to the currently selected connection, which is
-the last one opened by default. To change the selected connection, use:
+An asterisk appears next to the currently selected connection, which is the last one opened by default. To change the
+selected connection, use:
 
 ```
-%tql -n <connection name>
+%typedb -n <connection alias>
 ```
 
 for example:
 
 ```
-In [5]: %tql -n database_1@111.111.111.111:1729
+In [5]: %typedb -n database_1@111.111.111.111:1729
 
 Out[5]: Selected connection: database_1@111.111.111.111:1729
 ```
 
 ```
-In [6]: %tql -n test_connection
+In [6]: %typedb -n test_connection
 
 Out[6]: Selected connection: test_connection
 ```
 
 Close a connection with:
 
 ```
-%tql -c <connection name>
+%typedb -k <connection name>
 ```
 
 for example:
 
 ```
-In [7]: %tql -c database_2@222.222.222.222:1729
+In [7]: %typedb -c database_2@222.222.222.222:1729
 
 Out[7]: Closed connection: database_2@222.222.222.222:1729
 ```
 
-If the currently selected connection is closed, a new one must be
-manually selected. Using `-k` instead of `-c` will also delete the
-database.
+If the currently selected connection is closed, a new one must be manually selected before queries can be executed.
+Using `-x` instead of `-k` will also delete the database.
 
 ## Executing a query
 
-Run a query against the database using the selected connection with:
+Run a query against a database using the selected connection with:
 
 ```
-%tql <tql>
+%typeql <typeql string>
 ```
 
 or
 
 ```
-%%tql <multiline tql>
+%%typeql <multiline typeql string>
 ```
 
 For example:
 
 ```
-In [8]: %tql match $p isa person;
+In [8]: %typeql match $p isa person;
 
 Out[8]: [{'p': {'type': 'person'}},
    ...:  {'p': {'type': 'person'}}]
 ```
 
 ```
-In [9]: %%tql
+In [9]: %%typeql
    ...: match
    ...:   $p isa person,
    ...:   has name $n,
    ...:   has age $a;
 
 Out[9]: [{'a': {'type': 'age', 'value_type': 'long', 'value': 30},
    ...:   'p': {'type': 'person'},
    ...:   'n': {'type': 'name', 'value_type': 'string', 'value': 'Kevin'}},
    ...:  {'a': {'type': 'age', 'value_type': 'long', 'value': 50},
    ...:   'p': {'type': 'person'},
    ...:   'n': {'type': 'name', 'value_type': 'string', 'value': 'Gavin'}}]
 ```
 
-Results of read queries are returned in a JSON-like native Python
-object. The shape of the object is dependent on the type of query, as
-described in the following table:
-
-| Query type              | Output object type     |
-|-------------------------|------------------------|
-| `match`                 | `list<dict>`           |
-| `match-group`           | `dict<list<dict>>`     |
-| `match-aggregate`       | `int&#124;float`       |
-| `match-group-aggregate` | `dict<int&#124;float>` |
-
-A connection can be opened or selected in the same call it is utilised with
-`-d`, `-a`, and `-n` as specified above. Queries automatically interpolate
-variables from the notebook's Python namespace, specified using the syntax
+Results of read queries are returned in a JSON-like native Python object. The shape of the object is dependent on the
+type of query, as described in the following table:
+
+| Query type              | Output object type |
+|-------------------------|--------------------|
+| `match`                 | `list<dict>`       |
+| `match-group`           | `dict<list<dict>>` |
+| `match-aggregate`       | `intǀfloat`        |
+| `match-group-aggregate` | `dict<intǀfloat>`  |
+
+Queries automatically interpolate variables from the notebook's Python namespace, specified using the syntax
 `{<variable name>}`, for example:
 
 ```
 In [10]: age = 30
 
-In [11]: %tql match $p isa person, has name $n, has age {age}; count;
+In [11]: %typeql match $p isa person, has name $n, has age {age}; count;
 
 Out[11]: 1
 ```
 
-Similarly, results can be saved to a namespace variable by providing the variable
-name with:
+Similarly, results can be saved to a namespace variable by providing the variable name with:
 
 ```
-%tql -r <variable name> <tql>
+%typeql -r <variable name> <typeql string>
 ```
 
 for example:
 
 ```
-In [12]: %tql -r name_counts match $p isa person, has name $n, has age $a; group $n; count;
+In [12]: %typeql -r name_counts match $p isa person, has name $n, has age $a; group $n; count;
 
 In [13]: name_counts
 
 Out[13]: {'Gavin': 1, 'Kevin': 1}
 ```
 
 To execute a query in a stored TypeQL file, supply the filepath with:
 
 ```
-%tql -f <file path>
+%typeql -f <file path>
 ```
 
 Rule inference is disabled by default. It can be enabled for a query with:
 
 ```
-%tql -i True <tql>
+%typeql -i True <typeql string>
 ```
 
 In order to enable rule inference globally, see the [Configuring options](#configuring-options)
 section below.
 
 ## Information for advanced users
 
-Queries are syntactically analysed to automatically
-determine schema and transaction types, but these can be
-overridden with:
-
-```
-%tql [-s <session type>] [-t <transaction type>] <tql>
-```
-
-where `<session type>` is either `schema` or `data`, and `<transaction type>`
-is either `read` or `write`.
-
-When a connection is instantiated, a data
-session is opened and persisted for the duration of the connection unless the
-required session type changes. Each call of `%tql` or `%%tql` is executed in
-a new transaction, which is then immediately closed on completion. If a query
-is executed requiring a different session type to the one open, the open
-session is closed and a new one of the correct type is opened and persisted.
-All sessions and clients are closed automatically when the notebook's kernel
-is terminated. Note that opening a schema session to a TypeDB server requires
-that no other sessions be open, regardless of the client used, and once open,
-no other sessions can be opened on the server until the schema session is closed.
+Queries are syntactically analysed to automatically determine schema and transaction types, but these can be overridden
+with:
+
+```
+%typeql [-s <session type>] [-t <transaction type>] <typeql string>
+```
+
+where `<session type>` is either `schema` or `data`, and `<transaction type>` is either `read` or `write`.
+
+When a connection is instantiated, a data session is opened and persisted for the duration of the connection unless a
+schema query is issued, at which point the data session is closed and a schema session is opened. After the schema query
+has been executed, the schema session is then closed and a new data session opened. Each call of `%typeql` or `%%typeql`
+is executed in a new transaction, which is then immediately closed on completion. All clients, sessions, and
+transactions are closed automatically when the notebook's kernel is terminated.
+
+It is important to note that TypeDB sessions and transactions cannot be opened under certain conditions, regardless of
+the client:
+
+- Only one schema session can be opened at any time.
+- Data write transactions cannot be opened while a schema session is open.
+- Only one schema write transaction can be opened at any time.
+
+This means that, when a `define` or `undefine` query is executed in a notebook, this will interfere with queries
+performed by other users on the same database.
 
 ## Configuring options
 
 Certain options can be configured using the `%config` magic with:
 
 ```
 %config <config argument>`
 ```
 
 After being set, these options persist for the remainder of the notebook unless
 changed again. The following table describes the available arguments:
 
-| Argument                                 | Usage                                                                         | Default |
-|------------------------------------------|-------------------------------------------------------------------------------|---------|
-| `TQLMagic`                               | List config options and current set values.                                   |         |
-| `TQLMagic.create_database=<boolean>`     | Create database when opening a connection if it does not already exist.       | `True`  |
-| `TQLMagic.global_inference=<boolean>`    | Enable rule inference for all queries. Can be overridden per query with `-i`. | `False` |
-| `TQLMagic.show_connection=<boolean>`     | Always show current connection name when executing a query.                   | `True`  |
-| `TQLMagic.strict_transactions=<boolean>` | Require session and transaction types to be specified for every transaction.  | `False` |
+| Argument                                      | Usage                                                                         | Default |
+|-----------------------------------------------|-------------------------------------------------------------------------------|---------|
+| `TypeDBMagic`                                 | List config options and current set values for `%typedb`.                     |         |
+| `TypeDBMagic.create_database = <boolean>`     | Create database when opening a connection if it does not already exist.       | `True`  |
+| `TypeQLMagic`                                 | List config options and current set values for `%typeql`.                     |         |
+| `TypeQLMagic.global_inference = <boolean>`    | Enable rule inference for all queries. Can be overridden per query with `-i`. | `False` |
+| `TypeQLMagic.show_info = <boolean>`           | Always show full connection information when executing a query.               | `True`  |
+| `TypeQLMagic.strict_transactions = <boolean>` | Require session and transaction types to be specified for every transaction.  | `False` |
 
 ## Command glossary 
 
-The following tables list the arguments that can be provided to the `%tql` magic command:
-
-| Argument                | Usage                                                                         | Argument type        |
-|-------------------------|-------------------------------------------------------------------------------|----------------------|
-| `-a <server address>`   | TypeDB server address for new connection.                                     | Connection argument. |
-| `-d <database name>`    | Database name for new connection.                                             | Connection argument. |
-| `-n <connection name>`  | Custom name for new connection, or name of existing connection to select.     | Connection argument. |
-| `-l`                    | List currently open connections.                                              | Connection argument. |
-| `-c <connection name>`  | Close a connection by name.                                                   | Connection argument. |
-| `-k <connection name>`  | Close a connection by name and delete its database.                           | Connection argument. |
-| `-p <thread count>`     | Number of server communication threads for new connection (advanced feature). | Connection argument. |
-| `-r <variable name>`    | Assign query result to the named variable instead of printing.                | Query argument.      |
-| `-f <file path>`        | Read in query from a TypeQL file at the specified path.                       | Query argument.      |
-| `-i <inference option>` | Enable (`True`) or disable (`False`) rule inference for query.                | Query argument.      |
-| `-s <session type>`     | Force a particular session type for query, `schema` or `data`.                | Query argument.      |
-| `-t <transaction type>` | Force a particular transaction type for query, `read` or `write`.             | Query argument.      |
-
-
+The following tables list the arguments that can be provided to the `%typedb` and `%typeql` magic commands:
 
+| Magic command | Argument                | Usage                                                                       |
+|---------------|-------------------------|-----------------------------------------------------------------------------|
+| `%typedb`     | `-a <server address>`   | TypeDB server address for new connection.                                   |
+| `%typedb`     | `-d <database name>`    | Database name for new connection.                                           |
+| `%typedb`     | `-u <username>`         | Username for new Cloud/Cluster connection.                                  |
+| `%typedb`     | `-p <password>`         | Password for new Cloud/Cluster connection.                                  |
+| `%typedb`     | `-c <certificate path>` | TLS certificate path for new Cloud/Cluster connection.                      |
+| `%typedb`     | `-n <connection alias>` | Custom alias for new connection, or alias of existing connection to select. |
+| `%typedb`     | `-l`                    | List currently open connections.                                            |
+| `%typedb`     | `-k <connection name>`  | Close a connection by name.                                                 |
+| `%typedb`     | `-x <connection name>`  | Close a connection by name and delete its database.                         |
+| `%typeql`     | `-r <variable name>`    | Assign query result to the named variable instead of printing.              |
+| `%typeql`     | `-f <file path>`        | Read in query from a TypeQL file at the specified path.                     |
+| `%typeql`     | `-i <inference option>` | Enable (`True`) or disable (`False`) rule inference for query.              |
+| `%typeql`     | `-s <session type>`     | Force a particular session type for query, `schema` or `data`.              |
+| `%typeql`     | `-t <transaction type>` | Force a particular transaction type for query, `read` or `write`.           |
 
 ## Planned features
 
 - Add option to close all connections.
 - Add more output formats.
 
 ## Acknowledgements
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typedb-jupyter-0.2/src/tql/query.py` & `typedb-jupyter-0.3/src/typedb_jupyter/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,298 @@
+#
+# Copyright (C) 2023 Vaticle
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+#
+
 import math
-import typedb.client
+from typedb.client import TypeDBOptions
 from typedb.api.connection.session import SessionType
 from typedb.api.connection.transaction import TransactionType
-from typedb.common.exception import TypeDBClientException
 from typedb.concept.answer.concept_map import ConceptMap
 from typedb.concept.answer.concept_map_group import ConceptMapGroup
 from typedb.concept.answer.numeric import Numeric
 from typedb.concept.answer.numeric_group import NumericGroup
-from tql.exception import ArgumentError, QueryParsingError
+from typedb_jupyter.connection import Connection
+from typedb_jupyter.exception import ArgumentError, QueryParsingError
+
+
+class Query(object):
+    def __init__(self, query, session_arg, transaction_arg, inference_arg, strict_transactions, global_inference):
+        self.query = query
+        self.query_type = self._get_query_type(self.query)
+        self.session_type = self._get_session_type(self.query_type, session_arg, strict_transactions)
+        self.transaction_type = self._get_transaction_type(self.query_type, transaction_arg, strict_transactions)
+
+        if inference_arg is None:
+            self.infer = global_inference
+        else:
+            self.infer = inference_arg
+
+    @staticmethod
+    def _get_query_args(query):
+        # Warning: This method is experimental and not guaranteed to always function correctly. Copy at your own risk.
+
+        in_escape = False
+        in_literal = False
+        in_comment = False
+        literal_delimiter = None
+        arg_string = ""
+
+        for char in query:
+            if in_escape:
+                in_escape = False
+                arg_string += " "
+                continue
+
+            if in_literal and char == "\\":
+                in_escape = True
+                arg_string += " "
+                continue
+
+            if not in_comment and char in ("\"", "'"):
+                if not in_literal:
+                    in_literal = True
+                    literal_delimiter = char
+                    arg_string += " "
+                    continue
+                if in_literal and char == literal_delimiter:
+                    in_literal = False
+                    arg_string += " "
+                    continue
+
+            if not in_literal:
+                if char == "#":
+                    in_comment = True
+                    arg_string += " "
+                    continue
+                if in_comment and char == "\n":
+                    in_comment = False
+                    arg_string += " "
+                    continue
+
+            if not in_literal and not in_comment:
+                if char in (",", ";"):
+                    arg_string += " "
+                else:
+                    arg_string += char
+
+        return arg_string.split()
+
+    @staticmethod
+    def _get_query_type(query):
+        # Warning: This method is experimental and not guaranteed to always function correctly. Copy at your own risk.
+
+        query_args = Query._get_query_args(query)
+
+        keyword_counts = {
+            "match": 0,
+            "get": 0,
+            "define": 0,
+            "undefine": 0,
+            "insert": 0,
+            "delete": 0,
+            "group": 0,
+            "count": 0,
+            "sum": 0,
+            "max": 0,
+            "min": 0,
+            "mean": 0,
+            "median": 0,
+            "std": 0,
+        }
+
+        for arg in query_args:
+            if arg in keyword_counts:
+                keyword_counts[arg] += 1
+
+        aggregate_count = sum((
+            keyword_counts["count"],
+            keyword_counts["sum"],
+            keyword_counts["max"],
+            keyword_counts["min"],
+            keyword_counts["mean"],
+            keyword_counts["median"],
+            keyword_counts["std"],
+        ))
+
+        candidate_query_types = list()
+
+        if keyword_counts["group"] > 0 and aggregate_count > 0:
+            candidate_query_types.append("match-group-aggregate")
+        elif aggregate_count > 0:
+            candidate_query_types.append("match-aggregate")
+        elif keyword_counts["group"] > 0:
+            candidate_query_types.append("match-group")
+        elif keyword_counts["get"] > 0:
+            candidate_query_types.append("match")
+
+        if keyword_counts["define"] > 0:
+            candidate_query_types.append("define")
+
+        if keyword_counts["undefine"] > 0:
+            candidate_query_types.append("undefine")
+
+        if keyword_counts["insert"] > 0 and keyword_counts["delete"] > 0:
+            candidate_query_types.append("update")
+        elif keyword_counts["insert"] > 0:
+            candidate_query_types.append("insert")
+        elif keyword_counts["delete"] > 0:
+            candidate_query_types.append("delete")
+
+        if len(candidate_query_types) > 1:
+            raise QueryParsingError("Query contains incompatible keywords: '{}'".format("', '".join(candidate_query_types)))
+        elif len(candidate_query_types) == 1:
+            return candidate_query_types[0]
+        elif keyword_counts["match"] > 0:
+            return "match"
+        else:
+            raise QueryParsingError("Query contains no keywords.")
 
+    @staticmethod
+    def _get_session_type(query_type, session_arg, strict_transactions):
+        if session_arg is None:
+            if strict_transactions:
+                raise ArgumentError("Strict transaction types is enabled and no session type was provided. Use -s to specify session type.")
+            elif query_type in ("define", "undefine"):
+                return SessionType.SCHEMA
+            else:
+                return SessionType.DATA
+        else:
+            if session_arg.lower() == "schema":
+                return SessionType.SCHEMA
+            elif session_arg.lower() == "data":
+                return SessionType.DATA
+            else:
+                raise ArgumentError("Incorrect session type provided. Session type must be 'schema' or 'data'.")
 
-def group_key(concept):
-    if concept.is_type():
-        return str(concept.as_type().get_label())
-    elif concept.is_entity():
-        return concept.as_entity().get_iid()
-    elif concept.is_relation():
-        return concept.as_relation().get_iid()
-    elif concept.is_attribute():
-        return concept.as_attribute().get_value()
-    else:
-        raise ValueError("Unknown concept type. Please report this error.")
-
-
-def decode(answer, answer_type):
-    if answer_type is ConceptMap:
-        return [concept_map.to_json() for concept_map in answer]
-    elif answer_type is ConceptMapGroup:
-        return {group_key(map_group.owner()): decode(map_group.concept_maps(), ConceptMap) for map_group in answer}
-    elif answer_type is Numeric:
-        if answer.is_int():
-            return answer.as_int()
-        elif answer.is_float():
-            return answer.as_float()
-        else:
-            return math.nan
-    elif answer_type is NumericGroup:
-        return {group_key(numeric_group.owner()): decode(numeric_group.numeric(), Numeric) for numeric_group in answer}
-    else:
-        raise ValueError("Unknown answer type. Please report this error.")
-
-
-def run(connection, query, args, strict_transactions, global_inference):
-    query = query.strip()
-
-    if len(query) == 0:
-        return
-
-    query_args = "".join(query.split("\"")[::2]).replace(";", "").split()
-
-    keyword_counts = {
-        "match": 0,
-        "get": 0,
-        "define": 0,
-        "undefine": 0,
-        "insert": 0,
-        "delete": 0,
-        "group": 0,
-        "count": 0,
-        "sum": 0,
-        "max": 0,
-        "min": 0,
-        "mean": 0,
-        "median": 0,
-        "std": 0,
-    }
-
-    for arg in query_args:
-        if arg in keyword_counts:
-            keyword_counts[arg] += 1
-
-    aggregate_count = sum((
-        keyword_counts["count"],
-        keyword_counts["sum"],
-        keyword_counts["max"],
-        keyword_counts["min"],
-        keyword_counts["mean"],
-        keyword_counts["median"],
-        keyword_counts["std"],
-    ))
-
-    candidate_query_types = list()
-
-    if keyword_counts["group"] > 0 and aggregate_count > 0:
-        candidate_query_types.append("match_group_aggregate")
-    elif aggregate_count > 0:
-        candidate_query_types.append("match_aggregate")
-    elif keyword_counts["group"] > 0:
-        candidate_query_types.append("match_group")
-    elif keyword_counts["get"] > 0:
-        candidate_query_types.append("match")
-
-    if keyword_counts["define"] > 0:
-        candidate_query_types.append("define")
-
-    if keyword_counts["undefine"] > 0:
-        candidate_query_types.append("undefine")
-
-    if keyword_counts["insert"] > 0 and keyword_counts["delete"] > 0:
-        candidate_query_types.append("update")
-    elif keyword_counts["insert"] > 0:
-        candidate_query_types.append("insert")
-    elif keyword_counts["delete"] > 0:
-        candidate_query_types.append("delete")
-
-    if len(candidate_query_types) > 1:
-        raise QueryParsingError("Query contains incompatible keywords: '{}'".format("', '".join(candidate_query_types)))
-    elif len(candidate_query_types) == 1:
-        query_type = candidate_query_types[0]
-    elif keyword_counts["match"] > 0:
-        query_type = "match"
-    else:
-        raise QueryParsingError("Query contains no keywords.")
-
-    if args.session is None:
-        if strict_transactions:
-            raise ArgumentError("Strict transaction types is enabled and no session type was provided. Use -s to specify session type.")
-        elif query_type in ("define", "undefine"):
-            session_type = SessionType.SCHEMA
-        else:
-            session_type = SessionType.DATA
-    else:
-        if args.session.lower() == "schema":
-            session_type = SessionType.SCHEMA
-        elif args.session.lower() == "data":
-            session_type = SessionType.DATA
-        else:
-            raise ArgumentError("Incorrect session type provided. Session type must be 'schema' or 'data'.")
-
-    if args.transaction is None:
-        if strict_transactions:
-            raise ArgumentError("Strict transaction types is enabled and no transaction type was provided. Use -t to specify transaction type.")
-        elif query_type in ("define", "undefine", "insert", "update", "delete"):
-            transaction_type = TransactionType.WRITE
-        else:
-            transaction_type = TransactionType.READ
-    else:
-        if args.transaction.lower() == "read":
-            transaction_type = TransactionType.READ
-        elif args.transaction.lower() == "write":
-            transaction_type = TransactionType.WRITE
-        else:
-            raise ArgumentError("Incorrect transaction type provided. Transaction type must be 'read' or 'write'.")
-
-    if args.inference is None:
-        options = typedb.client.TypeDBOptions().core().set_infer(global_inference)
-    else:
-        options = typedb.client.TypeDBOptions().core().set_infer(args.inference)
-
-    connection.set_session(session_type)
-
-    try:
-        with connection.session.transaction(transaction_type, options) as transaction:
-            if query_type == "match":
-                results = decode(transaction.query().match(query), ConceptMap)
-            elif query_type == "match_aggregate":
-                results = decode(transaction.query().match_aggregate(query).get(), Numeric)
-            elif query_type == "match_group":
-                results = decode(transaction.query().match_group(query), ConceptMapGroup)
-            elif query_type == "match_group_aggregate":
-                results = decode(transaction.query().match_group_aggregate(query), NumericGroup)
-            elif query_type == "define":
-                transaction.query().define(query)
-            elif query_type == "undefine":
-                transaction.query().undefine(query)
-            elif query_type == "insert":
-                transaction.query().insert(query)
-            elif query_type == "delete":
-                transaction.query().delete(query)
-            elif query_type == "update":
-                transaction.query().update(query)
-
-            if transaction_type == TransactionType.WRITE:
-                transaction.commit()
-                print('{} query success.'.format(query_type.title()))
-                return
+    @staticmethod
+    def _get_transaction_type(query_type, transaction_arg, strict_transactions):
+        if transaction_arg is None:
+            if strict_transactions:
+                raise ArgumentError("Strict transaction types is enabled and no transaction type was provided. Use -t to specify transaction type.")
+            elif query_type in ("define", "undefine", "insert", "update", "delete"):
+                return TransactionType.WRITE
             else:
-                return results
-    except TypeDBClientException as exception:
-        if session_type == SessionType.SCHEMA:
-            print('Switching to data session due to failed schema query.')
-            connection.set_session(SessionType.DATA)
+                return TransactionType.READ
+        else:
+            if transaction_arg.lower() == "read":
+                return TransactionType.READ
+            elif transaction_arg.lower() == "write":
+                return TransactionType.WRITE
+            else:
+                raise ArgumentError("Incorrect transaction type provided. Transaction type must be 'read' or 'write'.")
+
+    def _get_options(self, connection):
+        if connection.client.is_cluster():
+            return TypeDBOptions().cluster().set_infer(self.infer)
+        else:
+            return TypeDBOptions().core().set_infer(self.infer)
+
+    def _print_info(self, connection):
+        connection_arg = "Connection: {}".format(connection.verbose_name)
+
+        if self.session_type == SessionType.SCHEMA:
+            session_arg = "Session: schema"
+        else:
+            session_arg = "Session: data"
+
+        if self.transaction_type == TransactionType.READ:
+            transaction_arg = "Transaction: read"
+        else:
+            transaction_arg = "Transaction: write"
+
+        query_arg = "Query: {}".format(self.query_type)
+
+        if self.infer:
+            inference_arg = "Inference: on"
+        else:
+            inference_arg = "Inference: off"
+
+        info = "{}\n{}\n{}\n{}\n{}".format(
+            connection_arg, session_arg, transaction_arg, query_arg, inference_arg
+        )
+
+        print(info)
+
+    @staticmethod
+    def _group_key(concept):
+        if concept.is_type():
+            return str(concept.as_type().get_label())
+        elif concept.is_entity():
+            return concept.as_entity().get_iid()
+        elif concept.is_relation():
+            return concept.as_relation().get_iid()
+        elif concept.is_attribute():
+            return concept.as_attribute().get_value()
+        else:
+            raise ValueError("Unknown concept type. Please report this error.")
+
+    @staticmethod
+    def _parse_answer(answer, answer_type):
+        if answer_type is ConceptMap:
+            return [concept_map.to_json() for concept_map in answer]
+        elif answer_type is ConceptMapGroup:
+            return {Query._group_key(map_group.owner()): Query._parse_answer(map_group.concept_maps(), ConceptMap) for map_group in answer}
+        elif answer_type is Numeric:
+            if answer.is_int():
+                return answer.as_int()
+            elif answer.is_float():
+                return answer.as_float()
+            else:
+                return math.nan
+        elif answer_type is NumericGroup:
+            return {Query._group_key(numeric_group.owner()): Query._parse_answer(numeric_group.numeric(), Numeric) for numeric_group in answer}
+        else:
+            raise ValueError("Unknown answer type. Please report this error.")
 
-        raise exception
+    def run(self, connection, show_info):
+        Connection.set_session(self.session_type)
+        options = self._get_options(connection)
+
+        if show_info:
+            self._print_info(connection)
+
+        try:
+            with connection.session.transaction(self.transaction_type, options) as transaction:
+                if self.query_type == "match":
+                    results = self._parse_answer(transaction.query().match(self.query), ConceptMap)
+                elif self.query_type == "match-aggregate":
+                    results = self._parse_answer(transaction.query().match_aggregate(self.query).get(), Numeric)
+                elif self.query_type == "match-group":
+                    results = self._parse_answer(transaction.query().match_group(self.query), ConceptMapGroup)
+                elif self.query_type == "match-group-aggregate":
+                    results = self._parse_answer(transaction.query().match_group_aggregate(self.query), NumericGroup)
+                elif self.query_type == "define":
+                    transaction.query().define(self.query)
+                elif self.query_type == "undefine":
+                    transaction.query().undefine(self.query)
+                elif self.query_type == "insert":
+                    transaction.query().insert(self.query)
+                elif self.query_type == "delete":
+                    transaction.query().delete(self.query)
+                elif self.query_type == "update":
+                    transaction.query().update(self.query)
+
+                if self.transaction_type == TransactionType.WRITE:
+                    transaction.commit()
+                    print('{} query success.'.format(self.query_type.title()))
+                    return
+                else:
+                    return results
+        finally:
+            Connection.set_session(SessionType.DATA)
```


# Comparing `tmp/fluctuate-1.0.1.tar.gz` & `tmp/fluctuate-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluctuate-1.0.1.tar", max compression
+gzip compressed data, was "fluctuate-2.0.0b1.tar", max compression
```

## Comparing `fluctuate-1.0.1.tar` & `fluctuate-2.0.0b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-22 20:29:57.910984 fluctuate-1.0.1/LICENSE
--rw-r--r--   0        0        0     9458 2023-05-22 20:29:57.911985 fluctuate-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/__init__.py
--rw-r--r--   0        0        0     4404 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/cli.py
--rw-r--r--   0        0        0    25195 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/migrations.py
--rw-r--r--   0        0        0     1136 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/secrets_manager.py
--rw-r--r--   0        0        0     1385 2023-05-22 20:30:37.007923 fluctuate-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    10393 1970-01-01 00:00:00.000000 fluctuate-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0    11094 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 00:43:50.085456 fluctuate-2.0.0b1/fluctuate/__init__.py
+-rw-r--r--   0        0        0     4404 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/fluctuate/cli.py
+-rw-r--r--   0        0        0    30650 2023-05-26 00:43:50.059456 fluctuate-2.0.0b1/fluctuate/migrations.py
+-rw-r--r--   0        0        0     1857 2023-05-26 00:43:50.059456 fluctuate-2.0.0b1/fluctuate/secrets_manager.py
+-rw-r--r--   0        0        0     1409 2023-05-26 00:44:29.723621 fluctuate-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0    12019 1970-01-01 00:00:00.000000 fluctuate-2.0.0b1/PKG-INFO
```

### Comparing `fluctuate-1.0.1/LICENSE` & `fluctuate-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluctuate-1.0.1/README.md` & `fluctuate-2.0.0b1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 To define your projects migrations, create a file named `fluctuate_migrations.py` in a
 subfolder of your project along with an `__init__.py` within that subfolder. Within
 `fluctuate_migrations.py` you need to create a tuple or list of `Migration`s named
 "migrations" that defines your migrations. An example from our test suite is below:
 
 ```python
 # fluctuate_migrations.py
+from fauna import fql
 from faunadb import query
 
 from fluctuate.migrations import Migration
 
 migrations = (
     Migration(
         name="test_migration_1",
@@ -72,86 +73,127 @@
         namespace="cli_test",
         migration=query.create_database({"name": "test_database_1"}),
         reverse_migration=query.delete(query.database("test_database_1")),
     ),
     Migration(
         name="test_migration_4",
         namespace="cli_test",
-        migration=query.create_collection(
-            {"name": "test_collection_3", "history_days": 0}
+        migration=fql(
+            """
+            Collection.create({name: "test_collection_3", history_days: 0})
+            """
         ),
-        reverse_migration=query.delete(query.collection("test_collection_3")),
+        reverse_migration=fql('Collection.byName("test_collection_3").delete()'),
         child_database="test_database_1",
     ),
     Migration(
         name="test_migration_5",
         namespace="cli_test",
-        migration=query.create_database({"name": "test_database_2"}),
-        reverse_migration=query.delete(query.database("test_database_2")),
+        migration=fql('Database.create({name: "test_database_2"})'),
+        reverse_migration=fql('Database.byName("test_database_2").delete()'),
         child_database="test_database_1",
     ),
     Migration(
         name="test_migration_6",
         namespace="cli_test",
         migration=query.create_collection(
             {"name": "test_collection_4", "history_days": 0}
         ),
         reverse_migration=query.delete(query.collection("test_collection_4")),
         child_database="test_database_1/test_database_2",
     ),
+    Migration(
+        name="test_migration_7",
+        namespace="cli_test",
+        migration=query.create_index(
+            {
+                "name": "test_collection_4_index",
+                "source": query.select(
+                    "ref", query.get(query.collection("test_collection_4"))
+                ),
+                "terms": [{"field": ["data", "name"]}],
+                "unique": True,
+            }
+        ),
+        reverse_migration=query.delete(query.index("test_collection_4_index")),
+        child_database="test_database_1/test_database_2",
+    ),
+    Migration(
+        name="test_migration_8",
+        namespace="cli_test",
+        migration=fql(
+            """
+            Collection.create(
+                {
+                    name: "test_collection_5",
+                    history_days: 0,
+                    indexes: {by_name: {terms: [{field: "name"}]}},
+                    constraints: [{unique: ["name"]}]
+                }
+            )
+            """
+        ),
+        reverse_migration=fql('Collection.byName("test_collection_5").delete()'),
+        child_database="test_database_1/test_database_2",
+    ),
 )
+
 ```
 
 Let's walk through this example. First a bit about migrations. Each `Migration` has 5
 fields, the first 4 of which are required:
 
 1. name: This is the migration name, and needs to be unique within the migration's
    namespace
 2. namespace: This is the namespace under which the migration resides. You should
    uniquely namespace your application's migrations so as not to clash with any other
    application's migrations that may also be applied to your database.
-3. migration: This is the FQL query used to create your schema documents, be it
-   collections, indexes, UDFs, or otherwise.
-4. reverse_migration: This is the FQL query that will be used to undo whatever the FQL
-   in the migration did, so it should be the opposite operation.
+3. migration: This is the FQLv4 or FQLv10 query used to create your schema documents, be
+   it collections, indexes, UDFs, or otherwise.
+4. reverse_migration: This is the FQLv4 or FQLv10 query that will be used to undo
+   whatever the FQL in the migration did, so it should be the opposite operation.
 5. (OPTIONAL) child_database: This defines the child database to which this migration
    should be applied. Fluctuate will attempt to log into this database and apply the
    migrations there. Nested child databases should be specified in the same format used
    for [scoped keys]. If no child database is defined, the migrations apply to the
    database the current key in use provides access to.
 
-In the example above, there are a total of 6 migrations to be preformed. The first 3
+In the example above, there are a total of 8 migrations to be preformed. The first 3
 migrations apply to the top level database, which is the database the key used to run
 the migration has access to. Then the next 2 migrations are applied to "test_database_1"
-which is created by migration number 3. Finally, the 6th and final migration is applied
-to "test_database_2" which was created in the 5th migration.
+which is created by migration number 3. Finally, the last 3 migrations are applied to
+"test_database_2" which is nested under "test_database_1" and was created in the 5th
+migration.
 
 In this example we applied each schema document in a separate migration, but as the
 `migration` field can be any arbitrary FQL, all schema documents could be created in one
-migration. This tool does not impose an opinion on how to lay out your migrations.
+migration. This tool does not impose an opinion on how to lay out your migrations. Both
+FQLv4 and FQLv10 migrations are supported and can be used interchangeably.
 
-Each migration is applied in a single transaction using [Do] to write both the migration
-and the record that keeps track of the applied migrations. You need to be aware of the
+Each migration is applied in a single transaction to write both the migration and the
+record that keeps track of the applied migrations. If the migration is written in FQLv4,
+a FQLv4 client will be used to apply it. If the migration is written in FQLv10, a FQLv10
+client will be used to apply it. You need to be aware of the
 [caveats of schema documents] when referring to them within the same migration. There is
 also the constraint of not being able to use any schema documents created within the
-same transaction.
+same transaction. This constraint is present in both FQLv4 and FQLv10.
 
 # Applying migrations
 
 The `fluctuate migrate` command is used to apply all unapplied migrations. As migrations
 are applied to your databases, their application is recorded in a separate collection.
 This is referred to when applying migrations to ensure the same migration is not applied
 twice. Migrations are applied in the order they are defined in the migrations tuple or
 list.
 
 Each migration, and the recording of the application of that migration, are applied in a
-single transaction using [Do]. If a migration fails, the transaction rolls back and no
-changes from that migration will be applied. Any migrations that were already
-successfully applied will remain applied. A unique index ensures that the same migration
-in the same namespace can only be applied once.
+single transaction. If a migration fails, the transaction rolls back and no changes from
+that migration will be applied. Any migrations that were already successfully applied
+will remain applied. A unique constraint ensures that the same migration in the same
+namespace can only be applied once.
 
 This tool will attempt to create a collection named "fluctuate_migrations" and an index
 named "fluctuate_migrations_unique_name_and_namespace" on all databases this is used on.
 If a collection and/or index with these names already exist, running this tool will
 fail.
 
 # Unapplying migrations
@@ -163,21 +205,23 @@
 
 Using the example above, if the following is run:
 
 ```bash
 fluctuate unmigrate --key some_key --target test_cli.test_migration_5
 ```
 
-Then the reverse_migration for test_cli.test_migration_6 is run, removing
-test_collection_4 from test_database_2 and then the reverse migration for
-test_cli.test_migration_5 is run deleting test_database_2 from test_database_1.
+Then the reverse_migrations for test_cli.test_migration_8, test_cli.test_migration_7,
+and test_cli.test_migration_6 are run, removing test_collection_5, the
+test_collection_4_index, and test_collection_4 from test_database_2. Then the reverse
+migration for test_cli.test_migration_5 is run deleting test_database_2 from
+test_database_1.
 
 Unapplying a migration, and the recording of unapplying that migration, is done in a
-single transaction using [Do]. If a reverse migration fails, the transaction rolls back
-and no changes from that migration will be reversed. Any migrations that were already
+single transaction. If a reverse migration fails, the transaction rolls back and no
+changes from that migration will be reversed. Any migrations that were already
 successfully unapplied will remain unapplied.
 
 # Specifying Fauna DB credentials
 
 Both commands above require access to a FaunaDB database in order to operate. A key can
 be specified directly when invoking the command using `--key` or the key can be fetched
 from [AWS SecretsManager] by specifying `--secret-arn` with the [ARN] of the secret to
@@ -197,11 +241,11 @@
 
 [Fauna DB]: https://docs.fauna.com/fauna/current/
 [Python]: https://www.python.org/
 [fauna-schema-migrate]: https://github.com/fauna-labs/fauna-schema-migrate
 [pip]: https://pip.pypa.io/en/stable/
 [scoped keys]: https://docs.fauna.com/fauna/current/security/keys?lang=python#scoped-keys
 [Do]: https://docs.fauna.com/fauna/current/api/fql/functions/do?lang=python
-[caveats of schema documents]: https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418/12
+[caveats of schema documents]: https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418/
 [AWS SecretsManager]: https://docs.aws.amazon.com/secretsmanager/
 [ARN]: https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html
 [admin role]: https://docs.fauna.com/fauna/current/security/keys?lang=python#admin-role
```

### Comparing `fluctuate-1.0.1/fluctuate/cli.py` & `fluctuate-2.0.0b1/fluctuate/cli.py`

 * *Files identical despite different names*

### Comparing `fluctuate-1.0.1/fluctuate/migrations.py` & `fluctuate-2.0.0b1/fluctuate/migrations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import importlib
 import itertools
 import logging
 import pkgutil
 import re
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
+from enum import Enum, auto
 from operator import attrgetter
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
+from fauna import fql
+from fauna.client import Client
+from fauna.query import Query
 from faunadb import query
 from faunadb.client import FaunaClient
 
 logger = logging.getLogger(__name__)
 
 
+class FqlVersion(Enum):
+    v4 = auto()
+    v10 = auto()
+
+
 @dataclass
 class Migration:
     """A simple dataclass for defining a migration with a name and operations to
     perform.
 
     name: The name of the migration.
 
     namespace: The namespace this migration lives under. This is used to prevent naming
                collisions of migrations applied to the same database from different
                projects.
 
-    migration: The actual FQL to run when performing the migration.
+    migration: The actual FQLv4 or FQLv10 to run when performing the migration.
 
-    reverse_migration: The FQL that undoes the FQL applied in the migration step.
+    reverse_migration: The FQLv4 or FQLv10 that undoes the FQL applied in the migration
+                       step.
 
     child_database: An optional child database to apply this migration to. The child
                     database name follows the same nesting rules as FaunaDB scoped keys.
                     The child database name is considered relative to the database of
                     the key used to invoke the migration process.
     """
 
     name: str
     namespace: str
-    migration: query
-    reverse_migration: query
+    migration: Union[query._Expr, Query]
+    reverse_migration: Union[query._Expr, Query]
     child_database: Optional[str] = None
 
     @property
     def full_name(self):
         """Return the namespace and name concatenated as f"{namespace}.{name}"."""
         return f"{self.namespace}.{self.name}"
 
@@ -54,51 +64,83 @@
 # Make public the names of the created migrations collection and index in case anyone
 # outside this module needs it.
 migrations_collection_name = "fluctuate_migrations"
 migrations_index_name = "fluctuate_migrations_unique_name_and_namespace"
 
 # This contains the query used to check if the migrations collection already exists, and
 # creates it if it doesn't.
-_create_migrations_collection = query.if_(
-    query.exists(query.collection(migrations_collection_name)),
-    query.get(query.collection(migrations_collection_name)),
-    query.create_collection({"name": migrations_collection_name, "history_days": 0}),
+_create_migrations_collection = fql(
+    """
+    let migrations_collection = Collection.byName(${migrations_collection_name})
+    if (migrations_collection == null) {
+        Collection.create(
+            {
+                name: ${migrations_collection_name},
+                indexes: {
+                    by_name_and_namespace: {
+                        terms: [{"field": "name"}, {"field": "namespace"}]
+                    }
+                },
+                constraints: [{unique: ["name", "namespace"]}]
+            }
+        )
+    } else {
+        if (
+            migrations_collection.indexes.by_name_and_namespace == null ||
+            migrations_collection.indexes.by_name_and_namespace.terms != [
+                {"field": "name"}, {"field": "namespace"}
+            ]
+        ) {
+            migrations_collection.update(
+                {
+                    indexes: {
+                        by_name_and_namespace: {
+                            terms: [{"field": "name"}, {"field": "namespace"}]
+                        }
+                    }
+                }
+            )
+        }
+        if (migrations_collection.constraints != [{unique: ["name", "namespace"]}]) {
+            migrations_collection.update(
+                {constraints: [{unique: ["name", "namespace"]}]}
+            )
+        }
+    }
+    """,
+    migrations_collection_name=migrations_collection_name,
 )
 
-# This contains the query used to check if the unique constraint on migrations already
-# exists, and creates it if it doesn't.
+# This contains the query used to check if the index on migrations already exists, and
+# creates it if it doesn't. We need to keep this around to support mixed FQLv4 and
+# FQLv10 migrations.
 _create_migrations_unique_index = query.if_(
     query.exists(query.index(migrations_index_name)),
     query.get(query.index(migrations_index_name)),
     query.create_index(
         {
             "name": migrations_index_name,
-            "source": query.select("ref", query.var("collection")),
+            "source": query.select(
+                "ref", query.get(query.collection(migrations_collection_name))
+            ),
             "terms": [
                 {"field": ["data", "name"]},
                 {"field": ["data", "namespace"]},
             ],
             "unique": True,
         }
     ),
 )
 
-# Combines the two previously defined queries using let. This is required because of the
-# fact that schema documents cannot be created and then referenced in the same query.
-# Details here: https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418
-_create_required_migrations_schema_objects = query.let(
-    {"collection": _create_migrations_collection}, _create_migrations_unique_index
-)
-
 
-def _create_fauna_client(key, child_db=None):
+def _create_fauna_client(key, fql_version, child_db=None):
     """Create the FaunaDB client using the provided key and return it.
 
-    This configures the FaunaDB client to use the US region group:
-    https://docs.fauna.com/fauna/current/learn/understanding/region_groups#how-to-use-region-groups
+    The `fql_version` parameter controls which version of the FQL client is returned. It
+    can either be a v4 client or a v10 client.
 
     If a `child_db` is provided, the client created will be scoped to that child
     database.
 
     If a `child_db` is provided and the `key` provided is itself a scoped key, the
     resulting key used to create the client will retain the role of the scoped key.
     The child database will also be appended to any child databases the provided key is
@@ -108,15 +150,24 @@
     # the child DB.
     if child_db is not None:
         key = _build_scoped_key(key=key, child_db=child_db)
         logger.debug("Creating FaunaDB client for child database %s.", child_db)
     else:
         logger.debug("Creating FaunaDB client for top level database.")
 
-    fauna_client = FaunaClient(secret=key)
+    if fql_version == FqlVersion.v10:
+        fauna_client = Client(secret=key)
+    elif fql_version == FqlVersion.v4:
+        fauna_client = FaunaClient(secret=key)
+    else:
+        raise ValueError(
+            f"Invalid fql_version of {fql_version} specified. Must be one of: "
+            f"{FqlVersion.v4.name}, {FqlVersion.v10.name}"
+        )
+
     logger.debug("FaunaDB client initialized.")
 
     return fauna_client
 
 
 # This FQL fragment matches the fluctuate_migrations_unique_name_and_namespace using the variables
 # "migration_name" and "migration_namespace" to retrieve the migration's name and
@@ -129,28 +180,41 @@
 
 def _filter_migrations(fauna_client, migrations, condition):
     """Filter to migrations matching the provided condition expression.
 
     The condition expression will be passed the variables of "migration_full_name",
     "migration_name", and "migration_namespace".
     """
+    # Convert to dictionaries so the FQLv10 will treat this as an array of objects. Drop
+    # the `migration` and `reverse_migration` fields as those cannot be serialized
+    # reliably in FQLv10 as they might be FQLv4 query expressions.
+    migration_dicts = tuple(
+        {
+            "full_name": migration.full_name,
+            **{
+                key: value
+                for key, value in asdict(migration).items()
+                if key not in ("migration", "reverse_migration")
+            },
+        }
+        for migration in migrations
+    )
+    # Filter the migrations by the condition and return just the full names.
     filtered_migrations = fauna_client.query(
-        query.filter_(
-            query.lambda_(
-                ["migration_full_name", "migration_name", "migration_namespace"],
-                condition,
-            ),
-            tuple(
-                (migration.full_name, migration.name, migration.namespace)
-                for migration in migrations
-            ),
+        fql(
+            """
+            let migrations = ${migration_objects}
+            let filtered_migrations = migrations.filter((migration) => { ${condition} })
+            // return just the full_name
+            filtered_migrations.map((migration) => { migration.full_name })
+            """,
+            migration_objects=migration_dicts,
+            condition=condition,
         )
-    )
-    # Turn it into a tuple of just the full names.
-    filtered_migrations = tuple(migration[0] for migration in filtered_migrations)
+    ).data
 
     # We should return the migrations list based on which migrations came back.
     return tuple(
         migration
         for migration in migrations
         if migration.full_name in filtered_migrations
     )
@@ -164,15 +228,22 @@
     )
 
     # We should return the migrations list based on which migrations came back as
     # unapplied.
     result = _filter_migrations(
         fauna_client=fauna_client,
         migrations=migrations,
-        condition=query.not_(query.exists(_match_on_name_and_namespace)),
+        condition=fql(
+            """
+            let result = fluctuate_migrations.by_name_and_namespace(
+                migration.name, migration.namespace
+            )
+            result.isEmpty()
+            """
+        ),
     )
     logger.debug("Found the following unapplied migrations: %s", result)
 
     return result
 
 
 def _filter_applied_migrations(fauna_client, migrations):
@@ -183,44 +254,78 @@
     )
 
     # We should return the migrations list based on which migrations came back as
     # applied.
     result = _filter_migrations(
         fauna_client=fauna_client,
         migrations=migrations,
-        condition=query.exists(_match_on_name_and_namespace),
+        condition=fql(
+            """
+            let result = fluctuate_migrations.by_name_and_namespace(
+                migration.name, migration.namespace
+            )
+            !result.isEmpty()
+            """
+        ),
     )
     logger.debug("Found the following applied migrations: %s", result)
 
     return result
 
 
 def _write_migration_document(migration):
-    """Write the migration name to the migrations table."""
+    """Write the migration name to the migrations table.
+
+    This returns a FQLv4 or FQLv10 query fragment based on the type of the migration.
+    """
     migration_data = {
         "name": migration.name,
         "namespace": migration.namespace,
         "child_database": migration.child_database,
     }
     logger.debug("Create migration record: %s", migration_data)
 
+    if isinstance(migration.migration, Query):
+        return fql(
+            "fluctuate_migrations.create(${migration_data})",
+            migration_data=migration_data,
+        )
+
     return query.create(
         query.collection(migrations_collection_name), {"data": migration_data}
     )
 
 
 def _delete_migration_document(migration):
-    """Delete the migration name in the migrations table."""
-    migration_tuple = (migration.name, migration.namespace)
-    logger.debug("Delete migration tuple: %s", migration_tuple)
+    """Delete the migration name in the migrations table.
+
+    This returns a FQLv4 or FQLv10 query fragment based on the type of the migration.
+    """
+    logger.debug("Delete migration %s.%s", migration.name, migration.namespace)
+
+    if isinstance(migration.reverse_migration, Query):
+        return fql(
+            """
+            fluctuate_migrations.by_name_and_namespace(
+                ${migration_name}, ${migration_namespace}
+            ).first().delete()
+            """,
+            migration_name=migration.name,
+            migration_namespace=migration.namespace,
+        )
 
     return query.delete(
         query.select(
             "ref",
-            query.get(query.match(query.index(migrations_index_name), migration_tuple)),
+            query.get(
+                query.match(
+                    query.index(migrations_index_name),
+                    (migration.name, migration.namespace),
+                )
+            ),
         )
     )
 
 
 def _log_package_import_error(module_name):
     """This logs that a module failed to be imported during discovery at the debug
     level to aid in debugging migration discovery issues.
@@ -393,17 +498,24 @@
 
     # We rely on zip stopping once the shortest iterable is exhausted. This means we
     # never fully iterate over `child_db_full_paths_parent`, as we always want to log
     # into the parent of the child DB we are checking for the existence of.
     for child_db_name, child_db_full_path, child_db_parent_full_path in zip(
         child_db_names, child_db_full_paths, child_db_full_paths_parent
     ):
-        fauna_client = _create_fauna_client(key=key, child_db=child_db_parent_full_path)
+        fauna_client = _create_fauna_client(
+            key=key, fql_version=FqlVersion.v10, child_db=child_db_parent_full_path
+        )
         # Ensure the child DB exists.
-        if not fauna_client.query(query.exists(query.database(child_db_name))):
+        if not fauna_client.query(
+            fql(
+                "Database.byName(${child_db_name}) != null",
+                child_db_name=child_db_name,
+            )
+        ).data:
             logger.debug("Child DB %s doesn't exist.", child_db_full_path)
             return False
 
         logger.debug("Child DB %s exists.", child_db_full_path)
 
     logger.debug("All child dbs in %s exist.", child_db)
     return True
@@ -448,47 +560,71 @@
         "Migrations to unapply after limiting to target migration %s: %s.",
         target,
         migrations,
     )
     return migrations
 
 
-def _apply_migration(fauna_client, migration):
+def _apply_migration(fauna_v4_client, fauna_v10_client, migration):
     """Apply an individual migration and write the migration document to record its
     application.
 
     This is done in a single transaction so that if the migration should fail, no
     actions are taken.
     """
-    logger.debug("Attempting to apply migration %s", migration.name)
-    fauna_client.query(
-        query.do(
-            # Apply the migration.
-            migration.migration,
-            # Then record that the migration was applied.
-            _write_migration_document(migration=migration),
+    logger.debug("Attempting to apply migration %s.", migration.name)
+
+    if isinstance(migration.migration, Query):
+        logger.debug("Using FQLv10 to apply migration %s.", migration.name)
+        fauna_v10_client.query(
+            fql(
+                """
+                ${migration}
+                ${write_migration_document}
+                """,
+                migration=migration.migration,
+                write_migration_document=_write_migration_document(migration=migration),
+            )
+        )
+    else:
+        logger.debug("Using FQLv4 to apply migration %s.", migration.name)
+        fauna_v4_client.query(
+            query.do(
+                # Apply the migration.
+                migration.migration,
+                # Then record that the migration was applied.
+                _write_migration_document(migration=migration),
+            )
         )
-    )
-    logger.debug("Successfully applied migration %s", migration.name)
+
+    logger.debug("Successfully applied migration %s.", migration.name)
 
 
 def _apply_migrations(key, child_db, migrations):
     """Apply the provided migrations to the specified child_db using the provided key."""
-    fauna_client = _create_fauna_client(key=key, child_db=child_db)
+    fauna_v10_client = _create_fauna_client(
+        key=key, fql_version=FqlVersion.v10, child_db=child_db
+    )
+    fauna_v4_client = _create_fauna_client(
+        key=key, fql_version=FqlVersion.v4, child_db=child_db
+    )
 
     logger.debug("Creating required schema documents for migration.")
     # Create the required migration schema documents. This cannot be done in the
     # same transaction as applying and recording the applied migrations due to the
     # issue noted here:
     # https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418
-    fauna_client.query(_create_required_migrations_schema_objects)
+    fauna_v10_client.query(_create_migrations_collection)
+    # We must also apply the v4 index since we might be operating on v4 migrations, and
+    # some v4 queries require this index, since v4 cannot use a v10 index.
+    fauna_v4_client.query(_create_migrations_unique_index)
 
     # We need to determine which migrations still need to be applied.
     unapplied_migrations = _filter_unapplied_migrations(
-        fauna_client=fauna_client, migrations=migrations
+        fauna_client=fauna_v10_client, migrations=migrations
     )
     if not unapplied_migrations:
         if child_db is not None:
             logger.info("No migrations to apply for child database %s.", child_db)
         else:
             logger.info("No migrations to apply.")
 
@@ -506,45 +642,67 @@
         logger.info(
             "Attempting to apply %d unapplied migrations.",
             len(unapplied_migrations),
         )
 
     # Apply each migration in its own transaction.
     for migration in unapplied_migrations:
-        _apply_migration(fauna_client=fauna_client, migration=migration)
+        _apply_migration(
+            fauna_v4_client=fauna_v4_client,
+            fauna_v10_client=fauna_v10_client,
+            migration=migration,
+        )
 
     if child_db is not None:
         logger.info(
             "Successfully applied %d unapplied migrations to child database %s.",
             len(unapplied_migrations),
             child_db,
         )
     else:
         logger.info(
             "Successfully applied %d unapplied migrations.",
             len(unapplied_migrations),
         )
 
 
-def _unapply_migration(fauna_client, migration):
+def _unapply_migration(fauna_v4_client, fauna_v10_client, migration):
     """Unapply an individual migration and remove the associated migration document.
 
     This is done in a single transaction so that if the migration should fail, no
     actions are taken.
     """
-    logger.debug("Attempting to unapply migration %s", migration.name)
-    fauna_client.query(
-        query.do(
-            # Unapply the migration.
-            migration.reverse_migration,
-            # Then record that the migration was unapplied.
-            _delete_migration_document(migration=migration),
+    logger.debug("Attempting to unapply migration %s.", migration.name)
+
+    if isinstance(migration.reverse_migration, Query):
+        logger.debug("Using FQLv10 to unapply migration %s.", migration.name)
+        fauna_v10_client.query(
+            fql(
+                """
+                ${reverse_migration}
+                ${delete_migration_document}
+                """,
+                reverse_migration=migration.reverse_migration,
+                delete_migration_document=_delete_migration_document(
+                    migration=migration
+                ),
+            )
         )
-    )
-    logger.debug("Successfully unapplied migration %s", migration.name)
+    else:
+        logger.debug("Using FQLv4 to unapply migration %s.", migration.name)
+        fauna_v4_client.query(
+            query.do(
+                # Unapply the migration.
+                migration.reverse_migration,
+                # Then record that the migration was unapplied.
+                _delete_migration_document(migration=migration),
+            )
+        )
+
+    logger.debug("Successfully unapplied migration %s.", migration.name)
 
 
 def _unapply_migrations(key, child_db, migrations):
     """Unapply the provided migrations for the child_db.
 
     If the child DB does not exist, no action will be performed.
 
@@ -556,25 +714,33 @@
         logger.info(
             "Child database %s does not exist. Skipping the unapply of migrations"
             " for this child database.",
             child_db,
         )
         return
 
-    fauna_client = _create_fauna_client(key=key, child_db=child_db)
+    fauna_v10_client = _create_fauna_client(
+        key=key, fql_version=FqlVersion.v10, child_db=child_db
+    )
+    fauna_v4_client = _create_fauna_client(
+        key=key, fql_version=FqlVersion.v4, child_db=child_db
+    )
 
     logger.debug("Creating required schema documents for migration.")
     # Create the required migration schema documents. This cannot be done in the
     # same transaction as unapplying and deleting the migration documents due to the
     # issue noted here:
     # https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418
-    fauna_client.query(_create_required_migrations_schema_objects)
+    fauna_v10_client.query(_create_migrations_collection)
+    # We must also apply the v4 index since we might be operating on v4 migrations, and
+    # some v4 queries require this index, since v4 cannot use a v10 index.
+    fauna_v4_client.query(_create_migrations_unique_index)
 
     applied_migrations = _filter_applied_migrations(
-        fauna_client=fauna_client, migrations=migrations
+        fauna_client=fauna_v10_client, migrations=migrations
     )
     if not applied_migrations:
         if child_db is not None:
             logger.info("No migrations to unapply for child database %s.", child_db)
         else:
             logger.info("No migrations to unapply.")
 
@@ -592,15 +758,19 @@
         logger.info(
             "Attempting to unapply %d applied migrations.",
             len(applied_migrations),
         )
 
     # Unapply each migration in its own transaction.
     for migration in applied_migrations:
-        _unapply_migration(fauna_client=fauna_client, migration=migration)
+        _unapply_migration(
+            fauna_v4_client=fauna_v4_client,
+            fauna_v10_client=fauna_v10_client,
+            migration=migration,
+        )
 
     if child_db is not None:
         logger.info(
             "Successfully unapplied %d applied migrations on child database %s.",
             len(applied_migrations),
             child_db,
         )
```

### Comparing `fluctuate-1.0.1/fluctuate/secrets_manager.py` & `fluctuate-2.0.0b1/fluctuate/secrets_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import json
 import logging
 
+from fauna.encoding import FaunaDecoder
 from faunadb._json import parse_json
 
 
 class DummyModule:
     """A dummy stand in for the boto3 import that will raise a useful error message
     if any attribute is accessed.
     """
@@ -22,17 +24,32 @@
 
 logger = logging.getLogger(__name__)
 
 
 def get_fauna_secret(arn):
     """Returns the current FaunaDB Key object stored in the AWS SecretsManaqer secret
     pointed to by the provided ARN.
+
+    This first attempts to decode the secret as FQLv10. If that fails, it falls back to
+    using the non-public FQLv4 `parse_json` funtion.
     """
     logger.debug("Attempting to instantiate the Secrets Manager client.")
     secrets_manager_client = boto3.client("secretsmanager")
     logger.debug("Successfully instantiated the Secrets Manager client.")
 
     logger.debug("Attempting to retrieve the secret value with ARN %s.", arn)
     secret = secrets_manager_client.get_secret_value(SecretId=arn)
     logger.debug("Successfully retrieved the secret value with ARN %s.", arn)
 
-    return parse_json(secret["SecretString"])
+    try:
+        logger.debug("Attempting to decode the secret with FQLv10 decoders.")
+        result = FaunaDecoder.decode(json.loads(secret["SecretString"]))
+        logger.debug("Successfully decoded the secret with FQLv10 decoders.")
+    except Exception:
+        logger.debug(
+            "Failed to decode the secret with FQLv10 decoders. Attempting to decode the"
+            " secret using FQLv4 decoders."
+        )
+        result = parse_json(secret["SecretString"])
+        logger.debug("Successfully decoded the secret with FQLv4 decoders.")
+
+    return result
```

### Comparing `fluctuate-1.0.1/pyproject.toml` & `fluctuate-2.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "fluctuate"
-version = "1.0.1"
+version = "2.0.0-beta.1"
 description = "A simple migration utility for Fauna DB."
 authors = ["Ryan Causey <ryan.causey@munipal.io>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/munipal-oss/fluctuate"
 homepage = "https://gitlab.com/munipal-oss/fluctuate"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 click = "^8.1.3"
 cloup = "^2.0.0"
 faunadb = "^4.3.1"
 boto3 = {extras = ["crt"], version = "^1.26.128", optional = true}
 click-log = "^0.4.0"
+fauna = "^0.6.1"
 
 [tool.poetry.group.dev.dependencies]
 prospector = "^1.7.7"
 black = "^23.0.0"
 isort = "^5.10.1"
 pre-commit = "^3.0.0"
 pytest = "^7.2.0"
```

### Comparing `fluctuate-1.0.1/PKG-INFO` & `fluctuate-2.0.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fluctuate
-Version: 1.0.1
+Version: 2.0.0b1
 Summary: A simple migration utility for Fauna DB.
 Home-page: https://gitlab.com/munipal-oss/fluctuate
 License: MIT
 Author: Ryan Causey
 Author-email: ryan.causey@munipal.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: aws-secrets-manager
 Requires-Dist: boto3[crt] (>=1.26.128,<2.0.0) ; extra == "aws-secrets-manager"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
 Requires-Dist: cloup (>=2.0.0,<3.0.0)
+Requires-Dist: fauna (>=0.6.1,<0.7.0)
 Requires-Dist: faunadb (>=4.3.1,<5.0.0)
 Project-URL: Repository, https://gitlab.com/munipal-oss/fluctuate
 Description-Content-Type: text/markdown
 
 # Fluctuate
 
 [![coverage report](https://gitlab.com/munipal-oss/fluctuate/badges/master/coverage.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
@@ -66,14 +66,15 @@
 To define your projects migrations, create a file named `fluctuate_migrations.py` in a
 subfolder of your project along with an `__init__.py` within that subfolder. Within
 `fluctuate_migrations.py` you need to create a tuple or list of `Migration`s named
 "migrations" that defines your migrations. An example from our test suite is below:
 
 ```python
 # fluctuate_migrations.py
+from fauna import fql
 from faunadb import query
 
 from fluctuate.migrations import Migration
 
 migrations = (
     Migration(
         name="test_migration_1",
@@ -96,86 +97,127 @@
         namespace="cli_test",
         migration=query.create_database({"name": "test_database_1"}),
         reverse_migration=query.delete(query.database("test_database_1")),
     ),
     Migration(
         name="test_migration_4",
         namespace="cli_test",
-        migration=query.create_collection(
-            {"name": "test_collection_3", "history_days": 0}
+        migration=fql(
+            """
+            Collection.create({name: "test_collection_3", history_days: 0})
+            """
         ),
-        reverse_migration=query.delete(query.collection("test_collection_3")),
+        reverse_migration=fql('Collection.byName("test_collection_3").delete()'),
         child_database="test_database_1",
     ),
     Migration(
         name="test_migration_5",
         namespace="cli_test",
-        migration=query.create_database({"name": "test_database_2"}),
-        reverse_migration=query.delete(query.database("test_database_2")),
+        migration=fql('Database.create({name: "test_database_2"})'),
+        reverse_migration=fql('Database.byName("test_database_2").delete()'),
         child_database="test_database_1",
     ),
     Migration(
         name="test_migration_6",
         namespace="cli_test",
         migration=query.create_collection(
             {"name": "test_collection_4", "history_days": 0}
         ),
         reverse_migration=query.delete(query.collection("test_collection_4")),
         child_database="test_database_1/test_database_2",
     ),
+    Migration(
+        name="test_migration_7",
+        namespace="cli_test",
+        migration=query.create_index(
+            {
+                "name": "test_collection_4_index",
+                "source": query.select(
+                    "ref", query.get(query.collection("test_collection_4"))
+                ),
+                "terms": [{"field": ["data", "name"]}],
+                "unique": True,
+            }
+        ),
+        reverse_migration=query.delete(query.index("test_collection_4_index")),
+        child_database="test_database_1/test_database_2",
+    ),
+    Migration(
+        name="test_migration_8",
+        namespace="cli_test",
+        migration=fql(
+            """
+            Collection.create(
+                {
+                    name: "test_collection_5",
+                    history_days: 0,
+                    indexes: {by_name: {terms: [{field: "name"}]}},
+                    constraints: [{unique: ["name"]}]
+                }
+            )
+            """
+        ),
+        reverse_migration=fql('Collection.byName("test_collection_5").delete()'),
+        child_database="test_database_1/test_database_2",
+    ),
 )
+
 ```
 
 Let's walk through this example. First a bit about migrations. Each `Migration` has 5
 fields, the first 4 of which are required:
 
 1. name: This is the migration name, and needs to be unique within the migration's
    namespace
 2. namespace: This is the namespace under which the migration resides. You should
    uniquely namespace your application's migrations so as not to clash with any other
    application's migrations that may also be applied to your database.
-3. migration: This is the FQL query used to create your schema documents, be it
-   collections, indexes, UDFs, or otherwise.
-4. reverse_migration: This is the FQL query that will be used to undo whatever the FQL
-   in the migration did, so it should be the opposite operation.
+3. migration: This is the FQLv4 or FQLv10 query used to create your schema documents, be
+   it collections, indexes, UDFs, or otherwise.
+4. reverse_migration: This is the FQLv4 or FQLv10 query that will be used to undo
+   whatever the FQL in the migration did, so it should be the opposite operation.
 5. (OPTIONAL) child_database: This defines the child database to which this migration
    should be applied. Fluctuate will attempt to log into this database and apply the
    migrations there. Nested child databases should be specified in the same format used
    for [scoped keys]. If no child database is defined, the migrations apply to the
    database the current key in use provides access to.
 
-In the example above, there are a total of 6 migrations to be preformed. The first 3
+In the example above, there are a total of 8 migrations to be preformed. The first 3
 migrations apply to the top level database, which is the database the key used to run
 the migration has access to. Then the next 2 migrations are applied to "test_database_1"
-which is created by migration number 3. Finally, the 6th and final migration is applied
-to "test_database_2" which was created in the 5th migration.
+which is created by migration number 3. Finally, the last 3 migrations are applied to
+"test_database_2" which is nested under "test_database_1" and was created in the 5th
+migration.
 
 In this example we applied each schema document in a separate migration, but as the
 `migration` field can be any arbitrary FQL, all schema documents could be created in one
-migration. This tool does not impose an opinion on how to lay out your migrations.
+migration. This tool does not impose an opinion on how to lay out your migrations. Both
+FQLv4 and FQLv10 migrations are supported and can be used interchangeably.
 
-Each migration is applied in a single transaction using [Do] to write both the migration
-and the record that keeps track of the applied migrations. You need to be aware of the
+Each migration is applied in a single transaction to write both the migration and the
+record that keeps track of the applied migrations. If the migration is written in FQLv4,
+a FQLv4 client will be used to apply it. If the migration is written in FQLv10, a FQLv10
+client will be used to apply it. You need to be aware of the
 [caveats of schema documents] when referring to them within the same migration. There is
 also the constraint of not being able to use any schema documents created within the
-same transaction.
+same transaction. This constraint is present in both FQLv4 and FQLv10.
 
 # Applying migrations
 
 The `fluctuate migrate` command is used to apply all unapplied migrations. As migrations
 are applied to your databases, their application is recorded in a separate collection.
 This is referred to when applying migrations to ensure the same migration is not applied
 twice. Migrations are applied in the order they are defined in the migrations tuple or
 list.
 
 Each migration, and the recording of the application of that migration, are applied in a
-single transaction using [Do]. If a migration fails, the transaction rolls back and no
-changes from that migration will be applied. Any migrations that were already
-successfully applied will remain applied. A unique index ensures that the same migration
-in the same namespace can only be applied once.
+single transaction. If a migration fails, the transaction rolls back and no changes from
+that migration will be applied. Any migrations that were already successfully applied
+will remain applied. A unique constraint ensures that the same migration in the same
+namespace can only be applied once.
 
 This tool will attempt to create a collection named "fluctuate_migrations" and an index
 named "fluctuate_migrations_unique_name_and_namespace" on all databases this is used on.
 If a collection and/or index with these names already exist, running this tool will
 fail.
 
 # Unapplying migrations
@@ -187,21 +229,23 @@
 
 Using the example above, if the following is run:
 
 ```bash
 fluctuate unmigrate --key some_key --target test_cli.test_migration_5
 ```
 
-Then the reverse_migration for test_cli.test_migration_6 is run, removing
-test_collection_4 from test_database_2 and then the reverse migration for
-test_cli.test_migration_5 is run deleting test_database_2 from test_database_1.
+Then the reverse_migrations for test_cli.test_migration_8, test_cli.test_migration_7,
+and test_cli.test_migration_6 are run, removing test_collection_5, the
+test_collection_4_index, and test_collection_4 from test_database_2. Then the reverse
+migration for test_cli.test_migration_5 is run deleting test_database_2 from
+test_database_1.
 
 Unapplying a migration, and the recording of unapplying that migration, is done in a
-single transaction using [Do]. If a reverse migration fails, the transaction rolls back
-and no changes from that migration will be reversed. Any migrations that were already
+single transaction. If a reverse migration fails, the transaction rolls back and no
+changes from that migration will be reversed. Any migrations that were already
 successfully unapplied will remain unapplied.
 
 # Specifying Fauna DB credentials
 
 Both commands above require access to a FaunaDB database in order to operate. A key can
 be specified directly when invoking the command using `--key` or the key can be fetched
 from [AWS SecretsManager] by specifying `--secret-arn` with the [ARN] of the secret to
@@ -221,12 +265,12 @@
 
 [Fauna DB]: https://docs.fauna.com/fauna/current/
 [Python]: https://www.python.org/
 [fauna-schema-migrate]: https://github.com/fauna-labs/fauna-schema-migrate
 [pip]: https://pip.pypa.io/en/stable/
 [scoped keys]: https://docs.fauna.com/fauna/current/security/keys?lang=python#scoped-keys
 [Do]: https://docs.fauna.com/fauna/current/api/fql/functions/do?lang=python
-[caveats of schema documents]: https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418/12
+[caveats of schema documents]: https://forums.fauna.com/t/do-and-creation-of-schema-documents/3418/
 [AWS SecretsManager]: https://docs.aws.amazon.com/secretsmanager/
 [ARN]: https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html
 [admin role]: https://docs.fauna.com/fauna/current/security/keys?lang=python#admin-role
```


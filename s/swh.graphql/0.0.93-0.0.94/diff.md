# Comparing `tmp/swh.graphql-0.0.93.tar.gz` & `tmp/swh.graphql-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.graphql-0.0.93.tar", last modified: Mon Mar 27 12:34:19 2023, max compression
+gzip compressed data, was "dist/swh.graphql-0.0.94.tar", last modified: Fri May 26 08:58:56 2023, max compression
```

## Comparing `swh.graphql-0.0.93.tar` & `swh.graphql-0.0.94.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/Dockerfile
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     2880 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1975 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docker-compose-dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docker-compose-staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docker-compose.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1975 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      267 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/requirements-dev.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       52 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/setup.cfg
--rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1892 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/app.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7080 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/backends/archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/backends/search.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/client/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/client/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5116 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/client/explorer.html
--rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/client/view.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/config/
--rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/config/dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/config/staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      276 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/config/test.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/errors/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/errors/errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1512 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/errors/handlers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/middlewares/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/middlewares/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/middlewares/logger.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/base_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3032 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/base_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4129 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2313 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/person.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/release.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4945 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11237 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1224 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2885 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/snapshot.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/snapshot_branch.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/swhid.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/target.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2031 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/visit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2065 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/resolvers/visit_status.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/schema/
--rw-r--r--   0 jenkins    (115) docker     (999)    19127 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/schema/schema.graphql
--rw-r--r--   0 jenkins    (115) docker     (999)     4277 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7809 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/data.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_branch_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6083 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_logger.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_origin_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3347 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_origin_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_pagination.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_query_cost.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_release_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_snapshot_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_swhid_resolve.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4342 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_visit_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/test_visit_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/functional/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/backends/test_archive.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)     1708 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/errors/test_errors.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1099 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/test_server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh/graphql/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/utils/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1812 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/swh/graphql/utils/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2880 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3408 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      171 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-27 12:34:19.000000 swh.graphql-0.0.93/swh.graphql.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-03-27 12:34:17.000000 swh.graphql-0.0.93/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Dockerfile
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose-dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose-staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      316 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-dev.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       52 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/setup.cfg
+-rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1892 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/app.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7564 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/search.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/client/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5116 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/explorer.html
+-rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/view.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/config/
+-rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      276 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/test.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/handlers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/middlewares/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/middlewares/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/middlewares/logger.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/base_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/base_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4129 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2313 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/person.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/release.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5128 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11486 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3435 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/snapshot.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/snapshot_branch.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/swhid.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/target.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2141 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/visit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/visit_status.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/schema/
+-rw-r--r--   0 jenkins    (115) docker     (999)    19570 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/schema/schema.graphql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4277 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7809 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/data.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_branch_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6083 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_logger.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4815 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_pagination.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_query_cost.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_release_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_snapshot_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_swhid_resolve.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5259 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/test_archive.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2022 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/errors/test_errors.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/test_server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/utils/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2102 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/utils/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3408 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      171 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/tox.ini
```

### Comparing `swh.graphql-0.0.93/.pre-commit-config.yaml` & `swh.graphql-0.0.94/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/CODE_OF_CONDUCT.md` & `swh.graphql-0.0.94/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/LICENSE` & `swh.graphql-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/Makefile.local` & `swh.graphql-0.0.94/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/setup.py` & `swh.graphql-0.0.94/setup.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/app.py` & `swh.graphql-0.0.94/swh/graphql/app.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/backends/archive.py` & `swh.graphql-0.0.94/swh/graphql/backends/archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,19 @@
     Release,
     Revision,
     Sha1Git,
     Snapshot,
     SnapshotBranch,
 )
 from swh.model.swhids import ObjectType
+from swh.storage.algos.origin import origin_get_latest_visit_status
 from swh.storage.algos.snapshot import snapshot_resolve_branch_target
 from swh.storage.interface import (
     HashDict,
+    ListOrder,
     PagedResult,
     PartialBranches,
     StorageInterface,
 )
 
 
 class Archive:
@@ -39,18 +41,22 @@
 
     def get_origins(
         self, after: Optional[str] = None, first: int = 50
     ) -> PagedResult[Origin]:
         return self.storage.origin_list(page_token=after, limit=first)
 
     def get_origin_visits(
-        self, origin_url: str, after: Optional[str] = None, first: int = 50
+        self,
+        origin_url: str,
+        order: ListOrder,
+        after: Optional[str] = None,
+        first: int = 50,
     ) -> PagedResult[OriginVisit]:
         return self.storage.origin_visit_get(
-            origin=origin_url, page_token=after, limit=first
+            origin=origin_url, page_token=after, limit=first, order=order
         )
 
     def get_origin_visit(self, origin_url: str, visit_id: int) -> Optional[OriginVisit]:
         return self.storage.origin_visit_get_by(origin=origin_url, visit=visit_id)
 
     def get_origin_latest_visit(
         self,
@@ -66,19 +72,24 @@
             require_snapshot=require_snapshot,
         )
 
     def get_visit_statuses(
         self,
         origin_url: str,
         visit_id: int,
+        order: ListOrder,
         after: Optional[str] = None,
         first: int = 50,
     ) -> PagedResult[OriginVisitStatus]:
         return self.storage.origin_visit_status_get(
-            origin=origin_url, visit=visit_id, page_token=after, limit=first
+            origin=origin_url,
+            visit=visit_id,
+            page_token=after,
+            limit=first,
+            order=order,
         )
 
     def get_latest_visit_status(
         self,
         origin_url: str,
         visit_id: int,
         allowed_statuses: Optional[List[str]] = None,
@@ -188,7 +199,14 @@
     ) -> Tuple[Optional[SnapshotBranch], List[bytes]]:
         return snapshot_resolve_branch_target(
             storage=self.storage,
             snapshot_id=snapshot_id,
             branch_obj=branch_obj,
             max_length=max_length,
         )
+
+    def get_latest_origin_visit_status(
+        self, origin: str, require_snapshot: bool = True
+    ):
+        return origin_get_latest_visit_status(
+            storage=self.storage, origin_url=origin, require_snapshot=require_snapshot
+        )
```

### Comparing `swh.graphql-0.0.93/swh/graphql/backends/search.py` & `swh.graphql-0.0.94/swh/graphql/backends/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/client/explorer.html` & `swh.graphql-0.0.94/swh/graphql/client/explorer.html`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/client/view.py` & `swh.graphql-0.0.94/swh/graphql/client/view.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/errors/__init__.py` & `swh.graphql-0.0.94/swh/graphql/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/errors/errors.py` & `swh.graphql-0.0.94/swh/graphql/errors/errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/middlewares/logger.py` & `swh.graphql-0.0.94/swh/graphql/middlewares/logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/base_connection.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/base_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/base_node.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/base_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def _get_node_from_data(self, node_data: Any) -> Optional[Any]:
         """
         Get the object from node_data
         In case of a dict, convert it to an object
         Override to support different data structures
         """
-        if type(node_data) is dict:
+        if isinstance(node_data, dict):
             return namedtuple("NodeObj", node_data.keys())(*node_data.values())
         return node_data
 
     def _handle_node_errors(self) -> None:
         """
         Handle any error related to node data
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/content.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/content.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/directory.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/directory_entry.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/directory_entry.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/origin.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/origin.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/person.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/person.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/release.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/release.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/resolver_factory.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/resolver_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2022 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+import logging
 from typing import ClassVar, Dict, Type
 
 from swh.core import statsd
 from swh.graphql.errors import NullableObjectError
 
 from .base_connection import BaseConnection, BaseList
 from .base_node import BaseNode
@@ -25,34 +26,37 @@
     LogRevisionConnection,
     ParentRevisionConnection,
     RevisionNode,
     TargetRevisionNode,
 )
 from .search import OriginSearchConnection
 from .snapshot import (
+    LatestSnapshotNode,
     OriginSnapshotConnection,
     SnapshotNode,
     TargetSnapshotNode,
     VisitSnapshotNode,
 )
 from .snapshot_branch import SnapshotBranchConnection
 from .swhid import ResolveSWHIDList
 from .target import BranchTargetNode, TargetNode
 from .visit import LatestVisitNode, OriginVisitConnection, OriginVisitNode
 from .visit_status import LatestVisitStatusNode, VisitStatusConnection
 
 this_statsd = statsd.Statsd(namespace="swh_graphql")
+logger = logging.getLogger(__name__)
 
 
 class NodeObjectFactory:
     mapping: ClassVar[Dict[str, Type[BaseNode]]] = {
         "origin": OriginNode,
         "visit": OriginVisitNode,
         "latest-visit": LatestVisitNode,
         "latest-status": LatestVisitStatusNode,
+        "latest-snapshot": LatestSnapshotNode,
         "visit-snapshot": VisitSnapshotNode,
         "snapshot": SnapshotNode,
         "revision": RevisionNode,
         "revision-directory": RevisionDirectoryNode,
         "release": ReleaseNode,
         "directory": DirectoryNode,
         "directory-entry": DirectoryEntryNode,
@@ -75,14 +79,15 @@
             raise AttributeError(f"Invalid node type: {node_type}")
         with this_statsd.timed("node_query_seconds", tags={"node": node_type}):
             try:
                 node_obj = resolver(obj, info, *args, **kw)
             except NullableObjectError:
                 # Return None instead of the object
                 # FIXME, add to the sentry transaction
+                logger.warning("Null %s object", node_type)
                 node_obj = None
         return node_obj
 
 
 class ConnectionObjectFactory:
     mapping: ClassVar[Dict[str, Type[BaseConnection]]] = {
         "origins": OriginConnection,
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/resolvers.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/resolvers.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,21 @@
 @origin.field("latestVisit")
 def latest_visit_resolver(
     obj: rs.origin.BaseOriginNode, info: GraphQLResolveInfo, **kw
 ) -> Optional[rs.visit.LatestVisitNode]:
     return NodeObjectFactory.create("latest-visit", obj, info, **kw)
 
 
+@origin.field("latestSnapshot")
+def latest_snapshot_resolver(
+    obj: rs.origin.BaseOriginNode, info: GraphQLResolveInfo, **kw
+) -> Optional[rs.snapshot.LatestSnapshotNode]:
+    return NodeObjectFactory.create("latest-snapshot", obj, info, **kw)
+
+
 @query.field("visit")
 def visit_resolver(
     obj: None, info: GraphQLResolveInfo, **kw
 ) -> rs.visit.OriginVisitNode:
     return NodeObjectFactory.create("visit", obj, info, **kw)
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/revision.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/scalars.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/scalars.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 datetime_scalar = ScalarType("DateTime")
 swhid_scalar = ScalarType("SWHID")
 id_scalar = ScalarType("ID")
 
 
 @id_scalar.serializer
 def serialize_id(value) -> str:
-    if type(value) is str:
+    if isinstance(value, str):
         value = value.encode()
     return value.hex()
 
 
 @datetime_scalar.serializer
 def serialize_datetime(value: Optional[datetime.datetime]) -> Optional[str]:
-    return utils.get_formatted_date(value) if type(value) == datetime.datetime else None
+    return None if value is None else utils.get_formatted_date(value)
 
 
 @swhid_scalar.value_parser
 def validate_swhid(value):
     try:
         swhid = CoreSWHID.from_string(value)
     except ValidationError as e:
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/search.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/snapshot.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/snapshot.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,14 +68,35 @@
 
     _can_be_null = True
 
     def _get_node_data(self):
         return self.archive.get_snapshot(snapshot_id=self.obj.target_hash, verify=False)
 
 
+class LatestSnapshotNode(BaseSnapshotNode):
+    """
+    Node resolver for the latest snapshot in an origin
+    """
+
+    obj: OriginNode
+
+    _can_be_null = True
+
+    def _get_node_data(self):
+        latest_status_with_snapshot = self.archive.get_latest_origin_visit_status(
+            origin=self.obj.url,
+            require_snapshot=True,
+        )
+        if not latest_status_with_snapshot:
+            return None
+        return self.archive.get_snapshot(
+            snapshot_id=latest_status_with_snapshot.snapshot, verify=False
+        )
+
+
 class OriginSnapshotConnection(BaseConnection):
     """
     Connection resolver for the snapshots in an origin
     """
 
     obj: OriginNode
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/snapshot_branch.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/snapshot_branch.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/swhid.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/swhid.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/target.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/target.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/visit.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/visit.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,10 +64,13 @@
 
     _node_class = BaseVisitNode
 
     def _get_connection_data(self) -> ConnectionData:
         # self.obj.url is the origin URL
         return ConnectionData(
             paged_result=self.archive.get_origin_visits(
-                self.obj.url, after=self._get_after_arg(), first=self._get_first_arg()
+                self.obj.url,
+                after=self._get_after_arg(),
+                first=self._get_first_arg(),
+                order=utils.get_storage_list_order(self.kwargs.get("sort")),
             )
         )
```

### Comparing `swh.graphql-0.0.93/swh/graphql/resolvers/visit_status.py` & `swh.graphql-0.0.94/swh/graphql/resolvers/visit_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,13 +55,14 @@
         # self.obj.origin is the origin URL
         return ConnectionData(
             paged_result=self.archive.get_visit_statuses(
                 self.obj.origin,
                 self.obj.visitId,
                 after=self._get_after_arg(),
                 first=self._get_first_arg(),
+                order=utils.get_storage_list_order(self.kwargs.get("sort")),
             )
         )
 
     def _get_index_cursor(self, index: int, node: BaseVisitStatusNode):
         # Visit status is using a different cursor, hence the override
         return utils.get_encoded_cursor(utils.get_formatted_date(node.date))
```

### Comparing `swh.graphql-0.0.93/swh/graphql/schema/schema.graphql` & `swh.graphql-0.0.94/swh/graphql/schema/schema.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,22 @@
   """
   Are there more pages in the connection?
   """
   hasNextPage: Boolean!
 }
 
 """
+Possible ways to order a list
+"""
+enum ListOrder {
+  ASC
+  DESC
+}
+
+"""
 Binary string with multiple encodings
 """
 type BinaryString {
   """
   Utf-8 encoded value, any non Unicode character will be replaced
   """
   text: String!
@@ -127,14 +135,19 @@
     """
     first: Int!
 
     """
     Returns the page after this cursor
     """
     after: String
+
+    """
+    Sort order on visitId; ascending by default
+    """
+    sort: ListOrder = ASC    # FIXME: Change this to VisitSortOrder type to support orderby specific/multiple columns
   ): VisitConnection! @cost(complexity: 1, multipliers: ["first"])
 
   """
   Latest visit object for the origin
   """
   latestVisit(
     """
@@ -163,14 +176,19 @@
     first: Int!
 
     """
     Returns the page after this cursor
     """
     after: String
   ): SnapshotConnection @cost(complexity: 2, multipliers: ["first"])  # This costs more because of local (graphql level) pagination
+
+  """
+  Latest snapshot for the Origin
+  """
+  latestSnapshot: Snapshot @cost(complexity: 1)
 }
 
 """
 Connection to origin visits
 """
 type VisitConnection {
   """
@@ -257,14 +275,19 @@
     """
     first: Int
 
     """
     Returns the page after this cursor
     """
     after: String
+
+    """
+    Sort order on status date; ascending by default
+    """
+    sort: ListOrder = ASC
   ): VisitStatusConnection @cost(complexity: 3)  # here first is optional, hence adding a higher value for cost
 
   """
   Latest status object for the Visit
   """
   latestStatus(
     """
```

### Comparing `swh.graphql-0.0.93/swh/graphql/server.py` & `swh.graphql-0.0.94/swh/graphql/server.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/conftest.py` & `swh.graphql-0.0.94/swh/graphql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/data.py` & `swh.graphql-0.0.94/swh/graphql/tests/data.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_branch_connection.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_branch_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_content.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_content.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_directory.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_directory_entry.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory_entry.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_errors.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_logger.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_origin_connection.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_origin_node.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -52,14 +52,39 @@
     assert data_origin["id"] == storage_origin.id.hex()
     assert len(data_origin["visits"]["nodes"]) == len(visits_and_statuses)
     assert data_origin["latestVisit"]["visitId"] == visits_and_statuses[-1].visit.visit
     snapshots = storage.origin_snapshot_get_all(origin.url)
     assert len(data_origin["snapshots"]["nodes"]) == len(snapshots)
 
 
+@pytest.mark.parametrize("origin", get_origins())
+@pytest.mark.parametrize("sort", ["ASC", "DESC"])
+def test_visits_sort_order(client, storage, origin, sort):
+    query_str = """
+    query getOrigin($url: String!, $sort: ListOrder) {
+      origin(url: $url) {
+        url
+        id
+        visits(first: 10, sort: $sort) {
+          nodes {
+            visitId
+          }
+        }
+      }
+    }
+    """
+    response, _ = utils.get_query_response(client, query_str, url=origin.url, sort=sort)
+    data_visits = response["origin"]["visits"]["nodes"]
+    if sort == "DESC":
+        data_visits.reverse()
+    assert [
+        {"visitId": x.visit} for x in storage.origin_visit_get(origin.url).results
+    ] == data_visits
+
+
 def test_latest_visit_type_filter(client):
     query_str = """
     query getOrigin($url: String!, $visitType: String!) {
       origin(url: $url) {
         latestVisit(visitType: $visitType) {
           visitId
         }
@@ -116,7 +141,37 @@
         query_str,
         url=get_origins()[1].url,
         allowedStatuses=["partial"],
     )
     assert data["origin"] == {
         "latestVisit": {"statuses": {"nodes": [{"status": "partial"}]}, "visitId": 2}
     }
+
+
+@pytest.mark.parametrize("origin", get_origins())
+def test_latest_snashot(client, origin):
+    query_str = """
+    query getOrigin($url: String!) {
+      origin(url: $url) {
+        latestSnapshot {
+          swhid
+        }
+        latestVisit(requireSnapshot: true) {
+          latestStatus(requireSnapshot: true) {
+            snapshot {
+              swhid
+            }
+          }
+        }
+      }
+    }
+    """
+    data, _ = utils.get_query_response(
+        client,
+        query_str,
+        url=origin.url,
+    )
+    # origin.latestSnapshot and origin.latestVisit.latestStatus.snapshot must be the same
+    assert (
+        data["origin"]["latestSnapshot"]
+        == data["origin"]["latestVisit"]["latestStatus"]["snapshot"]
+    )
```

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_pagination.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_pagination.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_query_cost.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_query_cost.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_release_node.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_release_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_revision.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_search.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_snapshot_node.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_snapshot_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_swhid_resolve.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_swhid_resolve.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_visit_node.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,14 +64,44 @@
         type
       }
     }
     """
     utils.assert_missing_object(client, query_str, "visit")
 
 
+@pytest.mark.parametrize("sort", ["ASC", "DESC"])
+def test_visit_status_sort_order(client, storage, sort):
+    query_str = """
+    query getVisit($origin: String!, $visitId: Int!, $sort: ListOrder) {
+      visit(originUrl: $origin, visitId: $visitId) {
+        visitId
+        statuses(sort: $sort) {
+          nodes {
+            date
+          }
+        }
+      }
+    }
+    """
+    # Testing the only test visit object with multiple statuses
+    origin = get_origins()[0].url
+    visit = 1
+    response, _ = utils.get_query_response(
+        client, query_str, origin=origin, visitId=visit, sort=sort
+    )
+    data_statuses = response["visit"]["statuses"]["nodes"]
+    if sort == "DESC":
+        data_statuses.reverse()
+    original_data = [
+        {"date": x.date.isoformat()}
+        for x in storage.origin_visit_status_get(origin=origin, visit=visit).results
+    ]
+    assert data_statuses == original_data
+
+
 def test_get_latest_visit_status_filter_by_status_return_null(client):
     query_str = """
     query getVisit($origin: String!, $visitId: Int!) {
       visit(originUrl: $origin, visitId: $visitId) {
         visitId
         date
         type
```

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/test_visit_status.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_status.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/functional/utils.py` & `swh.graphql-0.0.94/swh/graphql/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/errors/test_errors.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/errors/test_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2022 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from graphql import GraphQLError
+from graphql import GraphQLError, GraphQLSyntaxError
 import pytest
 import sentry_sdk
 
 from swh.graphql import errors
 
 
 def test_errors():
@@ -46,8 +46,15 @@
     [errors.ObjectNotFoundError, errors.PaginationError, errors.InvalidInputError],
 )
 def test_format_error_skip_sentry(mocker, error):
     mocked_senty_call = mocker.patch.object(sentry_sdk, "capture_exception")
     err = GraphQLError("test error")
     err.original_error = error("test error")
     errors.format_error(err)
-    mocked_senty_call.assert_not_called
+    mocked_senty_call.assert_not_called()
+
+
+def test_format_error_query_syntax_error_skip_sentry(mocker):
+    mocked_senty_call = mocker.patch.object(sentry_sdk, "capture_exception")
+    error = GraphQLSyntaxError(source=None, position=[1], description="test")
+    errors.format_error(error)
+    mocked_senty_call.assert_not_called()
```

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_resolver_factory.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolver_factory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_resolvers.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/resolvers/test_scalars.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_scalars.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 
 def test_serialize_datetime_from_datetime():
     dt = datetime.datetime(2010, 1, 15, 2, 12, 10, 2, datetime.timezone.utc)
     assert scalars.serialize_datetime(dt) == "2010-01-15T02:12:10.000002+00:00"
 
 
 def test_serialize_datetime_invalid_input():
-    assert scalars.serialize_datetime("test") is None
+    assert scalars.serialize_datetime(None) is None
```

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/test_server.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/tests/unit/utils/test_utils.py` & `swh.graphql-0.0.94/swh/graphql/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/swh/graphql/utils/utils.py` & `swh.graphql-0.0.94/swh/graphql/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import base64
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Optional
 
+from swh.graphql.errors import InvalidInputError
+
 if TYPE_CHECKING:
     from swh.graphql.resolvers.base_connection import ConnectionData
 
-from swh.storage.interface import PagedResult
+from swh.storage.interface import ListOrder, PagedResult
 
 ENCODING = "utf-8"
 
 
 def get_b64_string(source) -> str:
-    if type(source) is str:
+    if isinstance(source, str):
         source = source.encode(ENCODING)
     return base64.b64encode(source).decode("ascii")
 
 
 def get_encoded_cursor(cursor: Optional[str]) -> Optional[str]:
     if cursor is None:
         return None
@@ -34,14 +36,21 @@
 
 
 def get_formatted_date(date: datetime) -> str:
     # FIXME, handle error + return other formats
     return date.isoformat()
 
 
+def get_storage_list_order(order: str) -> ListOrder:
+    mapping = {"ASC": ListOrder.ASC, "DESC": ListOrder.DESC}
+    if order not in mapping:
+        raise InvalidInputError("Invalid sort order")
+    return mapping[order]
+
+
 def get_local_paginated_data(source: List, first: int, after=0) -> "ConnectionData":
     """
     Pagination at the GraphQL level
     This is a temporary fix and inefficient. Should eventually be moved to the
     backend (storage) level
     """
     from swh.graphql.resolvers.base_connection import ConnectionData
```

### Comparing `swh.graphql-0.0.93/swh.graphql.egg-info/SOURCES.txt` & `swh.graphql-0.0.94/swh.graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.93/tox.ini` & `swh.graphql-0.0.94/tox.ini`

 * *Files identical despite different names*


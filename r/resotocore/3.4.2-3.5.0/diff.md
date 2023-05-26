# Comparing `tmp/resotocore-3.4.2.tar.gz` & `tmp/resotocore-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.4.2.tar", last modified: Wed May 10 12:25:24 2023, max compression
+gzip compressed data, was "resotocore-3.5.0.tar", last modified: Fri May 26 18:28:10 2023, max compression
```

## Comparing `resotocore-3.4.2.tar` & `resotocore-3.5.0.tar`

### file list

```diff
@@ -1,707 +1,722 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.696707 resotocore-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 12:22:20.000000 resotocore-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 12:22:20.000000 resotocore-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-10 12:25:24.696707 resotocore-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 12:22:20.000000 resotocore-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 12:22:20.000000 resotocore-3.4.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 12:22:20.000000 resotocore-3.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-10 12:22:20.000000 resotocore-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27600 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   208744 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33828 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.604704 resotocore-3.4.2/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    63259 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.604704 resotocore-3.4.2/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.604704 resotocore-3.4.2/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.592704 resotocore-3.4.2/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.604704 resotocore-3.4.2/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 12:25:19.000000 resotocore-3.4.2/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.608705 resotocore-3.4.2/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 12:25:19.000000 resotocore-3.4.2/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 12:25:19.000000 resotocore-3.4.2/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.592704 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.668706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.672706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.592704 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.592704 resotocore-3.4.2/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.592704 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.596704 resotocore-3.4.2/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.596704 resotocore-3.4.2/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.596704 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.676706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.680706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.680706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.680706 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-05-10 12:25:16.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.680706 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.684707 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-05-10 12:25:09.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.684707 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-05-10 12:25:05.000000 resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-10 12:25:20.000000 resotocore-3.4.2/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.4.2/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.688707 resotocore-3.4.2/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    54880 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/report/report_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   117264 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.596704 resotocore-3.4.2/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.596704 resotocore-3.4.2/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/static/report/checks/aws/aws_s3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.692707 resotocore-3.4.2/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30960 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    27785 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/task/task_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.696707 resotocore-3.4.2/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59104 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-10 12:22:20.000000 resotocore-3.4.2/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:24.600705 resotocore-3.4.2/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31226 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 12:25:24.000000 resotocore-3.4.2/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-10 12:25:24.696707 resotocore-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-10 12:22:20.000000 resotocore-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.466279 resotocore-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 18:25:00.000000 resotocore-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 18:25:00.000000 resotocore-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-26 18:28:10.466279 resotocore-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 18:25:00.000000 resotocore-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 18:25:00.000000 resotocore-3.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-26 18:25:00.000000 resotocore-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 18:25:00.000000 resotocore-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27773 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   226381 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36431 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32045 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/deferred_edge_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64016 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 18:28:06.000000 resotocore-3.5.0/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.386279 resotocore-3.5.0/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 18:28:06.000000 resotocore-3.5.0/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 18:28:06.000000 resotocore-3.5.0/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.438279 resotocore-3.5.0/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1408.7461890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2557.75e9da2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/302.8bcc38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3444.47d5ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4931.430433b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5238.1751cc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6475.6037fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8370.8f855e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8685.d78bdab.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8732.9320f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9382.9014799.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/9960.64cd61e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.438279 resotocore-3.5.0/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.438279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.442279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.374279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.446279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.450279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.450279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.450279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.450279 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-05-26 18:28:03.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.450279 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.454279 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-05-26 18:27:56.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.454279 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.454279 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-05-26 18:27:53.000000 resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-26 18:28:06.000000 resotocore-3.5.0/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.5.0/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54880 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.458279 resotocore-3.5.0/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/report/report_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   127540 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.378279 resotocore-3.5.0/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.378279 resotocore-3.5.0/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/static/resoto_logo_and_text.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28187 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.462279 resotocore-3.5.0/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.466279 resotocore-3.5.0/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64774 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-26 18:25:00.000000 resotocore-3.5.0/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:28:10.382279 resotocore-3.5.0/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31633 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 18:28:10.000000 resotocore-3.5.0/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-26 18:28:10.466279 resotocore-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-26 18:25:00.000000 resotocore-3.5.0/setup.py
```

### Comparing `resotocore-3.4.2/LICENSE` & `resotocore-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/PKG-INFO` & `resotocore-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.4.2
+Version: 3.5.0
 Summary: Keeps all the things.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotocore
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resotocore-3.4.2/README.md` & `resotocore-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/__main__.py` & `resotocore-3.5.0/resotocore/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,45 +21,47 @@
 from resotocore import version
 from resotocore.action_handlers.merge_outer_edge_handler import MergeOuterEdgesHandler
 from resotocore.analytics import CoreEvent, NoEventSender
 from resotocore.analytics.posthog import PostHogEventSender
 from resotocore.analytics.recurrent_events import emit_recurrent_events
 from resotocore.cli.cli import CLIService
 from resotocore.cli.command import alias_names, all_commands
-from resotocore.cli.model import CLIDependencies
+from resotocore.cli.dependencies import CLIDependencies
 from resotocore.config.config_handler_service import ConfigHandlerService
 from resotocore.config.config_override_service import ConfigOverrideService, model_from_db, override_config_for_startup
 from resotocore.config.core_config_handler import CoreConfigHandler
 from resotocore.core_config import (
     config_from_db,
     CoreConfig,
     RunConfig,
     inside_docker,
     inside_kubernetes,
     helm_installation,
     ResotoCoreConfigId,
 )
 from resotocore.db import SystemData
 from resotocore.db.db_access import DbAccess
-from resotocore.dependencies import db_access, setup_process, parse_args, system_info, reconfigure_logging, event_stream
+from resotocore.dependencies import db_access, setup_process, parse_args, system_info, reconfigure_logging
 from resotocore.error import RestartService
 from resotocore.message_bus import MessageBus
 from resotocore.model.model_handler import ModelHandlerDB
 from resotocore.model.typed_model import to_json, class_fqn
 from resotocore.query.template_expander_service import TemplateExpanderService
 from resotocore.report.inspector_service import InspectorService
 from resotocore.task.scheduler import Scheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_handler import TaskHandlerService
+from resotocore.user.user_management import UserManagementService
 from resotocore.util import shutdown_process, utc
 from resotocore.web.api import Api
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.worker_task_queue import WorkerTaskQueue
 from resotocore.infra_apps.local_runtime import LocalResotocoreAppRuntime
 from resotocore.infra_apps.package_manager import PackageManager
+from resotocore.graph_manager.graph_manager import GraphManager
 from resotolib.asynchronous.web import runner
 
 log = logging.getLogger("resotocore")
 
 
 def main() -> None:
     """
@@ -150,24 +152,25 @@
         db.configs_model_db,
         worker_task_queue,
         message_bus,
         event_sender,
         config,
         config_override_service,
     )
-    log_ship = event_stream(config, cert_handler.client_context)
+    user_management = UserManagementService(db, config_handler, event_sender)
     cli_deps = CLIDependencies(
         message_bus=message_bus,
         event_sender=event_sender,
         db_access=db,
         model_handler=model,
         worker_task_queue=worker_task_queue,
         config=config,
         config_handler=config_handler,
         cert_handler=cert_handler,
+        user_management=user_management,
     )
     default_env = {"graph": config.cli.default_graph, "section": config.cli.default_section}
     cli = CLIService(cli_deps, all_commands(cli_deps), default_env, alias_names())
     template_expander = TemplateExpanderService(db.template_entity_db, cli)
     cli_deps.extend(template_expander=template_expander)
     inspector = InspectorService(cli)
     subscriptions = SubscriptionHandler(db.subscribers_db, message_bus)
@@ -177,30 +180,35 @@
     core_config_handler = CoreConfigHandler(
         config, message_bus, worker_task_queue, config_handler, event_sender, inspector
     )
     merge_outer_edges_handler = MergeOuterEdgesHandler(message_bus, subscriptions, task_handler, db, model)
     cli_deps.extend(task_handler=task_handler, inspector=inspector)
     infra_apps_runtime = LocalResotocoreAppRuntime(cli)
     cli_deps.extend(infra_apps_runtime=infra_apps_runtime)
-    infra_apps_package_manager = PackageManager(db.package_entity_db, config_handler)
+    infra_apps_package_manager = PackageManager(
+        db.package_entity_db, config_handler, cli.register_alias_template, cli.unregister_alias_template
+    )
     cli_deps.extend(infra_apps_package_manager=infra_apps_package_manager)
+    graph_manager = GraphManager(db, config.snapshots, core_config_handler, task_handler)
+    cli_deps.extend(graph_manager=graph_manager)
     api = Api(
         db,
         model,
         subscriptions,
         task_handler,
         message_bus,
         event_sender,
         worker_task_queue,
         cert_handler,
         config_handler,
         inspector,
         cli,
         template_expander,
         config,
+        user_management,
         config_override_service.get_override,
     )
     event_emitter = emit_recurrent_events(
         event_sender, model, subscriptions, worker_task_queue, message_bus, timedelta(hours=1), timedelta(hours=1)
     )
 
     async def on_start() -> None:
@@ -216,17 +224,17 @@
         await inspector.start()
         await task_handler.start()
         await config_override_service.start()
         await config_handler.start()
         await core_config_handler.start()
         await merge_outer_edges_handler.start()
         await cert_handler.start()
-        await log_ship.start()
         await api.start()
         await infra_apps_package_manager.start()
+        await graph_manager.start()
         if created:
             docker = inside_docker()
             kubernetes = inside_kubernetes()
             helm = helm_installation()
             await event_sender.core_event(
                 CoreEvent.SystemInstalled,
                 {
@@ -248,17 +256,17 @@
             cpu_count=info.cpus,
             mem_total=info.mem_total,
             mem_available=info.mem_available,
         )
 
     async def on_stop() -> None:
         duration = utc() - info.started_at
+        await graph_manager.stop()
         await infra_apps_package_manager.stop()
         await api.stop()
-        await log_ship.stop()
         await cert_handler.stop()
         await config_override_service.stop()
         await core_config_handler.stop()
         await merge_outer_edges_handler.stop()
         await task_handler.stop()
         await inspector.stop()
         await cli.stop()
```

### Comparing `resotocore-3.4.2/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.5.0/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/analytics/__init__.py` & `resotocore-3.5.0/resotocore/analytics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     WorkerQueueInfo = "worker-queue.info"
     TaskStarted = "task-handler.task-started"
     TaskCompleted = "task-handler.task-completed"
     ClientError = "error.client"
     ServerError = "error.server"
     UsageMetricsTurnedOff = "usage-metrics.turned-off"
     BenchmarkPerformed = "report.benchmark"
+    FirstUserCreated = "user.created.first"
+    UserCreated = "user.created"
 
 
 @define(frozen=True)
 class AnalyticsEvent:
     system: str  # e.g. creator of the event: resotocore, resotoui, resotosh, etc.
     kind: str  # kind of the event. Every kind has a specific set of data and context vars
     context: Mapping[str, JsonElement]  # context properties
```

### Comparing `resotocore-3.4.2/resotocore/analytics/posthog.py` & `resotocore-3.5.0/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/analytics/recurrent_events.py` & `resotocore-3.5.0/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/async_extensions.py` & `resotocore-3.5.0/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/cli/__init__.py` & `resotocore-3.5.0/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/cli/cli.py` & `resotocore-3.5.0/resotocore/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,29 +41,28 @@
 )
 from resotocore.cli.model import (
     ParsedCommand,
     ParsedCommands,
     ExecutableCommand,
     ParsedCommandLine,
     CLICommand,
-    CLIDependencies,
     InternalPart,
     CLIContext,
     CLI,
     EmptyContext,
     CLISource,
     NoTerminalOutput,
+    OutputTransformer,
+    PreserveOutputFormat,
     AliasTemplate,
     ArgsInfo,
     ArgInfo,
     AliasTemplateParameter,
-    WorkerCustomCommand,
-    OutputTransformer,
-    PreserveOutputFormat,
 )
+from resotocore.cli.dependencies import CLIDependencies
 from resotocore.console_renderer import ConsoleRenderer
 from resotocore.error import CLIParseError
 from resotocore.model.typed_model import class_fqn
 from resotocore.query.model import (
     Query,
     Navigation,
     AllTerm,
@@ -254,23 +253,29 @@
     def dependencies(self) -> CLIDependencies:
         return self.__dependencies
 
     @property
     def alias_templates(self) -> Dict[str, AliasTemplate]:
         return self.__alias_templates
 
-    def register_worker_custom_command(self, command: WorkerCustomCommand) -> None:
+    def register_alias_template(self, template: AliasTemplate) -> None:
         """
-        Called when a worker connects that introduces a custom command.
+        Called when something introduces a custom command.
         The registered templated will always override any existing template.
         """
-        if command.name not in self.direct_commands and command.name not in self.alias_commands:
-            template = command.to_template()
+        if template.name not in self.direct_commands and template.name not in self.alias_commands:
             self.alias_templates[template.name] = template
 
+    def unregister_alias_template(self, name: str) -> None:
+        """
+        Called when something removes a custom command.
+        """
+        if name in self.alias_templates:
+            del self.alias_templates[name]
+
     async def start(self) -> None:
         self.reaper = asyncio.create_task(self.reap_tasks())
 
     async def stop(self) -> None:
         if self.reaper:
             self.reaper.cancel()
             await asyncio.gather(self.reaper, return_exceptions=True)
@@ -519,15 +524,15 @@
             return ParsedCommandLine(ctx, parsed, rewritten, not_met, envelope)
 
         def expand_aliases(line: ParsedCommands) -> ParsedCommands:
             def expand_alias(alias_cmd: ParsedCommand) -> List[ParsedCommand]:
                 alias: AliasTemplate = self.alias_templates[alias_cmd.cmd]
                 available: Dict[str, AliasTemplateParameter] = {p.name: p for p in alias.parameters}
                 props: Dict[str, JsonElement] = self.replacements(**{**self.cli_env, **context.env})  # type: ignore
-                props["args"] = alias_cmd.args
+                props["args"] = alias_cmd.args or ""
                 for p in alias.parameters:
                     props[p.name] = p.default
                 # only parse properties, if there are any declared
                 if alias.parameters:
                     args = (alias_cmd.args or "").strip()
                     parser = args_values_parser if args.startswith("--") else key_values_parser
                     props.update(parser.parse(args))
```

### Comparing `resotocore-3.4.2/resotocore/cli/command.py` & `resotocore-3.5.0/resotocore/cli/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 from aiohttp import ClientTimeout, JsonPayload, BasicAuth
 from aiostream import stream, pipe
 from aiostream.aiter_utils import is_async_iterable
 from aiostream.core import Stream
 from attrs import define, field
 from dateutil import parser as date_parser
 from parsy import Parser, string
+from rich.padding import Padding
+from rich.panel import Panel
+from rich.table import Table
+from rich.text import Text
+
 from resotocore import version
 from resotocore.async_extensions import run_async
 from resotocore.cli import (
     JsGen,
     NoExitArgumentParser,
     args_parts_parser,
     args_parts_unquoted_parser,
@@ -70,31 +75,31 @@
     CLISource,
     CLIFlow,
     InternalPart,
     OutputTransformer,
     PreserveOutputFormat,
     MediaType,
     CLIFileRequirement,
-    CLIDependencies,
     ParsedCommand,
     NoTerminalOutput,
     ArgsInfo,
     ArgInfo,
 )
+from resotocore.cli.dependencies import CLIDependencies
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.db.graphdb import HistoryChange
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
-from resotocore.infra_apps.package_manager import Failure
-from resotocore.infra_apps.manifest import AppManifest
 from resotocore.dependencies import system_info
 from resotocore.error import CLIParseError, ClientError, CLIExecutionError
-from resotocore.ids import ConfigId, TaskId, InfraAppName, TaskDescriptorId, GraphName
+from resotocore.ids import ConfigId, TaskId, InfraAppName, TaskDescriptorId, GraphName, Email, Password
+from resotocore.infra_apps.manifest import AppManifest
+from resotocore.infra_apps.package_manager import Failure
 from resotocore.model.graph_access import Section, EdgeTypes
 from resotocore.model.model import (
     Model,
     Kind,
     ComplexKind,
     DictionaryKind,
     SimpleKind,
@@ -117,14 +122,15 @@
 )
 from resotocore.query.query_parser import parse_query, aggregate_parameter_parser
 from resotocore.query.template_expander import tpl_props_p
 from resotocore.report import BenchmarkConfigPrefix, ReportSeverity
 from resotocore.report.benchmark_renderer import respond_benchmark_result
 from resotocore.task.task_description import Job, TimeTrigger, EventTrigger, ExecuteCommand, Workflow, RunningTask
 from resotocore.types import Json, JsonElement, EdgeType
+from resotocore.user import ResotoUser, ValidRoles
 from resotocore.util import (
     uuid_str,
     utc,
     if_set,
     duration,
     identity,
     rnd_str,
@@ -151,18 +157,14 @@
     comma_p,
     variable_p,
     equals_p,
     json_value_p,
 )
 from resotolib.utils import safe_members_in_tarfile, get_local_tzinfo
 from resotolib.x509 import write_cert_to_file, write_key_to_file
-from rich.padding import Padding
-from rich.panel import Panel
-from rich.table import Table
-from rich.text import Text
 
 log = logging.getLogger(__name__)
 
 
 # A SearchCLIPart is a command that can be used on the command line.
 # Such a part is not executed, but builds a search, which is executed.
 # Therefore, the parse method is implemented in a dummy fashion here.
@@ -3145,15 +3147,15 @@
             def with_dependencies(model: Model) -> Stream:
                 load = self.load_by_id_merged(model, in_stream, variables, allowed_on_kind, **ctx.env)
                 handler = self.update_node_in_graphdb(model, **ctx.env) if expect_node_result else self.no_update
                 return self.send_to_queue_stream(stream.map(load, fn), handler, True)
 
             # dependencies are not resolved directly (no async function is allowed here)
             async def load_model() -> Model:
-                return await self.dependencies.model_handler.load_model(ctx.graph_name)
+                return await cast(CLIDependencies, self.dependencies).model_handler.load_model(ctx.graph_name)
 
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
         def setup_source() -> Stream:
             arg = {"args": args_parts_unquoted_parser.parse(formatter({}))}
             return self.send_to_queue_stream(stream.just((command_name, {}, arg)), self.no_update, True)
@@ -3268,15 +3270,15 @@
         def setup_stream(in_stream: Stream) -> Stream:
             def with_dependencies(model: Model) -> Stream:
                 load = self.load_by_id_merged(model, in_stream, variables, **ctx.env)
                 result_handler = self.update_node_in_graphdb(model, **ctx.env)
                 return self.send_to_queue_stream(stream.map(load, fn), result_handler, not ns.nowait)
 
             async def load_model() -> Model:
-                return await self.dependencies.model_handler.load_model(ctx.graph_name)
+                return await cast(CLIDependencies, self.dependencies).model_handler.load_model(ctx.graph_name)
 
             # dependencies are not resolved directly (no async function is allowed here)
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
         return CLIFlow(setup_stream)
 
@@ -3543,15 +3545,15 @@
 
             # create a background task, so that the current request can be executed completely
             asyncio.create_task(wait_and_exit())
 
     @staticmethod
     async def show_system_info() -> AsyncIterator[Json]:
         info = to_js(system_info())
-        yield {**{"name": "resotocore"}, **info}
+        yield {"name": "resotocore", **info}
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         parts = re.split(r"\s+", arg if arg else "")
         if len(parts) >= 2 and parts[0] == "backup" and parts[1] == "create":
             rest = parts[2:]
 
             def backup() -> AsyncIterator[str]:
@@ -3915,15 +3917,15 @@
 
         async def perform_request(e: JsonElement) -> int:
             nonlocal retries_left
             data = None if template.no_body else (JsonPayload(e) if isinstance(e, (dict, list)) else e)
             authuser, authpass = template.auth.split(":", 1) if template.auth else (None, None)
             log.debug(f"Perform request with this template={template} and data={data}")
             try:
-                async with self.dependencies.http_session.request(
+                async with cast(CLIDependencies, self.dependencies).http_session.request(
                     template.method,
                     template.url,
                     headers=template.headers,
                     params=template.params,
                     data=data,
                     compress=template.compress,
                     timeout=template.timeout,
@@ -4262,22 +4264,25 @@
 class ConfigsCommand(CLICommand):
     """
     ```shell
     configs list
     configs show <cfg_id>
     configs set <cfg_id> <prop>=<value> [, <prop>=<value>]
     configs edit <cfg_id>
+    configs copy <cfg_id> <new_cfg_id>
     configs update <cfg_id> <path>
     configs delete <cfg_id>
     ```
 
     - `configs list`: get the list of all config ids in the system.
     - `configs show <cfg_id>`: show the configuration with provided identifier.
     - `configs set <cfg_id> <prop>=<value>`: set one or more property values in the configuration with provided id.
     - `configs edit <cfg_id>`: edit the complete configuration with provided id as file
+    - `configs copy <cfg_id> <new_cfg_id>`: copy the configuration with provided id
+       to a new configuration with the provided new id.
     - `configs update <cfg_id> <path>`: update or create the configuration with provided id with content of given file.
     - `configs delete <cfg_id>`: delete the configuration with given identifier.
 
     ## Parameters
     - cfg_id [mandatory]: The identifier of the configuration.
     - prop: the path of the property to set. Nested properties can be accessed via `.`.
     - value: the value of the property path to set. It can be any json conform element.
@@ -4310,14 +4315,17 @@
     # This will open the configuration in your local editor.
     # Once the editor is closed, the configuration is updated.
     > config edit test
 
     # Update the configuration test by loading the provided config file.
     > config update test /path/to/my/local/config.yaml
 
+    # Copy the configuration test to a new configuration test2.
+    > config copy test test2
+
     # Get the list of all configuration keys.
     > config list
     config_test
     resoto.core
     resoto.worker.1
     resoto.worker.2
     resoto.metrics
@@ -4337,14 +4345,15 @@
 
     def args_info(self) -> ArgsInfo:
         return {
             "list": [],
             "set": [ArgInfo(None, expects_value=True, help_text="<config_id> <key>=<value>")],
             "show": [ArgInfo(None, expects_value=True, help_text="<config_id> e.g. resoto.core")],
             "edit": [ArgInfo(None, expects_value=True, help_text="<config_id>")],
+            "copy": [ArgInfo(None, expects_value=True, help_text="<config_id> <new_config_id>")],
             "update": [
                 ArgInfo(None, expects_value=True, help_text="<config_id> /path/to/config.yaml", value_hint="file")
             ],
             "delete": [ArgInfo(None, expects_value=True, help_text="<config_id>")],
         }
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
@@ -4379,14 +4388,21 @@
             # 1) download the config and make it available to edit
             # 2) upload the config file and update the config from content --> update_config
             yml = await self.dependencies.config_handler.config_yaml(cfg_id, revision=True)
             if not yml:
                 raise AttributeError(f"No config with this id: {cfg_id}")
             return send_file(yml)
 
+        async def copy_config(from_cfg_id: ConfigId, to_cfg_id: ConfigId) -> AsyncIterator[str]:
+            cfg = await self.dependencies.config_handler.get_config(from_cfg_id)
+            if not cfg:
+                raise AttributeError(f"No config with this id: {from_cfg_id}")
+            await self.dependencies.config_handler.copy_config(from_cfg_id, to_cfg_id)
+            yield f"Config {from_cfg_id} has been copied to {to_cfg_id}."
+
         async def update_config(cfg_id: ConfigId) -> AsyncIterator[str]:
             # Usually invoked by resh automatically via edit_config, but can also be triggered manually.
             # A config with given id is changed by the content of uploaded file "config"
             try:
                 content = ""
                 async with aiofiles.open(ctx.uploaded_files["config.yaml"], "r") as f:
                     content = await f.read()
@@ -4418,14 +4434,16 @@
         elif arg and len(args) == 2 and args[0] == "edit":
             config_id = args[1]
             return CLISource.single(
                 partial(edit_config, config_id),
                 produces=MediaType.FilePath,
                 envelope={"Resoto-Shell-Action": "edit", "Resoto-Shell-Command": f"configs update {config_id}"},
             )
+        elif arg and len(args) == 3 and args[0] == "copy":
+            return CLISource.single(partial(copy_config, args[1], args[2]))
         elif arg and len(args) == 3 and args[0] == "update":
             config_id = args[1]
             return CLISource.single(
                 partial(update_config, config_id),
                 produces=MediaType.FilePath,
                 envelope={"Resoto-Shell-Action": "edit", "Resoto-Shell-Command": f"configs update {config_id}"},
                 requires=[CLIFileRequirement("config.yaml", args[2])],
@@ -4761,15 +4779,15 @@
         async def list_benchmarks() -> AsyncIterator[str]:
             for benchmark in await self.dependencies.inspector.list_benchmarks():
                 yield benchmark.id
 
         async def show_benchmark(bid: str) -> AsyncIterator[Optional[str]]:
             yield await self.dependencies.config_handler.config_yaml(ConfigId(BenchmarkConfigPrefix + bid))
 
-        async def show_check(cid: str) -> AsyncIterator[Json]:
+        async def show_check(cid: str) -> AsyncIterator[str]:
             model = await self.dependencies.config_handler.get_configs_model()
             kind = model.get("resoto_core_report_check")
             for check in await self.dependencies.inspector.list_checks(check_ids=[cid]):
                 yield kind.create_yaml(to_js(check)) if isinstance(kind, ComplexKind) else yaml.safe_dump(to_js(check))
 
         async def list_checks() -> AsyncIterator[str]:
             for check in await self.dependencies.inspector.list_checks():
@@ -4966,45 +4984,43 @@
                     yield f"App {name} updated sucessfully to the latest version ({result.version})"
 
         async def apps_list() -> AsyncIterator[JsonElement]:
             async for app in self.dependencies.infra_apps_package_manager.list():
                 yield app
 
         async def app_run(
-            in_stream: JsGen, app_name: InfraAppName, dry_run: bool, config: Optional[str]
+            in_stream: JsGen, app_name: InfraAppName, dry_run: bool, config: Optional[str], argv: List[str]
         ) -> AsyncIterator[JsonElement]:
-            runtime = self.dependencies.infra_apps_runtime
+            runtime = cast(CLIDependencies, self.dependencies).infra_apps_runtime
             manifest = await self.dependencies.infra_apps_package_manager.get_manifest(app_name)
             if not manifest:
                 raise ValueError(f"App {app_name} is not installed.")
             app_config = None
-            if config:
-                ce = await self.dependencies.config_handler.get_config(ConfigId(config))
-                if ce:
-                    app_config = ce.config
-                else:
-                    raise ValueError(f"Config {config} not found.")
+            config = config or f"resoto.apps.{app_name}"
+            ce = await self.dependencies.config_handler.get_config(ConfigId(config))
+            if ce:
+                app_config = ce.config
             else:
-                app_config = manifest.default_config or {}
+                raise ValueError(f"Config {config} not found.")
 
             stdin: AsyncIterator[JsonElement] = (
                 stream.iterate(in_stream) if isinstance(in_stream, Stream) else in_stream
             )
 
             if dry_run:
                 return runtime.generate_template(
                     graph=ctx.graph_name,
                     manifest=manifest,
                     config=app_config,
                     stdin=stdin,
-                    kwargs=Namespace(),
+                    argv=argv,
                 )
             else:
                 return runtime.execute(
-                    graph=ctx.graph_name, manifest=manifest, config=app_config, stdin=stdin, kwargs=Namespace(), ctx=ctx
+                    graph=ctx.graph_name, manifest=manifest, config=app_config, stdin=stdin, argv=argv, ctx=ctx
                 )
 
         args = re.split("\\s+", arg, maxsplit=2) if arg else []
         if len(args) == 1 and args[0] == "search":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("--index-url", dest="url", type=str)
@@ -5064,38 +5080,417 @@
             return CLISource.single(apps_list)
         elif len(args) >= 2 and args[0] == "run":
             parser = NoExitArgumentParser()
             parser.add_argument("command", type=str)
             parser.add_argument("app_name", type=str)
             parser.add_argument("--dry-run", dest="dry_run", action="store_true", default=False)
             parser.add_argument("--config", dest="config", type=str, default=None)
-            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            parsed, argv = parser.parse_known_args(args_parts_parser.parse(arg))
 
             in_source_position = kwargs.get("position") == 0
 
             if in_source_position:
                 return CLISource.no_count(
                     partial(
                         app_run,
                         in_stream=stream.empty(),
                         app_name=InfraAppName(parsed.app_name),
                         dry_run=parsed.dry_run,
                         config=parsed.config,
+                        argv=argv,
                     )
                 )
             else:
                 return CLIFlow(
                     partial(
-                        app_run, app_name=InfraAppName(parsed.app_name), dry_run=parsed.dry_run, config=parsed.config
+                        app_run,
+                        app_name=InfraAppName(parsed.app_name),
+                        dry_run=parsed.dry_run,
+                        config=parsed.config,
+                        argv=argv,
                     )
                 )
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
+class UserCommand(CLICommand):
+    """
+    ```shell
+    user add <email> --fullname <name> --password <secret> --role <role> --role <role>
+    user delete <email>
+    user role add <email> <role>
+    user role delete <email> <role>
+    user password <email> <password>
+    user list
+    user show <email>
+    ```
+
+    Manage the database of users.
+
+    Note: the user database is stored as configuration item in the configuration store.
+    The password of the user is stored as hash using pbkdf2_hmac with sha512 and 210000 iterations.
+    It is stored in /etc/shadow format.
+    It is possible to maintain the user database externally by using config overrides.
+
+    Every user uses the email address as unique identifier.
+    Email + password is used for authentication.
+    The allowed actions of a user are defined by the roles assigned to the user.
+
+    ## Parameters
+    - `<email>`: The email address of the user.
+    - `--fullname` - Full name of the user
+    - `--password` - Password of the user
+    - `--role` - Role of the user. Can be repeated multiple times.
+
+    ## Examples
+    ```shell
+    # Add a user with a given name and read-only role. The password will be stored as hash.
+    > users add matthias@some.engineering --fullname "Matthias Veit" --role read-only --password changeme
+    email: matthias@some.engineering
+    fullname: Matthias Veit
+    roles:
+    - read-only
+
+    # List all users of the system.
+    > user list
+    admin@some.engineering
+    matthias@some.engineering
+    test@test.de
+
+    # Show a specific user.
+    > users show matthias@some.engineering
+    email: matthias@some.engineering
+    fullname: Matthias Veit
+    roles:
+    - read-only
+
+    # Add a role to a user.
+    > user role add matthias@some.engineering admin
+    email: matthias@some.engineering
+    fullname: Matthias Veit
+    roles:
+    - read-only
+    - admin
+
+    # Remove a role from a user.
+    > user role delete matthias@some.engineering admin
+    email: matthias@some.engineering
+    fullname: Matthias Veit
+    roles:
+    - read-only
+
+    # Change the password of a user.
+    > user password matthias@some.engineering bombproof
+    Password for matthias@some.engineering updated
+
+    # Delete a user.
+    > user delete matthias@some.engineering
+    User matthias@some.engineering deleted
+    """
+
+    @property
+    def name(self) -> str:
+        return "user"
+
+    def args_info(self) -> ArgsInfo:
+        return {
+            "add": [
+                ArgInfo(None, True, help_text="<email>"),
+                ArgInfo("--fullname", True, help_text="<name>"),
+                ArgInfo("--password", True, help_text="<secret>"),
+                ArgInfo(
+                    "--role",
+                    True,
+                    help_text="<role>",
+                    possible_values=list(ValidRoles),
+                    can_occur_multiple_times=True,
+                ),
+            ],
+            "delete": [
+                ArgInfo(None, True, help_text="<email>"),
+            ],
+            "role": {
+                "add": [
+                    ArgInfo(None, True, help_text="<email>"),
+                    ArgInfo(None, True, help_text="<role>"),
+                ],
+                "delete": [
+                    ArgInfo(None, True, help_text="<email>"),
+                    ArgInfo(None, True, help_text="<role>"),
+                ],
+            },
+            "password": [ArgInfo(None, True, help_text="<email>"), ArgInfo(None, True, help_text="<password>")],
+            "list": [ArgInfo(None, False)],
+            "show": [ArgInfo(None, True, help_text="<email>")],
+        }
+
+    def info(self) -> str:
+        return "Manage users"
+
+    @staticmethod
+    def user_to_json(email: Email, user: ResotoUser) -> JsonElement:
+        return {
+            "email": email,
+            "fullname": user.fullname,
+            "roles": list(user.roles),
+        }
+
+    async def add_user(
+        self, email: Email, fullname: str, password: Password, roles: List[str]
+    ) -> AsyncIterator[JsonElement]:
+        user = await self.dependencies.user_management.create_user(email, fullname, password, roles)
+        yield self.user_to_json(email, user)
+
+    async def delete_user(self, email: Email) -> AsyncIterator[JsonElement]:
+        await self.dependencies.user_management.delete_user(email)
+        yield f"User {email} deleted"
+
+    async def add_roles(self, email: Email, role: str) -> AsyncIterator[JsonElement]:
+        if user := await self.dependencies.user_management.user(email):
+            updated = user.roles.union({role})
+            user = await self.dependencies.user_management.update_user(email, roles=list(updated))
+            yield self.user_to_json(email, user)
+        else:
+            raise AttributeError(f"User {email} not found")
+
+    async def delete_role(self, email: Email, role: str) -> AsyncIterator[JsonElement]:
+        if user := await self.dependencies.user_management.user(email):
+            updated = user.roles.difference({role})
+            user = await self.dependencies.user_management.update_user(email, roles=list(updated))
+            yield self.user_to_json(email, user)
+        else:
+            raise AttributeError(f"User {email} not found")
+
+    async def change_password(self, email: Email, password: Password) -> AsyncIterator[JsonElement]:
+        await self.dependencies.user_management.update_user(email, password=password)
+        yield f"Password for {email} updated"
+
+    async def list_users(self) -> AsyncIterator[JsonElement]:
+        for email in await self.dependencies.user_management.users():
+            yield email
+
+    async def show_user(self, email: Email) -> AsyncIterator[JsonElement]:
+        if user := await self.dependencies.user_management.user(email):
+            yield self.user_to_json(email, user)
+        else:
+            raise AttributeError(f"User {email} not found")
+
+    def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
+        args = args_parts_unquoted_parser.parse(arg.strip()) if arg else []
+        if len(args) >= 2 and args[0] == "add":
+            parser = NoExitArgumentParser()
+            parser.add_argument("email", type=str)
+            parser.add_argument("--fullname", type=str, required=True)
+            parser.add_argument("--password", type=str, required=True)
+            parser.add_argument("--role", type=str, action="append", required=True)
+            parsed = parser.parse_args(args[1:])
+            return CLISource.single(
+                partial(self.add_user, Email(parsed.email), parsed.fullname, Password(parsed.password), parsed.role)
+            )
+        elif len(args) == 2 and args[0].startswith("del"):
+            return CLISource.single(partial(self.delete_user, Email(args[1])))
+        elif len(args) > 3 and args[0] == "role" and args[1] == "add":
+            return CLISource.single(partial(self.add_roles, Email(args[2]), args[3]))
+        elif len(args) > 3 and args[0] == "role" and args[1].startswith("del"):
+            return CLISource.single(partial(self.delete_role, Email(args[2]), args[3]))
+        elif len(args) >= 3 and args[0] in ("passwd", "password"):
+            return CLISource.single(partial(self.change_password, Email(args[1]), Password(args[2])))
+        elif len(args) == 1 and args[0] == "list":
+            return CLISource.no_count(self.list_users)
+        elif len(args) == 2 and args[0] == "show":
+            return CLISource.no_count(partial(self.show_user, args[1]))
+        else:
+            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+
+
+class GraphCommand(CLICommand):
+    """
+    ```shell
+    graph list [pattern]
+    graph copy [-force] [from_graph_namae] <to_graph_name>
+    graph snapshot [from_graph_name] <snapshot_label>
+    graph delete <graph_name>
+    graph export [--force] [graph_name] <file_name>
+    graph import [--force] [graph_name] <file_name>
+    ```
+
+    - `graph list [pattern]`: Lists all graphs. Supports filtering by pattern.
+    - `graph copy [--force] [from_graph_name] <to_graph_name>`: Copies the graph.
+       If the target graph alearly exists, and a --force flag is provided, the graph will be overwritten.
+    - `graph snapshot [from_graph_name] <snapshot_label>`: Make a graph snapshot.
+    - `graph delete <graph_name>`: Delete a graph.
+    - `graph export [--force] [graph_name] <file_name>`: Export the graph into a file. If the file already exists,
+       and a --force flag is provided, the file will be overwritten.
+    - `graph import [--force] [graph_name] <file_name>`: Impor the graph from a file. If the graph already exists,
+       and a --force flag is provided, the graph will be overwritten.
+
+    ## Parameters
+    - `pattern` [optional]: Pattern for searching for graps. Supports regex.
+    - `from_graph_name` [required]: The name of the graph to make a copy or snapshot from.
+    - `to_graph_name` [optional]: The name of the target graph to make a copy.
+       If not specified, the name of the current graph is used.
+    - `file_name` [required]: The name of the file to save the graph to.
+
+    ## Options
+    - `--force`: Overwrite the target graph or file if it already exists.
+    """
+
+    @property
+    def name(self) -> str:
+        return "graph"
+
+    def info(self) -> str:
+        return "Operations on graphs."
+
+    def args_info(self) -> ArgsInfo:
+        return {
+            "list": [
+                ArgInfo(None, True, help_text="<pattern>"),
+            ],
+            "copy": [
+                ArgInfo(None, True, help_text="<from_graph_name>"),
+                ArgInfo(None, True, help_text="<to_graph_name>"),
+                ArgInfo("--force", False),
+            ],
+            "snapshot": [
+                ArgInfo(None, True, help_text="<from_graph_name>"),
+                ArgInfo(None, True, help_text="<to_graph_name>"),
+            ],
+            "delete": [
+                ArgInfo(None, True, help_text="<graph_name>"),
+            ],
+            "export": [
+                ArgInfo(None, True, help_text="<from_graph_name>"),
+                ArgInfo(None, True, help_text="<to_graph_name>"),
+                ArgInfo("--force", False),
+            ],
+            "import": [
+                ArgInfo(None, True, help_text="<from_graph_name>"),
+                ArgInfo(None, True, help_text="<to_graph_name>"),
+                ArgInfo("--force", False),
+            ],
+        }
+
+    def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
+        async def graph_list(pattern: Optional[str]) -> AsyncIterator[JsonElement]:
+            graphs = await self.dependencies.graph_manager.list(pattern)
+            for graph in graphs:
+                yield graph
+
+        async def graph_copy(
+            source: Optional[GraphName], destination: GraphName, force: bool
+        ) -> AsyncIterator[JsonElement]:
+            if not source:
+                source = ctx.graph_name
+            result_name = await self.dependencies.graph_manager.copy(source, destination, replace_existing=force)
+            yield f"Graph {source} copied to {result_name}."
+
+        async def graph_snapshot(source: Optional[GraphName], label: str) -> AsyncIterator[JsonElement]:
+            if not source:
+                source = ctx.graph_name
+            snapshot_name = await self.dependencies.graph_manager.snapshot(source, label)
+            yield f"Graph {source} snapshoted to {snapshot_name}."
+
+        async def graph_delete(graph_name: GraphName) -> AsyncIterator[JsonElement]:
+            await self.dependencies.graph_manager.delete(graph_name)
+            yield f"Graph {graph_name} deleted."
+
+        async def write_result_to_file(export_lines: AsyncIterator[str], file_name: str) -> AsyncIterator[str]:
+            temp_dir: str = tempfile.mkdtemp()
+            path = os.path.join(temp_dir, file_name)
+            try:
+                async with aiofiles.open(path, "w") as f:
+                    async for line in export_lines:
+                        await f.write(line + "\n")
+                yield path
+            finally:
+                shutil.rmtree(temp_dir)
+
+        async def graph_export(graph_name: Optional[GraphName], file_name: str) -> AsyncIterator[JsonElement]:
+            if not graph_name:
+                graph_name = ctx.graph_name
+            lines = self.dependencies.graph_manager.export_graph(graph_name)
+            return write_result_to_file(lines, file_name)
+
+        async def graph_import(
+            graph_name: Optional[GraphName], file_name: str, force: bool
+        ) -> AsyncIterator[JsonElement]:
+            if not graph_name:
+                graph_name = ctx.graph_name
+
+            path = ctx.uploaded_files.get("dump")
+            if not path:
+                raise ValueError(f"File {file_name} was not uploaded.")
+
+            async with aiofiles.open(path, "r") as f:
+
+                async def lines_iterator() -> AsyncIterator[str]:
+                    async for line in f:
+                        yield line.strip()
+
+                await self.dependencies.graph_manager.import_graph(graph_name, lines_iterator(), replace_existing=force)
+            yield f"Graph {graph_name} imported from {file_name}."
+
+        args = re.split("\\s+", arg, maxsplit=2) if arg else []
+        if args[0] == "list":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("pattern", type=str, nargs="?", default=None)
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            return CLISource.single(partial(graph_list, parsed.pattern))
+        elif args[0] == "copy":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("source", type=str, nargs="?", default=None)
+            parser.add_argument("destination", type=str)
+            parser.add_argument("--force", action="store_true")
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            return CLISource.single(
+                partial(graph_copy, GraphName(parsed.source), GraphName(parsed.destination), parsed.force)
+            )
+        elif args[0] == "snapshot":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("source", type=str, nargs="?", default=None)
+            parser.add_argument("label", type=str)
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            return CLISource.single(partial(graph_snapshot, parsed.source, parsed.label))
+        elif args[0] == "delete":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("graph_name", type=str)
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            return CLISource.single(partial(graph_delete, GraphName(parsed.graph_name)))
+        elif args[0] == "export":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("graph_name", type=str, nargs="?", default=None)
+            parser.add_argument("file_name", type=str)
+            parser.add_argument("--force", action="store_true")
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+            return CLISource.single(partial(graph_export, parsed.graph_name, parsed.file_name), MediaType.FilePath)
+        elif args[0] == "import":
+            parser = NoExitArgumentParser()
+            parser.add_argument("command", type=str)
+            parser.add_argument("graph_name", type=str, nargs="?", default=None)
+            parser.add_argument("file_name", type=str)
+            parser.add_argument("--force", action="store_true")
+            parsed = parser.parse_args(strip_quotes(arg or "").split())
+
+            return CLISource.single(
+                partial(graph_import, parsed.graph_name, parsed.file_name, parsed.force),
+                MediaType.Json,
+                [CLIFileRequirement("dump", parsed.file_name)],
+            )
+
+        else:
+            return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
+
+
 def all_commands(d: CLIDependencies) -> List[CLICommand]:
     commands = [
         AggregateCommand(d, "search"),
         AggregateToCountCommand(d, "search"),
         AncestorsPart(d, "search"),
         CertificateCommand(d, "setup", allowed_in_source_position=True),
         ChunkCommand(d, "misc"),
@@ -5129,19 +5524,21 @@
         SleepCommand(d, "misc", allowed_in_source_position=True),
         SortPart(d, "search"),
         SuccessorsPart(d, "search"),
         SystemCommand(d, "setup", allowed_in_source_position=True),
         TagCommand(d, "action"),
         TailCommand(d, "misc"),
         UniqCommand(d, "misc"),
+        UserCommand(d, "setup", allowed_in_source_position=True),
         WorkflowsCommand(d, "action", allowed_in_source_position=True),
         WelcomeCommand(d, "misc", allowed_in_source_position=True),
         TipOfTheDayCommand(d, "misc", allowed_in_source_position=True),
         WriteCommand(d, "misc"),
         InfrastructureAppsCommand(d, "apps", allowed_in_source_position=True),
+        GraphCommand(d, "graph", allowed_in_source_position=True),
     ]
     # commands that are only available when the system is started in debug mode
     if d.config.runtime.debug:
         commands.extend(
             [
                 FileCommand(d, "misc"),
                 UploadCommand(d, "misc"),
@@ -5166,8 +5563,9 @@
         "ancestor": "ancestors",
         "job": "jobs",
         "lists": "list",
         "template": "templates",
         "workflow": "workflows",
         "app": "apps",
         "man": "help",
+        "users": "user",
     }
```

### Comparing `resotocore-3.4.2/resotocore/cli/model.py` & `resotocore-3.5.0/resotocore/cli/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 from __future__ import annotations
 
 import calendar
 import inspect
 import json
 from abc import ABC, abstractmethod
-from asyncio import Queue, Task, iscoroutine
+from asyncio import iscoroutine
 from datetime import timedelta
 from enum import Enum
 from functools import reduce
 from operator import attrgetter
 from textwrap import dedent
 from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set, AsyncIterator
 
-from aiohttp import ClientSession, TCPConnector
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import define, field
 from parsy import test_char, string
 from rich.jupyter import JupyterMixin
 
-from resotocore.analytics import AnalyticsEventSender
 from resotocore.cli import JsGen, T, Sink
-from resotocore.config import ConfigHandler
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
-from resotocore.core_config import CoreConfig, AliasTemplateConfig, AliasTemplateParameterConfig
-from resotocore.db.db_access import DbAccess
+from resotocore.core_config import AliasTemplateConfig, AliasTemplateParameterConfig
 from resotocore.error import CLIParseError
-from resotocore.message_bus import MessageBus
-from resotocore.model.model_handler import ModelHandler
+from resotocore.query.template_expander import render_template
 from resotocore.query.model import Query, variable_to_absolute, PathRoot
-from resotocore.query.template_expander import TemplateExpander, render_template
-from resotocore.report import Inspector
-from resotocore.task import TaskHandler
 from resotocore.types import Json, JsonElement
 from resotocore.ids import GraphName
 from resotocore.util import AccessJson, uuid_str, from_utc, utc, utc_str
-from resotocore.web.certificate_handler import CertificateHandler
-from resotocore.worker_task_queue import WorkerTaskQueue
-from resotocore.infra_apps.runtime import Runtime
-from resotocore.infra_apps.package_manager import PackageManager
 from resotolib.parse_util import l_curly_dp, r_curly_dp
 from resotolib.utils import get_local_tzinfo
 
 
 class MediaType(Enum):
     Json = 1
     FilePath = 2
@@ -159,96 +147,14 @@
     @abstractmethod
     async def evaluate_cli_command(
         self, cli_input: str, context: CLIContext = EmptyContext, replace_place_holder: bool = True
     ) -> List[ParsedCommandLine]:
         pass
 
 
-class CLIDependencies:
-    def __init__(self, **deps: Any) -> None:
-        self.lookup: Dict[str, Any] = deps
-
-    def extend(self, **deps: Any) -> CLIDependencies:
-        self.lookup = {**self.lookup, **deps}
-        return self
-
-    @property
-    def config(self) -> CoreConfig:
-        return self.lookup["config"]  # type: ignore
-
-    @property
-    def message_bus(self) -> MessageBus:
-        return self.lookup["message_bus"]  # type:ignore
-
-    @property
-    def event_sender(self) -> AnalyticsEventSender:
-        return self.lookup["event_sender"]  # type:ignore
-
-    @property
-    def db_access(self) -> DbAccess:
-        return self.lookup["db_access"]  # type:ignore
-
-    @property
-    def model_handler(self) -> ModelHandler:
-        return self.lookup["model_handler"]  # type:ignore
-
-    @property
-    def task_handler(self) -> TaskHandler:
-        return self.lookup["task_handler"]  # type:ignore
-
-    @property
-    def worker_task_queue(self) -> WorkerTaskQueue:
-        return self.lookup["worker_task_queue"]  # type:ignore
-
-    @property
-    def template_expander(self) -> TemplateExpander:
-        return self.lookup["template_expander"]  # type:ignore
-
-    @property
-    def forked_tasks(self) -> Queue[Tuple[Task[JsonElement], str]]:
-        return self.lookup["forked_tasks"]  # type:ignore
-
-    @property
-    def cli(self) -> CLIEngine:
-        return self.lookup["cli"]  # type:ignore
-
-    @property
-    def config_handler(self) -> ConfigHandler:
-        return self.lookup["config_handler"]  # type:ignore
-
-    @property
-    def cert_handler(self) -> CertificateHandler:
-        return self.lookup["cert_handler"]  # type:ignore
-
-    @property
-    def inspector(self) -> Inspector:
-        return self.lookup["inspector"]  # type:ignore
-
-    @property
-    def infra_apps_runtime(self) -> Runtime:
-        return self.lookup["infra_apps_runtime"]  # type:ignore
-
-    @property
-    def infra_apps_package_manager(self) -> PackageManager:
-        return self.lookup["infra_apps_package_manager"]  # type:ignore
-
-    @property
-    def http_session(self) -> ClientSession:
-        session: Optional[ClientSession] = self.lookup.get("http_session")
-        if not session:
-            connector = TCPConnector(limit=0, ssl=False, ttl_dns_cache=300)
-            session = ClientSession(connector=connector)
-            self.lookup["http_session"] = session
-        return session
-
-    async def stop(self) -> None:
-        if "http_session" in self.lookup:
-            await self.http_session.close()
-
-
 @define
 class CLICommandRequirement:
     name: str
 
 
 @define
 class CLIFileRequirement(CLICommandRequirement):
@@ -381,17 +287,15 @@
     """
     The CLIPart is the base for all participants of the cli execution.
     Source: generates a stream of objects
     Flow: transforms the elements in a stream of objects
     Sink: takes a stream of objects and creates a result
     """
 
-    def __init__(
-        self, dependencies: CLIDependencies, category: str = "misc", allowed_in_source_position: bool = False
-    ) -> None:
+    def __init__(self, dependencies: Any, category: str = "misc", allowed_in_source_position: bool = False) -> None:
         self.dependencies = dependencies
         self.category = category
         self.allowed_in_source_position = allowed_in_source_position
 
     @property
     @abstractmethod
     def name(self) -> str:
@@ -440,14 +344,15 @@
     info: str
     template: str
     parameters: List[AliasTemplateParameter] = field(factory=list)
     description: Optional[str] = None
     # only use args_description if the template does not use explicit parameters
     args_description: Dict[str, str] = field(factory=dict)
     allowed_in_source_position: bool = False
+    infra_app_parameters: Optional[Dict[str, Any]] = None  # todo: remove this abomination
 
     def render(self, props: Json) -> str:
         return render_template(self.template, props)
 
     def args_info(self) -> ArgsInfo:
         args_desc = [ArgInfo(name, expects_value=True, help_text=desc) for name, desc in self.args_description.items()]
         param = [
@@ -470,14 +375,36 @@
         indent = "            "
         arg_info = f"\n{indent}".join(param_info(arg) for arg in sorted(self.parameters, key=attrgetter("name")))
         minimal = " ".join(f'{p.arg_name} "{p.example_value()}"' for p in self.parameters if p.default is None)
         desc = ""
         if self.description:
             for line in self.description.splitlines():
                 desc += f"\n{indent}{line}"
+
+        if self.infra_app_parameters:
+
+            def param_info_infra_apps(name: str, arg_info: Dict[str, Any]) -> str:
+                default = f" [default: {arg_info.get('default')}]" if arg_info.get("default") else ""
+                return f"- `{name}`{default}: {arg_info.get('help')}"
+
+            arg_info = f"\n{indent}".join(
+                param_info_infra_apps(name, arg) for name, arg in self.infra_app_parameters.items()
+            )
+            result = dedent(
+                f"""
+            {self.name}: {self.info}
+            ```shell
+            {self.name} {args}
+            ```
+            {desc}
+            ## Parameters
+            {arg_info}"""
+            )
+            return result
+
         return dedent(
             f"""
             {self.name}: {self.info}
             ```shell
             {self.name} {args}
             ```
             {desc}
@@ -487,15 +414,15 @@
             ## Template
             ```shell
             > {self.template}
             ```
 
             ## Example
             ```shell
-            # Executing this alias template
+            # Executing this command
             > {self.name} {minimal}
             # Will expand to this command
             > {self.render({p.name: p.example_value() for p in self.parameters})}
             ```
             """
         )
 
@@ -509,14 +436,16 @@
         args_info = args_info or ("<args>" if "{args}" in self.template else "")
         return (
             f"{self.name}: {self.info}\n```shell\n{self.name} {args}\n```\n\n"
             f"## Parameters\n{args_info}\n\n{self.description}\n\n"
         )
 
     def help(self) -> str:
+        if self.infra_app_parameters:  # todo: remove this abomination
+            return self.help_with_params()
         return self.help_with_params() if self.parameters else self.help_no_params_args()
 
     def rendered_help(self, ctx: CLIContext) -> str:
         return ctx.render_console(self.help())
 
     @staticmethod
     def from_config(cfg: AliasTemplateConfig) -> AliasTemplate:
@@ -668,18 +597,23 @@
         pass
 
     @abstractmethod
     async def execute_cli_command(self, cli_input: str, sink: Sink[T], ctx: CLIContext = EmptyContext) -> List[T]:
         pass
 
     @abstractmethod
-    def register_worker_custom_command(self, command: WorkerCustomCommand) -> None:
+    def register_alias_template(self, template: AliasTemplate) -> None:
+        """
+        Called when something introduces a custom command.
+        """
+
+    @abstractmethod
+    def unregister_alias_template(self, name: str) -> None:
         """
-        Called when a worker connects that introduces a custom command.
-        The registered templated will always override any existing template.
+        Called when something removes a custom command.
         """
 
     @property
     @abstractmethod
     def direct_commands(self) -> Dict[str, CLICommand]:
         pass
 
@@ -696,15 +630,15 @@
     @property
     @abstractmethod
     def env(self) -> Dict[str, Any]:
         pass
 
     @property
     @abstractmethod
-    def dependencies(self) -> CLIDependencies:
+    def dependencies(self) -> Any:  # CliDependencies, but we can't import it here
         pass
 
     @property
     @abstractmethod
     def alias_templates(self) -> Dict[str, AliasTemplate]:
         pass
```

### Comparing `resotocore-3.4.2/resotocore/cli/tip_of_the_day.py` & `resotocore-3.5.0/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/config/__init__.py` & `resotocore-3.5.0/resotocore/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,18 @@
         pass
 
     @abstractmethod
     async def patch_config(self, cfg: ConfigEntity, *, validate: bool = True, dry_run: bool = False) -> ConfigEntity:
         pass
 
     @abstractmethod
+    async def copy_config(self, from_cfg_id: ConfigId, to_cfg_id: ConfigId) -> Optional[ConfigEntity]:
+        pass
+
+    @abstractmethod
     async def delete_config(self, cfg_id: ConfigId) -> None:
         pass
 
     @abstractmethod
     async def get_configs_model(self) -> Model:
         pass
```

### Comparing `resotocore-3.4.2/resotocore/config/config_handler_service.py` & `resotocore-3.5.0/resotocore/config/config_handler_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,14 +147,27 @@
 
     async def delete_config(self, cfg_id: ConfigId) -> None:
         await self.cfg_db.delete(cfg_id)
         await self.validation_db.delete(cfg_id)
         await self.message_bus.emit_event(CoreMessage.ConfigDeleted, dict(id=cfg_id))
         await self.event_sender.core_event(CoreEvent.SystemConfigurationDeleted)
 
+    async def copy_config(self, from_cfg_id: ConfigId, to_cfg_id: ConfigId) -> Optional[ConfigEntity]:
+        old = await self.cfg_db.get(from_cfg_id)
+        if old is None:
+            return None
+        if await self.cfg_db.get(to_cfg_id) is not None:
+            raise ValueError(f"Config with id {to_cfg_id} already exists")
+        result = await self.cfg_db.update(ConfigEntity(to_cfg_id, old.config, old.revision))
+        await self.message_bus.emit_event(
+            CoreMessage.ConfigUpdated, dict(old=old.id, new=result.id, revision=result.revision)
+        )
+        await self.event_sender.core_event(CoreEvent.SystemConfigurationChanged, result.analytics())
+        return result
+
     def list_config_validation_ids(self) -> AsyncIterator[str]:
         return self.validation_db.keys()
 
     async def get_config_validation(self, cfg_id: str) -> Optional[ConfigValidation]:
         return await self.validation_db.get(cfg_id)
 
     async def put_config_validation(self, validation: ConfigValidation) -> ConfigValidation:
```

### Comparing `resotocore-3.4.2/resotocore/config/config_override_service.py` & `resotocore-3.5.0/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/config/core_config_handler.py` & `resotocore-3.5.0/resotocore/config/core_config_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 import asyncio
 import logging
 from asyncio import Task
 from contextlib import suppress
 from functools import partial
-from typing import Optional, List, Callable
+from typing import Optional, List, Callable, Awaitable
+from apscheduler.triggers.cron import CronTrigger
 
 import yaml
 
 from resotocore.analytics import AnalyticsEventSender, CoreEvent
 from resotocore.config import ConfigHandler, ConfigEntity, ConfigValidation
 from resotocore.core_config import (
     CoreConfig,
     ResotoCoreConfigId,
     EditableConfig,
     ResotoCoreRoot,
     ResotoCoreCommandsConfigId,
     ResotoCoreCommandsRoot,
+    ResotoCoreSnapshotsConfigId,
+    ResotoCoreSnapshotsRoot,
+    SnapshotsScheduleConfig,
     CustomCommandsConfig,
     migrate_core_config,
     config_model as core_config_model,
     migrate_command_config,
 )
 from resotocore.dependencies import empty_config
-from resotocore.ids import SubscriberId, WorkerId
+from resotocore.ids import SubscriberId, WorkerId, ConfigId
 from resotocore.message_bus import MessageBus, CoreMessage
 from resotocore.model.model import Kind
 from resotocore.model.typed_model import from_js
 from resotocore.report import ResotoReportBenchmark, ResotoReportCheck, Inspector, BenchmarkConfigRoot, CheckConfigRoot
 from resotocore.report.report_config import config_model as report_config_model
 from resotocore.types import Json
+from resotocore.user import config_model as user_config_model, UsersConfigId, ResotoUsersConfig
 from resotocore.util import deep_merge, restart_service, value_in_path, value_in_path_get
 from resotocore.worker_task_queue import WorkerTaskQueue, WorkerTaskDescription, WorkerTaskName, WorkerTask
 
 log = logging.getLogger(__name__)
 
 
 class CoreConfigHandler:
@@ -51,14 +56,15 @@
         self.config_updated_listener: Optional[Task[None]] = None
         self.config_validator: Optional[Task[None]] = None
         self.config = config
         self.config_handler = config_handler
         self.event_sender = event_sender
         self.inspector = inspector
         self.exit_fn = exit_fn
+        self.config_updated_callbacks: List[Callable[[ConfigId], Awaitable[None]]] = []
 
     async def validate_config_entry(self, task_data: Json) -> Optional[Json]:
         def validate_core_config() -> Optional[Json]:
             config = value_in_path(task_data, ["config", ResotoCoreRoot])
             if isinstance(config, dict):
                 # try to read editable config, throws if there are errors
                 read = from_js(config, EditableConfig)
@@ -71,33 +77,61 @@
             if isinstance(config, dict):
                 # try to read editable config, throws if there are errors
                 read = from_js(config, CustomCommandsConfig)
                 return read.validate()
             else:
                 return {"error": "Expected a json object"}
 
+        def validate_snapshot_schedule() -> Optional[Json]:
+            config = value_in_path(task_data, ["config", ResotoCoreSnapshotsRoot])
+            if isinstance(config, dict):
+                config = {"snapshots": config}  # wrap in snapshots objects to match the dataclass
+                read = from_js(config, SnapshotsScheduleConfig)
+                # validate cron expressions
+                try:
+                    for schedule in read.snapshots.values():
+                        CronTrigger.from_crontab(schedule.schedule)
+                    return None
+                except Exception as ex:
+                    return {"error": f"Invalid cron expression: {ex}"}
+            else:
+                return {"error": "Expected a json object"}
+
         holder = value_in_path(task_data, ["config"])
         if not isinstance(holder, dict):
             return {"error": "Expected a json object in config"}
         elif ResotoCoreRoot in holder:
             return validate_core_config()
         elif ResotoCoreCommandsRoot in holder:
             return validate_commands_config()
         elif CheckConfigRoot in holder:
             return await self.inspector.validate_check_collection_config(task_data["config"])
         elif BenchmarkConfigRoot in holder:
             return await self.inspector.validate_benchmark_config(task_data["config"])
+        elif ResotoCoreSnapshotsRoot in holder:
+            return validate_snapshot_schedule()
         else:
             return {"error": "No known configuration found"}
 
+    def add_callback(self, callback: Callable[[ConfigId], Awaitable[None]]) -> None:
+        self.config_updated_callbacks.append(callback)
+
     async def __validate_config(self) -> None:
         worker_id = WorkerId("resotocore.config.validate")
         description = WorkerTaskDescription(
             WorkerTaskName.validate_config,
-            {"config_id": [ResotoCoreConfigId, ResotoCoreCommandsConfigId, ResotoReportBenchmark, ResotoReportCheck]},
+            {
+                "config_id": [
+                    ResotoCoreConfigId,
+                    ResotoCoreCommandsConfigId,
+                    ResotoReportBenchmark,
+                    ResotoReportCheck,
+                    ResotoCoreSnapshotsConfigId,
+                ]
+            },
         )
         async with self.worker_task_queue.attach(worker_id, [description]) as tasks:
             while True:
                 task: WorkerTask = await tasks.get()
                 try:
                     errors = await self.validate_config_entry(task.data)
                     if errors:
@@ -118,14 +152,21 @@
 
     async def __handle_events(self) -> None:
         subscriber_id = SubscriberId("resotocore.config.update")
         async with self.message_bus.subscribe(subscriber_id, [CoreMessage.ConfigUpdated]) as events:
             while True:
                 event = await events.get()
                 event_id = event.data.get("id")
+                if event_id:
+                    for callback in self.config_updated_callbacks:
+                        try:
+                            await callback(event_id)
+                        except Exception as ex:
+                            log.warning("Error in config update callback", exc_info=ex)
+
                 if event_id in (ResotoCoreConfigId, ResotoCoreCommandsConfigId):
                     log.info(f"Core config was updated: {event_id} Restart to take effect.")
                     await self.__detect_usage_metrics_turned_off()
                     # stop the process and rely on os to restart the service
                     self.exit_fn()
 
     async def __update_config(self) -> None:
@@ -151,33 +192,61 @@
             else:
                 to_update = migrate_command_config(existing_commands.config)
             if to_update is not None:
                 await self.config_handler.put_config(
                     ConfigEntity(ResotoCoreCommandsConfigId, to_update), validate=False
                 )
                 log.info("Default resoto commands config updated.")
-
         except Exception as ex:
             log.error(f"Could not update resoto command configuration: {ex}", exc_info=ex)
 
+        # make sure there is a default user configuration
+        try:
+            existing_users = await self.config_handler.get_config(UsersConfigId)
+            user_update: Optional[Json] = None
+            if existing_users is None:
+                user_update = ResotoUsersConfig().json()
+            if user_update is not None:
+                await self.config_handler.put_config(ConfigEntity(UsersConfigId, user_update), validate=False)
+                log.info("Default resoto users config updated.")
+        except Exception as ex:
+            log.error(f"Could not update resoto users configuration: {ex}", exc_info=ex)
+
+        # make sure there is a default snapshots configuration
+        try:
+            existing_snapshots = await self.config_handler.get_config(ResotoCoreSnapshotsConfigId)
+            snapshot_update: Optional[Json] = None
+            if existing_snapshots is None:
+                snapshot_update = SnapshotsScheduleConfig().json()
+            if snapshot_update is not None:
+                await self.config_handler.put_config(
+                    ConfigEntity(ResotoCoreSnapshotsConfigId, snapshot_update), validate=False
+                )
+                log.info("Default resoto snapshots config updated.")
+        except Exception as ex:
+            log.error(f"Could not update resoto snapshots configuration: {ex}", exc_info=ex)
+
     async def __update_model(self) -> None:
         try:
-            models = core_config_model() + report_config_model()
+            models = core_config_model() + report_config_model() + user_config_model()
             kinds = from_js(models, List[Kind])
             await self.config_handler.update_configs_model(kinds)
             await self.config_handler.put_config_validation(
                 ConfigValidation(ResotoCoreConfigId, external_validation=True)
             )
             await self.config_handler.put_config_validation(
                 ConfigValidation(ResotoCoreCommandsConfigId, external_validation=True)
             )
             await self.config_handler.put_config_validation(
                 ConfigValidation(ResotoCoreCommandsConfigId, external_validation=True)
             )
             await self.config_handler.put_config_validation(
+                ConfigValidation(ResotoCoreSnapshotsConfigId, external_validation=True)
+            )
+            await self.config_handler.put_config_validation(
                 ConfigValidation(ResotoReportBenchmark, external_validation=True)
             )
             await self.config_handler.put_config_validation(
                 ConfigValidation(ResotoReportCheck, external_validation=True)
             )
 
             log.debug("Resoto core config model updated.")
```

### Comparing `resotocore-3.4.2/resotocore/console_renderer.py` & `resotocore-3.5.0/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/constants.py` & `resotocore-3.5.0/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/core_config.py` & `resotocore-3.5.0/resotocore/core_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 from resotolib.utils import replace_env_vars, is_env_var_string, merge_json_elements
 
 log = logging.getLogger(__name__)
 
 # ids used in the config store
 ResotoCoreConfigId = ConfigId("resoto.core")
 ResotoCoreCommandsConfigId = ConfigId("resoto.core.commands")
+ResotoCoreSnapshotsConfigId = ConfigId("resoto.core.snapshots")
 
 # root note of the configuration value
 ResotoCoreRoot = "resotocore"
 ResotoCoreCommandsRoot = "custom_commands"
+ResotoCoreSnapshotsRoot = "snapshots"
 
 ResotoCoreRootRE = re.compile(r"^resotocore[.]")
 
 # created by the docker build process
 GitHashFile = "/usr/local/etc/git-commit.HEAD"
 
 
@@ -140,14 +142,20 @@
     )
     max_request_size: Optional[int] = field(
         default=1024**2 * 5, metadata={"description": "The maximum size of a request in bytes (default: 5MB)"}
     )
     host_certificate: CertificateConfig = field(
         factory=CertificateConfig, metadata={"description": "The certificate configuration for this server."}
     )
+    access_token_expiration_seconds: int = field(
+        default=3600, metadata={"description": "The expiration time of the access token in seconds (default: 1h)"}
+    )
+
+    def access_token_expiration(self) -> timedelta:
+        return timedelta(seconds=self.access_token_expiration_seconds)
 
 
 # Define rules to validate this config
 schema_registry.add(
     schema_name(ApiConfig),
     dict(
         tsdb_proxy_url={"type": "string", "nullable": True, "is_url": True},
@@ -475,14 +483,57 @@
         return {ResotoCoreCommandsRoot: to_js(self, strip_attr="kind")}
 
 
 # Define rules to validate this config
 schema_registry.add(schema_name(CustomCommandsConfig), {})
 
 
+SnapshotLabel = str
+
+
+@define
+class SnapshotSchedule(ConfigObject):
+    kind: ClassVar[str] = f"{ResotoCoreSnapshotsRoot}_schedule"
+    schedule: str = field(
+        metadata={
+            "description": "The schedule in cron format.\n"
+            "Example: `0 0 * * *` will create a snapshot every day at midnight.\n"
+            "See https://en.wikipedia.org/wiki/Cron for more information.",
+        }
+    )
+    retain: int = field(
+        metadata={
+            "description": "How many snapshots should be retained.\n"
+            "If the number of snapshots exceeds this value, the oldest snapshots will be deleted.\n"
+        }
+    )
+
+
+@define()
+class SnapshotsScheduleConfig(ConfigObject):
+    kind: ClassVar[str] = ResotoCoreSnapshotsRoot
+    snapshots: Dict[SnapshotLabel, SnapshotSchedule] = field(
+        default={
+            "hourly": SnapshotSchedule(schedule="0 * * * *", retain=24),
+            "daily": SnapshotSchedule(schedule="0 0 * * *", retain=7),
+            "weekly": SnapshotSchedule(schedule="0 0 * * 0", retain=4),
+            "monthly": SnapshotSchedule(schedule="0 0 1 * *", retain=12),
+            "yearly": SnapshotSchedule(schedule="0 0 1 1 *", retain=10),
+        },
+        metadata={
+            "description": "Here you can define all snapshot schedules.\n"
+            "The key is the label of the snapshot schedule.\n"
+            "The value is the schedule configuration.",
+        },
+    )
+
+    def json(self) -> Json:
+        return to_js(self, strip_attr="kind")
+
+
 @define()
 class GraphUpdateConfig(ConfigObject):
     kind: ClassVar[str] = f"{ResotoCoreRoot}_graph_update_config"
     merge_max_wait_time_seconds: int = field(
         default=3600, metadata={"description": "Max waiting time to complete a merge graph action."}
     )
     abort_after_seconds: int = field(
@@ -566,14 +617,15 @@
     api: ApiConfig
     cli: CLIConfig
     graph_update: GraphUpdateConfig
     runtime: RuntimeConfig
     db: DatabaseConfig
     workflows: Dict[str, WorkflowConfig]
     custom_commands: CustomCommandsConfig
+    snapshots: SnapshotsScheduleConfig
     args: Namespace
     run: RunConfig
 
     @property
     def editable(self) -> "EditableConfig":
         return EditableConfig(self.api, self.cli, self.graph_update, self.runtime, self.workflows)
 
@@ -633,14 +685,15 @@
 
 
 def parse_config(
     args: Namespace,
     core_config: Json,
     get_core_overrides: Callable[[], Optional[Json]],
     command_templates: Optional[Json] = None,
+    snapshot_schedule: Optional[Json] = None,
 ) -> CoreConfig:
     db = DatabaseConfig(
         server=args.graphdb_server,
         database=args.graphdb_database,
         username=args.graphdb_username,
         password=args.graphdb_password,
         root_password=args.graphdb_root_password,
@@ -697,19 +750,27 @@
         try:
             migrated_commands = migrate_command_config(command_templates)
             cmd_cfg_to_parse = migrated_commands or command_templates
             commands_config = from_js(cmd_cfg_to_parse.get(ResotoCoreCommandsRoot), CustomCommandsConfig)
         except Exception as e:
             log.error(f"Can not parse command templates. Fall back to defaults. Reason: {e}", exc_info=e)
 
+    snapshots_config = SnapshotsScheduleConfig()
+    if snapshot_schedule:
+        try:
+            snapshots_config = from_js(snapshot_schedule.get(ResotoCoreSnapshotsRoot), SnapshotsScheduleConfig)
+        except Exception as e:
+            log.error(f"Can not parse snapshot schedule. Fall back to defaults. Reason: {e}", exc_info=e)
+
     return CoreConfig(
         api=ed.api,
         args=args,
         cli=ed.cli,
         custom_commands=commands_config,
+        snapshots=snapshots_config,
         db=db,
         graph_update=ed.graph_update,
         runtime=ed.runtime,
         workflows=ed.workflows,
         run=RunConfig(),  # overridden for each run
     )
 
@@ -752,9 +813,13 @@
     collection_name: str = "configs",
 ) -> CoreConfig:
     if configs := db.collection(collection_name) if db.has_collection(collection_name) else None:
         if config_entity := cast(Optional[Json], configs.get(ResotoCoreConfigId)):
             if config := config_entity.get("config"):
                 command_config_entity = cast(Optional[Json], configs.get(ResotoCoreCommandsConfigId))
                 command_config = command_config_entity.get("config") if command_config_entity else None
-                return parse_config(args, config, get_core_overrides, command_config)
+
+                snapshots_config_entity = cast(Optional[Json], configs.get(ResotoCoreSnapshotsConfigId))
+                snapshots_config = snapshots_config_entity.get("config") if snapshots_config_entity else None
+
+                return parse_config(args, config, get_core_overrides, command_config, snapshots_config)
     return parse_config(args, {}, get_core_overrides)
```

### Comparing `resotocore-3.4.2/resotocore/db/arango_query.py` & `resotocore-3.5.0/resotocore/db/arango_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 def to_query(
     db: Any, query_model: QueryModel, with_edges: bool = False, from_collection: Optional[str] = None
 ) -> Tuple[str, Json]:
     count: Dict[str, int] = defaultdict(lambda: 0)
     query = query_model.query
     bind_vars: Json = {}
-    start = from_collection or db.vertex_name
+    start = from_collection or f"`{db.vertex_name}`"
     cursor, query_str = query_string(db, query, query_model, start, with_edges, bind_vars, count)
     return f"""{query_str} FOR result in {cursor} RETURN UNSET(result, {unset_props})""", bind_vars
 
 
 def query_string(
     db: Any,
     query: Query,
```

### Comparing `resotocore-3.4.2/resotocore/db/arangodb_extensions.py` & `resotocore-3.5.0/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/arangodb_functions.py` & `resotocore-3.5.0/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/async_arangodb.py` & `resotocore-3.5.0/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/configdb.py` & `resotocore-3.5.0/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/db_access.py` & `resotocore-3.5.0/resotocore/db/db_access.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,34 +9,37 @@
 from arango.client import ArangoClient
 from arango.database import StandardDatabase
 from dateutil.parser import parse
 from requests.exceptions import RequestException
 
 
 from resotocore.analytics import AnalyticsEventSender
+from resotocore.async_extensions import run_async
 from resotocore.core_config import CoreConfig
 from resotocore.db import SystemData
 from resotocore.db.arangodb_extensions import ArangoHTTPClient
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.db.configdb import config_entity_db, config_validation_entity_db
 from resotocore.db.entitydb import EventEntityDb
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB
 from resotocore.db.jobdb import job_db
 from resotocore.db.modeldb import ModelDb, model_db
 from resotocore.db.deferred_edge_db import pending_deferred_edge_db
 from resotocore.db.runningtaskdb import running_task_db
 from resotocore.db.subscriberdb import subscriber_db
+from resotocore.db.system_data_db import SystemDataDb
 from resotocore.db.templatedb import template_entity_db
 from resotocore.db.packagedb import app_package_entity_db
 from resotocore.error import NoSuchGraph, RequiredDependencyMissingError
 from resotocore.model.adjust_node import AdjustNode
 from resotocore.model.typed_model import from_js, to_js
+from resotocore.model.graph_access import EdgeTypes
 from resotocore.types import Json
 from resotocore.ids import GraphName
-from resotocore.util import Periodic, utc, shutdown_process, uuid_str
+from resotocore.util import Periodic, utc, shutdown_process, uuid_str, check_graph_name
 
 log = logging.getLogger(__name__)
 
 
 class DbAccess(ABC):
     def __init__(
         self,
@@ -58,14 +61,15 @@
         self.event_sender = event_sender
         self.database = arango_database
         self.db = AsyncArangoDB(arango_database)
         self.adjust_node = adjust_node
         self.model_db = EventEntityDb(model_db(self.db, model_name), event_sender, model_name)
         self.graph_model_dbs: Dict[GraphName, ModelDb] = {}
         self.subscribers_db = EventEntityDb(subscriber_db(self.db, subscriber_name), event_sender, subscriber_name)
+        self.system_data_db = SystemDataDb(self.db)
         self.running_task_db = running_task_db(self.db, running_task_name)
         self.pending_deferred_edge_db = pending_deferred_edge_db(self.db, deferred_edge_name)
         self.job_db = job_db(self.db, job_name)
         self.config_entity_db = config_entity_db(self.db, config_entity)
         self.config_validation_entity_db = config_validation_entity_db(self.db, config_validation_entity)
         self.configs_model_db = model_db(self.db, configs_model)
         self.template_entity_db = template_entity_db(self.db, template_entity)
@@ -82,38 +86,60 @@
         await self.config_entity_db.create_update_schema()
         await self.config_validation_entity_db.create_update_schema()
         await self.configs_model_db.create_update_schema()
         await self.template_entity_db.create_update_schema()
         await self.pending_deferred_edge_db.create_update_schema()
         await self.package_entity_db.create_update_schema()
         for graph in cast(List[Json], self.database.graphs()):
-            log.info(f'Found graph: {graph["name"]}')
-            db = self.get_graph_db(graph["name"])
+            graph_name = GraphName(graph["name"])
+            log.info(f"Found graph: {graph_name}")
+            db = self.get_graph_db(graph_name)
             await db.create_update_schema()
+            await self.get_graph_model_db(graph_name)
         await self.cleaner.start()
 
     async def stop(self) -> None:
         await self.cleaner.stop()
 
-    async def create_graph(self, name: GraphName) -> GraphDB:
+    def graph_model_name(self, graph_name: GraphName) -> str:
+        return f"{graph_name}_model"
+
+    async def create_graph(self, name: GraphName, validate_name: bool = True) -> GraphDB:
+        if validate_name:
+            check_graph_name(name)
+
         db = self.get_graph_db(name, no_check=True)
         await db.create_update_schema()
         return db
 
     async def delete_graph(self, name: GraphName) -> None:
-        db = self.database
-        if db.has_graph(name):
-            db.delete_graph(name, drop_collections=True, ignore_missing=True)
-            db.delete_collection(f"{name}_in_progress", ignore_missing=True)
-            db.delete_view(f"search_{name}", ignore_missing=True)
-            # remove all temp collection names
-            for coll in cast(List[Json], db.collections()):
-                if coll["name"].startswith(f"{name}_temp_"):
-                    db.delete_collection(coll["name"])
-            self.graph_dbs.pop(name, None)
+        def delete(name: GraphName) -> None:
+            db = self.database
+            if db.has_graph(name):
+                # delete arrangodb graph
+                db.delete_graph(name, drop_collections=True, ignore_missing=True)
+                # delete vertex collections just in case
+                db.delete_collection(name, ignore_missing=True)
+                # delete edge collections
+                for edge_type in EdgeTypes.all:
+                    db.delete_collection(f"{name}_{edge_type}", ignore_missing=True)
+                # delete the rest
+                db.delete_collection(f"{name}_in_progress", ignore_missing=True)
+                db.delete_view(f"search_{name}", ignore_missing=True)
+                # remove all temp collection names
+                for coll in cast(List[Json], db.collections()):
+                    if coll["name"].startswith(f"{name}_temp_"):
+                        db.delete_collection(coll["name"], ignore_missing=True)
+                self.graph_dbs.pop(name, None)
+
+        return await run_async(delete, name)
+
+    async def delete_graph_model(self, graph_name: GraphName) -> None:
+        await self.db.delete_collection(self.graph_model_name(graph_name), ignore_missing=True)
+        self.graph_model_dbs.pop(graph_name, None)
 
     async def list_graphs(self) -> List[GraphName]:
         return [a["name"] for a in cast(List[Json], self.database.graphs()) if not a["name"].endswith("_hs")]
 
     def get_graph_db(self, name: GraphName, no_check: bool = False) -> GraphDB:
         if name in self.graph_dbs:
             return self.graph_dbs[name]
@@ -128,15 +154,15 @@
     def get_model_db(self) -> ModelDb:
         return self.model_db
 
     async def get_graph_model_db(self, graph_name: GraphName) -> ModelDb:
         if db := self.graph_model_dbs.get(graph_name):
             return db
         else:
-            model_name = f"model_{graph_name}"
+            model_name = self.graph_model_name(graph_name)
             db = EventEntityDb(model_db(self.db, model_name), self.event_sender, model_name)
             await db.create_update_schema()
             self.graph_model_dbs[graph_name] = db
             return db
 
     async def check_outdated_updates(self) -> None:
         now = datetime.now(timezone.utc)
```

### Comparing `resotocore-3.4.2/resotocore/db/deferred_edge_db.py` & `resotocore-3.5.0/resotocore/db/deferred_edge_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/entitydb.py` & `resotocore-3.5.0/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/graphdb.py` & `resotocore-3.5.0/resotocore/db/graphdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1064,37 +1064,50 @@
             new_delete_edge = new_graph_db.edge_collection(EdgeTypes.delete)
 
             tx = f"""
                 function () {{
                     const db = require('@arangodb').db;
 
                     db._query(
-                        "FOR vertex IN {old_vertex} "
+                        query="FOR vertex IN @@old_vertex "
                         + "LET clean_vertex = UNSET(vertex, '_id', '_rev') "
-                        + "INSERT clean_vertex INTO {new_vertex}"
+                        + "INSERT clean_vertex INTO @@new_vertex",
+                        bindVars= {{
+                            "@old_vertex": "{old_vertex}",
+                            "@new_vertex": "{new_vertex}"
+                        }}
                     );
 
                     db._query(
-                        "FOR edge IN {old_default_edge} "
+                        query="FOR edge IN @@old_default_edge "
                         + "LET clean_edge = UNSET(edge, '_id', '_rev') "
-                        + "LET from = CONCAT('{new_vertex}/', PARSE_IDENTIFIER(edge._from)['key']) "
-                        + "LET to = CONCAT('{new_vertex}/', PARSE_IDENTIFIER(edge._to)['key']) "
-                        + "INSERT MERGE(clean_edge, {{_from: from, _to: to}}) INTO {new_default_edge}"
+                        + "LET from = CONCAT(@new_vertex, '/', PARSE_IDENTIFIER(edge._from)['key']) "
+                        + "LET to = CONCAT(@new_vertex, '/', PARSE_IDENTIFIER(edge._to)['key']) "
+                        + "INSERT MERGE(clean_edge, {{_from: from, _to: to}}) INTO @@new_default_edge",
+                        bindVars= {{
+                            "@old_default_edge": "{old_default_edge}",
+                            "@new_default_edge": "{new_default_edge}",
+                            "new_vertex": "{new_vertex}"
+                        }}
                     );
 
                     db._query(
-                        "FOR edge IN {old_delete_edge} "
+                        query="FOR edge IN @@old_delete_edge "
                         + "LET clean_edge = UNSET(edge, '_id', '_rev') "
-                        + "LET from = CONCAT('{new_vertex}/', PARSE_IDENTIFIER(edge._from)['key']) "
-                        + "LET to = CONCAT('{new_vertex}/', PARSE_IDENTIFIER(edge._to)['key']) "
-                        + "INSERT MERGE(clean_edge, {{_from: from, _to: to}}) INTO {new_delete_edge}"
+                        + "LET from = CONCAT(@new_vertex, '/', PARSE_IDENTIFIER(edge._from)['key']) "
+                        + "LET to = CONCAT(@new_vertex, '/', PARSE_IDENTIFIER(edge._to)['key']) "
+                        + "INSERT MERGE(clean_edge, {{_from: from, _to: to}}) INTO @@new_delete_edge",
+                        bindVars= {{
+                            "@old_delete_edge": "{old_delete_edge}",
+                            "@new_delete_edge": "{new_delete_edge}",
+                            "new_vertex": "{new_vertex}"
+                        }}
                     );
                 }}
             """
-
             await self.db.execute_transaction(
                 tx,
                 read=[old_vertex, old_default_edge, old_delete_edge],
                 write=[new_vertex, new_default_edge, new_delete_edge],
             )
 
         await create_new_collections(new_graph_db)
@@ -1106,98 +1119,98 @@
     def db_edge_key(from_node: str, to_node: str) -> str:
         return str(uuid.uuid5(uuid.NAMESPACE_DNS, f"{from_node}:{to_node}"))
 
     # parameter: rid
     # return: the complete document
     def query_node_by_id(self) -> str:
         return f"""
-      FOR resource in {self.vertex_name}
+      FOR resource in `{self.vertex_name}`
       FILTER resource._key==@rid
       LIMIT 1
       RETURN resource
       """
 
     def query_update_nodes(self, merge_node_kind: str) -> str:
         return f"""
-        FOR a IN {self.vertex_name}
+        FOR a IN `{self.vertex_name}`
         FILTER a.refs.{merge_node_kind}_id==@update_id
         RETURN {{_key: a._key, hash:a.hash, created:a.created}}
         """
 
     def query_update_edges(self, edge_type: EdgeType, merge_node_kind: str) -> str:
         collection = self.edge_collection(edge_type)
         return f"""
-        FOR a IN {collection}
+        FOR a IN `{collection}`
         FILTER a.refs.{merge_node_kind}_id==@update_id
         RETURN {{_key: a._key, _from: a._from, _to: a._to}}
         """
 
     def query_update_nodes_by_ids(self) -> str:
         return f"""
-        FOR a IN {self.vertex_name}
+        FOR a IN `{self.vertex_name}`
         FILTER a._key IN @ids
         RETURN {{_key: a._key, hash:a.hash, created:a.created}}
         """
 
     def query_update_edges_by_ids(self, edge_type: EdgeType) -> str:
         collection = self.edge_collection(edge_type)
         return f"""
-        FOR a IN {collection}
+        FOR a IN `{collection}`
         FILTER a._key in @ids
         RETURN {{_key: a._key, _from: a._from, _to: a._to}}
         """
 
     def query_update_parent_linked(self) -> str:
         return f"""
-        FOR a IN {self.edge_collection(EdgeTypes.default)}
+        FOR a IN `{self.edge_collection(EdgeTypes.default)}`
         FILTER a._from==@from and a._to==@to
         RETURN true
         """
 
     def query_update_desired_metadata_many(self, section: str) -> str:
         return f"""
-        FOR a IN {self.vertex_name}
+        FOR a IN `{self.vertex_name}`
         FILTER a._key in @node_ids
-        UPDATE a with {{ "{section}": @patch }} IN {self.vertex_name}
+        UPDATE a with {{ "{section}": @patch }} IN `{self.vertex_name}`
         RETURN NEW
         """
 
     def query_delete_desired_metadata_many(self, section: str) -> str:
         return f"""
-        FOR a IN {self.vertex_name}
+        FOR a IN `{self.vertex_name}`
         FILTER a._key in @node_ids
-        REPLACE a with UNSET(a, "{section}") IN {self.vertex_name}
+        REPLACE a with UNSET(a, "{section}") IN `{self.vertex_name}`
         RETURN NEW
         """
 
     def query_count_direct_children(self) -> str:
         return f"""
-        FOR pn in {self.vertex_name} FILTER pn._key==@rid LIMIT 1
+        FOR pn in `{self.vertex_name}` FILTER pn._key==@rid LIMIT 1
         FOR c IN 1..1 OUTBOUND pn {self.edge_collection(EdgeTypes.default)} COLLECT WITH COUNT INTO length
         RETURN length
         """
 
     def query_active_updates(self) -> str:
         return f"""
-        FOR c IN {self.in_progress}
+        FOR c IN `{self.in_progress}`
         RETURN {{id: c.change, created: c.created, affected_nodes: c.root_node_ids, is_batch: c.is_batch}}
         """
 
     def query_active_change(self) -> str:
         return f"""
-        FOR change IN {self.in_progress}
+        FOR change IN `{self.in_progress}`
         FILTER @root_node_ids any in change.parent_node_ids OR @root_node_ids any in change.root_node_ids
         RETURN change
         """
 
     def update_active_change(self) -> str:
         return f"""
-        FOR d in {self.in_progress}
+        FOR d in `{self.in_progress}`
         FILTER d.change == @change
-        UPDATE d WITH {{created: DATE_ISO8601(DATE_NOW())}} in {self.in_progress}
+        UPDATE d WITH {{created: DATE_ISO8601(DATE_NOW())}} in `{self.in_progress}`
         """
 
 
 class EventGraphDB(GraphDB):
     def __init__(self, real: ArangoGraphDB, event_sender: AnalyticsEventSender):
         self.real = real
         self.event_sender = event_sender
```

### Comparing `resotocore-3.4.2/resotocore/db/model.py` & `resotocore-3.5.0/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/packagedb.py` & `resotocore-3.5.0/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/db/runningtaskdb.py` & `resotocore-3.5.0/resotocore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/dependencies.py` & `resotocore-3.5.0/resotocore/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import multiprocessing as mp
 import os.path
 import sys
 from argparse import Namespace
 from collections import namedtuple
 from pathlib import Path
-from ssl import SSLContext
 from typing import Optional, List, Callable, Tuple
 
 import psutil
 from arango.database import StandardDatabase
 from parsy import Parser
 
 from resotocore import async_extensions, version
@@ -18,21 +17,14 @@
 from resotocore.core_config import CoreConfig, parse_config, git_hash_from_file, inside_docker
 from resotocore.db.db_access import DbAccess
 from resotocore.model.adjust_node import DirectAdjuster
 from resotocore.types import JsonElement
 from resotocore.util import utc
 from resotolib.args import ArgumentParser
 from resotolib.jwt import add_args as jwt_add_args
-from resotolib.log.logstream import (
-    EventStreamer,
-    EventStreamAsync,
-    LogStreamHandler,
-    EventStreamAsyncService,
-    NoEventStreamAsync,
-)
 from resotolib.logger import setup_logger
 from resotolib.parse_util import make_parser, variable_p, equals_p, comma_p, json_value_dp
 from resotolib.utils import iec_size_format, get_local_tzinfo
 
 log = logging.getLogger(__name__)
 
 SystemInfo = namedtuple(
@@ -209,17 +201,14 @@
         "--verbose", "-v", dest="verbose", default=False, action="store_true", help="Enable verbose logging."
     )
     parser.add_argument(  # No default here on purpose: it can be reconfigured!
         "--debug", default=None, action="store_true", help="Enable debug mode. If not defined use configuration."
     )
     parser.add_argument("--ui-path", help=argparse.SUPPRESS)  # no effect any longer, only here to not break anything
     parser.add_argument("--analytics-opt-out", default=None, action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument(
-        "--resotoeventlog-uri", dest="resotoeventlog_uri", default=None, help="URI to the resotoeventlog server."
-    )
 
     parsed: Namespace = parser.parse_args(args if args else [])
 
     if parsed.version:
         # print here on purpose, since logging is not set up yet.
         print(f"resotocore {version()}")
         sys.exit(0)
@@ -275,23 +264,14 @@
         # transitions (fsm) creates a lot of log noise. Only show warnings.
         logging.getLogger("transitions.core").setLevel(logging.WARNING)
         # apscheduler uses the term Job when it triggers, which confuses people.
         logging.getLogger("apscheduler.executors").setLevel(logging.WARNING)
         logging.getLogger("apscheduler.scheduler").setLevel(logging.WARNING)
 
 
-def event_stream(config: CoreConfig, ctx: SSLContext) -> EventStreamAsync:
-    if url := config.args.resotoeventlog_uri:
-        streamer = EventStreamer(f"{url}/ingest", ssl=ctx)
-        log_handler = LogStreamHandler("resotocore", streamer)
-        return EventStreamAsyncService(streamer, log_handler)
-    else:
-        return NoEventStreamAsync()
-
-
 def reset_process_start_method() -> None:
     preferred = "spawn"
     current = mp.get_start_method(True)
     if current != preferred:
         if preferred in mp.get_all_start_methods():
             log.debug(f"Set process start method to {preferred}")
             mp.set_start_method(preferred, True)
```

### Comparing `resotocore-3.4.2/resotocore/error.py` & `resotocore-3.5.0/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/infra_apps/local_runtime.py` & `resotocore-3.5.0/resotocore/infra_apps/local_runtime.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import List, AsyncIterator
+from typing import List, AsyncIterator, Type, Optional, Any
 from resotocore.infra_apps.runtime import Runtime
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.types import Json, JsonElement
 from resotocore.ids import GraphName
 from resotocore.db.model import QueryModel
 from resotocore.cli.model import CLI, CLIContext
+from resotocore.cli import NoExitArgumentParser
 from jinja2 import Environment
 import logging
 from aiostream.core import Stream
 from aiostream import stream
 from argparse import Namespace
 from resotolib.durations import parse_optional_duration
 from resotolib.asynchronous.utils import async_lines
+from pydoc import locate
 
 
 log = logging.getLogger(__name__)
 
 
 class LocalResotocoreAppRuntime(Runtime):
     """
@@ -31,37 +33,32 @@
 
     async def execute(
         self,
         graph: GraphName,
         manifest: AppManifest,
         config: Json,
         stdin: AsyncIterator[JsonElement],
-        kwargs: Namespace,
+        argv: List[str],
         ctx: CLIContext,
     ) -> AsyncIterator[JsonElement]:
         """
         Runtime implementation that runs the app locally.
         """
-        try:
-            async for line in self.generate_template(graph, manifest, config, stdin, kwargs):
-                async with (await self._interpret_line(line, ctx)).stream() as streamer:
-                    async for item in streamer:
-                        yield item
-
-        except Exception as e:
-            msg = f"Error running infrastructure app: {e}"
-            log.exception(msg)
+        async for line in self.generate_template(graph, manifest, config, stdin, argv):
+            async with (await self._interpret_line(line, ctx)).stream() as streamer:
+                async for item in streamer:
+                    yield item
 
     async def generate_template(
         self,
         graph: GraphName,
         manifest: AppManifest,
         config: Json,
         stdin: AsyncIterator[JsonElement],
-        kwargs: Namespace,
+        argv: List[str],
     ) -> AsyncIterator[str]:
         graphdb = self.dbaccess.get_graph_db(graph)
         env = Environment(extensions=["jinja2.ext.do", "jinja2.ext.loopcontrols"], enable_async=True)
         template = env.from_string(manifest.source)
 
         model = await self.model_handler.load_model(graph)
 
@@ -71,21 +68,48 @@
             async with await graphdb.search_graph_gen(QueryModel(query, model)) as ctx:
                 async for result in ctx:
                     yield result
 
         template.globals["parse_duration"] = parse_optional_duration
         template.globals["search"] = perform_search
 
-        async for line in async_lines(template.generate_async(config=config, args=kwargs, stdin=stdin)):
+        args = self._args_from_manifest(manifest, argv)
+
+        async for line in async_lines(template.generate_async(config=config, args=args, stdin=stdin)):
             line = line.strip()
             log.debug(f"Rendered infrastructure app line: {line}")
             if not line:
                 continue
             yield line
 
+    def _args_from_manifest(self, manifest: AppManifest, argv: Optional[List[str]] = None) -> Namespace:
+        args_schema = manifest.args_schema or {}
+
+        parser = NoExitArgumentParser(description=manifest.description)
+
+        def str_to_type(type_str: Optional[str]) -> Optional[Type[Any]]:
+            if type_str is None:
+                return None
+            supported_types = {"bool", "str", "int", "float", "complex"}
+            if type_str not in supported_types:
+                raise ValueError(f"Unsupported type: {type_str}")
+            return locate(type_str)  # type: ignore
+
+        for arg_name, arg_info in args_schema.items():
+            kwargs = {}
+            for flag in ["help", "action", "default", "type", "nargs", "required"]:
+                if flag in arg_info:
+                    if flag == "type":
+                        kwargs[flag] = str_to_type(arg_info[flag])
+                    else:
+                        kwargs[flag] = arg_info[flag]
+            parser.add_argument(f"--{arg_name}", **kwargs)  # type: ignore
+
+        return parser.parse_args(argv)
+
     async def _interpret_line(self, line: str, ctx: CLIContext) -> Stream:
         command_streams: List[Stream] = []
         total_nr_outputs: int = 0
         parsed_commands = await self.cli.evaluate_cli_command(line, ctx, True)
         for parsed in parsed_commands:
             nr_outputs, command_output_stream = await parsed.execute()
             total_nr_outputs = total_nr_outputs + (nr_outputs or 0)
```

### Comparing `resotocore-3.4.2/resotocore/infra_apps/package_manager.py` & `resotocore-3.5.0/resotocore/infra_apps/package_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterator, Optional, List, Dict, Union, Tuple
+from typing import AsyncIterator, Optional, List, Dict, Union, Tuple, Callable
 import asyncio
 from asyncio import Lock
 from pathlib import Path
 import aiohttp
 import aiofiles
 from collections import defaultdict
 from abc import ABC
@@ -13,14 +13,15 @@
 from resotocore.db.packagedb import PackageEntityDb, InfraAppPackage
 from resotocore.config import ConfigHandler
 from resotocore.config import ConfigEntity
 from resotocore.ids import InfraAppName, ConfigId
 from resotocore.model.model import Kind, ComplexKind
 from resotocore.types import Json
 from resotocore.model.typed_model import from_js
+from resotocore.cli.model import AliasTemplate
 from logging import getLogger
 from resotocore.web.service import Service
 
 logger = getLogger(__name__)
 
 
 def config_id(name: InfraAppName) -> ConfigId:
@@ -62,14 +63,16 @@
 
 
 class PackageManager(Service):
     def __init__(
         self,
         entity_db: PackageEntityDb,
         config_handler: ConfigHandler,
+        add_command_alias: Callable[[AliasTemplate], None],
+        remove_command_alias: Callable[[str], None],
         repos_cache_directory: Path = Path.home() / ".cache" / "resoto-infra-apps",
     ) -> None:
         """
         Package manager for infra apps.
 
         Args:
             entity_db: EntityDb for storing app manifests
@@ -79,19 +82,37 @@
 
         self.entity_db = entity_db
         self.config_handler = config_handler
         self.update_lock: Optional[Lock] = None
         self.repos_cache_directory: Path = repos_cache_directory
         self.cleanup_task: Optional[asyncio.Task[None]] = None
         self.cdn_url = "https://cdn.some.engineering/resoto/apps/index.json"
+        self.add_command_alias = add_command_alias
+        self.remove_command_alias = remove_command_alias
 
     async def start(self) -> None:
         self.update_lock = asyncio.Lock()
         self.repos_cache_directory.mkdir(parents=True, exist_ok=True)
 
+        # set up custom commands
+        manifests = [await self.get_manifest(name) async for name in self.list()]
+        self._setup_custom_commands([m for m in manifests if m is not None])
+
+    def _setup_custom_commands(self, manifests: List[AppManifest]) -> None:
+        for manifest in manifests:
+            alias_template = AliasTemplate(
+                name=manifest.name,
+                info=manifest.description,
+                template=f"apps run {manifest.name}" + r" {{args}}",
+                description=manifest.readme,
+                allowed_in_source_position=True,
+                infra_app_parameters=manifest.args_schema,
+            )
+            self.add_command_alias(alias_template)
+
     async def stop(self) -> None:
         if self.cleanup_task:
             self.cleanup_task.cancel()
             await self.cleanup_task
 
     async def search(self, query: Optional[str], url: Optional[str]) -> AsyncIterator[AppManifest]:
         maybe_available_manifests = await self._get_manifests(url)
@@ -202,16 +223,19 @@
 
     async def delete(self, name: InfraAppName) -> None:
         assert self.update_lock, "PackageManager not started"
         async with self.update_lock:
             await self._delete(name)
 
     async def _delete(self, name: InfraAppName) -> None:
+        if await self.entity_db.get(name) is None:
+            return
         await self.entity_db.delete(name)
-        await self.config_handler.delete_config(config_id(name))
+        # clean up the aliases
+        self.remove_command_alias(name)
 
     # user-facing method, errors are thrown as exceptions
     async def install(self, name: InfraAppName, url: Optional[str]) -> AppManifest:
         assert self.update_lock, "PackageManager not started"
 
         async with self.update_lock:
             if installed := await self.entity_db.get(name):
@@ -230,16 +254,21 @@
     ) -> Union[ManifestInstallFailed, AppManifest]:
         conf_id = config_id(manifest.name)
         if schema := manifest.config_schema:
             kinds: List[Kind] = [from_js(kind, ComplexKind) for kind in schema]
             await self.config_handler.update_configs_model(kinds)
         config_entity = ConfigEntity(conf_id, manifest.default_config or {}, None)
         try:
-            await self.config_handler.put_config(config_entity, validate=manifest.config_schema is not None)
+            if await self.config_handler.get_config(conf_id) is None:
+                await self.config_handler.put_config(config_entity, validate=manifest.config_schema is not None)
             stored = await self.entity_db.update(InfraAppPackage(manifest, url))
+
+            # add the custom command alias
+            self._setup_custom_commands([manifest])
+
             return stored.manifest
         except Exception as e:
             logger.error(f"Failed to install {manifest.name} from {url}", exc_info=e)
             return ManifestInstallFailed(manifest.name, str(e))
 
     async def _fetch_manifest(self, app_name: InfraAppName, url: str) -> Union[Failure, AppManifest]:
         url = url or self.cdn_url
```

### Comparing `resotocore-3.4.2/resotocore/infra_apps/runtime.py` & `resotocore-3.5.0/resotocore/infra_apps/runtime.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union, List, Any, AsyncIterator
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.types import JsonElement, Json
 from resotocore.ids import GraphName
 from attrs import frozen
 from abc import ABC, abstractmethod
-from argparse import Namespace
 
 
 @frozen
 class Failure:
     error: str
 
 
@@ -28,27 +27,27 @@
     @abstractmethod
     async def execute(
         self,
         graph: GraphName,
         manifest: AppManifest,
         config: Json,
         stdin: AsyncIterator[JsonElement],
-        kwargs: Namespace,
+        argv: List[str],
         ctx: Any,  # CLIContext, but here we use Any to avoid circular dependency
     ) -> AsyncIterator[JsonElement]:
         """
         Executes the infrastructure app."""
         yield None
 
     @abstractmethod
     async def generate_template(
         self,
         graph: GraphName,
         manifest: AppManifest,
         config: Json,
         stdin: AsyncIterator[JsonElement],
-        kwargs: Namespace,
+        argv: List[str],
     ) -> AsyncIterator[str]:
         """
         Generates the template for the infrastructure app. Does not execute any commands
         """
         yield ""
```

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/api/contents/all.json` & `resotocore-3.5.0/resotocore/jupyterlite/api/contents/all.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8949999999999999%*

 * *Differences: {"'content'": "{0: {'created': '2023-05-26T18:28:06.010286Z', 'last_modified': "*

 * *              "'2023-05-26T18:25:00.450546Z'}}",*

 * * "'created'": "'2023-05-26T18:28:06.010286Z'",*

 * * "'last_modified'": "'2023-05-26T18:28:06.010286Z'"}*

```diff
@@ -1,25 +1,25 @@
 {
     "content": [
         {
             "content": null,
-            "created": "2023-05-10T12:25:19.980588Z",
+            "created": "2023-05-26T18:28:06.010286Z",
             "format": null,
-            "last_modified": "2023-05-10T12:22:20.504118Z",
+            "last_modified": "2023-05-26T18:25:00.450546Z",
             "mimetype": null,
             "name": "example.ipynb",
             "path": "example.ipynb",
             "size": 7611,
             "type": "notebook",
             "writable": true
         }
     ],
-    "created": "2023-05-10T12:25:19.980588Z",
+    "created": "2023-05-26T18:28:06.010286Z",
     "format": "json",
-    "last_modified": "2023-05-10T12:25:19.980588Z",
+    "last_modified": "2023-05-26T18:28:06.010286Z",
     "mimetype": null,
     "name": "",
     "path": "",
     "size": null,
     "type": "directory",
     "writable": true
 }
```

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.5.0/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1408.7461890.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2557.75e9da2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/302.8bcc38f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3444.47d5ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4931.430433b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5238.1751cc3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6475.6037fbb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8370.8f855e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8685.d78bdab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8732.9320f73.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9382.9014799.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/9960.64cd61e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/build.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/close.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.5.0/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.5.0/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.5.0/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/json.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/python.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/react.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.5.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.5.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.5.0/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.5.0/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/config-utils.js` & `resotocore-3.5.0/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.5.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.5.0/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.5.0/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.5.0/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/index.html` & `resotocore-3.5.0/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.5.0/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.5.0/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.5.0/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.5.0/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.5.0/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/lab/index.html` & `resotocore-3.5.0/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.5.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/lab/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.5.0/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/package.json` & `resotocore-3.5.0/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.5.0/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/message_bus.py` & `resotocore-3.5.0/resotocore/message_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 log = logging.getLogger(__name__)
 
 
 class CoreMessage:
     Connected = "message-listener-connected"
     Disconnected = "message-listener-disconnected"
     ConfigUpdated = "config-updated"
+    ConfigCopied = "config-copied"
     ConfigDeleted = "config-deleted"
     ErrorMessage = "error"
     ProgressMessage = "progress"
 
 
 class Message(ABC):
     """
```

### Comparing `resotocore-3.4.2/resotocore/metrics.py` & `resotocore-3.5.0/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/adjust_node.py` & `resotocore-3.5.0/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/db_updater.py` & `resotocore-3.5.0/resotocore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/graph_access.py` & `resotocore-3.5.0/resotocore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/json_schema.py` & `resotocore-3.5.0/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/model.py` & `resotocore-3.5.0/resotocore/model/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/model_handler.py` & `resotocore-3.5.0/resotocore/model/model_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 from abc import ABC, abstractmethod
 from functools import reduce
-from typing import Optional, List, Set, Callable, Dict
+from typing import Optional, List, Set, Callable, Dict, Iterator
 
 from plantuml import PlantUML
 
 from resotocore.async_extensions import run_async
 from resotocore.db.db_access import DbAccess
 from resotocore.types import EdgeType
 from resotocore.ids import GraphName
@@ -34,30 +34,33 @@
         with_subclasses: bool = False,
         dependency_edges: Optional[Set[EdgeType]] = None,
         with_predecessors: bool = False,
         with_successors: bool = False,
         with_properties: bool = True,
         link_classes: bool = False,
         only_aggregate_roots: bool = True,
+        sort_props: bool = True,
     ) -> bytes:
         """
         Generate a PlantUML image of the model.
 
+        :param graph_name: the name of the graph
         :param output: "svg" or "png"
         :param show_packages: regexp that matches packages to show
         :param hide_packages: regexp that matches packages to hide
         :param with_inheritance: draw inheritance relationship between classes
         :param with_base_classes: include base classes for all matching classes to show in the diagram
         :param with_subclasses: include subclasses for all matching classes to show in the diagram
         :param dependency_edges: draw dependency edges of given edge type between classes
         :param with_predecessors: include predecessors for all matching classes to show in the diagram
         :param with_successors: include successors for all matching classes to show in the diagram
         :param with_properties: include properties for all matching classes to show in the diagram
         :param link_classes: add anchor links to all classes
         :param only_aggregate_roots: if the list of classes should be filtered for aggregate roots
+        :param sort_props: if the properties should be sorted by name
         :return: the generated image
         """
 
     @abstractmethod
     async def update_model(self, graph_name: GraphName, kinds: List[Kind]) -> Model:
         pass
 
@@ -121,21 +124,23 @@
         with_subclasses: bool = False,
         dependency_edges: Optional[Set[EdgeType]] = None,
         with_predecessors: bool = False,
         with_successors: bool = False,
         with_properties: bool = True,
         link_classes: bool = False,
         only_aggregate_roots: bool = True,
+        sort_props: bool = True,
     ) -> bytes:
         allowed_edge_types: Set[EdgeType] = dependency_edges or set()
         assert output in ("svg", "png", "puml"), "Only svg, png and puml is supported!"
         model = await self.load_model(graph_name)
         graph = model.graph()
         show = [re.compile(s) for s in show_packages] if show_packages else None
         hide = [re.compile(s) for s in hide_packages] if hide_packages else None
+        visited_complex: Set[str] = set()
 
         def not_hidden(key: str) -> bool:
             k: Kind = graph.nodes[key]["data"]
             return not (hide and exist(lambda r: r.fullmatch(k.fqn), hide))
 
         def node_visible(key: str) -> bool:
             k: Kind = graph.nodes[key]["data"]
@@ -149,15 +154,16 @@
 
         def class_node(cpx: ComplexKind) -> str:
             sth = {k.prop.name: k for k in cpx.synthetic_props() if len(k.path.path) == 1}
 
             def kind_name(p: Property) -> str:
                 return (sth[p.name].simple_kind.runtime_kind if p.name in sth else p.kind) if p.synthetic else p.kind
 
-            props = "\n".join([f"**{p.name}**: {kind_name(p)}" for p in cpx.properties]) if with_properties else ""
+            cpx_props = sorted(cpx.properties, key=lambda p: p.name) if sort_props else cpx.properties
+            props = "\n".join([f"**{p.name}**: {kind_name(p)}" for p in cpx_props]) if with_properties else ""
             link = f" [[#{cpx.fqn}]]" if link_classes else ""
             return f"class {cpx.fqn}{link} {{\n{props}\n}}"
 
         def descendants(cpx: ComplexKind) -> Set[str]:
             return {kind.fqn for kind in model.complex_kinds() if cpx.fqn in kind.kind_hierarchy()}
 
         def predecessors(cpx: ComplexKind) -> Set[str]:
@@ -172,14 +178,17 @@
             return (
                 {kind for et in allowed_edge_types for kind in cpx.successor_kinds.get(et, [])}
                 if isinstance(cpx, ComplexKind)
                 else set()
             )
 
         def complex_property_kinds(cpx: ComplexKind) -> Set[str]:
+            if cpx.fqn in visited_complex:
+                return set()
+            visited_complex.add(cpx.fqn)
             result: Set[str] = set()
             for _, k in cpx.property_with_kinds():
                 for cpl in k.nested_complex_kinds():
                     result.add(cpl.fqn)
                     result.update(complex_property_kinds(cpl))
             return result
 
@@ -197,17 +206,18 @@
         if with_predecessors:
             add_visible(predecessors)
         if with_successors:
             add_visible(successors)
         if with_properties:
             add_visible(complex_property_kinds)
 
-        nodes = "\n".join([class_node(node["data"]) for nid, node in graph.nodes(data=True) if nid in visible])
+        visible_nodes: Iterator[ComplexKind] = (node["data"] for nid, node in graph.nodes(data=True) if nid in visible)
+        nodes = "\n".join(class_node(node) for node in sorted(visible_nodes, key=lambda n: n.fqn))
         edges = ""
-        for fr, to, data in graph.edges(data=True):
+        for fr, to, data in sorted(graph.edges(data=True), key=lambda e: (e[0], e[1])):
             if fr in visible and to in visible:
                 if with_inheritance and data["type"] == "inheritance":
                     edges += f"{to} <|--- {fr}\n"
                 elif data["type"] == "successor" and data["edge_type"] in allowed_edge_types:
                     edges += f"{fr} -[#1A83AF]-> {to}\n"
                 elif data["type"] == "property" and with_properties:
                     edges += f"{fr} --> {to}\n"
```

### Comparing `resotocore-3.4.2/resotocore/model/resolve_in_graph.py` & `resotocore-3.5.0/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/transform_kind_convert.py` & `resotocore-3.5.0/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/model/typed_model.py` & `resotocore-3.5.0/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/query/__init__.py` & `resotocore-3.5.0/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/query/model.py` & `resotocore-3.5.0/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/query/query_parser.py` & `resotocore-3.5.0/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/query/template_expander.py` & `resotocore-3.5.0/resotocore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/query/template_expander_service.py` & `resotocore-3.5.0/resotocore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/report/__init__.py` & `resotocore-3.5.0/resotocore/report/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/report/benchmark_renderer.py` & `resotocore-3.5.0/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/report/inspector_service.py` & `resotocore-3.5.0/resotocore/report/inspector_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.template_expander = cli.dependencies.template_expander
         self.model_handler = cli.dependencies.model_handler
         self.event_sender = cli.dependencies.event_sender
 
     async def start(self) -> None:
         # TODO: we need a migration path for checks added in existing configs
         config_ids = {i async for i in self.config_handler.list_config_ids()}
-        overwrite = True  # only here to simplify development. True until we reach a stable version.
+        overwrite = False  # only here to simplify development. True until we reach a stable version.
         # we renamed this config in 3.2.6 - old installations still might have it
         # this line can be removed in a future version
         await self.config_handler.delete_config(ConfigId("resoto.report.benchmark.aws_cis_1.5"))
         for name, js in BenchmarkConfig.from_files().items():
             if overwrite or benchmark_id(name) not in config_ids:
                 cid = benchmark_id(name)
                 log.info(f"Creating benchmark config {cid}")
```

### Comparing `resotocore-3.4.2/resotocore/report/report_config.py` & `resotocore-3.5.0/resotocore/report/report_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         )
 
 
 @define
 class BenchmarkConfig(CheckCollectionConfig):
     kind: ClassVar[str] = BenchmarkConfigRoot
 
+    id: str = field(metadata={"description": "Unique ID of the benchmark."})
     framework: str = field(metadata={"description": "Framework the benchmark is based on."})
     version: str = field(metadata={"description": "Version of the benchmark."})
     clouds: Optional[List[str]] = field(
         default=None,
         metadata={
             "description": "List of applicable cloud providers. "
             "If the benchmark is not cloud specific, the value would be null."
```

### Comparing `resotocore-3.4.2/resotocore/static/api-doc.yaml` & `resotocore-3.5.0/resotocore/static/api-doc.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -30,24 +30,181 @@
     description: Endpoints to perform and maintain security, compliance and cost reports.
   - name: system
     description: Endpoints to get information about the system.
   - name: debug
     description: Endpoints to debug the system.
   - name: tsdb
     description: Endpoints to access the time series database.
+  - name: authorization
+    description: Endpoints to authorize access.
 
 paths:
 
   # region model
   /model:
     get:
+      summary: "[Deprecated] Get the currently defined model."
+      description: "Use /graph/{graph_id}/model instead."
+      deprecated: true
+      tags:
+        - model
+      parameters:
+        - name: flat
+          description: "If true, the hierarchy of complex kinds is flattened, holding all properties and all merged metadata."
+          in: query
+          schema:
+            type: boolean
+            default: false
+      responses:
+        "200":
+          description: "The list of all kinds."
+          content:
+            application/json:
+              schema:
+                $ref: "#/components/schemas/Kind"
+    patch:
+      summary: "[Deprecated] Add or update the current defined model."
+      description: "Use /graph/{graph_id}/model instead."
+      deprecated: true
+      tags:
+        - model
+      requestBody:
+        description: "Complete model or part of the model."
+        content:
+          application/json:
+            schema:
+              $ref: "#/components/schemas/Kind"
+      responses:
+        "200":
+          description: "OK if the model is updated successfully"
+          content:
+            application/json:
+              schema:
+                $ref: "#/components/schemas/Kind"
+        "400":
+          description: "Message that explains the error"
+          content:
+            text/plain:
+              schema:
+                type: string
+  /model/uml:
+    get:
+      summary: "[Deprecated] Get the currently defined model as svg uml image."
+      description: "Use /graph/{graph_id}/model/uml instead."
+      deprecated: true
+      tags:
+        - model
+      parameters:
+        - name: output
+          description: The output format.
+          in: query
+          schema:
+            type: string
+            enum:
+              - svg
+              - png
+            default: svg
+          required: false
+        - name: show
+          description: comma separated list of resources to show. Entries can be regexps.
+          in: query
+          schema:
+            type: string
+          required: false
+          explode: false
+          example: aws_ec2_instance,gcp.*
+        - name: hide
+          description: |
+            comma separated list of resources to hide. Entries can be regexps.
+            hide takes precedence over show.
+          in: query
+          schema:
+            type: string
+          required: false
+          explode: false
+          example: aws_ec2_instance,gcp.*
+        - name: with_inheritance
+          description: Include inheritance relations in the model.
+          in: query
+          schema:
+            type: boolean
+            default: true
+        - name: with_base_classes
+          description: Include all base classes of visible entries
+          in: query
+          schema:
+            type: boolean
+            default: true
+        - name: with_subclasses
+          description: Include all descendant classes of visible entries
+          in: query
+          schema:
+            type: boolean
+            default: false
+        - name: dependency
+          description: |
+            comma separated list of dependency relationships.
+          in: query
+          schema:
+            type: string
+          required: false
+          explode: false
+          example: default
+        - name: with_predecessors
+          description: Include all predecessors of selected entries
+          in: query
+          schema:
+            type: boolean
+            default: false
+        - name: with_successors
+          description: Include all successors of selected entries
+          in: query
+          schema:
+            type: boolean
+            default: false
+        - name: with_properties
+          description: Show properties of selected entries
+          in: query
+          schema:
+            type: boolean
+            default: true
+        - name: link_classes
+          description: Add anchor links to classes.
+          in: query
+          schema:
+            type: boolean
+            default: false
+        - name: aggregate_roots
+          description: Show aggregate roots.
+          in: query
+          schema:
+            type: boolean
+            default: true
+        - name: sort_props
+          description: Sort properties by name.
+          in: query
+          schema:
+            type: boolean
+            default: true
+      responses:
+        "200":
+          description: "Returns the model as uml diagram in svg format"
+  /graph/{graph_id}/model:
+    get:
       summary: "Get the currently defined model."
       tags:
         - model
       parameters:
+        - name: graph_id
+          in: path
+          description: "The identifier of the graph"
+          example: resoto
+          required: true
+          schema:
+            type: string
         - name: flat
           description: "If true, the hierarchy of complex kinds is flattened, holding all properties and all merged metadata."
           in: query
           schema:
               type: boolean
               default: false
       responses:
@@ -57,14 +214,22 @@
             application/json:
               schema:
                 $ref: "#/components/schemas/Kind"
     patch:
       summary: "Add or update the current defined model."
       tags:
         - model
+      parameters:
+        - name: graph_id
+          in: path
+          description: "The identifier of the graph"
+          example: resoto
+          required: true
+          schema:
+            type: string
       requestBody:
         description: "Complete model or part of the model."
         content:
           application/json:
             schema:
               $ref: "#/components/schemas/Kind"
       responses:
@@ -76,20 +241,27 @@
                 $ref: "#/components/schemas/Kind"
         "400":
           description: "Message that explains the error"
           content:
             text/plain:
               schema:
                 type: string
-  /model/uml:
+  /graph/{graph_id}/model/uml:
     get:
       summary: "Get the currently defined model as svg uml image."
       tags:
         - model
       parameters:
+        - name: graph_id
+          in: path
+          description: "The identifier of the graph"
+          example: resoto
+          required: true
+          schema:
+            type: string
         - name: output
           description: The output format.
           in: query
           schema:
             type: string
             enum:
               - svg
@@ -161,14 +333,26 @@
             default: true
         - name: link_classes
           description: Add anchor links to classes.
           in: query
           schema:
             type: boolean
             default: false
+        - name: aggregate_roots
+          description: Show aggregate roots.
+          in: query
+          schema:
+            type: boolean
+            default: true
+        - name: sort_props
+          description: Sort properties by name.
+          in: query
+          schema:
+            type: boolean
+            default: true
       responses:
         "200":
           description: "Returns the model as uml diagram in svg format"
   # endregion
 
   # region graph management
   /graph:
@@ -2829,14 +3013,162 @@
               schema:
                 type: string
                 example: "1.1 node1"
           description: "The response from the tsdb."
 
   # endregion
 
+  # region authorization
+
+  /.well-known/jwks.json:
+    description: "This endpoint is used by the authorization server to get the public keys of the configured JWT issuer."
+    get:
+      summary: "Get the public keys of the configured JWT issuer."
+      tags:
+        - authorization
+      responses:
+        "200":
+          description: "The public keys of the configured JWT issuer."
+          content:
+            application/json:
+              example: |
+                {
+                  "keys": [
+                    {
+                      "alg": "sha256WithRSAEncryption",
+                      "e": "AQAB",
+                      "kid": "fDKvq05HG0...",
+                      "kty": "RSA",
+                      "n": "u7cp95GkUOj...",
+                      "use": "sig",
+                      "x5c": [ "MIIDoTCCAomgAw..." ],
+                      "x5t": "DMpDIyR...",
+                      "x5t#S256": "fDKvq05HG0Oz...."
+                    }
+                  ]
+                }
+
+
+
+
+  /login:
+    get:
+      summary: "This endpoint is used to login the user."
+      tags:
+        - authorization
+      description: "Authenticate the user. This endpoint needs to be accessed from a browser! It is possible that the user is redirected to another authentication server."
+      responses:
+        "200":
+          description: "The login page."
+  /create-first-user:
+    post:
+      summary: "This endpoint is used to create the first user."
+      tags:
+          - authorization
+      description: "Create the first user from the create first user login form."
+      requestBody:
+        content:
+            application/x-www-form-urlencoded:
+              schema:
+                type: object
+                properties:
+                  company:
+                    type: string
+                    description: The company name.
+                  fullname:
+                    type: string
+                    description: The full name of the user.
+                  email:
+                    type: string
+                    description: The email of the user.
+                  password:
+                    type: string
+                    description: The password of the user.
+                  password_repeat:
+                    type: string
+                    description: The repeated password of the user.
+                  redirect:
+                    type: string
+                    description: The redirect url after the user is created.
+      responses:
+        "303":
+          description: "The redirect to the specified url in the form."
+
+  /authenticate:
+    summary: "This endpoint is used to authenticate the user."
+    post:
+      summary: "This endpoint is used to authenticate the user."
+      description: "Authenticate the user. This endpoint needs to be accessed from a browser! It is possible that the user is redirected to another authentication server."
+      tags:
+        - authorization
+      requestBody:
+        content:
+          application/x-www-form-urlencoded:
+            schema:
+              type: object
+              properties:
+                email:
+                  type: string
+                  description: The email of the user.
+                password:
+                  type: string
+                  description: The password of the user.
+                redirect:
+                  type: string
+                  description: The redirect url after the user is created.
+      responses:
+        "303":
+          description: "The redirect to the specified url in the form with a code parameter added."
+
+
+  /authorization/user:
+    get:
+      summary: "This endpoint is used to get the user information."
+      tags:
+        - authorization
+      description: "Get the user information."
+      responses:
+        "200":
+          description: "The user information."
+          content:
+            application/json:
+              example: |
+                {
+                  "email": "test@test.de",
+                  "exp": 1683660989,
+                  "roles": "admin"
+                }
+  /authorization/renew:
+    get:
+      summary: "This endpoint is used to renew a JWT that is about to expire."
+      tags:
+          - authorization
+      description: "Get the user information."
+      responses:
+        "200":
+          description: "The user information."
+          headers:
+            Authorization:
+              description: The authorization header with the renewed JWT.
+              schema:
+                type: string
+          content:
+            application/json:
+              example: |
+                {
+                  "email": "test@test.de",
+                  "exp": 1683665359,
+                  "roles": "admin"
+                }
+
+
+
+
+  # endregion
+
 components:
   schemas:
     AnalyticsEvent:
       description: "An analytics event."
       type: object
       properties:
         system:
```

### Comparing `resotocore-3.4.2/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.5.0/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.5.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/check_template.json` & `resotocore-3.5.0/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.5.0/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/task/model.py` & `resotocore-3.5.0/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/task/scheduler.py` & `resotocore-3.5.0/resotocore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.5.0/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/task/subscribers.py` & `resotocore-3.5.0/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/task/task_description.py` & `resotocore-3.5.0/resotocore/task/task_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 import logging
 import uuid
 from abc import ABC
+from asyncio import Task
 from contextlib import suppress
 from datetime import timedelta, datetime
 from enum import Enum
 from typing import Optional, Any, Sequence, MutableSequence, Callable, Dict, List, Set, Tuple, Union
 
-from attrs import define
-
-from asyncio import Task
-
 from apscheduler.triggers.cron import CronTrigger
+from attrs import define
 from frozendict import frozendict
 from jsons import set_deserializer, set_serializer
 from transitions import Machine, State, MachineError
 
-from resotocore.ids import TaskId
-from resotocore.task.model import Subscriber
+from resotocore.ids import SubscriberId, TaskDescriptorId, TaskId
 from resotocore.message_bus import Event, Action, ActionDone, Message, ActionError, ActionInfo, ActionProgress
 from resotocore.model.typed_model import to_json, from_js, to_js
+from resotocore.task.model import Subscriber
 from resotocore.types import Json
 from resotocore.util import first, interleave, empty, exist, identity, utc, utc_str
-from resotocore.ids import SubscriberId, TaskDescriptorId
 from resotolib.core.progress import ProgressTree, Progress, ProgressDone
 
 log = logging.getLogger(__name__)
 
 
 class StepErrorBehaviour(Enum):
     """
@@ -136,16 +133,15 @@
 class SendMessage(TaskCommand):
     message: Message
 
 
 @define(order=True, hash=True, frozen=True)
 class ExecuteOnCLI(TaskCommand):
     command: str
-    # noinspection PyUnresolvedReferences
-    env: frozendict
+    env: frozendict  # type: ignore # jsons can not handle frozendict type parameters
 
 
 # endregion
 
 
 # region Trigger: when a task should be triggered
 class Trigger(ABC):
```

### Comparing `resotocore-3.4.2/resotocore/task/task_handler.py` & `resotocore-3.5.0/resotocore/task/task_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     SendMessage,
     ExecuteOnCLI,
     StepErrorBehaviour,
     RestartAgainStepAction,
     Trigger,
 )
 from resotocore.util import first, Periodic, group_by, utc_str, utc, partition_by
+import re
 
 log = logging.getLogger(__name__)
 
 
 class TaskHandlerService(TaskHandler):
     # region init
 
@@ -308,15 +309,22 @@
 
     async def list_jobs(self) -> List[Job]:
         return [td for td in self.task_descriptions if isinstance(td, Job)]
 
     async def list_workflows(self) -> List[Workflow]:
         return [td for td in self.task_descriptions if isinstance(td, Workflow)]
 
-    async def add_job(self, job: Job) -> None:
+    def __check_system_job(self, name: str) -> None:
+        # : is not allowed in job names
+        if re.match(r"^[^:]+$", name) is None:
+            raise AttributeError(f"System jobs can't be modified: {name}")
+
+    async def add_job(self, job: Job, force: bool = False) -> None:
+        if not force:
+            self.__check_system_job(job.name)
         descriptions = list(self.task_descriptions)
         existing = first(lambda td: td.id == job.id, descriptions)
         if existing:
             if not existing.mutable:
                 raise AttributeError(f"There is an existing job with this {job.id} which can not be deleted!")
             log.info(f"Job with id {job.id} already exists. Update this job.")
             descriptions.remove(existing)
@@ -345,15 +353,17 @@
         if task.update_task and not task.update_task.done():
             task.update_task.cancel()
 
         # mark step as error
         task.end()
         await self.mark_done_in_database(task)
 
-    async def delete_job(self, job_id: str) -> Optional[Job]:
+    async def delete_job(self, job_id: str, force: bool = False) -> Optional[Job]:
+        if not force:
+            self.__check_system_job(job_id)
         job: Job = first(lambda td: td.id == job_id and isinstance(td, Job), self.task_descriptions)  # type: ignore
         if job:
             if not job.mutable:
                 raise AttributeError(f"Can not delete job: {job.id} - it is defined in a system file!")
             # delete all running tasks of this job
             for task in list(filter(lambda x: x.descriptor.id == job.id, self.tasks.values())):
                 log.info(f"Job: {job_id}: delete running task: {task.id}")
```

### Comparing `resotocore-3.4.2/resotocore/types.py` & `resotocore-3.5.0/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/util.py` & `resotocore-3.5.0/resotocore/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     List,
     Tuple,
     AsyncIterator,
     Iterator,
     Union,
     Sequence,
 )
+import re
 
 from dateutil.parser import isoparse, parse as parse_date
 from resotolib.asynchronous import periodic
 
 from resotolib.durations import parse_duration
 from resotocore.error import RestartService
 from resotocore.types import JsonElement, Json
@@ -69,29 +70,32 @@
     for key in keys:
         res.pop(key, None)  # type: ignore
     return res
 
 
 UTC_Date_Format = "%Y-%m-%dT%H:%M:%SZ"
 
+# short iso 8601 format, e.g. 20230504T080910Z
+UTC_Date_Format_short = "%Y%m%dT%H%M%SZ"
+
 
 def rnd_str(str_len: int = 10) -> str:
     return "".join(random.choice(string.ascii_uppercase + string.digits) for _ in range(str_len))
 
 
 def utc() -> datetime:
     return datetime.now(timezone.utc)
 
 
-def utc_str(dt: datetime = utc()) -> str:
+def utc_str(dt: datetime = utc(), date_format: str = UTC_Date_Format) -> str:
     if dt.tzinfo is not None and dt.tzname() != "UTC":
         offset = dt.tzinfo.utcoffset(dt)
         if offset is not None and offset.total_seconds() != 0:
             dt = (dt - offset).replace(tzinfo=timezone.utc)
-    return dt.strftime(UTC_Date_Format)
+    return dt.strftime(date_format)
 
 
 def from_utc(date_string: str) -> datetime:
     return isoparse(date_string)
 
 
 def parse_utc(date_string: str) -> datetime:
@@ -445,7 +449,12 @@
 
     @staticmethod
     def wrap_object(
         obj: Any, not_existent: Any = AccessNone(None), simple_formatter: Callable[[Any], Any] = identity
     ) -> AccessJson:
         # only here for a typed result
         return AccessJson.wrap(obj, not_existent, simple_formatter)  # type: ignore
+
+
+def check_graph_name(name: str) -> None:
+    if not re.match(r"^[a-zA-Z0-9_]+$", name):
+        raise ValueError(f"Graph name {name} contains invalid characters, only alphanumeric characters are allowed.")
```

### Comparing `resotocore-3.4.2/resotocore/validator.py` & `resotocore-3.5.0/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/web/api.py` & `resotocore-3.5.0/resotocore/web/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import shutil
 import string
 import tempfile
 import uuid
 import zipfile
 from asyncio import Future, Queue
 from contextlib import asynccontextmanager
-from datetime import timedelta
+from datetime import timedelta, datetime, timezone
 from functools import partial
 from io import BytesIO
 from pathlib import Path
 from random import SystemRandom
 from typing import (
     AsyncGenerator,
     Any,
@@ -24,30 +24,33 @@
     Dict,
     AsyncIterator,
     Tuple,
     Callable,
     Awaitable,
     Iterable,
 )
+from urllib.parse import urlencode, urlparse, parse_qs, urlunparse
 
+import aiohttp_jinja2
+import jinja2
 import prometheus_client
 import yaml
 from aiohttp import (
     web,
     MultipartWriter,
     AsyncIterablePayload,
     BufferedReaderPayload,
     MultipartReader,
     ClientSession,
     TCPConnector,
 )
 from aiohttp.abc import AbstractStreamWriter
 from aiohttp.hdrs import METH_ANY
 from aiohttp.web import Request, StreamResponse, WebSocketResponse
-from aiohttp.web_exceptions import HTTPNotFound, HTTPNoContent, HTTPOk, HTTPNotAcceptable
+from aiohttp.web_exceptions import HTTPNotFound, HTTPNoContent, HTTPOk, HTTPNotAcceptable, HTTPSeeOther
 from aiohttp.web_fileresponse import FileResponse
 from aiohttp.web_response import json_response
 from aiohttp_swagger3 import SwaggerFile, SwaggerUiSettings
 from aiostream import stream
 from attrs import evolve
 from networkx.readwrite import cytoscape_data
 from resotoui import ui_path
@@ -55,40 +58,41 @@
 from resotocore.analytics import AnalyticsEventSender, AnalyticsEvent
 from resotocore.cli.command import alias_names
 from resotocore.cli.model import (
     ParsedCommandLine,
     CLIContext,
     CLICommand,
     InternalPart,
-    AliasTemplate,
     WorkerCustomCommand,
     CLI,
+    AliasTemplate,
 )
 from resotocore.config import ConfigHandler, ConfigValidation, ConfigEntity
 from resotocore.console_renderer import ConsoleColorSystem, ConsoleRenderer
 from resotocore.core_config import CoreConfig
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import GraphDB, HistoryChange
 from resotocore.db.model import QueryModel
 from resotocore.error import NotFoundError
-from resotocore.ids import TaskId, ConfigId, NodeId, SubscriberId, WorkerId, GraphName
+from resotocore.ids import TaskId, ConfigId, NodeId, SubscriberId, WorkerId, GraphName, Email, Password
 from resotocore.message_bus import MessageBus, Message, ActionDone, Action, ActionError, ActionInfo, ActionProgress
 from resotocore.model.db_updater import merge_graph_process
 from resotocore.model.graph_access import Section
 from resotocore.model.json_schema import json_schema
 from resotocore.model.model import Kind, Model
 from resotocore.model.model_handler import ModelHandler
 from resotocore.model.typed_model import to_json, from_js, to_js_str, to_js
 from resotocore.query import QueryParser
 from resotocore.report import Inspector
 from resotocore.task.model import Subscription
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.types import Json, JsonElement
-from resotocore.util import uuid_str, force_gen, rnd_str, if_set, duration, utc_str, parse_utc, async_noop
+from resotocore.user import UserManagement
+from resotocore.util import uuid_str, force_gen, rnd_str, if_set, duration, utc_str, parse_utc, async_noop, utc
 from resotocore.web.certificate_handler import CertificateHandler
 from resotocore.web.content_renderer import result_binary_gen, single_result
 from resotocore.web.directives import (
     metrics_handler,
     error_handler,
     on_response_prepare,
     cors_handler,
@@ -99,32 +103,47 @@
 from resotocore.worker_task_queue import (
     WorkerTaskDescription,
     WorkerTaskQueue,
     WorkerTask,
     WorkerTaskResult,
     WorkerTaskInProgress,
 )
-from resotolib.asynchronous.web.auth import auth_handler, set_valid_jwt, raw_jwt_from_auth_message
+from resotocore.web.auth import raw_jwt_from_auth_message, AuthorizedUser, AuthHandler
 from resotolib.asynchronous.web.ws_handler import accept_websocket, clean_ws_handler
 from resotolib.jwt import encode_jwt
+from resotolib.x509 import cert_to_bytes
 
 log = logging.getLogger(__name__)
 
 
 def section_of(request: Request) -> Optional[str]:
     section = request.match_info.get("section", request.query.get("section"))
     if section and section != "/" and section not in Section.content:
         raise AttributeError(f"Given section does not exist: {section}")
     return section
 
 
 # No Authorization required for following paths
-AlwaysAllowed = {"/", "/metrics", "/api-doc.*", "/system/.*", "/ui.*", "/ca/cert", "/notebook.*"}
+AlwaysAllowed = {
+    "/",
+    "/.well-known/.*",
+    "/api-doc.*",
+    "/authenticate",
+    "/ca/cert",
+    "/create-first-user",
+    "/login",
+    "/metrics",
+    "/static/.*",
+    "/system/.*",
+    "/ui.*",
+    "/notebook/.*",
+    "/debug/.*",
+}
 # Authorization is not required, but implemented as part of the request handler
-DeferredCheck = {"/events"}
+DeferredCheck = {"/events", "/work/queue"}
 
 
 class Api:
     def __init__(
         self,
         db: DbAccess,
         model_handler: ModelHandler,
@@ -135,14 +154,15 @@
         worker_task_queue: WorkerTaskQueue,
         cert_handler: CertificateHandler,
         config_handler: ConfigHandler,
         inspector: Inspector,
         cli: CLI,
         query_parser: QueryParser,
         config: CoreConfig,
+        user_management: UserManagement,
         get_override: Callable[[ConfigId], Optional[Json]],
     ):
         self.db = db
         self.model_handler = model_handler
         self.subscription_handler = subscription_handler
         self.workflow_handler = workflow_handler
         self.message_bus = message_bus
@@ -150,34 +170,39 @@
         self.worker_task_queue = worker_task_queue
         self.cert_handler = cert_handler
         self.config_handler = config_handler
         self.inspector = inspector
         self.cli = cli
         self.query_parser = query_parser
         self.config = config
+        self.user_management = user_management
         self.get_override = get_override
+        self.auth_handler = AuthHandler(db.system_data_db, config, cert_handler, AlwaysAllowed | DeferredCheck)
 
         self.app = web.Application(
             client_max_size=config.api.max_request_size or 1024**2,
             # note on order: the middleware is passed in the order provided.
             middlewares=[
                 metrics_handler,
-                auth_handler(config.args.psk, AlwaysAllowed | DeferredCheck),
+                self.auth_handler.middleware(),
                 cors_handler,
                 error_handler(config, event_sender),
                 default_middleware(self),
             ],
         )
         self.app.on_response_prepare.append(on_response_prepare)
         self._session: Optional[ClientSession] = None
         self.in_shutdown = False
         self.websocket_handler: Dict[str, Tuple[Future[Any], WebSocketResponse]] = {}
         path_part = config.api.web_path.strip().strip("/").strip()
         web_path = "" if path_part == "" else f"/{path_part}"
         self.__add_routes(web_path)
+        aiohttp_jinja2.setup(
+            self.app, loader=jinja2.FileSystemLoader(os.path.abspath(os.path.dirname(__file__) + "/../templates"))
+        )
 
     @property
     def session(self) -> ClientSession:
         if self._session is None:
             # only keep connections alive for 15 seconds, cleanup closed transports
             connector = TCPConnector(keepalive_timeout=15.0, enable_cleanup_closed=True)
             self._session = ClientSession(connector=connector)
@@ -186,20 +211,22 @@
     def __add_routes(self, prefix: str) -> None:
         static_path = os.path.abspath(os.path.dirname(__file__) + "/../static")
         jupyterlite_path = Path(os.path.abspath(os.path.dirname(__file__) + "/../jupyterlite"))
         if not jupyterlite_path.exists():
             jupyterlite_path.mkdir(parents=True, exist_ok=True)
         self.app.add_routes(
             [
-                # Model operations
+                # Model operations (backwards compatible)
                 web.get(prefix + "/model", self.get_model),
-                web.get(prefix + "/model/{graph_id}", self.get_model),
-                web.get(prefix + "/model/{graph_id}/uml", self.model_uml),
                 web.patch(prefix + "/model", self.update_model),
-                web.patch(prefix + "/model/{graph_id}", self.update_model),
+                web.get(prefix + "/model/uml", self.model_uml),
+                # Graph based model operations
+                web.get(prefix + "/graph/{graph_id}/model", self.get_model),
+                web.patch(prefix + "/graph/{graph_id}/model", self.update_model),
+                web.get(prefix + "/graph/{graph_id}/model/uml", self.model_uml),
                 # CRUD Graph operations
                 web.get(prefix + "/graph", self.list_graphs),
                 web.get(prefix + "/graph/{graph_id}", self.get_node),
                 web.post(prefix + "/graph/{graph_id}", self.create_graph),
                 web.delete(prefix + "/graph/{graph_id}", self.wipe),
                 # search the graph
                 web.post(prefix + "/graph/{graph_id}/search/raw", self.raw),
@@ -276,52 +303,145 @@
                 # system operations
                 web.get(prefix + "/system/ping", self.ping),
                 web.get(prefix + "/system/ready", self.ready),
                 # forwards
                 web.get(prefix + "/tsdb", self.forward("/tsdb/")),
                 web.get(prefix + "/ui", self.forward("/ui/index.html")),
                 web.get(prefix + "/ui/", self.forward("/ui/index.html")),
-                web.get(prefix + "/debug/ui/{commit}/{path:.+}", self.serve_debug_ui),
+                # auth operations
+                web.get(prefix + "/.well-known/jwks.json", self.jwks),
+                web.get(prefix + "/login", self.login_page),
+                web.post(prefix + "/create-first-user", self.create_first_user),
+                web.post(prefix + "/authenticate", self.authenticate),
+                web.get(prefix + "/authorization/user", self.get_authorized_user),
+                web.get(prefix + "/authorization/renew", self.renew_authorization),
                 # tsdb operations
                 web.route(METH_ANY, prefix + "/tsdb/{tail:.+}", tsdb(self)),
                 web.static(f"{prefix}/ui/", ui_path),
             ]
         )
+        if self.config.runtime.debug:
+            self.app.add_routes([web.get(prefix + "/debug/ui/{commit}/{path:.+}", self.serve_debug_ui)])
         SwaggerFile(
             self.app,
             spec_file=f"{static_path}/api-doc.yaml",
             swagger_ui_settings=SwaggerUiSettings(path=prefix + "/api-doc", layout="BaseLayout", docExpansion="none"),
         )
 
     async def start(self) -> None:
-        pass
+        await self.auth_handler.start()
 
     async def stop(self) -> None:
+        await self.auth_handler.stop()
         if not self.in_shutdown:
             self.in_shutdown = True
             for ws_id in list(self.websocket_handler):
                 await clean_ws_handler(ws_id, self.websocket_handler)
             if self.session:
                 await self.session.close()
 
     @staticmethod
+    async def login_with_redirect(request: Request) -> StreamResponse:
+        params = request.query.copy()
+        params["redirect"] = request.raw_path
+        return web.HTTPSeeOther("/login?" + urlencode(params))
+
+    @staticmethod
     def forward(to: str) -> Callable[[Request], Awaitable[StreamResponse]]:
-        async def forward_to(_: Request) -> StreamResponse:
-            return web.HTTPFound(to)
+        async def forward_to(request: Request) -> StreamResponse:
+            goto = to + "?" + urlencode(request.query) if request.query else to
+            return web.HTTPFound(goto)
 
         return forward_to
 
     @staticmethod
     async def ping(_: Request) -> StreamResponse:
         return web.HTTPOk(text="pong", content_type="text/plain")
 
     @staticmethod
     async def ready(_: Request) -> StreamResponse:
         return web.HTTPOk(text="ok")
 
+    async def jwks(self, _: Request) -> StreamResponse:
+        return web.json_response(self.auth_handler.signing_key_jwk)
+
+    async def login_page(self, request: Request) -> StreamResponse:
+        template = "login.html" if await self.user_management.has_users() else "create_first_user.html"
+        return aiohttp_jinja2.render_template(template, request, context=request.query)
+
+    async def create_first_user(self, request: Request) -> StreamResponse:
+        post_data = await request.post()
+        errors = []
+        try:
+            email = Email(str(post_data.get("email", "")).strip())
+            password = Password(str(post_data.get("password", "")))
+            password_repeat = str(post_data.get("password_repeat", ""))
+            company = str(post_data.get("company", "")).strip()
+            fullname = str(post_data.get("fullname", "")).strip()
+            if not email or email.startswith("@") or email.endswith("@") or email.count("@") != 1:
+                errors.append("Invalid email address")
+            if not password:
+                errors.append("Password is required")
+            if not company:
+                errors.append("Company name is required")
+            if not fullname:
+                errors.append("Full name is required")
+            if password != password_repeat:
+                errors.append("Passwords do not match")
+            if not errors:
+                await self.user_management.create_first_user(company, fullname, email, password)
+                return await self.authenticate(request)
+        except Exception as e:
+            errors.append(str(e))
+        error_string = ". ".join(errors)
+        return aiohttp_jinja2.render_template(
+            "create_first_user.html", request, context={**post_data, "error": error_string}
+        )
+
+    async def authenticate(self, request: Request) -> StreamResponse:
+        post_data = await request.post()
+        email = Email(str(post_data.get("email", "")))
+        password = Password(str(post_data.get("password", "")))
+        redirect = str(post_data.get("redirect", ""))
+        if email and password and (user := await self.user_management.login(email, password)):
+            params: Dict[str, List[str]] = {}
+            if self.config.args.psk:
+                code = await self.auth_handler.add_authorized_user(AuthorizedUser(email, user.roles, utc()))
+                params["code"] = [code]
+            if redirect:
+                if params:
+                    parsed = urlparse(redirect)
+                    query_params = parse_qs(parsed.query)
+                    query_params.update(params)
+                    parsed = parsed._replace(query=urlencode(query_params, doseq=True))
+                    redirect = urlunparse(parsed)
+                response: StreamResponse = HTTPSeeOther(redirect)
+            else:
+                response = HTTPOk(text=urlencode(params, doseq=True))
+            return response
+        return aiohttp_jinja2.render_template(
+            "login.html", request, context=dict(**post_data, error="Invalid username or password")
+        )
+
+    @staticmethod
+    async def get_authorized_user(request: Request) -> StreamResponse:
+        if jwt := request.get("jwt"):
+            return web.json_response(jwt)
+        else:
+            return web.HTTPNoContent()
+
+    async def renew_authorization(self, request: Request) -> StreamResponse:
+        if jwt_raw := request.get("jwt"):
+            exp = datetime.fromtimestamp(int(jwt_raw["exp"]), tz=timezone.utc)
+            user = AuthorizedUser(jwt_raw["email"], set(jwt_raw["roles"].split(",")), exp)
+            renewed, data = self.auth_handler.user_jwt(user)
+            return web.json_response(data, headers={"Authorization": f"Bearer {renewed}"})
+        else:
+            return HTTPNoContent()  # no psk, no renewal
+
     async def list_configs(self, request: Request) -> StreamResponse:
         return await self.stream_response_from_gen(request, self.config_handler.list_config_ids())
 
     async def get_config(self, request: Request) -> StreamResponse:
         config_id = ConfigId(request.match_info["config_id"])
         accept = request.headers.get("accept", "application/json")
         not_found = HTTPNotFound(text="No config with this id")
@@ -433,15 +553,15 @@
             headers["Authorization"] = "Bearer " + encode_jwt({"sha256_fingerprint": fingerprint}, self.config.args.psk)
         return HTTPOk(headers=headers, body=cert, content_type="application/x-pem-file")
 
     async def sign_certificate(self, request: Request) -> StreamResponse:
         csr_bytes = await request.content.read()
         cert, fingerprint = self.cert_handler.sign(csr_bytes)
         headers = {"SHA256-Fingerprint": fingerprint}
-        return HTTPOk(headers=headers, body=cert, content_type="application/x-pem-file")
+        return HTTPOk(headers=headers, body=cert_to_bytes(cert), content_type="application/x-pem-file")
 
     @staticmethod
     async def metrics(_: Request) -> StreamResponse:
         resp = web.Response(body=prometheus_client.generate_latest())
         resp.content_type = prometheus_client.CONTENT_TYPE_LATEST
         return resp
 
@@ -533,17 +653,14 @@
         graph = GraphName(request.match_info["graph_id"])
         check_id = request.match_info["check_id"]
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
         inspections = await self.inspector.list_failing_resources(graph, check_id, accounts)
         return await self.stream_response_from_gen(request, inspections)
 
-    async def redirect_to_api_doc(self, request: Request) -> StreamResponse:
-        raise web.HTTPFound("api-doc")
-
     async def handle_events(self, request: Request) -> StreamResponse:
         show = request.query["show"].split(",") if "show" in request.query else ["*"]
         return await self.listen_to_events(request, SubscriberId(str(uuid.uuid1())), show)
 
     async def send_analytics_events(self, request: Request) -> StreamResponse:
         events_json = await self.json_from_request(request)
         events = from_js(events_json, List[AnalyticsEvent])
@@ -557,15 +674,15 @@
         event_types: List[str],
         initial_messages: Optional[Sequence[Message]] = None,
     ) -> WebSocketResponse:
         handler: Callable[[str], Awaitable[None]] = async_noop
 
         async def authorize_request(msg: str) -> None:
             nonlocal handler
-            if (r := raw_jwt_from_auth_message(msg)) and set_valid_jwt(request, r, self.config.args.psk) is not None:
+            if (r := raw_jwt_from_auth_message(msg)) and await self.auth_handler.validate_jwt(r, request) is not None:
                 handler = handle_message
             else:
                 raise ValueError("No Authorization header provided and no valid auth message sent")
 
         async def handle_message(msg: str) -> None:
             js = json.loads(msg)
             if "data" in js:
@@ -597,28 +714,28 @@
     async def handle_work_tasks(self, request: Request) -> WebSocketResponse:
         worker_id = WorkerId(uuid_str())
         worker_descriptions: Future[List[WorkerTaskDescription]] = asyncio.get_event_loop().create_future()
         handler: Callable[[str], Awaitable[None]] = async_noop
 
         async def authorize_request(msg: str) -> None:
             nonlocal handler
-            if (r := raw_jwt_from_auth_message(msg)) and set_valid_jwt(request, r, self.config.args.psk) is not None:
+            if (r := raw_jwt_from_auth_message(msg)) and await self.auth_handler.validate_jwt(r, request) is not None:
                 handler = handle_connect
             else:
                 raise ValueError("No Authorization header provided and no valid auth message sent")
 
         async def handle_connect(msg: str) -> None:
             nonlocal handler
             cmds = from_js(json.loads(msg), List[WorkerCustomCommand])
             description = [WorkerTaskDescription(cmd.name, cmd.filter) for cmd in cmds]
             # set the future and allow attaching the worker to the task queue
             worker_descriptions.set_result(description)
             # register the descriptions as custom command on the CLI
             for cmd in cmds:
-                self.cli.register_worker_custom_command(cmd)
+                self.cli.register_alias_template(cmd.to_template())
             # the connect process is done, define the final handler
             handler = handle_message
 
         async def handle_message(msg: str) -> None:
             tr = from_js(json.loads(msg), WorkerTaskResult)
             if tr.result == "error":
                 error = tr.error if tr.error else "worker signalled error without detailed error message"
@@ -670,28 +787,30 @@
         with_subclasses = request.query.get("with_subclasses", "false") != "false"
         dependency = set(request.query["dependency"].split(",")) if "dependency" in request.query else None
         with_predecessors = request.query.get("with_predecessors", "false") != "false"
         with_successors = request.query.get("with_successors", "false") != "false"
         with_properties = request.query.get("with_properties", "true") != "false"
         aggregate_roots = request.query.get("aggregate_roots", "true") != "false"
         link_classes = request.query.get("link_classes", "false") != "false"
+        sort_props = request.query.get("sort_props", "true") != "false"
         result = await self.model_handler.uml_image(
-            graph=graph_id,
+            graph_name=graph_id,
             output=output,
             show_packages=show,
             hide_packages=hide,
             with_inheritance=with_inheritance,
             with_base_classes=with_base_classes,
             with_subclasses=with_subclasses,
             dependency_edges=dependency,  # type: ignore
             with_predecessors=with_predecessors,
             with_successors=with_successors,
             with_properties=with_properties,
             link_classes=link_classes,
             only_aggregate_roots=aggregate_roots,
+            sort_props=sort_props,
         )
         response = web.StreamResponse()
         mt = {"svg": "image/svg+xml", "png": "image/png", "puml": "text/plain"}
         response.headers["Content-Type"] = mt[output]
         await response.prepare(request)
         await response.write_eof(result)
         return response
```

### Comparing `resotocore-3.4.2/resotocore/web/certificate_handler.py` & `resotocore-3.5.0/resotocore/web/certificate_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import logging
 from datetime import timedelta
 from pathlib import Path
 from ssl import SSLContext, create_default_context, Purpose
 from tempfile import TemporaryDirectory
-from typing import Tuple, Optional, List
+from typing import Tuple, Optional, List, Union, Dict
 
 from arango.database import StandardDatabase
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
-from cryptography.x509 import Certificate
+from cryptography.x509 import Certificate, CertificateSigningRequest
 
 from resotocore.core_config import CoreConfig, CertificateConfig
 from resotocore.types import Json
 from resotocore.util import Periodic
 from resotolib.utils import get_local_ip_addresses, get_local_hostnames
 from resotolib.x509 import (
     bootstrap_ca,
@@ -87,18 +87,25 @@
             san_ip_addresses=ip_addresses,
             discover_local_dns_names=False,
             discover_local_ip_addresses=False,
         )
         cert = sign_csr(csr, self._ca_key, self._ca_cert, days_valid)
         return key, cert
 
-    def sign(self, csr_bytes: bytes) -> Tuple[bytes, str]:
-        csr = load_csr_from_bytes(csr_bytes)
-        certificate = sign_csr(csr, self._ca_key, self._ca_cert)
-        return cert_to_bytes(certificate), cert_fingerprint(certificate)
+    def sign(
+        self,
+        csr_or_bytes: Union[CertificateSigningRequest, bytes],
+        days_valid: int = 365,
+        server_auth: bool = True,
+        client_auth: bool = True,
+        key_usage: Optional[Dict[str, bool]] = None,
+    ) -> Tuple[Certificate, str]:
+        csr = load_csr_from_bytes(csr_or_bytes) if isinstance(csr_or_bytes, bytes) else csr_or_bytes
+        certificate = sign_csr(csr, self._ca_key, self._ca_cert, days_valid, server_auth, client_auth, key_usage)
+        return certificate, cert_fingerprint(certificate)
 
     @property
     def host_context(self) -> Optional[SSLContext]:
         return self._host_context
 
     @property
     def client_context(self) -> SSLContext:
```

### Comparing `resotocore-3.4.2/resotocore/web/content_renderer.py` & `resotocore-3.5.0/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/web/directives.py` & `resotocore-3.5.0/resotocore/web/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 
     if request.method in (METH_GET, METH_HEAD, METH_POST, METH_PUT, METH_DELETE, METH_PATCH):
         response.headers["Access-Control-Allow-Origin"] = request.headers.get("origin", "*")
         response.headers["Access-Control-Allow-Methods"] = request.headers.get("access-control-request-method", "*")
         response.headers["Access-Control-Allow-Headers"] = request.headers.get("access-control-request-headers", "*")
         response.headers["Access-Control-Max-Age"] = "86400"
 
+    # If requested, send the JWT in the response header
+    if auth_header := request.get("send_auth_response_header"):
+        response.headers["Authorization"] = auth_header
+
 
 @middleware
 async def cors_handler(request: Request, handler: RequestHandler) -> StreamResponse:
     if request.method == METH_OPTIONS:
         return HTTPNoContent(
             headers={
                 # allow origin of request or all if none is defined.
```

### Comparing `resotocore-3.4.2/resotocore/web/tsdb.py` & `resotocore-3.5.0/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore/worker_task_queue.py` & `resotocore-3.5.0/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/resotocore.egg-info/PKG-INFO` & `resotocore-3.5.0/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.4.2
+Version: 3.5.0
 Summary: Keeps all the things.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotocore
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `resotocore-3.4.2/resotocore.egg-info/SOURCES.txt` & `resotocore-3.5.0/resotocore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 resotocore/action_handlers/merge_outer_edge_handler.py
 resotocore/analytics/__init__.py
 resotocore/analytics/posthog.py
 resotocore/analytics/recurrent_events.py
 resotocore/cli/__init__.py
 resotocore/cli/cli.py
 resotocore/cli/command.py
+resotocore/cli/dependencies.py
 resotocore/cli/model.py
 resotocore/cli/tip_of_the_day.py
 resotocore/config/__init__.py
 resotocore/config/config_handler_service.py
 resotocore/config/config_override_service.py
 resotocore/config/core_config_handler.py
 resotocore/db/__init__.py
@@ -54,15 +55,18 @@
 resotocore/db/graphdb.py
 resotocore/db/jobdb.py
 resotocore/db/model.py
 resotocore/db/modeldb.py
 resotocore/db/packagedb.py
 resotocore/db/runningtaskdb.py
 resotocore/db/subscriberdb.py
+resotocore/db/system_data_db.py
 resotocore/db/templatedb.py
+resotocore/graph_manager/__init__.py
+resotocore/graph_manager/graph_manager.py
 resotocore/infra_apps/__init__.py
 resotocore/infra_apps/local_runtime.py
 resotocore/infra_apps/manifest.py
 resotocore/infra_apps/package_manager.py
 resotocore/infra_apps/runtime.py
 resotocore/jupyterlite/bootstrap.js
 resotocore/jupyterlite/config-utils.js
@@ -591,14 +595,16 @@
 resotocore/query/template_expander_service.py
 resotocore/report/__init__.py
 resotocore/report/benchmark_renderer.py
 resotocore/report/inspector_service.py
 resotocore/report/report_config.py
 resotocore/static/api-doc.yaml
 resotocore/static/ck-unicode-truecolor.ans
+resotocore/static/resoto.css
+resotocore/static/resoto_logo_and_text.svg
 resotocore/static/report/benchmark_template.json
 resotocore/static/report/check_template.json
 resotocore/static/report/benchmark/aws/aws_cis_1_5.json
 resotocore/static/report/checks/aws/aws_apigateway.json
 resotocore/static/report/checks/aws/aws_cloudtrail.json
 resotocore/static/report/checks/aws/aws_config.json
 resotocore/static/report/checks/aws/aws_ec2.json
@@ -612,14 +618,20 @@
 resotocore/task/job_handler.py
 resotocore/task/model.py
 resotocore/task/scheduler.py
 resotocore/task/start_workflow_on_first_subscriber.py
 resotocore/task/subscribers.py
 resotocore/task/task_description.py
 resotocore/task/task_handler.py
+resotocore/templates/base.html
+resotocore/templates/create_first_user.html
+resotocore/templates/login.html
+resotocore/user/__init__.py
+resotocore/user/user_management.py
 resotocore/web/__init__.py
 resotocore/web/api.py
+resotocore/web/auth.py
 resotocore/web/certificate_handler.py
 resotocore/web/content_renderer.py
 resotocore/web/directives.py
 resotocore/web/service.py
 resotocore/web/tsdb.py
```

### Comparing `resotocore-3.4.2/setup.cfg` & `resotocore-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `resotocore-3.4.2/setup.py` & `resotocore-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
             pip.main(["install", "-r", "requirements-jupyterlite.txt"])
             check_call(["jupyter", "lite", "build", "--config", "jupyter_lite_config.json"])
 
 
 setup(
     name="resotocore",
-    version="3.4.2",
+    version="3.5.0",
     description="Keeps all the things.",
     python_requires=">=3.5",
     classifiers=["Programming Language :: Python :: 3"],
     entry_points={"console_scripts": ["resotocore=resotocore.__main__:main"]},
     install_requires=read_requirements("requirements.txt"),
     license="Apache Software License 2.0",
     long_description=read("README.md"),
```


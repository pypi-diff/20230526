# Comparing `tmp/taskcluster-taskgraph-5.1.1.tar.gz` & `tmp/taskcluster-taskgraph-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.1.1.tar", last modified: Tue May 23 20:45:28 2023, max compression
+gzip compressed data, was "dist/taskcluster-taskgraph-5.2.0.tar", last modified: Fri May 26 16:55:09 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.1.1.tar` & `taskcluster-taskgraph-5.2.0.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.200580 taskcluster-taskgraph-5.1.1/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/MANIFEST.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-05-23 20:45:28.200580 taskcluster-taskgraph-5.1.1/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/README.rst
--rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/pyproject.toml
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/requirements/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/base.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)    20973 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/base.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/dev.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1182 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/dev.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/test.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9437 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/requirements/test.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-05-23 20:45:28.200580 taskcluster-taskgraph-5.1.1/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3839 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-05-23 20:45:28.000000 taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-05-23 20:23:06.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/cancel.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/actions/util.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/config.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/filter_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15585 2023-05-23 18:38:54.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/graph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/loader/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/loader/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/loader/default.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/loader/transform.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    26094 2023-05-23 18:38:54.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/morph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/parameters.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/hgrc
--rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    44051 2023-05-02 13:20:13.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/run-task
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-02-08 18:55:54.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.180580 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/fetch.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.190580 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    51225 2023-05-23 18:38:54.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.190580 taskcluster-taskgraph-5.1.1/src/taskgraph/util/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/archive.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2617 2023-05-23 18:38:49.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/hash.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/shell.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/templates.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-23 20:45:28.200580 taskcluster-taskgraph-5.1.1/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.1.1/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_actions_registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.1.1/test/test_create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_graph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7403 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_morph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15145 2023-05-23 18:38:49.000000 taskcluster-taskgraph-5.1.1/test/test_optimize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_optimize_strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_parameters.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_scripts_fetch_content.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11792 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_scripts_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_transform_docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_job.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_job_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_job_toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-23 18:38:54.000000 taskcluster-taskgraph-5.1.1/test/test_transforms_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_util_parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.1.1/test/test_util_python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_util_taskcluster.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_templates.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_util_vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.1.1/test/test_util_verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_util_workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.1.1/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      710 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20557 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8476 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      710 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3911 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       51 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-05-26 16:54:36.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15585 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    44051 2023-05-02 13:20:13.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6695 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    51243 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-05-26 16:55:09.000000 taskcluster-taskgraph-5.2.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.2.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.2.0/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11792 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4891 2023-05-26 13:56:54.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.2.0/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.2.0/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.2.0/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.2.0/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taskcluster-taskgraph-5.1.1/LICENSE` & `taskcluster-taskgraph-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/PKG-INFO` & `taskcluster-taskgraph-5.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.1.1
+Version: 5.2.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Provides-Extra: load-image
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `taskcluster-taskgraph-5.1.1/README.rst` & `taskcluster-taskgraph-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/pyproject.toml` & `taskcluster-taskgraph-5.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/requirements/base.txt` & `taskcluster-taskgraph-5.2.0/requirements/base.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,119 +9,106 @@
     --hash=sha256:7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41 \
     --hash=sha256:a841dacd6b99318a741b166adb07e19ee71a274450e68237b4650ca1055ab128
     # via -r requirements/base.in
 arrow==1.2.3 \
     --hash=sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1 \
     --hash=sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2
     # via jinja2-time
-attrs==22.2.0 \
-    --hash=sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836 \
-    --hash=sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99
+attrs==23.1.0 \
+    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
+    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
     # via -r requirements/base.in
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via requests
 chardet==5.1.0 \
     --hash=sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5 \
     --hash=sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9
     # via binaryornot
-charset-normalizer==3.0.1 \
-    --hash=sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b \
-    --hash=sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42 \
-    --hash=sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d \
-    --hash=sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b \
-    --hash=sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a \
-    --hash=sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59 \
-    --hash=sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154 \
-    --hash=sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1 \
-    --hash=sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c \
-    --hash=sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a \
-    --hash=sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d \
-    --hash=sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6 \
-    --hash=sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b \
-    --hash=sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b \
-    --hash=sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783 \
-    --hash=sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5 \
-    --hash=sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918 \
-    --hash=sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555 \
-    --hash=sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639 \
-    --hash=sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786 \
-    --hash=sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e \
-    --hash=sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed \
-    --hash=sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820 \
-    --hash=sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8 \
-    --hash=sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3 \
-    --hash=sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541 \
-    --hash=sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14 \
-    --hash=sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be \
-    --hash=sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e \
-    --hash=sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76 \
-    --hash=sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b \
-    --hash=sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c \
-    --hash=sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b \
-    --hash=sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3 \
-    --hash=sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc \
-    --hash=sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6 \
-    --hash=sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59 \
-    --hash=sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4 \
-    --hash=sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d \
-    --hash=sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d \
-    --hash=sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3 \
-    --hash=sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a \
-    --hash=sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea \
-    --hash=sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6 \
-    --hash=sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e \
-    --hash=sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603 \
-    --hash=sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24 \
-    --hash=sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a \
-    --hash=sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58 \
-    --hash=sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678 \
-    --hash=sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a \
-    --hash=sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c \
-    --hash=sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6 \
-    --hash=sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18 \
-    --hash=sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174 \
-    --hash=sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317 \
-    --hash=sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f \
-    --hash=sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc \
-    --hash=sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837 \
-    --hash=sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41 \
-    --hash=sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c \
-    --hash=sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579 \
-    --hash=sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753 \
-    --hash=sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8 \
-    --hash=sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291 \
-    --hash=sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087 \
-    --hash=sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866 \
-    --hash=sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3 \
-    --hash=sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d \
-    --hash=sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1 \
-    --hash=sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca \
-    --hash=sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e \
-    --hash=sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db \
-    --hash=sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72 \
-    --hash=sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d \
-    --hash=sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc \
-    --hash=sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539 \
-    --hash=sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d \
-    --hash=sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af \
-    --hash=sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b \
-    --hash=sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602 \
-    --hash=sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f \
-    --hash=sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478 \
-    --hash=sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c \
-    --hash=sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e \
-    --hash=sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479 \
-    --hash=sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7 \
-    --hash=sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8
+charset-normalizer==3.1.0 \
+    --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
+    --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
+    --hash=sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e \
+    --hash=sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373 \
+    --hash=sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62 \
+    --hash=sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230 \
+    --hash=sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be \
+    --hash=sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c \
+    --hash=sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0 \
+    --hash=sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448 \
+    --hash=sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f \
+    --hash=sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649 \
+    --hash=sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d \
+    --hash=sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0 \
+    --hash=sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706 \
+    --hash=sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a \
+    --hash=sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59 \
+    --hash=sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23 \
+    --hash=sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5 \
+    --hash=sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb \
+    --hash=sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e \
+    --hash=sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e \
+    --hash=sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c \
+    --hash=sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28 \
+    --hash=sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d \
+    --hash=sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41 \
+    --hash=sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974 \
+    --hash=sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce \
+    --hash=sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f \
+    --hash=sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1 \
+    --hash=sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d \
+    --hash=sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8 \
+    --hash=sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017 \
+    --hash=sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31 \
+    --hash=sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7 \
+    --hash=sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8 \
+    --hash=sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e \
+    --hash=sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14 \
+    --hash=sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd \
+    --hash=sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d \
+    --hash=sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795 \
+    --hash=sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b \
+    --hash=sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b \
+    --hash=sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b \
+    --hash=sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203 \
+    --hash=sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f \
+    --hash=sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19 \
+    --hash=sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1 \
+    --hash=sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a \
+    --hash=sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac \
+    --hash=sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9 \
+    --hash=sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0 \
+    --hash=sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137 \
+    --hash=sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f \
+    --hash=sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6 \
+    --hash=sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5 \
+    --hash=sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909 \
+    --hash=sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f \
+    --hash=sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0 \
+    --hash=sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324 \
+    --hash=sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755 \
+    --hash=sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb \
+    --hash=sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854 \
+    --hash=sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c \
+    --hash=sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60 \
+    --hash=sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84 \
+    --hash=sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0 \
+    --hash=sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b \
+    --hash=sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1 \
+    --hash=sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531 \
+    --hash=sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1 \
+    --hash=sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11 \
+    --hash=sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326 \
+    --hash=sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df \
+    --hash=sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
     --hash=sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48
     # via cookiecutter
 cookiecutter==2.1.1 \
     --hash=sha256:9f3ab027cec4f70916e28f03470bdb41e637a3ad354b4d65c765d93aad160022 \
@@ -131,27 +118,33 @@
     --hash=sha256:04ba1a3a099c3093fa8d24a422913c6a9b2c2cd22bcffc939cf72e3e98f672d7 \
     --hash=sha256:2595ab291d30717cda8474b874c9fd509f1b9802ad7f6968c36a45e4b13eb337
     # via mozilla-repo-urls
 idna==3.4 \
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
+importlib-metadata==6.6.0 \
+    --hash=sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed \
+    --hash=sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705
+    # via
+    #   attrs
+    #   click
 jinja2==3.1.2 \
     --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
     --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
     # via
     #   cookiecutter
     #   jinja2-time
 jinja2-time==0.2.0 \
     --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
     --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
-json-e==4.5.0 \
-    --hash=sha256:618a94aecc8b8bc7733d6cd0ee7b676e45675566625a38958aa8b30379d9758f \
-    --hash=sha256:e733ce77b4acbbc2c48211057f8cb5af45999e6be4ce0f07585c5580df45826e
+json-e==4.5.2 \
+    --hash=sha256:0d1203645a5753dec2da1ceab279f82169023948eff858b87968117e8a592e10 \
+    --hash=sha256:b1c82e79ec232b8a86393488b39aa086f8c098cf67fa190ac03517daf0e51aed
     # via -r requirements/base.in
 markupsafe==2.1.2 \
     --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
     --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
     --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
     --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
     --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
@@ -257,17 +250,17 @@
     # via
     #   -r requirements/base.in
     #   cookiecutter
 redo==2.0.4 \
     --hash=sha256:81066955041c853b0e6491eb65a0877dce45131c4cfa3d42d923fc2aa8f7a043 \
     --hash=sha256:c76e4c23ab2f8840261736a851323cd98493710e7a9d36a1058535dca501f293
     # via -r requirements/base.in
-requests==2.28.2 \
-    --hash=sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa \
-    --hash=sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf
+requests==2.31.0 \
+    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
+    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   -r requirements/base.in
     #   cookiecutter
     #   requests-unixsocket
 requests-unixsocket==0.3.0 \
     --hash=sha256:28304283ea9357d45fff58ad5b11e47708cfbf5806817aa59b2a363228ee971e \
     --hash=sha256:c685c680f0809e1b2955339b1e5afc3c0022b3066f4f7eb343f43a6065fc0e5d
@@ -285,15 +278,25 @@
     --hash=sha256:b25e122ecec249c4299ac7b20b08db76e3e2025bdaeb699a9d444556de5fd367 \
     --hash=sha256:f66dcbd6572a6216ab65949f0fa0b91f2df647918028436c384e6af5cd12ae2b
     # via -r requirements/base.in
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
     # via python-slugify
-urllib3==1.26.14 \
-    --hash=sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72 \
-    --hash=sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1
+typing-extensions==4.6.2 \
+    --hash=sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c \
+    --hash=sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98
+    # via
+    #   arrow
+    #   importlib-metadata
+urllib3==2.0.2 \
+    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
+    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
     # via requests
 voluptuous==0.13.1 \
     --hash=sha256:4b838b185f5951f2d6e8752b68fcf18bd7a9c26ded8f143f92d6d28f3921a3e6 \
     --hash=sha256:e8d31c20601d6773cb14d4c0f42aee29c6821bbd1018039aac7ac5605b489723
     # via -r requirements/base.in
+zipp==3.15.0 \
+    --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
+    --hash=sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556
+    # via importlib-metadata
```

### Comparing `taskcluster-taskgraph-5.1.1/requirements/test.txt` & `taskcluster-taskgraph-5.2.0/requirements/test.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,170 +2,146 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-cachetools==5.2.1 \
-    --hash=sha256:5991bc0e08a1319bb618d3195ca5b6bc76646a49c21d55962977197b301cc1fe \
-    --hash=sha256:8462eebf3a6c15d25430a8c27c56ac61340b2ecf60c9ce57afc2b97e450e47da
+cachetools==5.3.0 \
+    --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
+    --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
     # via tox
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
-coverage==7.0.5 \
-    --hash=sha256:051afcbd6d2ac39298d62d340f94dbb6a1f31de06dfaf6fcef7b759dd3860c45 \
-    --hash=sha256:0a1890fca2962c4f1ad16551d660b46ea77291fba2cc21c024cd527b9d9c8809 \
-    --hash=sha256:0ee30375b409d9a7ea0f30c50645d436b6f5dfee254edffd27e45a980ad2c7f4 \
-    --hash=sha256:13250b1f0bd023e0c9f11838bdeb60214dd5b6aaf8e8d2f110c7e232a1bff83b \
-    --hash=sha256:17e01dd8666c445025c29684d4aabf5a90dc6ef1ab25328aa52bedaa95b65ad7 \
-    --hash=sha256:19245c249aa711d954623d94f23cc94c0fd65865661f20b7781210cb97c471c0 \
-    --hash=sha256:1caed2367b32cc80a2b7f58a9f46658218a19c6cfe5bc234021966dc3daa01f0 \
-    --hash=sha256:1f66862d3a41674ebd8d1a7b6f5387fe5ce353f8719040a986551a545d7d83ea \
-    --hash=sha256:220e3fa77d14c8a507b2d951e463b57a1f7810a6443a26f9b7591ef39047b1b2 \
-    --hash=sha256:276f4cd0001cd83b00817c8db76730938b1ee40f4993b6a905f40a7278103b3a \
-    --hash=sha256:29de916ba1099ba2aab76aca101580006adfac5646de9b7c010a0f13867cba45 \
-    --hash=sha256:2a7f23bbaeb2a87f90f607730b45564076d870f1fb07b9318d0c21f36871932b \
-    --hash=sha256:2c407b1950b2d2ffa091f4e225ca19a66a9bd81222f27c56bd12658fc5ca1209 \
-    --hash=sha256:30b5fec1d34cc932c1bc04017b538ce16bf84e239378b8f75220478645d11fca \
-    --hash=sha256:3c2155943896ac78b9b0fd910fb381186d0c345911f5333ee46ac44c8f0e43ab \
-    --hash=sha256:411d4ff9d041be08fdfc02adf62e89c735b9468f6d8f6427f8a14b6bb0a85095 \
-    --hash=sha256:436e103950d05b7d7f55e39beeb4d5be298ca3e119e0589c0227e6d0b01ee8c7 \
-    --hash=sha256:49640bda9bda35b057b0e65b7c43ba706fa2335c9a9896652aebe0fa399e80e6 \
-    --hash=sha256:4a950f83fd3f9bca23b77442f3a2b2ea4ac900944d8af9993743774c4fdc57af \
-    --hash=sha256:50a6adc2be8edd7ee67d1abc3cd20678987c7b9d79cd265de55941e3d0d56499 \
-    --hash=sha256:52ab14b9e09ce052237dfe12d6892dd39b0401690856bcfe75d5baba4bfe2831 \
-    --hash=sha256:54f7e9705e14b2c9f6abdeb127c390f679f6dbe64ba732788d3015f7f76ef637 \
-    --hash=sha256:66e50680e888840c0995f2ad766e726ce71ca682e3c5f4eee82272c7671d38a2 \
-    --hash=sha256:790e4433962c9f454e213b21b0fd4b42310ade9c077e8edcb5113db0818450cb \
-    --hash=sha256:7a38362528a9115a4e276e65eeabf67dcfaf57698e17ae388599568a78dcb029 \
-    --hash=sha256:7b05ed4b35bf6ee790832f68932baf1f00caa32283d66cc4d455c9e9d115aafc \
-    --hash=sha256:7e109f1c9a3ece676597831874126555997c48f62bddbcace6ed17be3e372de8 \
-    --hash=sha256:949844af60ee96a376aac1ded2a27e134b8c8d35cc006a52903fc06c24a3296f \
-    --hash=sha256:95304068686545aa368b35dfda1cdfbbdbe2f6fe43de4a2e9baa8ebd71be46e2 \
-    --hash=sha256:9e662e6fc4f513b79da5d10a23edd2b87685815b337b1a30cd11307a6679148d \
-    --hash=sha256:a9fed35ca8c6e946e877893bbac022e8563b94404a605af1d1e6accc7eb73289 \
-    --hash=sha256:b69522b168a6b64edf0c33ba53eac491c0a8f5cc94fa4337f9c6f4c8f2f5296c \
-    --hash=sha256:b78729038abea6a5df0d2708dce21e82073463b2d79d10884d7d591e0f385ded \
-    --hash=sha256:b8c56bec53d6e3154eaff6ea941226e7bd7cc0d99f9b3756c2520fc7a94e6d96 \
-    --hash=sha256:b9727ac4f5cf2cbf87880a63870b5b9730a8ae3a4a360241a0fdaa2f71240ff0 \
-    --hash=sha256:ba3027deb7abf02859aca49c865ece538aee56dcb4871b4cced23ba4d5088904 \
-    --hash=sha256:be9fcf32c010da0ba40bf4ee01889d6c737658f4ddff160bd7eb9cac8f094b21 \
-    --hash=sha256:c18d47f314b950dbf24a41787ced1474e01ca816011925976d90a88b27c22b89 \
-    --hash=sha256:c76a3075e96b9c9ff00df8b5f7f560f5634dffd1658bafb79eb2682867e94f78 \
-    --hash=sha256:cbfcba14a3225b055a28b3199c3d81cd0ab37d2353ffd7f6fd64844cebab31ad \
-    --hash=sha256:d254666d29540a72d17cc0175746cfb03d5123db33e67d1020e42dae611dc196 \
-    --hash=sha256:d66187792bfe56f8c18ba986a0e4ae44856b1c645336bd2c776e3386da91e1dd \
-    --hash=sha256:d8d04e755934195bdc1db45ba9e040b8d20d046d04d6d77e71b3b34a8cc002d0 \
-    --hash=sha256:d8f3e2e0a1d6777e58e834fd5a04657f66affa615dae61dd67c35d1568c38882 \
-    --hash=sha256:e057e74e53db78122a3979f908973e171909a58ac20df05c33998d52e6d35757 \
-    --hash=sha256:e4ce984133b888cc3a46867c8b4372c7dee9cee300335e2925e197bcd45b9e16 \
-    --hash=sha256:ea76dbcad0b7b0deb265d8c36e0801abcddf6cc1395940a24e3595288b405ca0 \
-    --hash=sha256:ecb0f73954892f98611e183f50acdc9e21a4653f294dfbe079da73c6378a6f47 \
-    --hash=sha256:ef14d75d86f104f03dea66c13188487151760ef25dd6b2dbd541885185f05f40 \
-    --hash=sha256:f26648e1b3b03b6022b48a9b910d0ae209e2d51f50441db5dce5b530fad6d9b1 \
-    --hash=sha256:f67472c09a0c7486e27f3275f617c964d25e35727af952869dd496b9b5b7f6a3
+coverage==7.2.6 \
+    --hash=sha256:004948e296149644d208964300cb3d98affc5211e9e490e9979af4030b0d6473 \
+    --hash=sha256:13cde6bb0e58fb67d09e2f373de3899d1d1e866c5a9ff05d93615f2f54fbd2bb \
+    --hash=sha256:1c9e4a5eb1bbc3675ee57bc31f8eea4cd7fb0cbcbe4912cf1cb2bf3b754f4a80 \
+    --hash=sha256:2025f913f2edb0272ef15d00b1f335ff8908c921c8eb2013536fcaf61f5a683d \
+    --hash=sha256:25bad4196104761bc26b1dae9b57383826542ec689ff0042f7f4f4dd7a815cba \
+    --hash=sha256:2692306d3d4cb32d2cceed1e47cebd6b1d2565c993d6d2eda8e6e6adf53301e6 \
+    --hash=sha256:272ab31228a9df857ab5df5d67936d8861464dc89c5d3fab35132626e9369379 \
+    --hash=sha256:2e8c0e79820cdd67978e1120983786422d279e07a381dbf89d03bbb23ec670a6 \
+    --hash=sha256:3062fd5c62df988cea9f2972c593f77fed1182bfddc5a3b12b1e606cb7aba99e \
+    --hash=sha256:3436927d1794fa6763b89b60c896f9e3bd53212001026ebc9080d23f0c2733c1 \
+    --hash=sha256:35db06450272473eab4449e9c2ad9bc6a0a68dab8e81a0eae6b50d9c2838767e \
+    --hash=sha256:392154d09bd4473b9d11351ab5d63391f3d5d24d752f27b3be7498b0ee2b5226 \
+    --hash=sha256:3cff6980fe7100242170092bb40d2b1cdad79502cd532fd26b12a2b8a5f9aee0 \
+    --hash=sha256:42c692b55a647a832025a4c048007034fe77b162b566ad537ce65ad824b12a84 \
+    --hash=sha256:44c9b9f1a245f3d0d202b1a8fa666a80b5ecbe4ad5d0859c0fb16a52d9763224 \
+    --hash=sha256:496b86f1fc9c81a1cd53d8842ef712e950a4611bba0c42d33366a7b91ba969ec \
+    --hash=sha256:4bbd58eb5a2371bf160590f4262109f66b6043b0b991930693134cb617bc0169 \
+    --hash=sha256:4e3783a286d5a93a2921396d50ce45a909aa8f13eee964465012f110f0cbb611 \
+    --hash=sha256:4f3c7c19581d471af0e9cb49d928172cd8492cd78a2b7a4e82345d33662929bb \
+    --hash=sha256:52c139b7ab3f0b15f9aad0a3fedef5a1f8c0b2bdc291d88639ca2c97d3682416 \
+    --hash=sha256:541280dde49ce74a4262c5e395b48ea1207e78454788887118c421cb4ffbfcac \
+    --hash=sha256:5906f6a84b47f995cd1bf0aca1c72d591c55ee955f98074e93660d64dfc66eb9 \
+    --hash=sha256:6284a2005e4f8061c58c814b1600ad0074ccb0289fe61ea709655c5969877b70 \
+    --hash=sha256:6727a0d929ff0028b1ed8b3e7f8701670b1d7032f219110b55476bb60c390bfb \
+    --hash=sha256:697f4742aa3f26c107ddcb2b1784a74fe40180014edbd9adaa574eac0529914c \
+    --hash=sha256:6b9f64526286255735847aed0221b189486e0b9ed943446936e41b7e44b08783 \
+    --hash=sha256:6babcbf1e66e46052442f10833cfc4a0d3554d8276aa37af8531a83ed3c1a01d \
+    --hash=sha256:6e7f1a8328eeec34c54f1d5968a708b50fc38d31e62ca8b0560e84a968fbf9a9 \
+    --hash=sha256:71f739f97f5f80627f1fee2331e63261355fd1e9a9cce0016394b6707ac3f4ec \
+    --hash=sha256:76d06b721c2550c01a60e5d3093f417168658fb454e5dfd9a23570e9bffe39a1 \
+    --hash=sha256:77a04b84d01f0e12c66f16e69e92616442dc675bbe51b90bfb074b1e5d1c7fbd \
+    --hash=sha256:97729e6828643f168a2a3f07848e1b1b94a366b13a9f5aba5484c2215724edc8 \
+    --hash=sha256:9a8723ccec4e564d4b9a79923246f7b9a8de4ec55fa03ec4ec804459dade3c4f \
+    --hash=sha256:a5ffd45c6b93c23a8507e2f436983015c6457aa832496b6a095505ca2f63e8f1 \
+    --hash=sha256:a6f03f87fea579d55e0b690d28f5042ec1368650466520fbc400e7aeaf09e995 \
+    --hash=sha256:aac1d5fdc5378f6bac2c0c7ebe7635a6809f5b4376f6cf5d43243c1917a67087 \
+    --hash=sha256:ae82c5f168d2a39a5d69a12a69d4dc23837a43cf2ca99be60dfe59996ea6b113 \
+    --hash=sha256:bc7b667f8654376e9353dd93e55e12ce2a59fb6d8e29fce40de682273425e044 \
+    --hash=sha256:c1d7a31603c3483ac49c1726723b0934f88f2c011c660e6471e7bd735c2fa110 \
+    --hash=sha256:c534431153caffc7c495c3eddf7e6a6033e7f81d78385b4e41611b51e8870446 \
+    --hash=sha256:c93d52c3dc7b9c65e39473704988602300e3cc1bad08b5ab5b03ca98bbbc68c1 \
+    --hash=sha256:cbcc874f454ee51f158afd604a315f30c0e31dff1d5d5bf499fc529229d964dd \
+    --hash=sha256:d3cacc6a665221108ecdf90517a8028d07a2783df3417d12dcfef1c517e67478 \
+    --hash=sha256:d712cefff15c712329113b01088ba71bbcef0f7ea58478ca0bbec63a824844cb \
+    --hash=sha256:d7786b2fa7809bf835f830779ad285215a04da76293164bb6745796873f0942d \
+    --hash=sha256:dc11b42fa61ff1e788dd095726a0aed6aad9c03d5c5984b54cb9e1e67b276aa5 \
+    --hash=sha256:dc4d5187ef4d53e0d4c8eaf530233685667844c5fb0b855fea71ae659017854b \
+    --hash=sha256:f5440cdaf3099e7ab17a5a7065aed59aff8c8b079597b61c1f8be6f32fe60636 \
+    --hash=sha256:fa079995432037b5e2ef5ddbb270bcd2ded9f52b8e191a5de11fe59a00ea30d8 \
+    --hash=sha256:fbe6e8c0a9a7193ba10ee52977d4d5e7652957c1f56ccefed0701db8801a2a3b \
+    --hash=sha256:fde5c7a9d9864d3e07992f66767a9817f24324f354caa3d8129735a3dc74f126
     # via -r requirements/test.in
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
-exceptiongroup==1.1.0 \
-    --hash=sha256:327cbda3da756e2de031a3107b81ab7b3770a602c4d16ca618298c526f4bec1e \
-    --hash=sha256:bcb67d800a4497e1b404c2dd44fca47d3b7a5e5433dbab67f96c1a685cdfdf23
+exceptiongroup==1.1.1 \
+    --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
+    --hash=sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785
     # via pytest
-filelock==3.9.0 \
-    --hash=sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de \
-    --hash=sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d
+filelock==3.12.0 \
+    --hash=sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9 \
+    --hash=sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718
     # via
     #   tox
     #   virtualenv
-importlib-metadata==6.0.0 \
-    --hash=sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad \
-    --hash=sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d
-    # via
-    #   pluggy
-    #   pytest
-    #   tox
-    #   virtualenv
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
-mock==5.0.1 \
-    --hash=sha256:c41cfb1e99ba5d341fbcc5308836e7d7c9786d302f995b2c271ce2144dece9eb \
-    --hash=sha256:e3ea505c03babf7977fd21674a69ad328053d414f05e6433c30d8fa14a534a6b
+mock==5.0.2 \
+    --hash=sha256:06f18d7d65b44428202b145a9a36e99c2ee00d1eb992df0caf881d4664377891 \
+    --hash=sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56
     # via -r requirements/test.in
-packaging==23.0 \
-    --hash=sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2 \
-    --hash=sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97
+packaging==23.1 \
+    --hash=sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61 \
+    --hash=sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f
     # via
     #   pyproject-api
     #   pytest
     #   tox
-platformdirs==2.6.2 \
-    --hash=sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490 \
-    --hash=sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2
+platformdirs==3.5.1 \
+    --hash=sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f \
+    --hash=sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0 \
     --hash=sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159 \
     --hash=sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3
     # via
     #   pytest
     #   tox
-pyproject-api==1.4.0 \
-    --hash=sha256:ac85c1f82e0291dbae5a7739dbb9a990e11ee4034c9b5599ea714f07a24ecd71 \
-    --hash=sha256:c34226297781efdd1ba4dfb74ce21076d9a8360e2125ea31803c1a02c76b2460
+pyproject-api==1.5.1 \
+    --hash=sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9 \
+    --hash=sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43
     # via tox
-pytest==7.2.1 \
-    --hash=sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5 \
-    --hash=sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42
+pytest==7.3.1 \
+    --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
+    --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
     # via
     #   -r requirements/test.in
     #   pytest-mock
 pytest-mock==3.10.0 \
     --hash=sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b \
     --hash=sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f
     # via -r requirements/test.in
-responses==0.22.0 \
-    --hash=sha256:396acb2a13d25297789a5866b4881cf4e46ffd49cc26c43ab1117f40b973102e \
-    --hash=sha256:dcf294d204d14c436fddcc74caefdbc5764795a40ff4e6a7740ed8ddbf3294be
+responses==0.23.1 \
+    --hash=sha256:8a3a5915713483bf353b6f4079ba8b2a29029d1d1090a503c70b0dc5d9d0c7bd \
+    --hash=sha256:c4d9aa9fc888188f0c673eff79a8dadbe2e75b7fe879dc80a221a06e0a68138f
     # via -r requirements/test.in
-toml==0.10.2 \
-    --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
-    --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
-    # via responses
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   pyproject-api
     #   pytest
     #   tox
-tox==4.3.1 \
-    --hash=sha256:3b4c8bb7f281989b5ea2c39e862711ef2dbd15fedbf0c5f64e7c04c7d8cd8957 \
-    --hash=sha256:df2bf3c8329d1bc23a618329480ddefc0400af42804f801599b2ec38914f6309
+tox==4.5.1 \
+    --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
+    --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
     # via -r requirements/test.in
-types-toml==0.10.8.1 \
-    --hash=sha256:171bdb3163d79a520560f24ba916a9fc9bff81659c5448a9fea89240923722be \
-    --hash=sha256:b7b5c4977f96ab7b5ac06d8a6590d17c0bf252a96efc03b109c2711fb3e0eafd
+types-pyyaml==6.0.12.10 \
+    --hash=sha256:662fa444963eff9b68120d70cda1af5a5f2aa57900003c2006d7626450eaae5f \
+    --hash=sha256:ebab3d0700b946553724ae6ca636ea932c1b0868701d4af121630e78d695fc97
     # via responses
-typing-extensions==4.4.0 \
-    --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
-    --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
-    # via
-    #   importlib-metadata
-    #   platformdirs
-    #   responses
-    #   tox
-virtualenv==20.17.1 \
-    --hash=sha256:ce3b1684d6e1a20a3e5ed36795a97dfc6af29bc3970ca8dab93e11ac6094b3c4 \
-    --hash=sha256:f8b927684efc6f1cc206c9db297a570ab9ad0e51c16fa9e45487d36d1905c058
+virtualenv==20.23.0 \
+    --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
+    --hash=sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924
     # via tox
-zipp==3.11.0 \
-    --hash=sha256:83a28fcb75844b5c0cdaf5aa4003c2d728c77e05f5aeabe8e95e56727005fbaa \
-    --hash=sha256:a7a22e05929290a67401440b39690ae6563279bced5f314609d9d03798f56766
-    # via importlib-metadata
```

### Comparing `taskcluster-taskgraph-5.1.1/setup.py` & `taskcluster-taskgraph-5.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.1.1
+Version: 5.2.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Provides-Extra: load-image
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.2.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 src/taskgraph/run-task/run-task
 src/taskgraph/transforms/__init__.py
 src/taskgraph/transforms/base.py
 src/taskgraph/transforms/cached_tasks.py
 src/taskgraph/transforms/code_review.py
 src/taskgraph/transforms/docker_image.py
 src/taskgraph/transforms/fetch.py
+src/taskgraph/transforms/from_deps.py
 src/taskgraph/transforms/notify.py
 src/taskgraph/transforms/task.py
 src/taskgraph/transforms/job/__init__.py
 src/taskgraph/transforms/job/common.py
 src/taskgraph/transforms/job/index_search.py
 src/taskgraph/transforms/job/run_task.py
 src/taskgraph/transforms/job/toolchain.py
@@ -100,14 +101,15 @@
 test/test_scripts_fetch_content.py
 test/test_scripts_run_task.py
 test/test_target_tasks.py
 test/test_taskgraph.py
 test/test_transform_docker_image.py
 test/test_transforms_base.py
 test/test_transforms_fetch.py
+test/test_transforms_from_deps.py
 test/test_transforms_job.py
 test/test_transforms_job_run_task.py
 test/test_transforms_job_toolchain.py
 test/test_transforms_notify.py
 test/test_transforms_task.py
 test/test_util_attributes.py
 test/test_util_docker.py
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.1.1"
+__version__ = "5.2.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/config.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/create.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/main.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,40 +185,44 @@
 
     # Don't bother using futures if there's only one parameter. This can make
     # tracebacks a little more readable and avoids additional process overhead.
     if len(parameters) == 1:
         spec = parameters[0]
         out = format_taskgraph(options, spec, logfile(spec))
         dump_output(out, options["output_file"])
-        return
+        return 0
 
     futures = {}
     with ProcessPoolExecutor() as executor:
         for spec in parameters:
             f = executor.submit(format_taskgraph, options, spec, logfile(spec))
             futures[f] = spec
 
+    returncode = 0
     for future in as_completed(futures):
         output_file = options["output_file"]
         spec = futures[future]
         e = future.exception()
         if e:
+            returncode = 1
             out = "".join(traceback.format_exception(type(e), e, e.__traceback__))
             if options["diff"]:
                 # Dump to console so we don't accidentally diff the tracebacks.
                 output_file = None
         else:
             out = future.result()
 
         dump_output(
             out,
             path=output_file,
             params_spec=spec if len(parameters) > 1 else None,
         )
 
+    return returncode
+
 
 @command(
     "tasks",
     help="Show all tasks in the taskgraph.",
     defaults={"graph_attr": "full_task_set"},
 )
 @command(
@@ -405,15 +409,15 @@
             os.makedirs(logdir)
     else:
         # Only setup logging if we have a single parameter spec. Otherwise
         # logging will go to files. This is also used as a hook for Gecko
         # to setup its `mach` based logging.
         setup_logging()
 
-    generate_taskgraph(options, parameters, logdir)
+    ret = generate_taskgraph(options, parameters, logdir)
 
     if options["diff"]:
         assert diffdir is not None
         assert repo is not None
 
         # Reload taskgraph modules to pick up changes and clear global state.
         for mod in sys.modules.copy():
@@ -429,15 +433,15 @@
         try:
             repo.update(base_rev)
             base_rev = repo.head_rev[:12]
             options["output_file"] = os.path.join(
                 diffdir, f"{options['graph_attr']}_{base_rev_file}"
             )
             print(f"Generating {options['graph_attr']} @ {base_rev}", file=sys.stderr)
-            generate_taskgraph(options, parameters, logdir)
+            ret |= generate_taskgraph(options, parameters, logdir)
         finally:
             repo.update(cur_rev)
 
         # Generate diff(s)
         diffcmd = [
             "diff",
             "-U20",
@@ -489,14 +493,16 @@
                 'you should pass "-J"\n',
                 file=sys.stderr,
             )
 
     if len(parameters) > 1:
         print(f"See '{logdir}' for logs", file=sys.stderr)
 
+    return ret
+
 
 @command("build-image", help="Build a Docker image")
 @argument("image_name", help="Name of the image to build")
 @argument(
     "-t", "--tag", help="tag that the image should be built as.", metavar="name:tag"
 )
 @argument(
@@ -834,11 +840,11 @@
 
 
 def main(args=sys.argv[1:]):
     setup_logging()
     parser = create_parser()
     args = parser.parse_args(args)
     try:
-        args.command(vars(args))
+        return args.command(vars(args))
     except Exception:
         traceback.print_exc()
         sys.exit(1)
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.2.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/task.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/transforms/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1276,18 +1276,19 @@
     paths = {c["mount-point"] for c in task["worker"].get("caches", [])}
     missing = paths - volumes
 
     if not missing:
         return
 
     raise Exception(
-        "task %s (image %s) has caches that are not declared as "
-        "Docker volumes: %s "
-        "(have you added them as VOLUMEs in the Dockerfile?)"
-        % (task["label"], task["worker"]["docker-image"], ", ".join(sorted(missing)))
+        "task {} (image {}) has caches that are not declared as "
+        "Docker volumes: {} "
+        "(have you added them as VOLUMEs in the Dockerfile?)".format(
+            task["label"], task["worker"]["docker-image"], ", ".join(sorted(missing))
+        )
     )
 
 
 @transforms.add
 def check_run_task_caches(config, tasks):
     """Audit for caches requiring run-task.
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,38 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import re
 
 
 def attrmatch(attributes, **kwargs):
-    """Determine whether the given set of task attributes matches.  The
-    conditions are given as keyword arguments, where each keyword names an
-    attribute.  The keyword value can be a literal, a set, or a callable.  A
-    literal must match the attribute exactly.  Given a set, the attribute value
-    must be in the set.  A callable is called with the attribute value.  If an
-    attribute is specified as a keyword argument but not present in the
-    attributes, the result is False."""
+    """Determine whether the given set of task attributes matches.
+
+    The conditions are given as keyword arguments, where each keyword names an
+    attribute. The keyword value can be a literal, a set, or a callable:
+
+        * A literal must match the attribute exactly.
+        * Given a set or list, the attribute value must be contained within it.
+        * A callable is called with the attribute value and returns a boolean.
+
+    If an attribute is specified as a keyword argument but not present in the
+    task's attributes, the result is False.
+
+    Args:
+        attributes (dict): The task's attributes object.
+        kwargs (dict): The conditions the task's attributes must satisfy in
+                       order to match.
+    Returns:
+        bool: Whether the task's attributes match the conditions or not.
+    """
     for kwkey, kwval in kwargs.items():
         if kwkey not in attributes:
             return False
         attval = attributes[kwkey]
-        if isinstance(kwval, set):
+        if isinstance(kwval, (set, list)):
             if attval not in kwval:
                 return False
         elif callable(kwval):
             if not kwval(attval):
                 return False
         elif kwval != attributes[kwkey]:
             return False
```

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.2.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.2.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_actions_registry.py` & `taskcluster-taskgraph-5.2.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_create.py` & `taskcluster-taskgraph-5.2.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_decision.py` & `taskcluster-taskgraph-5.2.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_files_changed.py` & `taskcluster-taskgraph-5.2.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_generator.py` & `taskcluster-taskgraph-5.2.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_graph.py` & `taskcluster-taskgraph-5.2.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_main.py` & `taskcluster-taskgraph-5.2.0/test/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,18 @@
 
         def fake_get_taskgraph_generator(*args):
             return tgg
 
         monkeypatch.setattr(
             taskgraph.main, "get_taskgraph_generator", fake_get_taskgraph_generator
         )
-        taskgraph_main(args)
-        return tgg
+        try:
+            return taskgraph_main(args)
+        except SystemExit as e:
+            return e.code
 
     return inner
 
 
 @pytest.mark.parametrize(
     "attr,expected",
     (
@@ -43,19 +45,36 @@
         ("target", ["_fake-t-0", "_fake-t-1"]),
         ("target-graph", ["_fake-t-0", "_fake-t-1"]),
         ("optimized", ["_fake-t-0", "_fake-t-1"]),
         ("morphed", ["_fake-t-0", "_fake-t-1"]),
     ),
 )
 def test_show_taskgraph(run_show_taskgraph, capsys, attr, expected):
-    run_show_taskgraph([attr])
+    res = run_show_taskgraph([attr])
+    assert res == 0
+
     out, err = capsys.readouterr()
     assert out.strip() == "\n".join(expected)
     assert "Dumping result" in err
 
+    # Craft params to cause an exception
+    res = run_show_taskgraph(["full"], params={"_kinds": None})
+    assert res == 1
+
+
+def test_show_taskgraph_parallel(run_show_taskgraph):
+    res = run_show_taskgraph(["full", "-p", "taskcluster/test/params"])
+    assert res == 0
+
+    # Craft params to cause an exception
+    res = run_show_taskgraph(
+        ["full", "-p", "taskcluster/test/params"], params={"_kinds": None}
+    )
+    assert res == 1
+
 
 def test_tasks_regex(run_show_taskgraph, capsys):
     run_show_taskgraph(["full", "--tasks=_.*-t-1"])
     out, _ = capsys.readouterr()
     assert out.strip() == "_fake-t-1"
```

### Comparing `taskcluster-taskgraph-5.1.1/test/test_morph.py` & `taskcluster-taskgraph-5.2.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_optimize.py` & `taskcluster-taskgraph-5.2.0/test/test_optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     """
     Make a "triangle" graph like this:
 
       t1 <-------- t3
        `---- t2 --'
     """
     return make_graph(
-        make_task("t1", opts.get("t1")),
-        make_task("t2", opts.get("t2")),
-        make_task("t3", opts.get("t3")),
+        make_task("t1", optimization=opts.get("t1")),
+        make_task("t2", optimization=opts.get("t2")),
+        make_task("t3", optimization=opts.get("t3")),
         ("t3", "t2", "dep"),
         ("t3", "t1", "dep2"),
         ("t2", "t1", "dep"),
         deps=deps,
     )
 
 
@@ -107,16 +107,16 @@
             # expectations
             set(),
             id="composite_strategies_all",
         ),
         # Tasks with the 'not' composite strategy are removed when the substrategy says not to
         pytest.param(
             make_graph(
-                make_task("t1", {"not-never": None}),
-                make_task("t2", {"not-remove": None}),
+                make_task("t1", optimization={"not-never": None}),
+                make_task("t2", optimization={"not-remove": None}),
             ),
             {
                 "strategies": lambda: {
                     "not-never": Not("never"),
                     "not-remove": Not("remove"),
                 }
             },
@@ -146,84 +146,90 @@
             # expectations
             {"t3"},
             id="do_not_optimize",
         ),
         # Tasks with 'if_dependencies' are removed when deps are not run
         pytest.param(
             make_graph(
-                make_task("t1", {"remove": None}),
-                make_task("t2", {"remove": None}),
-                make_task("t3", {"never": None}, if_dependencies=["t1", "t2"]),
-                make_task("t4", {"never": None}, if_dependencies=["t1"]),
+                make_task("t1", optimization={"remove": None}),
+                make_task("t2", optimization={"remove": None}),
+                make_task(
+                    "t3", optimization={"never": None}, if_dependencies=["t1", "t2"]
+                ),
+                make_task("t4", optimization={"never": None}, if_dependencies=["t1"]),
                 ("t3", "t2", "dep"),
                 ("t3", "t1", "dep2"),
                 ("t2", "t1", "dep"),
                 ("t4", "t1", "dep3"),
             ),
             {"requested_tasks": {"t3", "t4"}},
             # expectations
             {"t1", "t2", "t3", "t4"},
             id="if_deps_removed",
         ),
         # Parents of tasks with 'if_dependencies' are also removed even if requested
         pytest.param(
             make_graph(
-                make_task("t1", {"remove": None}),
-                make_task("t2", {"remove": None}),
-                make_task("t3", {"never": None}, if_dependencies=["t1", "t2"]),
-                make_task("t4", {"never": None}, if_dependencies=["t1"]),
+                make_task("t1", optimization={"remove": None}),
+                make_task("t2", optimization={"remove": None}),
+                make_task(
+                    "t3", optimization={"never": None}, if_dependencies=["t1", "t2"]
+                ),
+                make_task("t4", optimization={"never": None}, if_dependencies=["t1"]),
                 ("t3", "t2", "dep"),
                 ("t3", "t1", "dep2"),
                 ("t2", "t1", "dep"),
                 ("t4", "t1", "dep3"),
             ),
             {},
             # expectations
             {"t1", "t2", "t3", "t4"},
             id="if_deps_parents_removed",
         ),
         # Tasks with 'if_dependencies' are kept if at least one of said dependencies are kept
         pytest.param(
             make_graph(
-                make_task("t1", {"never": None}),
-                make_task("t2", {"remove": None}),
-                make_task("t3", {"never": None}, if_dependencies=["t1", "t2"]),
-                make_task("t4", {"never": None}, if_dependencies=["t1"]),
+                make_task("t1", optimization={"never": None}),
+                make_task("t2", optimization={"remove": None}),
+                make_task(
+                    "t3", optimization={"never": None}, if_dependencies=["t1", "t2"]
+                ),
+                make_task("t4", optimization={"never": None}, if_dependencies=["t1"]),
                 ("t3", "t2", "dep"),
                 ("t3", "t1", "dep2"),
                 ("t2", "t1", "dep"),
                 ("t4", "t1", "dep3"),
             ),
             {},
             # expectations
             set(),
             id="if_deps_kept",
         ),
         # Ancestor of task with 'if_dependencies' does not cause it to be kept
         pytest.param(
             make_graph(
-                make_task("t1", {"never": None}),
-                make_task("t2", {"remove": None}),
-                make_task("t3", {"never": None}, if_dependencies=["t2"]),
+                make_task("t1", optimization={"never": None}),
+                make_task("t2", optimization={"remove": None}),
+                make_task("t3", optimization={"never": None}, if_dependencies=["t2"]),
                 ("t3", "t2", "dep"),
                 ("t2", "t1", "dep2"),
             ),
             {},
             # expectations
             {"t2", "t3"},
             id="if_deps_ancestor_does_not_keep",
         ),
         # Unhandled edge case where 't1' and 't2' are kept even though they
         # don't have any dependents and are not in 'requested_tasks'
         pytest.param(
             make_graph(
-                make_task("t1", {"never": None}),
-                make_task("t2", {"never": None}, if_dependencies=["t1"]),
-                make_task("t3", {"remove": None}),
-                make_task("t4", {"never": None}, if_dependencies=["t3"]),
+                make_task("t1", optimization={"never": None}),
+                make_task("t2", optimization={"never": None}, if_dependencies=["t1"]),
+                make_task("t3", optimization={"remove": None}),
+                make_task("t4", optimization={"never": None}, if_dependencies=["t3"]),
                 ("t2", "t1", "e1"),
                 ("t4", "t2", "e2"),
                 ("t4", "t3", "e3"),
             ),
             {"requested_tasks": {"t3", "t4"}},
             # expectations
             {"t1", "t2", "t3", "t4"},
@@ -329,15 +335,15 @@
             {"t2", "t3"},
             {"t1": "e1"},
             id="tasks_removed",
         ),
         # A task which expires before a dependents deadline is not a valid replacement.
         pytest.param(
             make_graph(
-                make_task("t1", {"replace": "e1"}),
+                make_task("t1", optimization={"replace": "e1"}),
                 make_task(
                     "t2", task_def={"deadline": {"relative-datestamp": "2 days"}}
                 ),
                 make_task(
                     "t3", task_def={"deadline": {"relative-datestamp": "1 minute"}}
                 ),
                 ("t2", "t1", "dep1"),
```

### Comparing `taskcluster-taskgraph-5.1.1/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.2.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_parameters.py` & `taskcluster-taskgraph-5.2.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.2.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.2.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_target_tasks.py` & `taskcluster-taskgraph-5.2.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_taskgraph.py` & `taskcluster-taskgraph-5.2.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.2.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_base.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_job.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_transforms_task.py` & `taskcluster-taskgraph-5.2.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_attributes.py` & `taskcluster-taskgraph-5.2.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_docker.py` & `taskcluster-taskgraph-5.2.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_memoize.py` & `taskcluster-taskgraph-5.2.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.2.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_path.py` & `taskcluster-taskgraph-5.2.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_python_path.py` & `taskcluster-taskgraph-5.2.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.2.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_schema.py` & `taskcluster-taskgraph-5.2.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.2.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_templates.py` & `taskcluster-taskgraph-5.2.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_time.py` & `taskcluster-taskgraph-5.2.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.2.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_vcs.py` & `taskcluster-taskgraph-5.2.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_verify.py` & `taskcluster-taskgraph-5.2.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.2.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.1.1/test/test_util_yaml.py` & `taskcluster-taskgraph-5.2.0/test/test_util_yaml.py`

 * *Files identical despite different names*


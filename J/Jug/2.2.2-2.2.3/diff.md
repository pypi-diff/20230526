# Comparing `tmp/Jug-2.2.2.tar.gz` & `tmp/Jug-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jug-2.2.2.tar", last modified: Mon Jul 18 23:09:23 2022, max compression
+gzip compressed data, was "Jug-2.2.3.tar", last modified: Fri May 26 11:38:17 2023, max compression
```

## Comparing `Jug-2.2.2.tar` & `Jug-2.2.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.745180 Jug-2.2.2/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1087 2020-10-10 13:38:46.000000 Jug-2.2.2/COPYING.MIT
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.729179 Jug-2.2.2/Jug.egg-info/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7471 2022-07-18 23:09:23.000000 Jug-2.2.2/Jug.egg-info/PKG-INFO
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2788 2022-07-18 23:09:23.000000 Jug-2.2.2/Jug.egg-info/SOURCES.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        1 2022-07-18 23:09:23.000000 Jug-2.2.2/Jug.egg-info/dependency_links.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       38 2022-07-18 23:09:23.000000 Jug-2.2.2/Jug.egg-info/entry_points.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        4 2022-07-18 23:09:23.000000 Jug-2.2.2/Jug.egg-info/top_level.txt
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2021-03-18 04:18:20.000000 Jug-2.2.2/MANIFEST.in
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     7471 2022-07-18 23:09:23.745180 Jug-2.2.2/PKG-INFO
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6415 2022-07-18 23:09:16.000000 Jug-2.2.2/README.rst
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.729179 Jug-2.2.2/bin/
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)      182 2022-04-28 11:10:27.000000 Jug-2.2.2/bin/jug-execute
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.729179 Jug-2.2.2/jug/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2178 2017-01-12 09:06:55.000000 Jug-2.2.2/jug/__init__.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.733179 Jug-2.2.2/jug/backends/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1279 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/backends/__init__.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6760 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/backends/base.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6857 2022-05-19 20:42:40.000000 Jug-2.2.2/jug/backends/dict_store.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6225 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/backends/encode.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2508 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/backends/file_keepalive_monitor.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    18350 2022-07-18 23:06:59.000000 Jug-2.2.2/jug/backends/file_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4863 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/backends/memoize_store.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6093 2022-05-19 20:42:40.000000 Jug-2.2.2/jug/backends/redis_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2140 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/backends/select.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5153 2020-06-11 19:25:43.000000 Jug-2.2.2/jug/barrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3204 2017-05-21 08:34:10.000000 Jug-2.2.2/jug/compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3493 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/hash.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.733179 Jug-2.2.2/jug/hooks/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2016-03-05 23:58:02.000000 Jug-2.2.2/jug/hooks/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1156 2020-10-28 22:12:26.000000 Jug-2.2.2/jug/hooks/execution.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3950 2020-09-25 14:40:43.000000 Jug-2.2.2/jug/hooks/exit_checks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2374 2016-10-16 21:10:32.000000 Jug-2.2.2/jug/hooks/register.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.733179 Jug-2.2.2/jug/internal/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2020-06-11 19:25:43.000000 Jug-2.2.2/jug/internal/__init__.py
--rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     2748 2020-06-11 19:25:43.000000 Jug-2.2.2/jug/internal/debugger.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7483 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/io.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10352 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/jug.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)      218 2022-07-18 23:07:03.000000 Jug-2.2.2/jug/jug_version.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7881 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10469 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/options.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.737179 Jug-2.2.2/jug/subcommands/
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    11604 2021-05-31 13:02:23.000000 Jug-2.2.2/jug/subcommands/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2974 2020-01-31 13:24:44.000000 Jug-2.2.2/jug/subcommands/check.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3309 2020-12-16 03:43:22.000000 Jug-2.2.2/jug/subcommands/cleanup.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1864 2017-05-19 19:02:51.000000 Jug-2.2.2/jug/subcommands/count.py
--rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     3057 2017-07-14 23:30:06.000000 Jug-2.2.2/jug/subcommands/demo.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6180 2020-10-28 22:12:46.000000 Jug-2.2.2/jug/subcommands/execute.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5451 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/subcommands/graph.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2072 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/subcommands/internal_validation.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3285 2017-05-19 19:02:51.000000 Jug-2.2.2/jug/subcommands/invalidate.py
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     2014 2022-01-06 01:22:59.000000 Jug-2.2.2/jug/subcommands/pack.py
--rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     6368 2022-07-18 23:09:16.000000 Jug-2.2.2/jug/subcommands/shell.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10506 2022-05-02 20:30:18.000000 Jug-2.2.2/jug/subcommands/status.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4839 2022-05-02 20:33:19.000000 Jug-2.2.2/jug/subcommands/webstatus.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)    19139 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/task.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.741180 Jug-2.2.2/jug/tests/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      158 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/__init__.py
-drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2022-07-18 23:09:23.745180 Jug-2.2.2/jug/tests/jugfiles/
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2014-01-24 15:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/__init__.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      471 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/barrier_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      192 2018-04-13 18:55:39.000000 Jug-2.2.2/jug/tests/jugfiles/barrier_recurse.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      341 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/jugfiles/block_access.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      108 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/builtin_function.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      134 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/bvalue.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      337 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      380 2014-01-24 15:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/compound_nonsimple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      280 2019-08-11 14:57:49.000000 Jug-2.2.2/jug/tests/jugfiles/compound_wbarrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      277 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/custom_hash_function.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      141 2014-01-24 15:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/empty_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       65 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/tests/jugfiles/exceptions.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      498 2019-08-11 14:59:21.000000 Jug-2.2.2/jug/tests/jugfiles/failing.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      226 2020-01-31 13:24:44.000000 Jug-2.2.2/jug/tests/jugfiles/iteratetask.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      244 2018-04-13 19:35:09.000000 Jug-2.2.2/jug/tests/jugfiles/mapgenerator.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2018-04-07 13:03:52.000000 Jug-2.2.2/jug/tests/jugfiles/mapreduce_generator.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      394 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/jugfiles/no_load.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      327 2020-06-11 19:49:14.000000 Jug-2.2.2/jug/tests/jugfiles/run-simple-create-file.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      329 2017-08-29 16:56:39.000000 Jug-2.2.2/jug/tests/jugfiles/simple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      312 2017-05-19 19:02:51.000000 Jug-2.2.2/jug/tests/jugfiles/simple_multiple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/sleep_until_tasklet.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      348 2016-12-29 09:23:55.000000 Jug-2.2.2/jug/tests/jugfiles/slice_task.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      117 2016-03-04 01:41:49.000000 Jug-2.2.2/jug/tests/jugfiles/tasklet_simple.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      268 2014-01-24 15:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/tasklets.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      372 2014-01-24 15:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/wbarrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      331 2016-03-04 01:42:10.000000 Jug-2.2.2/jug/tests/jugfiles/write_with_meta.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      482 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/task_reset.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2010 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_barrier.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2376 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_compound.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1557 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/tests/test_encode.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     2245 2022-07-18 23:06:59.000000 Jug-2.2.2/jug/tests/test_file_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      809 2016-12-29 00:15:41.000000 Jug-2.2.2/jug/tests/test_hash.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1558 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_hooks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1125 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_io.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1666 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_jug_check.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4784 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_jug_execute.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3482 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_jug_invalidate.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3139 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_lock.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2835 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_mapreduce.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      382 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_no_load.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2059 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/tests/test_options.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1886 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_status.py
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     4622 2022-05-19 20:42:40.000000 Jug-2.2.2/jug/tests/test_store.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3503 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/tests/test_subcommand_api.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1158 2021-03-21 03:34:18.000000 Jug-2.2.2/jug/tests/test_sys_argv.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1341 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_tasklet.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6747 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_tasks.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      476 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_utils_customhash.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      154 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_utils_identity.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      742 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/test_utils_timed_path.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      464 2022-05-02 20:33:48.000000 Jug-2.2.2/jug/tests/test_webstatus.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)      649 2020-10-10 13:38:46.000000 Jug-2.2.2/jug/tests/utils.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7531 2020-10-28 22:12:52.000000 Jug-2.2.2/jug/utils.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2021-03-21 03:34:18.000000 Jug-2.2.2/requirements.txt
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)       38 2022-07-18 23:09:23.745180 Jug-2.2.2/setup.cfg
--rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3000 2022-04-28 11:10:43.000000 Jug-2.2.2/setup.py
--rw-r--r--   0 luispedro  (1000) luispedro  (1000)       19 2021-03-18 04:18:20.000000 Jug-2.2.2/test-requirements.txt
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.338914 Jug-2.2.3/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1087 2020-10-10 13:38:46.000000 Jug-2.2.3/COPYING.MIT
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/Jug.egg-info/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7550 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/PKG-INFO
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2788 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/SOURCES.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        1 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/dependency_links.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       37 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/entry_points.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        4 2023-05-26 11:38:17.000000 Jug-2.2.3/Jug.egg-info/top_level.txt
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2021-03-18 04:18:20.000000 Jug-2.2.3/MANIFEST.in
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     7550 2023-05-26 11:38:17.338914 Jug-2.2.3/PKG-INFO
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6496 2023-05-26 11:36:42.000000 Jug-2.2.3/README.rst
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/bin/
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)      182 2022-04-28 11:10:27.000000 Jug-2.2.3/bin/jug-execute
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.326914 Jug-2.2.3/jug/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2178 2017-01-12 09:06:55.000000 Jug-2.2.3/jug/__init__.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/backends/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1279 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/backends/__init__.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6760 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/backends/base.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6857 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/backends/dict_store.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6225 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/backends/encode.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2508 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/file_keepalive_monitor.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    18350 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/backends/file_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4863 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/memoize_store.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     6093 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/backends/redis_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2140 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/backends/select.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5153 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/barrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3204 2017-05-21 08:34:10.000000 Jug-2.2.3/jug/compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3493 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/hash.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/hooks/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2016-03-05 23:58:02.000000 Jug-2.2.3/jug/hooks/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1156 2020-10-28 22:12:26.000000 Jug-2.2.3/jug/hooks/execution.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3950 2020-09-25 14:40:43.000000 Jug-2.2.3/jug/hooks/exit_checks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2374 2016-10-16 21:10:32.000000 Jug-2.2.3/jug/hooks/register.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/internal/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/internal/__init__.py
+-rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     2748 2020-06-11 19:25:43.000000 Jug-2.2.3/jug/internal/debugger.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7483 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/io.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10352 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/jug.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)      218 2023-05-26 11:36:16.000000 Jug-2.2.3/jug/jug_version.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7881 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/mapreduce.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    10469 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/options.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.330914 Jug-2.2.3/jug/subcommands/
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)    11604 2021-05-31 13:02:23.000000 Jug-2.2.3/jug/subcommands/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2974 2020-01-31 13:24:44.000000 Jug-2.2.3/jug/subcommands/check.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3309 2020-12-16 03:43:22.000000 Jug-2.2.3/jug/subcommands/cleanup.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1864 2017-05-19 19:02:51.000000 Jug-2.2.3/jug/subcommands/count.py
+-rwxr-xr-x   0 luispedro  (1000) luispedro  (1000)     3057 2017-07-14 23:30:06.000000 Jug-2.2.3/jug/subcommands/demo.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6180 2020-10-28 22:12:46.000000 Jug-2.2.3/jug/subcommands/execute.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     5451 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/subcommands/graph.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2072 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/subcommands/internal_validation.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3285 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/subcommands/invalidate.py
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     2014 2022-01-06 01:22:59.000000 Jug-2.2.3/jug/subcommands/pack.py
+-rwxrwxr-x   0 luispedro  (1000) luispedro  (1000)     6099 2023-05-26 11:33:24.000000 Jug-2.2.3/jug/subcommands/shell.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    10506 2022-05-02 20:30:18.000000 Jug-2.2.3/jug/subcommands/status.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4839 2022-05-02 20:33:19.000000 Jug-2.2.3/jug/subcommands/webstatus.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)    19139 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/task.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.334914 Jug-2.2.3/jug/tests/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      158 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/__init__.py
+drwxrwxr-x   0 luispedro  (1000) luispedro  (1000)        0 2023-05-26 11:38:17.338914 Jug-2.2.3/jug/tests/jugfiles/
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/__init__.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      471 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/barrier_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      192 2018-04-13 18:55:39.000000 Jug-2.2.3/jug/tests/jugfiles/barrier_recurse.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      341 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/jugfiles/block_access.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      108 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/builtin_function.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      134 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/bvalue.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      337 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      380 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/compound_nonsimple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      280 2019-08-11 14:57:49.000000 Jug-2.2.3/jug/tests/jugfiles/compound_wbarrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      277 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/custom_hash_function.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      141 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/empty_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       65 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/tests/jugfiles/exceptions.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      498 2019-08-11 14:59:21.000000 Jug-2.2.3/jug/tests/jugfiles/failing.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      226 2020-01-31 13:24:44.000000 Jug-2.2.3/jug/tests/jugfiles/iteratetask.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      244 2018-04-13 19:35:09.000000 Jug-2.2.3/jug/tests/jugfiles/mapgenerator.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      210 2018-04-07 13:03:52.000000 Jug-2.2.3/jug/tests/jugfiles/mapreduce_generator.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      394 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/jugfiles/no_load.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      327 2020-06-11 19:49:14.000000 Jug-2.2.3/jug/tests/jugfiles/run-simple-create-file.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      329 2017-08-29 16:56:39.000000 Jug-2.2.3/jug/tests/jugfiles/simple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      312 2017-05-19 19:02:51.000000 Jug-2.2.3/jug/tests/jugfiles/simple_multiple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      150 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/sleep_until_tasklet.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      348 2016-12-29 09:23:55.000000 Jug-2.2.3/jug/tests/jugfiles/slice_task.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      117 2016-03-04 01:41:49.000000 Jug-2.2.3/jug/tests/jugfiles/tasklet_simple.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      268 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/tasklets.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      372 2014-01-24 15:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/wbarrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      331 2016-03-04 01:42:10.000000 Jug-2.2.3/jug/tests/jugfiles/write_with_meta.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      482 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/task_reset.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2010 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_barrier.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2376 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_compound.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1557 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_encode.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     2245 2022-07-18 23:06:59.000000 Jug-2.2.3/jug/tests/test_file_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      809 2016-12-29 00:15:41.000000 Jug-2.2.3/jug/tests/test_hash.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1558 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_hooks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1125 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_io.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1666 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_check.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     4784 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_execute.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3482 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_jug_invalidate.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3139 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_lock.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2835 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_mapreduce.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      382 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_no_load.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     2059 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_options.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1886 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_status.py
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     4622 2022-05-19 20:42:40.000000 Jug-2.2.3/jug/tests/test_store.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     3503 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_subcommand_api.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1158 2021-03-21 03:34:18.000000 Jug-2.2.3/jug/tests/test_sys_argv.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     1341 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_tasklet.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     6747 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_tasks.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      476 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_customhash.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      154 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_identity.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      742 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/test_utils_timed_path.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      464 2022-05-02 20:33:48.000000 Jug-2.2.3/jug/tests/test_webstatus.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)      649 2020-10-10 13:38:46.000000 Jug-2.2.3/jug/tests/utils.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)     7531 2020-10-28 22:12:52.000000 Jug-2.2.3/jug/utils.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)        0 2021-03-21 03:34:18.000000 Jug-2.2.3/requirements.txt
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)       38 2023-05-26 11:38:17.338914 Jug-2.2.3/setup.cfg
+-rw-rw-r--   0 luispedro  (1000) luispedro  (1000)     3000 2022-04-28 11:10:43.000000 Jug-2.2.3/setup.py
+-rw-r--r--   0 luispedro  (1000) luispedro  (1000)       19 2021-03-18 04:18:20.000000 Jug-2.2.3/test-requirements.txt
```

### Comparing `Jug-2.2.2/COPYING.MIT` & `Jug-2.2.3/COPYING.MIT`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/Jug.egg-info/PKG-INFO` & `Jug-2.2.3/Jug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jug
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Task Based Parallelization Framework
 Home-page: https://jug.readthedocs.io
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
@@ -154,14 +154,17 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.2.3 (*26 May 2023*)
+- Fix ``jug shell`` for newer versions of IPython
+
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
 - Fix bug with ``jug cleanup`` and the redis backend (`#86 <https://github.com/luispedro/jug/issues/86>`__)
 
 Version 2.2.0 (*3 May 2022*)
@@ -206,9 +209,7 @@
 
 For older version see ``ChangeLog`` file or the `full history
 <https://jug.readthedocs.io/en/latest/history.html>`__.
 
 
 
 
-
-
```

### Comparing `Jug-2.2.2/Jug.egg-info/SOURCES.txt` & `Jug-2.2.3/Jug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/PKG-INFO` & `Jug-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jug
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Task Based Parallelization Framework
 Home-page: https://jug.readthedocs.io
 Author: Luis Pedro Coelho
 Author-email: luis@luispedro.org
 License: MIT
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
@@ -154,14 +154,17 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.2.3 (*26 May 2023*)
+- Fix ``jug shell`` for newer versions of IPython
+
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
 - Fix bug with ``jug cleanup`` and the redis backend (`#86 <https://github.com/luispedro/jug/issues/86>`__)
 
 Version 2.2.0 (*3 May 2022*)
@@ -206,9 +209,7 @@
 
 For older version see ``ChangeLog`` file or the `full history
 <https://jug.readthedocs.io/en/latest/history.html>`__.
 
 
 
 
-
-
```

### Comparing `Jug-2.2.2/README.rst` & `Jug-2.2.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,17 @@
 
     In [2]: primes100[:10]
     Out[2]: [True, True, False, True, False, True, False, False, False, True]
 
 What's New
 ----------
 
+Version 2.2.3 (*26 May 2023*)
+- Fix ``jug shell`` for newer versions of IPython
+
 Version 2.2.2 (*19 July 2022*)
 - Fix ``jug cleanup`` when packs are used (``jug pack``)
 
 Version 2.2.1 (*19 May 2022*)
 - Fix bug with ``jug cleanup`` and the redis backend (`#86 <https://github.com/luispedro/jug/issues/86>`__)
 
 Version 2.2.0 (*3 May 2022*)
```

### Comparing `Jug-2.2.2/jug/__init__.py` & `Jug-2.2.3/jug/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/__init__.py` & `Jug-2.2.3/jug/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/base.py` & `Jug-2.2.3/jug/backends/base.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/dict_store.py` & `Jug-2.2.3/jug/backends/dict_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/encode.py` & `Jug-2.2.3/jug/backends/encode.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/file_keepalive_monitor.py` & `Jug-2.2.3/jug/backends/file_keepalive_monitor.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/file_store.py` & `Jug-2.2.3/jug/backends/file_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/memoize_store.py` & `Jug-2.2.3/jug/backends/memoize_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/redis_store.py` & `Jug-2.2.3/jug/backends/redis_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/backends/select.py` & `Jug-2.2.3/jug/backends/select.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/barrier.py` & `Jug-2.2.3/jug/barrier.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/compound.py` & `Jug-2.2.3/jug/compound.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/hash.py` & `Jug-2.2.3/jug/hash.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/hooks/execution.py` & `Jug-2.2.3/jug/hooks/execution.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/hooks/exit_checks.py` & `Jug-2.2.3/jug/hooks/exit_checks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/hooks/register.py` & `Jug-2.2.3/jug/hooks/register.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/internal/debugger.py` & `Jug-2.2.3/jug/internal/debugger.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/io.py` & `Jug-2.2.3/jug/io.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/jug.py` & `Jug-2.2.3/jug/jug.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/mapreduce.py` & `Jug-2.2.3/jug/mapreduce.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/options.py` & `Jug-2.2.3/jug/options.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/__init__.py` & `Jug-2.2.3/jug/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/check.py` & `Jug-2.2.3/jug/subcommands/check.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/cleanup.py` & `Jug-2.2.3/jug/subcommands/cleanup.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/count.py` & `Jug-2.2.3/jug/subcommands/count.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/demo.py` & `Jug-2.2.3/jug/subcommands/demo.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/execute.py` & `Jug-2.2.3/jug/subcommands/execute.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/graph.py` & `Jug-2.2.3/jug/subcommands/graph.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/internal_validation.py` & `Jug-2.2.3/jug/subcommands/internal_validation.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/invalidate.py` & `Jug-2.2.3/jug/subcommands/invalidate.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/pack.py` & `Jug-2.2.3/jug/subcommands/pack.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/shell.py` & `Jug-2.2.3/jug/subcommands/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-# Copyright (C) 2008-2021, Luis Pedro Coelho <luis@luispedro.org>
+# Copyright (C) 2008-2023, Luis Pedro Coelho <luis@luispedro.org>
 # vim: set ts=4 sts=4 sw=4 expandtab smartindent:
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
@@ -91,31 +91,25 @@
     Currently depends on Ipython being installed.
     '''
     name = "shell"
 
     def run(self, store, options, jugspace, *args, **kwargs):
         try:
             import IPython
-            if IPython.version_info[0] >= 1:
-                from IPython.terminal.embed import InteractiveShellEmbed
-                from IPython.terminal.ipapp import load_default_config
-            else:
-                from IPython.frontend.terminal.embed import InteractiveShellEmbed
-                from IPython.frontend.terminal.ipapp import load_default_config
+            from IPython.terminal.embed import InteractiveShellEmbed
+            from IPython.terminal.ipapp import load_default_config
             config = load_default_config()
-            ipshell = InteractiveShellEmbed(config=config, display_banner=_ipython_banner)
+            if IPython.core.getipython.get_ipython() is None:
+                ipshell = InteractiveShellEmbed.instance(config=config, display_banner=_ipython_banner)
+            else:
+                ipshell = InteractiveShellEmbed(config=config, display_banner=_ipython_banner)
         except ImportError:
-            try:
-                # Fallback for older Python:
-                from IPython.Shell import IPShellEmbed
-                ipshell = IPShellEmbed(banner=_ipython_banner)
-            except ImportError:
-                import sys
-                sys.stderr.write(_ipython_not_found_msg)
-                sys.exit(1)
+            import sys
+            sys.stderr.write(_ipython_not_found_msg)
+            sys.exit(1)
 
         def _load_all():
             '''
             load_all()
 
             Loads all task results.
             '''
```

### Comparing `Jug-2.2.2/jug/subcommands/status.py` & `Jug-2.2.3/jug/subcommands/status.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/subcommands/webstatus.py` & `Jug-2.2.3/jug/subcommands/webstatus.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/task.py` & `Jug-2.2.3/jug/task.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_barrier.py` & `Jug-2.2.3/jug/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_compound.py` & `Jug-2.2.3/jug/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_encode.py` & `Jug-2.2.3/jug/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_file_store.py` & `Jug-2.2.3/jug/tests/test_file_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_hash.py` & `Jug-2.2.3/jug/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_hooks.py` & `Jug-2.2.3/jug/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_io.py` & `Jug-2.2.3/jug/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_jug_check.py` & `Jug-2.2.3/jug/tests/test_jug_check.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_jug_execute.py` & `Jug-2.2.3/jug/tests/test_jug_execute.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_jug_invalidate.py` & `Jug-2.2.3/jug/tests/test_jug_invalidate.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_lock.py` & `Jug-2.2.3/jug/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_mapreduce.py` & `Jug-2.2.3/jug/tests/test_mapreduce.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_options.py` & `Jug-2.2.3/jug/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_status.py` & `Jug-2.2.3/jug/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_store.py` & `Jug-2.2.3/jug/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_subcommand_api.py` & `Jug-2.2.3/jug/tests/test_subcommand_api.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_sys_argv.py` & `Jug-2.2.3/jug/tests/test_sys_argv.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_tasklet.py` & `Jug-2.2.3/jug/tests/test_tasklet.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_tasks.py` & `Jug-2.2.3/jug/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/test_utils_timed_path.py` & `Jug-2.2.3/jug/tests/test_utils_timed_path.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/tests/utils.py` & `Jug-2.2.3/jug/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/jug/utils.py` & `Jug-2.2.3/jug/utils.py`

 * *Files identical despite different names*

### Comparing `Jug-2.2.2/setup.py` & `Jug-2.2.3/setup.py`

 * *Files identical despite different names*


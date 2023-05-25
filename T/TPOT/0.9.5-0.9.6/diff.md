# Comparing `tmp/TPOT-0.9.5.tar.gz` & `tmp/TPOT-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TPOT-0.9.5.tar", last modified: Fri Aug 31 04:43:46 2018, max compression
+gzip compressed data, was "dist/TPOT-0.9.6.tar", last modified: Fri Mar  1 18:00:14 2019, max compression
```

## Comparing `TPOT-0.9.5.tar` & `TPOT-0.9.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1344 2018-08-31 04:43:46.000000 TPOT-0.9.5/PKG-INFO
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/tpot/
--rw-r--r--   0 weixuanfu   (501) staff       (20)     2459 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/metrics.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    11791 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/export_utils.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)      946 2018-08-31 04:38:29.000000 TPOT-0.9.5/tpot/_version.py
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/tpot/config/
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3726 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/config/classifier_sparse.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3341 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/config/classifier_light.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     6196 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/config/classifier.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1737 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/config/regressor_mdr.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3059 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/config/regressor_sparse.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1360 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/config/__init__.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1756 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/config/classifier_mdr.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3611 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/config/regressor_light.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     5792 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/config/regressor.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1031 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/__init__.py
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/tpot/builtins/
--rw-r--r--   0 weixuanfu   (501) staff       (20)     5706 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/builtins/feature_transformers.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     2215 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/builtins/zero_count.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1216 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/builtins/__init__.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3303 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/builtins/stacking_estimator.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1121 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/builtins/combine_dfs.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    18753 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/builtins/one_hot_encoder.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1609 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/tpot.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     9764 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/operator_utils.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1003 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/gp_types.py
--rwxr-xr-x   0 weixuanfu   (501) staff       (20)    17295 2018-08-31 04:38:21.000000 TPOT-0.9.5/tpot/driver.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    72400 2018-08-31 04:38:29.000000 TPOT-0.9.5/tpot/base.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    20597 2018-08-31 04:38:29.000000 TPOT-0.9.5/tpot/gp_deap.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     3784 2018-01-17 18:46:22.000000 TPOT-0.9.5/tpot/decorators.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     7651 2018-01-17 18:46:22.000000 TPOT-0.9.5/LICENSE
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/images/
--rw-r--r--   0 weixuanfu   (501) staff       (20)   223359 2018-01-17 18:46:22.000000 TPOT-0.9.5/images/tpot-ml-pipeline.png
--rw-r--r--   0 weixuanfu   (501) staff       (20)   286325 2018-01-17 18:46:22.000000 TPOT-0.9.5/images/tpot-demo.gif
--rw-r--r--   0 weixuanfu   (501) staff       (20)   204264 2018-01-17 18:46:22.000000 TPOT-0.9.5/images/tpot-pipeline-example.png
--rw-r--r--   0 weixuanfu   (501) staff       (20)   181208 2018-01-17 18:46:22.000000 TPOT-0.9.5/images/tpot-logo.jpg
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/TPOT.egg-info/
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1344 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/PKG-INFO
--rw-r--r--   0 weixuanfu   (501) staff       (20)        1 2018-01-17 18:48:54.000000 TPOT-0.9.5/TPOT.egg-info/zip-safe
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1274 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/SOURCES.txt
--rw-r--r--   0 weixuanfu   (501) staff       (20)       36 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/entry_points.txt
--rw-r--r--   0 weixuanfu   (501) staff       (20)      257 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/requires.txt
--rw-r--r--   0 weixuanfu   (501) staff       (20)        5 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/top_level.txt
--rw-r--r--   0 weixuanfu   (501) staff       (20)        1 2018-08-31 04:43:45.000000 TPOT-0.9.5/TPOT.egg-info/dependency_links.txt
-drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2018-08-31 04:43:46.000000 TPOT-0.9.5/tests/
--rw-r--r--   0 weixuanfu   (501) staff       (20)    12460 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/driver_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    12412 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/one_hot_encoder_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    81680 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/tpot_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1442 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/test_dask_based.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1422 2018-01-17 18:46:22.000000 TPOT-0.9.5/tests/test_config_sparse.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    24191 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/export_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1587 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/zero_count_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)    21188 2018-01-17 18:46:22.000000 TPOT-0.9.5/tests/tests.csv
--rw-r--r--   0 weixuanfu   (501) staff       (20)     1262 2018-01-17 18:46:22.000000 TPOT-0.9.5/tests/test_config.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     4926 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/stats_test.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     2511 2018-08-31 04:38:21.000000 TPOT-0.9.5/tests/feature_transformers_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)     4622 2018-01-17 18:46:22.000000 TPOT-0.9.5/tests/stacking_estimator_tests.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)      116 2018-01-17 18:46:22.000000 TPOT-0.9.5/MANIFEST.in
--rw-r--r--   0 weixuanfu   (501) staff       (20)    10917 2018-08-31 04:38:21.000000 TPOT-0.9.5/README.md
--rw-r--r--   0 weixuanfu   (501) staff       (20)     2310 2018-08-31 04:38:21.000000 TPOT-0.9.5/setup.py
--rw-r--r--   0 weixuanfu   (501) staff       (20)       59 2018-08-31 04:43:46.000000 TPOT-0.9.5/setup.cfg
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:14.000000 TPOT-0.9.6/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1434 2019-03-01 18:00:14.000000 TPOT-0.9.6/PKG-INFO
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:13.000000 TPOT-0.9.6/tpot/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     2459 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/metrics.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    11791 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/export_utils.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)      946 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/_version.py
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:14.000000 TPOT-0.9.6/tpot/config/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3726 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/config/classifier_sparse.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3341 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/config/classifier_light.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     6196 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/config/classifier.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1737 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/config/regressor_mdr.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3059 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/config/regressor_sparse.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1360 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/config/__init__.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1756 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/config/classifier_mdr.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3611 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/config/regressor_light.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     5757 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/config/regressor.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1031 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/__init__.py
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:13.000000 TPOT-0.9.6/tpot/builtins/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     5696 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/builtins/feature_transformers.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     2215 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/builtins/zero_count.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1216 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/builtins/__init__.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3303 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/builtins/stacking_estimator.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1121 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/builtins/combine_dfs.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    18753 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/builtins/one_hot_encoder.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1609 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/tpot.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    10412 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/operator_utils.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1003 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/gp_types.py
+-rwxr-xr-x   0 weixuanfu   (501) staff       (20)    17295 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/driver.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    75015 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/base.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    20385 2019-03-01 17:58:10.000000 TPOT-0.9.6/tpot/gp_deap.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     3784 2018-01-02 16:27:50.000000 TPOT-0.9.6/tpot/decorators.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     7651 2018-01-02 16:27:50.000000 TPOT-0.9.6/LICENSE
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:13.000000 TPOT-0.9.6/images/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)   223359 2018-01-02 16:27:50.000000 TPOT-0.9.6/images/tpot-ml-pipeline.png
+-rw-r--r--   0 weixuanfu   (501) staff       (20)   286325 2018-01-02 16:27:50.000000 TPOT-0.9.6/images/tpot-demo.gif
+-rw-r--r--   0 weixuanfu   (501) staff       (20)   204264 2018-01-02 16:27:50.000000 TPOT-0.9.6/images/tpot-pipeline-example.png
+-rw-r--r--   0 weixuanfu   (501) staff       (20)   181208 2018-01-02 16:27:50.000000 TPOT-0.9.6/images/tpot-logo.jpg
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1434 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/PKG-INFO
+-rw-r--r--   0 weixuanfu   (501) staff       (20)        1 2019-03-01 17:59:08.000000 TPOT-0.9.6/TPOT.egg-info/zip-safe
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1274 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/SOURCES.txt
+-rw-r--r--   0 weixuanfu   (501) staff       (20)       36 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/entry_points.txt
+-rw-r--r--   0 weixuanfu   (501) staff       (20)      257 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/requires.txt
+-rw-r--r--   0 weixuanfu   (501) staff       (20)        5 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/top_level.txt
+-rw-r--r--   0 weixuanfu   (501) staff       (20)        1 2019-03-01 18:00:13.000000 TPOT-0.9.6/TPOT.egg-info/dependency_links.txt
+drwxr-xr-x   0 weixuanfu   (501) staff       (20)        0 2019-03-01 18:00:13.000000 TPOT-0.9.6/tests/
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    12460 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/driver_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    12412 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/one_hot_encoder_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    82897 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/tpot_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1444 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/test_dask_based.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1422 2018-01-02 16:27:50.000000 TPOT-0.9.6/tests/test_config_sparse.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    24191 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/export_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1587 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/zero_count_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    21188 2018-01-02 16:27:50.000000 TPOT-0.9.6/tests/tests.csv
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     1262 2018-01-02 16:27:50.000000 TPOT-0.9.6/tests/test_config.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     4926 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/stats_test.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     2511 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/feature_transformers_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     4679 2019-03-01 17:58:10.000000 TPOT-0.9.6/tests/stacking_estimator_tests.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)      116 2019-03-01 17:58:10.000000 TPOT-0.9.6/MANIFEST.in
+-rw-r--r--   0 weixuanfu   (501) staff       (20)    10917 2019-03-01 17:58:10.000000 TPOT-0.9.6/README.md
+-rw-r--r--   0 weixuanfu   (501) staff       (20)     2310 2019-03-01 17:58:10.000000 TPOT-0.9.6/setup.py
+-rw-r--r--   0 weixuanfu   (501) staff       (20)       38 2019-03-01 18:00:14.000000 TPOT-0.9.6/setup.cfg
```

### Comparing `TPOT-0.9.5/PKG-INFO` & `TPOT-0.9.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: TPOT
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot
 Author: Randal S. Olson
 Author-email: rso@randalolson.com
 License: GNU/LGPLv3
 Description: 
         A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
@@ -26,7 +26,11 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: skrebate
+Provides-Extra: dask
+Provides-Extra: xgboost
+Provides-Extra: mdr
```

### Comparing `TPOT-0.9.5/tpot/metrics.py` & `TPOT-0.9.6/tpot/metrics.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/export_utils.py` & `TPOT-0.9.6/tpot/export_utils.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/_version.py` & `TPOT-0.9.6/tpot/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General Public
 License along with TPOT. If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-__version__ = '0.9.5'
+__version__ = '0.9.6'
```

### Comparing `TPOT-0.9.5/tpot/config/classifier_sparse.py` & `TPOT-0.9.6/tpot/config/classifier_sparse.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/classifier_light.py` & `TPOT-0.9.6/tpot/config/classifier_light.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/classifier.py` & `TPOT-0.9.6/tpot/config/classifier.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/regressor_mdr.py` & `TPOT-0.9.6/tpot/config/regressor_mdr.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/regressor_sparse.py` & `TPOT-0.9.6/tpot/config/regressor_sparse.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/__init__.py` & `TPOT-0.9.6/tpot/config/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/classifier_mdr.py` & `TPOT-0.9.6/tpot/config/classifier_mdr.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/regressor_light.py` & `TPOT-0.9.6/tpot/config/regressor_light.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/config/regressor.py` & `TPOT-0.9.6/tpot/config/regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,15 @@
         'max_features': np.arange(0.05, 1.01, 0.05),
         'alpha': [0.75, 0.8, 0.85, 0.9, 0.95, 0.99]
     },
 
     'sklearn.ensemble.AdaBoostRegressor': {
         'n_estimators': [100],
         'learning_rate': [1e-3, 1e-2, 1e-1, 0.5, 1.],
-        'loss': ["linear", "square", "exponential"],
-        'max_depth': range(1, 11)
+        'loss': ["linear", "square", "exponential"]
     },
 
     'sklearn.tree.DecisionTreeRegressor': {
         'max_depth': range(1, 11),
         'min_samples_split': range(2, 21),
         'min_samples_leaf': range(1, 21)
     },
```

### Comparing `TPOT-0.9.5/tpot/__init__.py` & `TPOT-0.9.6/tpot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/builtins/feature_transformers.py` & `TPOT-0.9.6/tpot/builtins/feature_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         X : array-like
         """
         X = check_array(X)
         return self
 
 
     def transform(self, X):
-        """Select continuous features and transform them using OneHotEncoder.
+        """Select continuous features and transform them using PCA.
 
         Parameters
         ----------
         X: numpy ndarray, {n_samples, n_components}
             New data, where n_samples is the number of samples and n_components is the number of components.
 
         Returns
```

### Comparing `TPOT-0.9.5/tpot/builtins/zero_count.py` & `TPOT-0.9.6/tpot/builtins/zero_count.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/builtins/__init__.py` & `TPOT-0.9.6/tpot/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/builtins/stacking_estimator.py` & `TPOT-0.9.6/tpot/builtins/stacking_estimator.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/builtins/combine_dfs.py` & `TPOT-0.9.6/tpot/builtins/combine_dfs.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/builtins/one_hot_encoder.py` & `TPOT-0.9.6/tpot/builtins/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/tpot.py` & `TPOT-0.9.6/tpot/tpot.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/operator_utils.py` & `TPOT-0.9.6/tpot/operator_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,21 +39,25 @@
 
 class ARGType(object):
     """Base class for parameter specifications."""
 
     pass
 
 
-def source_decode(sourcecode):
+def source_decode(sourcecode, verbose=0):
     """Decode operator source and import operator class.
 
     Parameters
     ----------
     sourcecode: string
         a string of operator source (e.g 'sklearn.feature_selection.RFE')
+    verbose: int, optional (default: 0)
+        How much information TPOT communicates while it's running.
+        0 = none, 1 = minimal, 2 = high, 3 = all.
+        if verbose > 2 then ImportError will rasie during initialization
 
 
     Returns
     -------
     import_str: string
         a string of operator class source (e.g. 'sklearn.feature_selection')
     op_str: string
@@ -67,16 +71,19 @@
     import_str = '.'.join(tmp_path)
     try:
         if sourcecode.startswith('tpot.'):
             exec('from {} import {}'.format(import_str[4:], op_str))
         else:
             exec('from {} import {}'.format(import_str, op_str))
         op_obj = eval(op_str)
-    except ImportError:
-        print('Warning: {} is not available and will not be used by TPOT.'.format(sourcecode))
+    except Exception as e:
+        if verbose > 2:
+            raise ImportError('Error: could not import {}.\n{}'.format(sourcecode, e))
+        else:
+            print('Warning: {} is not available and will not be used by TPOT.'.format(sourcecode))
         op_obj = None
 
     return import_str, op_str, op_obj
 
 
 def set_sample_weight(pipeline_steps, sample_weight=None):
     """Recursively iterates through all objects in the pipeline and sets sample weight.
@@ -123,15 +130,15 @@
     Class
         parameter class
 
     """
     return type(classname, (BaseClass,), {'values': prange})
 
 
-def TPOTOperatorClassFactory(opsourse, opdict, BaseClass=Operator, ArgBaseClass=ARGType):
+def TPOTOperatorClassFactory(opsourse, opdict, BaseClass=Operator, ArgBaseClass=ARGType, verbose=0):
     """Dynamically create operator class.
 
     Parameters
     ----------
     opsourse: string
         operator source in config dictionary (key)
     opdict: dictionary
@@ -140,27 +147,31 @@
         True if it can be used in TPOTRegressor
     classification: bool
         True if it can be used in TPOTClassifier
     BaseClass: Class
         inherited BaseClass for operator
     ArgBaseClass: Class
         inherited BaseClass for parameter
+    verbose: int, optional (default: 0)
+        How much information TPOT communicates while it's running.
+        0 = none, 1 = minimal, 2 = high, 3 = all.
+        if verbose > 2 then ImportError will rasie during initialization
 
     Returns
     -------
     op_class: Class
         a new class for a operator
     arg_types: list
         a list of parameter class
 
     """
     class_profile = {}
     dep_op_list = {} # list of nested estimator/callable function
     dep_op_type = {} # type of nested estimator/callable function
-    import_str, op_str, op_obj = source_decode(opsourse)
+    import_str, op_str, op_obj = source_decode(opsourse, verbose=verbose)
 
     if not op_obj:
         return None, None
     else:
         # define if the operator can be the root of a pipeline
         if issubclass(op_obj, ClassifierMixin) or issubclass(op_obj, RegressorMixin):
             class_profile['root'] = True
@@ -186,15 +197,15 @@
         for pname in sorted(opdict.keys()):
             prange = opdict[pname]
             if not isinstance(prange, dict):
                 classname = '{}__{}'.format(op_str, pname)
                 arg_types.append(ARGTypeClassFactory(classname, prange, ArgBaseClass))
             else:
                 for dkey, dval in prange.items():
-                    dep_import_str, dep_op_str, dep_op_obj = source_decode(dkey)
+                    dep_import_str, dep_op_str, dep_op_obj = source_decode(dkey, verbose=verbose)
                     if dep_import_str in import_hash:
                         import_hash[import_str].append(dep_op_str)
                     else:
                         import_hash[dep_import_str] = [dep_op_str]
                     dep_op_list[pname] = dep_op_str
                     dep_op_type[pname] = dep_op_obj
                     if dval:
```

### Comparing `TPOT-0.9.5/tpot/gp_types.py` & `TPOT-0.9.6/tpot/gp_types.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/driver.py` & `TPOT-0.9.6/tpot/driver.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tpot/base.py` & `TPOT-0.9.6/tpot/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 from .config.regressor_mdr import tpot_mdr_regressor_config_dict
 from .config.regressor_sparse import regressor_config_sparse
 from .config.classifier_sparse import classifier_config_sparse
 
 from .metrics import SCORERS
 from .gp_types import Output_Array
 from .gp_deap import eaMuPlusLambda, mutNodeReplacement, _wrapped_cross_val_score, cxOnePoint
+with warnings.catch_warnings():
+    warnings.simplefilter('ignore')
+    from tqdm.autonotebook import tqdm
 
 # hot patch for Windows: solve the problem of crashing python after Ctrl + C in Windows OS
 # https://github.com/ContinuumIO/anaconda-issues/issues/905
 if sys.platform.startswith('win'):
     import win32api
 
     try:
@@ -89,33 +92,14 @@
             hook_sigint()
             return 1  # don't chain to the next handler
         return 0
 
 
     win32api.SetConsoleCtrlHandler(handler, 1)
 
-def is_notebook():
-    """Check if TPOT is running in Jupyter notebook.
-    Returns
-    -------
-    True: TPOT is running in Jupyter notebook
-    False: TPOT is running in other terminals
-    """
-    try:
-        from IPython import get_ipython
-        shell = get_ipython().__class__.__name__
-        # if shell == 'TerminalInteractiveShell', then Terminal running IPython
-        return shell == 'ZMQInteractiveShell'
-    except:
-        return False
-
-if is_notebook():
-    from tqdm import tqdm_notebook as tqdm
-else:
-    from tqdm import tqdm
 
 
 class TPOTBase(BaseEstimator):
     """Automatically creates and optimizes machine learning pipelines using GP."""
 
     def __init__(self, generations=100, population_size=100, offspring_size=None,
                  mutation_rate=0.9, crossover_rate=0.1,
@@ -241,15 +225,15 @@
             the same estimator on the same split of data multiple times. It
             will also provide more detailed diagnostics when using Dask's
             distributed scheduler.
 
             See `avoid repeated work <https://dask-ml.readthedocs.io/en/latest/hyper-parameter-search.html#avoid-repeated-work>`__
             for more details.
         periodic_checkpoint_folder: path string, optional (default: None)
-            If supplied, a folder in which tpot will periodically save the best pipeline so far while optimizing.
+            If supplied, a folder in which tpot will periodically save pipelines in pareto front so far while optimizing.
             Currently once per generation but not more often than once per 30 seconds.
             Useful in multiple cases:
                 Sudden death before tpot could save optimized pipeline
                 Track its progress
                 Grab pipelines while it's still optimizing
         early_stop: int or None (default: None)
             How many generations TPOT checks whether there is no improvement in optimization process.
@@ -456,15 +440,15 @@
             self._pop = []
             self._pareto_front = None
             self._last_optimized_pareto_front = None
             self._last_optimized_pareto_front_n_gens = 0
 
         self._optimized_pipeline = None
         self._optimized_pipeline_score = None
-        self._exported_pipeline_text = ""
+        self._exported_pipeline_text = []
         self.fitted_pipeline_ = None
         self._fitted_imputer = None
         self._imputed = False
         self._memory = None # initial Memory setting for sklearn pipeline
 
         # dont save periodic pipelines more often than this
         self._output_best_pipeline_period_seconds = 30
@@ -478,15 +462,16 @@
         self.operators = []
         self.arguments = []
         for key in sorted(self._config_dict.keys()):
             op_class, arg_types = TPOTOperatorClassFactory(
                 key,
                 self._config_dict[key],
                 BaseClass=Operator,
-                ArgBaseClass=ARGType
+                ArgBaseClass=ARGType,
+                verbose=self.verbosity
             )
             if op_class:
                 self.operators.append(op_class)
                 self.arguments += arg_types
 
         # Schedule TPOT to run for many generations if the user specifies a
         # run-time limit TPOT will automatically interrupt itself when the timer
@@ -926,84 +911,102 @@
         # We handle them in reverse so we do not mess up indices
         pretty = dirty_string
         for (start, end) in reversed(parameter_prefixes):
             pretty = pretty[:start + 2] + pretty[end:]
 
         return pretty
 
-    def _check_periodic_pipeline(self):
-        """If enough time has passed, save a new optimized pipeline.
+    def _check_periodic_pipeline(self, gen):
+        """If enough time has passed, save a new optimized pipeline. Currently used in the per generation hook in the optimization loop.
+        Parameters
+        ----------
+        gen: int
+            Generation number
 
-        Currently used in the per generation hook in the optimization loop.
+        Returns
+        -------
+        None
         """
         self._update_top_pipeline()
         if self.periodic_checkpoint_folder is not None:
             total_since_last_pipeline_save = (datetime.now() - self._last_pipeline_write).total_seconds()
             if total_since_last_pipeline_save > self._output_best_pipeline_period_seconds:
                 self._last_pipeline_write = datetime.now()
-                self._save_periodic_pipeline()
+                self._save_periodic_pipeline(gen)
 
         if self.early_stop is not None:
             if self._last_optimized_pareto_front_n_gens >= self.early_stop:
                 raise StopIteration("The optimized pipeline was not improved after evaluating {} more generations. "
                                     "Will end the optimization process.\n".format(self.early_stop))
 
-    def _save_periodic_pipeline(self):
+    def _save_periodic_pipeline(self, gen):
         try:
             self._create_periodic_checkpoint_folder()
-            filename = os.path.join(self.periodic_checkpoint_folder, 'pipeline_{}.py'.format(datetime.now().strftime('%Y.%m.%d_%H-%M-%S')))
-            did_export = self.export(filename, skip_if_repeated=True)
-            if not did_export:
-                self._update_pbar(pbar_num=0, pbar_msg='Periodic pipeline was not saved, probably saved before...')
-            else:
-                self._update_pbar(pbar_num=0, pbar_msg='Saving best periodic pipeline to {}'.format(filename))
+            for pipeline, pipeline_scores in zip(self._pareto_front.items, reversed(self._pareto_front.keys)):
+                idx = self._pareto_front.items.index(pipeline)
+                pareto_front_pipeline_score = pipeline_scores.wvalues[1]
+                sklearn_pipeline_str = generate_pipeline_code(expr_to_tree(pipeline, self._pset), self.operators)
+                to_write = export_pipeline(pipeline,
+                                            self.operators, self._pset,
+                                            self._imputed, pareto_front_pipeline_score,
+                                            self.random_state)
+                # dont export a pipeline you  had
+                if self._exported_pipeline_text.count(sklearn_pipeline_str):
+                    self._update_pbar(pbar_num=0, pbar_msg='Periodic pipeline was not saved, probably saved before...')
+                else:
+                    filename = os.path.join(self.periodic_checkpoint_folder,
+                                            'pipeline_gen_{}_idx_{}_{}.py'.format(gen,
+                                                                                idx ,
+                                                                                datetime.now().strftime('%Y.%m.%d_%H-%M-%S')
+                                                                                )
+                                            )
+                    self._update_pbar(pbar_num=0, pbar_msg='Saving periodic pipeline from pareto front to {}'.format(filename))
+                    with open(filename, 'w') as output_file:
+                        output_file.write(to_write)
+                    self._exported_pipeline_text.append(sklearn_pipeline_str)
+
         except Exception as e:
             self._update_pbar(pbar_num=0, pbar_msg='Failed saving periodic pipeline, exception:\n{}'.format(str(e)[:250]))
 
     def _create_periodic_checkpoint_folder(self):
         try:
             os.makedirs(self.periodic_checkpoint_folder)
             self._update_pbar(pbar_msg='Created new folder to save periodic pipeline: {}'.format(self.periodic_checkpoint_folder))
         except OSError as e:
             if e.errno == errno.EEXIST and os.path.isdir(self.periodic_checkpoint_folder):
                 pass # Folder already exists. User probably created it.
             else:
                 raise ValueError('Failed creating the periodic_checkpoint_folder:\n{}'.format(e))
 
-    def export(self, output_file_name, skip_if_repeated=False):
+
+    def export(self, output_file_name):
         """Export the optimized pipeline as Python code.
 
         Parameters
         ----------
         output_file_name: string
             String containing the path and file name of the desired output file
-        skip_if_repeated: boolean
-            If True, skip the actual writing if a pipeline
-            code would be identical to the last pipeline exported
 
         Returns
         -------
         False if it skipped writing the pipeline to file
         True if the pipeline was actually written
 
         """
         if self._optimized_pipeline is None:
             raise RuntimeError('A pipeline has not yet been optimized. Please call fit() first.')
 
-        to_write = export_pipeline(self._optimized_pipeline, self.operators, self._pset, self._imputed, self._optimized_pipeline_score, self.random_state)
-
-        # dont export a pipeline you just had
-        if skip_if_repeated and (self._exported_pipeline_text == to_write):
-            return False
+        to_write = export_pipeline(self._optimized_pipeline,
+                                    self.operators, self._pset,
+                                    self._imputed, self._optimized_pipeline_score,
+                                    self.random_state)
 
         with open(output_file_name, 'w') as output_file:
             output_file.write(to_write)
-            self._exported_pipeline_text = to_write
 
-        return True
 
     def _impute_values(self, features):
         """Impute missing values in a feature set.
 
         Parameters
         ----------
         features: array-like {n_samples, n_features}
@@ -1158,20 +1161,20 @@
             and all the statistics contained in the 'individual_stats' parameter
         """
         stats = deepcopy(individual_stats)  # Deepcopy, since the string reference to predecessor should be cloned
         stats['operator_count'] = operator_count
         stats['internal_cv_score'] = cv_score
         return stats
 
-    def _evaluate_individuals(self, individuals, features, target, sample_weight=None, groups=None):
+    def _evaluate_individuals(self, population, features, target, sample_weight=None, groups=None):
         """Determine the fit of the provided individuals.
 
         Parameters
         ----------
-        individuals: a list of DEAP individual
+        population: a list of DEAP individual
             One individual is a list of pipeline operators and model parameters that can be
             compiled by DEAP into a callable function
         features: numpy.ndarray {n_samples, n_features}
             A numpy matrix containing the training and testing features for the individual's evaluation
         target: numpy.ndarray {n_samples}
             A numpy matrix containing the training and testing target for the individual's evaluation
         sample_weight: array-like {n_samples}, optional
@@ -1182,14 +1185,20 @@
         Returns
         -------
         fitnesses_ordered: float
             Returns a list of tuple value indicating the individual's fitness
             according to its performance on the provided data
 
         """
+        # Evaluate the individuals with an invalid fitness
+        individuals = [ind for ind in population if not ind.fitness.valid]
+
+        # update pbar for valid individuals (with fitness values)
+        if self.verbosity > 0:
+            self._pbar.update(len(population)-len(individuals))
 
         operator_counts, eval_individuals_str, sklearn_pipeline_list, stats_dicts = self._preprocess_individuals(individuals)
 
         # Make the partial function that will be called below
         partial_wrapped_cross_val_score = partial(
             _wrapped_cross_val_score,
             features=features,
@@ -1199,58 +1208,82 @@
             sample_weight=sample_weight,
             groups=groups,
             timeout=max(int(self.max_eval_time_mins * 60), 1),
             use_dask=self.use_dask
         )
 
         result_score_list = []
-        # Don't use parallelization if n_jobs==1
-        if self._n_jobs == 1 and not self.use_dask:
-            for sklearn_pipeline in sklearn_pipeline_list:
-                self._stop_by_max_time_mins()
-                val = partial_wrapped_cross_val_score(sklearn_pipeline=sklearn_pipeline)
-                result_score_list = self._update_val(val, result_score_list)
-        else:
-            if self.use_dask:
-                import dask
-
-                result_score_list = [
-                    partial_wrapped_cross_val_score(sklearn_pipeline=sklearn_pipeline)
-                    for sklearn_pipeline in sklearn_pipeline_list
-                ]
-
-                self.dask_graphs_ = result_score_list
-                with warnings.catch_warnings():
-                    warnings.simplefilter('ignore')
-                    result_score_list = list(dask.compute(*result_score_list))
-
-                self._update_pbar(len(result_score_list))
-
+        try:
+            # Don't use parallelization if n_jobs==1
+            if self._n_jobs == 1 and not self.use_dask:
+                for sklearn_pipeline in sklearn_pipeline_list:
+                    self._stop_by_max_time_mins()
+                    val = partial_wrapped_cross_val_score(sklearn_pipeline=sklearn_pipeline)
+                    result_score_list = self._update_val(val, result_score_list)
             else:
                 # chunk size for pbar update
                 # chunk size is min of cpu_count * 2 and n_jobs * 4
                 chunk_size = min(cpu_count()*2, self._n_jobs*4)
-
                 for chunk_idx in range(0, len(sklearn_pipeline_list), chunk_size):
                     self._stop_by_max_time_mins()
+                    if self.use_dask:
+                        import dask
+                        tmp_result_scores = [
+                            partial_wrapped_cross_val_score(sklearn_pipeline=sklearn_pipeline)
+                            for sklearn_pipeline in sklearn_pipeline_list[chunk_idx:chunk_idx + chunk_size]
+                        ]
+
+                        self.dask_graphs_ = tmp_result_scores
+                        with warnings.catch_warnings():
+                            warnings.simplefilter('ignore')
+                            tmp_result_scores = list(dask.compute(*tmp_result_scores))
+
+                    else:
 
-                    parallel = Parallel(n_jobs=self._n_jobs, verbose=0, pre_dispatch='2*n_jobs')
-                    tmp_result_scores = parallel(
-                        delayed(partial_wrapped_cross_val_score)(sklearn_pipeline=sklearn_pipeline)
-                        for sklearn_pipeline in sklearn_pipeline_list[chunk_idx:chunk_idx + chunk_size])
+                        parallel = Parallel(n_jobs=self._n_jobs, verbose=0, pre_dispatch='2*n_jobs')
+                        tmp_result_scores = parallel(
+                            delayed(partial_wrapped_cross_val_score)(sklearn_pipeline=sklearn_pipeline)
+                            for sklearn_pipeline in sklearn_pipeline_list[chunk_idx:chunk_idx + chunk_size])
                     # update pbar
                     for val in tmp_result_scores:
                         result_score_list = self._update_val(val, result_score_list)
 
+        except (KeyboardInterrupt, SystemExit, StopIteration) as e:
+            if self.verbosity > 0:
+                self._pbar.write('', file=self._file)
+                self._pbar.write('{}\nTPOT closed during evaluation in one generation.\n'
+                                    'WARNING: TPOT may not provide a good pipeline if TPOT is stopped/interrupted in a early generation.'.format(e),
+                                 file=self._file)
+            # number of individuals already evaluated in this generation
+            num_eval_ind = len(result_score_list)
+            self._update_evaluated_individuals_(result_score_list,
+                                                eval_individuals_str[:num_eval_ind],
+                                                operator_counts,
+                                                stats_dicts)
+            for ind in individuals[:num_eval_ind]:
+                ind_str = str(ind)
+                ind.fitness.values = (self.evaluated_individuals_[ind_str]['operator_count'],
+                                    self.evaluated_individuals_[ind_str]['internal_cv_score'])
+            # for individuals were not evaluated in this generation, TPOT will assign a bad fitness score
+            for ind in individuals[num_eval_ind:]:
+                ind.fitness.values = (5000.,-float('inf'))
+
+            self._pareto_front.update(population)
+            raise KeyboardInterrupt
+
         self._update_evaluated_individuals_(result_score_list, eval_individuals_str, operator_counts, stats_dicts)
 
-        """Look up the operator count and cross validation score to use in the optimization"""
-        return [(self.evaluated_individuals_[str(individual)]['operator_count'],
-                 self.evaluated_individuals_[str(individual)]['internal_cv_score'])
-                for individual in individuals]
+        for ind in individuals:
+            ind_str = str(ind)
+            ind.fitness.values = (self.evaluated_individuals_[ind_str]['operator_count'],
+                                self.evaluated_individuals_[ind_str]['internal_cv_score'])
+        individuals = [ind for ind in population if not ind.fitness.valid]
+        self._pareto_front.update(population)
+
+        return population
 
     def _preprocess_individuals(self, individuals):
         """Preprocess DEAP individuals before pipeline evaluation.
 
         Parameters
         ----------
         individuals: a list of DEAP individual
```

### Comparing `TPOT-0.9.5/tpot/gp_deap.py` & `TPOT-0.9.6/tpot/gp_deap.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,56 +220,48 @@
     logbook = tools.Logbook()
     logbook.header = ['gen', 'nevals'] + (stats.fields if stats else [])
 
     # Initialize statistics dict for the individuals in the population, to keep track of mutation/crossover operations and predecessor relations
     for ind in population:
         initialize_stats_dict(ind)
 
-    # Evaluate the individuals with an invalid fitness
-    invalid_ind = [ind for ind in population if not ind.fitness.valid]
-
-    fitnesses = toolbox.evaluate(invalid_ind)
-    for ind, fit in zip(invalid_ind, fitnesses):
-        ind.fitness.values = fit
-
-    if halloffame is not None:
-        halloffame.update(population)
+    population = toolbox.evaluate(population)
 
     record = stats.compile(population) if stats is not None else {}
-    logbook.record(gen=0, nevals=len(invalid_ind), **record)
+    logbook.record(gen=0, nevals=len(population), **record)
 
     # Begin the generational process
     for gen in range(1, ngen + 1):
-        # after each population save a periodic pipeline
-        if per_generation_function is not None:
-            per_generation_function()
+
 
         # Vary the population
         offspring = varOr(population, toolbox, lambda_, cxpb, mutpb)
 
         # Update generation statistic for all individuals which have invalid 'generation' stats
         # This hold for individuals that have been altered in the varOr function
         for ind in population:
             if ind.statistics['generation'] == 'INVALID':
                 ind.statistics['generation'] = gen
 
         # Evaluate the individuals with an invalid fitness
         invalid_ind = [ind for ind in offspring if not ind.fitness.valid]
-
+        """
         # update pbar for valid individuals (with fitness values)
         if not pbar.disable:
             pbar.update(len(offspring)-len(invalid_ind))
 
         fitnesses = toolbox.evaluate(invalid_ind)
         for ind, fit in zip(invalid_ind, fitnesses):
             ind.fitness.values = fit
 
         # Update the hall of fame with the generated individuals
         if halloffame is not None:
-            halloffame.update(offspring)
+            halloffame.update(offspring)"""
+
+        offspring = toolbox.evaluate(offspring)
 
         # Select the next generation population
         population[:] = toolbox.select(population + offspring, mu)
 
         # pbar process
         if not pbar.disable:
             # Print only the best individual fitness
@@ -285,14 +277,18 @@
                             int(pipeline_scores.wvalues[0]),
                             pipeline_scores.wvalues[1],
                             pipeline
                         )
                     )
                 pbar.write('')
 
+        # after each population save a periodic pipeline
+        if per_generation_function is not None:
+            per_generation_function(gen)
+
         # Update the statistics with the new population
         record = stats.compile(population) if stats is not None else {}
         logbook.record(gen=gen, nevals=len(invalid_ind), **record)
 
     return population, logbook
```

### Comparing `TPOT-0.9.5/tpot/decorators.py` & `TPOT-0.9.6/tpot/decorators.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/LICENSE` & `TPOT-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/images/tpot-ml-pipeline.png` & `TPOT-0.9.6/images/tpot-ml-pipeline.png`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/images/tpot-demo.gif` & `TPOT-0.9.6/images/tpot-demo.gif`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/images/tpot-pipeline-example.png` & `TPOT-0.9.6/images/tpot-pipeline-example.png`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/images/tpot-logo.jpg` & `TPOT-0.9.6/images/tpot-logo.jpg`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/TPOT.egg-info/PKG-INFO` & `TPOT-0.9.6/TPOT.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: TPOT
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tree-based Pipeline Optimization Tool
 Home-page: https://github.com/EpistasisLab/tpot
 Author: Randal S. Olson
 Author-email: rso@randalolson.com
 License: GNU/LGPLv3
 Description: 
         A Python tool that automatically creates and optimizes machine learning pipelines using genetic programming.
@@ -26,7 +26,11 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: skrebate
+Provides-Extra: dask
+Provides-Extra: xgboost
+Provides-Extra: mdr
```

### Comparing `TPOT-0.9.5/TPOT.egg-info/SOURCES.txt` & `TPOT-0.9.6/TPOT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/driver_tests.py` & `TPOT-0.9.6/tests/driver_tests.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/one_hot_encoder_tests.py` & `TPOT-0.9.6/tests/one_hot_encoder_tests.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/tpot_tests.py` & `TPOT-0.9.6/tests/tpot_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
 You should have received a copy of the GNU Lesser General Public
 License along with TPOT. If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 from tpot import TPOTClassifier, TPOTRegressor
-from tpot.base import TPOTBase, is_notebook
+from tpot.base import TPOTBase
 from tpot.driver import float_range
 from tpot.gp_types import Output_Array
 from tpot.gp_deap import mutNodeReplacement, _wrapped_cross_val_score, pick_two_individuals_eligible_for_crossover, cxOnePoint, varOr, initialize_stats_dict
 from tpot.metrics import balanced_accuracy, SCORERS
-from tpot.operator_utils import TPOTOperatorClassFactory, set_sample_weight
+from tpot.operator_utils import TPOTOperatorClassFactory, set_sample_weight, source_decode
 from tpot.decorators import pretest_X, pretest_y
 
 from tpot.config.classifier import classifier_config_dict
 from tpot.config.classifier_light import classifier_config_dict_light
 from tpot.config.regressor_light import regressor_config_dict_light
 from tpot.config.classifier_mdr import tpot_mdr_classifier_config_dict
 from tpot.config.regressor_mdr import tpot_mdr_regressor_config_dict
@@ -59,15 +59,17 @@
 from sklearn.externals.joblib import Memory
 from sklearn.metrics import make_scorer, roc_auc_score
 from deap import creator, gp
 from deap.tools import ParetoFront
 from nose.tools import assert_raises, assert_not_equal, assert_greater_equal, assert_equal, assert_in
 from driver_tests import captured_output
 
-from tqdm import tqdm
+with warnings.catch_warnings():
+    warnings.simplefilter('ignore')
+    from tqdm.autonotebook import tqdm
 
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 # Ensure we can use `with closing(...) as ... :` syntax
@@ -150,21 +152,15 @@
     assert tpot_obj._pop == []
     assert tpot_obj._pareto_front == None
     assert tpot_obj._last_optimized_pareto_front == None
     assert tpot_obj._last_optimized_pareto_front_n_gens == 0
     assert tpot_obj._optimized_pipeline == None
     assert tpot_obj._optimized_pipeline_score == None
     assert tpot_obj.fitted_pipeline_ == None
-    assert tpot_obj._exported_pipeline_text == ""
-
-
-def test_is_notebook():
-    """Assert that isnotebook function works as expected."""
-    ret = is_notebook()
-    assert not ret
+    assert tpot_obj._exported_pipeline_text == []
 
 
 def test_init_default_scoring():
     """Assert that TPOT intitializes with the correct default scoring function."""
     tpot_obj = TPOTRegressor()
     assert tpot_obj.scoring_function == 'neg_mean_squared_error'
 
@@ -221,15 +217,15 @@
         return roc_auc_score(y_true, y_pred)
     with warnings.catch_warnings(record=True) as w:
         tpot_obj = TPOTClassifier(scoring=my_scorer)
         tpot_obj._fit_init()
     assert len(w) == 1
     assert issubclass(w[-1].category, DeprecationWarning)
     assert "This scoring type was deprecated" in str(w[-1].message)
-    print(tpot_obj.scoring_function)
+
     assert tpot_obj.scoring_function == 'my_scorer'
 
 
 def test_invalid_score_warning():
     """Assert that the TPOT intitializes raises a ValueError when the scoring metrics is not available in SCORERS."""
     # Mis-spelled scorer
     tpot_obj = TPOTClassifier(scoring='balanced_accuray')
@@ -523,15 +519,15 @@
     assert np.allclose(known_score, score)
 
 
 def test_score_3():
     """Assert that the TPOTRegressor score function outputs a known score for a fixed pipeline."""
     tpot_obj = TPOTRegressor(scoring='neg_mean_squared_error', random_state=72)
     tpot_obj._fit_init()
-    known_score = -12.1791953611
+    known_score = -11.682841148312662
 
     # Reify pipeline with known score
     pipeline_string = (
         "ExtraTreesRegressor("
         "GradientBoostingRegressor(input_matrix, GradientBoostingRegressor__alpha=0.8,"
         "GradientBoostingRegressor__learning_rate=0.1,GradientBoostingRegressor__loss=huber,"
         "GradientBoostingRegressor__max_depth=5, GradientBoostingRegressor__max_features=0.5,"
@@ -586,17 +582,18 @@
 
     np.random.seed(42)
     cv_score_weight = cross_val_score(tpot_obj.fitted_pipeline_, training_features_r, training_target_r, cv=3, scoring='neg_mean_squared_error', fit_params=training_target_r_weight_dict)
 
     np.random.seed(42)
     tpot_obj.fitted_pipeline_.fit(training_features_r, training_target_r, **training_target_r_weight_dict)
     # Get score from TPOT
-    known_score = -11.5790430757
+    known_score = -11.586816877933911
     score = tpot_obj.score(testing_features_r, testing_target_r)
 
+
     assert np.allclose(cv_score1, cv_score2)
     assert not np.allclose(cv_score1, cv_score_weight)
     assert np.allclose(known_score, score)
 
 
 def test_fit_GroupKFold():
     """Assert that TPOT properly handles the group parameter when using GroupKFold."""
@@ -1001,71 +998,39 @@
     tpot_obj.fit(training_features, training_target)
     with closing(StringIO()) as our_file:
         tpot_obj._file = our_file
         tpot_obj.verbosity = 3
         tpot_obj._last_pipeline_write = datetime.now()
         sleep(0.11)
         tpot_obj._output_best_pipeline_period_seconds = 0.1
-        tpot_obj.periodic_checkpoint_folder = './'
-        tpot_obj._check_periodic_pipeline()
+        tmpdir = mkdtemp() + '/'
+        tpot_obj.periodic_checkpoint_folder = tmpdir
+        tpot_obj._check_periodic_pipeline(1)
         our_file.seek(0)
-
-        assert_in('Saving best periodic pipeline to ./pipeline', our_file.read())
+        assert_in('Saving periodic pipeline from pareto front', our_file.read())
         # clean up
-        for f in os.listdir('./'):
-            if search('pipeline_', f):
-                os.remove(os.path.join('./', f))
+        rmtree(tmpdir)
 
 
 def test_check_periodic_pipeline_2():
-    """Assert that the _check_periodic_pipeline does not export periodic pipeline if the pipeline has been saved before."""
-    tpot_obj = TPOTClassifier(
-        random_state=42,
-        population_size=1,
-        offspring_size=2,
-        generations=1,
-        verbosity=0,
-        config_dict='TPOT light'
-    )
-    tpot_obj.fit(training_features, training_target)
-    with closing(StringIO()) as our_file:
-        tpot_obj._file = our_file
-        tpot_obj.verbosity = 3
-        tpot_obj._last_pipeline_write = datetime.now()
-        sleep(0.11)
-        tpot_obj._output_best_pipeline_period_seconds = 0.1
-        tpot_obj.periodic_checkpoint_folder = './'
-        # export once before
-        tpot_obj.export('./pipeline_test.py')
-        tpot_obj._check_periodic_pipeline()
-        our_file.seek(0)
-
-        assert_in('Periodic pipeline was not saved, probably saved before...', our_file.read())
-        # clean up
-        for f in os.listdir('./'):
-            if search('pipeline_', f):
-                os.remove(os.path.join('./', f))
-
-
-def test_check_periodic_pipeline_3():
     """Assert that the _check_periodic_pipeline rasie StopIteration if self._last_optimized_pareto_front_n_gens >= self.early_stop."""
     tpot_obj = TPOTClassifier(
         random_state=42,
         population_size=1,
         offspring_size=2,
         generations=1,
         verbosity=0,
         config_dict='TPOT light'
     )
     tpot_obj.fit(training_features, training_target)
     tpot_obj.early_stop = 3
     # will pass
-    tpot_obj._check_periodic_pipeline()
+    tpot_obj._check_periodic_pipeline(1)
     tpot_obj._last_optimized_pareto_front_n_gens = 3
-    assert_raises(StopIteration, tpot_obj._check_periodic_pipeline)
+    assert_raises(StopIteration, tpot_obj._check_periodic_pipeline, 1)
 
 
 def test_save_periodic_pipeline():
     """Assert that the _save_periodic_pipeline does not export periodic pipeline if exception happened"""
     tpot_obj = TPOTClassifier(
         random_state=42,
         population_size=1,
@@ -1077,26 +1042,26 @@
     tpot_obj.fit(training_features, training_target)
     with closing(StringIO()) as our_file:
         tpot_obj._file = our_file
         tpot_obj.verbosity = 3
         tpot_obj._last_pipeline_write = datetime.now()
         sleep(0.11)
         tpot_obj._output_best_pipeline_period_seconds = 0.1
-        tpot_obj.periodic_checkpoint_folder = './'
-        # reset _optimized_pipeline to rasie exception
-        tpot_obj._optimized_pipeline = None
+        tmpdir = mkdtemp() + '/'
+        tpot_obj.periodic_checkpoint_folder = tmpdir
+        # reset _pareto_front to rasie exception
+        tpot_obj._pareto_front = None
 
-        tpot_obj._save_periodic_pipeline()
+        tpot_obj._save_periodic_pipeline(1)
         our_file.seek(0)
 
         assert_in('Failed saving periodic pipeline, exception', our_file.read())
-        # clean up
-        for f in os.listdir('./'):
-            if search('pipeline_', f):
-                os.remove(os.path.join('./', f))
+        #clean up
+        rmtree(tmpdir)
+
 
 def test_save_periodic_pipeline_2():
     """Assert that _save_periodic_pipeline creates the checkpoint folder and exports to it if it didn't exist"""
     tpot_obj = TPOTClassifier(
         random_state=42,
         population_size=1,
         offspring_size=2,
@@ -1107,28 +1072,57 @@
     tpot_obj.fit(training_features, training_target)
     with closing(StringIO()) as our_file:
         tpot_obj._file = our_file
         tpot_obj.verbosity = 3
         tpot_obj._last_pipeline_write = datetime.now()
         sleep(0.11)
         tpot_obj._output_best_pipeline_period_seconds = 0.1
-        tpot_obj.periodic_checkpoint_folder = './tmp'
-        tpot_obj._save_periodic_pipeline()
+        tmpdir = mkdtemp() + '_test/'
+        tpot_obj.periodic_checkpoint_folder = tmpdir
+        tpot_obj._save_periodic_pipeline(1)
         our_file.seek(0)
 
         msg = our_file.read()
-        expected_filepath_prefix = os.path.join('./tmp', 'pipeline_')
-        assert_in('Saving best periodic pipeline to ' + expected_filepath_prefix, msg)
-        assert_in('Created new folder to save periodic pipeline: ./tmp', msg)
 
-        # clean up
-        for f in os.listdir('./tmp'):
-            if search('pipeline_', f):
-                os.remove(os.path.join('./tmp', f))
-        os.rmdir('./tmp')
+        assert_in('Saving periodic pipeline from pareto front to {}'.format(tmpdir), msg)
+        assert_in('Created new folder to save periodic pipeline: {}'.format(tmpdir), msg)
+
+        #clean up
+        rmtree(tmpdir)
+
+
+def test_check_periodic_pipeline_3():
+    """Assert that the _save_periodic_pipeline does not export periodic pipeline if the pipeline has been saved before."""
+    tpot_obj = TPOTClassifier(
+        random_state=42,
+        population_size=1,
+        offspring_size=2,
+        generations=1,
+        verbosity=0,
+        config_dict='TPOT light'
+    )
+    tpot_obj.fit(training_features, training_target)
+    with closing(StringIO()) as our_file:
+        tpot_obj._file = our_file
+        tpot_obj.verbosity = 3
+        tpot_obj._exported_pipeline_text = []
+        tpot_obj._last_pipeline_write = datetime.now()
+        sleep(0.11)
+        tpot_obj._output_best_pipeline_period_seconds = 0
+        tmpdir = mkdtemp() + '/'
+        tpot_obj.periodic_checkpoint_folder = tmpdir
+        # export once before
+        tpot_obj._save_periodic_pipeline(1)
+
+        tpot_obj._save_periodic_pipeline(2)
+
+        our_file.seek(0)
+        assert_in('Periodic pipeline was not saved, probably saved before...', our_file.read())
+    #clean up
+    rmtree(tmpdir)
 
 
 def test_fit_predict():
     """Assert that the TPOT fit_predict function provides an optimized pipeline and correct output."""
     tpot_obj = TPOTClassifier(
         random_state=42,
         population_size=1,
@@ -1317,18 +1311,23 @@
     """Assert that _evaluate_individuals returns operator_counts and CV scores in correct order."""
     tpot_obj = TPOTClassifier(
         random_state=42,
         verbosity=0,
         config_dict='TPOT light'
     )
     tpot_obj._fit_init()
+    def pareto_eq(ind1, ind2):
+        return np.allclose(ind1.fitness.values, ind2.fitness.values)
+
+    tpot_obj._pareto_front = ParetoFront(similar=pareto_eq)
 
     tpot_obj._pbar = tqdm(total=1, disable=True)
     pop = tpot_obj._toolbox.population(n=10)
-    fitness_scores = tpot_obj._evaluate_individuals(pop, training_features, training_target)
+    pop = tpot_obj._evaluate_individuals(pop, training_features, training_target)
+    fitness_scores = [ind.fitness.values for ind in pop]
 
     for deap_pipeline, fitness_score in zip(pop, fitness_scores):
         operator_count = tpot_obj._operator_count(deap_pipeline)
         sklearn_pipeline = tpot_obj._toolbox.compile(expr=deap_pipeline)
         tpot_obj._set_param_recursive(sklearn_pipeline.steps, 'random_state', 42)
 
         try:
@@ -1347,18 +1346,23 @@
     tpot_obj = TPOTClassifier(
         n_jobs=2,
         random_state=42,
         verbosity=0,
         config_dict='TPOT light'
     )
     tpot_obj._fit_init()
+    def pareto_eq(ind1, ind2):
+        return np.allclose(ind1.fitness.values, ind2.fitness.values)
+
+    tpot_obj._pareto_front = ParetoFront(similar=pareto_eq)
 
     tpot_obj._pbar = tqdm(total=1, disable=True)
     pop = tpot_obj._toolbox.population(n=10)
-    fitness_scores = tpot_obj._evaluate_individuals(pop, training_features, training_target)
+    pop = tpot_obj._evaluate_individuals(pop, training_features, training_target)
+    fitness_scores = [ind.fitness.values for ind in pop]
 
     for deap_pipeline, fitness_score in zip(pop, fitness_scores):
         operator_count = tpot_obj._operator_count(deap_pipeline)
         sklearn_pipeline = tpot_obj._toolbox.compile(expr=deap_pipeline)
         tpot_obj._set_param_recursive(sklearn_pipeline.steps, 'random_state', 42)
 
         try:
@@ -1764,14 +1768,37 @@
         verbosity=0,
         config_dict='tests/test_config_sparse.py'
     )
 
     tpot_obj.fit(sparse_features, sparse_target)
 
 
+def test_source_decode():
+    """Assert that the source_decode can decode operator source and import operator class."""
+    import_str, op_str, op_obj = source_decode("sklearn.linear_model.LogisticRegression")
+    from sklearn.linear_model import LogisticRegression
+    assert import_str == "sklearn.linear_model"
+    assert op_str == "LogisticRegression"
+    assert op_obj == LogisticRegression
+
+
+def test_source_decode_2():
+    """Assert that the source_decode return None when sourcecode is not available."""
+    import_str, op_str, op_obj = source_decode("sklearn.linear_model.LogisticReg")
+    from sklearn.linear_model import LogisticRegression
+    assert import_str == "sklearn.linear_model"
+    assert op_str == "LogisticReg"
+    assert op_obj is None
+
+
+def test_source_decode_3():
+    """Assert that the source_decode raise ImportError when sourcecode is not available and verbose=3."""
+    assert_raises(ImportError, source_decode, "sklearn.linear_model.LogisticReg", 3)
+
+
 def test_tpot_operator_factory_class():
     """Assert that the TPOT operators class factory."""
     test_config_dict = {
         'sklearn.svm.LinearSVC': {
             'penalty': ["l1", "l2"],
             'loss': ["hinge", "squared_hinge"],
             'dual': [True, False],
@@ -1806,14 +1833,18 @@
     assert tpot_argument_list[1].values == [True, False]
 
 
 def test_PolynomialFeatures_exception():
     """Assert that TPOT allows only one PolynomialFeatures operator in a pipeline."""
 
     tpot_obj._pbar = tqdm(total=1, disable=True)
+    def pareto_eq(ind1, ind2):
+        return np.allclose(ind1.fitness.values, ind2.fitness.values)
+
+    tpot_obj._pareto_front = ParetoFront(similar=pareto_eq)
     # pipeline with one PolynomialFeatures operator
     pipeline_string_1 = (
         'LogisticRegression(PolynomialFeatures'
         '(input_matrix, PolynomialFeatures__degree=2, PolynomialFeatures__include_bias=False, '
         'PolynomialFeatures__interaction_only=False), LogisticRegression__C=10.0, '
         'LogisticRegression__dual=False, LogisticRegression__penalty=l2)'
     )
@@ -1832,15 +1863,16 @@
     pipelines = []
     pipelines.append(creator.Individual.from_string(pipeline_string_1, tpot_obj._pset))
     pipelines.append(creator.Individual.from_string(pipeline_string_2, tpot_obj._pset))
 
     for pipeline in pipelines:
         initialize_stats_dict(pipeline)
 
-    fitness_scores = tpot_obj._evaluate_individuals(pipelines, pretest_X, pretest_y)
+    pop = tpot_obj._evaluate_individuals(pipelines, pretest_X, pretest_y)
+    fitness_scores = [ind.fitness.values for ind in pop]
     known_scores = [(2, 0.94000000000000006), (5000.0, -float('inf'))]
     assert np.allclose(known_scores, fitness_scores)
 
 
 def test_pick_two_individuals_eligible_for_crossover():
     """Assert that pick_two_individuals_eligible_for_crossover() picks the correct pair of nodes to perform crossover with"""
```

### Comparing `TPOT-0.9.5/tests/test_dask_based.py` & `TPOT-0.9.6/tests/test_dask_based.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests that ensure the dask-based fit matches.
 
 https://github.com/DEAP/deap/issues/75
 """
 import unittest
-
 import nose
 from sklearn.datasets import make_classification
 
 from tpot import TPOTClassifier
 
 try:
     import dask  # noqa
@@ -17,32 +16,32 @@
 
 
 class TestDaskMatches(unittest.TestCase):
 
     def test_dask_matches(self):
         with dask.config.set(scheduler='single-threaded'):
             for n_jobs in [-1]:
-                X, y = make_classification(random_state=0)
+                X, y = make_classification(random_state=42)
                 a = TPOTClassifier(
-                    generations=2,
+                    generations=0,
                     population_size=5,
                     cv=3,
-                    random_state=0,
+                    random_state=42,
                     n_jobs=n_jobs,
                     use_dask=False,
                 )
                 b = TPOTClassifier(
-                    generations=2,
+                    generations=0,
                     population_size=5,
                     cv=3,
-                    random_state=0,
+                    random_state=42,
                     n_jobs=n_jobs,
                     use_dask=True,
                 )
-                b.fit(X, y)
                 a.fit(X, y)
+                b.fit(X, y)
 
                 self.assertEqual(a.score(X, y), b.score(X, y))
                 self.assertEqual(a.pareto_front_fitted_pipelines_.keys(),
                                  b.pareto_front_fitted_pipelines_.keys())
                 self.assertEqual(a.evaluated_individuals_,
                                  b.evaluated_individuals_)
```

### Comparing `TPOT-0.9.5/tests/test_config_sparse.py` & `TPOT-0.9.6/tests/test_config_sparse.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/export_tests.py` & `TPOT-0.9.6/tests/export_tests.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/zero_count_tests.py` & `TPOT-0.9.6/tests/zero_count_tests.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/tests.csv` & `TPOT-0.9.6/tests/tests.csv`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/test_config.py` & `TPOT-0.9.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/stats_test.py` & `TPOT-0.9.6/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/feature_transformers_tests.py` & `TPOT-0.9.6/tests/feature_transformers_tests.py`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/tests/stacking_estimator_tests.py` & `TPOT-0.9.6/tests/stacking_estimator_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 import numpy as np
 from tpot.builtins import StackingEstimator
 from sklearn.linear_model import LogisticRegression, Lasso
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
 from sklearn.pipeline import make_pipeline
 from tpot_tests import training_features, training_target, training_features_r, training_target_r
 from sklearn.model_selection import cross_val_score
+import warnings
+warnings.filterwarnings("ignore")
 
 def test_StackingEstimator_1():
     """Assert that the StackingEstimator returns transformed X with synthetic features in classification."""
     clf = RandomForestClassifier(random_state=42)
     stack_clf = StackingEstimator(estimator=RandomForestClassifier(random_state=42))
     # fit
     clf.fit(training_features, training_target)
@@ -72,16 +74,15 @@
     # scoring
     score = meta_clf.score(X_clf_transformed, training_target)
     pipeline_score = sklearn_pipeline.score(training_features, training_target)
     assert np.allclose(score, pipeline_score)
 
     # test cv score
     cv_score = np.mean(cross_val_score(sklearn_pipeline, training_features, training_target, cv=3, scoring='accuracy'))
-
-    known_cv_score = 0.947282375315
+    known_cv_score = 0.9472823753147593
 
     assert np.allclose(known_cv_score, cv_score)
 
 
 def test_StackingEstimator_4():
     """Assert that the StackingEstimator worked as expected in scikit-learn pipeline in regression."""
     stack_reg = StackingEstimator(estimator=RandomForestRegressor(random_state=42))
@@ -96,10 +97,10 @@
     # scoring
     score = meta_reg.score(X_reg_transformed, training_target_r)
     pipeline_score = sklearn_pipeline.score(training_features_r, training_target_r)
     assert np.allclose(score, pipeline_score)
 
     # test cv score
     cv_score = np.mean(cross_val_score(sklearn_pipeline, training_features_r, training_target_r, cv=3, scoring='r2'))
-    known_cv_score = 0.795877470354
+    known_cv_score = 0.7989564328211737
 
     assert np.allclose(known_cv_score, cv_score)
```

### Comparing `TPOT-0.9.5/README.md` & `TPOT-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `TPOT-0.9.5/setup.py` & `TPOT-0.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ''',
     zip_safe=True,
     install_requires=['numpy>=1.12.1',
                     'scipy>=0.19.0',
                     'scikit-learn>=0.18.1',
                     'deap>=1.0',
                     'update_checker>=0.16',
-                    'tqdm>=4.11.2',
+                    'tqdm>=4.26.0',
                     'stopit>=1.1.1',
                     'pandas>=0.20.2'],
     extras_require={
         'xgboost': ['xgboost==0.6a2'],
         'skrebate': ['skrebate>=0.3.4'],
         'mdr': ['scikit-mdr>=0.4.4'],
         'dask': ['dask>=0.18.2',
```


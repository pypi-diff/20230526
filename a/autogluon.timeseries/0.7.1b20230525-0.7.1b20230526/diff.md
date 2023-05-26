# Comparing `tmp/autogluon.timeseries-0.7.1b20230525.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230525.tar", last modified: Thu May 25 09:04:29 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230526.tar", last modified: Fri May 26 09:04:24 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230525.tar` & `autogluon.timeseries-0.7.1b20230526.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.069214 autogluon.timeseries-0.7.1b20230525/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.069214 autogluon.timeseries-0.7.1b20230525/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.073214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.073214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.073214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.077214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    48501 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41339 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.081214 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-25 09:03:38.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 09:04:28.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:29.073214 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:29.000000 autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.192174 autogluon.timeseries-0.7.1b20230526/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.192174 autogluon.timeseries-0.7.1b20230526/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.192174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.192174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10150 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48369 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41339 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.196174 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-26 09:03:32.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:04:24.192174 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:04:24.000000 autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230525/PKG-INFO` & `autogluon.timeseries-0.7.1b20230526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230525/setup.py` & `autogluon.timeseries-0.7.1b20230526/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 install_requires = [
     # version ranges added in ag.get_dependency_version_ranges()
     "joblib>=1.1,<2",
     "numpy",  # version range defined in `core/_setup_utils.py`
     "scipy",  # version range defined in `core/_setup_utils.py`
     "pandas",  # version range defined in `core/_setup_utils.py`
     "statsmodels>=0.13.0,<0.14",
-    "gluonts>=0.12.4,<0.13",
+    "gluonts>=0.13.1,<0.14",
     "torch>=1.9,<1.14",
     "pytorch-lightning>=1.7.4,<1.10.0",
     "networkx",  # version range defined in `core/_setup_utils.py`
     "statsforecast>=1.4.0,<1.5",
     "mlforecast>=0.7.0,<0.8.0",
     "tqdm",  # version range defined in `core/_setup_utils.py`
     "ujson>=5,<6",  # needed to silence GluonTS warning
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 
 import copy
 import itertools
+import logging
 from collections.abc import Iterable
 from typing import Any, List, Optional, Tuple, Type
 
 import numpy as np
 import pandas as pd
 from joblib.parallel import Parallel, delayed
 from pandas.core.internals import ArrayManager, BlockManager
 
 from autogluon.common.loaders import load_pd
 
+logger = logging.getLogger(__name__)
+
 ITEMID = "item_id"
 TIMESTAMP = "timestamp"
 
 IRREGULAR_TIME_INDEX_FREQSTR = "IRREG"
 
 
 class TimeSeriesDataFrame(pd.DataFrame):
@@ -319,19 +322,25 @@
         df: pd.DataFrame,
         id_column: Optional[str] = None,
         timestamp_column: Optional[str] = None,
     ) -> pd.DataFrame:
 
         df = df.copy()
         if id_column is not None:
-            assert id_column in df.columns, f"Column {id_column} not found!"
+            assert id_column in df.columns, f"Column '{id_column}' not found!"
+            if id_column != ITEMID and ITEMID in df.columns:
+                logger.warning(f"Renaming existing column '{ITEMID}' -> '__{ITEMID}' to avoid name collisions.")
+                df.rename(columns={ITEMID: "__" + ITEMID}, inplace=True)
             df.rename(columns={id_column: ITEMID}, inplace=True)
 
         if timestamp_column is not None:
-            assert timestamp_column in df.columns, f"Column {timestamp_column} not found!"
+            assert timestamp_column in df.columns, f"Column '{timestamp_column}' not found!"
+            if timestamp_column != TIMESTAMP and TIMESTAMP in df.columns:
+                logger.warning(f"Renaming existing column '{TIMESTAMP}' -> '__{TIMESTAMP}' to avoid name collisions.")
+                df.rename(columns={TIMESTAMP: "__" + TIMESTAMP}, inplace=True)
             df.rename(columns={timestamp_column: TIMESTAMP}, inplace=True)
 
         if TIMESTAMP in df.columns:
             df[TIMESTAMP] = pd.to_datetime(df[TIMESTAMP])
 
         cls._validate_data_frame(df)
         return df.set_index([ITEMID, TIMESTAMP])
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .autogluon_tabular import DirectTabularModel, RecursiveTabularModel
-from .gluonts import DeepARModel, SimpleFeedForwardModel, TemporalFusionTransformerModel
+from .gluonts import DeepARModel, DLinearModel, PatchTSTModel, SimpleFeedForwardModel, TemporalFusionTransformerModel
 from .local import (
     ARIMAModel,
     AutoARIMAModel,
     AutoETSModel,
     DynamicOptimizedThetaModel,
     ETSModel,
     NaiveModel,
     SeasonalNaiveModel,
     ThetaModel,
     ThetaStatsmodelsModel,
 )
 
 __all__ = [
     "DeepARModel",
+    "DLinearModel",
+    "PatchTSTModel",
     "SimpleFeedForwardModel",
     "TemporalFusionTransformerModel",
     "ARIMAModel",
     "ETSModel",
     "ThetaModel",
     "DirectTabularModel",
     "RecursiveTabularModel",
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from gluonts.model.predictor import Predictor as GluonTSPredictor
 from gluonts.torch.model.forecast import DistributionForecast
 from pandas.tseries.frequencies import to_offset
 
 from autogluon.common.utils.log_utils import set_logger_verbosity
 from autogluon.core.hpo.constants import RAY_BACKEND
 from autogluon.core.utils import warning_filter
-from autogluon.core.utils.savers import save_pkl
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 from autogluon.timeseries.utils.warning_filters import disable_root_logger
 
 logger = logging.getLogger(__name__)
 gts_logger = logging.getLogger(gluonts.__name__)
@@ -220,19 +219,23 @@
             disable_past_covariates = model_params.get("disable_past_covariates", False)
             if not disable_past_covariates and self.supports_past_covariates:
                 self.num_past_feat_dynamic_real = len(self.metadata.past_covariates_real)
 
         if "callbacks" in kwargs:
             self.callbacks += kwargs["callbacks"]
 
+    @property
+    def default_context_length(self) -> int:
+        return max(10, 2 * self.prediction_length)
+
     def _get_model_params(self) -> dict:
         """Gets params that are passed to the inner model."""
         args = super()._get_model_params().copy()
         args.setdefault("batch_size", 64)
-        args.setdefault("context_length", max(10, 2 * self.prediction_length))
+        args.setdefault("context_length", self.default_context_length)
         args.update(
             dict(
                 freq=self.freq,
                 prediction_length=self.prediction_length,
                 quantiles=self.quantile_levels,
                 callbacks=self.callbacks,
             )
@@ -383,29 +386,30 @@
 
         forecast_init_args = dict(
             forecast_arrays=np.array(forecast_arrays),
             start_date=forecast.start_date,
             forecast_keys=["mean"] + quantile_keys,
             item_id=str(forecast.item_id),
         )
-        if isinstance(forecast.start_date, pd.Timestamp):  # GluonTS version is <0.10
-            forecast_init_args.update({"freq": forecast.freq})
         return QuantileForecast(**forecast_init_args)
 
     @staticmethod
-    def _distribution_to_quantile_forecast(forecast: SampleForecast, quantile_levels: List[float]) -> QuantileForecast:
+    def _distribution_to_quantile_forecast(
+        forecast: DistributionForecast, quantile_levels: List[float]
+    ) -> QuantileForecast:
         raise NotImplementedError
 
     def _gluonts_forecasts_to_data_frame(
         self,
         forecasts: List[Forecast],
         quantile_levels: List[float],
         forecast_index: pd.MultiIndex,
     ) -> TimeSeriesDataFrame:
-        # if predictions are gluonts SampleForecasts, convert to quantile forecasts
+        # TODO: Concatenate all forecasts into a single tensor/object before converting?
+        # Especially for DistributionForecast this could result in massive speedups
         if isinstance(forecasts[0], SampleForecast):
             forecasts = [self._sample_to_quantile_forecast(f, quantile_levels) for f in forecasts]
         elif isinstance(forecasts[0], DistributionForecast):
             forecasts = [self._distribution_to_quantile_forecast(f, quantile_levels) for f in forecasts]
         else:
             assert isinstance(forecasts[0], QuantileForecast), f"Unrecognized forecast type {type(forecasts[0])}"
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 import shutil
 from datetime import timedelta
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type
 
 import gluonts
 import numpy as np
-import pandas as pd
 import torch
 from gluonts.core.component import from_hyperparameters
 from gluonts.model.forecast import QuantileForecast
+from gluonts.torch.model.d_linear import DLinearEstimator
 from gluonts.torch.model.deepar import DeepAREstimator
 from gluonts.torch.model.estimator import PyTorchLightningEstimator as GluonTSPyTorchLightningEstimator
 from gluonts.torch.model.forecast import DistributionForecast
+from gluonts.torch.model.patch_tst import PatchTSTEstimator
 from gluonts.torch.model.predictor import PyTorchPredictor as GluonTSPyTorchPredictor
 from gluonts.torch.model.simple_feedforward import SimpleFeedForwardEstimator
 from gluonts.torch.model.tft import TemporalFusionTransformerEstimator
 from pytorch_lightning.callbacks import Timer
 
 from autogluon.core.hpo.constants import CUSTOM_BACKEND
 from autogluon.core.utils.loaders import load_pkl
@@ -120,29 +121,26 @@
             model.gts_predictor = GluonTSPyTorchPredictor.deserialize(Path(path) / cls.gluonts_model_path)
         return model
 
     @staticmethod
     def _distribution_to_quantile_forecast(
         forecast: DistributionForecast, quantile_levels: List[float]
     ) -> QuantileForecast:
-        forecast_arrays = [forecast.mean]
-        forecast_keys = ["mean"]
-
-        for q in quantile_levels:
-            forecast_arrays.append(forecast.quantile(q))
-            forecast_keys.append(str(q))
+        # Compute all quantiles in parallel instead of a for-loop
+        quantiles = torch.tensor(quantile_levels, device=forecast.distribution.mean.device).reshape(-1, 1)
+        quantile_predictions = forecast.distribution.icdf(quantiles).cpu().detach().numpy()
+        forecast_arrays = np.vstack([forecast.mean, quantile_predictions])
+        forecast_keys = ["mean"] + [str(q) for q in quantile_levels]
 
         forecast_init_args = dict(
-            forecast_arrays=np.array(forecast_arrays),
+            forecast_arrays=forecast_arrays,
             start_date=forecast.start_date,
             forecast_keys=forecast_keys,
             item_id=str(forecast.item_id),
         )
-        if isinstance(forecast.start_date, pd.Timestamp):  # GluonTS version is <0.10
-            forecast_init_args.update({"freq": forecast.freq})
         return QuantileForecast(**forecast_init_args)
 
 
 class DeepARModel(AbstractGluonTSPyTorchModel):
     """DeepAR model from GluonTS based on the PyTorch backend.
 
     The model consists of an LSTM encoder and a decoder that outputs the
@@ -156,17 +154,16 @@
     .. [Salinas2020] Salinas, David, et al.
         "DeepAR: Probabilistic forecasting with autoregressive recurrent networks."
         International Journal of Forecasting. 2020.
 
 
     Other Parameters
     ----------------
-    context_length : int, optional
+    context_length : int, default = max(10, 2 * prediction_length)
         Number of steps to unroll the RNN for before computing predictions
-        (default: None, in which case context_length = prediction_length)
     disable_static_features : bool, default = False
         If True, static features won't be used by the model even if they are present in the dataset.
         If False, static features will be used by the model if they are present in the dataset.
     disable_known_covariates : bool, default = False
         If True, known covariates won't be used by the model even if they are present in the dataset.
         If False, known covariates will be used by the model if they are present in the dataset.
     num_layers : int, default = 2
@@ -213,17 +210,16 @@
 
     Based on `gluonts.torch.model.simple_feedforward.SimpleFeedForwardEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.simple_feedforward.html>`_.
     See GluonTS documentation for additional hyperparameters.
 
 
     Other Parameters
     ----------------
-    context_length : int, optional
+    context_length : int, default = max(10, 2 * prediction_length)
         Number of time units that condition the predictions
-        (default: None, in which case context_length = prediction_length)
     hidden_dimensions: List[int], default = [20, 20]
         Size of hidden layers in the feedforward network
     distr_output : gluonts.torch.distributions.DistributionOutput, default = StudentTOutput()
         Distribution to fit.
     batch_normalization : bool, default = False
         Whether to use batch normalization
     mean_scaling : bool, default = True
@@ -256,15 +252,15 @@
     .. [Lim2021] Lim, Bryan, et al.
         "Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting."
         International Journal of Forecasting. 2021.
 
 
     Other Parameters
     ----------------
-    context_length : int, default = 64
+    context_length : int, default = max(64, 2 * prediction_length)
         Number of past values used for prediction.
     disable_static_features : bool, default = False
         If True, static features won't be used by the model even if they are present in the dataset.
         If False, static features will be used by the model if they are present in the dataset.
     disable_known_covariates : bool, default = False
         If True, known covariates won't be used by the model even if they are present in the dataset.
         If False, known covariates will be used by the model if they are present in the dataset.
@@ -289,19 +285,122 @@
         Learning rate used during training
     """
 
     gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator] = TemporalFusionTransformerEstimator
     supports_known_covariates = True
     supports_past_covariates = True
 
+    @property
+    def default_context_length(self) -> int:
+        return max(64, 2 * self.prediction_length)
+
     def _get_estimator_init_args(self) -> Dict[str, Any]:
         init_kwargs = super()._get_estimator_init_args()
-        init_kwargs["context_length"] = max(64, init_kwargs["context_length"])
         if self.num_feat_dynamic_real > 0:
             init_kwargs["dynamic_dims"] = [self.num_feat_dynamic_real]
         if self.num_past_feat_dynamic_real > 0:
             init_kwargs["past_dynamic_dims"] = [self.num_past_feat_dynamic_real]
         if self.num_feat_static_real > 0:
             init_kwargs["static_dims"] = [self.num_feat_static_real]
         if len(self.feat_static_cat_cardinality):
             init_kwargs["static_cardinalities"] = self.feat_static_cat_cardinality
         return init_kwargs
+
+
+class DLinearModel(AbstractGluonTSPyTorchModel):
+    """D-Linear model from GluonTS.
+
+    The model combines a moving window detrender with a multilayer perceptron (MLP) that predicts the distribution of
+    all the target value in the forecast horizon.
+
+    Based on `gluonts.torch.model.d_linear.DLinearEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.d_linear.html>`_.
+    See GluonTS documentation for additional hyperparameters.
+
+    References
+    ----------
+    .. [Zeng2023] Zeng, Ailing, et al.
+        "Are transformers effective for time series forecasting?"
+        AAAI Conference on Artificial Intelligence. 2023.
+
+    Other Parameters
+    ----------------
+    context_length : int, default = 96
+        Number of time units that condition the predictions
+    hidden_dimension: int, default = 20
+        Size of hidden layers in the feedforward network
+    distr_output : gluonts.torch.distributions.DistributionOutput, default = StudentTOutput()
+        Distribution to fit.
+    scaling : {"mean", "std", None}, default = "mean"
+        Scaling applied to the inputs. One of ``"mean"`` (mean absolute scaling), ``"std"`` (standardization), ``None`` (no scaling).
+    epochs : int, default = 100
+        Number of epochs the model will be trained for
+    batch_size : int, default = 64
+        Size of batches used during training
+    num_batches_per_epoch : int, default = 50
+        Number of batches processed every epoch
+    learning_rate : float, default = 1e-3,
+        Learning rate used during training
+    weight_decay : float, default = 1e-8
+        Weight decay regularization parameter.
+    """
+
+    gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator] = DLinearEstimator
+
+    @property
+    def default_context_length(self) -> int:
+        return 96
+
+
+class PatchTSTModel(AbstractGluonTSPyTorchModel):
+    """PatchTST model from GluonTS.
+
+    The model is based on a transformer that segments each time series into subseries-level patches.
+
+    Based on `gluonts.torch.model.d_linear.PatchTSTEstimator <https://ts.gluon.ai/stable/api/gluonts/gluonts.torch.model.patch_tst.html>`_.
+    See GluonTS documentation for additional hyperparameters.
+
+    References
+    ----------
+    .. [Nie2023] Nie, Yuqi, et al.
+        "A Time Series is Worth 64 Words: Long-term Forecasting with Transformers."
+        International Conference on Learning Representations. 2023.
+
+    Other Parameters
+    ----------------
+    context_length : int, default = 96
+        Number of time units that condition the predictions
+    patch_len : int, default = 16
+        Length of the patch.
+    stride : int, default = 8
+        Stride of the patch.
+    d_model : int, default = 32
+        Size of hidden layers in the Transformer encoder.
+    nhead : int, default = 4
+        Number of attention heads in the Transformer encoder which must divide d_model.
+    num_encoder_layers : int, default = 2
+        Number of layers in the Transformer encoder.
+    distr_output : gluonts.torch.distributions.DistributionOutput, default = StudentTOutput()
+        Distribution to fit.
+    scaling : {"mean", "std", None}, default = "mean"
+        Scaling applied to the inputs. One of ``"mean"`` (mean absolute scaling), ``"std"`` (standardization), ``None`` (no scaling).
+    epochs : int, default = 100
+        Number of epochs the model will be trained for
+    batch_size : int, default = 64
+        Size of batches used during training
+    num_batches_per_epoch : int, default = 50
+        Number of batches processed every epoch
+    learning_rate : float, default = 1e-3,
+        Learning rate used during training
+    weight_decay : float, default = 1e-8
+        Weight decay regularization parameter.
+    """
+
+    gluonts_estimator_class: Type[GluonTSPyTorchLightningEstimator] = PatchTSTEstimator
+
+    @property
+    def default_context_length(self) -> int:
+        return 96
+
+    def _get_estimator_init_args(self) -> Dict[str, Any]:
+        init_kwargs = super()._get_estimator_init_args()
+        init_kwargs.setdefault("patch_len", 16)
+        return init_kwargs
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/models/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 from . import (
     ARIMAModel,
     AutoARIMAModel,
     AutoETSModel,
     DeepARModel,
     DirectTabularModel,
+    DLinearModel,
     DynamicOptimizedThetaModel,
     ETSModel,
     NaiveModel,
+    PatchTSTModel,
     RecursiveTabularModel,
     SeasonalNaiveModel,
     SimpleFeedForwardModel,
     TemporalFusionTransformerModel,
     ThetaModel,
     ThetaStatsmodelsModel,
 )
@@ -31,14 +33,16 @@
 
 ModelHyperparameters = Dict[str, Any]
 
 # define the model zoo with their aliases
 MODEL_TYPES = dict(
     SimpleFeedForward=SimpleFeedForwardModel,
     DeepAR=DeepARModel,
+    DLinear=DLinearModel,
+    PatchTST=PatchTSTModel,
     TemporalFusionTransformer=TemporalFusionTransformerModel,
     RecursiveTabular=RecursiveTabularModel,
     DirectTabular=DirectTabularModel,
     Naive=NaiveModel,
     SeasonalNaive=SeasonalNaiveModel,
     AutoETS=AutoETSModel,
     AutoARIMA=AutoARIMAModel,
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,23 +200,18 @@
                     )
             else:
                 raise ValueError(
                     f"Please provide data in TimeSeriesDataFrame format (received an object of type {type(df)})."
                 )
         if self.ignore_time_index:
             df = df.get_reindexed_view(freq="S")
-        timestamps = df.reset_index(level=TIMESTAMP)[TIMESTAMP]
-        is_sorted = timestamps.groupby(level=ITEMID, sort=False).apply(lambda x: x.is_monotonic_increasing).all()
-        if not is_sorted:
-            warnings.warn(
-                "Provided data contains timestamps that are not sorted chronologically. "
-                "This will lead to TimeSeriesPredictor not working as intended. "
-                "Please make sure that the timestamps are sorted in increasing order for all time series."
-            )
-        # TODO: Make sure that entries for each item_id are contiguous -> https://github.com/autogluon/autogluon/issues/3036
+        # MultiIndex.is_monotonic_increasing checks if index is sorted by ["item_id", "timestamp"]
+        if not df.index.is_monotonic_increasing:
+            df = df.sort_index()
+            df._cached_freq = None  # in case frequency was incorrectly cached as IRREGULAR_TIME_INDEX_FREQSTR
         if df.freq is None:
             raise ValueError(
                 "Frequency not provided and cannot be inferred. This is often due to the "
                 "time index of the data being irregularly sampled. Please ensure that the "
                 "data set used has a uniform time index, or create the `TimeSeriesPredictor` "
                 "setting `ignore_time_index=True`."
             )
@@ -619,16 +614,19 @@
         A       2020-01-08    30.2
                 2020-01-09    27.0
         B       2020-03-04    17.1
                 2020-03-05     8.3
         """
         if random_seed is not None:
             set_random_seed(random_seed)
+        # Don't use data.item_ids in case data is not a TimeSeriesDataFrame
+        original_item_id_order = data.reset_index()[ITEMID].unique()
         data = self._check_and_prepare_data_frame(data)
-        return self._learner.predict(data, known_covariates=known_covariates, model=model)
+        predictions = self._learner.predict(data, known_covariates=known_covariates, model=model)
+        return predictions.reindex(original_item_id_order, level=ITEMID)
 
     def evaluate(self, data: Union[TimeSeriesDataFrame, pd.DataFrame], **kwargs):
         """Evaluate the performance for given dataset, computing the score determined by ``self.eval_metric``
         on the given data set, and with the same ``prediction_length`` used when training models.
 
         Parameters
         ----------
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230526/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230525/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230526/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*


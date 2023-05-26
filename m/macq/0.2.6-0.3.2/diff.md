# Comparing `tmp/macq-0.2.6.tar.gz` & `tmp/macq-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macq-0.2.6.tar", last modified: Tue Jun  7 04:09:24 2022, max compression
+gzip compressed data, was "macq-0.3.2.tar", last modified: Fri May 26 19:44:29 2023, max compression
```

## Comparing `macq-0.2.6.tar` & `macq-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.798223 macq-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-07 04:09:13.000000 macq-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-06-07 04:09:24.798223 macq-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-06-07 04:09:13.000000 macq-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.794223 macq-0.2.6/macq/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-07 04:09:13.000000 macq-0.2.6/macq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.794223 macq-0.2.6/macq/extract/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30726 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/amdn.py
--rw-r--r--   0 runner    (1001) docker     (121)    37842 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/arms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/learned_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/learned_fluent.py
--rw-r--r--   0 runner    (1001) docker     (121)     7685 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5147 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/observer.py
--rw-r--r--   0 runner    (1001) docker     (121)    22703 2022-06-07 04:09:13.000000 macq-0.2.6/macq/extract/slaf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.794223 macq-0.2.6/macq/generate/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2249 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/csv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.794223 macq-0.2.6/macq/generate/pddl/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4022 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/fd_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (121)    18029 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9195 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/planning_domains_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9454 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/random_goal_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/trace_from_goal.py
--rw-r--r--   0 runner    (1001) docker     (121)     5513 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/pddl/vanilla_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-06-07 04:09:13.000000 macq-0.2.6/macq/generate/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.798223 macq-0.2.6/macq/observation/
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/atomic_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/id_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/identity_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/noisy_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/noisy_partial_disordered_parallel_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/noisy_partial_observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/observation.py
--rw-r--r--   0 runner    (1001) docker     (121)    10196 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     3812 2022-06-07 04:09:13.000000 macq-0.2.6/macq/observation/partial_observation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.798223 macq-0.2.6/macq/trace/
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3095 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/action.py
--rw-r--r--   0 runner    (1001) docker     (121)    13669 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/disordered_parallel_actions_observation_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/fluent.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/partial_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/step.py
--rw-r--r--   0 runner    (1001) docker     (121)    11321 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     5206 2022-06-07 04:09:13.000000 macq-0.2.6/macq/trace/trace_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.798223 macq-0.2.6/macq/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/common_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/complex_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/pysat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/tokenization_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/tokenization_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/trace_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-06-07 04:09:13.000000 macq-0.2.6/macq/utils/trace_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 04:09:24.794223 macq-0.2.6/macq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-06-07 04:09:24.000000 macq-0.2.6/macq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-06-07 04:09:24.000000 macq-0.2.6/macq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 04:09:24.000000 macq-0.2.6/macq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-07 04:09:24.000000 macq-0.2.6/macq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-07 04:09:24.000000 macq-0.2.6/macq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-06-07 04:09:13.000000 macq-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 04:09:24.798223 macq-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-06-07 04:09:13.000000 macq-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 19:43:50.000000 macq-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-26 19:44:29.606325 macq-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-26 19:43:50.000000 macq-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.586324 macq-0.3.2/macq/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 19:43:50.000000 macq-0.3.2/macq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31307 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/amdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38083 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/learned_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/learned_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31604 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/locm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-05-26 19:43:50.000000 macq-0.3.2/macq/extract/slaf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.594325 macq-0.3.2/macq/generate/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/fd_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/planning_domains_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/random_goal_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/trace_from_goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/pddl/vanilla_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 19:43:50.000000 macq-0.3.2/macq/generate/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.598325 macq-0.3.2/macq/observation/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/action_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/atomic_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/id_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/identity_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_partial_disordered_parallel_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/noisy_partial_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/observed_tracelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-26 19:43:50.000000 macq-0.3.2/macq/observation/partial_observation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.602325 macq-0.3.2/macq/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/disordered_parallel_actions_observation_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/partial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-26 19:43:50.000000 macq-0.3.2/macq/trace/trace_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/macq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/complex_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/pysat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/tokenization_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/tokenization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/trace_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 19:43:50.000000 macq-0.3.2/macq/utils/trace_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.590324 macq-0.3.2/macq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 19:44:29.000000 macq-0.3.2/macq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 19:43:50.000000 macq-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:44:29.606325 macq-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-26 19:43:50.000000 macq-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:44:29.606325 macq-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 19:43:50.000000 macq-0.3.2/tests/test_readme.py
```

### Comparing `macq-0.2.6/LICENSE` & `macq-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/PKG-INFO` & `macq-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.2.6
+Version: 0.3.2
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
@@ -40,16 +40,16 @@
 
 # get a domain-specific generator: uses api.planning.domains problem_id/
 # generate 100 traces of length 20 using vanilla sampling
 traces = generate.pddl.VanillaSampling(problem_id = 123, plan_len = 20, num_traces = 100).traces
 
 traces.generate_more(10)
 
-action1 = traces[0][0].action
-traces.get_usage(action1)
+action = traces[0][0].action
+traces.get_usage(action)
 [0.05, 0.05, ..., 0.05]
 
 trace = traces[0]
 len(trace)
 20
 
 trace.fluents
```

### Comparing `macq-0.2.6/README.md` & `macq-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 # get a domain-specific generator: uses api.planning.domains problem_id/
 # generate 100 traces of length 20 using vanilla sampling
 traces = generate.pddl.VanillaSampling(problem_id = 123, plan_len = 20, num_traces = 100).traces
 
 traces.generate_more(10)
 
-action1 = traces[0][0].action
-traces.get_usage(action1)
+action = traces[0][0].action
+traces.get_usage(action)
 [0.05, 0.05, ..., 0.05]
 
 trace = traces[0]
 len(trace)
 20
 
 trace.fluents
```

### Comparing `macq-0.2.6/macq/extract/amdn.py` & `macq-0.3.2/macq/extract/amdn.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from nnf import Aux, Var, And, Or
 from bauhaus import Encoding  # only used for pretty printing in debug mode
 from .exceptions import (
     IncompatibleObservationToken,
 )
 from .model import Model
 from ..trace import ActionPair
-from ..observation import NoisyPartialDisorderedParallelObservation, ObservationLists
+from ..observation import NoisyPartialDisorderedParallelObservation, ObservedTraceList
 from ..utils.pysat import to_wcnf, extract_raw_model
 
 e = Encoding
 
 
 def pre(r: Fluent, act: Action):
     """Create a Var that enforces that the given fluent is a precondition of the given action.
@@ -62,56 +62,59 @@
 
 
 WMAX = 1
 
 
 class AMDN:
     def __new__(
-        cls, obs_lists: ObservationLists, debug: bool = False, occ_threshold: int = 1
+        cls,
+        obs_tracelist: ObservedTraceList,
+        debug: bool = False,
+        occ_threshold: int = 1,
     ):
         """Creates a new Model object.
 
         Args:
-            obs_lists (ObservationList):
+            obs_tracelist (ObservationList):
                 The state observations to extract the model from.
             debug (bool):
                 Optional debugging mode.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
 
         Raises:
             IncompatibleObservationToken:
                 Raised if the observations are not identity observation.
         """
-        if obs_lists.type is not NoisyPartialDisorderedParallelObservation:
-            raise IncompatibleObservationToken(obs_lists.type, AMDN)
+        if obs_tracelist.type is not NoisyPartialDisorderedParallelObservation:
+            raise IncompatibleObservationToken(obs_tracelist.type, AMDN)
 
-        return AMDN._amdn(obs_lists, debug, occ_threshold)
+        return AMDN._amdn(obs_tracelist, debug, occ_threshold)
 
     @staticmethod
-    def _amdn(obs_lists: ObservationLists, debug: bool, occ_threshold: int):
+    def _amdn(obs_tracelist: ObservedTraceList, debug: bool, occ_threshold: int):
         """Main driver for the entire AMDN algorithm.
         The first line contains steps 1-4.
         The second line contains step 5.
         Finally, the final line corresponds to step 6 (return the model).
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be fed into the algorithm.
             debug (bool):
                 Optional debugging mode.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
 
         Returns:
             The extracted `Model`.
         """
-        wcnf, decode = AMDN._solve_constraints(obs_lists, occ_threshold, debug)
+        wcnf, decode = AMDN._solve_constraints(obs_tracelist, occ_threshold, debug)
         raw_model = extract_raw_model(wcnf, decode)
-        return AMDN._extract_model(obs_lists, raw_model)
+        return AMDN._extract_model(obs_tracelist, raw_model)
 
     @staticmethod
     def _or_refactor(maybe_lit: Union[Or, Var]):
         """Converts a "Var" fluent to an "Or" fluent.
 
         Args:
             maybe_lit (Union[Or, Var]):
@@ -144,26 +147,26 @@
                 if isinstance(var.name, Aux) and var.true:
                     # aux variables are the soft clauses that get the original weight
                     constraints[AMDN._or_refactor(var)] = prob_disordered * WMAX
             # set each original constraint to be a hard clause
             constraints[clause] = "HARD"
 
     @staticmethod
-    def _get_observe(obs_lists: ObservationLists):
+    def _get_observe(obs_tracelist: ObservedTraceList):
         """Gets from the user which fluents they want to observe (for debug mode).
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that contain the fluents.
 
         Returns:
             A list of of which fluents the user wants to observe.
         """
         print("Select a proposition to observe:")
-        sorted_f = [str(f) for f in obs_lists.propositions]
+        sorted_f = [str(f) for f in obs_tracelist.propositions]
         sorted_f.sort()
         for f in sorted_f:
             print(f)
         to_obs = []
         user_input = ""
         while user_input != "x":
             user_input = input(
@@ -255,47 +258,47 @@
                     if aux == child.name:
                         e.pprint(e, v)
                         print(constraints[c])
                         break
             print()
 
     @staticmethod
-    def _build_disorder_constraints(obs_lists: ObservationLists):
+    def _build_disorder_constraints(obs_tracelist: ObservedTraceList):
         """Builds disorder constraints. Corresponds to step 1 of the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be analyzed.
 
         Returns:
             The disorder constraints to be used in the algorithm.
         """
         disorder_constraints = {}
 
         # iterate through all traces
-        for i in range(len(obs_lists.all_par_act_sets)):
+        for i in range(len(obs_tracelist.all_par_act_sets)):
             # get the parallel action sets for this trace
-            par_act_sets = obs_lists.all_par_act_sets[i]
+            par_act_sets = obs_tracelist.all_par_act_sets[i]
             # iterate through all pairs of parallel action sets for this trace
             # use -1 since we will be referencing the current parallel action set and the following one
             for j in range(len(par_act_sets) - 1):
                 # for each action in psi_i+1
                 for act_y in par_act_sets[j + 1]:
                     # for each action in psi_i
                     # NOTE: we do not use an existential here, as the paper describes (for each act_y in psi_i + 1,
                     # there exists an act_x in psi_i such that the condition holds.)
                     # this is due to the fact that the weights must be set for each action pair.
                     for act_x in par_act_sets[j]:
                         if act_x != act_y:
                             # calculate the probability of the actions being disordered (p)
-                            p = obs_lists.probabilities[ActionPair({act_x, act_y})]
+                            p = obs_tracelist.probabilities[ActionPair({act_x, act_y})]
                             # each constraint only needs to hold for one proposition to be true
                             constraint_1 = []
                             constraint_2 = []
-                            for r in obs_lists.propositions:
+                            for r in obs_tracelist.propositions:
                                 constraint_1.append(
                                     Or(
                                         [
                                             And(
                                                 [
                                                     pre(r, act_x),
                                                     ~delete(r, act_x),
@@ -331,178 +334,184 @@
                             )
                             AMDN._extract_aux_set_weights(
                                 disjunct_all_constr_2, disorder_constraints, p
                             )
         return disorder_constraints
 
     @staticmethod
-    def _build_hard_parallel_constraints(obs_lists: ObservationLists):
+    def _build_hard_parallel_constraints(obs_tracelist: ObservedTraceList):
         """Builds hard parallel constraints.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be analyzed.
 
         Returns:
             The hard parallel constraints to be used in the algorithm.
         """
         hard_constraints = {}
         # create a list of all <a, r> tuples
-        for act in obs_lists.actions:
-            for r in obs_lists.propositions:
+        for act in obs_tracelist.actions:
+            for r in obs_tracelist.propositions:
                 # for each action x proposition pair, enforce the two hard constraints with weight wmax
                 hard_constraints[implies(add(r, act), ~pre(r, act))] = WMAX
                 hard_constraints[implies(delete(r, act), pre(r, act))] = WMAX
         return hard_constraints
 
     @staticmethod
-    def _build_soft_parallel_constraints(obs_lists: ObservationLists):
+    def _build_soft_parallel_constraints(obs_tracelist: ObservedTraceList):
         """Builds soft parallel constraints.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be analyzed.
 
         Returns:
             The soft parallel constraints to be used in the algorithm.
         """
         soft_constraints = {}
 
         # NOTE: the paper does not take into account possible conflicts between the preconditions of actions
         # and the add/delete effects of other actions (similar to the hard constraints, but with other actions
         # in the parallel action set).
 
         # iterate through all traces
-        for i in range(len(obs_lists.all_par_act_sets)):
-            par_act_sets = obs_lists.all_par_act_sets[i]
+        for i in range(len(obs_tracelist.all_par_act_sets)):
+            par_act_sets = obs_tracelist.all_par_act_sets[i]
             # iterate through all parallel action sets for this trace
             for j in range(len(par_act_sets)):
                 # within each parallel action set, iterate through the same action set again to compare
                 # each action to every other action in the set; setting constraints assuming actions are not disordered
                 for act_x in par_act_sets[j]:
                     for act_x_prime in par_act_sets[j] - {act_x}:
-                        p = obs_lists.probabilities[ActionPair({act_x, act_x_prime})]
+                        p = obs_tracelist.probabilities[
+                            ActionPair({act_x, act_x_prime})
+                        ]
                         # iterate through all propositions
-                        for r in obs_lists.propositions:
+                        for r in obs_tracelist.propositions:
                             soft_constraints[
                                 implies(add(r, act_x), ~delete(r, act_x_prime))
                             ] = (1 - p) * WMAX
 
         # iterate through all traces
-        for i in range(len(obs_lists.all_par_act_sets)):
-            par_act_sets = obs_lists.all_par_act_sets[i]
+        for i in range(len(obs_tracelist.all_par_act_sets)):
+            par_act_sets = obs_tracelist.all_par_act_sets[i]
             # then, iterate through all pairs of parallel action sets for each trace
             for j in range(len(par_act_sets) - 1):
                 # for each pair, compare every action in act_y to every action in act_x_prime; setting constraints assuming actions are disordered
                 for act_y in par_act_sets[j + 1]:
                     for act_x_prime in par_act_sets[j] - {act_y}:
-                        p = obs_lists.probabilities[ActionPair({act_y, act_x_prime})]
+                        p = obs_tracelist.probabilities[
+                            ActionPair({act_y, act_x_prime})
+                        ]
                         # iterate through all propositions and similarly set the constraint
-                        for r in obs_lists.propositions:
+                        for r in obs_tracelist.propositions:
                             soft_constraints[
                                 implies(add(r, act_y), ~delete(r, act_x_prime))
                             ] = (p * WMAX)
 
         return soft_constraints
 
     @staticmethod
     def _build_parallel_constraints(
-        obs_lists: ObservationLists, debug: bool, to_obs: Optional[List[str]]
+        obs_tracelist: ObservedTraceList, debug: bool, to_obs: Optional[List[str]]
     ):
         """Main driver for building parallel constraints. Corresponds to step 2 of the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             debug (bool):
                 Optional debugging mode.
             to_obs (Optional[List[str]]):
                 If in the optional debugging mode, the list of fluents to observe.
 
         Returns:
             The parallel constraints.
         """
-        hard_constraints = AMDN._build_hard_parallel_constraints(obs_lists)
-        soft_constraints = AMDN._build_soft_parallel_constraints(obs_lists)
+        hard_constraints = AMDN._build_hard_parallel_constraints(obs_tracelist)
+        soft_constraints = AMDN._build_soft_parallel_constraints(obs_tracelist)
         if debug:
             print("\nHard parallel constraints:")
             AMDN._debug_simple_pprint(hard_constraints, to_obs)
             print("\nSoft parallel constraints:")
             AMDN._debug_simple_pprint(soft_constraints, to_obs)
         return {**hard_constraints, **soft_constraints}
 
     @staticmethod
-    def _calculate_all_r_occ(obs_lists: ObservationLists):
+    def _calculate_all_r_occ(obs_tracelist: ObservedTraceList):
         """Calculates the total number of (true) propositions in the provided traces/tokens.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be analyzed.
 
         Returns:
             The total number of (true) propositions in the provided traces/tokens.
         """
         # tracks occurrences of all propositions
         all_occ = 0
-        for trace in obs_lists:
+        for trace in obs_tracelist:
             for step in trace:
                 all_occ += len([f for f in step.state if step.state[f]])
         return all_occ
 
     @staticmethod
-    def _set_up_occurrences_dict(obs_lists: ObservationLists):
+    def _set_up_occurrences_dict(obs_tracelist: ObservedTraceList):
         """Helper function used when constructing noise constraints.
         Sets up an "occurrence" dictionary used to track the occurrences of propositions
         before or after actions.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens to be analyzed.
 
         Returns:
             The blank "occurrences" dictionary.
         """
         # set up dict
         occurrences = {}
-        for a in obs_lists.actions:
+        for a in obs_tracelist.actions:
             occurrences[a] = {}
-            for r in obs_lists.propositions:
+            for r in obs_tracelist.propositions:
                 occurrences[a][r] = 0
         return occurrences
 
     @staticmethod
     def _noise_constraints_6(
-        obs_lists: ObservationLists, all_occ: int, occ_threshold: int
+        obs_tracelist: ObservedTraceList, all_occ: int, occ_threshold: int
     ):
         """Noise constraints (6) in the AMDN paper.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             all_occ (int):
                 The number of occurrences of all (true) propositions in the given observation list.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
 
         Returns:
             The noise constraints.
         """
         noise_constraints_6 = {}
-        occurrences = AMDN._set_up_occurrences_dict(obs_lists)
+        occurrences = AMDN._set_up_occurrences_dict(obs_tracelist)
 
         # iterate over ALL the plan traces, adding occurrences accordingly
-        for i in range(len(obs_lists)):
+        for i in range(len(obs_tracelist)):
             # iterate through each step in each trace, omitting the last step because the last action is None/we access the state in the next step
-            for j in range(len(obs_lists[i]) - 1):
+            for j in range(len(obs_tracelist[i]) - 1):
                 true_prop = [
-                    f for f in obs_lists[i][j + 1].state if obs_lists[i][j + 1].state[f]
+                    f
+                    for f in obs_tracelist[i][j + 1].state
+                    if obs_tracelist[i][j + 1].state[f]
                 ]
                 for r in true_prop:
                     # count the number of occurrences of each action and its following proposition
-                    occurrences[obs_lists[i][j].action][r] += 1
+                    occurrences[obs_tracelist[i][j].action][r] += 1
 
         # iterate through actions
         for a in occurrences:
             # iterate through all propositions for this action
             for r in occurrences[a]:
                 occ_r = occurrences[a][r]
                 # if the # of occurrences is higher than the user-provided threshold:
@@ -510,84 +519,86 @@
                     # set constraint 6 with the calculated weight
                     noise_constraints_6[AMDN._or_refactor(~delete(r, a))] = (
                         occ_r / all_occ
                     ) * WMAX
         return noise_constraints_6
 
     @staticmethod
-    def _noise_constraints_7(obs_lists: ObservationLists, all_occ: int):
+    def _noise_constraints_7(obs_tracelist: ObservedTraceList, all_occ: int):
         """Noise constraints (7) in the AMDN paper.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             all_occ (int):
                 The number of occurrences of all (true) propositions in the given observation list.
 
         Returns:
             The noise constraints.
         """
         noise_constraints_7 = {}
         # set up dict
         occurrences = {}
-        for r in obs_lists.propositions:
+        for r in obs_tracelist.propositions:
             occurrences[r] = 0
 
-        for trace in obs_lists.all_states:
+        for trace in obs_tracelist.all_states:
             for state in trace:
                 true_prop = [r for r in state if state[r]]
                 for r in true_prop:
                     occurrences[r] += 1
 
         # iterate through all traces
-        for i in range(len(obs_lists.all_par_act_sets)):
+        for i in range(len(obs_tracelist.all_par_act_sets)):
             # get the next trace/states
-            par_act_sets = obs_lists.all_par_act_sets[i]
-            states = obs_lists.all_states[i]
+            par_act_sets = obs_tracelist.all_par_act_sets[i]
+            states = obs_tracelist.all_states[i]
             # iterate through all parallel action sets within the trace
             for j in range(len(par_act_sets)):
                 # examine the states before and after each parallel action set; set constraints accordinglly
                 true_prop = [r for r in states[j + 1] if states[j + 1][r]]
                 for r in true_prop:
                     if not states[j][r]:
                         noise_constraints_7[
                             Or([add(r, act) for act in par_act_sets[j]])
                         ] = (occurrences[r] / all_occ) * WMAX
         return noise_constraints_7
 
     @staticmethod
-    def _noise_constraints_8(obs_lists, all_occ: int, occ_threshold: int):
+    def _noise_constraints_8(obs_tracelist, all_occ: int, occ_threshold: int):
         """Noise constraints (8) in the AMDN paper.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             all_occ (int):
                 The number of occurrences of all (true) propositions in the given observation list.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
 
         Returns:
             The noise constraints.
         """
         noise_constraints_8 = {}
-        occurrences = AMDN._set_up_occurrences_dict(obs_lists)
+        occurrences = AMDN._set_up_occurrences_dict(obs_tracelist)
 
         # iterate over ALL the plan traces, adding occurrences accordingly
-        for i in range(len(obs_lists)):
+        for i in range(len(obs_tracelist)):
             # iterate through each step in each trace
-            for j in range(len(obs_lists[i])):
+            for j in range(len(obs_tracelist[i])):
                 # if the action is not None
-                if obs_lists[i][j].action:
+                if obs_tracelist[i][j].action:
                     true_prop = [
-                        f for f in obs_lists[i][j].state if obs_lists[i][j].state[f]
+                        f
+                        for f in obs_tracelist[i][j].state
+                        if obs_tracelist[i][j].state[f]
                     ]
                     for r in true_prop:
                         # count the number of occurrences of each action and its previous proposition
-                        occurrences[obs_lists[i][j].action][r] += 1
+                        occurrences[obs_tracelist[i][j].action][r] += 1
 
         # iterate through actions
         for a in occurrences:
             # iterate through all propositions for this action
             for r in occurrences[a]:
                 occ_r = occurrences[a][r]
                 # if the # of occurrences is higher than the user-provided threshold:
@@ -596,96 +607,96 @@
                     noise_constraints_8[AMDN._or_refactor(pre(r, a))] = (
                         occ_r / all_occ
                     ) * WMAX
         return noise_constraints_8
 
     @staticmethod
     def _build_noise_constraints(
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         occ_threshold: int,
         debug: bool,
         to_obs: Optional[List[str]],
     ):
         """Driver for building all noise constraints. Corresponds to step 3 of the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
             debug (bool):
                 Optional debugging mode.
             to_obs (Optional[List[str]]):
                 If in the optional debugging mode, the list of fluents to observe.
         """
         # calculate all occurrences for use in weights
-        all_occ = AMDN._calculate_all_r_occ(obs_lists)
-        nc_6 = AMDN._noise_constraints_6(obs_lists, all_occ, occ_threshold)
-        nc_7 = AMDN._noise_constraints_7(obs_lists, all_occ)
-        nc_8 = AMDN._noise_constraints_8(obs_lists, all_occ, occ_threshold)
+        all_occ = AMDN._calculate_all_r_occ(obs_tracelist)
+        nc_6 = AMDN._noise_constraints_6(obs_tracelist, all_occ, occ_threshold)
+        nc_7 = AMDN._noise_constraints_7(obs_tracelist, all_occ)
+        nc_8 = AMDN._noise_constraints_8(obs_tracelist, all_occ, occ_threshold)
         if debug:
             print("\nNoise constraints 6:")
             AMDN._debug_simple_pprint(nc_6, to_obs)
             print("\nNoise constraints 7:")
             AMDN._debug_simple_pprint(nc_7, to_obs)
             print("\nNoise constraints 8:")
             AMDN._debug_simple_pprint(nc_8, to_obs)
         return {**nc_6, **nc_7, **nc_8}
 
     @staticmethod
     def _set_all_constraints(
-        obs_lists: ObservationLists, occ_threshold: int, debug: bool
+        obs_tracelist: ObservedTraceList, occ_threshold: int, debug: bool
     ):
         """Main driver for generating all constraints in the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
             debug (bool):
                 Optional debugging mode.
 
         Returns:
             A dictionary that constains all of the constraints set and all of their weights.
         """
         to_obs = None
         if debug:
-            to_obs = AMDN._get_observe(obs_lists)
-        disorder_constraints = AMDN._build_disorder_constraints(obs_lists)
+            to_obs = AMDN._get_observe(obs_tracelist)
+        disorder_constraints = AMDN._build_disorder_constraints(obs_tracelist)
         if debug:
             print("\nDisorder constraints:")
             AMDN._debug_aux_pprint(disorder_constraints, to_obs)
         parallel_constraints = AMDN._build_parallel_constraints(
-            obs_lists, debug, to_obs
+            obs_tracelist, debug, to_obs
         )
         noise_constraints = AMDN._build_noise_constraints(
-            obs_lists, occ_threshold, debug, to_obs
+            obs_tracelist, occ_threshold, debug, to_obs
         )
         return {**disorder_constraints, **parallel_constraints, **noise_constraints}
 
     @staticmethod
     def _solve_constraints(
-        obs_lists: ObservationLists, occ_threshold: int, debug: bool
+        obs_tracelist: ObservedTraceList, occ_threshold: int, debug: bool
     ):
         """Returns the WCNF and the decoder according to the constraints generated.
         Corresponds to step 4 of the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             occ_threshold (int):
                 Threshold to be used for noise constraints.
             debug (bool):
                 Optional debugging mode.
 
         Returns:
             The WCNF and corresponding decode dictionary.
         """
-        constraints = AMDN._set_all_constraints(obs_lists, occ_threshold, debug)
+        constraints = AMDN._set_all_constraints(obs_tracelist, occ_threshold, debug)
         # extract hard constraints
         hard_constraints = []
         for c, weight in constraints.items():
             if weight == "HARD":
                 hard_constraints.append(c)
         for c in hard_constraints:
             del constraints[c]
@@ -719,32 +730,32 @@
             f, act = raw_f.split(add_str)
             learned_actions[act].update_add({f})
         else:
             f, act = raw_f.split(del_str)
             learned_actions[act].update_delete({f})
 
     @staticmethod
-    def _extract_model(obs_lists: ObservationLists, model: Dict[Hashable, bool]):
+    def _extract_model(obs_tracelist: ObservedTraceList, model: Dict[Hashable, bool]):
         """Converts a raw model generated from the pysat module into a macq `Model`.
         Corresponds to step 5 of the AMDN algorithm.
 
         Args:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The tokens that were analyzed.
             model (Dict[Hashable, bool]):
                 The raw model to parse and analyze.
 
         Returns:
             The macq action `Model`.
         """
         # convert the result to a Model
-        fluents = obs_lists.propositions
+        fluents = obs_tracelist.propositions
         # set up LearnedActions
         learned_actions = {}
-        for a in obs_lists.actions:
+        for a in obs_tracelist.actions:
             # set up a base LearnedAction with the known information
             learned_actions[a.details()] = extract.LearnedAction(
                 a.name, a.obj_params, cost=a.cost
             )
         # iterate through all fluents
         for raw_f in model:
             # update learned_actions (ignore auxiliary variables)
```

### Comparing `macq-0.2.6/macq/extract/arms.py` & `macq-0.3.2/macq/extract/arms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """.. include:: ../../docs/templates/extract/arms.md"""
 
-from collections import defaultdict, Counter
+from collections import Counter, defaultdict
 from dataclasses import dataclass
+from typing import Dict, Hashable, List, Set, Tuple
 from warnings import warn
-from typing import Set, List, Dict, Tuple, Hashable
-from nnf import Var, And, Or, false as nnffalse
-from . import LearnedAction, Model, LearnedFluent
-from .exceptions import (
-    IncompatibleObservationToken,
-    InvalidMaxSATModel,
-)
-from ..observation import PartialObservation as Observation, ObservationLists
-from ..trace import Fluent, Action  # Action only used for typing
-from ..utils.pysat import to_wcnf, RC2, WCNF
+
+from nnf import And, Or, Var
+from nnf import false as nnffalse
+
+from ..observation import Observation, ObservedTraceList, PartialObservation
+from ..trace import Action, Fluent
+from ..utils.pysat import RC2, WCNF, to_wcnf
+from . import LearnedAction, LearnedFluent, Model
+from .exceptions import IncompatibleObservationToken, InvalidMaxSATModel
 
 
 @dataclass
 class Relation:
     """Fluents with the parameters replaced by their types."""
 
     name: str
@@ -61,27 +61,27 @@
         def __init__(self, threshold):
             super().__init__(
                 f"Invalid threshold value: {threshold}. Threshold must be a float between 0-1 (inclusive)."
             )
 
     def __new__(
         cls,
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         debug: bool,
         upper_bound: int,
         min_support: int = 2,
         action_weight: int = 110,
         info_weight: int = 100,
         threshold: float = 0.6,
         info3_default: int = 30,
         plan_default: int = 30,
     ):
         """
         Arguments:
-            obs_lists (ObservationLists):
+            obs_tracelist (ObservationLists):
                 The observations to extract the model from.
             upper_bound (int):
                 The upper bound for the maximum size of an action's preconditions and
                 add/delete lists. Determines when an action schemata is fully learned.
             min_support (int):
                 The minimum support count for an action pair to be considered frequent.
             action_weight (int):
@@ -94,25 +94,25 @@
                 (0-1). The probability threshold θ to determine if an I3/plan constraint
                 is weighted by its probability or set to a default value.
             info3_default (int):
                 The default weight for I3 constraints with probability below the threshold.
             plan_default (int):
                 The default weight for plan constraints with probability below the threshold.
         """
-        if obs_lists.type is not Observation:
-            raise IncompatibleObservationToken(obs_lists.type, ARMS)
+        if obs_tracelist.type is not PartialObservation:
+            raise IncompatibleObservationToken(obs_tracelist.type, ARMS)
 
         if not (threshold >= 0 and threshold <= 1):
             raise ARMS.InvalidThreshold(threshold)
 
-        fluents = obs_lists.get_fluents()
+        fluents = obs_tracelist.get_fluents()
         # get fluents from initial state
         # call algorithm to get actions
         actions = ARMS._arms(
-            obs_lists,
+            obs_tracelist,
             upper_bound,
             fluents,
             min_support,
             action_weight,
             info_weight,
             threshold,
             info3_default,
@@ -130,32 +130,32 @@
             learned_fluents.update(act.precond)
             learned_fluents.update(act.add)
             learned_fluents.update(act.delete)
         return Model(learned_fluents, actions)
 
     @staticmethod
     def _arms(
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         upper_bound: int,
         fluents: Set[Fluent],
         min_support: int,
         action_weight: int,
         info_weight: int,
         threshold: float,
         info3_default: int,
         plan_default: int,
         debug: bool,
     ) -> Set[LearnedAction]:
         """The main driver for the ARMS algorithm."""
         learned_actions = set()  # The set of learned action models Θ
         # pointers to the earliest unlearned action for each observation list
-        early_actions = [0] * len(obs_lists)
+        early_actions = [0] * len(obs_tracelist)
 
         debug1 = ARMS.debug_menu("Debug step 1?") if debug else False
-        connected_actions, action_map = ARMS.step1(obs_lists, debug1)
+        connected_actions, action_map = ARMS.step1(obs_tracelist, debug1)
         if debug1:
             input("Press enter to continue...")
 
         action_map_rev: Dict[LearnedAction, List[Action]] = defaultdict(list)
         for obs_action, learned_action in action_map.items():
             action_map_rev[learned_action].append(obs_action)
 
@@ -163,15 +163,20 @@
         while action_map_rev:
             if debug:
                 print("Iteration", count)
                 count += 1
 
             debug2 = ARMS.debug_menu("Debug step 2?") if debug else False
             constraints, relation_map = ARMS.step2(
-                obs_lists, connected_actions, action_map, fluents, min_support, debug2
+                obs_tracelist,
+                connected_actions,
+                action_map,
+                fluents,
+                min_support,
+                debug2,
             )
             if debug2:
                 input("Press enter to continue...")
 
             relation_map_rev: Dict[Relation, List[Fluent]] = defaultdict(list)
             for fluent, relation in relation_map.items():
                 relation_map_rev[relation].append(fluent)
@@ -200,36 +205,38 @@
             )
 
             # Step 5 updates
 
             # Progress observed states if early actions have been learned
             setA = set()
             for action in action_map_rev.keys():
-                for i, obs_list in enumerate(obs_lists):
-                    obs_action: Action = obs_list[early_actions[i]].action
-                    # if current action is the early action for obs_list i,
+                for i, obs_trace in enumerate(obs_tracelist):
+                    obs_action: Action = obs_trace[early_actions[i]].action
+                    # if current action is the early action for obs_trace i,
                     # update the next state with the effects and update the
                     # early action pointer
                     if obs_action in action_map and action == action_map[obs_action]:
                         print()
                         # Set add effects true
                         for add in action.add:
                             # get candidate fluents from add relation
-                            # get fluent by cross referencing obs_list.action params
+                            # get fluent by cross referencing obs_trace.action params
                             candidates = relation_map_rev[add]
                             for fluent in candidates:
                                 if set(fluent.objects).issubset(obs_action.obj_params):
-                                    obs_list[early_actions[i] + 1].state[fluent] = True
+                                    obs_trace[early_actions[i] + 1].state[fluent] = True
                                     early_actions[i] += 1
                         # Set del effects false
                         for delete in action.delete:
                             candidates = relation_map_rev[delete]
                             for fluent in candidates:
                                 if set(fluent.objects).issubset(obs_action.obj_params):
-                                    obs_list[early_actions[i] + 1].state[fluent] = False
+                                    obs_trace[early_actions[i] + 1].state[
+                                        fluent
+                                    ] = False
                                     early_actions[i] += 1
 
                 if debug:
                     print()
                     print(action.details())
                     print("precond:", action.precond)
                     print("add:", action.add)
@@ -264,24 +271,24 @@
             if debug5:
                 input("Press enter to continue...")
 
         return learned_actions
 
     @staticmethod
     def step1(
-        obs_lists: ObservationLists, debug: bool
+        obs_tracelist: ObservedTraceList, debug: bool
     ) -> Tuple[
         Dict[LearnedAction, Dict[LearnedAction, Set[str]]],
         Dict[Action, LearnedAction],
     ]:
         """(Step 1) Substitute instantiated objects in each action instance with the object type."""
 
         learned_actions: Set[LearnedAction] = set()
         action_map: Dict[Action, LearnedAction] = {}
-        for obs_action in obs_lists.get_actions():
+        for obs_action in obs_tracelist.get_actions():
             # We don't support objects with multiple types right now, so no
             # multiple type clauses need to be generated.
 
             # Create LearnedActions for each action, replacing instantiated
             # objects with the object type.
             types = [obj.obj_type for obj in obs_action.obj_params]
             learned_action = LearnedAction(obs_action.name, types)
@@ -300,15 +307,15 @@
                             f"{a1.details()} is connected to {a2.details()} by {intersection}"
                         )
 
         return connected_actions, action_map
 
     @staticmethod
     def step2(
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         connected_actions: Dict[LearnedAction, Dict[LearnedAction, Set[str]]],
         action_map: Dict[Action, LearnedAction],
         fluents: Set[Fluent],
         min_support: int,
         debug: bool,
     ) -> Tuple[ARMSConstraints, Dict[Fluent, Relation]]:
         """(Step 2) Generate action constraints, information constraints, and plan constraints.
@@ -339,20 +346,20 @@
 
         action_constraints = ARMS.step2A(
             connected_actions, set(relations.values()), debuga
         )
 
         debugi = ARMS.debug_menu("Debug info constraints?") if debug else False
         info_constraints, info_support_counts = ARMS.step2I(
-            obs_lists, relations, action_map, debugi
+            obs_tracelist, relations, action_map, debugi
         )
 
         debugp = ARMS.debug_menu("Debug plan constraints?") if debug else False
         plan_constraints = ARMS.step2P(
-            obs_lists,
+            obs_tracelist,
             connected_actions,
             action_map,
             set(relations.values()),
             min_support,
             debugp,
         )
 
@@ -442,15 +449,15 @@
                         )
                     )
 
         return constraints
 
     @staticmethod
     def step2I(
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         relations: Dict[Fluent, Relation],
         actions: Dict[Action, LearnedAction],
         debug: bool,
     ) -> Tuple[List[Or[Var]], Dict[Or[Var], int]]:
         """Information constraints.
 
         Suppose we observe a relation p to be true between two actions
@@ -471,65 +478,65 @@
         then we set a corresponding relation constraint \(p ∈ \\text{PRECOND}_a\), which
         receives a weight value equal to its prior probability.
         """
         if debug:
             print("\nBuilding information constraints...")
         constraints: List[Or[Var]] = []
         support_counts: Dict[Or[Var], int] = defaultdict(int)
-        obs_list: List[Observation]
-        for obs_list_i, obs_list in enumerate(obs_lists):
-            for i, obs in enumerate(obs_list):
+        obs_trace: List[Observation]
+        for obs_trace_i, obs_trace in enumerate(obs_tracelist):
+            for i, obs in enumerate(obs_trace):
                 if obs.state is not None and i > 0:
                     n = i - 1
                     if debug:
                         print(
-                            f"\nStep {i} of observation list {obs_list_i} contains state information."
+                            f"\nStep {i} of observation list {obs_trace_i} contains state information."
                         )
                     for fluent, val in obs.state.items():
                         relation = relations[fluent]
                         # Information constraints only apply to true relations
                         if val:
                             if debug:
                                 print(
                                     f"  Fluent {fluent} is true.\n"
                                     f"    ({relation.var()})∈ ("
-                                    f"{' ∪ '.join([f'add_{{ {actions[obs_list[ik].action].details()} }}' for ik in range(0,n+1) if obs_list[ik].action in actions] )}"  # type: ignore
+                                    f"{' ∪ '.join([f'add_{{ {actions[obs_trace[ik].action].details()} }}' for ik in range(0,n+1) if obs_trace[ik].action in actions] )}"  # type: ignore
                                     ")"
                                 )
                             # I1
                             # relation in the add list of an action <= n (i-1)
                             i1: List[Var] = []
-                            for obs_i in obs_list[: i - 1]:
+                            for obs_i in obs_trace[: i - 1]:
                                 if obs_i.action in actions and obs_i.action is not None:
                                     ai = actions[obs_i.action]
                                     if relation.matches(ai):
                                         i1.append(
                                             Var(
                                                 f"{relation.var()} (BREAK) in (BREAK) add (BREAK) {ai.details()}"
                                             )
                                         )
 
                             # I2
                             # relation not in del list of action n (i-1)
                             i2 = None
-                            a_n = obs_list[i - 1].action
+                            a_n = obs_trace[i - 1].action
                             if a_n in actions and a_n is not None:
                                 i2 = Var(
                                     f"{relation.var()} (BREAK) in (BREAK) del (BREAK) {actions[a_n].details()}"
                                 ).negate()
 
                             if i1:
                                 constraints.append(Or(i1))
                             if i2:
                                 constraints.append(Or([i2]))
 
                             # I3
                             # count occurences
                             if (
-                                i < len(obs_list) - 1
+                                i < len(obs_trace) - 1
                                 and obs.action in actions
                                 and obs.action is not None  # for the linter
                                 and relation.matches(actions[obs.action])
                             ):
                                 # corresponding constraint is related to the current action's precondition list
                                 support_counts[
                                     Or(
@@ -598,15 +605,15 @@
             if count >= minsup:
                 frequent_pairs[(ai, aj)] = count
 
         return frequent_pairs
 
     @staticmethod
     def step2P(
-        obs_lists: ObservationLists,
+        obs_tracelist: ObservedTraceList,
         connected_actions: Dict[LearnedAction, Dict[LearnedAction, Set]],
         action_map: Dict[Action, LearnedAction],
         relations: Set[Relation],
         min_support: int,
         debug: bool,
     ) -> Dict[Or[Var], int]:
         """Plan constraints.
@@ -643,18 +650,18 @@
         The above constraints can be combined into one constraint:
         $$\exists p ((p \in (pre_i \cap pre_j) \land p \\not \in (del_i)) \lor (p \in (add_i \cap pre_j)) \lor (p \in (del_i \cap add_j)))$$
         """
         frequent_pairs = ARMS._apriori(
             [
                 [
                     action_map[obs.action]
-                    for obs in obs_list
+                    for obs in obs_trace
                     if obs.action is not None and obs.action in action_map
                 ]
-                for obs_list in obs_lists
+                for obs_trace in obs_tracelist
             ],
             min_support,
         )
         if debug:
             print("Frequent pairs:")
             print(frequent_pairs)
 
@@ -673,15 +680,14 @@
                 continue
 
             # for each relation, save constraint
             relevant_relations = {p for p in relations if connectors.issubset(p.types)}
             # relation_constraints: List[Or[And[Var]]] = []
             relation_constraints: List[Var] = []
             for relation in relevant_relations:
-
                 relation_constraints.append(
                     Var(
                         f"{relation.var()} (BREAK) relevant (BREAK) {ai.details()} (BREAK) {aj.details()}"
                     )
                 )
                 if debug:
                     print(
```

### Comparing `macq-0.2.6/macq/extract/exceptions.py` & `macq-0.3.2/macq/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/extract/extract.py` & `macq-0.3.2/macq/extract/extract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """.. include:: ../../docs/templates/extract/extract.md"""
 
 from dataclasses import dataclass
 from enum import Enum, auto
+from typing import Dict, List, Union
+
+from ..observation import ObservedTraceList
 from ..trace import Action, State
-from ..observation import ObservationLists
+from .amdn import AMDN
+from .arms import ARMS
+from .locm import LOCM
 from .model import Model
 from .observer import Observer
 from .slaf import SLAF
-from .amdn import AMDN
-from .arms import ARMS
 
 
 @dataclass
 class SAS:
     pre_state: State
     action: Action
     post_state: State
@@ -24,47 +27,55 @@
     An Enum where each value represents a model extraction technique.
     """
 
     OBSERVER = auto()
     SLAF = auto()
     AMDN = auto()
     ARMS = auto()
+    LOCM = auto()
 
 
 class Extract:
     """Extracts models from observations.
 
     The Extract class uses an extraction method to retrieve an action Model
     from state observations.
     """
 
     def __new__(
-        cls, obs_lists: ObservationLists, mode: modes, debug: bool = False, **kwargs
+        cls,
+        obs_tracelist: ObservedTraceList,
+        mode: modes,
+        debug: Union[bool, Dict[str, bool], List[str]] = False,
+        **kwargs
     ) -> Model:
         """Extracts a Model object.
 
         Extracts a model from the observations using the specified extraction
         technique.
 
         Args:
-            obs_lists (ObservationList):
+            obs_tracelist (ObservationList):
                 The state observations to extract the model from.
             mode (Enum):
                 The extraction technique to use.
+            debug (bool, dict, list):
+                Model specific debugging options. Either a boolean, or a list/dict indicating the functions to debug.
             **kwargs: (keyword arguments)
                 Any extra arguments to supply to the extraction technique.
 
         Returns:
             A Model object. The model's characteristics are determined by the
             extraction technique used.
         """
+
+        if len(obs_tracelist) == 0:
+            raise ValueError("ObservationList is empty. Nothing to extract from.")
+
         techniques = {
             modes.OBSERVER: Observer,
             modes.SLAF: SLAF,
             modes.AMDN: AMDN,
             modes.ARMS: ARMS,
+            modes.LOCM: LOCM,
         }
-        if mode == modes.SLAF:
-            if len(obs_lists) != 1:
-                raise Exception("The SLAF extraction technique only takes one trace.")
-
-        return techniques[mode](obs_lists, debug, **kwargs)
+        return techniques[mode](obs_tracelist, debug=debug, **kwargs)
```

### Comparing `macq-0.2.6/macq/extract/learned_action.py` & `macq-0.3.2/macq/observation/observation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,98 +1,93 @@
-from __future__ import annotations
-from typing import List, Set
+from warnings import warn
+from json import dumps
+from typing import Union
+import random
+from ..trace import State, Action
+
+
+class InvalidQueryParameter(Exception):
+    def __init__(self, obs, param, message=None):
+        if message is None:
+            message = f"{param} is not a valid query parameter for {obs.__name__}"
+        super().__init__(message)
+
+
+class Observation:
+    """
+    An Observation object stores an observation token representation of a step.
+
+    Attributes:
+        step (Step):
+            The step associated with this observation.
+        index (int):
+            The index of the associated step in the trace it is a part of.
+    """
+
+    index: int
+    state: Union[State, None]
+    action: Union[Action, None]
 
+    def __init__(self, **kwargs):
+        """
+        Creates an Observation object, storing the step as a token, as well as its index/"place"
+        in the trace (which corresponds to that of the step).
 
-class LearnedAction:
-    def __init__(self, name: str, obj_params: List[str], **kwargs):
-        self.name = name
-        self.obj_params = obj_params
-        if "cost" in kwargs:
-            self.cost = kwargs["cost"]
-
-        self.precond = set() if "precond" not in kwargs else kwargs["precond"]
-        self.add = set() if "add" not in kwargs else kwargs["add"]
-        self.delete = set() if "delete" not in kwargs else kwargs["delete"]
-
-    def __eq__(self, other):
-        return (
-            isinstance(other, LearnedAction)
-            and self.name == other.name
-            and self.obj_params == other.obj_params
-        )
+        Args:
+            step (Step):
+                The step associated with this observation.
+        """
+        if "index" in kwargs.keys():
+            self.index = kwargs["index"]
+        else:
+            warn("Creating an Observation token without an index.")
 
     def __hash__(self):
-        # Order of obj_params is important!
-        return hash(self.details())
+        string = str(self)
+        if string == "Observation\n":
+            warn("Observation has no unique information. Generating a generic hash.")
+        return hash(string)
+
+    def __str__(self):
+        out = "Observation\n"
+        if self.index is not None:
+            out += f"  Index: {str(self.index)}\n"
+        if self.state:
+            out += f"  State: {str(self.state)}\n"
+        if self.action:
+            out += f"  Action: {str(self.action)}\n"
+
+        return out
+
+    def get_details(self):
+        ind = str(self.index) if self.index else "-"
+        state = self.state.details() if self.state else "-"
+        action = self.action.details() if self.action else ""
+        return (ind, state, action)
 
-    def details(self):
-        # obj_params can be either a list of strings or a list of PlanningObject depending on the token type and extraction method used to learn the action
-        try:
-            string = f"({self.name} {' '.join(self.obj_params)})"
-        except TypeError:
-            string = f"({self.name} {' '.join([o.details() for o in self.obj_params])})"
+    def _matches(self, *_):
+        raise NotImplementedError()
 
-        return string
-
-    def update_precond(self, fluents: Set[str]):
-        """Adds preconditions to the action.
+    def extract_fluent_subset(self, state: State, percent: float):
+        """Randomly extracts a subset of fluents from a state, according to the percentage given.
 
         Args:
-            fluents (set):
-                The set of fluents to be added to the action's preconditions.
-        """
-        self.precond.update(fluents)
+            fluents (State):
+                The state to extract fluents from.
+            percent (float):
+                The percent of the state to be extracted.
 
-    def update_add(self, fluents: Set[str]):
-        """Adds add effects to the action.
-
-        Args:
-            fluents (set):
-                The set of fluents to be added to the action's add effects.
+        Returns:
+            The random subset of fluents.
         """
-        self.add.update(fluents)
+        num_new_f = int(len(state) * (percent))
 
-    def update_delete(self, fluents: Set[str]):
-        """Adds delete effects to the action.
+        # shuffle keys and take an appropriate subset of them
+        extracted_f = list(state)
+        random.shuffle(extracted_f)
+        return extracted_f[:num_new_f]
 
-        Args:
-            fluents (set):
-                The set of fluents to be added to the action's delete effects.
-        """
-        self.delete.update(fluents)
+    def matches(self, query: dict):
+        return all([self._matches(key, value) for key, value in query.items()])
 
-    def clear(self):
-        self.precond = set()
-        self.add = set()
-        self.delete = set()
-
-    def compare(self, orig_action: LearnedAction):
-        """Compares the learned action to an original, ground truth action."""
-        precond_diff = orig_action.precond.difference(self.precond)
-        add_diff = orig_action.add.difference(self.add)
-        delete_diff = orig_action.delete.difference(self.delete)
-        return precond_diff, add_diff, delete_diff
-
-    def _serialize(self):
-        return dict(
-            name=self.name,
-            obj_params=self.obj_params,
-            cost=self.cost,
-            precond=list(self.precond),
-            add=list(self.add),
-            delete=list(self.delete),
-        )
-
-    @classmethod
-    def _deserialize(cls, data):
-        """Converts a json object to an Action."""
-        precond = set(data["precond"])
-        add = set(data["add"])
-        delete = set(data["delete"])
-        return cls(
-            data["name"],
-            data["obj_params"],
-            cost=data["cost"],
-            precond=precond,
-            add=add,
-            delete=delete,
-        )
+    def serialize(self):
+        return dumps(self, default=lambda o: o.__dict__, indent=2)
```

### Comparing `macq-0.2.6/macq/extract/observer.py` & `macq-0.3.2/macq/extract/observer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """.. include:: ../../docs/templates/extract/observer.md"""
 
-from typing import List, Set
 from collections import defaultdict
+from dataclasses import dataclass
+from typing import List, Set
 
-from attr import dataclass
+from dataclasses import dataclass
+from ..observation import IdentityObservation, ObservedTraceList
 from . import LearnedAction, Model
 from .exceptions import IncompatibleObservationToken
-from .model import Model
 from .learned_fluent import LearnedFluent
-from ..observation import IdentityObservation, ObservationLists
+from .model import Model
 
 
 @dataclass
 class DeltaObservation:
     added: Set[str]
     deleted: Set[str]
 
@@ -28,59 +29,59 @@
     The preconditions of an action are defined as the (positive) intersection
     of all pre-states to that action. The effects are the union off all fluents
     that changed state from a pre-state to a post-state of an action. Add this
     effects are fluents that went from False to True, delete effects are
     fluents that went from True to False.
     """
 
-    def __new__(cls, obs_lists: ObservationLists, debug: bool):
+    def __new__(cls, obs_tracelist: ObservedTraceList, **kwargs):
         """Creates a new Model object.
 
         Args:
             observations (ObservationList):
                 The state observations to extract the model from.
         Raises:
             IncompatibleObservationToken:
                 Raised if the observations are not identity observation.
         """
-        if obs_lists.type is not IdentityObservation:
-            raise IncompatibleObservationToken(obs_lists.type, Observer)
-        fluents = Observer._get_fluents(obs_lists)
-        actions = Observer._get_actions(obs_lists)
+        if obs_tracelist.type is not IdentityObservation:
+            raise IncompatibleObservationToken(obs_tracelist.type, Observer)
+        fluents = Observer._get_fluents(obs_tracelist)
+        actions = Observer._get_actions(obs_tracelist)
         return Model(fluents, actions)
 
     @staticmethod
-    def _get_fluents(obs_lists: ObservationLists):
+    def _get_fluents(obs_tracelist: ObservedTraceList):
         """Retrieves the set of fluents in the observations."""
         fluents = set()
-        obs_list: List[IdentityObservation]
-        for obs_list in obs_lists:
-            for obs in obs_list:
+        obs_trace: List[IdentityObservation]
+        for obs_trace in obs_tracelist:
+            for obs in obs_trace:
                 # Update fluents with the fluents in this observation
                 fluents.update(
                     LearnedFluent(f.name, [o.details() for o in f.objects])
                     for f in obs.state.keys()
                 )
         return fluents
 
     @staticmethod
-    def _get_actions(obs_lists: ObservationLists):
+    def _get_actions(obs_tracelist: ObservedTraceList):
         """Retrieves and augments the set of actions in the observations."""
         # Get the unique actions and the relevant traces
         action_obs = defaultdict(list)
-        obs_list: List[IdentityObservation]
-        for obs_list in obs_lists:
-            for obs in obs_list:
+        obs_trace: List[IdentityObservation]
+        for obs_trace in obs_tracelist:
+            for obs in obs_trace:
                 action = obs.action
                 if action:  # Final step has no action
-                    action_obs[action].append(obs_list)
+                    action_obs[action].append(obs_trace)
 
         action_pre_states = defaultdict(set)
         # Get transitions for each action
-        action_transitions = obs_lists.get_all_transitions()
+        action_transitions = obs_tracelist.get_all_transitions()
         for action, transitions in action_transitions.items():
             # Create a LearnedAction for the current action
             model_action = LearnedAction(
                 action.name, action.obj_params, cost=action.cost
             )
 
             for pre, post in transitions:
```

### Comparing `macq-0.2.6/macq/extract/slaf.py` & `macq-0.3.2/macq/extract/slaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """.. include:: ../../docs/templates/extract/slaf.md"""
 
-import macq.extract as extract
 from typing import Set, Union
-from nnf import Var, Or, And, true, false, config
+
 from bauhaus import Encoding
+from nnf import And, Or, Var, config, false, true
+
+import macq.extract as extract
+
+from ..observation import AtomicPartialObservation, ObservedTraceList
 from .exceptions import IncompatibleObservationToken
-from .model import Model
 from .learned_fluent import LearnedFluent
-from ..observation import AtomicPartialObservation, ObservationLists
+from .model import Model
 
 # only used for pretty printing in debug mode
 e = Encoding()
 
 
 class SLAF:
     """SLAF model extraction method.
@@ -36,36 +39,40 @@
     iterated through to determine which ones are entailed. This information is then used to extract the Model.
     """
 
     # only need one true and one false
     top = true
     bottom = false
 
-    def __new__(cls, o_list: ObservationLists, debug_mode: bool = False):
+    def __new__(cls, o_list: ObservedTraceList, debug: bool = False):
         """Creates a new Model object.
 
         Args:
             o_list (ObservationList):
                 The state observations to extract the model from.
             debug_mode (bool):
                 An optional mode that helps the user track any fluents they desire by examining the evolution
                 of their fluent-factored formulas through the steps.
         Raises:
             IncompatibleObservationToken:
                 Raised if the observations are not identity observation.
         """
         if o_list.type is not AtomicPartialObservation:
             raise IncompatibleObservationToken(o_list.type, SLAF)
-        SLAF.debug_mode = debug_mode
+
+        if len(o_list) != 1:
+            raise Exception("The SLAF extraction technique only takes one trace.")
+
+        SLAF.debug_mode = debug
         entailed = SLAF.__as_strips_slaf(o_list)
         # return the Model
         return SLAF.__sort_results(o_list, entailed)
 
     @staticmethod
-    def __get_initial_fluent_factored(o_list: ObservationLists):
+    def __get_initial_fluent_factored(o_list: ObservedTraceList):
         """Gets the initial fluent-factored formula of an observation/trace.
 
         Args:
             o_list (ObservationList):
                 The observation list to extract the fluent-factored formula from.
 
         Returns:
@@ -147,29 +154,29 @@
 
         Returns:
             A corresponding fluent of type "Or."
         """
         return Or([maybe_lit]) if isinstance(maybe_lit, Var) else maybe_lit
 
     @staticmethod
-    def __sort_results(observations: ObservationLists, entailed: Set):
+    def __sort_results(observations: ObservedTraceList, entailed: Set):
         """Generates a `Model` given the set of entailed propositions.
 
         Args:
             observations (ObservationLists):
                 The observations supplied for extraction.
             entailed (Set)
                 The set of propositions that were found to be entailed.
 
         Returns:
             The extracted `Model`.
         """
         learned_actions = {}
         model_fluents = observations.get_fluents()
-        
+
         # iterate through each step
         for o in observations:
             for token in o:
                 # if an action was taken on this step
                 if token.action:
                     # set up a base LearnedAction with the known information
                     learned_actions[str(token.action)] = extract.LearnedAction(
@@ -205,15 +212,15 @@
                     learned_actions[action].update_delete({effect})
                 else:
                     # update the add effects of this action with the appropriate fluent
                     learned_actions[action].update_add({effect})
         return Model(model_fluents, set(learned_actions.values()))
 
     @staticmethod
-    def __as_strips_slaf(o_list: ObservationLists):
+    def __as_strips_slaf(o_list: ObservedTraceList):
         """Implements the AS-STRIPS-SLAF algorithm from section 5.3 of the SLAF paper.
         Iterates through the action/observation pairs of each observation/trace, returning
         a fluent-factored transition belief formula that filters according to that action/observation.
         The transition belief formulas for each trace/observation are conjoined to get one final formula,
         which is then solved using a SAT solver to extract models.
 
         Args:
@@ -276,15 +283,16 @@
                 account of all of the current observations BEFORE the next action is taken."""
                 for phi in raw_fluent_factored.values():
                     f = phi["fluent"]
                     if str(f) in all_o:
                         """Step 1 (d): If this fluent is observed, update the formula accordingly.
                         Since we know the fluent is now true, the prior possible explanation for the fluent being true
                         (involving past actions, etc) are now set to the neutral explanation; that is, one of those explanations
-                        has to be true in order for the prior action to have no effect on the fluent currently being true."""
+                        has to be true in order for the prior action to have no effect on the fluent currently being true.
+                        """
                         phi["neutral"].update([p.simplify() for p in phi["pos expl"]])
                         phi["pos expl"] = {top}
                         phi["neg expl"] = {bottom}
                         if debug_mode and str(f) in to_obs:
                             print(
                                 f"{f} was observed to be true after the previous action was taken."
                             )
```

### Comparing `macq-0.2.6/macq/generate/csv.py` & `macq-0.3.2/macq/generate/csv.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/generate/pddl/fd_random_walk.py` & `macq-0.3.2/macq/generate/pddl/fd_random_walk.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,14 @@
     def _avg_op_cost(self):
         """Computes the average operator cost"""
 
         def _op_cost(a):
             if self.problem.get_action(a).cost is None:
                 return 1
             else:
-                return float(str(self.problem.get_action(a).cost))
+                return float(self.problem.get_action(a).cost.symbol)
 
         costs = {a: _op_cost(a) for a in self.problem.actions}
         total = 0
         for o in self.instance.operators:
             total += costs[o.name.split('(')[0]]
         return total / len(self.instance.operators)
```

### Comparing `macq-0.2.6/macq/generate/pddl/generator.py` & `macq-0.3.2/macq/generate/pddl/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
         self.observe_pres_effs = observe_pres_effs
         # read the domain and problem
         reader = PDDLReader(raise_on_error=True)
         if not problem_id:
             reader.parse_domain(dom)
             self.problem = reader.parse_instance(prob)
         else:
-            dom = requests.get(get_problem(problem_id)["domain_url"]).text
-            prob = requests.get(get_problem(problem_id)["problem_url"]).text
+            dom = requests.get(get_problem(problem_id, formalism='classical')["domain_url"]).text
+            prob = requests.get(get_problem(problem_id, formalism='classical')["problem_url"]).text
             reader.parse_domain_string(dom)
             self.problem = reader.parse_instance_string(prob)
         self.lang = self.problem.language
         # ground the problem
         operators = ground_problem_schemas_into_plain_operators(self.problem)
         self.instance = GroundForwardSearchModel(self.problem, operators)
         self.grounded_fluents = self.__get_all_grounded_fluents()
@@ -389,15 +389,15 @@
         Returns:
             A `Plan` object that holds all the actions taken.
         """
         if not from_ipc_file:
             # if the files are only being generated from the problem ID and are unaltered, retrieve the existing plan (note that
             # if any changes were made, the local files would be used as the PDDL files are rewritten when changes are made).
             if self.problem_id and not self.pddl_dom and not self.pddl_prob:
-                plan = get_plan(self.problem_id)
+                plan = get_plan(self.problem_id, formalism='classical')
             # if you are not just using the unaltered files, use the local files instead
             else:
                 data = {
                     "domain": open(self.pddl_dom, "r").read(),
                     "problem": open(self.pddl_prob, "r").read(),
                 }
```

### Comparing `macq-0.2.6/macq/generate/pddl/random_goal_sampling.py` & `macq-0.3.2/macq/generate/pddl/random_goal_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/generate/pddl/trace_from_goal.py` & `macq-0.3.2/macq/generate/pddl/trace_from_goal.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/generate/pddl/vanilla_sampling.py` & `macq-0.3.2/macq/generate/pddl/vanilla_sampling.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/generate/plan.py` & `macq-0.3.2/macq/generate/plan.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/__init__.py` & `macq-0.3.2/macq/observation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .observation import Observation, InvalidQueryParameter
-from .observation_lists import ObservationLists
+from .observed_tracelist import ObservedTraceList
 from .identity_observation import IdentityObservation
 from .partial_observation import PartialObservation
 from .atomic_partial_observation import AtomicPartialObservation
 from .noisy_observation import NoisyObservation
+from .action_observation import ActionObservation
 from .noisy_partial_observation import NoisyPartialObservation
 from .noisy_partial_disordered_parallel_observation import (
     NoisyPartialDisorderedParallelObservation,
 )
 
 
 __all__ = [
     "Observation",
-    "ObservationLists",
+    "ObservedTraceList",
     "InvalidQueryParameter",
     "IdentityObservation",
     "PartialObservation",
+    "ActionObservation",
     "AtomicPartialObservation",
     "NoisyObservation",
     "NoisyPartialObservation",
     "NoisyPartialDisorderedParallelObservation",
 ]
```

### Comparing `macq-0.2.6/macq/observation/atomic_partial_observation.py` & `macq-0.3.2/macq/observation/atomic_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/identity_observation.py` & `macq-0.3.2/macq/observation/identity_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/noisy_observation.py` & `macq-0.3.2/macq/observation/noisy_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/noisy_partial_disordered_parallel_observation.py` & `macq-0.3.2/macq/observation/noisy_partial_disordered_parallel_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/noisy_partial_observation.py` & `macq-0.3.2/macq/observation/noisy_partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/observation/observation_lists.py` & `macq-0.3.2/macq/observation/observed_tracelist.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 "Token type does not match observation tokens."
                 f"Token type: {token}"
                 f"Observation type: {obs_type}"
             )
         super().__init__(message)
 
 
-class ObservationLists(MutableSequence):
+class ObservedTraceList(MutableSequence):
     """A sequence of observations.
 
     A `list`-like object, where each element is a list of `Observation`s.
 
     Attributes:
         observations (List[List[Observation]]):
             The internal list of lists of `Observation` objects.
@@ -109,39 +109,39 @@
         if self.type == Observation:
             self.type = type(value[0])
         elif type(value[0]) != self.type:
             raise TokenTypeMismatch(self.type, type(value[0]))
 
     def get_actions(self) -> Set[Action]:
         actions: Set[Action] = set()
-        for obs_list in self:
-            for obs in obs_list:
+        for obs_trace in self:
+            for obs in obs_trace:
                 action = obs.action
                 if action is not None:
                     actions.add(action)
         return actions
 
     def get_fluents(self) -> Set[Fluent]:
         fluents: Set[Fluent] = set()
-        for obs_list in self:
-            for obs in obs_list:
+        for obs_trace in self:
+            for obs in obs_trace:
                 if obs.state:
                     fluents.update(list(obs.state.keys()))
         return fluents
 
     def tokenize(self, trace_list: TraceList, **kwargs):
         for trace in trace_list:
             tokens = trace.tokenize(self.type, **kwargs)
             self.append(tokens)
 
     def fetch_observations(self, query: dict) -> List[Set[Observation]]:
         matches: List[Set[Observation]] = []
-        for i, obs_list in enumerate(self.observations):
+        for i, obs_trace in enumerate(self.observations):
             matches.append(set())
-            for obs in obs_list:
+            for obs in obs_trace:
                 if obs.matches(query):
                     matches[i].add(obs)
         return matches
 
     def fetch_observation_windows(
         self, query: dict, left: int, right: int
     ) -> List[List[Observation]]:
@@ -187,43 +187,43 @@
         console = Console()
 
         views = ["details", "color"]
         if view not in views:
             warn(f'Invalid view {view}. Defaulting to "details".')
             view = "details"
 
-        obs_lists = []
+        obs_tracelist = []
         if view == "details":
             if wrap is None:
                 wrap = False
-            obs_lists = [self._details(obs_list, wrap=wrap) for obs_list in self]
+            obs_tracelist = [self._details(obs_trace, wrap=wrap) for obs_trace in self]
 
         elif view == "color":
             if wrap is None:
                 wrap = True
-            obs_lists = [
-                self._colorgrid(obs_list, filter_func=filter_func, wrap=wrap)
-                for obs_list in self
+            obs_tracelist = [
+                self._colorgrid(obs_trace, filter_func=filter_func, wrap=wrap)
+                for obs_trace in self
             ]
 
-        for obs_list in obs_lists:
-            console.print(obs_list)
+        for obs_trace in obs_tracelist:
+            console.print(obs_trace)
             print()
 
-    def _details(self, obs_list: List[Observation], wrap: bool):
+    def _details(self, obs_trace: List[Observation], wrap: bool):
         indent = " " * 2
         # Summarize class attributes
         details = Table.grid(expand=True)
         details.title = "Trace"
         details.add_column()
         details.add_row(
             cleandoc(
                 f"""
             Attributes:
-            {indent}{len(obs_list)} steps
+            {indent}{len(obs_trace)} steps
             {indent}{len(self.get_fluents())} fluents
             """
             )
         )
         steps = Table(
             title="Steps", box=None, show_edge=False, pad_edge=False, expand=True
         )
@@ -233,77 +233,77 @@
             justify="center",
             overflow="ellipsis",
             max_width=100,
             no_wrap=(not wrap),
         )
         steps.add_column("Action", overflow="ellipsis", no_wrap=(not wrap))
 
-        for obs in obs_list:
+        for obs in obs_trace:
             ind, state, action = obs.get_details()
             steps.add_row(ind, state, action)
 
         details.add_row(steps)
 
         return details
 
     @staticmethod
-    def _colorgrid(obs_list: List[Observation], filter_func: Callable, wrap: bool):
+    def _colorgrid(obs_trace: List[Observation], filter_func: Callable, wrap: bool):
         colorgrid = Table(
             title="Trace", box=None, show_edge=False, pad_edge=False, expand=False
         )
         colorgrid.add_column("Fluent", justify="right")
         colorgrid.add_column(
             header=Text("Step", justify="center"), overflow="fold", no_wrap=(not wrap)
         )
         colorgrid.add_row(
             "",
             "".join(
                 [
-                    "|" if i < len(obs_list) and (i + 1) % 5 == 0 else " "
-                    for i in range(len(obs_list))
+                    "|" if i < len(obs_trace) and (i + 1) % 5 == 0 else " "
+                    for i in range(len(obs_trace))
                 ]
             ),
         )
 
-        static = ObservationLists.get_obs_static_fluents(obs_list)
+        static = ObservedTraceList.get_obs_static_fluents(obs_trace)
         fluents = list(
             filter(
                 filter_func,
                 sorted(
-                    ObservationLists.get_obs_fluents(obs_list),
+                    ObservedTraceList.get_obs_fluents(obs_trace),
                     key=lambda f: float("inf") if f in static else len(str(f)),
                 ),
             )
         )
 
         for fluent in fluents:
             step_str = ""
-            for obs in obs_list:
+            for obs in obs_trace:
                 if obs.state and obs.state[fluent]:
                     step_str += "[green]"
                 else:
                     step_str += "[red]"
                 step_str += "■"
 
             colorgrid.add_row(str(fluent), step_str)
 
         return colorgrid
 
     @staticmethod
-    def get_obs_fluents(obs_list: List[Observation]):
+    def get_obs_fluents(obs_trace: List[Observation]):
         fluents = set()
-        for obs in obs_list:
+        for obs in obs_trace:
             if obs.state:
                 fluents.update(list(obs.state.keys()))
         return fluents
 
     @staticmethod
-    def get_obs_static_fluents(obs_list: List[Observation]):
+    def get_obs_static_fluents(obs_trace: List[Observation]):
         fstates = defaultdict(list)
-        for obs in obs_list:
+        for obs in obs_trace:
             if obs.state:
                 for f, v in obs.state.items():
                     fstates[f].append(v)
 
         static = set()
         for f, states in fstates.items():
             if all(states) or not any(states):
```

### Comparing `macq-0.2.6/macq/observation/partial_observation.py` & `macq-0.3.2/macq/observation/partial_observation.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/trace/__init__.py` & `macq-0.3.2/macq/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/trace/action.py` & `macq-0.3.2/macq/trace/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Set
+from typing import List, Optional, Set
 from .fluent import PlanningObject, Fluent
 
 
 class Action:
     """Grounded action.
 
     An Action represents a grounded action in a Trace or a Model. The action's
@@ -25,17 +25,17 @@
     """
 
     def __init__(
         self,
         name: str,
         obj_params: List[PlanningObject],
         cost: int = 0,
-        precond: Set[Fluent] = None,
-        add: Set[Fluent] = None,
-        delete: Set[Fluent] = None,
+        precond: Optional[Set[Fluent]] = None,
+        add: Optional[Set[Fluent]] = None,
+        delete: Optional[Set[Fluent]] = None,
     ):
         """Initializes an Action with the parameters provided.
         The `precond`, `add`, and `delete` args should only be provided in
         Model deserialization.
         Args:
             name (str):
                 The name of the action.
```

### Comparing `macq-0.2.6/macq/trace/disordered_parallel_actions_observation_lists.py` & `macq-0.3.2/macq/trace/disordered_parallel_actions_observation_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from math import exp
 from numpy import dot
 from random import random
 from typing import Callable, Type, Set, List
 from . import TraceList, Step, Action, PartialState, State
-from ..observation import Observation, ObservationLists
+from ..observation import Observation, ObservedTraceList
 
 
 @dataclass
 class ActionPair:
     """dataclass that allows a pair of actions to be referenced regardless of order
     (that is, {action1, action2} is equivalent to {action2, action1}.)
     """
@@ -91,15 +91,15 @@
 
      Returns:
         The (bool) decision made.
     """
     return random() < probability
 
 
-class DisorderedParallelActionsObservationLists(ObservationLists):
+class DisorderedParallelActionsObservationLists(ObservedTraceList):
     """Alternate ObservationLists type that enforces appropriate actions to be disordered and/or parallel.
     Inherits the base ObservationLists class.
 
     The default feature functions and theta vector described in the AMDN paper are available for use in this module.
 
     Attributes:
         observations (List[List[Token]]):
```

### Comparing `macq-0.2.6/macq/trace/fluent.py` & `macq-0.3.2/macq/trace/fluent.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/trace/state.py` & `macq-0.3.2/macq/trace/state.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/trace/step.py` & `macq-0.3.2/macq/trace/step.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/trace/trace.py` & `macq-0.3.2/macq/trace/trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import List, Type, Iterable, Callable, Set
 from inspect import cleandoc
+from warnings import warn
 from rich.table import Table
 from rich.text import Text
+from rich.console import Console
 from . import Action, Step, State
 from ..observation import Observation, NoisyPartialDisorderedParallelObservation
 from ..utils import TokenizationError
 
 
 @dataclass
 class SAS:
@@ -194,14 +196,50 @@
                     step_str += "[red]"
                 step_str += "■"
 
             colorgrid.add_row(str(fluent), step_str)
 
         return colorgrid
 
+    def get_printable(self, view="details", filter_func=lambda _: True, wrap=None):
+        """Returns a printable representation of the trace in the specified view."""
+        views = ["details", "color", "actions"]
+        if view not in views:
+            warn(f'Invalid view {view}. Defaulting to "details".')
+            view = "details"
+
+        if view == "details":
+            if wrap is None: wrap = False
+            return self.details(wrap=wrap)
+        elif view == "color":
+            if wrap is None: wrap = True
+            return self.colorgrid(filter_func=filter_func, wrap=wrap)
+        elif view == "actions":
+            return [step.action for step in self]
+
+
+    def print(self, view="details", filter_func=lambda _: True, wrap=None):
+        """Pretty prints the trace in the specified view.
+
+        Arguments:
+            view ("details" | "color" | "actions"):
+                Specifies the view format to print in. "details" prints a
+                detailed summary of each step in a trace. "color" prints a
+                color grid, mapping fluents in a step to either red or green
+                corresponding to the truth value. "actions" prints the actions
+                in the trace.
+            filter_func (Callable):
+                A function used to filter the fluents to be printed.
+            wrap (bool):
+                Specifies whether or not to wrap the text in the printed output.
+        """
+        console = Console()
+        console.print(self.get_printable(view=view, filter_func=filter_func, wrap=wrap))
+        print()
+
     def get_static_fluents(self):
         fstates = defaultdict(list)
         for step in self:
             for f, v in step.state.items():
                 fstates[f].append(v)
 
         static = set()
```

### Comparing `macq-0.2.6/macq/trace/trace_list.py` & `macq-0.3.2/macq/trace/trace_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from warnings import warn
-from typing import List, Callable, Type, Optional, Union
-from logging import warn
 from collections.abc import MutableSequence
-from rich.console import Console
+from typing import Callable, List, Type, Union
+from warnings import warn
 
+from ..observation import Observation, ObservedTraceList
 from . import Action, Trace
-from ..observation import Observation, ObservationLists
 
 
 class TraceList(MutableSequence):
     """A sequence of traces.
 
     A `list`-like object, where each element is a `Trace` of the same planning
     problem.
@@ -118,15 +116,15 @@
             for step in trace:
                 fluents.update(step.state.fluents)
         return fluents
 
     def tokenize(
         self,
         Token: Type[Observation],
-        ObsLists: Type[ObservationLists] = ObservationLists,
+        ObsLists: Type[ObservedTraceList] = ObservedTraceList,
         **kwargs,
     ):
         """Tokenizes the steps in this trace.
 
         Args:
             Token (Observation):
                 A subclass of `Observation`, defining the method of tokenization
@@ -137,35 +135,20 @@
         return ObsLists(self, Token, **kwargs)
 
     def print(self, view="details", filter_func=lambda _: True, wrap=None):
         """Pretty prints the trace list in the specified view.
 
         Arguments:
             view ("details" | "color"):
-                Specifies the view format to print in. "details" provides a
-                detailed summary of each step in a trace. "color" provides a
+                Specifies the view format to print in. "details" prints a
+                detailed summary of each step in a trace. "color" prints a
                 color grid, mapping fluents in a step to either red or green
-                corresponding to the truth value.
+                corresponding to the truth value. "actions" prints the actions
+                in the traces.
         """
-        console = Console()
-
-        views = ["details", "color"]
+        views = ["details", "color", "actions"]
         if view not in views:
             warn(f'Invalid view {view}. Defaulting to "details".')
             view = "details"
 
-        traces = []
-        if view == "details":
-            if wrap is None:
-                wrap = False
-            traces = [trace.details(wrap=wrap) for trace in self]
-
-        elif view == "color":
-            if wrap is None:
-                wrap = True
-            traces = [
-                trace.colorgrid(filter_func=filter_func, wrap=wrap) for trace in self
-            ]
-
-        for trace in traces:
-            console.print(trace)
-            print()
+        for trace in self:
+            trace.print(view, filter_func, wrap)
```

### Comparing `macq-0.2.6/macq/utils/__init__.py` & `macq-0.3.2/macq/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/utils/progress.py` & `macq-0.3.2/macq/utils/progress.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/utils/pysat.py` & `macq-0.3.2/macq/utils/pysat.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/utils/timer.py` & `macq-0.3.2/macq/utils/timer.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/utils/trace_errors.py` & `macq-0.3.2/macq/utils/trace_errors.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq/utils/trace_utils.py` & `macq-0.3.2/macq/utils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `macq-0.2.6/macq.egg-info/PKG-INFO` & `macq-0.3.2/macq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macq
-Version: 0.2.6
+Version: 0.3.2
 Summary: Action model acquisition from state trace data.
 Home-page: https://github.com/ai-planning/macq
 Author: Ethan Callanan, Rebecca De Venezia, Victoria Armstrong, Alison Parades, Tathagata Chakraborti, Christian Muise
 Author-email: christian.muise@queensu.ca
 License: MIT
 Keywords: planning model acquisition trace
 Classifier: Intended Audience :: Science/Research
@@ -40,16 +40,16 @@
 
 # get a domain-specific generator: uses api.planning.domains problem_id/
 # generate 100 traces of length 20 using vanilla sampling
 traces = generate.pddl.VanillaSampling(problem_id = 123, plan_len = 20, num_traces = 100).traces
 
 traces.generate_more(10)
 
-action1 = traces[0][0].action
-traces.get_usage(action1)
+action = traces[0][0].action
+traces.get_usage(action)
 [0.05, 0.05, ..., 0.05]
 
 trace = traces[0]
 len(trace)
 20
 
 trace.fluents
```

### Comparing `macq-0.2.6/macq.egg-info/SOURCES.txt` & `macq-0.3.2/macq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,38 @@
 macq/extract/__init__.py
 macq/extract/amdn.py
 macq/extract/arms.py
 macq/extract/exceptions.py
 macq/extract/extract.py
 macq/extract/learned_action.py
 macq/extract/learned_fluent.py
+macq/extract/locm.py
 macq/extract/model.py
 macq/extract/observer.py
 macq/extract/slaf.py
 macq/generate/__init__.py
 macq/generate/csv.py
 macq/generate/plan.py
 macq/generate/pddl/__init__.py
 macq/generate/pddl/fd_random_walk.py
 macq/generate/pddl/generator.py
 macq/generate/pddl/planning_domains_api.py
 macq/generate/pddl/random_goal_sampling.py
 macq/generate/pddl/trace_from_goal.py
 macq/generate/pddl/vanilla_sampling.py
 macq/observation/__init__.py
+macq/observation/action_observation.py
 macq/observation/atomic_partial_observation.py
 macq/observation/id_observation.py
 macq/observation/identity_observation.py
 macq/observation/noisy_observation.py
 macq/observation/noisy_partial_disordered_parallel_observation.py
 macq/observation/noisy_partial_observation.py
 macq/observation/observation.py
-macq/observation/observation_lists.py
+macq/observation/observed_tracelist.py
 macq/observation/partial_observation.py
 macq/trace/__init__.py
 macq/trace/action.py
 macq/trace/disordered_parallel_actions_observation_lists.py
 macq/trace/fluent.py
 macq/trace/partial_state.py
 macq/trace/state.py
@@ -52,8 +54,9 @@
 macq/utils/complex_encoder.py
 macq/utils/progress.py
 macq/utils/pysat.py
 macq/utils/timer.py
 macq/utils/tokenization_errors.py
 macq/utils/tokenization_utils.py
 macq/utils/trace_errors.py
-macq/utils/trace_utils.py
+macq/utils/trace_utils.py
+tests/test_readme.py
```

### Comparing `macq-0.2.6/setup.py` & `macq-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.6"
+VERSION = "0.3.2"
 
 NAME = "macq"
 
 DESCRIPTION = "Action model acquisition from state trace data."
 
 DEPENDENCIES = [
     "tarski",
     "requests",
     "rich",
     "nnf",
     "python-sat",
     "bauhaus",
     "numpy",
     "clingo",
+    "graphviz",
 ]
 
 DEV_DEPENDENCIES = [
     "pytest",
     "pytest-cov",
     "flake8",
     "black",
```


# Comparing `tmp/cluster_experiments-0.8.5.tar.gz` & `tmp/cluster_experiments-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluster_experiments-0.8.5.tar", last modified: Wed May 17 18:30:50 2023, max compression
+gzip compressed data, was "cluster_experiments-0.9.0.tar", last modified: Fri May 26 08:05:02 2023, max compression
```

## Comparing `cluster_experiments-0.8.5.tar` & `cluster_experiments-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.128725 cluster_experiments-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 18:30:50.128725 cluster_experiments-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.120725 cluster_experiments-0.8.5/cluster_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/cupac.py
--rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/perturbator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19753 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/power_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/random_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/cluster_experiments/washover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.120725 cluster_experiments-0.8.5/cluster_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 18:30:50.000000 cluster_experiments-0.8.5/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 18:30:50.000000 cluster_experiments-0.8.5/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:30:50.000000 cluster_experiments-0.8.5/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 18:30:50.000000 cluster_experiments-0.8.5/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 18:30:50.000000 cluster_experiments-0.8.5/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 18:30:50.128725 cluster_experiments-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.120725 cluster_experiments-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.124724 cluster_experiments-0.8.5/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/analysis/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.124724 cluster_experiments-0.8.5/tests/cupac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/cupac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/cupac/test_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.124724 cluster_experiments-0.8.5/tests/perturbator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/perturbator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.124724 cluster_experiments-0.8.5/tests/power_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:30:50.128725 cluster_experiments-0.8.5/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/test_time_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/splitter/test_washover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/test_non_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-17 18:29:28.000000 cluster_experiments-0.8.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.590408 cluster_experiments-0.9.0/cluster_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/cupac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21014 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29720 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/perturbator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19919 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/power_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19223 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/random_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/cluster_experiments/washover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/cluster_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 08:05:02.000000 cluster_experiments-0.9.0/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/cupac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/test_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/perturbator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/perturbator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/power_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:05:02.594408 cluster_experiments-0.9.0/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_time_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/splitter/test_washover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_non_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-26 08:02:36.000000 cluster_experiments-0.9.0/tests/utils.py
```

### Comparing `cluster_experiments-0.8.5/LICENSE` & `cluster_experiments-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/PKG-INFO` & `cluster_experiments-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster_experiments
-Version: 0.8.5
+Version: 0.9.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.5/README.md` & `cluster_experiments-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -148,19 +148,22 @@
 * Regarding power analysis:
     * `PowerAnalysis`: to run power analysis on a clustered/switchback design
     * `UniformPerturbator`: to artificially perturb treated group with uniform perturbations
     * `BinaryPerturbator`: to artificially perturb treated group for binary outcomes
     * `RelativePositivePerturbator`: to artificially perturb treated group with relative positive perturbations
     * `NormalPerturbator`: to artificially perturb treated group with normal distribution perturbations
     * `BetaRelativePositivePerturbator`: to artificially perturb treated group with relative positive beta distribution perturbations
+    * `BetaRelativePerturbator`: to artificially perturb treated group with relative beta distribution perturbations in a specified support interval
+    * `SegmentedBetaRelativePerturbator`: to artificially perturb treated group with relative beta distribution perturbations in a specified support interval, but using clusters
 * Regarding splitting data:
     * `ClusteredSplitter`: to split data based on clusters
     * `BalancedClusteredSplitter`: to split data based on clusters in a balanced way
     * `NonClusteredSplitter`: Regular data splitting, no clusters
     * `StratifiedClusteredSplitter`: to split based on clusters and strata, balancing the number of clusters in each stratus
+    * `RepeatedSampler`: for backtests where we have access to counterfactuals, does not split the data, just duplicates the data for all groups
     * Switchback splitters (the same can be done with clustered splitters, but there is a convenient way to define switchback splitters using switch frequency):
         * `SwitchbackSplitter`: to split data based on clusters and dates, for switchback experiments
         * `BalancedSwitchbackSplitter`: to split data based on clusters and dates, for switchback experiments, balancing treatment and control among all clusters
         * `StratifiedSwitchbackSplitter`: to split data based on clusters and dates, for switchback experiments, balancing the number of clusters in each stratus
         * Washover for switchback experiments:
             * `EmptyWashover`: no washover done at all.
             * `ConstantWashover`: accepts a timedelta parameter and removes the data when we switch from A to B for the timedelta interval.
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments/__init__.py` & `cluster_experiments-0.9.0/cluster_experiments/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,32 @@
     GeeExperimentAnalysis,
     MLMExperimentAnalysis,
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     TTestClusteredAnalysis,
 )
 from cluster_experiments.perturbator import (
+    BetaRelativePerturbator,
     BetaRelativePositivePerturbator,
     BinaryPerturbator,
     NormalPerturbator,
     Perturbator,
     RelativePositivePerturbator,
+    SegmentedBetaRelativePerturbator,
     UniformPerturbator,
 )
 from cluster_experiments.power_analysis import PowerAnalysis
 from cluster_experiments.power_config import PowerConfig
 from cluster_experiments.random_splitter import (
     BalancedClusteredSplitter,
     BalancedSwitchbackSplitter,
     ClusteredSplitter,
     NonClusteredSplitter,
     RandomSplitter,
+    RepeatedSampler,
     StratifiedClusteredSplitter,
     StratifiedSwitchbackSplitter,
     SwitchbackSplitter,
 )
 from cluster_experiments.washover import ConstantWashover, EmptyWashover, Washover
 
 __all__ = [
@@ -36,26 +39,29 @@
     "OLSAnalysis",
     "BinaryPerturbator",
     "Perturbator",
     "UniformPerturbator",
     "RelativePositivePerturbator",
     "NormalPerturbator",
     "BetaRelativePositivePerturbator",
+    "BetaRelativePerturbator",
+    "SegmentedBetaRelativePerturbator",
     "PowerAnalysis",
     "PowerConfig",
     "EmptyRegressor",
     "TargetAggregation",
     "BalancedClusteredSplitter",
     "ClusteredSplitter",
     "RandomSplitter",
     "NonClusteredSplitter",
     "StratifiedClusteredSplitter",
     "SwitchbackSplitter",
     "BalancedSwitchbackSplitter",
     "StratifiedSwitchbackSplitter",
+    "RepeatedSampler",
     "ClusteredOLSAnalysis",
     "TTestClusteredAnalysis",
     "PairedTTestClusteredAnalysis",
     "EmptyWashover",
     "ConstantWashover",
     "Washover",
     "MLMExperimentAnalysis",
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments/cupac.py` & `cluster_experiments-0.9.0/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.9.0/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/cluster_experiments/power_analysis.py` & `cluster_experiments-0.9.0/cluster_experiments/power_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cluster_experiments.power_config import (
     PowerConfig,
     analysis_mapping,
     cupac_model_mapping,
     perturbator_mapping,
     splitter_mapping,
 )
-from cluster_experiments.random_splitter import RandomSplitter
+from cluster_experiments.random_splitter import RandomSplitter, RepeatedSampler
 from cluster_experiments.utils import _get_mapping_key
 
 
 class PowerAnalysis:
     """
     Class used to run Power analysis. It does so by running simulations. In each simulation:
     1. Assign treatment to dataframe randomly
@@ -280,14 +280,16 @@
             average_effect: Average effect of treatment. If None, it will use the perturbator average effect.
             n_simulations: Number of simulations to run.
             alpha: Significance level.
         """
         n_detected_mde = 0
         for _ in tqdm(range(n_simulations), disable=not verbose):
             p_value = self._run_simulation((df, average_effect))
+            if verbose:
+                print(f"p_value of simulation run: {p_value:.3f}")
             n_detected_mde += p_value < alpha
 
         return n_detected_mde / n_simulations
 
     def _parallel_loop(
         self,
         df: pd.DataFrame,
@@ -462,14 +464,15 @@
             or self.analysis.cluster_cols == self.splitter.cluster_cols
         ), f"cluster_cols in analysis ({self.analysis.cluster_cols}) must be the same as cluster_cols in splitter ({self.splitter.cluster_cols})"
 
         assert (
             has_splitter_clusters
             or not has_analysis_clusters
             or not self.analysis.cluster_cols
+            or isinstance(self.splitter, RepeatedSampler)
         ), "analysis has cluster_cols but splitter does not."
 
         assert (
             has_analysis_clusters
             or not has_splitter_clusters
             or not self.splitter.cluster_cols
         ), "splitter has cluster_cols but analysis does not."
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments/power_config.py` & `cluster_experiments-0.9.0/cluster_experiments/power_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,28 @@
     GeeExperimentAnalysis,
     MLMExperimentAnalysis,
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     TTestClusteredAnalysis,
 )
 from cluster_experiments.perturbator import (
+    BetaRelativePerturbator,
     BetaRelativePositivePerturbator,
     BinaryPerturbator,
     NormalPerturbator,
     RelativePositivePerturbator,
+    SegmentedBetaRelativePerturbator,
     UniformPerturbator,
 )
 from cluster_experiments.random_splitter import (
     BalancedClusteredSplitter,
     BalancedSwitchbackSplitter,
     ClusteredSplitter,
     NonClusteredSplitter,
+    RepeatedSampler,
     StratifiedClusteredSplitter,
     StratifiedSwitchbackSplitter,
     SwitchbackSplitter,
 )
 
 
 @dataclass(eq=True)
@@ -51,14 +54,18 @@
         splitter_weights: weights to use for the splitter, should have the same length as treatments, each weight should correspond to an element in treatments
         switch_frequency: how often to switch treatments
         time_col: column to use as time in switchback splitter
         washover_time_delta: optional, int indicating the washover time in minutes or datetime.timedelta object
         covariates: list of columns to use as covariates
         average_effect: average effect to use in the perturbator
         scale: scale to use in stochastic perturbators
+        range_min: minimum value of the target range for relative beta perturbator, must be >-1
+        range_max: maximum value of the target range for relative beta perturbator
+        reduce_variance: whether to reduce variance in the BetaRelative perturbator
+        segment_cols: list of segmentation columns for segmented perturbator
         treatments: list of treatments to use
         alpha: alpha value to use in the power analysis
         agg_col: column to use for aggregation in the CUPAC model
         smoothing_factor: smoothing value to use in the CUPAC model
         features_cupac_model: list of features to use in the CUPAC model
         seed: seed to make the power analysis reproducible
 
@@ -96,14 +103,18 @@
     target_col: str = "target"
     treatment_col: str = "treatment"
     treatment: str = "B"
 
     # Perturbator
     average_effect: Optional[float] = None
     scale: Optional[float] = None
+    range_min: Optional[float] = None
+    range_max: Optional[float] = None
+    reduce_variance: Optional[bool] = None
+    segment_cols: Optional[List[str]] = None
 
     # Splitter
     treatments: Optional[List[str]] = None
     strata_cols: Optional[List[str]] = None
     splitter_weights: Optional[List[float]] = None
     switch_frequency: Optional[str] = None
     # Switchback
@@ -136,14 +147,26 @@
             if self._are_different(self.time_col, None):
                 self._set_and_log("time_col", None, "splitter")
 
         if self.perturbator not in {"normal", "beta_relative_positive"}:
             if self._are_different(self.scale, None):
                 self._set_and_log("scale", None, "perturbator")
 
+        if self.perturbator not in {"beta_relative", "clustered_beta_relative"}:
+            if self._are_different(self.range_min, None):
+                self._set_and_log("range_min", None, "perturbator")
+            if self._are_different(self.range_max, None):
+                self._set_and_log("range_max", None, "perturbator")
+            if self._are_different(self.reduce_variance, None):
+                self._set_and_log("reduce_variance", None, "perturbator")
+
+        if self.perturbator not in {"clustered_beta_relative"}:
+            if self._are_different(self.segment_cols, None):
+                self._set_and_log("segment_cols", None, "perturbator")
+
         if "stratified" not in self.splitter and "paired_ttest" not in self.analysis:
             if self._are_different(self.strata_cols, None):
                 self._set_and_log("strata_cols", None, "splitter")
 
         if "stratified" in self.splitter or "balanced" in self.splitter:
             if self._are_different(self.splitter_weights, None):
                 self._set_and_log("splitter_weights", None, "splitter")
@@ -175,24 +198,27 @@
 
 perturbator_mapping = {
     "binary": BinaryPerturbator,
     "uniform": UniformPerturbator,
     "relative_positive": RelativePositivePerturbator,
     "normal": NormalPerturbator,
     "beta_relative_positive": BetaRelativePositivePerturbator,
+    "beta_relative": BetaRelativePerturbator,
+    "segmented_beta_relative": SegmentedBetaRelativePerturbator,
 }
 
 splitter_mapping = {
     "clustered": ClusteredSplitter,
     "clustered_balance": BalancedClusteredSplitter,
     "non_clustered": NonClusteredSplitter,
     "clustered_stratified": StratifiedClusteredSplitter,
     "switchback": SwitchbackSplitter,
     "switchback_balance": BalancedSwitchbackSplitter,
     "switchback_stratified": StratifiedSwitchbackSplitter,
+    "backtest": RepeatedSampler,
 }
 
 analysis_mapping = {
     "gee": GeeExperimentAnalysis,
     "ols_non_clustered": OLSAnalysis,
     "ols_clustered": ClusteredOLSAnalysis,
     "ttest_clustered": TTestClusteredAnalysis,
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments/random_splitter.py` & `cluster_experiments-0.9.0/cluster_experiments/random_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,7 +477,59 @@
             strata_cols=config.strata_cols,
             treatment_col=config.treatment_col,
             time_col=config.time_col,
             switch_frequency=config.switch_frequency,
             splitter_weights=config.splitter_weights,
             washover=washover_cls.from_config(config),
         )
+
+
+class RepeatedSampler(RandomSplitter):
+    """
+    Doesn't actually split the data, but repeatedly samples (i.e. duplicates) all rows for all treatments.
+    This is useful for backtesting, where we assume to have access to all counterfactuals.
+
+    Arguments:
+        treatments: list of treatments
+        treatment_col: Name of the column with the treatment variable.
+
+    Usage:
+    ```python
+    import pandas as pd
+    from cluster_experiments.random_splitter import RepeatedSampler
+    splitter = RepeatedSampler(
+        treatments=["A", "B"],
+    )
+    df = pd.DataFrame({"city": ["A", "B", "C"]})
+    df = splitter.assign_treatment_df(df)
+    print(df)
+    ```
+    """
+
+    def __init__(
+        self,
+        treatments: Optional[List[str]] = None,
+        treatment_col: str = "treatment",
+    ) -> None:
+        self.treatments = treatments or ["A", "B"]
+        self.treatment_col = treatment_col
+
+    def assign_treatment_df(
+        self,
+        df: pd.DataFrame,
+    ) -> pd.DataFrame:
+        df = df.copy()
+
+        dfs = []
+        for treatment in self.treatments:
+            df_treat = df.copy().assign(**{self.treatment_col: treatment})
+            dfs.append(df_treat)
+
+        return pd.concat(dfs).reset_index(drop=True)
+
+    @classmethod
+    def from_config(cls, config):
+        """Creates a RepeatedSampler from a PowerConfig"""
+        return cls(
+            treatments=config.treatments,
+            treatment_col=config.treatment_col,
+        )
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments/washover.py` & `cluster_experiments-0.9.0/cluster_experiments/washover.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             time_col="time",
             cluster_cols=["city", "time"],
             treatment_col="treatment",
             switch_frequency="30T",
         )
 
         out_df = splitter.assign_treatment_df(df=washover_split_df)
-
+        ```
         """
         return df
 
 
 class ConstantWashover(Washover):
     """Constant washover - we drop all rows in the washover period when
     there is a switch where the treatment is different."""
@@ -133,15 +133,15 @@
             time_col="time",
             cluster_cols=["city", "time"],
             treatment_col="treatment",
             switch_frequency="30T",
         )
 
         out_df = splitter.assign_treatment_df(df=washover_split_df)
-
+        ```
         """
         # Set original time column
         original_time_col = (
             original_time_col
             if original_time_col
             else _original_time_column(truncated_time_col)
         )
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments.egg-info/PKG-INFO` & `cluster_experiments-0.9.0/cluster_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluster-experiments
-Version: 0.8.5
+Version: 0.9.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cluster_experiments-0.8.5/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.9.0/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.9.0/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/setup.py` & `cluster_experiments-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.8.5",
+    version="0.9.0",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.8.5/tests/analysis/test_analysis.py` & `cluster_experiments-0.9.0/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/cupac/test_aggregator.py` & `cluster_experiments-0.9.0/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.9.0/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/examples.py` & `cluster_experiments-0.9.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.9.0/tests/perturbator/test_perturbator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from cluster_experiments.perturbator import (
+    BetaRelativePerturbator,
     BetaRelativePositivePerturbator,
     BinaryPerturbator,
     NormalPerturbator,
     RelativePositivePerturbator,
+    SegmentedBetaRelativePerturbator,
     UniformPerturbator,
 )
 from cluster_experiments.power_config import PowerConfig
-from tests.examples import binary_df, continuous_df
+from tests.examples import binary_df, continuous_df, generate_clustered_data
 
 
 def test_binary_perturbator_from_config():
     config = PowerConfig(
         analysis="gee",
         splitter="clustered_balance",
         perturbator="binary",
@@ -197,14 +199,113 @@
     )
 
     # then
     assert np.mean(perturbated_values) == np.mean(effect)
     assert np.var(perturbated_values) == np.var(effect)
 
 
+@pytest.mark.parametrize("average_effect", [0.1, 0.04])
+def test_beta_relative_perturbate(average_effect):
+    # given
+    range_min = -0.8
+    range_max = 5
+    pert = BetaRelativePerturbator(range_min=range_min, range_max=range_max)
+
+    average_effect_inv_transf = (average_effect - range_min) / (range_max - range_min)
+    scale_inv_transf = average_effect_inv_transf
+    a = average_effect_inv_transf / (scale_inv_transf * scale_inv_transf)
+    b = (1 - average_effect_inv_transf) / (scale_inv_transf * scale_inv_transf)
+
+    np.random.seed(24)
+    beta = np.random.beta(a / abs(average_effect), b / abs(average_effect), 2)
+    beta_transf = beta * (range_max - range_min) + range_min
+
+    effect = (1 + beta_transf) * continuous_df.query("treatment == 'B'")[
+        "target"
+    ].values
+
+    # when
+    np.random.seed(24)
+    perturbated_values = (
+        pert.perturbate(continuous_df, average_effect=average_effect)
+        .query("treatment == 'B'")["target"]
+        .values
+    )
+
+    # then
+    assert np.isclose(np.mean(perturbated_values), np.mean(effect))
+    assert np.isclose(np.var(perturbated_values), np.var(effect))
+
+
+@pytest.mark.parametrize("average_effect", [0.1, 0.04])
+def test_segmented_beta_relative_perturbate(average_effect):
+    range_min = -0.8
+    range_max = 4
+
+    df_clustered = generate_clustered_data()
+    pert = SegmentedBetaRelativePerturbator(
+        range_min=range_min, range_max=range_max, segment_cols=["city_code"]
+    )
+
+    mean_effects = []
+    # repeat multiple times to decrease variability
+    for _ in range(100):
+        df_pert = pert.perturbate(
+            pd.concat([df_clustered for _ in range(100)]), average_effect=average_effect
+        )
+        df_merged = df_clustered.merge(
+            df_pert,
+            on=["country_code", "city_code", "user_id", "date", "treatment"],
+            suffixes=["", "_pert"],
+        )
+        df_merged = df_merged.assign(
+            rel_pert=df_merged["target_pert"] / df_merged["target"]
+        )
+        mean_effects.append(
+            df_merged.loc[df_merged["treatment"] == "B", "rel_pert"].mean()
+        )
+
+    # maximum relative difference we expect between the simulated relative perturbations and the passed average_effect
+    max_rel_diff = 0.2
+    assert abs((np.mean(mean_effects) - 1) / average_effect - 1) < max_rel_diff
+
+
+@pytest.mark.parametrize("average_effect", [0.1, 0.04])
+def test_segmented_beta_relative_perturbate_multiple_segments(average_effect):
+    range_min = -0.8
+    range_max = 4
+
+    df_clustered = generate_clustered_data()
+    pert = SegmentedBetaRelativePerturbator(
+        range_min=range_min, range_max=range_max, segment_cols=["city_code", "date"]
+    )
+
+    mean_effects = []
+    # repeat multiple times to decrease variability
+    for _ in range(100):
+        df_pert = pert.perturbate(
+            pd.concat([df_clustered for _ in range(100)]), average_effect=average_effect
+        )
+        df_merged = df_clustered.merge(
+            df_pert,
+            on=["country_code", "city_code", "user_id", "date", "treatment"],
+            suffixes=["", "_pert"],
+        )
+        df_merged = df_merged.assign(
+            rel_pert=df_merged["target_pert"] / df_merged["target"]
+        )
+        mean_effects.append(
+            df_merged.loc[df_merged["treatment"] == "B", "rel_pert"].mean()
+        )
+
+    # maximum relative difference we expect between the simulated relative perturbations and the passed average_effect
+    max_rel_diff = 0.2
+    assert abs((np.mean(mean_effects) - 1) / average_effect - 1) < max_rel_diff
+
+
 def test_binary_raises():
     binary_df_repeated = pd.concat([binary_df for _ in range(50)])
     bp = BinaryPerturbator()
     with pytest.raises(ValueError, match="average_effect must be provided"):
         bp.perturbate(binary_df_repeated)
```

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/conftest.py` & `cluster_experiments-0.9.0/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_seed.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.9.0/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/splitter/conftest.py` & `cluster_experiments-0.9.0/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/splitter/test_splitter.py` & `cluster_experiments-0.9.0/tests/splitter/test_splitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 import pytest
 
 from cluster_experiments.power_config import PowerConfig
 from cluster_experiments.random_splitter import (
     BalancedClusteredSplitter,
     ClusteredSplitter,
+    RepeatedSampler,
     StratifiedClusteredSplitter,
 )
 from tests.utils import assert_balanced_strata
 
 random.seed(421)
 np.random.seed(421)
 
@@ -320,7 +321,16 @@
     # testing that the value error is raised when two strata have the same cluster
     splitter = StratifiedClusteredSplitter(
         strata_cols=["segment"], cluster_cols=["cluster"]
     )
 
     with pytest.raises(ValueError):
         splitter.assign_treatment_df(df_strata_multiple_values)
+
+
+def test_backtest_splitter(treatments, df_cluster):
+    splitter = RepeatedSampler(treatments=treatments)
+    n_duplicates = 100
+    df_cluster = pd.concat([df_cluster for _ in range(n_duplicates)])
+    sampled_treatment = splitter.assign_treatment_df(df_cluster)
+    assert len(sampled_treatment) == len(treatments) * len(df_cluster)
+    assert (sampled_treatment.treatment.value_counts() == len(df_cluster)).all()
```

### Comparing `cluster_experiments-0.8.5/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.9.0/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/splitter/test_time_col.py` & `cluster_experiments-0.9.0/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/splitter/test_washover.py` & `cluster_experiments-0.9.0/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/test_docs.py` & `cluster_experiments-0.9.0/tests/test_docs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from mktestdocs import check_docstring, check_md_file, get_codeblock_members
 
 from cluster_experiments import (
     BalancedClusteredSplitter,
     BalancedSwitchbackSplitter,
+    BetaRelativePerturbator,
     BetaRelativePositivePerturbator,
     BinaryPerturbator,
     ClusteredOLSAnalysis,
     ClusteredSplitter,
     ConstantWashover,
     EmptyRegressor,
     EmptyWashover,
@@ -19,14 +20,16 @@
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     Perturbator,
     PowerAnalysis,
     PowerConfig,
     RandomSplitter,
     RelativePositivePerturbator,
+    RepeatedSampler,
+    SegmentedBetaRelativePerturbator,
     StratifiedClusteredSplitter,
     StratifiedSwitchbackSplitter,
     SwitchbackSplitter,
     TargetAggregation,
     TTestClusteredAnalysis,
     UniformPerturbator,
 )
@@ -53,18 +56,21 @@
     UniformPerturbator,
     _original_time_column,
     ConstantWashover,
     EmptyWashover,
     BalancedSwitchbackSplitter,
     StratifiedSwitchbackSplitter,
     SwitchbackSplitter,
+    RepeatedSampler,
     MLMExperimentAnalysis,
     RelativePositivePerturbator,
     NormalPerturbator,
     BetaRelativePositivePerturbator,
+    BetaRelativePerturbator,
+    SegmentedBetaRelativePerturbator,
 ]
 
 
 def flatten(items):
     """Flattens a list"""
     return [item for sublist in items for item in sublist]
```

### Comparing `cluster_experiments-0.8.5/tests/test_non_clustered.py` & `cluster_experiments-0.9.0/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.5/tests/utils.py` & `cluster_experiments-0.9.0/tests/utils.py`

 * *Files identical despite different names*


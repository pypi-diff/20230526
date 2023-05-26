# Comparing `tmp/seldonian_experiments-0.1.1.tar.gz` & `tmp/seldonian_experiments-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_experiments-0.1.1.tar", last modified: Mon Apr 24 16:32:29 2023, max compression
+gzip compressed data, was "seldonian_experiments-0.2.0.tar", last modified: Fri May 26 15:37:18 2023, max compression
```

## Comparing `seldonian_experiments-0.1.1.tar` & `seldonian_experiments-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.216580 seldonian_experiments-0.1.1/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.1.1/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-04-24 16:32:29.216421 seldonian_experiments-0.1.1/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.1.1/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.211504 seldonian_experiments-0.1.1/examples/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.1.1/examples/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.1.1/examples/run_examples.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.214419 seldonian_experiments-0.1.1/experiments/
--rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.1.1/experiments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4058 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/base_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    46934 2023-03-27 18:09:43.000000 seldonian_experiments-0.1.1/experiments/experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    38683 2023-04-24 16:30:24.000000 seldonian_experiments-0.1.1/experiments/generate_plots.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3357 2023-04-24 16:25:04.000000 seldonian_experiments-0.1.1/experiments/headless_example.py
--rw-r--r--   0 ahoag      (501) staff       (20)    17185 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/headless_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/headless_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     9342 2023-03-27 18:29:04.000000 seldonian_experiments-0.1.1/experiments/utils.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.215300 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)      615 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-04-24 16:32:29.000000 seldonian_experiments-0.1.1/seldonian_experiments.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-04-24 16:32:29.216623 seldonian_experiments-0.1.1/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-04-24 16:32:18.000000 seldonian_experiments-0.1.1/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-04-24 16:32:29.216085 seldonian_experiments-0.1.1/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.1.1/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4257 2023-01-09 18:12:54.000000 seldonian_experiments-0.1.1/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)      713 2022-09-27 22:42:46.000000 seldonian_experiments-0.1.1/tests/test_experiments.py
--rw-r--r--   0 ahoag      (501) staff       (20)    15190 2023-04-13 15:54:44.000000 seldonian_experiments-0.1.1/tests/test_generate_plots.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.889847 seldonian_experiments-0.2.0/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-04-25 15:36:26.000000 seldonian_experiments-0.2.0/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-05-26 15:37:18.889677 seldonian_experiments-0.2.0/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      295 2022-11-11 21:28:20.000000 seldonian_experiments-0.2.0/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.883975 seldonian_experiments-0.2.0/examples/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2023-03-09 21:51:03.000000 seldonian_experiments-0.2.0/examples/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4973 2023-03-27 18:38:58.000000 seldonian_experiments-0.2.0/examples/run_examples.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.887174 seldonian_experiments-0.2.0/experiments/
+-rw-r--r--   0 ahoag      (501) staff       (20)       81 2023-03-09 00:38:52.000000 seldonian_experiments-0.2.0/experiments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4062 2023-05-25 23:09:19.000000 seldonian_experiments-0.2.0/experiments/base_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13564 2023-05-25 22:51:03.000000 seldonian_experiments-0.2.0/experiments/experiment_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    44773 2023-05-25 23:07:24.000000 seldonian_experiments-0.2.0/experiments/experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    39631 2023-05-25 22:09:58.000000 seldonian_experiments-0.2.0/experiments/generate_plots.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3527 2023-05-25 22:54:38.000000 seldonian_experiments-0.2.0/experiments/headless_example.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    17446 2023-05-21 09:38:11.000000 seldonian_experiments-0.2.0/experiments/headless_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8933 2023-04-25 19:01:34.000000 seldonian_experiments-0.2.0/experiments/headless_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2127 2023-05-08 15:32:53.000000 seldonian_experiments-0.2.0/experiments/perf_eval_funcs.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.888167 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)      816 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)      680 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       17 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       21 2023-05-26 15:37:18.000000 seldonian_experiments-0.2.0/seldonian_experiments.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-05-26 15:37:18.889893 seldonian_experiments-0.2.0/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)      869 2023-05-26 15:37:03.000000 seldonian_experiments-0.2.0/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-05-26 15:37:18.889320 seldonian_experiments-0.2.0/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-07-11 18:48:12.000000 seldonian_experiments-0.2.0/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4257 2023-01-09 18:12:54.000000 seldonian_experiments-0.2.0/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9611 2023-05-26 14:48:12.000000 seldonian_experiments-0.2.0/tests/test_examples.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      848 2023-05-26 14:46:07.000000 seldonian_experiments-0.2.0/tests/test_experiments.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     9041 2023-05-22 23:02:27.000000 seldonian_experiments-0.2.0/tests/test_generate_plots.py
```

### Comparing `seldonian_experiments-0.1.1/LICENSE` & `seldonian_experiments-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.1/PKG-INFO` & `seldonian_experiments-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_experiments
-Version: 0.1.1
+Version: 0.2.0
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.1.1/examples/run_examples.py` & `seldonian_experiments-0.2.0/examples/run_examples.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.1/experiments/base_example.py` & `seldonian_experiments-0.2.0/experiments/base_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 results_dir=results_dir,
                 perf_eval_kwargs=perf_eval_kwargs,
             )
 
         # Baselines first
         for baseline_model in baselines:
             plot_generator.run_baseline_experiment(
-                model_name=baseline_model, verbose=verbose
+                baseline_model=baseline_model, verbose=verbose
             )
         # Check if fairlearn requested
         if include_fairlearn_models:
             fairlearn_sensitive_feature_names = fairlearn_kwargs[
                 "fairlearn_sensitive_feature_names"
             ]
             fairlearn_constraint_name = fairlearn_kwargs[
```

### Comparing `seldonian_experiments-0.1.1/experiments/experiments.py` & `seldonian_experiments-0.2.0/experiments/experiments.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Module for running Seldonian Experiments """
 
 import os
-import pickle
+from operator import itemgetter
 import autograd.numpy as np  # Thinly-wrapped version of Numpy
-import pandas as pd
 from concurrent.futures import ProcessPoolExecutor
 import multiprocessing as mp
-from functools import partial
 from tqdm import tqdm
+from functools import partial
 import copy
 
+import pandas as pd
 from sklearn.preprocessing import StandardScaler
 from sklearn.pipeline import make_pipeline
 from sklearn.linear_model import LogisticRegression
 
 from seldonian.utils.io_utils import load_pickle
 from seldonian.dataset import SupervisedDataSet, RLDataSet
 from seldonian.seldonian_algorithm import SeldonianAlgorithm
@@ -21,15 +21,20 @@
 from seldonian.models.models import (
     LinearRegressionModel,
     BinaryLogisticRegressionModel,
     DummyClassifierModel,
     RandomClassifierModel,
 )
 
-from .utils import batch_predictions
+from .experiment_utils import (
+    batch_predictions,
+    load_resampled_dataset,
+    prep_feat_labels,
+    setup_SA_spec_for_exp,
+)
 
 try:
     from fairlearn.reductions import ExponentiatedGradient
     from fairlearn.metrics import (
         MetricFrame,
         selection_rate,
         false_positive_rate,
@@ -61,44 +66,41 @@
         :param model_name: The string name of the baseline model,
                 e.g 'logistic_regression'
         :type model_name: str
 
         :param results_dir: Parent directory for saving any
                 experimental results
         :type results_dir: str
-
         """
         self.model_name = model_name
         self.results_dir = results_dir
 
     def aggregate_results(self, **kwargs):
         """Group together the data in each
         trial file into a single CSV file.
         """
-        savedir_results = os.path.join(self.results_dir, f"{self.model_name}_results")
-        os.makedirs(savedir_results, exist_ok=True)
-        savename_results = os.path.join(
-            savedir_results, f"{self.model_name}_results.csv"
-        )
+        d = os.path.join(self.results_dir, f"{self.model_name}_results")
+        os.makedirs(d, exist_ok=True)
+        res_fname = os.path.join(d, f"{self.model_name}_results.csv")
 
-        trial_dir = os.path.join(
+        d_trial = os.path.join(
             self.results_dir, f"{self.model_name}_results", "trial_data"
         )
         df_list = []
         for data_frac in kwargs["data_fracs"]:
             for trial_i in range(kwargs["n_trials"]):
                 filename = os.path.join(
-                    trial_dir, f"data_frac_{data_frac:.4f}_trial_{trial_i}.csv"
+                    d_trial, f"data_frac_{data_frac:.4f}_trial_{trial_i}.csv"
                 )
                 df = pd.read_csv(filename)
                 df_list.append(df)
 
-        result_df = pd.concat(df_list)
-        result_df.to_csv(savename_results, index=False)
-        print(f"Saved {savename_results}")
+        res_df = pd.concat(df_list)
+        res_df.to_csv(res_fname, index=False)
+        print(f"Saved {res_fname}")
         return
 
     def write_trial_result(self, data, colnames, trial_dir, verbose=False):
         """Write out the results from a single trial
         to a file.
 
         :param data: The information to save
@@ -110,72 +112,77 @@
 
         :param trial_dir: The directory in which to save the file
         :type trial_dir: str
 
         :param verbose: if True, prints out saved filename
         :type verbose: bool
         """
-        result_df = pd.DataFrame([data])
-        result_df.columns = colnames
+        res_df = pd.DataFrame([data])
+        res_df.columns = colnames
         data_frac, trial_i = data[0:2]
 
-        savename = os.path.join(
+        fname = os.path.join(
             trial_dir, f"data_frac_{data_frac:.4f}_trial_{trial_i}.csv"
         )
 
-        result_df.to_csv(savename, index=False)
+        res_df.to_csv(fname, index=False)
         if verbose:
-            print(f"Saved {savename}")
+            print(f"Saved {fname}")
         return
 
 
 class BaselineExperiment(Experiment):
-    def __init__(self, model_name, results_dir):
+    def __init__(self, baseline_model, results_dir):
         """Class for running baseline experiments
         against which to compare Seldonian Experiments
 
         :param model_name: The string name of the baseline model,
                 e.g 'logistic_regression'
         :type model_name: str
 
         :param results_dir: Parent directory for saving any
                 experimental results
         :type results_dir: str
         """
+        self.baseline_model = baseline_model
+        model_name = self.baseline_model.model_name
         super().__init__(model_name, results_dir)
 
     def run_experiment(self, **kwargs):
         """Run the baseline experiment"""
         partial_kwargs = {
             key: kwargs[key] for key in kwargs if key not in ["data_fracs", "n_trials"]
         }
 
         helper = partial(self.run_baseline_trial, **partial_kwargs)
 
         data_fracs = kwargs["data_fracs"]
         n_trials = kwargs["n_trials"]
         n_workers = kwargs["n_workers"]
 
-        data_fracs_vector = np.array([x for x in data_fracs for y in range(n_trials)])
-        trials_vector = np.array(
+        data_fracs_vec = np.array([x for x in data_fracs for y in range(n_trials)])
+        trials_vec = np.array(
             [x for y in range(len(data_fracs)) for x in range(n_trials)]
         )
 
         if n_workers == 1:
-            for ii in range(len(data_fracs_vector)):
-                data_frac = data_fracs_vector[ii]
-                trial_i = trials_vector[ii]
+            # run all trials synchronously
+            for ii in range(len(data_fracs_vec)):
+                data_frac = data_fracs_vec[ii]
+                trial_i = trials_vec[ii]
                 helper(data_frac, trial_i)
+
         elif n_workers > 1:
+            # run trials asynchronously
             with ProcessPoolExecutor(
                 max_workers=n_workers, mp_context=mp.get_context("fork")
             ) as ex:
                 results = tqdm(
-                    ex.map(helper, data_fracs_vector, trials_vector),
-                    total=len(data_fracs_vector),
+                    ex.map(helper, data_fracs_vec, trials_vec),
+                    total=len(data_fracs_vec),
                 )
                 for exc in results:
                     if exc:
                         print(exc)
         else:
             raise ValueError(f"value of {n_workers} must be >=1 ")
 
@@ -188,47 +195,57 @@
         :param data_frac: Fraction of overall dataset size to use
         :type data_frac: float
 
         :param trial_i: The index of the trial
         :type trial_i: int
         """
 
-        spec = kwargs["spec"]
+        spec = copy.deepcopy(kwargs["spec"])
         if isinstance(spec, RLSpec):
             raise NotImplementedError("Baselines are not yet implemented for RL")
         dataset = spec.dataset
         parse_trees = spec.parse_trees
-        verbose = kwargs["verbose"]
-        datagen_method = kwargs["datagen_method"]
-        perf_eval_fn = kwargs["perf_eval_fn"]
-        perf_eval_kwargs = kwargs["perf_eval_kwargs"]
-        batch_epoch_dict = kwargs["batch_epoch_dict"]
-        constraint_eval_kwargs = kwargs["constraint_eval_kwargs"]
+        (
+            verbose,
+            datagen_method,
+            perf_eval_fn,
+            perf_eval_kwargs,
+            batch_epoch_dict,
+            constraint_eval_fns,
+            constraint_eval_kwargs,
+        ) = itemgetter(
+            "verbose",
+            "datagen_method",
+            "perf_eval_fn",
+            "perf_eval_kwargs",
+            "batch_epoch_dict",
+            "constraint_eval_fns",
+            "constraint_eval_kwargs",
+        )(kwargs)
+
         if (
             batch_epoch_dict == {}
             and (spec.optimization_technique == "gradient_descent")
             and (spec.optimization_hyperparams["use_batches"] == True)
         ):
             warning_msg = (
                 "WARNING: No batch_epoch_dict was provided. "
                 "Each data_frac will use the same values "
                 "for batch_size and n_epochs. "
-                "This can have adverse effects, "
-                "especially for small values of data_frac."
+                "This can have adverse effects",
+                " " "especially for small values of data_frac.",
             )
             warnings.warn(warning_msg)
 
-        trial_dir = os.path.join(
+        d_trial = os.path.join(
             self.results_dir, f"{self.model_name}_results", "trial_data"
         )
-
-        os.makedirs(trial_dir, exist_ok=True)
-
+        os.makedirs(d_trial, exist_ok=True)
         savename = os.path.join(
-            trial_dir, f"data_frac_{data_frac:.4f}_trial_{trial_i}.csv"
+            d_trial, f"data_frac_{data_frac:.4f}_trial_{trial_i}.csv"
         )
 
         if os.path.exists(savename):
             if verbose:
                 print(
                     f"Trial {trial_i} already run for "
                     f"this data_frac: {data_frac}. Skipping this trial. "
@@ -236,146 +253,209 @@
             return
 
         ##############################################
         """ Setup for running baseline algorithm """
         ##############################################
 
         if datagen_method == "resample":
-            resampled_filename = os.path.join(
-                self.results_dir, "resampled_dataframes", f"trial_{trial_i}.pkl"
+            trial_dataset, n_points = load_resampled_dataset(
+                self.results_dir, trial_i, data_frac
             )
-            resampled_dataset = load_pickle(resampled_filename)
-            num_datapoints_tot = resampled_dataset.num_datapoints
-            n_points = int(round(data_frac * num_datapoints_tot))
-
-            if verbose:
-                print(
-                    f"Using resampled dataset {resampled_filename} "
-                    f"with {num_datapoints_tot} datapoints"
-                )
         else:
             raise NotImplementedError(
                 f"datagen_method: {datagen_method} "
                 f"not supported for regime: {regime}"
             )
 
-        # Prepare features and labels
-        features = resampled_dataset.features
-        labels = resampled_dataset.labels
-        # Only use first n_points for this trial
-        if type(features) == list:
-            features = [x[:n_points] for x in features]
-        else:
-            features = features[:n_points]
-        labels = labels[:n_points]
+        features, labels = prep_feat_labels(trial_dataset, n_points)
 
         ####################################################
         """" Instantiate model and fit to resampled data """
         ####################################################
         X_test_baseline = perf_eval_kwargs["X"]
+        baseline_model = copy.deepcopy(self.baseline_model)
+        train_kwargs = {}
+        pred_kwargs = {}
+        try:
+            if hasattr(baseline_model,"batch_epoch_dict"):
+                batch_size, n_epochs = baseline_model.batch_epoch_dict[data_frac]
+                train_kwargs["batch_size"] = batch_size
+                train_kwargs["n_epochs"] = n_epochs
+            solution = baseline_model.train(features, labels, **train_kwargs)
+            
+            # predict the probabilities (e.g. 0.85) not the labels (e.g., 1) 
+            if hasattr(baseline_model,"eval_batch_size"):
+                pred_kwargs["eval_batch_size"] = getattr(baseline_model,"eval_batch_size")
+                if hasattr(baseline_model,"N_output_classes"):
+                    pred_kwargs["N_output_classes"] = getattr(baseline_model,"N_output_classes")
 
-        if self.model_name == "linear_regression":
-            baseline_model = LinearRegressionModel()
-            try:
-                solution = baseline_model.fit(features, labels)
-                # predict the probabilities not the class labels
-                y_pred = baseline_model.predict(solution, X_test_baseline)
-            except ValueError:
-                solution = "NSF"
-
-        if self.model_name == "logistic_regression":
-            baseline_model = BinaryLogisticRegressionModel()
-            try:
-                solution = baseline_model.fit(features, labels)
-                # predict the probabilities not the class labels
-                y_pred = baseline_model.predict(solution, X_test_baseline)
-            except ValueError:
-                solution = "NSF"
-
-        if self.model_name == "random_classifier":
-            # Returns the positive class with p=0.5 every time
-            baseline_model = RandomClassifierModel()
-            solution = None
-            y_pred = baseline_model.predict(solution, X_test_baseline)
-
-        if self.model_name == "weighted_random_classifier":
-            # Returns the positive class with p=num_pos_class/num_neg_class every time
-            from .baselines.random_classifiers import WeightedRandomClassifierModel
-
-            baseline_model = WeightedRandomClassifierModel(0.4772833)
-            solution = None
-            y_pred = baseline_model.predict(solution, X_test_baseline)
-
-        if self.model_name == "facial_recog_cnn":
-            from .baselines.facial_recog_cnn import PytorchFacialRecog
-
-            device = perf_eval_kwargs["device"]
-            baseline_model = PytorchFacialRecog(device=device)
-            batch_size, n_epochs = batch_epoch_dict[data_frac]
-            baseline_model.train(
-                features, labels, batch_size=batch_size, num_epochs=n_epochs
-            )
-            solution = baseline_model.get_model_params()
-            y_pred = batch_predictions(
-                baseline_model, solution, X_test_baseline, **perf_eval_kwargs
-            )
+                y_pred = batch_predictions(
+                    model=baseline_model,
+                    solution=solution,
+                    X_test=X_test_baseline,
+                    **pred_kwargs,
+                )
+            else:
+                y_pred = baseline_model.predict(
+                    solution, 
+                    X_test_baseline, 
+                    **pred_kwargs)
+        except ValueError:
+            solution = "NSF"
+
+        # if self.model_name == "linear_regression":
+        #     baseline_model = LinearRegressionModel()
+        #     try:
+        #         solution = baseline_model.fit(features, labels)
+        #         y_pred = baseline_model.predict(solution, X_test_baseline)
+        #     except ValueError:
+        #         solution = "NSF"
+
+        # if self.model_name == "logistic_regression":
+        #     baseline_model = BinaryLogisticRegressionModel()
+        #     try:
+        #         solution = baseline_model.fit(features, labels)
+        #         # predict the probabilities not the class labels
+        #         y_pred = baseline_model.predict(solution, X_test_baseline)
+        #     except ValueError:
+        #         solution = "NSF"
+
+        # if self.model_name == "random_classifier":
+        #     # Returns the positive class with p=0.5 every time
+        #     baseline_model = RandomClassifierModel()
+        #     solution = None
+        #     y_pred = baseline_model.predict(solution, X_test_baseline)
+
+        # if self.model_name == "weighted_random_classifier":
+        #     # Returns the positive class with p=num_pos_class/num_neg_class every time
+        #     from .baselines.random_classifiers import WeightedRandomClassifierModel
+
+        #     baseline_model = WeightedRandomClassifierModel(0.4772833)
+        #     solution = None
+        #     y_pred = baseline_model.predict(solution, X_test_baseline)
+
+        # if self.model_name == "facial_recog_cnn":
+        #     from .baselines.facial_recog_cnn import PytorchFacialRecog
+
+        #     device = perf_eval_kwargs["device"]
+        #     baseline_model = PytorchFacialRecog(device=device)
+        #     batch_size, n_epochs = batch_epoch_dict[data_frac]
+        #     baseline_model.train(
+        #         features, labels, batch_size=batch_size, num_epochs=n_epochs
+        #     )
+        #     solution = baseline_model.get_model_params()
+        #     y_pred = batch_predictions(
+        #         baseline_model, solution, X_test_baseline, **perf_eval_kwargs
+        #     )
+
+        
 
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
         # Handle whether solution was found
         solution_found = True
         if type(solution) == str and solution == "NSF":
             solution_found = False
 
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
-
-        failed = False  # flag for whether we were actually safe on test set
         if solution_found:
             performance = perf_eval_fn(y_pred, **perf_eval_kwargs)
 
             if verbose:
                 print(f"Performance = {performance}")
-            if "eval_batch_size" in constraint_eval_kwargs:
-                batch_size_safety = constraint_eval_kwargs["eval_batch_size"]
-            else:
-                batch_size_safety = None
+
             # Determine whether this solution
             # violates any of the constraints
             # on the test dataset, which is the dataset from spec
+            if constraint_eval_fns == []:
+                constraint_eval_kwargs["baseline_model"] = baseline_model
+                constraint_eval_kwargs["dataset"] = dataset
+                constraint_eval_kwargs["parse_trees"] = parse_trees
+                constraint_eval_kwargs["verbose"] = verbose
+
+            gvec = self.evaluate_constraint_functions(
+                solution=solution,
+                constraint_eval_fns=constraint_eval_fns,
+                constraint_eval_kwargs=constraint_eval_kwargs,
+            )
+        else:
+            print("NSF")
+            # NSF is safe, so set g=-inf for all constraints
+            n_constraints = len(spec.parse_trees)
+            gvec = -np.inf * np.ones(
+                n_constraints
+            )  
+            performance = np.nan
+
+        # Write out file for this data_frac,trial_i combo
+        # data = [data_frac, trial_i, performance, failed]
+        # colnames = ["data_frac", "trial_i", "performance", "failed"]
+        data = [data_frac, trial_i, performance, gvec]
+        colnames = ["data_frac", "trial_i", "performance", "gvec"]
+        self.write_trial_result(data, colnames, d_trial, verbose=kwargs["verbose"])
+        return
+
+    def evaluate_constraint_functions(
+        self, solution, constraint_eval_fns, constraint_eval_kwargs
+    ):
+        """Helper function to evaluate
+        the constraint functions to determine
+        whether baseline solution was safe on ground truth
+
+        :param solution: The weights of the model found
+                during model training in a given trial
+        :type solution: numpy ndarray
+        :param constraint_eval_fns: List of functions
+                to use to evaluate each constraint.
+                An empty list (default) results in using the parse
+                tree to evaluate the constraints
+        :type constraint_eval_fns: List(function)
+        :param constraint_eval_kwargs: keyword arguments
+                to pass to each constraint function
+                in constraint_eval_fns
+        :type constraint_eval_kwargs: dict
+        :return: a vector of g values for the constraints
+        :rtype: np.ndarray
+        """
+        # Use safety test branch so the confidence bounds on
+        # leaf nodes are not inflated
+        gvals = []
+        if constraint_eval_fns == []:
+            parse_trees = constraint_eval_kwargs["parse_trees"]
+            dataset = constraint_eval_kwargs["dataset"]
+            baseline_model = constraint_eval_kwargs["baseline_model"]
+            if hasattr(baseline_model,"eval_batch_size"):
+                batch_size_safety = getattr(baseline_model,"eval_batch_size")
+            else:
+                batch_size_safety = None
             for parse_tree in parse_trees:
                 parse_tree.reset_base_node_dict(reset_data=True)
                 parse_tree.evaluate_constraint(
                     theta=solution,
                     dataset=dataset,
                     model=baseline_model,
-                    regime="supervised_learning",
+                    regime=dataset.regime,
                     branch="safety_test",
                     batch_size_safety=batch_size_safety,
                 )
-
                 g = parse_tree.root.value
 
-                if g > 0 or np.isnan(g):
-                    failed = True
-                    if verbose:
-                        print("Failed on test set")
-                if verbose:
-                    print(f"g (baseline={self.model_name}) = {g}")
+                gvals.append(g)
+                parse_tree.reset_base_node_dict(
+                    reset_data=True
+                )  # to clear out anything so the next trial has fresh data
         else:
-            print("NSF")
-            performance = np.nan
-
-        # Write out file for this data_frac,trial_i combo
-        data = [data_frac, trial_i, performance, failed]
-        colnames = ["data_frac", "trial_i", "performance", "failed"]
-        self.write_trial_result(data, colnames, trial_dir, verbose=kwargs["verbose"])
-        return
+            # User provided functions to evaluate constraints
+            for eval_fn in constraint_eval_fns:
+                g = eval_fn(solution, **constraint_eval_kwargs)
+                gvals.append(g)
+        return np.array(gvals)
 
 
 class SeldonianExperiment(Experiment):
     def __init__(self, model_name, results_dir):
         """Class for running Seldonian experiments
 
         :param model_name: The string name of the Seldonian model,
@@ -472,137 +552,36 @@
                     f"Trial {trial_i} already run for "
                     f"this data_frac: {data_frac}. Skipping this trial. "
                 )
             return
 
         os.makedirs(trial_dir, exist_ok=True)
 
-        parse_trees = spec.parse_trees
-        dataset = spec.dataset
-
         ##############################################
         """ Setup for running Seldonian algorithm """
         ##############################################
 
-        if regime == "supervised_learning":
-            if datagen_method == "resample":
-                resampled_filename = os.path.join(
-                    self.results_dir, "resampled_dataframes", f"trial_{trial_i}.pkl"
-                )
-                resampled_dataset = load_pickle(resampled_filename)
-                num_datapoints_tot = resampled_dataset.num_datapoints
-                n_points = int(round(data_frac * num_datapoints_tot))
-
-                if verbose:
-                    print(
-                        f"Using resampled dataset {resampled_filename} "
-                        f"with {num_datapoints_tot} datapoints"
-                    )
-                    if n_points < 1:
-                        raise ValueError(
-                            f"This data_frac={data_frac} "
-                            f"results in {n_points} data points. "
-                            "Must have at least 1 data point to run a trial."
-                        )
-
-                features = resampled_dataset.features
-                labels = resampled_dataset.labels
-                sensitive_attrs = resampled_dataset.sensitive_attrs
-                # Only use first n_points for this trial
-                if type(features) == list:
-                    features = [x[:n_points] for x in features]
-                else:
-                    features = features[:n_points]
-                labels = labels[:n_points]
-                sensitive_attrs = sensitive_attrs[:n_points]
-
-            else:
-                raise NotImplementedError(
-                    f"Eval method {datagen_method} "
-                    f"not supported for regime={regime}"
-                )
-
-            dataset_for_experiment = SupervisedDataSet(
-                features=features,
-                labels=labels,
-                sensitive_attrs=sensitive_attrs,
-                num_datapoints=n_points,
-                meta_information=resampled_dataset.meta_information,
-            )
-
-            # Make a new spec object
-            # and update the dataset
-
-            spec_for_experiment = copy.deepcopy(spec)
-            spec_for_experiment.dataset = dataset_for_experiment
-
-        elif regime == "reinforcement_learning":
-            hyperparameter_and_setting_dict = kwargs["hyperparameter_and_setting_dict"]
-
-            if datagen_method == "generate_episodes":
-                n_episodes_for_eval = perf_eval_kwargs["n_episodes_for_eval"]
-                # Sample from resampled dataset on disk of n_episodes
-                save_dir = os.path.join(self.results_dir, "regenerated_datasets")
-
-                savename = os.path.join(
-                    save_dir, f"regenerated_data_trial{trial_i}.pkl"
-                )
-
-                episodes_all = load_pickle(savename)
-                # Take data_frac episodes from this df
-                n_episodes_all = len(episodes_all)
-
-                n_episodes_for_exp = int(round(n_episodes_all * data_frac))
-                if n_episodes_for_exp < 1:
-                    raise ValueError(
-                        f"This data_frac={data_frac} "
-                        f"results in {n_episodes_for_exp} episodes. "
-                        "Must have at least 1 episode to run a trial."
-                    )
-
-                print(f"Orig dataset should have {n_episodes_all} episodes")
-                print(
-                    f"This dataset with data_frac={data_frac} should have"
-                    f" {n_episodes_for_exp} episodes"
-                )
-
-                # Take first n_episodes episodes
-                episodes_for_exp = episodes_all[0:n_episodes_for_exp]
-                assert len(episodes_for_exp) == n_episodes_for_exp
-
-                dataset_for_experiment = RLDataSet(
-                    episodes=episodes_for_exp,
-                    meta_information=dataset.meta_information,
-                    regime=regime,
-                )
-
-                # Make a new spec object from a copy of spec, where the
-                # only thing that is different is the dataset
+        spec_for_exp = setup_SA_spec_for_exp(
+            spec=spec,
+            regime=regime,
+            results_dir=self.results_dir,
+            trial_i=trial_i,
+            data_frac=data_frac,
+            datagen_method=datagen_method,
+            batch_epoch_dict=batch_epoch_dict,
+            kwargs=kwargs,
+            perf_eval_kwargs=perf_eval_kwargs,
+        )
 
-                spec_for_experiment = copy.deepcopy(spec)
-                spec_for_experiment.dataset = dataset_for_experiment
-            else:
-                raise NotImplementedError(
-                    f"Eval method {datagen_method} " "not supported for regime={regime}"
-                )
-        # If optimizing using gradient descent,
-        # and using mini-batches,
-        # update the batch_size and n_epochs
-        # using batch_epoch_dict
-        if spec_for_experiment.optimization_technique == "gradient_descent":
-            if spec_for_experiment.optimization_hyperparams["use_batches"] == True:
-                batch_size, n_epochs = batch_epoch_dict[data_frac]
-                spec_for_experiment.optimization_hyperparams["batch_size"] = batch_size
-                spec_for_experiment.optimization_hyperparams["n_epochs"] = n_epochs
         ################################
         """" Run Seldonian algorithm """
         ################################
 
         try:
-            SA = SeldonianAlgorithm(spec_for_experiment)
+            SA = SeldonianAlgorithm(spec_for_exp)
             passed_safety, solution = SA.run(write_cs_logfile=verbose, debug=verbose)
 
         except (ValueError, ZeroDivisionError):
             passed_safety = False
             solution = "NSF"
 
         if verbose:
@@ -615,16 +594,14 @@
         if type(solution) == str and solution == "NSF":
             solution_found = False
 
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
 
-        failed = False  # flag for whether we were actually safe on test set
-
         if solution_found:
             solution = copy.deepcopy(solution)
             # If passed the safety test, calculate performance
             # using solution
             if passed_safety:
                 if verbose:
                     print("Passed safety test! Calculating performance")
@@ -645,140 +622,147 @@
                             **perf_eval_kwargs,
                         )
                     else:
                         y_pred = model.predict(solution, X_test)
 
                     performance = perf_eval_fn(y_pred, model=model, **perf_eval_kwargs)
 
-                if regime == "reinforcement_learning":
+                elif regime == "reinforcement_learning":
                     model = copy.deepcopy(SA.model)
                     model.policy.set_new_params(solution)
                     perf_eval_kwargs["model"] = model
                     perf_eval_kwargs[
                         "hyperparameter_and_setting_dict"
                     ] = hyperparameter_and_setting_dict
                     episodes_for_eval, performance = perf_eval_fn(**perf_eval_kwargs)
-                if verbose:
-                    print(f"Performance = {performance}")
 
-                ########################################
-                """ Calculate safety on ground truth """
-                ########################################
                 if verbose:
+                    print(f"Performance = {performance}")
                     print(
                         "Determining whether solution "
                         "is actually safe on ground truth"
                     )
+                ########################################
+                """ Calculate safety on ground truth """
+                ########################################
 
                 if constraint_eval_fns == []:
                     constraint_eval_kwargs["model"] = model
                     constraint_eval_kwargs["spec_orig"] = spec
-                    constraint_eval_kwargs["spec_for_experiment"] = spec_for_experiment
+                    constraint_eval_kwargs["spec_for_exp"] = spec_for_exp
                     constraint_eval_kwargs["regime"] = regime
                     constraint_eval_kwargs["branch"] = "safety_test"
                     constraint_eval_kwargs["verbose"] = verbose
 
                 if regime == "reinforcement_learning":
                     constraint_eval_kwargs["episodes_for_eval"] = episodes_for_eval
 
-                failed = self.evaluate_constraint_functions(
+                gvec = self.evaluate_constraint_functions(
                     solution=solution,
                     constraint_eval_fns=constraint_eval_fns,
                     constraint_eval_kwargs=constraint_eval_kwargs,
                 )
 
                 if verbose:
-                    if failed:
-                        print("Solution was not actually safe on ground truth!")
-                    else:
-                        print("Solution was safe on ground truth")
+                    print(f"gvec: {gvec}")
                     print()
             else:
                 if verbose:
-                    print("Failed safety test ")
+                    print("Failed safety test")
                     performance = np.nan
 
-        else:
+        else:  # solution_found=False
+            n_constraints = len(spec.parse_trees)
+            # NSF is safe, so set g=-inf for all constraints
+            gvec = -np.inf * np.ones(n_constraints)
             if verbose:
                 print("NSF")
             performance = np.nan
+
+        # Clear out any cached data in the parse trees for the next trial.
+        # This also handles the case where solution_found=False.
+        for parse_tree in spec_for_exp.parse_trees:
+            parse_tree.reset_base_node_dict(reset_data=True)
+
         # Write out file for this data_frac,trial_i combo
-        data = [data_frac, trial_i, performance, passed_safety, failed]
-        colnames = ["data_frac", "trial_i", "performance", "passed_safety", "failed"]
+        data = [data_frac, trial_i, performance, passed_safety, gvec]
+        colnames = ["data_frac", "trial_i", "performance", "passed_safety", "gvec"]
         self.write_trial_result(data, colnames, trial_dir, verbose=kwargs["verbose"])
         return
 
     def evaluate_constraint_functions(
         self, solution, constraint_eval_fns, constraint_eval_kwargs
     ):
         """Helper function for QSA() to evaluate
         the constraint functions to determine
         whether solution was safe on ground truth
 
         :param solution: The weights of the model found
                 during candidate selection in a given trial
         :type solution: numpy ndarray
-
         :param constraint_eval_fns: List of functions
                 to use to evaluate each constraint.
                 An empty list results in using the parse
                 tree to evaluate the constraints
         :type constraint_eval_fns: List(function)
-
         :param constraint_eval_kwargs: keyword arguments
                 to pass to each constraint function
                 in constraint_eval_fns
         :type constraint_eval_kwargs: dict
+        :return: a vector of g values for the constraints
+        :rtype: np.ndarray
         """
         # Use safety test branch so the confidence bounds on
         # leaf nodes are not inflated
-        failed = False
+        gvals = []
         if constraint_eval_fns == []:
             """User did not provide their own functions
             to evaluate the constraints. Use the default:
             the parse tree has a built-in way to evaluate constraints.
             """
             constraint_eval_kwargs["theta"] = solution
             spec_orig = constraint_eval_kwargs["spec_orig"]
-            spec_for_experiment = constraint_eval_kwargs["spec_for_experiment"]
+            spec_for_exp = constraint_eval_kwargs["spec_for_exp"]
             regime = constraint_eval_kwargs["regime"]
             if "eval_batch_size" in constraint_eval_kwargs:
                 constraint_eval_kwargs["batch_size_safety"] = constraint_eval_kwargs[
                     "eval_batch_size"
                 ]
             if regime == "supervised_learning":
                 # Use the original dataset as ground truth
                 constraint_eval_kwargs["dataset"] = spec_orig.dataset
 
             elif regime == "reinforcement_learning":
                 episodes_for_eval = constraint_eval_kwargs["episodes_for_eval"]
 
                 dataset_for_eval = RLDataSet(
                     episodes=episodes_for_eval,
-                    meta_information=spec_for_experiment.dataset.meta_information,
+                    meta_information=spec_for_exp.dataset.meta_information,
                     regime=regime,
                 )
 
                 constraint_eval_kwargs["dataset"] = dataset_for_eval
 
-            for parse_tree in spec_for_experiment.parse_trees:
+            for parse_tree in spec_for_exp.parse_trees:
                 parse_tree.reset_base_node_dict(reset_data=True)
                 parse_tree.evaluate_constraint(**constraint_eval_kwargs)
 
                 g = parse_tree.root.value
-                if g > 0 or np.isnan(g):
-                    failed = True
+                gvals.append(g)
+                parse_tree.reset_base_node_dict(
+                    reset_data=True
+                )  # to clear out anything so the next trial has fresh data
 
         else:
             # User provided functions to evaluate constraints
             for eval_fn in constraint_eval_fns:
-                g = eval_fn(solution)
-                if g > 0 or np.isnan(g):
-                    failed = True
-        return failed
+                g = eval_fn(solution, **constraint_eval_kwargs)
+                gvals.append(g)
+
+        return np.array(gvals)
 
 
 class FairlearnExperiment(Experiment):
     def __init__(self, results_dir, fairlearn_epsilon_constraint):
         """Class for running Fairlearn experiments
 
         :param results_dir: Parent directory for saving any
@@ -873,57 +857,38 @@
                     f"Trial {trial_i} already run for "
                     f"this data_frac: {data_frac}. Skipping this trial. "
                 )
             return
 
         os.makedirs(trial_dir, exist_ok=True)
 
-        parse_trees = spec.parse_trees
-        dataset = spec.dataset
-
         ##############################################
         """ Setup for running Fairlearn algorithm """
         ##############################################
 
         if datagen_method == "resample":
-            resampled_filename = os.path.join(
-                self.results_dir, "resampled_dataframes", f"trial_{trial_i}.pkl"
+            trial_dataset, n_points = load_resampled_dataset(
+                self.results_dir, trial_i, data_frac
             )
-            resampled_dataset = load_pickle(resampled_filename)
-            num_datapoints_tot = resampled_dataset.num_datapoints
-            n_points = int(round(data_frac * num_datapoints_tot))
-
-            if verbose:
-                print(
-                    f"Using resampled dataset {resampled_filename} "
-                    f"with {num_datapoints_tot} datapoints"
-                )
         else:
             raise NotImplementedError(
                 f"datagen_method: {datagen_method} "
                 f"not supported for regime: {regime}"
             )
 
         # Prepare features and labels
-        features = resampled_dataset.features
-        labels = resampled_dataset.labels
-        # Only use first n_points for this trial
-        if type(features) == list:
-            features = [x[:n_points] for x in features]
-        else:
-            features = features[:n_points]
-        labels = labels[:n_points]
+        features, labels = prep_feat_labels(trial_dataset, n_points)
 
         sensitive_col_indices = [
-            resampled_dataset.sensitive_col_names.index(col)
+            trial_dataset.sensitive_col_names.index(col)
             for col in fairlearn_sensitive_feature_names
         ]
 
         fairlearn_sensitive_features = np.squeeze(
-            resampled_dataset.sensitive_attrs[:, sensitive_col_indices]
+            trial_dataset.sensitive_attrs[:, sensitive_col_indices]
         )[:n_points]
 
         ##############################################
         """" Run Fairlearn algorithm on trial data """
         ##############################################
 
         if fairlearn_constraint_name == "disparate_impact":
@@ -974,54 +939,43 @@
         except:
             print("Error when fitting. Returning NSF")
             solution_found = False
             performance = np.nan
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
+
         if solution_found:
             fairlearn_eval_kwargs["model"] = mitigator
-
+            # predict the class label, not the probability
             performance = perf_eval_fn(y_pred, **fairlearn_eval_kwargs)
 
-        if verbose:
-            print(f"Performance = {performance}")
-
-        ########################################
-        """ Calculate safety on ground truth """
-        ########################################
-        if verbose:
-            print("Determining whether solution " "is actually safe on ground truth")
-
-        # predict the class label, not the probability
-        # Determine whether this solution
-        # violates any of the constraints
-        # on the test dataset
-        failed = False
-        if solution_found:
+            # Determine whether this solution
+            # violates any of the constraints
+            # on the test dataset
             fairlearn_eval_method = fairlearn_eval_kwargs["eval_method"]
-            failed = self.evaluate_constraint_function(
+            gvec = self.evaluate_constraint_function(
                 y_pred=y_pred,
                 test_labels=fairlearn_eval_kwargs["y"],
                 fairlearn_constraint_name=fairlearn_constraint_name,
                 epsilon_eval=fairlearn_epsilon_eval,
                 eval_method=fairlearn_eval_method,
                 sensitive_features=fairlearn_eval_kwargs["sensitive_features"],
             )
-        else:
-            failed = False
+        else:  # solution_found=False
+            n_constraints = len(spec.parse_trees)
+            gvec = -np.inf * np.ones(
+                n_constraints
+            )  # NSF is safe, so set g=-inf for all constraints
+            if verbose:
+                print("NSF")
 
-        if failed:
-            print("Fairlearn trial UNSAFE on ground truth")
-        else:
-            print("Fairlearn trial SAFE on ground truth")
         # Write out file for this data_frac,trial_i combo
-        data = [data_frac, trial_i, performance, failed]
-
-        colnames = ["data_frac", "trial_i", "performance", "failed"]
+        data = [data_frac, trial_i, performance, gvec]
+        colnames = ["data_frac", "trial_i", "performance", "gvec"]
         self.write_trial_result(data, colnames, trial_dir, verbose=kwargs["verbose"])
         return
 
     def get_fairlearn_predictions(self, mitigator, X_test_fairlearn):
         """
         Get the predicted labels from the fairlearn mitigator.
         The mitigator consists of potentially more than one predictor.
@@ -1089,15 +1043,14 @@
 
         :param sensitive_features: List of column names that are considered
                 sensitive in the Fairlearn dataset
         :type sensitive_features: List(str)
         """
         print(f"Evaluating constraint for: {fairlearn_constraint_name}")
         failed = False
-
         if fairlearn_constraint_name == "demographic_parity":
             # g = abs((PR | ATR1) - (PR | ATR2)) - eps
             PR_frame = MetricFrame(
                 metrics=selection_rate,
                 y_true=test_labels,
                 y_pred=y_pred >= 0.5,
                 sensitive_features=sensitive_features,
@@ -1203,13 +1156,8 @@
                 g = abs(FNR_group1 - FNR_group2) - epsilon_eval
         else:
             raise NotImplementedError(
                 "Evaluation for Fairlearn constraints of type: "
                 f"{fairlearn_constraint.short_name} "
                 "is not supported."
             )
-
-        print(f"g (fairlearn) = {g}")
-        if g > 0 or np.isnan(g):
-            failed = True
-
-        return failed
+        return np.array([g])
```

### Comparing `seldonian_experiments-0.1.1/experiments/generate_plots.py` & `seldonian_experiments-0.2.0/experiments/generate_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib.ticker import FormatStrFormatter
 import matplotlib.pyplot as plt
 from matplotlib import style
 
 from seldonian.utils.io_utils import save_pickle
 
 from .experiments import BaselineExperiment, SeldonianExperiment, FairlearnExperiment
-from .utils import generate_resampled_datasets
+from .experiment_utils import generate_resampled_datasets, has_failed
 
 seldonian_model_set = set(["qsa","headless_qsa", "sa"])
 plot_colormap = matplotlib.cm.get_cmap("tab10")
 marker_list = ["s", "p", "d", "*", "x", "h", "+"]
 
 
 class PlotGenerator:
@@ -138,34 +138,25 @@
         :type performance_label: str, defaults to "accuracy"
 
         :param savename: If not None, the filename path to which the plot
                 will be saved on disk.
         :type savename: str, defaults to None
         """
         plt.style.use("bmh")
-        # plt.style.use('grayscale')
         regime = self.spec.dataset.regime
         if regime == "supervised_learning":
             tot_data_size = self.spec.dataset.num_datapoints
         else:
             tot_data_size = self.hyperparameter_and_setting_dict['num_episodes']
 
         # Read in constraints
         parse_trees = self.spec.parse_trees
-
-        constraint_dict = {}
-        for pt_ii, pt in enumerate(parse_trees):
-            delta = pt.delta
-            constraint_str = pt.constraint_str
-            constraint_dict[f"constraint_{pt_ii}"] = {
-                "delta": delta,
-                "constraint_str": constraint_str,
-            }
-
-        constraints = list(constraint_dict.keys())
+        n_constraints = len(parse_trees)
+        constraint_strs = [pt.constraint_str for pt in parse_trees]
+        deltas = [pt.delta for pt in parse_trees]
 
         # Figure out what experiments we have from subfolders in results_dir
         subfolders = [
             os.path.basename(f) for f in os.scandir(self.results_dir) if f.is_dir()
         ]
         all_models = [
             x.split("_results")[0] for x in subfolders if x.endswith("_results")
@@ -183,14 +174,20 @@
             savename_baseline = os.path.join(
                 self.results_dir, f"{baseline}_results", f"{baseline}_results.csv"
             )
             df_baseline = pd.read_csv(savename_baseline)
             df_baseline["solution_returned"] = df_baseline["performance"].apply(
                 lambda x: ~np.isnan(x)
             )
+            df_baseline['gvec'] = df_baseline['gvec'].apply(lambda t: np.fromstring(t[1:-1],sep=' '))
+            new_colnames = ['g' + str(ii) + '_failed' for ii in range(1,n_constraints+1)]
+            for ii in range(len(new_colnames)):
+                colname = new_colnames[ii]
+                df_baseline[colname] = df_baseline['gvec'].str[ii].apply(has_failed)
+            df_baseline = df_baseline.drop('gvec', axis=1)
 
             valid_mask = ~np.isnan(df_baseline["performance"])
             df_baseline_valid = df_baseline[valid_mask]
             # Get the list of all data_fracs
             X_all = df_baseline.groupby("data_frac").mean().index * tot_data_size
             # Get the list of data_fracs for which there is at least one trial that has non-nan performance
             X_valid = (
@@ -209,14 +206,21 @@
             savename_seldonian = os.path.join(
                 self.results_dir,
                 f"{seldonian_model}_results",
                 f"{seldonian_model}_results.csv",
             )
 
             df_seldonian = pd.read_csv(savename_seldonian)
+            df_seldonian['gvec'] = df_seldonian['gvec'].apply(lambda t: np.fromstring(t[1:-1],sep=' '))
+            new_colnames = ['g' + str(ii) + '_failed' for ii in range(1,n_constraints+1)]
+            for ii in range(len(new_colnames)):
+                colname = new_colnames[ii]
+                df_seldonian[colname] = df_seldonian['gvec'].str[ii].apply(has_failed)
+            df_seldonian = df_seldonian.drop('gvec', axis=1)
+
             passed_mask = df_seldonian["passed_safety"] == True
             df_seldonian_passed = df_seldonian[passed_mask]
             # Get the list of all data_fracs
             X_all = df_seldonian.groupby("data_frac").mean().index * tot_data_size
             # Get the list of data_fracs for which there is at least one trial that passed the safety test
             X_passed = (
                 df_seldonian_passed.groupby("data_frac").mean().index * tot_data_size
@@ -225,30 +229,33 @@
             seldonian_dict[seldonian_model][
                 "df_seldonian_passed"
             ] = df_seldonian_passed.copy()
             seldonian_dict[seldonian_model]["X_all"] = X_all
             seldonian_dict[seldonian_model]["X_passed"] = X_passed
 
         ## PLOTTING SETUP
+        vert_size = 3 + n_constraints
         if include_legend:
-            figsize = (9, 4.5)
+            vert_size+=0.5
+            figsize = (9, vert_size)
         else:
-            figsize = (9, 4)
+            figsize = (9, vert_size)
         fig = plt.figure(figsize=figsize)
         plot_index = 1
-        n_rows = len(constraints)
+        n_rows = len(constraint_strs)
         n_cols = 3
         fontsize = fontsize
         legend_fontsize = legend_fontsize
         legend_handles = []
         legend_labels = []
-        ## Loop over constraints and make three plots for each constraint
-        for ii, constraint in enumerate(constraints):
-            constraint_str = constraint_dict[constraint]["constraint_str"]
-            delta = constraint_dict[constraint]["delta"]
+
+        # One row per constraint
+        for constraint_index, constraint_str in enumerate(constraint_strs):
+            constraint_num = constraint_index+1
+            delta = deltas[constraint_index]
 
             # SETUP FOR PLOTTING
             ax_performance = fig.add_subplot(n_rows, n_cols, plot_index)
             plot_index += 1
             ax_sr = fig.add_subplot(n_rows, n_cols, plot_index, sharex=ax_performance)
             plot_index += 1
             ax_fr = fig.add_subplot(n_rows, n_cols, plot_index, sharex=ax_performance)
@@ -260,22 +267,19 @@
                     title = custom_title
                 else:
                     title = f"constraint: \ng={constraint_str}"
                 ax_sr.set_title(title, y=1.05, fontsize=10)
 
             # Plot labels
             ax_performance.set_ylabel(performance_label, fontsize=fontsize)
-            ax_sr.set_ylabel("Probability of solution", fontsize=fontsize)
-            ax_fr.set_ylabel("Probability constraint was violated", fontsize=fontsize)
+            ax_sr.set_ylabel("Prob. of solution", fontsize=fontsize)
+            ax_fr.set_ylabel("Prob. of violation", fontsize=fontsize)
 
             # Only put horizontal axis labels on last row of plots
-            if ii == len(constraints) - 1:
-                # ax_performance.set_xlabel('Training samples',fontsize=fontsize)
-                # ax_sr.set_xlabel('Training samples',fontsize=fontsize)
-                # ax_fr.set_xlabel('Training samples',fontsize=fontsize)
+            if constraint_index == n_constraints - 1:
                 ax_performance.set_xlabel("Amount of data", fontsize=fontsize)
                 ax_sr.set_xlabel("Amount of data", fontsize=fontsize)
                 ax_fr.set_xlabel("Amount of data", fontsize=fontsize)
 
             # axis scaling
             ax_performance.set_xscale("log")
             if performance_yscale.lower() == "log":
@@ -319,19 +323,20 @@
                 X_valid_baseline = this_baseline_dict["X_valid"]
                 (pl,) = ax_performance.plot(
                     X_valid_baseline.to_numpy(),
                     baseline_mean_performance.to_numpy(),
                     color=baseline_color,
                     label=baseline,
                 )
-                legend_handles.append(pl)
-                if baseline in model_label_dict:
-                    legend_labels.append(model_label_dict[baseline])
-                else:
-                    legend_labels.append(baseline)
+                if constraint_index == 0:
+                    legend_handles.append(pl)
+                    if baseline in model_label_dict:
+                        legend_labels.append(model_label_dict[baseline])
+                    else:
+                        legend_labels.append(baseline)
                 ax_performance.scatter(
                     X_valid_baseline,
                     baseline_mean_performance,
                     color=baseline_color,
                     s=marker_size,
                     marker=marker_list[baseline_i],
                 )
@@ -361,19 +366,20 @@
                 X_passed_seldonian = this_seldonian_dict["X_passed"].to_numpy()
                 (pl,) = ax_performance.plot(
                     X_passed_seldonian,
                     mean_performance,
                     color=seldonian_color,
                     linestyle="--",
                 )
-                legend_handles.append(pl)
-                if seldonian_model in model_label_dict:
-                    legend_labels.append(model_label_dict[seldonian_model])
-                else:
-                    legend_labels.append(seldonian_model)
+                if constraint_index == 0:
+                    legend_handles.append(pl)
+                    if seldonian_model in model_label_dict:
+                        legend_labels.append(model_label_dict[seldonian_model])
+                    else:
+                        legend_labels.append(seldonian_model)
 
                 ax_performance.scatter(
                     X_passed_seldonian,
                     mean_performance,
                     color=seldonian_color,
                     s=marker_size,
                     marker="o",
@@ -465,58 +471,72 @@
             ##########################
 
             # Baseline failure rate
             for baseline_i, baseline in enumerate(baselines):
                 baseline_color = plot_colormap(baseline_i + len(seldonian_models))
                 # Baseline performance
                 this_baseline_dict = baseline_dict[baseline]
-                df_baseline_valid = this_baseline_dict["df_baseline_valid"]
-                n_trials = df_baseline_valid["trial_i"].max() + 1
+                df_baseline = this_baseline_dict["df_baseline"]
+                n_trials = df_baseline["trial_i"].max() + 1
 
-                baseline_mean_fr = df_baseline_valid.groupby("data_frac").mean()[
-                    "failed"
-                ].to_numpy()
-                baseline_std_fr = df_baseline_valid.groupby("data_frac").std()["failed"].to_numpy()
+                # baseline_mean_fr = df_baseline_valid.groupby("data_frac").mean()[
+                #     "failed"
+                # ].to_numpy()
+                # baseline_std_fr = df_baseline_valid.groupby("data_frac").std()["failed"].to_numpy()
+                gstr_failed = 'g' + str(constraint_num) + '_failed'
+
+                baseline_mean_fr = df_baseline.groupby("data_frac").mean()[
+                    gstr_failed].to_numpy()
+                # Need to groupby data frac
+                baseline_std_fr = df_baseline.groupby("data_frac").std()[
+                    gstr_failed].to_numpy()
                 baseline_ste_fr = baseline_std_fr / np.sqrt(n_trials)
 
-                X_valid_baseline = this_baseline_dict["X_valid"].to_numpy()
+                X_all_baseline = this_baseline_dict["X_all"].to_numpy()
 
                 ax_fr.plot(
-                    X_valid_baseline,
+                    X_all_baseline,
                     baseline_mean_fr,
                     color=baseline_color,
                     label=baseline,
                 )
                 ax_fr.scatter(
-                    X_valid_baseline,
+                    X_all_baseline,
                     baseline_mean_fr,
                     color=baseline_color,
                     marker=marker_list[baseline_i],
                     s=marker_size,
                 )
                 ax_fr.fill_between(
-                    X_valid_baseline,
+                    X_all_baseline,
                     baseline_mean_fr - baseline_ste_fr,
                     baseline_mean_fr + baseline_ste_fr,
                     color=baseline_color,
                     alpha=0.5,
                 )
 
             # Seldonian failure rate
             for seldonian_i, seldonian_model in enumerate(seldonian_models):
                 this_seldonian_dict = seldonian_dict[seldonian_model]
                 seldonian_color = plot_colormap(seldonian_i)
                 df_seldonian = this_seldonian_dict["df_seldonian"]
                 n_trials = df_seldonian["trial_i"].max() + 1
-                mean_fr = df_seldonian.groupby("data_frac").mean()["failed"].to_numpy()
-                std_fr = df_seldonian.groupby("data_frac").std()["failed"].to_numpy()
+
+                gstr_failed = 'g' + str(constraint_num) + '_failed'
+
+                mean_fr = df_seldonian.groupby("data_frac").mean()[
+                    gstr_failed].to_numpy()
+                # Need to groupby data frac
+                std_fr = df_seldonian.groupby("data_frac").std()[
+                    gstr_failed].to_numpy()
+
                 ste_fr = std_fr / np.sqrt(n_trials)
 
                 X_all_seldonian = this_seldonian_dict["X_all"].to_numpy()
-                
+
                 ax_fr.plot(
                     X_all_seldonian,
                     mean_fr,
                     color=seldonian_color,
                     linestyle="--",
                     label="QSA",
                 )
@@ -677,15 +697,14 @@
 
         ## Run experiment
         sd_exp = SeldonianExperiment(model_name="qsa", results_dir=self.results_dir)
 
         sd_exp.run_experiment(**run_seldonian_kwargs)
         return
 
-
     def run_headless_seldonian_experiment(
         self, 
         full_pretraining_model,
         initial_state_dict, 
         headless_pretraining_model, 
         head_layer_names,
         latent_feature_shape,
@@ -744,24 +763,18 @@
         sd_exp = HeadlessSeldonianExperiment(
             model_name="headless_qsa",
             results_dir=self.results_dir)
 
         sd_exp.run_experiment(**run_kwargs)
         return
 
-
-
-    def run_baseline_experiment(self, model_name, verbose=False):
+    def run_baseline_experiment(self, baseline_model, verbose=False):
         """Run a supervised Seldonian experiment using the spec attribute
         assigned to the class in __init__().
 
-        :param model_name: The name of the baseline model to use
-
-        :type model_name: str
-
         :param verbose: Whether to display results to stdout
                 while the Seldonian algorithms are running in each trial
         :type verbose: bool, defaults to False
         """
 
         dataset = self.spec.dataset
 
@@ -784,15 +797,15 @@
             constraint_eval_fns=self.constraint_eval_fns,
             constraint_eval_kwargs=self.constraint_eval_kwargs,
             batch_epoch_dict=self.batch_epoch_dict,
             verbose=verbose,
         )
 
         ## Run experiment
-        bl_exp = BaselineExperiment(model_name=model_name, results_dir=self.results_dir)
+        bl_exp = BaselineExperiment(baseline_model=baseline_model, results_dir=self.results_dir)
 
         bl_exp.run_experiment(**run_baseline_kwargs)
         return
 
     def run_fairlearn_experiment(
         self,
         fairlearn_sensitive_feature_names,
```

### Comparing `seldonian_experiments-0.1.1/experiments/headless_example.py` & `seldonian_experiments-0.2.0/experiments/headless_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,26 @@
         batch_epoch_dict_pretraining,
         safety_batch_size_pretraining,
         n_trials,
         data_fracs,
         results_dir,
         perf_eval_fn,
         perf_eval_kwargs,
+        constraint_eval_kwargs,
         n_workers=1,
         batch_epoch_dict={},
         datagen_method="resample",
         verbose=False,
         baselines=[],
         performance_label="performance",
         performance_yscale="linear",
         plot_savename=None,
         plot_fontsize=12,
         legend_fontsize=8,
+        model_label_dict={},
     ):
         """Run the experiment for this example.
         Runs any baseline models included in baselines
         parameter first. Then produces the three plots.
         """
         # assert baselines == [], "No baselines supported for headless examples yet"
         os.makedirs(results_dir, exist_ok=True)
@@ -50,24 +52,24 @@
             data_fracs=data_fracs,
             n_workers=n_workers,
             datagen_method=datagen_method,
             perf_eval_fn=perf_eval_fn,
             constraint_eval_fns=[],
             results_dir=results_dir,
             perf_eval_kwargs=perf_eval_kwargs,
+            constraint_eval_kwargs=constraint_eval_kwargs,
             batch_epoch_dict=batch_epoch_dict,
         )
 
         # Baselines first
         for baseline_model in baselines:
             plot_generator.run_baseline_experiment(
-                model_name=baseline_model, verbose=verbose
+                baseline_model=baseline_model, verbose=verbose
             )
         
-
         # Run Seldonian headless experiment
         # A special thing we need to do for headless experiments is get the 
         # initial weights of the model and freeze them so we can 
         # re-initialize the same weights in each train when we pretrain
         initial_state_dict = full_pretraining_model.state_dict()
 
         plot_generator.run_headless_seldonian_experiment(
@@ -84,9 +86,10 @@
             verbose=verbose)
 
         plot_generator.make_plots(
             fontsize=plot_fontsize,
             legend_fontsize=legend_fontsize,
             performance_label=performance_label,
             performance_yscale=performance_yscale,
+            model_label_dict=model_label_dict,
             savename=plot_savename,
         )
```

### Comparing `seldonian_experiments-0.1.1/experiments/headless_experiments.py` & `seldonian_experiments-0.2.0/experiments/headless_experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import os
 import numpy as np
 from functools import partial
 
 from .experiments import Experiment 
 from . import headless_utils
-from .utils import batch_predictions
+from .experiment_utils import batch_predictions
 
 from seldonian.dataset import SupervisedDataSet
 from seldonian.seldonian_algorithm import SeldonianAlgorithm
 from seldonian.utils.io_utils import load_pickle
 
 import warnings
 from seldonian.warnings.custom_warnings import *
@@ -125,17 +125,14 @@
                     f"Trial {trial_i} already run for "
                     f"this data_frac: {data_frac}. Skipping this trial. "
                 )
             return
 
         os.makedirs(trial_dir, exist_ok=True)
 
-        parse_trees = spec.parse_trees
-        dataset = spec.dataset
-
         ##############################################
         """ Setup for running Seldonian algorithm """
         ##############################################
 
         if regime != "supervised_learning":
             raise NotImplementedError(
                 "Headless experiments are only available for supervised_learning")
@@ -192,14 +189,15 @@
             print(f"With data_frac: {data_frac}, have {n_points} data points")
 
         # Obtain latent features by training the full model 
         # and then passing the data through a headless version of this model
 
         # First re-initialize weights
         full_pretraining_model.load_state_dict(initial_state_dict)
+        
         latent_features = headless_utils.generate_latent_features(
             full_pretraining_model=full_pretraining_model,
             headless_pretraining_model=headless_pretraining_model,
             head_layer_names=head_layer_names,
             orig_features=features,
             labels=labels, 
             latent_feature_shape=latent_feature_shape,
@@ -227,14 +225,16 @@
 
         # If optimizing using gradient descent,
         # and using mini-batches,
         # update the batch_size and n_epochs
         # using batch_epoch_dict
         if spec_for_experiment.optimization_technique == "gradient_descent":
             if spec_for_experiment.optimization_hyperparams["use_batches"] == True:
+                if verbose:
+                    print("Using batches in Seldonian trial")
                 batch_size, n_epochs = batch_epoch_dict[data_frac]
                 spec_for_experiment.optimization_hyperparams["batch_size"] = batch_size
                 spec_for_experiment.optimization_hyperparams["n_epochs"] = n_epochs
         ################################
         """" Run Seldonian algorithm """
         ################################
 
@@ -256,16 +256,14 @@
         if type(solution) == str and solution == "NSF":
             solution_found = False
 
         #########################################################
         """" Calculate performance and safety on ground truth """
         #########################################################
 
-        failed = False  # flag for whether we were actually safe on test set
-
         if solution_found:
             solution = copy.deepcopy(solution)
             # If passed the safety test, calculate performance
             # using solution
             if passed_safety:
                 if verbose:
                     print("Passed safety test! Calculating performance")
@@ -317,38 +315,43 @@
                         constraint_eval_kwargs["eval_batch_size"] = perf_eval_kwargs["eval_batch_size"]
                     constraint_eval_kwargs["spec_orig"] = spec
                     constraint_eval_kwargs["spec_for_experiment"] = spec_for_experiment
                     constraint_eval_kwargs["regime"] = regime
                     constraint_eval_kwargs["branch"] = "safety_test"
                     constraint_eval_kwargs["verbose"] = verbose
 
-                failed = self.evaluate_constraint_functions(
+                gvec = self.evaluate_constraint_functions(
                     solution=solution,
                     constraint_eval_fns=constraint_eval_fns,
                     constraint_eval_kwargs=constraint_eval_kwargs,
                 )
 
                 if verbose:
-                    if failed:
-                        print("Solution was not actually safe on ground truth!")
-                    else:
-                        print("Solution was safe on ground truth")
+                    print(f"gvec: {gvec}")
                     print()
             else:
                 if verbose:
                     print("Failed safety test ")
                     performance = np.nan
 
         else:
+            n_constraints = len(spec.parse_trees)
+            gvec = -np.inf*np.ones(n_constraints) # NSF is safe, so set g=-inf for all constraints
             if verbose:
                 print("NSF")
             performance = np.nan
+
+        # Clear out any cached data in the parse trees for the next trial.
+        # This handles the case where solution_found=False.
+        for parse_tree in spec_for_experiment.parse_trees:
+            parse_tree.reset_base_node_dict(reset_data=True)
+            
         # Write out file for this data_frac,trial_i combo
-        data = [data_frac, trial_i, performance, passed_safety, failed]
-        colnames = ["data_frac", "trial_i", "performance", "passed_safety", "failed"]
+        data = [data_frac, trial_i, performance, passed_safety, gvec]
+        colnames = ["data_frac", "trial_i", "performance", "passed_safety", "gvec"]
         self.write_trial_result(data, colnames, trial_dir, verbose=kwargs["verbose"])
         return
 
     def evaluate_constraint_functions(
         self, solution, constraint_eval_fns, constraint_eval_kwargs
     ):
         """Helper function for QSA() to evaluate
@@ -368,15 +371,15 @@
         :param constraint_eval_kwargs: keyword arguments
                 to pass to each constraint function
                 in constraint_eval_fns
         :type constraint_eval_kwargs: dict
         """
         # Use safety test branch so the confidence bounds on
         # leaf nodes are not inflated
-        failed = False
+        gvals = []
         if constraint_eval_fns == []:
             """User did not provide their own functions
             to evaluate the constraints. Use the default:
             the parse tree has a built-in way to evaluate constraints.
             """
             constraint_eval_kwargs["theta"] = solution
             orig_dataset = constraint_eval_kwargs["spec_orig"].dataset
@@ -399,18 +402,18 @@
                 constraint_eval_kwargs["dataset"] = dataset_for_eval
 
             for parse_tree in spec_for_experiment.parse_trees:
                 parse_tree.reset_base_node_dict(reset_data=True)
                 parse_tree.evaluate_constraint(**constraint_eval_kwargs)
 
                 g = parse_tree.root.value
-                if g > 0 or np.isnan(g):
-                    failed = True
+                gvals.append(g)
+                parse_tree.reset_base_node_dict(reset_data=True) # to clear out anything so the next trial has fresh data
 
         else:
             # User provided functions to evaluate constraints
             for eval_fn in constraint_eval_fns:
                 g = eval_fn(solution)
-                if g > 0 or np.isnan(g):
-                    failed = True
-        return failed
+                gvals.append(g)
+        
+        return np.array(gvals)
```

### Comparing `seldonian_experiments-0.1.1/experiments/headless_utils.py` & `seldonian_experiments-0.2.0/experiments/headless_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.1/experiments/utils.py` & `seldonian_experiments-0.2.0/experiments/experiment_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Utilities used in the rest of the library """
 
-import os
-import pickle
+import os, copy, pickle, math
 import numpy as np
-import math
 
 from seldonian.RL.RL_runner import create_agent, run_trial_given_agent_and_env
 from seldonian.utils.stats_utils import weighted_sum_gamma
-from seldonian.dataset import SupervisedDataSet
+from seldonian.dataset import SupervisedDataSet,RLDataSet
+from seldonian.utils.io_utils import load_pickle
+
 
 def generate_resampled_datasets(dataset, n_trials, save_dir):
     """Utility function for supervised learning to generate the
     resampled datasets to use in each trial. Resamples (with replacement)
     features, labels and sensitive attributes to create n_trials versions of these
     of the same shape as the inputs
 
@@ -63,14 +63,180 @@
                 meta_information=dataset.meta_information,
             )
 
             with open(savename, "wb") as outfile:
                 pickle.dump(resampled_dataset, outfile)
             print(f"Saved {savename}")
 
+
+def load_resampled_dataset(results_dir, trial_i, data_frac, verbose=False):
+    """Utility function for supervised learning to generate the
+    resampled datasets to use in each trial. Resamples (with replacement)
+    features, labels and sensitive attributes to create n_trials versions of these
+    of the same shape as the inputs
+
+    :param results_dir: The directory in which results are saved for this trial
+    :type results_dir: str
+
+    :param trial_i: Trial index
+    :type trial_i: int
+
+    :param data_frac: data fraction
+    :type data_frac: float
+
+    :param verbose: boolean verbosity flag
+    """
+    resampled_filename = os.path.join(
+        results_dir, "resampled_dataframes", f"trial_{trial_i}.pkl"
+    )
+    resampled_dataset = load_pickle(resampled_filename)
+    num_datapoints_tot = resampled_dataset.num_datapoints
+    n_points = int(round(data_frac * num_datapoints_tot))
+
+    if verbose:
+        print(
+            f"Using resampled dataset {resampled_filename} "
+            f"with {num_datapoints_tot} datapoints"
+        )
+    if n_points < 1:
+        raise ValueError(
+            f"This data_frac={data_frac} "
+            f"results in {n_points} data points. "
+            "Must have at least 1 data point to run a trial."
+        )
+    return resampled_dataset, n_points
+
+
+def prep_feat_labels(trial_dataset, n_points, include_sensitive_attrs=False):
+    """Utility function for preparing features and labels
+    for a given trial
+
+    :param trial_dataset: The Seldonian dataset object containing trial data
+    :param n_points: Number of points in this trial
+    :type n_points: int
+    :param include_sensitive_attrs: Whether to prep and return sensitive attributes
+        as well.
+    :type include_sensitive_attrs: bool
+    """
+    features = trial_dataset.features
+    labels = trial_dataset.labels
+    # Only use first n_points for this trial
+    if type(features) == list:
+        features = [x[:n_points] for x in features]
+    else:
+        features = features[:n_points]
+    labels = labels[:n_points]
+
+    if include_sensitive_attrs:
+        sensitive_attrs = trial_dataset.sensitive_attrs
+        sensitive_attrs = sensitive_attrs[:n_points]
+        return features, labels, sensitive_attrs
+
+    return features, labels
+
+
+def setup_SA_spec_for_exp(
+    spec,
+    regime,
+    results_dir,
+    trial_i,
+    data_frac,
+    datagen_method,
+    batch_epoch_dict,
+    kwargs,
+    perf_eval_kwargs,
+):
+    if regime == "supervised_learning":
+        if datagen_method == "resample":
+            trial_dataset, n_points = load_resampled_dataset(
+                results_dir, trial_i, data_frac
+            )
+
+        else:
+            raise NotImplementedError(
+                f"Eval method {datagen_method} " f"not supported for regime={regime}"
+            )
+
+        features, labels, sensitive_attrs = prep_feat_labels(
+            trial_dataset, n_points, include_sensitive_attrs=True
+        )
+
+        dataset_for_exp = SupervisedDataSet(
+            features=features,
+            labels=labels,
+            sensitive_attrs=sensitive_attrs,
+            num_datapoints=n_points,
+            meta_information=trial_dataset.meta_information,
+        )
+
+        # Make a new spec object and update its dataset
+        spec_for_exp = copy.deepcopy(spec)
+        spec_for_exp.dataset = dataset_for_exp
+
+    elif regime == "reinforcement_learning":
+        hyperparameter_and_setting_dict = kwargs["hyperparameter_and_setting_dict"]
+
+        if datagen_method == "generate_episodes":
+            n_episodes_for_eval = perf_eval_kwargs["n_episodes_for_eval"]
+            # Sample from resampled dataset on disk of n_episodes
+            save_dir = os.path.join(results_dir, "regenerated_datasets")
+
+            savename = os.path.join(save_dir, f"regenerated_data_trial{trial_i}.pkl")
+
+            episodes_all = load_pickle(savename)
+            # Take data_frac episodes from this df
+            n_episodes_all = len(episodes_all)
+
+            n_episodes_for_exp = int(round(n_episodes_all * data_frac))
+            if n_episodes_for_exp < 1:
+                raise ValueError(
+                    f"This data_frac={data_frac} "
+                    f"results in {n_episodes_for_exp} episodes. "
+                    "Must have at least 1 episode to run a trial."
+                )
+
+            print(f"Orig dataset should have {n_episodes_all} episodes")
+            print(
+                f"This dataset with data_frac={data_frac} should have"
+                f" {n_episodes_for_exp} episodes"
+            )
+
+            # Take first n_episodes episodes
+            episodes_for_exp = episodes_all[0:n_episodes_for_exp]
+            assert len(episodes_for_exp) == n_episodes_for_exp
+
+            dataset_for_exp = RLDataSet(
+                episodes=episodes_for_exp,
+                meta_information=spec.dataset.meta_information,
+                regime=regime,
+            )
+
+            # Make a new spec object from a copy of spec, where the
+            # only thing that is different is the dataset
+
+            spec_for_exp = copy.deepcopy(spec)
+            spec_for_exp.dataset = dataset_for_exp
+        else:
+            raise NotImplementedError(
+                f"Eval method {datagen_method} not supported for regime={regime}"
+            )
+
+    """ If optimizing using gradient descent and using mini-batches,
+     update the batch_size and n_epochs using batch_epoch_dict """
+    if (
+        batch_epoch_dict != {}
+        and spec_for_exp.optimization_technique == "gradient_descent"
+        and (spec_for_exp.optimization_hyperparams["use_batches"] == True)
+    ):
+        batch_size, n_epochs = batch_epoch_dict[data_frac]
+        spec_for_exp.optimization_hyperparams["batch_size"] = batch_size
+        spec_for_exp.optimization_hyperparams["n_epochs"] = n_epochs
+    return spec_for_exp
+
+
 def generate_episodes_and_calc_J(**kwargs):
     """Calculate the expected discounted return
     by generating episodes
 
     :return: episodes, J, where episodes is the list
             of generated ground truth episodes and J is
             the expected discounted return
@@ -95,14 +261,15 @@
     )
 
     # Calculate J, the discounted sum of rewards
     returns = np.array([weighted_sum_gamma(ep.rewards, env.gamma) for ep in episodes])
     J = np.mean(returns)
     return episodes, J
 
+
 def batch_predictions(model, solution, X_test, **kwargs):
     batch_size = kwargs["eval_batch_size"]
     if type(X_test) == list:
         N_eval = len(X_test[0])
     else:
         N_eval = len(X_test)
     if "N_output_classes" in kwargs:
@@ -119,138 +286,85 @@
             X_test_batch = [x[batch_start:batch_end] for x in X_test]
         else:
             X_test_batch = X_test[batch_start:batch_end]
         y_pred[batch_start:batch_end] = model.predict(solution, X_test_batch)
         batch_start = batch_end
     return y_pred
 
-def make_batch_epoch_dict_fixedniter(niter,data_fracs,N_max,batch_size):
+
+def make_batch_epoch_dict_fixedniter(niter, data_fracs, N_max, batch_size):
     """
     Convenience function for figuring out the number of epochs necessary
-    to ensure that at each data fraction, the total 
-    number of iterations (and batch size) will be fixed. 
+    to ensure that at each data fraction, the total
+    number of iterations (and batch size) will be fixed.
 
     :param niter: The total number of iterations you want run at every data_frac
     :type niter: int
     :param data_fracs: 1-D array of data fractions
-    :type data_fracs: np.ndarray 
+    :type data_fracs: np.ndarray
     :param N_max: The maximum number of data points in the optimization process
     :type N_max: int
-    :param batch_size: The fixed batch size 
+    :param batch_size: The fixed batch size
     :type batch_size: int
-    :return batch_epoch_dict: A dictionary where keys are data fractions 
+    :return batch_epoch_dict: A dictionary where keys are data fractions
         and values are [batch_size,num_epochs]
     """
-    data_sizes=data_fracs*N_max # number of points used in candidate selection in each data frac
-    n_batches=data_sizes/batch_size # number of batches in each data frac
-    n_batches=np.array([math.ceil(x) for x in n_batches])
-    n_epochs_arr=niter/n_batches # number of epochs needed to get to niter iterations in each data frac
+    data_sizes = (
+        data_fracs * N_max
+    )  # number of points used in candidate selection in each data frac
+    n_batches = data_sizes / batch_size  # number of batches in each data frac
+    n_batches = np.array([math.ceil(x) for x in n_batches])
+    n_epochs_arr = (
+        niter / n_batches
+    )  # number of epochs needed to get to niter iterations in each data frac
     n_epochs_arr = np.array([math.ceil(x) for x in n_epochs_arr])
     batch_epoch_dict = {
-        data_fracs[ii]:[batch_size,n_epochs_arr[ii]] for ii in range(len(data_fracs))}
+        data_fracs[ii]: [batch_size, n_epochs_arr[ii]] for ii in range(len(data_fracs))
+    }
     return batch_epoch_dict
 
+
 def make_batch_epoch_dict_min_sample_repeat(
-    niter_min,
-    data_fracs,
-    N_max,
-    batch_size,
-    num_repeats):
+    niter_min, data_fracs, N_max, batch_size, num_repeats
+):
     """
     Convenience function for figuring out the number of epochs necessary
     to ensure that the number of iterations for each data frac is:
     max(niter_min,# of iterations s.t. each sample is seen num_repeat times)
 
     :param niter_min: The minimum total number of iterations you want run at every data_frac
     :type niter_min: int
     :param data_fracs: 1-D array of data fractions
-    :type data_fracs: np.ndarray 
+    :type data_fracs: np.ndarray
     :param N_max: The maximum number of data points in the optimization process
     :type N_max: int
     :param batch_size: The fixed batch size
     :type batch_size: int
     :param num_repeats: The minimum number of times each sample must be seen in the optimization process
     :type num_repeats: int
-    :return batch_epoch_dict: A dictionary where keys are data fractions 
+    :return batch_epoch_dict: A dictionary where keys are data fractions
         and values are [batch_size,num_epochs]
     """
     batch_epoch_dict = {}
     n_epochs_arr = np.zeros_like(data_fracs)
     for data_frac in data_fracs:
-        niter2 = num_repeats*N_max*data_frac/batch_size
+        niter2 = num_repeats * N_max * data_frac / batch_size
         if niter2 > niter_min:
             num_epochs = num_repeats
         else:
-            n_batches = max(1,N_max*data_frac/batch_size)
-            num_epochs = math.ceil(niter_min/n_batches)
-        batch_epoch_dict[data_frac] = [batch_size,num_epochs]
-    
-    return batch_epoch_dict
-
-##### performance evaluation functions #####
-
-def binary_logistic_loss(y_pred,y,**kwargs):    
-    return log_loss(y,y_pred)
-
-def multiclass_logistic_loss(y_pred, y, **kwargs):
-    """Calculate average logistic loss
-    over all data points for multi-class classification
+            n_batches = max(1, N_max * data_frac / batch_size)
+            num_epochs = math.ceil(niter_min / n_batches)
+        batch_epoch_dict[data_frac] = [batch_size, num_epochs]
 
-    :return: logistic loss
-    :rtype: float
-    """
-    # In the multi-class setting, y_pred is an i x k matrix
-    # where i is the number of samples and k is the number of classes
-    # Each entry is the probability of predicting the kth class
-    # for the ith sample. We need to get the probability of predicting
-    # the true class for each sample and then take the sum of the
-    # logs of that.
-    n = len(y)
-    probs_trueclasses = y_pred[np.arange(n), y.astype("int")]
-    return -1 / n * sum(np.log(probs_trueclasses))
-
-def probabilistic_accuracy(y_pred, y, **kwargs):
-    """For binary classification only.
-    1 - error rate. Use when output of 
-    model y_pred is a probability
-
-    :param y_pred: Array of predicted probabilities of each label
-    :param y: Array of true labels, 1-dimensional
-
-    """
-    v = np.where(y != 1.0, 1.0 - y_pred, y_pred)
-    return sum(v) / len(v)
-
-def multiclass_accuracy(y_pred,y,**kwargs):
-    """For multi-class classification.
-    1 - error rate. Use when output of 
-    model y_pred is a probability
-
-    :param y_pred: Array of predicted probabilities of each label
-    :param y: Array of true labels, 1-dimensional
-
-    """
-    n = len(y)
-    return np.sum(y_pred[np.arange(n),y.astype("int")])/n
-
-def deterministic_accuracy(y_pred, y, **kwargs):
-    """The fraction of correct samples. Best to use
-    only when the output of the model, y_pred
-    is 0 or 1. 
-
-    :param y_pred: Array of predicted labels
-    :param y: Array of true labels
+    return batch_epoch_dict
 
-    """
-    from sklearn.metrics import accuracy_score
-    return accuracy_score(y,y_pred > 0.5)
 
+def has_failed(g):
+    """Condition for whether a value of g is unsafe. This is used
+    to determine the failure rate in the right-most plot of the experiments plots.
 
-def MSE(y_pred, y, **kwargs):
-    """Calculate sample mean squared error
+    :param g: The value of the behavioral constraint evaluated using a model and data
+    :type g: float
 
-    :param y_pred: Array of predicted labels
-    :param y: Array of true labels
+    :return: True if g is unsafe, False if g is safe
     """
-    n = len(y)
-    res = sum(pow(y_pred - y, 2)) / n
-    return res
+    return g > 0 or np.isnan(g)
```

### Comparing `seldonian_experiments-0.1.1/seldonian_experiments.egg-info/PKG-INFO` & `seldonian_experiments-0.2.0/seldonian_experiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-experiments
-Version: 0.1.1
+Version: 0.2.0
 Summary: Library for running experiments with Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Experiments/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_experiments-0.1.1/seldonian_experiments.egg-info/SOURCES.txt` & `seldonian_experiments-0.2.0/seldonian_experiments.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 setup.py
 examples/__init__.py
 examples/run_examples.py
 experiments/__init__.py
 experiments/base_example.py
+experiments/experiment_utils.py
 experiments/experiments.py
 experiments/generate_plots.py
 experiments/headless_example.py
 experiments/headless_experiments.py
 experiments/headless_utils.py
-experiments/utils.py
+experiments/perf_eval_funcs.py
 seldonian_experiments.egg-info/PKG-INFO
 seldonian_experiments.egg-info/SOURCES.txt
 seldonian_experiments.egg-info/dependency_links.txt
 seldonian_experiments.egg-info/requires.txt
 seldonian_experiments.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_examples.py
 tests/test_experiments.py
 tests/test_generate_plots.py
```

### Comparing `seldonian_experiments-0.1.1/setup.py` & `seldonian_experiments-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_experiments",
-    version="0.1.1",
+    version="0.2.0",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Library for running experiments with Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_experiments-0.1.1/tests/conftest.py` & `seldonian_experiments-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldonian_experiments-0.1.1/tests/test_generate_plots.py` & `seldonian_experiments-0.2.0/tests/test_generate_plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import numpy as np
 import pandas as pd
 
 import pytest
 
-from sklearn.metrics import log_loss,accuracy_score
-
 from experiments.generate_plots import (
 	SupervisedPlotGenerator,RLPlotGenerator)
 
-from experiments.utils import MSE,generate_episodes_and_calc_J
+from experiments.experiment_utils import (
+	generate_episodes_and_calc_J,has_failed)
+
+from experiments.perf_eval_funcs import (MSE,probabilistic_accuracy)
 
 from seldonian.RL.environments.gridworld import Gridworld
 
 @pytest.mark.parametrize('experiment', ["./tests/static/results"], indirect=True)
 def test_regression_plot_generator(gpa_regression_spec,experiment):
 	np.random.seed(42)
 	constraint_strs = ['Mean_Squared_Error - 3.0','2.0 - Mean_Squared_Error']
@@ -66,243 +67,47 @@
 	# Make sure length of df is correct
 	df = pd.read_csv(results_file)
 	assert len(df) == 4
 	dps = df.data_frac
 	trial_is = df.trial_i
 	perfs = df.performance
 	passed_safetys = df.passed_safety
-	faileds = df.failed
+	gvecs = df.gvec.apply(lambda t: np.fromstring(t[1:-1],sep=' '))
 	
 	assert dps[0] == 0.01
 	assert trial_is[0] == 0
+	assert passed_safetys[0] == False
+	assert gvecs.str[0][0] == -np.inf
 
 	assert dps[1] == 0.01
 	assert trial_is[1] == 1
+	assert passed_safetys[1] == False
+	assert gvecs.str[0][1] == -np.inf
 
 	assert dps[2] == 0.1
 	assert trial_is[2] == 0
+	assert passed_safetys[2] == False
+	assert gvecs.str[0][2] == -np.inf
 
 	assert dps[3] == 0.1
 	assert trial_is[3] == 1
+	assert passed_safetys[3] == False
+	assert gvecs.str[0][3] == -np.inf
 	
 	# Make sure number of trial files created is correct
 	trial_dir = os.path.join(results_dir,"qsa_results/trial_data")
 	trial_files = os.listdir(trial_dir)
 	assert len(trial_files) == 4
 
 	# Make sure the trial files have the right format
 	trial_file_0 = os.path.join(trial_dir,trial_files[0])
 	df_trial0 = pd.read_csv(trial_file_0)
 	assert len(df_trial0) == 1
 
 @pytest.mark.parametrize('experiment', ["./tests/static/results"], indirect=True)
-def test_classification_plot_generator(gpa_classification_spec,experiment):
-	np.random.seed(42)
-	constraint_strs = ['abs((PR | [M]) - (PR | [F])) <= 0.2']
-	deltas = [0.05]
-	spec = gpa_classification_spec(constraint_strs,deltas)
-	n_trials = 2
-	data_fracs = [0.01,0.1]
-	datagen_method="resample"
-	performance_metric = 'accuracy'
-	def perf_eval_fn(y_pred,y,**kwargs):
-		if performance_metric == 'log_loss':
-			return log_loss(y,y_pred)
-		elif performance_metric == 'accuracy':
-			return accuracy_score(y,y_pred > 0.5)
-
-	perf_eval_fn = perf_eval_fn
-	results_dir = "./tests/static/results"
-	n_workers = 1
-	# Get performance evaluation kwargs set up
-	# Use entire original dataset as ground truth for test set
-	dataset = spec.dataset
-	test_features = dataset.features
-	test_labels = dataset.labels
-
-	# Define any additional keyword arguments (besides theta)
-	# of the performance evaluation function,
-	# which in our case is accuracy
-	perf_eval_kwargs = {
-		'X':test_features,
-		'y':test_labels,
-		}
-	
-	spg = SupervisedPlotGenerator(
-		spec=spec,
-		n_trials=n_trials,
-		data_fracs=data_fracs,
-		datagen_method=datagen_method,
-		perf_eval_fn=perf_eval_fn,
-		results_dir=results_dir,
-		n_workers=n_workers,
-		constraint_eval_fns=[],
-		perf_eval_kwargs=perf_eval_kwargs,
-		constraint_eval_kwargs={})
-	
-	assert spg.n_trials == n_trials
-	assert spg.regime == 'supervised_learning'
-
-	# Run two baselines and test that files are created correctly
-	for baseline_model_name in ['random_classifier','logistic_regression']:
-		spg.run_baseline_experiment(
-			model_name=baseline_model_name,verbose=True)
-
-		## Make sure results file was created
-		baseline_results_file = os.path.join(results_dir,
-			f"{baseline_model_name}_results/{baseline_model_name}_results.csv")
-		assert os.path.exists(baseline_results_file)
-
-		# Make sure length of df is correct
-		baseline_df = pd.read_csv(baseline_results_file)
-		assert len(baseline_df) == 4
-		dps = baseline_df.data_frac
-		trial_is = baseline_df.trial_i
-		perfs = baseline_df.performance
-		faileds = baseline_df.failed
-	
-		assert dps[0] == 0.01
-		assert trial_is[0] == 0
-
-		assert dps[1] == 0.01
-		assert trial_is[1] == 1
-
-		assert dps[2] == 0.1
-		assert trial_is[2] == 0
-
-		assert dps[3] == 0.1
-		assert trial_is[3] == 1
-		
-		# Make sure number of trial files created is correct
-		baseline_trial_dir = os.path.join(results_dir,
-			f"{baseline_model_name}_results/trial_data")
-		trial_files = os.listdir(baseline_trial_dir)
-		assert len(trial_files) == 4
-
-		# Make sure the trial files have the right format
-		trial_file_0 = os.path.join(baseline_trial_dir,trial_files[0])
-		df_trial0 = pd.read_csv(trial_file_0)
-		assert len(df_trial0) == 1
-
-	# Fairlearn baseline
-	fairlearn_constraint_name = 'demographic_parity'
-	fairlearn_epsilon_eval = 0.2 # the epsilon used to evaluate g, needs to be same as epsilon in our definition
-	fairlearn_eval_method = 'two-groups' # the epsilon used to evaluate g, needs to be same as epsilon in our definition
-	fairlearn_epsilons_constraint = [0.2] # the epsilons used in the fitting constraint
-	fairlearn_sensitive_feature_names=['M']
-	fairlearn_sensitive_col_indices = [dataset.sensitive_col_names.index(
-	    col) for col in fairlearn_sensitive_feature_names]
-	fairlearn_sensitive_features = dataset.sensitive_attrs[:,fairlearn_sensitive_col_indices]
-	# Make dict of test set features, labels and sensitive feature vectors
-	
-	test_features_fairlearn = test_features
-
-	fairlearn_eval_kwargs = {
-		'X':test_features_fairlearn,
-		'y':test_labels,
-		'sensitive_features':fairlearn_sensitive_features,
-		'eval_method':fairlearn_eval_method,
-		}
-
-	for fairlearn_epsilon_constraint in fairlearn_epsilons_constraint:
-		baseline_model_name = f'fairlearn_eps{fairlearn_epsilon_constraint:.2f}'
-		spg.run_fairlearn_experiment(
-			verbose=True,
-			fairlearn_sensitive_feature_names=fairlearn_sensitive_feature_names,
-			fairlearn_constraint_name=fairlearn_constraint_name,
-			fairlearn_epsilon_constraint=fairlearn_epsilon_constraint,
-			fairlearn_epsilon_eval=fairlearn_epsilon_eval,
-			fairlearn_eval_kwargs=fairlearn_eval_kwargs,
-			)
-		## Make sure results file was created
-		baseline_results_file = os.path.join(results_dir,
-			f"{baseline_model_name}_results/{baseline_model_name}_results.csv")
-		assert os.path.exists(baseline_results_file)
-
-		# Make sure length of df is correct
-		baseline_df = pd.read_csv(baseline_results_file)
-	
-		assert len(baseline_df) == 4
-		dps = baseline_df.data_frac
-		trial_is = baseline_df.trial_i
-		perfs = baseline_df.performance
-		faileds = baseline_df.failed
-	
-		assert dps[0] == 0.01
-		assert trial_is[0] == 0
-
-		assert dps[1] == 0.01
-		assert trial_is[1] == 1
-
-		assert dps[2] == 0.1
-		assert trial_is[2] == 0
-
-		assert dps[3] == 0.1
-		assert trial_is[3] == 1
-		
-		# Make sure number of trial files created is correct
-		baseline_trial_dir = os.path.join(results_dir,
-			f"{baseline_model_name}_results/trial_data")
-		trial_files = os.listdir(baseline_trial_dir)
-		assert len(trial_files) == 4
-
-		# Make sure the trial files have the right format
-		trial_file_0 = os.path.join(baseline_trial_dir,trial_files[0])
-		df_trial0 = pd.read_csv(trial_file_0)
-		assert len(df_trial0) == 1
-
-	# Seldonian experiment
-
-	spg.run_seldonian_experiment(verbose=True)
-
-	## Make sure results file was created
-	results_file = os.path.join(results_dir,"qsa_results/qsa_results.csv")
-	assert os.path.exists(results_file)
-
-	# Make sure length of df is correct
-	df = pd.read_csv(results_file)
-	assert len(df) == 4
-	dps = df.data_frac
-	trial_is = df.trial_i
-	perfs = df.performance
-	passed_safetys = df.passed_safety
-	faileds = df.failed
-	
-	assert dps[0] == 0.01
-	assert trial_is[0] == 0
-
-	assert dps[1] == 0.01
-	assert trial_is[1] == 1
-
-	assert dps[2] == 0.1
-	assert trial_is[2] == 0
-
-	assert dps[3] == 0.1
-	assert trial_is[3] == 1
-	
-	# Make sure number of trial files created is correct
-	trial_dir = os.path.join(results_dir,"qsa_results/trial_data")
-	trial_files = os.listdir(trial_dir)
-	assert len(trial_files) == 4
-
-	# Make sure the trial files have the right format
-	trial_file_0 = os.path.join(trial_dir,trial_files[0])
-	df_trial0 = pd.read_csv(trial_file_0)
-	assert len(df_trial0) == 1
-
-	# Now make plot
-	savename = os.path.join(results_dir,"test_gpa_classification_plot.png")
-	spg.make_plots(fontsize=12,legend_fontsize=8,
-		performance_label='Accuracy',
-		save_format="png",
-		savename=savename)
-	# Make sure it was saved
-	assert os.path.exists(savename)
-
-@pytest.mark.parametrize('experiment', ["./tests/static/results"], indirect=True)
 def test_too_few_datapoints(gpa_regression_spec,experiment):
 	""" Test that too small of a data_frac resulting in < 1
 	data points in a trial raises an error """
 	np.random.seed(42)
 	constraint_strs = ['Mean_Squared_Error <= 2.0']
 	deltas = [0.05]
 	spec = gpa_regression_spec(constraint_strs,deltas)
@@ -459,15 +264,16 @@
 	# Make sure length of df is correct
 	df = pd.read_csv(results_file)
 	assert len(df) == 4
 	dps = df.data_frac
 	trial_is = df.trial_i
 	perfs = df.performance
 	passed_safetys = df.passed_safety
-	faileds = df.failed
+	print("df:")
+	print(df)
 	
 	assert dps[0] == 0.01
 	assert trial_is[0] == 0
 
 	assert dps[1] == 0.01
 	assert trial_is[1] == 1
```


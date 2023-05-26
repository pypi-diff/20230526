# Comparing `tmp/truesight-0.0.2a3.tar.gz` & `tmp/truesight-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truesight-0.0.2a3.tar", last modified: Mon May 22 18:09:04 2023, max compression
+gzip compressed data, was "truesight-0.0.3a1.tar", last modified: Fri May 26 19:31:07 2023, max compression
```

## Comparing `truesight-0.0.2a3.tar` & `truesight-0.0.3a1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 18:08:42.000000 truesight-0.0.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-22 18:09:04.820492 truesight-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-22 18:08:42.000000 truesight-0.0.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 18:09:04.820492 truesight-0.0.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-22 18:08:42.000000 truesight-0.0.2a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/truesight/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-22 18:08:42.000000 truesight-0.0.2a3/truesight/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:04.820492 truesight-0.0.2a3/truesight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 18:09:04.000000 truesight-0.0.2a3/truesight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:31:07.511654 truesight-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 19:30:42.000000 truesight-0.0.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-26 19:31:07.511654 truesight-0.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-26 19:30:42.000000 truesight-0.0.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 19:31:07.511654 truesight-0.0.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-26 19:30:42.000000 truesight-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:31:07.511654 truesight-0.0.3a1/truesight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-26 19:30:42.000000 truesight-0.0.3a1/truesight/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:31:07.511654 truesight-0.0.3a1/truesight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-26 19:31:07.000000 truesight-0.0.3a1/truesight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 19:31:07.000000 truesight-0.0.3a1/truesight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:31:07.000000 truesight-0.0.3a1/truesight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 19:31:07.000000 truesight-0.0.3a1/truesight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 19:31:07.000000 truesight-0.0.3a1/truesight.egg-info/top_level.txt
```

### Comparing `truesight-0.0.2a3/LICENSE` & `truesight-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `truesight-0.0.2a3/PKG-INFO` & `truesight-0.0.3a1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truesight
-Version: 0.0.2a3
+Version: 0.0.3a1
 Summary: Truesight is a python package for time series prediction using deep learning and statistical models.
 Home-page: https://github.com/renanklehm/true-sight
 Download-URL: https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz
 Author: Renan Otvin Klehm
 Author-email: renanotivin@hotmail.com
 Keywords: time series,prediction
 Description-Content-Type: text/markdown
@@ -41,15 +41,15 @@
 Import the necessary modules
 
 ``` python
 import tensorflow as tf
 from truesight.preprocessing import Preprocessor
 from truesight.core import TrueSight
 from truesight.metrics import Evaluator, smape, mape, mse, rmse, mae
-from truesight.utils import get_input_shapes, generate_syntetic_data
+from truesight.utils import AutoTune, generate_syntetic_data
 ```
 
 Load the data
 
 ``` python
 num_time_steps = 60
 season_length = 12
@@ -61,15 +61,15 @@
 ``` python
 from statsforecast.models import SeasonalNaive, AutoETS
 from sklearn.linear_model import LinearRegression
 from truesight.models import AdditiveDecomposition
 from truesight.utils import ModelWrapper
 
 models = [
-    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length, alias="LinearRegression"), 
     ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length), 
     ModelWrapper(AutoETS, horizon=forecast_horizon, season_length=season_length),
     ModelWrapper(AdditiveDecomposition, horizon=forecast_horizon, season_length=season_length)
 ]
 
 preprocessor = Preprocessor(df)
 X_train, Y_train, ids_train, X_val, Y_val, ids_val, models = preprocessor.make_dataset(
@@ -78,88 +78,65 @@
     date_freq = "MS", 
     models = models, 
     fallback_model = ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length),
     verbose = True
     )
 ```
 
-Create the model
+Create the model and automatical automatically find the hyperparameters
 
 ``` python
-input_shapes = get_input_shapes(X_train)
-truesight = TrueSight(models, input_shapes, forecast_horizon = forecast_horizon)
-truesight.auto_tune(X_train, Y_train, X_val, Y_val, n_trials = 50, batch_size = 512, epochs = 5)
-```
-
-Use the `auto_tune` to automatically define the hyperparameters
-
-``` python
-truesight.auto_tune(X_train, Y_train, X_val, Y_val, n_trials = 10, batch_size = 512, epochs = 5)
+optimizer = tf.keras.optimizers.Adam
+hparams, optimizer = AutoTune(optimizer=optimizer).tune(X_train, Y_train, n_trials = 20, epochs = 10, batch_size = 32, stats_models = models)
+ts = TrueSight(models, forecast_horizon)
+ts.set_hparams(hparams)
+ts.compile(optimizer=optimizer, loss='mse')
 ```
 
 Or set then manually
 
 ``` python
-truesight.set_hparams(lstm_units=256, hidden_size=1024, num_heads=8, dropout_rate=0.1)
+optimizer = tf.keras.optimizers.Adam
+ts = TrueSight(models, forecast_horizon, filter_size = 128, context_size = 512, hidden_size = 1024, dropout_rate = 0.1)
+ts.compile(optimizer=optimizer, loss='mse')
 ```
 
 Train the model, as the model is built on the tensorflow framework, any tensorflow callback can be used
 
 ``` python
 callbacks = [
     tf.keras.callbacks.EarlyStopping(patience = 100, restore_best_weights = True, monitor = "val_loss"),
-    tf.keras.callbacks.ReduceLROnPlateau(monitor = "val_loss", factor = 0.5, patience = 25, verbose = 1),
+    tf.keras.callbacks.ReduceLROnPlateau(monitor = "val_loss", factor = 0.5, patience = 25, verbose = False),
 ]
-truesight.fit(
-    X_train, Y_train, 
-    X_val, Y_val, 
+ts.fit(
+    x = X_train, y = Y_train, 
+    validation_data = [X_val, Y_val], 
     batch_size = 128, 
     epochs = 1000, 
     verbose = False, 
     callbacks = callbacks,
- )
-truesight.plot_history()
+)
+ts.plot_training_history()
 ```
 ![Training Log](figures/training_history.png)
 
 
 Evaluate the results
 
 ``` python
-Y_hat = truesight.predict(
-    X_val, 
-    batch_size = 500, 
-    n_repeats = 100, 
-    n_quantiles = 15, 
-    return_quantiles = True, 
-    verbose = False,
- )
-evaluator = Evaluator(X_val, Y_val, Y_hat, ids_val)
-evaluator.evaluate_prediction([smape, mape, mse, rmse, mae], return_mean=False)
-```
-| id |         mse |      rmse |      mae |
-|---:|------------:|----------:|---------:|
-| 10 |  1164.51    |  34.1249  | 25.9397  |
-| 13 |     2.91094 |   1.70615 |  1.69313 |
-| 18 |     2.62309 |   1.6196  |  1.5549  |
-| 38 |     2.77819 |   1.66679 |  1.62896 |
-| 45 |   892.701   |  29.8781  | 10.0897  |
-| 46 |     2.96284 |   1.72129 |  1.71549 |
-| 50 |  3585.54    |  59.8794  | 49.0362  |
-| 51 | 12199.1     | 110.449   | 93.9491  |
-| 53 |     2.6345  |   1.62311 |  1.56625 |
-| 54 |     2.77184 |   1.66488 |  1.63493 |
-| 61 |   303.464   |  17.4202  | 14.6694  |
-| 67 |     2.70393 |   1.64436 |  1.60988 |
-| 69 |  2578.09    |  50.7749  | 38.986   |
-| 70 |     3.09074 |   1.75805 |  1.75805 |
-| 73 |     2.80945 |   1.67614 |  1.65109 |
-| 75 |     2.88333 |   1.69804 |  1.68085 |
-| 78 |     3.09091 |   1.7581  |  1.7581  |
-| 81 |     2.64539 |   1.62647 |  1.56712 |
-| 83 |   491.263   |  22.1644  | 18.4432  |
-| 86 |     2.84002 |   1.68523 |  1.64177 |
+yhat = ts.predict(X_val, n_repeats = 100, n_quantiles = 15, verbose = False)
+evaluator = Evaluator(X_val, Y_val, yhat, ids_val)
+evaluator.evaluate_prediction(evaluators = [smape, mape, mse, rmse, mae], return_mean = True)
+```
+| metric |   value   |
+|-------:|----------:|
+|smape   |   0.234369|
+|mape    |   0.293816|
+|mse     | 816.238082|
+|rmse    |  21.218396|
+|mae     |  15.885432|
+
 
 ``` python
 evaluator.plot_exemple()
 ```
 ![Output Exemple](figures/output.png)
```

### Comparing `truesight-0.0.2a3/README.md` & `truesight-0.0.3a1/truesight.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: truesight
+Version: 0.0.3a1
+Summary: Truesight is a python package for time series prediction using deep learning and statistical models.
+Home-page: https://github.com/renanklehm/true-sight
+Download-URL: https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz
+Author: Renan Otvin Klehm
+Author-email: renanotivin@hotmail.com
+Keywords: time series,prediction
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # TrueSight ✨
 
 The TrueSight model is a hybrid forecasting tool that uses statistical forecasting models together with a Deep Neural Network (DNN) to make predictions. The TrueSight `Preprocessor` class is responsible for getting all the statistical forecasters in one place. It can handle forecasters from packages like `statsforecast`, `scikit-learn`, `pmdarima`, and others. You just need to the `ModelWrapper` Class to standardize the method calls.
 
 All you need to do before using this package, is create a pandas dataframe with the following structure:
 
  - unique_id: A string that uniquely identifies each time series in the dataframe
@@ -29,15 +41,15 @@
 Import the necessary modules
 
 ``` python
 import tensorflow as tf
 from truesight.preprocessing import Preprocessor
 from truesight.core import TrueSight
 from truesight.metrics import Evaluator, smape, mape, mse, rmse, mae
-from truesight.utils import get_input_shapes, generate_syntetic_data
+from truesight.utils import AutoTune, generate_syntetic_data
 ```
 
 Load the data
 
 ``` python
 num_time_steps = 60
 season_length = 12
@@ -49,15 +61,15 @@
 ``` python
 from statsforecast.models import SeasonalNaive, AutoETS
 from sklearn.linear_model import LinearRegression
 from truesight.models import AdditiveDecomposition
 from truesight.utils import ModelWrapper
 
 models = [
-    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length), 
+    ModelWrapper(LinearRegression, horizon=forecast_horizon, season_length=season_length, alias="LinearRegression"), 
     ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length), 
     ModelWrapper(AutoETS, horizon=forecast_horizon, season_length=season_length),
     ModelWrapper(AdditiveDecomposition, horizon=forecast_horizon, season_length=season_length)
 ]
 
 preprocessor = Preprocessor(df)
 X_train, Y_train, ids_train, X_val, Y_val, ids_val, models = preprocessor.make_dataset(
@@ -66,88 +78,65 @@
     date_freq = "MS", 
     models = models, 
     fallback_model = ModelWrapper(SeasonalNaive, horizon=forecast_horizon, season_length=season_length),
     verbose = True
     )
 ```
 
-Create the model
-
-``` python
-input_shapes = get_input_shapes(X_train)
-truesight = TrueSight(models, input_shapes, forecast_horizon = forecast_horizon)
-truesight.auto_tune(X_train, Y_train, X_val, Y_val, n_trials = 50, batch_size = 512, epochs = 5)
-```
-
-Use the `auto_tune` to automatically define the hyperparameters
+Create the model and automatical automatically find the hyperparameters
 
 ``` python
-truesight.auto_tune(X_train, Y_train, X_val, Y_val, n_trials = 10, batch_size = 512, epochs = 5)
+optimizer = tf.keras.optimizers.Adam
+hparams, optimizer = AutoTune(optimizer=optimizer).tune(X_train, Y_train, n_trials = 20, epochs = 10, batch_size = 32, stats_models = models)
+ts = TrueSight(models, forecast_horizon)
+ts.set_hparams(hparams)
+ts.compile(optimizer=optimizer, loss='mse')
 ```
 
 Or set then manually
 
 ``` python
-truesight.set_hparams(lstm_units=256, hidden_size=1024, num_heads=8, dropout_rate=0.1)
+optimizer = tf.keras.optimizers.Adam
+ts = TrueSight(models, forecast_horizon, filter_size = 128, context_size = 512, hidden_size = 1024, dropout_rate = 0.1)
+ts.compile(optimizer=optimizer, loss='mse')
 ```
 
 Train the model, as the model is built on the tensorflow framework, any tensorflow callback can be used
 
 ``` python
 callbacks = [
     tf.keras.callbacks.EarlyStopping(patience = 100, restore_best_weights = True, monitor = "val_loss"),
-    tf.keras.callbacks.ReduceLROnPlateau(monitor = "val_loss", factor = 0.5, patience = 25, verbose = 1),
+    tf.keras.callbacks.ReduceLROnPlateau(monitor = "val_loss", factor = 0.5, patience = 25, verbose = False),
 ]
-truesight.fit(
-    X_train, Y_train, 
-    X_val, Y_val, 
+ts.fit(
+    x = X_train, y = Y_train, 
+    validation_data = [X_val, Y_val], 
     batch_size = 128, 
     epochs = 1000, 
     verbose = False, 
     callbacks = callbacks,
- )
-truesight.plot_history()
+)
+ts.plot_training_history()
 ```
 ![Training Log](figures/training_history.png)
 
 
 Evaluate the results
 
 ``` python
-Y_hat = truesight.predict(
-    X_val, 
-    batch_size = 500, 
-    n_repeats = 100, 
-    n_quantiles = 15, 
-    return_quantiles = True, 
-    verbose = False,
- )
-evaluator = Evaluator(X_val, Y_val, Y_hat, ids_val)
-evaluator.evaluate_prediction([smape, mape, mse, rmse, mae], return_mean=False)
-```
-| id |         mse |      rmse |      mae |
-|---:|------------:|----------:|---------:|
-| 10 |  1164.51    |  34.1249  | 25.9397  |
-| 13 |     2.91094 |   1.70615 |  1.69313 |
-| 18 |     2.62309 |   1.6196  |  1.5549  |
-| 38 |     2.77819 |   1.66679 |  1.62896 |
-| 45 |   892.701   |  29.8781  | 10.0897  |
-| 46 |     2.96284 |   1.72129 |  1.71549 |
-| 50 |  3585.54    |  59.8794  | 49.0362  |
-| 51 | 12199.1     | 110.449   | 93.9491  |
-| 53 |     2.6345  |   1.62311 |  1.56625 |
-| 54 |     2.77184 |   1.66488 |  1.63493 |
-| 61 |   303.464   |  17.4202  | 14.6694  |
-| 67 |     2.70393 |   1.64436 |  1.60988 |
-| 69 |  2578.09    |  50.7749  | 38.986   |
-| 70 |     3.09074 |   1.75805 |  1.75805 |
-| 73 |     2.80945 |   1.67614 |  1.65109 |
-| 75 |     2.88333 |   1.69804 |  1.68085 |
-| 78 |     3.09091 |   1.7581  |  1.7581  |
-| 81 |     2.64539 |   1.62647 |  1.56712 |
-| 83 |   491.263   |  22.1644  | 18.4432  |
-| 86 |     2.84002 |   1.68523 |  1.64177 |
+yhat = ts.predict(X_val, n_repeats = 100, n_quantiles = 15, verbose = False)
+evaluator = Evaluator(X_val, Y_val, yhat, ids_val)
+evaluator.evaluate_prediction(evaluators = [smape, mape, mse, rmse, mae], return_mean = True)
+```
+| metric |   value   |
+|-------:|----------:|
+|smape   |   0.234369|
+|mape    |   0.293816|
+|mse     | 816.238082|
+|rmse    |  21.218396|
+|mae     |  15.885432|
+
 
 ``` python
 evaluator.plot_exemple()
 ```
 ![Output Exemple](figures/output.png)
```

### Comparing `truesight-0.0.2a3/setup.py` & `truesight-0.0.3a1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name = 'truesight',
     packages = ['truesight'],
-    version = 'v0.0.2a3',
+    version = 'v0.0.3a1',
     description = 'Truesight is a python package for time series prediction using deep learning and statistical models.',
     author = 'Renan Otvin Klehm',
     author_email = 'renanotivin@hotmail.com',
     url = 'https://github.com/renanklehm/true-sight',
     download_url = 'https://github.com/renanklehm/true-sight/archive/refs/tags/v0.0.1-alpha.tar.gz',
     keywords = ['time series', 'prediction'],
     classifiers = [],
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'tensorflow>=2.11.0',
         'optuna>=2.10.1',
         'numpy>=1.23.5',
-        'pandas>=1.5.3',
-        'matplotlib>=3.6.3',
-        'scipy>=1.10.0',
-        'tqdm>=4.64.1',
+        'pandas',
+        'matplotlib',
+        'scipy',
+        'tqdm',
     ]
 )
```

### Comparing `truesight-0.0.2a3/truesight/core.py` & `truesight-0.0.3a1/truesight/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 import os
 import json
 import optuna
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
 from datetime import datetime
+from truesight.layers import FeedForward, WeightedSumLayer
 
-class TrueSight:
+
+class OLD(tf.keras.Model):
 
     def __init__(
             self,
-            models: list,
             input_shape: list, 
             forecast_horizon: int,
+            hparams_folder: str = './hparams',
+            model_folder: str = 'best_model'            
         ) -> None:
-        self.model_folder = 'best_model'
-        self.hparams_folder = './hparams'
+        self.model_folder = hparams_folder
+        self.hparams_folder = model_folder
         os.makedirs(self.hparams_folder, exist_ok=True)
+        
         self.input_shape = input_shape
         self.forecast_horizon = forecast_horizon
-        self.models = models
-        self.set_hparams()
-        self.model = self.get_model(self.hparams)
 
     def get_model(
             self, 
             hparams: dict = {}
         ) -> tf.keras.Model:
         x_inputs = []
         x_outputs = []
@@ -126,41 +127,14 @@
             'hidden_size': hidden_size,
             'num_heads': num_heads,
             'key_dim': key_dim,
             'learning_rate': learning_rate,
             'dropout_rate': dropout_rate,
         }
 
-    def objective(self, trial):
-        num_filters = trial.suggest_int("num_filters", self.min_num_filters, self.max_num_filters)
-        kernel_size = trial.suggest_int("kernel_size", self.min_kernel_size, self.max_kernel_size)
-        lstm_units = trial.suggest_int("lstm_units", self.min_lstm_units, self.max_lstm_units)
-        hidden_size = trial.suggest_int("hidden_size", self.min_hidden_size, self.max_hidden_size)
-        num_heads = trial.suggest_int("num_heads", self.min_num_heads, self.max_num_heads)
-        key_dim = trial.suggest_int("key_dim", self.min_key_dim, self.max_key_dim)
-        dropout_rate = trial.suggest_float("dropout_rate", self.min_dropout_rate, self.max_dropout_rate )
-        learning_rate = trial.suggest_float("learning_rate", self.min_learning_rate, self.max_learning_rate)
-        hparams = {
-            'num_filters': num_filters,
-            'kernel_size': kernel_size,
-            'lstm_units': lstm_units,
-            'hidden_size': hidden_size,
-            'num_heads': num_heads,
-            'key_dim': key_dim,
-            'learning_rate': learning_rate,
-            'dropout_rate': dropout_rate,
-        }
-
-        model = self.get_model(hparams)
-        model.fit(self.X_train, self.Y_train, epochs = self.epochs, batch_size = self.batch_size, verbose = 0)
-        score = model.evaluate(self.X_val, self.Y_val, batch_size = self.batch_size, verbose = 0)
-        score = np.array(score).mean()
-        with open(f'{self.hparams_folder}/{datetime.now().strftime("%Y%m%d%H%M%S")}-{score}.json', 'w') as file: json.dump(hparams, file)
-        return score
-
     def auto_tune(
             self,
             X_train: list,
             Y_train: np.ndarray,
             X_val: list,
             Y_val: np.ndarray,
             n_trials: int,
@@ -220,8 +194,107 @@
         return self.hparams
 
     def plot_history(self):
         if not hasattr(self, 'history'): raise Exception('No history found. Please train the model first.')
         plt.plot(self.history.history['loss'], label='train')
         plt.plot(self.history.history['val_loss'], label='validation')
         plt.legend()
-        plt.show()
+        plt.show()
+
+class TrueSight(tf.keras.Model):
+
+    def __init__(
+            self,
+            models: list,
+            forecast_horizon: int,
+            filter_size: int = 64,
+            context_size: int = 256,
+            hidden_size: int = 512,
+            dropout_rate: int = 0.1,
+        ) -> None:
+        
+        super(TrueSight, self).__init__()
+        self.models = models
+        self.n_models = len(models)
+        self.forecast_horizon = forecast_horizon
+        self.filter_size = filter_size
+        self.context_size = context_size
+        self.hidden_size = hidden_size
+        self.dropout_rate = dropout_rate
+        
+        self.branches = {}
+        for i in range(self.n_models):
+            self.branches[models[i]] = tf.keras.layers.Dense(context_size, activation='selu', name=f'branch_{models[i]}')
+        self.weighted_sum = WeightedSumLayer(n_models=self.n_models, name='weighted_sum')
+        self.ff = FeedForward(filter_size=filter_size, context_size=context_size, hidden_size=hidden_size, dropout_rate=dropout_rate, name='feed_forward')
+        self.output_layer = tf.keras.layers.Dense(forecast_horizon, activation='relu', name='output')
+    
+    def set_hparams(
+        self,
+        hparams: dict,
+    ) -> None:
+        
+        self.__init__(self.models, self.forecast_horizon, hparams['filter_size'], hparams['context_size'], hparams['hidden_size'], hparams['dropout_rate'])
+    
+    def build(
+        self, 
+        input_shape: list,
+    ) -> None:
+        
+        for idx, branch in enumerate(self.branches.values()):
+            branch.build(input_shape[idx])
+        self.ff.build((None, 1))
+        self.output_layer.build((None, self.hidden_size))
+        return 
+    
+    def call(
+        self, 
+        inputs: list,
+    ) -> tf.Tensor:
+        
+        outputs = []
+        for idx, model in enumerate(self.models):
+            outputs.append(self.branches[model](inputs[idx]))
+        outputs = self.weighted_sum(outputs)
+        outputs = self.ff(outputs, training=True)
+        outputs = self.output_layer(outputs)
+        return outputs
+    
+    def fit(
+        self,
+        **kwargs
+    ) -> None:
+        
+        self.history = super(TrueSight, self).fit(**kwargs)
+    
+    def plot_training_history(
+        self,
+    ) -> None:
+        
+        if not hasattr(self, 'history'): raise Exception('No history found. Please train the model first.')
+        plt.plot(self.history.history['loss'], label='train')
+        plt.plot(self.history.history['val_loss'], label='validation')
+        plt.legend()
+        plt.show(
+    )
+
+    def predict(
+        self,
+        X: list,
+        n_repeats: int = 1,
+        batch_size: int = 128,
+        n_quantiles: int = 10,
+        return_quantiles: bool = False,
+        verbose: bool = True
+    ) -> np.ndarray:
+
+        yhat = []
+        for i in range(n_repeats):
+            yhat.append(super(TrueSight, self).predict(X, batch_size=batch_size, verbose=verbose))
+        yhat = np.array(yhat)
+
+        if return_quantiles or n_quantiles > 1: 
+            yhat = np.quantile(yhat, np.linspace(0, 1, n_quantiles), axis=0)
+        else: 
+            yhat = np.mean(yhat, axis=0)
+        
+        return yhat
```

### Comparing `truesight-0.0.2a3/truesight/metrics.py` & `truesight-0.0.3a1/truesight/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+import warnings
 import matplotlib.pyplot as plt
 
 np.seterr(divide='ignore')
 
 def bias(
         y_true: np.ndarray, 
         y_pred: np.ndarray,  
@@ -30,110 +31,125 @@
 
 def smape(
         y_true: np.ndarray, 
         y_pred: np.ndarray,  
         axis: int = -1, 
         return_mean: bool = False
     ) -> np.ndarray:
-    smape = abs(y_true - y_pred)
-    smape = smape / (abs(y_true) + abs(y_pred))
-    smape = np.where((y_true==0) & (y_pred==0), np.zeros(smape.shape), smape)
-    smape = np.where(np.isnan(smape), np.ones(smape.shape), smape)
-    smape = np.where(np.isinf(smape), np.ones(smape.shape), smape)
-    if (return_mean):
-        return np.mean(smape)
-    else:
-        return np.mean(smape, axis = axis)
+    
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
+        smape = abs(y_true - y_pred)
+        smape = smape / (abs(y_true) + abs(y_pred))
+        smape = np.where((y_true==0) & (y_pred==0), np.zeros(smape.shape), smape)
+        smape = np.where(np.isnan(smape), np.ones(smape.shape), smape)
+        smape = np.where(np.isinf(smape), np.ones(smape.shape), smape)
+        if (return_mean):
+            return np.mean(smape)
+        else:
+            return np.mean(smape, axis = axis)
 
 def mape(
         y_true: np.ndarray, 
         y_pred: np.ndarray,  
         axis: int = -1, 
         return_mean: bool = False
     ) -> np.ndarray:
-    mape = abs(y_true - y_pred)
-    mape = mape / y_true
-    mape = np.where((y_true==0) & (y_pred==0), np.zeros(mape.shape), mape)
-    mape = np.where(np.isnan(mape), np.ones(mape.shape), mape)
-    mape = np.where(np.isinf(mape), np.ones(mape.shape), mape)
-    if (return_mean):
-        return np.mean(mape)
-    else:
-        return np.mean(mape, axis = axis)
+    
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
+        mape = abs(y_true - y_pred)
+        mape = mape / y_true
+        mape = np.where((y_true==0) & (y_pred==0), np.zeros(mape.shape), mape)
+        mape = np.where(np.isnan(mape), np.ones(mape.shape), mape)
+        mape = np.where(np.isinf(mape), np.ones(mape.shape), mape)
+        if (return_mean):
+            return np.mean(mape)
+        else:
+            return np.mean(mape, axis = axis)
 
 def mse(
         y_true: np.ndarray, 
         y_pred: np.ndarray,  
         axis: int = -1, 
         return_mean: bool = False
     ) -> np.ndarray:
+    
     mse = (y_true - y_pred) ** 2
     if (return_mean):
         return np.mean(mse)
     else:
         return np.mean(mse, axis = axis)
 
 def rmse(
         y_true: np.ndarray, 
         y_pred: np.ndarray,  
         axis: int = -1, 
         return_mean: bool = False
     ) -> np.ndarray:
+    
     rmse = (y_true - y_pred) ** 2
     if (return_mean):
         return np.sqrt(np.mean(rmse))
     else:
         return np.sqrt(np.mean(rmse, axis = axis))
 
 class Evaluator:
+    
     def __init__(
-            self,
-            x: np.ndarray,
-            y_true: np.ndarray,
-            y_pred: np.ndarray,
-            ids: np.ndarray):
+        self,
+        x: np.ndarray,
+        y_true: np.ndarray,
+        y_pred: np.ndarray,
+        ids: np.ndarray
+    ) -> None:
+        
         self.x = x
         self.y_true = y_true
         self.y_pred = y_pred
         self.ids = ids
 
     def evaluate_prediction(
-            self,
-            evaluators: list = [],
-            return_mean: bool = False
-        ):
+        self,
+        evaluators: list = [],
+        return_mean: bool = False
+    ) -> pd.DataFrame:
+        
         df_list = []
         for i, id in enumerate(self.ids):
             df = {}
             for evaluator in evaluators:
                 df[evaluator.__name__] = evaluator(self.y_true[i], self.y_pred.mean(axis=0)[i], return_mean = True)
             df_list.append(pd.DataFrame(df, index = [id]))
         if (return_mean):
             return pd.concat(df_list).mean()
         else:
             return pd.concat(df_list)
 
-    def plot_exemple(self):
+    def plot_exemple(
+        self
+    ) -> None:
+        
         idx = np.random.randint(0, len(self.y_true))
 
-        ytrue = np.squeeze(self.y_true[idx])
-        yhat = np.squeeze(self.y_pred.mean(axis=0)[idx])
+        ytrue = self.y_true[idx]
+        yhat = self.y_pred.mean(axis=0)[idx]
 
         range_input = np.arange(0, self.x[-1].shape[1])
         range_output = np.arange(self.x[-1].shape[1], len(ytrue) + self.x[-1].shape[1])
 
         _, ax = plt.subplots(figsize=(10, 6), dpi=100)
         ax.plot(range_output, ytrue, ".-", color = "darkslategray", label = "True data")
-        ax.plot(range_input, np.squeeze(self.x[-1][idx]), label = "Input", color = "darkslategray", alpha = 0.5)
+        ax.plot(range_input, self.x[-1][idx], label = "Input", color = "darkslategray", alpha = 0.5)
 
         for i in range(yhat.shape[0] // 2):
             if (i == 0):
-                ax.fill_between(range_output, np.squeeze(self.y_pred[-i-1,idx]), np.squeeze(self.y_pred[i,idx]), alpha = 0.3 / (self.y_pred.shape[0] / 2), color = "brown")
+                ax.fill_between(range_output, self.y_pred[-i-1,idx], self.y_pred[i,idx], alpha = 0.5 / (self.y_pred.shape[0] / 2), color = "brown")
             else:
-                ax.fill_between(range_output, np.squeeze(self.y_pred[-i-1,idx]), np.squeeze(self.y_pred[i,idx]), alpha = 0.3 / (self.y_pred.shape[0] / 2), color = "brown")
+                ax.fill_between(range_output, self.y_pred[-i-1,idx], self.y_pred[i,idx], alpha = 0.5 / (self.y_pred.shape[0] / 2), color = "brown")
         ax.plot(range_output, yhat, "v-", label = "TrueSight Prediction", color = "brown")
         ax.axvline(x = range_output[0], linestyle = "--", color = 'crimson', label = 'Training Data')
         ax.set_ylim(0)
 
         plt.legend()
         plt.tight_layout()
         plt.show()
```

### Comparing `truesight-0.0.2a3/truesight/models.py` & `truesight-0.0.3a1/truesight/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 from truesight.metrics import mse
 from statsmodels.tsa.seasonal import seasonal_decompose
 
 class AdditiveDecomposition(StatisticalForecaster):
 
     def __init__(
         self, 
-        season_length: int
+        season_length: int,
+        alias: str = 'AdditiveDecomposition'
     ) -> None:
         
         self.season_length = season_length
         self.trend_coeff = None
         self.seasonality = None
         self.noise = None
+        self.alias = alias
 
     def fit(
         self, 
         y: np.ndarray,
         trend_degrees: list = [1, 2]
     ) -> None:
 
@@ -47,8 +49,11 @@
 
         trend_forecast = np.polyval(self.trend_coeff, x)
         seasonality_forecast = np.tile(self.seasonality[:forecast_horizon], forecast_horizon // self.season_length + 1)[:forecast_horizon]
         noise_forecast = np.random.choice(self.noise, size=forecast_horizon)
 
         forecast = trend_forecast + seasonality_forecast + noise_forecast
 
-        return forecast
+        return forecast
+
+    def __repr__(self) -> str:
+        return f'{self.alias}'
```

### Comparing `truesight-0.0.2a3/truesight/preprocessing.py` & `truesight-0.0.3a1/truesight/preprocessing.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,18 +48,18 @@
             local_df: pd.DataFrame
         ) -> tuple:
         pivot = pd.pivot_table(local_df, index = "unique_id", columns = "ds")
         models = np.unique(pivot.columns.get_level_values(0))
         x = []
         for model in models:
             if (model == "y"):
-                x.append(np.expand_dims(pivot[model].iloc[:,:-self.forecast_horizon].to_numpy(), -1))
+                x.append(pivot[model].iloc[:,:-self.forecast_horizon].to_numpy())
             else:
-                x.append(np.expand_dims(pivot[model].to_numpy(), -1))
-        y = np.expand_dims(pivot["y"].iloc[:,-self.forecast_horizon:].to_numpy(), -1)
+                x.append(pivot[model].to_numpy())
+        y = pivot["y"].iloc[:,-self.forecast_horizon:].to_numpy()
         ids = pivot.index
         return x, y, ids, models
 
     def get_statistical_forecast(
             self, 
             local_df: pd.DataFrame, 
             models: list = [],
```


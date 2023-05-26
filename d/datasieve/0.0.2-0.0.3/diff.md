# Comparing `tmp/datasieve-0.0.2.tar.gz` & `tmp/datasieve-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.2.tar", max compression
+gzip compressed data, was "datasieve-0.0.3.tar", max compression
```

## Comparing `datasieve-0.0.2.tar` & `datasieve-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-25 13:22:18.715702 datasieve-0.0.2/LICENSE
--rw-r--r--   0        0        0     9987 2023-05-25 14:11:51.276521 datasieve-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-25 12:33:12.836729 datasieve-0.0.2/datasieve/__init__.py
--rw-r--r--   0        0        0     6059 2023-05-25 12:33:45.700647 datasieve-0.0.2/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-25 12:50:22.661676 datasieve-0.0.2/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5458 2023-05-25 12:45:29.750610 datasieve-0.0.2/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     2874 2023-05-25 12:38:23.699896 datasieve-0.0.2/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-25 12:48:33.926026 datasieve-0.0.2/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1553 2023-05-25 12:39:53.967634 datasieve-0.0.2/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1502 2023-05-25 12:36:20.980240 datasieve-0.0.2/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1305 2023-05-25 12:50:35.305635 datasieve-0.0.2/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     2999 2023-05-25 12:37:08.608108 datasieve-0.0.2/datasieve/utils.py
--rw-r--r--   0        0        0      522 2023-05-25 14:20:54.206414 datasieve-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    10959 1970-01-01 00:00:00.000000 datasieve-0.0.2/setup.py
--rw-r--r--   0        0        0    10675 1970-01-01 00:00:00.000000 datasieve-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-26 13:34:19.758625 datasieve-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10058 2023-05-26 13:34:19.758625 datasieve-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/__init__.py
+-rw-r--r--   0        0        0     6164 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5593 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3007 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1567 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1502 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1432 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/utils.py
+-rw-r--r--   0        0        0      542 2023-05-26 13:34:19.758625 datasieve-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10698 1970-01-01 00:00:00.000000 datasieve-0.0.3/PKG-INFO
```

### Comparing `datasieve-0.0.2/LICENSE` & `datasieve-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.2/README.md` & `datasieve-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
 
 - removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
+- customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
 These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
 An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
 
 ```python
 class SVMOutlierExtractor(SGDOneClassSVM):
```

### Comparing `datasieve-0.0.2/datasieve/pipeline.py` & `datasieve-0.0.3/datasieve/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,18 @@
             self.feature_list = X.columns
             if y is not None:
                 self.label_list = y.columns
         elif fit:
             self.pandas_types = False
             self.feature_list = list(np.arange(0, X.shape[1]))
             if y is not None:
-                self.label_list = list(np.arange(0, y.shape[1]))
+                if len(y.shape) > 1:
+                    self.label_list = list(np.arange(0, y.shape[1]))
+                else:
+                    self.label_list = [0]
         elif isinstance(X, pd.DataFrame) and not fit:
             if list(X.columns) != list(self.feature_list):
                 raise Exception(f"Pipeline expected {self.feature_list} but got {X.columns}.")
         elif not isinstance(X, pd.DataFrame) and not fit and self.pandas_types:
             X = pd.DataFrame(X, columns=self.feature_list)
 
         if self.pandas_types:
```

### Comparing `datasieve-0.0.2/datasieve/transforms/__init__.py` & `datasieve-0.0.3/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.2/datasieve/transforms/dbscan.py` & `datasieve-0.0.3/datasieve/transforms/dbscan.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 
     fit() automatically finds the optimal epsilon and min_samples for a set of train_features
     transform() appends datapoints to the train_features, using the same epsilon and
     min_samples as computed in fit, to then determing if any of the appended data points
     are outliers.
     """
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, backend="loky", n_jobs=-1, **kwargs) -> None:
         super().__init__(**kwargs)
         self.train_features: npt.ArrayLike = np.array([])
+        self.backend = backend
+        self.n_jobs = n_jobs
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight)
 
         # in a fit_transform() situation, the user only wants
         # to get the outliers assocciated with the train_features.
         # In contrast, a user in the future wants to use the
@@ -51,15 +53,15 @@
         """
         Given a set of training features, find the best
         epsilond and min_samples
         """
         self.eps, self.min_samples = self.compute_epsilon_and_minpts(X)
         logger.info(f"Found eps {self.eps} and min_samples {self.min_samples} in fit")
 
-        with parallel_backend("dask", n_jobs=4):
+        with parallel_backend(self.backend, n_jobs=self.n_jobs):
             super().fit(X)
 
         self.train_features = X
 
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
@@ -67,15 +69,15 @@
         Given a data point (or data points), append them to the
         train_features and determine if they are inliers.
         """
 
         num_X = X.shape[0]
         fullX = np.concatenate([self.train_features, X], axis=0)
 
-        with parallel_backend("dask", n_jobs=4):
+        with parallel_backend(self.backend, n_jobs=self.n_jobs):
             logger.info(f"Using eps {self.eps} and min_samples {self.min_samples} to transform")
             clustering = super().fit(fullX)
 
         inliers = np.where(clustering.labels_[-num_X:] == -1, 0, 1)
 
         X, y, sample_weight = remove_outliers(X, y, sample_weight, inliers=inliers)
 
@@ -110,15 +112,15 @@
             y = origin[1] + np.sin(angle) * (point[0] - origin[0]) + \
                 np.cos(angle) * (point[1] - origin[1])
             return (x, y)
 
         MinPts = int(X.shape[0] * 0.25)
 
         # measure pairwise distances to nearest neighbours
-        with parallel_backend("dask", n_jobs=4):
+        with parallel_backend(self.backend, n_jobs=self.n_jobs):
             neighbors = NearestNeighbors(n_neighbors=MinPts)
             neighbors_fit = neighbors.fit(X)
             distances, _ = neighbors_fit.kneighbors(X)
 
         distances = np.sort(distances, axis=0).mean(axis=1)
         normalised_distances = normalise_distances(distances)
         x_range = np.linspace(0, 1, len(distances))
```

### Comparing `datasieve-0.0.2/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.3/datasieve/transforms/dissimilarity_index.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,32 +12,35 @@
     """
     Object designed for computing the dissimilarity index for a set of training data and
     prediction points. fit() computes the avg_mean distance for the training data and
     stores the data for future "transforms" transform() uses the `di_threshold` to
     identify and remove outliers
     """
 
-    def __init__(self, di_threshold: float = 1, **kwargs):
+    def __init__(self, di_threshold: float = 1, n_jobs=-1, backend="loky", **kwargs):
         self.avg_mean_dist: float = 0
         self.trained_data: npt.ArrayLike = np.array([])
         self.di_threshold = di_threshold
         self.di_values: npt.ArrayLike = np.array([])
+        self.n_jobs = n_jobs
+        self.backend = backend
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight)
-        X, y, sample_weight, feature_list = self.transform(X, y, sample_weight, feature_list)
+        X, y, sample_weight, feature_list = self.transform(
+            X, y, sample_weight, feature_list)
         return X, y, sample_weight, feature_list
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Compute the distances, save the average mean distance
         and save the trained_data array for future use
         """
 
-        with parallel_backend("loky", n_jobs=4):
+        with parallel_backend(self.backend, n_jobs=self.n_jobs):
             pairwise = pairwise_distances(X)
 
         # remove the diagonal distances which are itself distances ~0
         np.fill_diagonal(pairwise, np.NaN)
         pairwise = pairwise.reshape(-1, 1)
         self.avg_mean_dist = pairwise[~np.isnan(pairwise)].mean()
         self.trained_data = X
@@ -48,15 +51,15 @@
         """
         Compares the distance from each prediction point to each training data
         point. It uses this information to estimate a Dissimilarity Index (DI)
         and avoid making predictions on any points that are too far away
         from the training data set.
         """
 
-        with parallel_backend("dask", n_jobs=4):
+        with parallel_backend(self.backend, n_jobs=self.n_jobs):
             distance = pairwise_distances(self.trained_data, X)
 
         self.di_values = distance.min(axis=0) / self.avg_mean_dist
         y_pred = np.where(self.di_values < self.di_threshold, 1, 0)
 
         X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
 
@@ -69,8 +72,8 @@
 
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Unused
         """
-        return X, y, sample_weight, feature_list
+        return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.0.2/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.3/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.2/datasieve/transforms/pca.py` & `datasieve-0.0.3/datasieve/transforms/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         return X, y, sample_weight, self.feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         X = super().transform(X)
         return X, y, sample_weight, self.feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        return super().inverse_transform(X), y, sample_weight
+        return super().inverse_transform(X), y, sample_weight, feature_list
```

### Comparing `datasieve-0.0.2/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.3/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight=sample_weight)
-        return self.transform(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         super().fit(X, y=y, sample_weight=sample_weight)
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         y_pred = self.predict(X)
```

### Comparing `datasieve-0.0.2/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.3/datasieve/transforms/variance_threshold.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,21 @@
     def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self.fit(X, y, sample_weight, feature_list)
         return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         super().fit(X)
         self.mask = self.get_support()
-        self.feature_list = np.array(feature_list)[self.mask]
-        logger.info(f"Variance will remove features {len(feature_list) - len(self.feature_list)} "
-                    f"on transform. {np.array(feature_list)[~self.mask]}")
+        if feature_list is not None:
+            self.feature_list = np.array(feature_list)[self.mask]
+            logger.info("Variance will remove features "
+                        f"{len(feature_list) - len(self.feature_list)} "
+                        f"on transform. {np.array(feature_list)[~self.mask]}")
+        else:
+            self.feature_list = None
 
         return X, y, sample_weight, self.feature_list
 
     def transform(self, X, y=None, sample_weight=None, feature_list=None):
 
         # use mask to filter X array
         X = X[:, self.mask]
```

### Comparing `datasieve-0.0.2/datasieve/utils.py` & `datasieve-0.0.3/datasieve/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         y = y[(inliers == 1)]
     if sample_weight is not None:
         sample_weight = sample_weight[(inliers == 1)]
 
     return X, y, sample_weight
 
 
-def find_training_horizon(df: pd.DataFrame, target_horizon, test_pct=0.05, threshold=0.25e-3):
+def find_training_horizon(df: pd.DataFrame, target_horizon, test_pct=0.05,
+                          threshold=0.25e-3, backend="loky", n_jobs=-1):
     """
     Given a set of raw data, determine the necessariy training horizon
     associated to the target horizon
     """
     step_size = 1
     change_window = 100
     std_ratio = np.array([])
@@ -42,15 +43,15 @@
         test_size = test_pct
     else:
         test_size = int(df.shape[0] * test_pct)
     horizon_features = df.iloc[-target_horizon:]
 
     for t in np.arange(0, max_window, step_size):
         current_window = df.iloc[-target_horizon-t:]
-        with parallel_backend("loky", n_jobs=8):
+        with parallel_backend(backend, n_jobs=n_jobs):
             current_window_distances = pairwise_distances(
                 current_window, metric="euclidean", n_jobs=8)
             # remove the diagonal distances which are itself distances ~0
             # np.fill_diagonal(current_window_distances, np.NaN)
             current_window_distances = current_window_distances.reshape(-1, 1)
             std_train_dist = current_window_distances[~np.isnan(current_window_distances)].std()
             distances_horizon_current_window = pairwise_distances(
```

### Comparing `datasieve-0.0.2/pyproject.toml` & `datasieve-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.2"
+version = "0.0.3"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8.1,<4.0"
 scikit-learn = "^1.2.0"
 pandas = "^1.3.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
 autopep8 = "1.6.0"
+flake8 = "^6.0.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datasieve-0.0.2/setup.py` & `datasieve-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,221 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: datasieve
+Version: 0.0.3
+Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
+License: MIT
+Author: Robert Caulk
+Requires-Python: >=3.8.1,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['datasieve', 'datasieve.transforms']
+# DataSieve
 
-package_data = \
-{'': ['*']}
+DataSieve is very similar to the SKlearn Pipeline in that it:
 
-install_requires = \
-['pandas>=1.3.3,<2.0.0', 'scikit-learn>=1.2.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'datasieve',
-    'version': '0.0.2',
-    'description': 'This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)',
-    'long_description': '# DataSieve\n\nDataSieve is very similar to the SKlearn Pipeline in that it:\n\n- fits an arbitrary series of transformations to an array X\n- transforms subsequent arrays of the same dimension according to the fit from the original X\n- inverse transforms arrays by inverting the series of transformations\n\nThis means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.\n\nThe main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:\n\n- removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria\n- remove feature columns based on arbitrary criteria (e.g. low variance features)\n- change feature column names at certain transformations (e.g. PCA)\n- passing dynamic parameters to individual transforms of the pipeline\n- passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns\n\nThese improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. \n\nAn example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:\n\n```python\nclass SVMOutlierExtractor(SGDOneClassSVM):\n    """\n    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method\n    for removing detected outliers from X (as well as the associated y and\n    sample_weight if they are also furnished.\n    """\n\n    def __init__(self, **kwargs):\n        super().__init__(**kwargs)\n\n    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        self.fit(X, y, sample_weight=sample_weight)\n        return self.transform(X, y, sample_weight=sample_weight)\n\n    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        super().fit(X, y=y, sample_weight=sample_weight)\n        return X, y, sample_weight, feature_list\n\n    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        y_pred = self.predict(X)\n\n        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)\n\n        num_tossed = len(y_pred) - len(X)\n        if num_tossed > 0:\n            logger.info(\n                f"SVM detected {num_tossed} data points"\n                "as outliers."\n            )\n\n        return X, y, sample_weight, feature_list\n\n    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        """\n        Unused, pass through X, y, sample_weight, and feature_list\n        """\n        return X, y, sample_weight, feature_list\n```\n\n\nAs shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.\n\n\n# Usage\nThe user builds the pipeline similarly to SKLearn:\n\n```python\n    from datasieve.pipeline import Pipeline\n    from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor\n\n    feature_pipeline = Pipeline([\n        ("detect_constants", DataSieveVarianceThreshold(threshold=0)),\n        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))\n        ("svm", SVMOutlierExtractor()),\n        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))\n        ("pca", DataSievePCA(n_components=0.95),\n        ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))\n    ])\n\n```\n\nOnce the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:\n\n```python\nX, y, sample_weight = feature_pipeline.fit_transform(X, y, sample_weight)\n```\n\nThis pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn\'s pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.\n\nNext, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:\n\n```python\nX2, _, _ = feature_pipeline.transform(X2)\n\n```\n\nFinally, similar to SKLearn\'s pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:\n\n```python\nXinv, _ ,_ = feature_pipeline.inverse_transform(X)\n```\n\n## Data removal\n\nThe command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step\'s `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. \n\n## Feature modification\n\nAnother feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.\n\n## Adding a custom step\n\nEach step of the `Pipeline` *must* contain the following methods:\n\n```python\nclass MyTransformer:\n    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        X, y, sample_weight = self.fit(X, y, sample_weight)\n        X, y, sample_weight = self.transform(X, y, sample_weight)\n        return X, y, sample_weight, feature_list\n\n    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        return X, y, sample_weight, feature_list\n\n    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        return X, y, sample_weight, feature_list\n\n    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        return X, y, sample_weight, feature_list\n```\n\nThis is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:\n\n```python\nclass DataSieveMinMaxScaler(MinMaxScaler):\n    """\n    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and\n    inverse_transform all take the full set of params X, y, sample_weight (even if they\n    are unused) to follow the FlowdaptPipeline API.\n    """\n\n    def __init__(self, **kwargs):\n        super().__init__(**kwargs)\n\n    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        super().fit(X)\n        X = super().transform(X)\n        return X, y, sample_weight, feature_list\n\n    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        super().fit(X)\n        return X, y, sample_weight, feature_list\n\n    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        X = super().transform(X)\n        return X, y, sample_weight, feature_list\n\n    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):\n        return super().inverse_transform(X), y, sample_weight, feature_list\n```\n\n\n\n# Installation\n\nThe easiest way to install `datasieve` is with:\n\n```\npip install datasieve\n```\n\nbut you can also clone this repository and install it with:\n\n```\ngit clone https://github.com/emergentmethods/datasieve.git\ncd datasieve\npoetry install\n```\n\n\n# License\n\nCopyright (c) 2023 DataSieve\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.',
-    'author': 'Robert Caulk',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+- fits an arbitrary series of transformations to an array X
+- transforms subsequent arrays of the same dimension according to the fit from the original X
+- inverse transforms arrays by inverting the series of transformations
 
+This means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.
 
-setup(**setup_kwargs)
+The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
+
+- removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
+- remove feature columns based on arbitrary criteria (e.g. low variance features)
+- change feature column names at certain transformations (e.g. PCA)
+- passing dynamic parameters to individual transforms of the pipeline
+- passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
+- customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
+
+These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
+
+An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
+
+```python
+class SVMOutlierExtractor(SGDOneClassSVM):
+    """
+    A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
+    for removing detected outliers from X (as well as the associated y and
+    sample_weight if they are also furnished.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self.fit(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight=sample_weight)
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X, y=y, sample_weight=sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        y_pred = self.predict(X)
+
+        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+
+        num_tossed = len(y_pred) - len(X)
+        if num_tossed > 0:
+            logger.info(
+                f"SVM detected {num_tossed} data points"
+                "as outliers."
+            )
+
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        """
+        Unused, pass through X, y, sample_weight, and feature_list
+        """
+        return X, y, sample_weight, feature_list
+```
+
+
+As shown here, the `fit()` method is actually identical to the SKLearn `fit()` method, but the `transform()` removes data points from X, y, and sample_weight for any outliers detected in the `X` array.
+
+
+# Usage
+The user builds the pipeline similarly to SKLearn:
+
+```python
+    from datasieve.pipeline import Pipeline
+    from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
+
+    feature_pipeline = Pipeline([
+        ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
+        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("svm", SVMOutlierExtractor()),
+        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pca", DataSievePCA(n_components=0.95),
+        ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+    ])
+
+```
+
+Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
+
+```python
+X, y, sample_weight = feature_pipeline.fit_transform(X, y, sample_weight)
+```
+
+This pipeline demonstrates the various components of `DataSieve` which are missing from SKLearn's pipeline. A dataframe `X` (if desired, else users can input a simply array without column names) is input with its associated `y` and `sample_weight` arrays/vectors. The `VarianceThreshold` will first detect and remove any features that have zero variance in X, the `SVMOutlierExtractor` will fit `SGDOneClassSVM` to `X` and then remove the detected outliers in `X`, while also propagating those row removals from `y` and `sample_weight`. Finally, the `PCA` will be fit to the remaining `X` array with the features count changing and getting renamed. The returned `X` dataframe will have the correctly named column features/count, and equal row counts across the `X`, `y`, and `sample_weight` arrays.
+
+Next, the `feature_pipeline` can then be used to transform other datasets with the same input feature dimension:
+
+```python
+X2, _, _ = feature_pipeline.transform(X2)
+
+```
+
+Finally, similar to SKLearn's pipeline, the `feature_pipeline` can be used to inverse_transform an array `X3` array that has the same dimensions as the returned `X` array from the pipeline:
+
+```python
+Xinv, _ ,_ = feature_pipeline.inverse_transform(X)
+```
+
+## Data removal
+
+The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `FlowdaptMinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `FlowdaptPipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
+
+## Feature modification
+
+Another feature is demonstrated in the `FlowdaptPCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `FlowdaptPipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `FlowdaptVarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `FlowdaptVarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
+
+## Adding a custom step
+
+Each step of the `Pipeline` *must* contain the following methods:
+
+```python
+class MyTransformer:
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X, y, sample_weight = self.fit(X, y, sample_weight)
+        X, y, sample_weight = self.transform(X, y, sample_weight)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return X, y, sample_weight, feature_list
+```
+
+This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
+
+```python
+class DataSieveMinMaxScaler(MinMaxScaler):
+    """
+    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
+    inverse_transform all take the full set of params X, y, sample_weight (even if they
+    are unused) to follow the FlowdaptPipeline API.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        super().fit(X)
+        return X, y, sample_weight, feature_list
+
+    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        X = super().transform(X)
+        return X, y, sample_weight, feature_list
+
+    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        return super().inverse_transform(X), y, sample_weight, feature_list
+```
+
+
+
+# Installation
+
+The easiest way to install `datasieve` is with:
+
+```
+pip install datasieve
+```
+
+but you can also clone this repository and install it with:
+
+```
+git clone https://github.com/emergentmethods/datasieve.git
+cd datasieve
+poetry install
+```
+
+
+# License
+
+Copyright (c) 2023 DataSieve
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```


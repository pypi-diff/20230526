# Comparing `tmp/datasieve-0.0.3.tar.gz` & `tmp/datasieve-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.3.tar", max compression
+gzip compressed data, was "datasieve-0.0.5.tar", max compression
```

## Comparing `datasieve-0.0.3.tar` & `datasieve-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-26 13:34:19.758625 datasieve-0.0.3/LICENSE
--rw-r--r--   0        0        0    10058 2023-05-26 13:34:19.758625 datasieve-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/__init__.py
--rw-r--r--   0        0        0     6164 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5593 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3007 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1567 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1502 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1432 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-26 13:34:19.758625 datasieve-0.0.3/datasieve/utils.py
--rw-r--r--   0        0        0      542 2023-05-26 13:34:19.758625 datasieve-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    10698 1970-01-01 00:00:00.000000 datasieve-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-26 15:11:03.067443 datasieve-0.0.5/LICENSE
+-rw-r--r--   0        0        0    11154 2023-05-26 15:11:03.067443 datasieve-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/__init__.py
+-rw-r--r--   0        0        0     6886 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3137 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1567 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1724 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1432 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/utils.py
+-rw-r--r--   0        0        0      542 2023-05-26 15:11:03.067443 datasieve-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11794 1970-01-01 00:00:00.000000 datasieve-0.0.5/PKG-INFO
```

### Comparing `datasieve-0.0.3/LICENSE` & `datasieve-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/README.md` & `datasieve-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 This means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.
 
 The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
 
 - removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
+- needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
 These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
 An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
@@ -160,14 +161,31 @@
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         return super().inverse_transform(X), y, sample_weight, feature_list
 ```
 
 
+## Outlier checking
+
+DataSieve also allows users to fit a pipeline that can be used to flag outliers in data *without* removing them from the dataset. This may be handy in a variety of cases where keeping the data point is important but having some indication of which points are outliers is also important. In order to use this functionality, you can take an already `fit` pipeline and call `transform(X, outlier_check=True)` which will return X as well as a vector of 1s and 0s indicating which points are outliers. This is demonstrated in the following example:
+
+```python
+pipeline = Pipeline([
+    ("pre_svm_scaler", transforms.DataSieveMinMaxScaler()),
+    ("svm", transforms.SVMOutlierExtractor())
+])
+
+pipeline.fit(X)
+
+X, outliers, _ = pipeline.transform(X, outlier_check=True)
+```
+
+Now X will *not* have any of the outlier data points removed, but the vector `outliers` will be an indication of which points were classified as outliers, where 0 means the point was an outlier and 1 means that the point was an inlier.
+
 
 # Installation
 
 The easiest way to install `datasieve` is with:
 
 ```
 pip install datasieve
```

### Comparing `datasieve-0.0.3/datasieve/pipeline.py` & `datasieve-0.0.5/datasieve/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import copy
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
 class Pipeline:
 
-    def __init__(self, steps: List[Tuple] = [], fitparams: dict[str, dict] = {}):
+    def __init__(self, steps: List[Tuple] = [],
+                 fitparams: dict[str, dict] = {}):
         """
         Pipeline object which holds a list of fit/transform objects.
         :param steps: list of tuples (str, transform())
         :param fitparams: dictionary of dictionaries, where the string key
         matches the str used to name the step in the steps list.
         """
         self.steps: List[Tuple] = steps
@@ -50,27 +51,28 @@
                 **self.fitparams[name]
             )
 
         X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list)
 
         return X, y, sample_weight
 
-    def transform(self, X, y=None, sample_weight=None) -> Tuple[npt.ArrayLike,
+    def transform(self, X, y=None, sample_weight=None, outlier_check=False) -> Tuple[npt.ArrayLike,
                                                                 npt.ArrayLike,
                                                                 npt.ArrayLike]:
-        X, y, sample_weight = self._validate_arguments(X, y, sample_weight)
+        X, y, sample_weight = self._validate_arguments(X, y, sample_weight, outlier_check=outlier_check)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in enumerate(self.steps):
             logger.debug(f"Transforming {name}")
             X, y, sample_weight, feature_list = trans.transform(
                 X,
                 y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
+                outlier_check=outlier_check,
                 **self.fitparams[name]
             )
 
         X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list)
 
         return X, y, sample_weight
 
@@ -106,15 +108,16 @@
                 **self.fitparams[name]
             )
 
         X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list)
 
         return X, y, sample_weight
 
-    def _validate_arguments(self, X, y, sample_weight, fit=False):
+    # flake8: noqa: C901
+    def _validate_arguments(self, X, y, sample_weight, fit=False, outlier_check=False):
         if isinstance(X, pd.DataFrame) and fit:
             self.pandas_types = True
             self.feature_list = X.columns
             if y is not None:
                 self.label_list = y.columns
         elif fit:
             self.pandas_types = False
@@ -138,14 +141,26 @@
             except AttributeError:
                 raise Exception("Pipeline was fit with a dataframe, but it received "
                                 f" {type(X)} instead.")
 
         if isinstance(sample_weight, pd.DataFrame) and sample_weight is not None:
             sample_weight = sample_weight.to_numpy()
 
+        if not fit and outlier_check:
+            if y is not None:
+                raise Exception("Asking for outlier_check vector, but passed in y."
+                                "outlier_check functionality only works when passing X"
+                                "for pipeline.transform(X)")
+            else:
+                y = np.ones(X.shape[0])
+
+        if fit and outlier_check:
+            raise Exception("Asking for outlier_check with fit() is not possible."
+                            "outlier_check functionality only works with transform.")
+
         return X, y, sample_weight
 
     def _convert_back_to_df(self, X, y, sample_weight, feature_list):
         if not self.pandas_types:
             return X, y, sample_weight
 
         assert X.shape[1] == len(feature_list)
```

### Comparing `datasieve-0.0.3/datasieve/transforms/__init__.py` & `datasieve-0.0.5/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/datasieve/transforms/dbscan.py` & `datasieve-0.0.5/datasieve/transforms/dbscan.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,35 +60,39 @@
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             super().fit(X)
 
         self.train_features = X
 
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None, feature_list=None,
+                  outlier_check=False, **kwargs):
         """
         Given a data point (or data points), append them to the
         train_features and determine if they are inliers.
         """
 
         num_X = X.shape[0]
         fullX = np.concatenate([self.train_features, X], axis=0)
 
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             logger.info(f"Using eps {self.eps} and min_samples {self.min_samples} to transform")
             clustering = super().fit(fullX)
 
         inliers = np.where(clustering.labels_[-num_X:] == -1, 0, 1)
 
-        X, y, sample_weight = remove_outliers(X, y, sample_weight, inliers=inliers)
-
-        logger.info(
-            f"DBSCAN tossed {len(inliers) - X.shape[0]}"
-            f" train points from {len(self.labels_)} in transform()"
-        )
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, inliers=inliers)
+            logger.info(
+                f"DBSCAN tossed {len(inliers) - X.shape[0]}"
+                f" train points from {len(self.labels_)} in transform()"
+            )
+        else:
+            y += inliers
+            y -= 1
 
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Unused
         """
```

### Comparing `datasieve-0.0.3/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.5/datasieve/transforms/dissimilarity_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,29 +43,34 @@
         np.fill_diagonal(pairwise, np.NaN)
         pairwise = pairwise.reshape(-1, 1)
         self.avg_mean_dist = pairwise[~np.isnan(pairwise)].mean()
         self.trained_data = X
 
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  feature_list=None, outlier_check=False, **kwargs):
         """
         Compares the distance from each prediction point to each training data
         point. It uses this information to estimate a Dissimilarity Index (DI)
         and avoid making predictions on any points that are too far away
         from the training data set.
         """
 
         with parallel_backend(self.backend, n_jobs=self.n_jobs):
             distance = pairwise_distances(self.trained_data, X)
 
         self.di_values = distance.min(axis=0) / self.avg_mean_dist
         y_pred = np.where(self.di_values < self.di_threshold, 1, 0)
 
-        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+        else:
+            y += y_pred
+            y -= 1
 
         num_tossed = len(y_pred) - len(X)
         if num_tossed > 0:
             logger.info(
                 f"DI tossed {num_tossed} predictions for "
                 "being too far from training data."
             )
```

### Comparing `datasieve-0.0.3/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.5/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/datasieve/transforms/pca.py` & `datasieve-0.0.5/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.5/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from sklearn.linear_model import SGDOneClassSVM
 from datasieve.utils import remove_outliers
 import logging
+import numpy as np
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
 class SVMOutlierExtractor(SGDOneClassSVM):
     """
     A subclass of the SKLearn SGDOneClassSVM that adds a transform() method
@@ -19,25 +20,29 @@
         self.fit(X, y, sample_weight=sample_weight)
         return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         super().fit(X, y=y, sample_weight=sample_weight)
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None, feature_list=None,
+                  outlier_check=False, **kwargs):
         y_pred = self.predict(X)
-
-        X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
-
-        num_tossed = len(y_pred) - len(X)
-        if num_tossed > 0:
-            logger.info(
-                f"SVM detected {num_tossed} data points"
-                "as outliers."
-            )
+        y_pred = np.where(y_pred == -1, 0, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+            num_tossed = len(y_pred) - len(X)
+            if num_tossed > 0:
+                logger.info(
+                    f"SVM detected {num_tossed} data points"
+                    "as outliers."
+                )
+        else:
+            y += y_pred
+            y -= 1
 
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
         Unused
         """
```

### Comparing `datasieve-0.0.3/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.5/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/datasieve/utils.py` & `datasieve-0.0.5/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.3/pyproject.toml` & `datasieve-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.3"
+version = "0.0.5"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.0.3/PKG-INFO` & `datasieve-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.3
+Version: 0.0.5
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,15 @@
 This means that it follows the SKLearn API very closely, and in fact most of the methods inherit directly from SKLearn methods.
 
 The main **difference** is that DataSieve allows for the manipulation of the y and sample_weight arrays in addition to the X array. This is useful if you find yourself wishing to use the SKLearn pipeline for:
 
 - removing outliers across your X, y, and sample_weights arrays according to simple or complex criteria
 - remove feature columns based on arbitrary criteria (e.g. low variance features)
 - change feature column names at certain transformations (e.g. PCA)
+- needing outlier classification without removal (see `oulier_check`)
 - passing dynamic parameters to individual transforms of the pipeline
 - passing dataframes/arrays without worrying about converting to arrays and maintaining the proper feature columns
 - customizing backend for parallelization (e.g. Dask, Ray, loky, etc.)
 
 These improved flexibilities allow for more customized/creative transformations. For example, the included `DataSieveDBSCAN` has automated parameter fitting and outlier removal based on clustering. 
 
 An example would be someone who wants to use `SGDOneClassSVM` to detect and remove outliers from their data set before training:
@@ -176,14 +177,31 @@
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         return super().inverse_transform(X), y, sample_weight, feature_list
 ```
 
 
+## Outlier checking
+
+DataSieve also allows users to fit a pipeline that can be used to flag outliers in data *without* removing them from the dataset. This may be handy in a variety of cases where keeping the data point is important but having some indication of which points are outliers is also important. In order to use this functionality, you can take an already `fit` pipeline and call `transform(X, outlier_check=True)` which will return X as well as a vector of 1s and 0s indicating which points are outliers. This is demonstrated in the following example:
+
+```python
+pipeline = Pipeline([
+    ("pre_svm_scaler", transforms.DataSieveMinMaxScaler()),
+    ("svm", transforms.SVMOutlierExtractor())
+])
+
+pipeline.fit(X)
+
+X, outliers, _ = pipeline.transform(X, outlier_check=True)
+```
+
+Now X will *not* have any of the outlier data points removed, but the vector `outliers` will be an indication of which points were classified as outliers, where 0 means the point was an outlier and 1 means that the point was an inlier.
+
 
 # Installation
 
 The easiest way to install `datasieve` is with:
 
 ```
 pip install datasieve
```


# Comparing `tmp/datasieve-0.0.5.tar.gz` & `tmp/datasieve-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.5.tar", max compression
+gzip compressed data, was "datasieve-0.0.6.tar", max compression
```

## Comparing `datasieve-0.0.5.tar` & `datasieve-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-26 15:11:03.067443 datasieve-0.0.5/LICENSE
--rw-r--r--   0        0        0    11154 2023-05-26 15:11:03.067443 datasieve-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/__init__.py
--rw-r--r--   0        0        0     6886 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3137 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1567 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1724 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1432 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-26 15:11:03.067443 datasieve-0.0.5/datasieve/utils.py
--rw-r--r--   0        0        0      542 2023-05-26 15:11:03.067443 datasieve-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11794 1970-01-01 00:00:00.000000 datasieve-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-26 18:39:04.053830 datasieve-0.0.6/LICENSE
+-rw-r--r--   0        0        0    11157 2023-05-26 18:39:04.053830 datasieve-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/__init__.py
+-rw-r--r--   0        0        0     7110 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3137 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1567 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1725 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1432 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/utils.py
+-rw-r--r--   0        0        0      542 2023-05-26 18:39:04.057830 datasieve-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11797 1970-01-01 00:00:00.000000 datasieve-0.0.6/PKG-INFO
```

### Comparing `datasieve-0.0.5/LICENSE` & `datasieve-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/README.md` & `datasieve-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         y_pred = self.predict(X)
 
         X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
 
         num_tossed = len(y_pred) - len(X)
         if num_tossed > 0:
             logger.info(
-                f"SVM detected {num_tossed} data points"
+                f"SVM detected {num_tossed} data points "
                 "as outliers."
             )
 
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
@@ -71,17 +71,17 @@
 
 ```python
     from datasieve.pipeline import Pipeline
     from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
 
     feature_pipeline = Pipeline([
         ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
         ("svm", SVMOutlierExtractor()),
-        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
         ("pca", DataSievePCA(n_components=0.95),
         ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
```

### Comparing `datasieve-0.0.5/datasieve/pipeline.py` & `datasieve-0.0.6/datasieve/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 
     def _validate_fitparams(self, fitparams: dict[str, dict], steps: List[Tuple]):
         for _, (name, _) in enumerate(steps):
             if name not in fitparams.keys():
                 fitparams[name] = {}  # add an empty dict
 
         return fitparams
+    
+    def get_step(self, name: str):
+        for _, (step_name, step) in enumerate(self.steps):
+            if step_name == name:
+                return step
+
+        raise Exception(f"Step {name} not found in pipeline")
 
     def fit_transform(self, X, y=None, sample_weight=None) -> Tuple[npt.ArrayLike,
                                                                     npt.ArrayLike,
                                                                     npt.ArrayLike]:
         """
         Iterate through the pipeline calling fit_transform() on each of the
         transformations
```

### Comparing `datasieve-0.0.5/datasieve/transforms/__init__.py` & `datasieve-0.0.6/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/transforms/dbscan.py` & `datasieve-0.0.6/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.6/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.6/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/transforms/pca.py` & `datasieve-0.0.6/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.6/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         y_pred = self.predict(X)
         y_pred = np.where(y_pred == -1, 0, y_pred)
         if not outlier_check:
             X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
             num_tossed = len(y_pred) - len(X)
             if num_tossed > 0:
                 logger.info(
-                    f"SVM detected {num_tossed} data points"
+                    f"SVM detected {num_tossed} data points "
                     "as outliers."
                 )
         else:
             y += y_pred
             y -= 1
 
         return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.0.5/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.6/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/datasieve/utils.py` & `datasieve-0.0.6/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.5/pyproject.toml` & `datasieve-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.5"
+version = "0.0.6"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.0.5/PKG-INFO` & `datasieve-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -61,15 +61,15 @@
         y_pred = self.predict(X)
 
         X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
 
         num_tossed = len(y_pred) - len(X)
         if num_tossed > 0:
             logger.info(
-                f"SVM detected {num_tossed} data points"
+                f"SVM detected {num_tossed} data points "
                 "as outliers."
             )
 
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         """
@@ -87,17 +87,17 @@
 
 ```python
     from datasieve.pipeline import Pipeline
     from datasieve.transforms import DataSieveMinMaxScaler, DataSievePCA, DataSieveVarianceThreshold, SVMOutlierExtractor
 
     feature_pipeline = Pipeline([
         ("detect_constants", DataSieveVarianceThreshold(threshold=0)),
-        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pre_svm_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
         ("svm", SVMOutlierExtractor()),
-        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
+        ("pre_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1))),
         ("pca", DataSievePCA(n_components=0.95),
         ("post_pca_scaler", DataSieveMinMaxScaler(feature_range=(-1, 1)))
     ])
 
 ```
 
 Once the pipeline is built, it can be fit and transformed similar to a SKLearn pipeline:
```


# Comparing `tmp/td_ml_cltv-0.0.4.tar.gz` & `tmp/td_ml_cltv-0.0.5.tar.gz`

## Comparing `td_ml_cltv-0.0.4.tar` & `td_ml_cltv-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/.DS_Store
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/src/td_ml_cltv/__init__.py
--rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/src/td_ml_cltv/cltv_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/.DS_Store
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/src/td_ml_cltv/__init__.py
+-rw-r--r--   0        0        0    12626 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/src/td_ml_cltv/cltv_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.5/PKG-INFO
```

### Comparing `td_ml_cltv-0.0.4/.DS_Store` & `td_ml_cltv-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_cltv-0.0.4/src/td_ml_cltv/cltv_helpers.py` & `td_ml_cltv-0.0.5/src/td_ml_cltv/cltv_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 from sklearn.linear_model import LinearRegression
 from xgboost import XGBRegressor, plot_importance
 # import lightgbm as lgb
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, RobustScaler
 from sklearn.model_selection import train_test_split
 import sklearn.metrics as metrics
 from scipy.stats import skew, kurtosis, binned_statistic
+from sklearn import preprocessing
 
 import shap
+from sklearn.cluster import KMeans
+from sklearn.impute import SimpleImputer
+from scipy.sparse import issparse
+from shap.utils._legacy import DenseData
 import warnings
 warnings.filterwarnings("ignore")
 
 #Read data from TD using new optimized query     
 @profile
 def new_query(database, query_syntax, td_api_key, td_api_server):
 
@@ -108,33 +113,31 @@
     return df_final
 
 
 
    
 # Function for getting importances via coefficients
 @profile
-def impt_coef(model, x_data, target, k=100):
-
+def impt_coef(model, x_data):
     try:
         importances = model.coef_
     except:
         importances = model.feature_importances_
 
     features = x_data.columns
-    
     feat_impt = sorted(list(zip(features, importances)), key=lambda x: x[1])
     
     return pd.DataFrame(feat_impt, columns=['feature', 'weight'])
 
 # Feature importances for trees
-def impt_tree(model, x_data, target, k=100):
+def impt_tree(model, x_data, canonical_id):
 
     try:
       #Try Standard Method
-        baseline = get_feature_kmeans(x_data)
+        baseline = get_feature_kmeans(x_data, canonical_id)
         shap_values = shap.TreeExplainer(model).shap_values(baseline)
 
         #Get SHAP Values from Kmeans features
         features = baseline.columns
         shap_vals = np.abs(shap_values).mean(0)
         shap_list = list(zip(features, shap_vals))
         shap_sorted = sorted(shap_list, key=lambda tup: tup[1], reverse = True)
@@ -264,18 +267,14 @@
         For all i, round the ith dimension of each mean sample to match the nearest value
         from X[:,i]. This ensures discrete features always get a valid value.
 
     Returns
     -------
     DenseData object.
     """
-    from sklearn.cluster import KMeans
-    from sklearn.impute import SimpleImputer
-    from scipy.sparse import issparse
-
     group_names = [str(i) for i in range(X.shape[1])]
     df_X = X
     if str(type(X)).endswith("'pandas.core.frame.DataFrame'>"):
         group_names = X.columns
         X = X.values
 
     # in case there are any missing values in data impute them
@@ -289,21 +288,20 @@
 
     if round_values:
         for i in range(k):
             for j in range(X.shape[1]):
                 xj = X[:, j].toarray().flatten() if issparse(X) else X[:, j]  # sparse support courtesy of @PrimozGodec
                 ind = np.argmin(np.abs(xj - kmeans.cluster_centers_[i, j]))
                 kmeans.cluster_centers_[i, j] = X[ind, j]
-    from shap.utils._legacy import DenseData
 
     return DenseData(kmeans.cluster_centers_, group_names, None, 1.0 * np.bincount(kmeans.labels_))
 
 def get_feature_kmeans(x_data, canonical_id):
     
-    from sklearn import preprocessing
+    
     le = preprocessing.LabelEncoder()
     
     #drop index from DF
     df = x_data.copy()
     df.reset_index(inplace = True)
     df.drop([canonical_id], axis =1, inplace = True)
```

### Comparing `td_ml_cltv-0.0.4/pyproject.toml` & `td_ml_cltv-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "td_ml_cltv"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Yish Lim", email="yish.lim@treasure-data.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```


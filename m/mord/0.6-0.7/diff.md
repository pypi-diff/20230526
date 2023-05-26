# Comparing `tmp/mord-0.6.tar.gz` & `tmp/mord-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mord-0.6.tar", last modified: Wed Jul 25 14:34:06 2018, max compression
+gzip compressed data, was "mord-0.7.tar", last modified: Fri May 26 11:50:49 2023, max compression
```

## Comparing `mord-0.6.tar` & `mord-0.7.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2018-07-25 14:34:06.000000 mord-0.6/
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2018-07-25 14:34:06.000000 mord-0.6/mord.egg-info/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        5 2018-07-25 14:34:06.000000 mord-0.6/mord.egg-info/top_level.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      240 2018-07-25 14:34:06.000000 mord-0.6/mord.egg-info/SOURCES.txt
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      727 2018-07-25 14:34:06.000000 mord-0.6/mord.egg-info/PKG-INFO
--rw-rw-r--   0 jeff      (1000) jeff      (1000)        1 2018-07-25 14:34:06.000000 mord-0.6/mord.egg-info/dependency_links.txt
-drwxrwxr-x   0 jeff      (1000) jeff      (1000)        0 2018-07-25 14:34:06.000000 mord-0.6/mord/
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1872 2018-07-25 14:31:11.000000 mord-0.6/mord/multiclass.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      134 2018-07-25 14:31:40.000000 mord-0.6/mord/__init__.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)     1390 2018-07-25 14:31:11.000000 mord-0.6/mord/regression_based.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)    10202 2018-07-25 14:31:11.000000 mord-0.6/mord/threshold_based.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      284 2018-07-25 14:31:11.000000 mord-0.6/mord/utils.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      363 2018-07-25 14:31:11.000000 mord-0.6/README.rst
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      154 2018-07-25 14:34:06.000000 mord-0.6/setup.cfg
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      343 2018-07-25 14:31:31.000000 mord-0.6/setup.py
--rw-rw-r--   0 jeff      (1000) jeff      (1000)      727 2018-07-25 14:34:06.000000 mord-0.6/PKG-INFO
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.516692 mord-0.7/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     1516 2023-05-26 11:49:51.000000 mord-0.7/LICENSE.txt
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)       44 2023-05-26 11:49:51.000000 mord-0.7/MANIFEST.in
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      901 2023-05-26 11:50:49.516774 mord-0.7/PKG-INFO
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      610 2023-05-26 11:49:51.000000 mord-0.7/README.rst
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.514924 mord-0.7/mord/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      134 2023-05-26 11:50:36.000000 mord-0.7/mord/__init__.py
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.516007 mord-0.7/mord/datasets/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:49:51.000000 mord-0.7/mord/datasets/__init__.py
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     1840 2023-05-26 11:49:51.000000 mord-0.7/mord/datasets/base.py
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.516300 mord-0.7/mord/datasets/data/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     2461 2023-05-26 11:49:51.000000 mord-0.7/mord/datasets/data/copenhagen_housing_survey.csv
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.516517 mord-0.7/mord/datasets/descr/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     1289 2023-05-26 11:49:51.000000 mord-0.7/mord/datasets/descr/copenhagen_housing_survey.rst
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     1872 2023-05-26 11:49:51.000000 mord-0.7/mord/multiclass.py
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)     1389 2023-05-26 11:49:51.000000 mord-0.7/mord/regression_based.py
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)    10190 2023-05-26 11:49:51.000000 mord-0.7/mord/threshold_based.py
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      284 2023-05-26 11:49:51.000000 mord-0.7/mord/utils.py
+drwxr-xr-x   0 pedregosa (610101) primarygroup (89939)        0 2023-05-26 11:50:49.515766 mord-0.7/mord.egg-info/
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      901 2023-05-26 11:50:49.000000 mord-0.7/mord.egg-info/PKG-INFO
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      411 2023-05-26 11:50:49.000000 mord-0.7/mord.egg-info/SOURCES.txt
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)        1 2023-05-26 11:50:49.000000 mord-0.7/mord.egg-info/dependency_links.txt
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)        5 2023-05-26 11:50:49.000000 mord-0.7/mord.egg-info/top_level.txt
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      154 2023-05-26 11:50:49.517102 mord-0.7/setup.cfg
+-rw-r--r--   0 pedregosa (610101) primarygroup (89939)      448 2023-05-26 11:50:17.000000 mord-0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mord-0.6/mord.egg-info/PKG-INFO` & `mord-0.7/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 1.1
-Name: mord
-Version: 0.6
-Summary: Ordinal regression models
-Home-page: https://pypi.python.org/pypi/mord
-Author: Fabian Pedregosa
-Author-email: f@bianp.net
-License: UNKNOWN
-Description: .. image:: https://travis-ci.org/fabianp/mord.svg?branch=master
-            :target: https://travis-ci.org/fabianp/mord
-        
-        mord: ordinal regression in Python
-        ==================================
-        
-        Collection of Ordinal Regression algorithms in Python, following a scikit-learn compatible API.
-        
-        Docs: https://pythonhosted.org/mord/
-        
-        Github repo: http://github.com/fabianp/mord
-        
-Platform: UNKNOWN
-Requires: numpy
-Requires: scipy
-Requires: sklearn
+.. image:: https://travis-ci.org/fabianp/mord.svg?branch=master
+    :target: https://travis-ci.org/fabianp/mord
+
+mord: ordinal regression in Python
+==================================
+
+Collection of Ordinal Regression algorithms in Python, following a scikit-learn compatible API.
+
+Docs: https://pythonhosted.org/mord/
+
+Github repo: http://github.com/fabianp/mord
+
+
+References
+----------
+
+Pedregosa, Fabian, Francis Bach, and Alexandre Gramfort. "On the consistency of ordinal regression methods." The Journal of Machine Learning Research 18.1 (2017) `JMLR <http://jmlr.csail.mit.edu/papers/v18/15-495.html>`_.
```

### Comparing `mord-0.6/mord/multiclass.py` & `mord-0.7/mord/multiclass.py`

 * *Files identical despite different names*

### Comparing `mord-0.6/mord/regression_based.py` & `mord-0.7/mord/regression_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from sklearn import linear_model, svm, metrics
 
 
 class OrdinalRidge(linear_model.Ridge):
     """
     Overwrite Ridge from scikit-learn to use
-    the (minus) absolute error as score function.
+    the (minus) squared error as score function.
 
     (see https://github.com/scikit-learn/scikit-learn/issues/3848
     on why this cannot be accomplished using a GridSearchCV object)
     """
 
     def fit(self, X, y, **fit_params):
         self.unique_y_ = np.unique(y)
```

### Comparing `mord-0.6/mord/threshold_based.py` & `mord-0.7/mord/threshold_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 
 def threshold_predict(X, w, theta):
     """
     Class numbers are assumed to be between 0 and k-1
     """
     tmp = theta[:, None] - np.asarray(X.dot(w))
-    pred = np.sum(tmp < 0, axis=0).astype(np.int)
+    pred = np.sum(tmp < 0, axis=0).astype(int)
     return pred
 
 
 def threshold_proba(X, w, theta):
     """
     Class numbers are assumed to be between 0 and k-1. Assumes
     the `sigmoid` link function is used.
@@ -182,15 +182,15 @@
     """
     def __init__(self, alpha=1., verbose=0, max_iter=1000):
         self.alpha = alpha
         self.verbose = verbose
         self.max_iter = max_iter
 
     def fit(self, X, y, sample_weight=None):
-        _y = np.array(y).astype(np.int)
+        _y = np.array(y).astype(int)
         if np.abs(_y - y).sum() > 0.1:
             raise ValueError('y must only contain integer values')
         self.classes_ = np.unique(y)
         self.n_class_ = self.classes_.max() - self.classes_.min() + 1
         y_tmp = y - y.min()  # we need classes that start at zero
         self.coef_, self.theta_ = threshold_fit(
             X, y_tmp, self.alpha, self.n_class_, mode='AE',
@@ -238,15 +238,15 @@
     """
     def __init__(self, alpha=1., verbose=0, max_iter=1000):
         self.alpha = alpha
         self.verbose = verbose
         self.max_iter = max_iter
 
     def fit(self, X, y, sample_weight=None):
-        _y = np.array(y).astype(np.int)
+        _y = np.array(y).astype(int)
         if np.abs(_y - y).sum() > 0.1:
             raise ValueError('y must only contain integer values')
         self.classes_ = np.unique(y)
         self.n_class_ = self.classes_.max() - self.classes_.min() + 1
         y_tmp = y - y.min()  # we need classes that start at zero
         self.coef_, self.theta_ = threshold_fit(
             X, y_tmp, self.alpha, self.n_class_,
@@ -293,15 +293,15 @@
     """
     def __init__(self, alpha=1., verbose=0, max_iter=100000):
         self.alpha = alpha
         self.verbose = verbose
         self.max_iter = max_iter
 
     def fit(self, X, y, sample_weight=None):
-        _y = np.array(y).astype(np.int)
+        _y = np.array(y).astype(int)
         if np.abs(_y - y).sum() > 1e-3:
             raise ValueError('y must only contain integer values')
         self.classes_ = np.unique(y)
         self.n_class_ = self.classes_.max() - self.classes_.min() + 1
         y_tmp = y - y.min()  # we need classes that start at zero
         self.coef_, self.theta_ = threshold_fit(
             X, y_tmp, self.alpha, self.n_class_,
```


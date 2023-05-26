# Comparing `tmp/edamame-0.58.tar.gz` & `tmp/edamame-0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.58.tar", last modified: Thu May 25 09:24:37 2023, max compression
+gzip compressed data, was "edamame-0.59.tar", last modified: Fri May 26 19:45:03 2023, max compression
```

## Comparing `edamame-0.58.tar` & `edamame-0.59.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.175084 edamame-0.58/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.58/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:24:37.174610 edamame-0.58/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.58/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.164454 edamame-0.58/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-25 09:22:13.000000 edamame-0.58/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.168510 edamame-0.58/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.58/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22458 2023-05-25 09:08:17.000000 edamame-0.58/edamame/classifier/classification.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8677 2023-05-25 09:21:20.000000 edamame-0.58/edamame/classifier/diagnose.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.170628 edamame-0.58/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.58/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.58/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.58/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.173268 edamame-0.58/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.58/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.58/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.58/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-25 09:24:37.166535 edamame-0.58/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-25 09:24:37.000000 edamame-0.58/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-25 09:24:37.000000 edamame-0.58/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-25 09:24:37.000000 edamame-0.58/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-25 09:24:37.000000 edamame-0.58/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-25 09:24:37.000000 edamame-0.58/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-25 09:22:03.000000 edamame-0.58/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-25 09:24:37.175191 edamame-0.58/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.202644 edamame-0.59/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.59/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-26 19:45:03.201966 edamame-0.59/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10192 2023-05-23 09:35:51.000000 edamame-0.59/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.188220 edamame-0.59/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-05-26 19:36:41.000000 edamame-0.59/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.194460 edamame-0.59/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      194 2023-05-04 19:56:56.000000 edamame-0.59/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22458 2023-05-25 09:08:17.000000 edamame-0.59/edamame/classifier/classification.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9114 2023-05-26 19:44:05.000000 edamame-0.59/edamame/classifier/diagnose.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.198036 edamame-0.59/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      876 2023-05-06 16:04:28.000000 edamame-0.59/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-05-23 21:20:45.000000 edamame-0.59/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4460 2023-05-22 20:40:47.000000 edamame-0.59/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.200803 edamame-0.59/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.59/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8347 2023-05-04 19:55:27.000000 edamame-0.59/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    22021 2023-05-23 08:36:34.000000 edamame-0.59/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-26 19:45:03.191191 edamame-0.59/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11946 2023-05-26 19:45:03.000000 edamame-0.59/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      461 2023-05-26 19:45:03.000000 edamame-0.59/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-26 19:45:03.000000 edamame-0.59/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-05-26 19:45:03.000000 edamame-0.59/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-05-26 19:45:03.000000 edamame-0.59/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-05-26 19:36:32.000000 edamame-0.59/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-26 19:45:03.202758 edamame-0.59/setup.cfg
```

### Comparing `edamame-0.58/LICENSE` & `edamame-0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.58/PKG-INFO` & `edamame-0.59/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.58
+Version: 0.59
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.58/README.md` & `edamame-0.59/README.md`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/classifier/classification.py` & `edamame-0.59/edamame/classifier/classification.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/classifier/diagnose.py` & `edamame-0.59/edamame/classifier/diagnose.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#TODO - fix plot ROC curve if y is a pd.Series
-
+#TODO - update dimension of plot 
 import edamame.eda as eda
 import pandas as pd
 import numpy as np 
 import matplotlib.pyplot as plt 
 from typing import Union
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
@@ -75,28 +74,29 @@
     def __init__(self, X_train: pd.DataFrame, y_train: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame) -> None:
         self.X_train = X_train
         self.y_train = y_train
         self.X_test = X_test
         self.y_test = y_test
 
     
-    def class_prediction_error(self, model: Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC], train_data: bool = True) -> None:
+    def class_prediction_error(self, model: Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC], figsize: Tuple[float, float] = (8.,6.), train_data: bool = True) -> None:
         """
         This plot method shows the support (number of training samples) for each class in the fitted classification model as a stacked bar chart. Each bar is segmented to show the proportion of predictions (including false negatives and false positives, like a Confusion Matrix) for each class
 
         Args:
             model (Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC]): Classification model.
+            figsize (Tuple[float, float]): Figure size for the plot. Defaults to (8, 6).
             train_data (bool): Defines if you want to plot the stacked barplot on train or test data (train by default).
         
         Returns: 
             None
         """
         def stacked_barplot(matrix: np.array, num_of_class: int) -> None:
             cmap = plt.get_cmap('rainbow')
-            plt.figure(figsize=(8,6))
+            plt.figure(figsize=figsize)
             cm_bottom = np.zeros((num_of_class,))
             for i in range(len(matrix)):
                 value = random.uniform(0, 1)
                 clr = cmap(value)
                 if i == 0:
                     plt.bar(range(num_of_class), matrix[i], label=f'Class {i}', color=clr)
                 else: 
@@ -118,20 +118,21 @@
             y_pred = model.predict(self.X_test)
             y_true = self.y_test.squeeze().to_numpy() 
             num_classes = y_true.max() + 1
             cm = confusion_matrix(y_true=y_true, y_pred=y_pred)
             stacked_barplot(matrix=cm, num_of_class=num_classes)
     
 
-    def random_forest_fi(self, model: RandomForestClassifier, figsize: Tuple[float, float] = (12,10)) -> None:
+    def random_forest_fi(self, model: RandomForestClassifier, figsize: Tuple[float, float] = (8.,6.)) -> None:
         """
-        The method displays the feature importance plot of the random forest model. 
+        Displays the feature importance plot of the random forest model.
 
         Args:
             model (RandomForestClassifier): The input random forest model.
+            figsize (Tuple[float, float]): Figure size for the plot. Defaults to (8, 6).
 
         Returns:
             None
         """
         check_random_forest(model)
         importances = model.feature_importances_
         std = np.std([tree.feature_importances_ for tree in model.estimators_], axis=0)
@@ -140,36 +141,38 @@
         plt.figure(figsize=figsize)
         forest_importances.plot.bar(yerr=std)
         plt.title("Feature importances using mean decrease in impurity")
         plt.ylabel("Mean decrease in impurity")
         plt.show()
 
     
-    def xgboost_fi(self, model: XGBClassifier, figsize: tuple[float, float] = (14,12)) -> None:
+    def xgboost_fi(self, model: XGBClassifier, figsize: Tuple[float, float] = (8.,6.)) -> None:
         """
-        The method displays the feature importance plot.
+        Displays the feature importance plot of the xgboost model.
 
         Args:
             model (XGBClassifier): The input xgboost model.
+            figsize (Tuple[float, float]): Figure size for the plot. Defaults to (8, 6).
 
         Returns:
             None
         """
         check_xgboost(model)
         xgb.plot_importance(model)
         plt.rcParams['figure.figsize'] = [figsize[0], figsize[1]]
         plt.show()
 
     
-    def plot_roc_auc(self, model: Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC], train_data: bool = True) -> None: 
+    def plot_roc_auc(self, model: Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC], figsize: Tuple[float, float] = (8.,6.), train_data: bool = True) -> None: 
         """
         Method for plotting the ROC curve and calculating the AUC values for a given model.
 
         Args: 
             model (Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC]): Classification model.
+            figsize (Tuple[float, float]): Figure size for the plot. Defaults to (8, 6).
             train_data (bool): Defines if you want to plot the stacked barplot on train or test data (train by default).
         
         Returns: 
             None
         """
         # One VS All strategy
         def _OVR_roc_curve(x, y, target_data):
@@ -180,15 +183,15 @@
             fpr = dict()
             tpr = dict()
             roc_auc = dict()
             for i in range(n_classes):
                 fpr[i], tpr[i], _ = roc_curve(y_ohe[:, i], y_score[:, i])
                 roc_auc[i] = auc(fpr[i], tpr[i])
             # Plot ROC curve for each class
-            plt.figure()
+            plt.figure(figsize=figsize)
             colors = ['blue', 'red', 'green']
             for i, color in zip(range(n_classes), colors):
                 plt.plot(fpr[i], tpr[i], color=color, lw=2, label=f'ROC curve of class {i} (area = {roc_auc[i]:.2f})')
             # Plot the random chance line
             plt.plot([0, 1], [0, 1], 'k--', lw=2)
             # Set plot properties
             plt.xlim([0.0, 1.0])
```

### Comparing `edamame-0.58/edamame/eda/__init__.py` & `edamame-0.59/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/eda/eda.py` & `edamame-0.59/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/eda/tools.py` & `edamame-0.59/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/regressor/diagnose.py` & `edamame-0.59/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame/regressor/regression.py` & `edamame-0.59/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.58/edamame.egg-info/PKG-INFO` & `edamame-0.59/edamame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.58
+Version: 0.59
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `edamame-0.58/pyproject.toml` & `edamame-0.59/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.58"
+version = "0.59"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```


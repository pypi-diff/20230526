# Comparing `tmp/regi-1.2.tar.gz` & `tmp/regi-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regi-1.2.tar", last modified: Fri May 26 23:14:39 2023, max compression
+gzip compressed data, was "regi-2.0.tar", last modified: Sat May 27 00:00:10 2023, max compression
```

## Comparing `regi-1.2.tar` & `regi-2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.122681 regi-1.2/
--rw-rw-rw-   0        0        0        0 2023-05-26 22:43:45.000000 regi-1.2/LICENCE.txt
--rw-rw-rw-   0        0        0      180 2023-05-26 23:14:39.119684 regi-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.053722 regi-1.2/main/
--rw-rw-rw-   0        0        0        0 2023-05-26 22:42:48.000000 regi-1.2/main/__init__.py
--rw-rw-rw-   0        0        0     3177 2023-05-26 22:56:58.000000 regi-1.2/main/regi.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:14:39.114686 regi-1.2/regi.egg-info/
--rw-rw-rw-   0        0        0      180 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 23:14:38.000000 regi-1.2/regi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 23:14:39.122681 regi-1.2/setup.cfg
--rw-rw-rw-   0        0        0      278 2023-05-26 23:14:20.000000 regi-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.736354 regi-2.0/
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:02.000000 regi-2.0/LICENCE.txt
+-rw-rw-rw-   0        0        0      180 2023-05-27 00:00:10.734354 regi-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-26 23:25:16.000000 regi-2.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.671391 regi-2.0/regi/
+-rw-rw-rw-   0        0        0       42 2023-05-26 23:59:55.000000 regi-2.0/regi/__init__.py
+-rw-rw-rw-   0        0        0     2033 2023-05-26 23:59:52.000000 regi-2.0/regi/regi.py
+drwxrwxrwx   0        0        0        0 2023-05-27 00:00:10.729359 regi-2.0/regi.egg-info/
+-rw-rw-rw-   0        0        0      180 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-27 00:00:09.000000 regi-2.0/regi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 00:00:10.736354 regi-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      353 2023-05-26 23:59:54.000000 regi-2.0/setup.py
```

### Comparing `regi-1.2/main/regi.py` & `regi-2.0/regi/regi.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,30 +16,18 @@
         
     slope = numerator / denominator
     y_intercept = y_mean - slope * x_mean
     
     return slope, y_intercept
 
 # define a function to make predictions using the calculated slope and y-intercept
-def predict(x, slope, y_intercept):
+def predict_linear(x, slope, y_intercept):
     y_pred = slope * x + y_intercept
     return y_pred
 
-# example usage
-np.random.seed(0)
-x = np.random.rand(100, 1)
-y = 2 + 3 * x + np.random.randn(100, 1)
-
-slope, y_intercept = linear_regression(x, y)
-print('slope:', slope)
-print('y-intercept:', y_intercept)
-
-x_new = 6
-y_pred = predict(x_new, slope, y_intercept)
-print('predicted value for x = {}:'.format(x_new), y_pred)
 
 
 
 #polynomial regression
 import numpy as np
 
 # define a function to create a polynomial feature matrix
@@ -55,61 +43,39 @@
 def polynomial_regression(x, y, degree):
     x_poly = create_polynomial_features(x, degree)
     model = np.linalg.lstsq(x_poly, y, rcond=None)[0]
     
     return model
 
 # define a function to make predictions using the polynomial model
-def predict(x, model):
+def predict_polynomial(x, model):
     y_pred = np.zeros_like(x)
     
     for i in range(len(model)):
         y_pred += model[i] * x ** (i+1)
     
     return y_pred
 
-# example usage
-x = np.array([1, 2, 3, 4, 5])
-y = np.array([2, 4, 5, 4, 5])
-degree = 2
-
-model = polynomial_regression(x, y, degree)
-print('polynomial coefficients:', model)
-
-x_new = np.array([6])
-x_new_poly = create_polynomial_features(x_new, degree)
-y_pred = predict(x_new_poly, model)
-print('predicted value for x = {}:'.format(x_new[0]), y_pred[0])
+
+
 
 #multiple linear regression
 import numpy as np
 
 # define a function to perform multiple linear regression
 def multiple_linear_regression(x, y):
     X = np.column_stack((np.ones(len(x)), x)) # add a column of ones for the intercept term
     model = np.linalg.lstsq(X, y, rcond=None)[0]
     
     return model
 
 # define a function to make predictions using the multiple linear regression model
-def predict(x, model):
+def predict_multiple(x, model):
     X = np.column_stack((np.ones(len(x)), x))
     y_pred = np.dot(X, model)
     
     return y_pred
 
-# example usage
-X = np.random.rand(100, 3)
-# Generate random output data
-y = 3*X[:,0] + 2*X[:,1] - 5*X[:,2] + np.random.randn(100)
-
-#x1 = np.array([1, 2, 3, 4, 5])
-#x2 = np.array([2, 4, 5, 4, 5])
-#y = np.array([5, 7, 8, 8, 10])
-
-#X = np.column_stack((x1, x2))
-model = multiple_linear_regression(X, y)
-print('intercept and coefficients:', model)
-
-X_new = np.random.rand(3, 3) # new values of x1, x2, and x3
-y_pred = predict(X_new, model)
-print('predicted values:', y_pred)
+
+
+
+
```


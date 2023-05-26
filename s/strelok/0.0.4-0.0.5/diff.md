# Comparing `tmp/strelok-0.0.4.tar.gz` & `tmp/strelok-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strelok-0.0.4.tar", last modified: Fri May 26 02:06:11 2023, max compression
+gzip compressed data, was "strelok-0.0.5.tar", last modified: Fri May 26 02:25:39 2023, max compression
```

## Comparing `strelok-0.0.4.tar` & `strelok-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:06:11.233848 strelok-0.0.4/
--rw-r--r--   0 juliusriel   (501) staff       (20)    15011 2023-05-26 02:06:11.233671 strelok-0.0.4/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)    14336 2023-05-26 02:05:49.000000 strelok-0.0.4/README.rst
--rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-26 02:06:11.233894 strelok-0.0.4/setup.cfg
--rw-r--r--   0 juliusriel   (501) staff       (20)      964 2023-05-26 02:06:04.000000 strelok-0.0.4/setup.py
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:06:11.232926 strelok-0.0.4/strelok/
--rw-r--r--   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:50.000000 strelok-0.0.4/strelok/__init__.py
--rw-r--r--   0 juliusriel   (501) staff       (20)    13370 2023-05-26 02:02:51.000000 strelok-0.0.4/strelok/feat.py
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:06:11.233491 strelok-0.0.4/strelok.egg-info/
--rw-r--r--   0 juliusriel   (501) staff       (20)    15011 2023-05-26 02:06:10.000000 strelok-0.0.4/strelok.egg-info/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)      209 2023-05-26 02:06:11.000000 strelok-0.0.4/strelok.egg-info/SOURCES.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-26 02:06:11.000000 strelok-0.0.4/strelok.egg-info/dependency_links.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)       37 2023-05-26 02:06:11.000000 strelok-0.0.4/strelok.egg-info/requires.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        8 2023-05-26 02:06:11.000000 strelok-0.0.4/strelok.egg-info/top_level.txt
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.307133 strelok-0.0.5/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 02:25:39.306957 strelok-0.0.5/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)    14635 2023-05-26 02:23:48.000000 strelok-0.0.5/README.rst
+-rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-26 02:25:39.307172 strelok-0.0.5/setup.cfg
+-rw-r--r--   0 juliusriel   (501) staff       (20)      964 2023-05-26 02:24:43.000000 strelok-0.0.5/setup.py
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.306210 strelok-0.0.5/strelok/
+-rw-r--r--   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:50.000000 strelok-0.0.5/strelok/__init__.py
+-rw-r--r--   0 juliusriel   (501) staff       (20)    13597 2023-05-26 02:16:29.000000 strelok-0.0.5/strelok/feat.py
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.306779 strelok-0.0.5/strelok.egg-info/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)      209 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/SOURCES.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/dependency_links.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)       37 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/requires.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        8 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/top_level.txt
```

### Comparing `strelok-0.0.4/PKG-INFO` & `strelok-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.4
+Version: 0.0.5
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 
 .. image:: https://static.pepy.tech/badge/strelok/month
    :target: https://pepy.tech/project/strelok
 
 Overview
 ========
 
-The Strelok library is a tool for streamlining the process of feature engineering in machine learning projects. It provides a simple and intuitive way to generate new features, handle missing values, perform feature selection, and create interaction features. With Strelok, you can streamline your feature engineering process and improve the performance of your models.
+The Strelok library is a tool that offers support in the feature engineering process of machine learning projects. It aids in generating new features, dealing with missing values, creating interaction features, and executing feature selection. With Strelok, feature engineering can become a more streamlined process, contributing to shortened development times and potentially improved model performance.
 
 Installation
 ============
 
 To install Strelok, you can use `pip`:
 
 .. code-block:: bash
@@ -97,14 +97,15 @@
     - 'binning': Applies binning to the input column. Optional parameter 'num_bins' (int) can be provided to specify the number of bins. Default is 10.
     - 'standardization': Applies standardization to the input column. Optional parameters 'mean' (float) and 'std' (float) can be provided to specify the mean and standard deviation for standardization. By default, the mean and standard deviation are calculated from the input column.
     - 'rank': Computes the rank of the values in the input column.
     - 'difference': Computes the difference between the values in the input column and another feature specified by the 'other_feature' parameter.
     - 'relative_difference': Computes the relative difference between the values in the input column and a specified 'other_value'.
     - 'sin': Applies the sine transformation to the values in the input column.
     - 'cos': Applies the cosine transformation to the values in the input column.
+    - 'mod_tan': Applies the modified tangent transformation to the values in the input column. It computes the tangent of the values as the ratio of the sine to the cosine of the values, with a small constant added to the denominator to prevent division by zero.
 
 - `diff_col` (string, optional): The name of the existing column to be transformed, if not defined the column default to target_col in `Pipeline`
 - `kwargs` (dictionary, optional): Additional parameters for specific transformation types.
 
 In addition to the common inputs mentioned earlier, some mathematical transformations in the `MathematicalTransformation` class require additional parameters:
 
 - 'exponential' transformation:
```

### Comparing `strelok-0.0.4/README.rst` & `strelok-0.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 .. image:: https://static.pepy.tech/badge/strelok/month
    :target: https://pepy.tech/project/strelok
 
 Overview
 ========
 
-The Strelok library is a tool for streamlining the process of feature engineering in machine learning projects. It provides a simple and intuitive way to generate new features, handle missing values, perform feature selection, and create interaction features. With Strelok, you can streamline your feature engineering process and improve the performance of your models.
+The Strelok library is a tool that offers support in the feature engineering process of machine learning projects. It aids in generating new features, dealing with missing values, creating interaction features, and executing feature selection. With Strelok, feature engineering can become a more streamlined process, contributing to shortened development times and potentially improved model performance.
 
 Installation
 ============
 
 To install Strelok, you can use `pip`:
 
 .. code-block:: bash
@@ -82,14 +82,15 @@
     - 'binning': Applies binning to the input column. Optional parameter 'num_bins' (int) can be provided to specify the number of bins. Default is 10.
     - 'standardization': Applies standardization to the input column. Optional parameters 'mean' (float) and 'std' (float) can be provided to specify the mean and standard deviation for standardization. By default, the mean and standard deviation are calculated from the input column.
     - 'rank': Computes the rank of the values in the input column.
     - 'difference': Computes the difference between the values in the input column and another feature specified by the 'other_feature' parameter.
     - 'relative_difference': Computes the relative difference between the values in the input column and a specified 'other_value'.
     - 'sin': Applies the sine transformation to the values in the input column.
     - 'cos': Applies the cosine transformation to the values in the input column.
+    - 'mod_tan': Applies the modified tangent transformation to the values in the input column. It computes the tangent of the values as the ratio of the sine to the cosine of the values, with a small constant added to the denominator to prevent division by zero.
 
 - `diff_col` (string, optional): The name of the existing column to be transformed, if not defined the column default to target_col in `Pipeline`
 - `kwargs` (dictionary, optional): Additional parameters for specific transformation types.
 
 In addition to the common inputs mentioned earlier, some mathematical transformations in the `MathematicalTransformation` class require additional parameters:
 
 - 'exponential' transformation:
```

### Comparing `strelok-0.0.4/setup.py` & `strelok-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name="strelok",
-    version="0.0.4",
+    version="0.0.5",
     author="Julius Riel",
     author_email="julius.riel@icloud.com",
     description="Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     install_requires=['numpy', 'pandas', 'sklearn', 'scipy', 'itertools'],
     packages=find_packages(),
```

### Comparing `strelok-0.0.4/strelok/feat.py` & `strelok-0.0.5/strelok/feat.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,21 @@
             transformed_data[self.name] = (data[target_col] - other_value) / other_value
         
         elif self.transformation_type == 'cos':
             transformed_data[self.name] = np.cos(data[target_col])
 
         elif self.transformation_type == 'sin':
             transformed_data[self.name] = np.sin(data[target_col])
+        
+        elif self.transformation_type == 'mod_tan':
+            sin_ = np.sin(data[target_col])
+            cos_ = np.cos(data[target_col])
+
+            transformed_data[self.name] = sin_ / (cos_ + 1e-10)
+            
 
 
 
         return transformed_data[[self.name]]
```

### Comparing `strelok-0.0.4/strelok.egg-info/PKG-INFO` & `strelok-0.0.5/strelok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.4
+Version: 0.0.5
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 
 .. image:: https://static.pepy.tech/badge/strelok/month
    :target: https://pepy.tech/project/strelok
 
 Overview
 ========
 
-The Strelok library is a tool for streamlining the process of feature engineering in machine learning projects. It provides a simple and intuitive way to generate new features, handle missing values, perform feature selection, and create interaction features. With Strelok, you can streamline your feature engineering process and improve the performance of your models.
+The Strelok library is a tool that offers support in the feature engineering process of machine learning projects. It aids in generating new features, dealing with missing values, creating interaction features, and executing feature selection. With Strelok, feature engineering can become a more streamlined process, contributing to shortened development times and potentially improved model performance.
 
 Installation
 ============
 
 To install Strelok, you can use `pip`:
 
 .. code-block:: bash
@@ -97,14 +97,15 @@
     - 'binning': Applies binning to the input column. Optional parameter 'num_bins' (int) can be provided to specify the number of bins. Default is 10.
     - 'standardization': Applies standardization to the input column. Optional parameters 'mean' (float) and 'std' (float) can be provided to specify the mean and standard deviation for standardization. By default, the mean and standard deviation are calculated from the input column.
     - 'rank': Computes the rank of the values in the input column.
     - 'difference': Computes the difference between the values in the input column and another feature specified by the 'other_feature' parameter.
     - 'relative_difference': Computes the relative difference between the values in the input column and a specified 'other_value'.
     - 'sin': Applies the sine transformation to the values in the input column.
     - 'cos': Applies the cosine transformation to the values in the input column.
+    - 'mod_tan': Applies the modified tangent transformation to the values in the input column. It computes the tangent of the values as the ratio of the sine to the cosine of the values, with a small constant added to the denominator to prevent division by zero.
 
 - `diff_col` (string, optional): The name of the existing column to be transformed, if not defined the column default to target_col in `Pipeline`
 - `kwargs` (dictionary, optional): Additional parameters for specific transformation types.
 
 In addition to the common inputs mentioned earlier, some mathematical transformations in the `MathematicalTransformation` class require additional parameters:
 
 - 'exponential' transformation:
```


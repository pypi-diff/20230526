# Comparing `tmp/deformation-inversion-layer-1.0.0.tar.gz` & `tmp/deformation-inversion-layer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deformation-inversion-layer-1.0.0.tar", last modified: Fri May 26 12:58:57 2023, max compression
+gzip compressed data, was "deformation-inversion-layer-1.0.1.tar", last modified: Fri May 26 13:29:27 2023, max compression
```

## Comparing `deformation-inversion-layer-1.0.0.tar` & `deformation-inversion-layer-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1070 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/LICENSE
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     3057 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/PKG-INFO
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1551 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/README.md
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1163 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/description.md
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      766 2023-05-26 12:58:01.000000 deformation-inversion-layer-1.0.0/pyproject.toml
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       38 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/setup.cfg
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       37 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/setup.py
-drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/src/
-drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      868 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/__init__.py
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     8280 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/fixed_point_invert_deformation.py
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)    10413 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/fixed_point_iteration.py
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     2415 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interface.py
-drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       67 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/__init__.py
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     5473 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/algorithm.py
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      981 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/wrapper.py
-drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 12:58:57.887338 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     3057 2023-05-26 12:58:57.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/PKG-INFO
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      713 2023-05-26 12:58:57.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/SOURCES.txt
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)        1 2023-05-26 12:58:57.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/dependency_links.txt
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       12 2023-05-26 12:58:57.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/requires.txt
--rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       28 2023-05-26 12:58:57.000000 deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/top_level.txt
+drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1070 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/LICENSE
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     2916 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/PKG-INFO
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1410 2023-05-26 13:25:07.000000 deformation-inversion-layer-1.0.1/README.md
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     1022 2023-05-26 13:25:26.000000 deformation-inversion-layer-1.0.1/description.md
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      766 2023-05-26 13:25:30.000000 deformation-inversion-layer-1.0.1/pyproject.toml
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       38 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/setup.cfg
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       37 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/setup.py
+drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 13:29:27.831909 deformation-inversion-layer-1.0.1/src/
+drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      868 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/__init__.py
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     8280 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/fixed_point_invert_deformation.py
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)    10413 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/fixed_point_iteration.py
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     2415 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interface.py
+drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       67 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/__init__.py
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     5473 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/algorithm.py
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      981 2023-05-26 12:57:08.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/wrapper.py
+drwxrwxr-x   0 honkamj2  (1009) honkamj2  (1010)        0 2023-05-26 13:29:27.835909 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)     2916 2023-05-26 13:29:27.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/PKG-INFO
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)      713 2023-05-26 13:29:27.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/SOURCES.txt
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)        1 2023-05-26 13:29:27.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/dependency_links.txt
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       12 2023-05-26 13:29:27.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/requires.txt
+-rw-rw-r--   0 honkamj2  (1009) honkamj2  (1010)       28 2023-05-26 13:29:27.000000 deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/top_level.txt
```

### Comparing `deformation-inversion-layer-1.0.0/LICENSE` & `deformation-inversion-layer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/PKG-INFO` & `deformation-inversion-layer-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deformation-inversion-layer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deformation inversion layer is a neural network layer for inverting deformation fields
 Author: Joel Honkamaa
 License: MIT License
         
         Copyright (c) 2023 Joel Honkamaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,12 +59,12 @@
 
 ## Publication
 
 If you use deformation inversion layer, please cite the SITReg paper. Details for citing can be found at the GitHub repository.
 
 ## Acknowledgments
 
-Small parts of the repository are rewritten from [NITorch](https://github.com/balbasty/nitorch), [VoxelMorph](https://github.com/voxelmorph/voxelmorph), [TorchIR](https://github.com/BDdeVos/TorchIR), [DeepReg](https://github.com/DeepRegNet/DeepReg), and [SciPy](https://scipy.org/).
+[Tutorial](http://implicit-layers-tutorial.org/) by Zico Kolter, David Duvenaud, and Matt Johnson was very helpful in implementing the layer.
 
 ## License
 
 Deformation inversion layer is released under the MIT license.
```

### Comparing `deformation-inversion-layer-1.0.0/README.md` & `deformation-inversion-layer-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 
 - **SITReg: Multi-resolution architecture for symmetric, inverse consistent, and topology preserving image registration using deformation inversion layers**  
 [Joel Honkamaa](https://github.com/honkamj), Pekka Marttinen  
 Under review ([eprint arXiv:2303.10211](https://arxiv.org/abs/2303.10211))
 
 ## Acknowledgments
 
-Small parts of the repository are rewritten from [NITorch](https://github.com/balbasty/nitorch), [VoxelMorph](https://github.com/voxelmorph/voxelmorph), [TorchIR](https://github.com/BDdeVos/TorchIR), [DeepReg](https://github.com/DeepRegNet/DeepReg), and [SciPy](https://scipy.org/).
+[Tutorial](http://implicit-layers-tutorial.org/) by Zico Kolter, David Duvenaud, and Matt Johnson was very helpful in implementing the layer.
 
 ## License
 
 Deformation inversion layer and SITReg are released under the MIT license.
```

### Comparing `deformation-inversion-layer-1.0.0/description.md` & `deformation-inversion-layer-1.0.1/description.md`

 * *Files 23% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
 ## Publication
 
 If you use deformation inversion layer, please cite the SITReg paper. Details for citing can be found at the GitHub repository.
 
 ## Acknowledgments
 
-Small parts of the repository are rewritten from [NITorch](https://github.com/balbasty/nitorch), [VoxelMorph](https://github.com/voxelmorph/voxelmorph), [TorchIR](https://github.com/BDdeVos/TorchIR), [DeepReg](https://github.com/DeepRegNet/DeepReg), and [SciPy](https://scipy.org/).
+[Tutorial](http://implicit-layers-tutorial.org/) by Zico Kolter, David Duvenaud, and Matt Johnson was very helpful in implementing the layer.
 
 ## License
 
 Deformation inversion layer is released under the MIT license.
```

### Comparing `deformation-inversion-layer-1.0.0/pyproject.toml` & `deformation-inversion-layer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deformation-inversion-layer"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Joel Honkamaa" },
 ]
 description = "Deformation inversion layer is a neural network layer for inverting deformation fields"
 readme = "description.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/__init__.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/fixed_point_invert_deformation.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/fixed_point_invert_deformation.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/fixed_point_iteration.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/fixed_point_iteration.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interface.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interface.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/algorithm.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/algorithm.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer/interpolator/wrapper.py` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer/interpolator/wrapper.py`

 * *Files identical despite different names*

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/PKG-INFO` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deformation-inversion-layer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deformation inversion layer is a neural network layer for inverting deformation fields
 Author: Joel Honkamaa
 License: MIT License
         
         Copyright (c) 2023 Joel Honkamaa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,12 +59,12 @@
 
 ## Publication
 
 If you use deformation inversion layer, please cite the SITReg paper. Details for citing can be found at the GitHub repository.
 
 ## Acknowledgments
 
-Small parts of the repository are rewritten from [NITorch](https://github.com/balbasty/nitorch), [VoxelMorph](https://github.com/voxelmorph/voxelmorph), [TorchIR](https://github.com/BDdeVos/TorchIR), [DeepReg](https://github.com/DeepRegNet/DeepReg), and [SciPy](https://scipy.org/).
+[Tutorial](http://implicit-layers-tutorial.org/) by Zico Kolter, David Duvenaud, and Matt Johnson was very helpful in implementing the layer.
 
 ## License
 
 Deformation inversion layer is released under the MIT license.
```

### Comparing `deformation-inversion-layer-1.0.0/src/deformation_inversion_layer.egg-info/SOURCES.txt` & `deformation-inversion-layer-1.0.1/src/deformation_inversion_layer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


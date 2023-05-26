# Comparing `tmp/BaseNN-0.1.4.tar.gz` & `tmp/BaseNN-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.4.tar", last modified: Thu May 25 09:12:34 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.5.tar", last modified: Fri May 26 06:31:28 2023, max compression
```

## Comparing `BaseNN-0.1.4.tar` & `BaseNN-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 09:12:34.000000 BaseNN-0.1.4/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    38766 2023-05-25 09:07:04.000000 BaseNN-0.1.4/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.4/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22843 2023-05-25 09:05:57.000000 BaseNN-0.1.4/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.4/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.4/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.4/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-25 09:12:10.000000 BaseNN-0.1.4/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-25 09:12:34.000000 BaseNN-0.1.4/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.4/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-25 09:12:34.000000 BaseNN-0.1.4/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-25 09:12:34.000000 BaseNN-0.1.4/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-25 09:12:06.000000 BaseNN-0.1.4/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    38762 2023-05-26 06:29:57.000000 BaseNN-0.1.5/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.5/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    22843 2023-05-25 09:05:57.000000 BaseNN-0.1.5/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.5/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.5/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.5/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-26 06:30:24.000000 BaseNN-0.1.5/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-26 06:31:28.000000 BaseNN-0.1.5/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.5/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-26 06:31:28.000000 BaseNN-0.1.5/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-26 06:31:28.000000 BaseNN-0.1.5/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-26 06:30:17.000000 BaseNN-0.1.5/setup.py
```

### Comparing `BaseNN-0.1.4/BaseNN/BaseNN.py` & `BaseNN-0.1.5/BaseNN/BaseNN.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
             self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
             self.label = torch.Tensor()
             for train_x, train_y in self.dataloader:
                 # test_x = test_x.to(self.device)
                 # test_y = test_y.to(self.device)
                 # batch_res = self.model(test_x)
                 self.label = torch.cat([self.label, train_y], dim=0)
-                self.label = self.label.cpu().detach().numpy()
+            self.label = self.label.cpu().detach().numpy()
             return self.dataloader
 
     def load_tab_data(self, data_path,batch_size=32, train_val_ratio=1.0, shuffle=True):
         from .load_data import TabularDataset
         dataset = TabularDataset(data_path)
         self.dataset_size = int(len(dataset))
         # print(self.dataset_size)
```

### Comparing `BaseNN-0.1.4/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.5/BaseNN/examples/BaseNN_demo.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.4/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.5/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.4/BaseNN/load_data.py` & `BaseNN-0.1.5/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.4/BaseNN/version.py` & `BaseNN-0.1.5/BaseNN/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.4'
+__version__='0.1.5'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.4/setup.py` & `BaseNN-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.4',
+    version='0.1.5',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```


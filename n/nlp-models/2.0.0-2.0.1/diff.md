# Comparing `tmp/nlp-models-2.0.0.tar.gz` & `tmp/nlp-models-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.0.0.tar", last modified: Thu May 25 17:21:22 2023, max compression
+gzip compressed data, was "nlp-models-2.0.1.tar", last modified: Fri May 26 14:52:52 2023, max compression
```

## Comparing `nlp-models-2.0.0.tar` & `nlp-models-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:22.237032 nlp-models-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 17:21:11.000000 nlp-models-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 17:21:22.237032 nlp-models-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 17:21:11.000000 nlp-models-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-25 17:21:11.000000 nlp-models-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 17:21:22.237032 nlp-models-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 17:21:11.000000 nlp-models-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:22.233032 nlp-models-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:22.237032 nlp-models-2.0.0/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:22.237032 nlp-models-2.0.0/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 17:21:11.000000 nlp-models-2.0.0/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:21:22.237032 nlp-models-2.0.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-25 17:21:22.000000 nlp-models-2.0.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 17:21:22.000000 nlp-models-2.0.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:21:22.000000 nlp-models-2.0.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 17:21:22.000000 nlp-models-2.0.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 17:21:22.000000 nlp-models-2.0.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 14:52:40.000000 nlp-models-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-26 14:52:52.185801 nlp-models-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 14:52:40.000000 nlp-models-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 14:52:40.000000 nlp-models-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-26 14:52:52.185801 nlp-models-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 14:52:40.000000 nlp-models-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.181801 nlp-models-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-26 14:52:40.000000 nlp-models-2.0.1/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:52:52.185801 nlp-models-2.0.1/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 14:52:52.000000 nlp-models-2.0.1/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.0.0/LICENSE` & `nlp-models-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/PKG-INFO` & `nlp-models-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.0.0
+Version: 2.0.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.0.0/README.md` & `nlp-models-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/setup.cfg` & `nlp-models-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.0.0
+version = 2.0.1
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.0.0/src/bert_classifier/bert.py` & `nlp-models-2.0.1/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/bert_classifier/data.py` & `nlp-models-2.0.1/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/bert_classifier/io.py` & `nlp-models-2.0.1/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/bert_classifier/metrics.py` & `nlp-models-2.0.1/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/bert_classifier/predict.py` & `nlp-models-2.0.1/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/bert_classifier/train.py` & `nlp-models-2.0.1/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/multi_task_model/layers.py` & `nlp-models-2.0.1/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/multi_task_model/metrics.py` & `nlp-models-2.0.1/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/multi_task_model/mtl.py` & `nlp-models-2.0.1/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/multi_task_model/trainer.py` & `nlp-models-2.0.1/src/multi_task_model/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,22 +50,21 @@
             for param in self.model.base_model.parameters():
                 param.requires_grad = False
 
         self.optimizer = self.get_optimizer(
             list(self.model.named_parameters()), 
             self.configs.optimizer_class, 
             self.configs.optimizer_params, 
-            self.configs.weight_decay
-            )
+            self.configs.weight_decay)
+        
         self.scheduler = self.get_scheduler(
             self.optimizer, 
             self.configs.scheduler, 
             self.configs.warmup_steps, 
-            len(self.train_dataloader)*self.configs.epochs
-            )
+            len(self.train_dataloader)*self.configs.epochs)
 
     def logger(self, epoch, metrics, loss, mode):
         log = {
             f'epoch_{epoch-1}': {
                 'loss': loss,
                 'accuracy': metrics
             }
@@ -100,14 +99,19 @@
             'val_acc': self.val_logs[epoch][f'epoch_{epoch}']['accuracy'],
         }, chkpt_path)
 
     def load_checkpoint(self, chkpt_dir):
         chkpt = torch.load(chkpt_dir)
         self.model.load_state_dict(chkpt['model_state_dict'])
         self.optimizer.load_state_dict(chkpt['optimizer_state_dict'])
+        self.scheduler = self.get_scheduler(
+            self.optimizer, 
+            self.configs.scheduler, 
+            0, 
+            len(self.train_dataloader)*self.configs.epochs)
 
     def clear(self):
         gc.collect()
         torch.cuda.empty_cache()
     
     def fit(self):
         epochs = tqdm(range(1, self.configs.epochs+1), leave = True, desc="Training...")
```

### Comparing `nlp-models-2.0.0/src/multi_task_model/utils.py` & `nlp-models-2.0.1/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.0.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-2.0.1/src/nlp_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.0.0
+Version: 2.0.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.0.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.0.1/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/edu_segmentation-0.0.75.tar.gz` & `tmp/edu_segmentation-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.75.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.76.tar", max compression
```

## Comparing `edu_segmentation-0.0.75.tar` & `edu_segmentation-0.0.76.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.75/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
--rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
--rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/model.py
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-r--r--   0        0        0     7541 2023-05-26 08:49:52.210965 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/solver.py
--rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/solver_bart.py
--rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     8950 2023-05-26 08:29:52.430340 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     7031 2023-05-26 08:19:36.793780 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.75/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.75/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0     1867 2023-05-26 08:32:06.723542 edu_segmentation-0.0.75/edu_segmentation/main.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.75/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.75/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.75/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.75/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0      589 2023-05-26 08:50:12.601075 edu_segmentation-0.0.75/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.75/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.75/PKG-INFO
+-rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.76/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
+-rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
+-rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/model.py
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/model_bart_v2.py
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-r--r--   0        0        0     7541 2023-05-26 08:49:52.210965 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/solver_bart.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/train_segbot_bart.py
+-rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8950 2023-05-26 08:29:52.430340 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     7031 2023-05-26 08:19:36.793780 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.76/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.76/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0     1867 2023-05-26 08:32:06.723542 edu_segmentation-0.0.76/edu_segmentation/main.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.76/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.76/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0      589 2023-05-26 08:54:57.896908 edu_segmentation-0.0.76/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.76/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.76/PKG-INFO
```

### Comparing `edu_segmentation-0.0.75/edu_segmentation/__init__.py` & `edu_segmentation-0.0.76/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/model.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/solver.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.76/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.76/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/main.py` & `edu_segmentation-0.0.76/edu_segmentation/main.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.76/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.76/edu_segmentation/BARTTokenClassification/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.76/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/pyproject.toml` & `edu_segmentation-0.0.76/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.75"
+version = "v0.0.76"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.75/readme.md` & `edu_segmentation-0.0.76/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.75/PKG-INFO` & `edu_segmentation-0.0.76/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.75
+Version: 0.0.76
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```


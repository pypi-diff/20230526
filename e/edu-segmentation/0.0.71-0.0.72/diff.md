# Comparing `tmp/edu_segmentation-0.0.71.tar.gz` & `tmp/edu_segmentation-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.71.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.72.tar", max compression
```

## Comparing `edu_segmentation-0.0.71.tar` & `edu_segmentation-0.0.72.tar`

### file list

```diff
@@ -1,33 +1,38 @@
--rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.71/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/model.py
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-r--r--   0        0        0     7483 2023-05-26 07:56:01.905628 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/solver.py
--rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/solver_bart.py
--rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4321 2023-04-27 10:53:25.927765 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4882 2023-04-27 10:53:25.959014 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3312 2023-04-27 10:53:25.990406 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3226 2023-04-27 10:53:26.030012 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     7030 2023-05-26 07:56:06.614724 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-r--r--   0        0        0     6409 2023-04-27 10:53:26.103614 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6978 2023-04-27 10:53:26.134865 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1023 2023-04-27 10:53:26.197363 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1313 2023-04-27 10:53:26.228615 edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.71/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.71/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0     1865 2023-05-26 07:59:57.504246 edu_segmentation-0.0.71/edu_segmentation/main.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.71/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.71/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.71/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.71/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0      589 2023-05-26 08:09:45.007737 edu_segmentation-0.0.71/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.71/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.71/PKG-INFO
+-rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.72/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
+-rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
+-rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/model.py
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-r--r--   0        0        0     7483 2023-05-26 07:56:01.905628 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver_bart.py
+-rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8945 2023-05-26 08:17:50.845444 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     7031 2023-05-26 08:19:36.793780 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.72/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.72/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0     1865 2023-05-26 07:59:57.504246 edu_segmentation-0.0.72/edu_segmentation/main.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.72/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0      589 2023-05-26 08:21:31.350945 edu_segmentation-0.0.72/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.72/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.72/PKG-INFO
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/__init__.py` & `edu_segmentation-0.0.72/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/model.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/solver.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import List
 import numpy as np
 
-from config import PATH, SAMPLE_NUM, TOKENIZER
+from .config import PATH, SAMPLE_NUM, TOKENIZER
 
 
 def get_average_max_edu_len():
     all_files = os.listdir(PATH)
     total_edu_len = 0
     edu_num = 0
     max_edu_len = 0
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import spacy
-from config import PATH, SAMPLE_NUM,TOKENIZER
+from .config import PATH, SAMPLE_NUM,TOKENIZER
 from typing import List
 import os
 import numpy as np
 
 
 # TODO: postag2id dict as global var, currently wrgggg and skip all the wrgly mapped edus
 nlp = spacy.load('en_core_web_sm')
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import spacy
-from config import TOKENIZER
+from .config import TOKENIZER
 from typing import List
 
 
 nlp = spacy.load('en_core_web_sm')
 sentence = "Energetic and concrete action has been taken in Colombia during the past 60 days against the mafiosi of the drug trade , "
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #TODO: use 2 pointer method and parse through all bert tokens and postags words and tokens and fix logic
 import spacy
-from config import TOKENIZER
+from .config import TOKENIZER
 from typing import List
 
 
 nlp = spacy.load('en_core_web_sm')
 sentence = "when the price rose $ 2 a share to $ 78.50 . Between then and his bid on Oct. 5 , the price fluctuated between $ 75.625 and $ 87.375 ."
 
 '''
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 warnings.filterwarnings('ignore')
 
 import os
 import torch
 import transformers
 import numpy as np
 
-from config import TOKENIZER
+from .config import TOKENIZER
 
 
 def bert_tokenizer(text: str) -> List[int]:
     '''
     :param text:
     :return:
     Add special tokens to the start and end of each sentence
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 import torch.nn as nn
 import transformers
 from tqdm import tqdm
 from sklearn.metrics import f1_score, precision_score, recall_score
 
-from config import DEVICE, SAVE_PATH
+from .config import DEVICE, SAVE_PATH
 import os
 
 def train_fn(x, x_mask, y, model, optimizer):
     '''
     Function to train the model
     '''
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 import torch.nn as nn
 import transformers
 from tqdm import tqdm
 from sklearn.metrics import f1_score, precision_score, recall_score
 
-from config import DEVICE, SAVE_PATH
+from .config import DEVICE, SAVE_PATH
 import os
 
 def train_fn(x, x_mask, x_postag_ids, y, model, optimizer):
     '''
     Function to train the model
     '''
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from import_data_bert import read_data
-from solver import train_engine
+from .import_data_bert import read_data
+from .solver import train_engine
 
 all_tokens, all_masks, all_boundaries = read_data()
 print("len all tokens:", len(all_tokens))
 idx = int(len(all_tokens)*0.8)
 train_x = all_tokens[:idx]
 train_x_mask = all_masks[:idx]
 train_y = all_boundaries[:idx]
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from import_data_bert_postag import read_data
-from solver_postag import train_engine
+from .import_data_bert_postag import read_data
+from .solver_postag import train_engine
 
 all_tokens, all_masks, all_postags, all_boundaries = read_data()
 print("len all tokens:", len(all_tokens))
 idx = int(len(all_tokens)*0.8)
 train_x = all_tokens[:idx]
 train_x_mask = all_masks[:idx]
 train_x_postag_ids = all_postags[:idx]
```

### Comparing `edu_segmentation-0.0.71/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.72/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/main.py` & `edu_segmentation-0.0.72/edu_segmentation/main.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.72/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/pyproject.toml` & `edu_segmentation-0.0.72/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.71"
+version = "v0.0.72"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.71/readme.md` & `edu_segmentation-0.0.72/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.71/PKG-INFO` & `edu_segmentation-0.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.71
+Version: 0.0.72
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```


# Comparing `tmp/fastcoref-2.1.5.tar.gz` & `tmp/fastcoref-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcoref-2.1.5.tar", last modified: Tue May  9 16:58:08 2023, max compression
+gzip compressed data, was "fastcoref-2.1.6.tar", last modified: Fri May 26 14:43:49 2023, max compression
```

## Comparing `fastcoref-2.1.5.tar` & `fastcoref-2.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.441208 fastcoref-2.1.5/
--rw-r--r--   0 shono    (847860209) 305066103     1070 2023-04-16 21:51:10.000000 fastcoref-2.1.5/LICENSE
--rw-r--r--   0 shono    (847860209) 305066103     6754 2023-05-09 16:58:08.441059 fastcoref-2.1.5/PKG-INFO
--rw-r--r--   0 shono    (847860209) 305066103     6467 2023-04-16 21:51:10.000000 fastcoref-2.1.5/README.md
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.438076 fastcoref-2.1.5/fastcoref/
--rw-r--r--   0 shono    (847860209) 305066103      104 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/__init__.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.439500 fastcoref-2.1.5/fastcoref/coref_models/
--rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/__init__.py
--rwxr-xr-x   0 shono    (847860209) 305066103    14767 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/modeling_fcoref.py
--rwxr-xr-x   0 shono    (847860209) 305066103    19662 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/coref_models/modeling_lingmess.py
--rw-r--r--   0 shono    (847860209) 305066103    11812 2023-05-09 16:56:18.000000 fastcoref-2.1.5/fastcoref/modeling.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.439866 fastcoref-2.1.5/fastcoref/spacy_component/
--rw-r--r--   0 shono    (847860209) 305066103       46 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/spacy_component/__init__.py
--rw-r--r--   0 shono    (847860209) 305066103     7554 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/spacy_component/spacy_component.py
--rw-r--r--   0 shono    (847860209) 305066103    12762 2023-05-09 11:22:56.000000 fastcoref-2.1.5/fastcoref/trainer.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.440813 fastcoref-2.1.5/fastcoref/utilities/
--rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/__init__.py
--rwxr-xr-x   0 shono    (847860209) 305066103     4548 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/collate.py
--rw-r--r--   0 shono    (847860209) 305066103      984 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/consts.py
--rw-r--r--   0 shono    (847860209) 305066103     6185 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/coref_dataset.py
--rwxr-xr-x   0 shono    (847860209) 305066103     5003 2023-04-16 21:51:10.000000 fastcoref-2.1.5/fastcoref/utilities/metrics.py
--rw-r--r--   0 shono    (847860209) 305066103     9445 2023-05-09 16:56:18.000000 fastcoref-2.1.5/fastcoref/utilities/util.py
-drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-09 16:58:08.438865 fastcoref-2.1.5/fastcoref.egg-info/
--rw-r--r--   0 shono    (847860209) 305066103     6754 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/PKG-INFO
--rw-r--r--   0 shono    (847860209) 305066103      648 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/SOURCES.txt
--rw-r--r--   0 shono    (847860209) 305066103        1 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/dependency_links.txt
--rw-r--r--   0 shono    (847860209) 305066103      127 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/requires.txt
--rw-r--r--   0 shono    (847860209) 305066103       10 2023-05-09 16:58:08.000000 fastcoref-2.1.5/fastcoref.egg-info/top_level.txt
--rw-r--r--   0 shono    (847860209) 305066103       38 2023-05-09 16:58:08.441255 fastcoref-2.1.5/setup.cfg
--rw-r--r--   0 shono    (847860209) 305066103      991 2023-05-09 16:57:35.000000 fastcoref-2.1.5/setup.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.380323 fastcoref-2.1.6/
+-rw-r--r--   0 shono    (847860209) 305066103     1070 2023-04-16 21:51:10.000000 fastcoref-2.1.6/LICENSE
+-rw-r--r--   0 shono    (847860209) 305066103     6811 2023-05-26 14:43:49.380127 fastcoref-2.1.6/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103     6524 2023-05-26 14:41:38.000000 fastcoref-2.1.6/README.md
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.376768 fastcoref-2.1.6/fastcoref/
+-rw-r--r--   0 shono    (847860209) 305066103      104 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/__init__.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.378044 fastcoref-2.1.6/fastcoref/coref_models/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/coref_models/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    14767 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/coref_models/modeling_fcoref.py
+-rwxr-xr-x   0 shono    (847860209) 305066103    19662 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/coref_models/modeling_lingmess.py
+-rw-r--r--   0 shono    (847860209) 305066103    11812 2023-05-09 16:56:18.000000 fastcoref-2.1.6/fastcoref/modeling.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.378431 fastcoref-2.1.6/fastcoref/spacy_component/
+-rw-r--r--   0 shono    (847860209) 305066103       46 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/spacy_component/__init__.py
+-rw-r--r--   0 shono    (847860209) 305066103     7554 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/spacy_component/spacy_component.py
+-rw-r--r--   0 shono    (847860209) 305066103    12877 2023-05-26 14:41:38.000000 fastcoref-2.1.6/fastcoref/trainer.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.379629 fastcoref-2.1.6/fastcoref/utilities/
+-rw-r--r--   0 shono    (847860209) 305066103        0 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/utilities/__init__.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     4548 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/utilities/collate.py
+-rw-r--r--   0 shono    (847860209) 305066103      984 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/utilities/consts.py
+-rw-r--r--   0 shono    (847860209) 305066103     6185 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/utilities/coref_dataset.py
+-rwxr-xr-x   0 shono    (847860209) 305066103     5003 2023-04-16 21:51:10.000000 fastcoref-2.1.6/fastcoref/utilities/metrics.py
+-rw-r--r--   0 shono    (847860209) 305066103     9445 2023-05-09 16:56:18.000000 fastcoref-2.1.6/fastcoref/utilities/util.py
+drwxr-xr-x   0 shono    (847860209) 305066103        0 2023-05-26 14:43:49.377599 fastcoref-2.1.6/fastcoref.egg-info/
+-rw-r--r--   0 shono    (847860209) 305066103     6811 2023-05-26 14:43:49.000000 fastcoref-2.1.6/fastcoref.egg-info/PKG-INFO
+-rw-r--r--   0 shono    (847860209) 305066103      648 2023-05-26 14:43:49.000000 fastcoref-2.1.6/fastcoref.egg-info/SOURCES.txt
+-rw-r--r--   0 shono    (847860209) 305066103        1 2023-05-26 14:43:49.000000 fastcoref-2.1.6/fastcoref.egg-info/dependency_links.txt
+-rw-r--r--   0 shono    (847860209) 305066103      127 2023-05-26 14:43:49.000000 fastcoref-2.1.6/fastcoref.egg-info/requires.txt
+-rw-r--r--   0 shono    (847860209) 305066103       10 2023-05-26 14:43:49.000000 fastcoref-2.1.6/fastcoref.egg-info/top_level.txt
+-rw-r--r--   0 shono    (847860209) 305066103       38 2023-05-26 14:43:49.380380 fastcoref-2.1.6/setup.cfg
+-rw-r--r--   0 shono    (847860209) 305066103      991 2023-05-26 14:41:52.000000 fastcoref-2.1.6/setup.py
```

### Comparing `fastcoref-2.1.5/LICENSE` & `fastcoref-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/PKG-INFO` & `fastcoref-2.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcoref
-Version: 2.1.5
+Version: 2.1.6
 Home-page: https://github.com/shon-otmazgin/fastcoref
 Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
 Author-email: shon711@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
@@ -182,15 +182,16 @@
     eval_steps=100
 )   # you can control other arguments such as learning head and others.
 
 trainer = CorefTrainer(
     args=args,
     train_file='train_file_with_clusters.jsonlines', 
     dev_file='path-to-dev-file',    # optional
-    test_file='path-to-test-file'   # optional
+    test_file='path-to-test-file',   # optional
+    nlp=nlp # optional, for custom nlp class from spacy
 )
 trainer.train()
 trainer.evaluate(test=True)
 
 trainer.push_to_hub('your-fast-coref-model-path')
 
 ```
```

### Comparing `fastcoref-2.1.5/README.md` & `fastcoref-2.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -171,15 +171,16 @@
     eval_steps=100
 )   # you can control other arguments such as learning head and others.
 
 trainer = CorefTrainer(
     args=args,
     train_file='train_file_with_clusters.jsonlines', 
     dev_file='path-to-dev-file',    # optional
-    test_file='path-to-test-file'   # optional
+    test_file='path-to-test-file',   # optional
+    nlp=nlp # optional, for custom nlp class from spacy
 )
 trainer.train()
 trainer.evaluate(test=True)
 
 trainer.push_to_hub('your-fast-coref-model-path')
 
 ```
```

### Comparing `fastcoref-2.1.5/fastcoref/coref_models/modeling_fcoref.py` & `fastcoref-2.1.6/fastcoref/coref_models/modeling_fcoref.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/coref_models/modeling_lingmess.py` & `fastcoref-2.1.6/fastcoref/coref_models/modeling_lingmess.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/modeling.py` & `fastcoref-2.1.6/fastcoref/modeling.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/spacy_component/spacy_component.py` & `fastcoref-2.1.6/fastcoref/spacy_component/spacy_component.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/trainer.py` & `fastcoref-2.1.6/fastcoref/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import logging
 import numpy as np
 import torch
 import spacy
+from spacy.language import Language
+from spacy.cli import download
 from dataclasses import dataclass
 
 from torch.optim.adamw import AdamW
 from tqdm.auto import tqdm
 
 import transformers
 from transformers import AutoConfig, AutoTokenizer, get_linear_schedule_with_warmup
@@ -80,26 +82,26 @@
     if model.base_model_prefix not in SUPPORTED_MODELS:
         raise NotImplementedError(f'Not supporting {model.base_model_prefix}, choose one of {SUPPORTED_MODELS}')
 
     return model, tokenizer
 
 
 class CorefTrainer:
-    def __init__(self, args: TrainingArgs, train_file, dev_file=None, test_file=None):
+    def __init__(self, args: TrainingArgs, train_file, dev_file=None, test_file=None, nlp=None):
         import wandb
 
         transformers.logging.set_verbosity_error()
         self.args = args
         wandb.init(project=self.args.output_dir, config=self.args)
         self.wandb_logger = wandb.log
         self.wandb_runner = wandb.run
 
         self._set_device()
+        self.nlp = nlp if isinstance(nlp, Language) else spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
 
-        self.nlp = spacy.load("en_core_web_sm", exclude=["tagger", "parser", "lemmatizer", "ner", "textcat"])
         self.model, self.tokenizer = _load_f_coref_model(self.args)
         self.model.to(self.device)
 
         self.collator = LeftOversCollator(
             tokenizer=self.tokenizer,
             device=self.device,
             max_segment_len=self.args.max_segment_len
```

### Comparing `fastcoref-2.1.5/fastcoref/utilities/collate.py` & `fastcoref-2.1.6/fastcoref/utilities/collate.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/utilities/consts.py` & `fastcoref-2.1.6/fastcoref/utilities/consts.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/utilities/coref_dataset.py` & `fastcoref-2.1.6/fastcoref/utilities/coref_dataset.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/utilities/metrics.py` & `fastcoref-2.1.6/fastcoref/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref/utilities/util.py` & `fastcoref-2.1.6/fastcoref/utilities/util.py`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/fastcoref.egg-info/PKG-INFO` & `fastcoref-2.1.6/fastcoref.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastcoref
-Version: 2.1.5
+Version: 2.1.6
 Home-page: https://github.com/shon-otmazgin/fastcoref
 Author: Shon Otmazgin, Arie Cattan, Yoav Goldberg
 Author-email: shon711@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: train
 License-File: LICENSE
@@ -182,15 +182,16 @@
     eval_steps=100
 )   # you can control other arguments such as learning head and others.
 
 trainer = CorefTrainer(
     args=args,
     train_file='train_file_with_clusters.jsonlines', 
     dev_file='path-to-dev-file',    # optional
-    test_file='path-to-test-file'   # optional
+    test_file='path-to-test-file',   # optional
+    nlp=nlp # optional, for custom nlp class from spacy
 )
 trainer.train()
 trainer.evaluate(test=True)
 
 trainer.push_to_hub('your-fast-coref-model-path')
 
 ```
```

### Comparing `fastcoref-2.1.5/fastcoref.egg-info/SOURCES.txt` & `fastcoref-2.1.6/fastcoref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastcoref-2.1.5/setup.py` & `fastcoref-2.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='fastcoref',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.1.5',
+    version='2.1.6',
     license='MIT',
     author="Shon Otmazgin, Arie Cattan, Yoav Goldberg",
     author_email='shon711@gmail.com',
     packages=['fastcoref', 'fastcoref.coref_models', 'fastcoref.utilities', 'fastcoref.spacy_component'],
     url='https://github.com/shon-otmazgin/fastcoref',
     install_requires=[
         'tqdm>=4.64.0',
```


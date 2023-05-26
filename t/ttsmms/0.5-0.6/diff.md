# Comparing `tmp/ttsmms-0.5.tar.gz` & `tmp/ttsmms-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttsmms-0.5.tar", last modified: Thu May 25 06:51:15 2023, max compression
+gzip compressed data, was "ttsmms-0.6.tar", last modified: Fri May 26 07:30:44 2023, max compression
```

## Comparing `ttsmms-0.5.tar` & `ttsmms-0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:51:15.404372 ttsmms-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 06:50:59.000000 ttsmms-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 06:51:15.400372 ttsmms-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-25 06:50:59.000000 ttsmms-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 06:51:15.404372 ttsmms-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-25 06:50:59.000000 ttsmms-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:51:15.400372 ttsmms-0.5/ttsmms/
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/attentions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/mel_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:51:15.400372 ttsmms-0.5/ttsmms/text/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/text/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-25 06:50:59.000000 ttsmms-0.5/ttsmms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:51:15.400372 ttsmms-0.5/ttsmms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 06:51:15.000000 ttsmms-0.5/ttsmms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 07:30:31.000000 ttsmms-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 07:30:44.738598 ttsmms-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 07:30:31.000000 ttsmms-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:30:44.738598 ttsmms-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 07:30:31.000000 ttsmms-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/mel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms/text/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/text/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-26 07:30:31.000000 ttsmms-0.6/ttsmms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:30:44.738598 ttsmms-0.6/ttsmms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 07:30:44.000000 ttsmms-0.6/ttsmms.egg-info/top_level.txt
```

### Comparing `ttsmms-0.5/LICENSE` & `ttsmms-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/PKG-INFO` & `ttsmms-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.5
+Version: 0.6
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
```

### Comparing `ttsmms-0.5/README.md` & `ttsmms-0.6/README.md`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/setup.py` & `ttsmms-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "torchvision",
     "Unidecode",
     "monotonic-align"
 ]
 
 setup(
     name="ttsmms",
-    version="0.5",
+    version="0.6",
     description="Text-to-speech with The Massively Multilingual Speech (MMS) project",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/ttsmms",
     packages=find_packages(),
```

### Comparing `ttsmms-0.5/ttsmms/__init__.py` & `ttsmms-0.6/ttsmms/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 import os
 import glob
+import re
 import json
+import tempfile
+import subprocess
 import math
+import logging
 import torch
 from torch import nn
 from torch.nn import functional as F
 from torch.utils.data import DataLoader
 import numpy as np
 import ttsmms.commons
 import ttsmms.utils
@@ -35,47 +39,81 @@
         '''
         sequence = []
         clean_text = text.strip()
         for symbol in clean_text:
             symbol_id = self._symbol_to_id[symbol]
             sequence += [symbol_id]
         return sequence
+    def uromanize(self, text, uroman_pl):
+        iso = "xxx"
+        with tempfile.NamedTemporaryFile() as tf, \
+             tempfile.NamedTemporaryFile() as tf2:
+            with open(tf.name, "w") as f:
+                f.write("\n".join([text]))
+            cmd = f"perl " + uroman_pl
+            cmd += f" -l {iso} "
+            cmd +=  f" < {tf.name} > {tf2.name}"
+            os.system(cmd)
+            outtexts = []
+            with open(tf2.name) as f:
+                for line in f:
+                    line =  re.sub(r"\s+", " ", line).strip()
+                    outtexts.append(line)
+            outtext = outtexts[0]
+        return outtext
 
     def get_text(self, text, hps):
         text_norm = self.text_to_sequence(text, hps.data.text_cleaners)
         if hps.data.add_blank:
             text_norm = ttsmms.commons.intersperse(text_norm, 0)
         text_norm = torch.LongTensor(text_norm)
         return text_norm
 
     def filter_oov(self, text):
         val_chars = self._symbol_to_id
         txt_filt = "".join(list(filter(lambda x: x in val_chars, text)))
         return txt_filt
 
 class TTS:
-    def __init__(self, model_dir_path: str) -> None:
+    def __init__(self, model_dir_path: str, uroman_dir:str=None) -> None:
         self.model_path = model_dir_path
         self.vocab_file = f"{self.model_path}/vocab.txt"
         self.config_file = f"{self.model_path}/config.json"
+        self.uroman_dir = uroman_dir
         assert os.path.isfile(self.config_file), f"{self.config_file} doesn't exist"
         self.hps = ttsmms.utils.get_hparams_from_file(self.config_file)
         self.text_mapper = TextMapper(self.vocab_file)
         self.net_g = SynthesizerTrn(
             len(self.text_mapper.symbols),
             self.hps.data.filter_length // 2 + 1,
             self.hps.train.segment_size // self.hps.data.hop_length,
             **self.hps.model
         )
         _ = self.net_g.eval()
 
         self.g_pth = f"{self.model_path}/G_100000.pth"
         _ = ttsmms.utils.load_checkpoint(self.g_pth, self.net_g, None)
         self.sampling_rate=self.hps.data.sampling_rate
+        self.is_uroman = self.hps.data.training_files.split('.')[-1] == 'uroman'
+    def _use_uroman(self, txt):
+        if self.is_uroman != True:
+            return txt
+        if self.uroman_dir is None:
+            tmp_dir = os.path.join(os.getcwd(),"uroman")
+            if os.path.exists(tmp_dir) == False:
+                cmd = f"git clone https://github.com/isi-nlp/uroman.git {tmp_dir}"
+                logging.info(f"downloading uroman and save to {tmp_dir}")
+                subprocess.check_output(cmd, shell=True)
+            self.uroman_dir = tmp_dir
+        uroman_pl = os.path.join(self.uroman_dir, "bin", "uroman.pl")
+        logging.info("uromanize")
+        txt =  self.text_mapper.uromanize(txt, uroman_pl)
+        return txt
     def synthesis(self, txt, wav_path=None):
+        txt = self._use_uroman(txt)
         txt = self.text_mapper.filter_oov(txt)
         stn_tst = self.text_mapper.get_text(txt, self.hps)
         with torch.no_grad():
             x_tst = stn_tst.unsqueeze(0)#.cuda()
             x_tst_lengths = torch.LongTensor([stn_tst.size(0)])#.cuda()
             hyp = self.net_g.infer(
                 x_tst, x_tst_lengths, noise_scale=.667,
```

### Comparing `ttsmms-0.5/ttsmms/attentions.py` & `ttsmms-0.6/ttsmms/attentions.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/commons.py` & `ttsmms-0.6/ttsmms/commons.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/data_utils.py` & `ttsmms-0.6/ttsmms/data_utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/losses.py` & `ttsmms-0.6/ttsmms/losses.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/mel_processing.py` & `ttsmms-0.6/ttsmms/mel_processing.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/models.py` & `ttsmms-0.6/ttsmms/models.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/modules.py` & `ttsmms-0.6/ttsmms/modules.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/preprocess.py` & `ttsmms-0.6/ttsmms/preprocess.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/text/__init__.py` & `ttsmms-0.6/ttsmms/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/text/cleaners.py` & `ttsmms-0.6/ttsmms/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/text/symbols.py` & `ttsmms-0.6/ttsmms/text/symbols.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/transforms.py` & `ttsmms-0.6/ttsmms/transforms.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms/utils.py` & `ttsmms-0.6/ttsmms/utils.py`

 * *Files identical despite different names*

### Comparing `ttsmms-0.5/ttsmms.egg-info/PKG-INFO` & `ttsmms-0.6/ttsmms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttsmms
-Version: 0.5
+Version: 0.6
 Summary: Text-to-speech with The Massively Multilingual Speech (MMS) project
 Home-page: https://github.com/wannaphong/ttsmms
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: MIT License
 Project-URL: Source, https://github.com/wannaphong/ttsmms
 Keywords: tts,NLP
```


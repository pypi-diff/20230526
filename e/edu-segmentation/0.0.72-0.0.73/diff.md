# Comparing `tmp/edu_segmentation-0.0.72.tar.gz` & `tmp/edu_segmentation-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.72.tar", max compression
+gzip compressed data, was "edu_segmentation-0.0.73.tar", max compression
```

## Comparing `edu_segmentation-0.0.72.tar` & `edu_segmentation-0.0.73.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.72/edu_segmentation/__init__.py
--rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
--rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
--rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
--rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/config.py
--rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/model.py
--rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-r--r--   0        0        0     7483 2023-05-26 07:56:01.905628 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver.py
--rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver_bart.py
--rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     8945 2023-05-26 08:17:50.845444 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
--rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
--rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/config.py
--rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging.py
--rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-r--r--   0        0        0     7031 2023-05-26 08:19:36.793780 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver.py
--rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/test_model.py
--rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model.py
--rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.72/edu_segmentation/initial_dep.txt
--rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.72/edu_segmentation/initial_dep_conda.txt
--rw-r--r--   0        0        0     1865 2023-05-26 07:59:57.504246 edu_segmentation-0.0.72/edu_segmentation/main.py
--rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/all_vocabulary.pickle
--rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/model_bart_v2.py
--rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.72/edu_segmentation/model_dependencies/train_segbot_bart.py
--rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.72/edu_segmentation/requirements.txt
--rw-r--r--   0        0        0      589 2023-05-26 08:21:31.350945 edu_segmentation-0.0.72/pyproject.toml
--rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.72/readme.md
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.72/PKG-INFO
+-rw-r--r--   0        0        0     3575 2023-05-26 07:37:08.573024 edu_segmentation-0.0.73/edu_segmentation/__init__.py
+-rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
+-rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
+-rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/model.py
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-r--r--   0        0        0     7483 2023-05-26 07:56:01.905628 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/solver_bart.py
+-rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8950 2023-05-26 08:29:52.430340 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     7031 2023-05-26 08:19:36.793780 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0        0 2023-04-27 16:13:15.942549 edu_segmentation-0.0.73/edu_segmentation/initial_dep.txt
+-rw-r--r--   0        0        0     2572 2023-04-27 16:14:15.149001 edu_segmentation-0.0.73/edu_segmentation/initial_dep_conda.txt
+-rw-r--r--   0        0        0     1867 2023-05-26 08:32:06.723542 edu_segmentation-0.0.73/edu_segmentation/main.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.73/edu_segmentation/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.73/edu_segmentation/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.73/edu_segmentation/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     2584 2023-04-28 09:07:59.951990 edu_segmentation-0.0.73/edu_segmentation/requirements.txt
+-rw-r--r--   0        0        0      589 2023-05-26 08:32:17.300217 edu_segmentation-0.0.73/pyproject.toml
+-rw-r--r--   0        0        0      737 2023-04-28 16:39:16.999884 edu_segmentation-0.0.73/readme.md
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 edu_segmentation-0.0.73/PKG-INFO
```

### Comparing `edu_segmentation-0.0.72/edu_segmentation/__init__.py` & `edu_segmentation-0.0.73/edu_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/model.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu_segmentation-0.0.73/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x16667064 (Fri May 26 07:56:06 2023 UTC)
-files sz: 7030
+moddate:  0x986b7064 (Fri May 26 08:19:36 2023 UTC)
+files sz: 7031
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02020065026a0300
       000000000000006403a6010000ab0100000000000000000100640064026c
-      045a04640064026c055a05640064026c065a06640064026c075a08640064
-      046c096d0a5a0a01006405650b64066501650c1900000000000000000066
-      04640784045a0d6408650b6602640984045a0e640a84005a0f640b84005a
+      045a04640064026c055a05640064026c065a06640064026c075a08640464
+      056c096d0a5a0a01006406650b64076501650c1900000000000000000066
+      04640884045a0d6409650b6602640a84045a0e640b84005a0f640c84005a
       1064025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('List',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
@@ -51,53 +51,54 @@
                 76 STORE_NAME               6 (transformers)
    
      9          78 LOAD_CONST               0 (0)
                 80 LOAD_CONST               2 (None)
                 82 IMPORT_NAME              7 (numpy)
                 84 STORE_NAME               8 (np)
    
-    11          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               4 (('TOKENIZER',))
+    11          86 LOAD_CONST               4 (1)
+                88 LOAD_CONST               5 (('TOKENIZER',))
                 90 IMPORT_NAME              9 (config)
                 92 IMPORT_FROM             10 (TOKENIZER)
                 94 STORE_NAME              10 (TOKENIZER)
                 96 POP_TOP
    
-    14          98 LOAD_CONST               5 ('text')
+    14          98 LOAD_CONST               6 ('text')
                100 LOAD_NAME               11 (str)
-               102 LOAD_CONST               6 ('return')
+               102 LOAD_CONST               7 ('return')
                104 LOAD_NAME                1 (List)
                106 LOAD_NAME               12 (int)
                108 BINARY_SUBSCR
                118 BUILD_TUPLE              4
-               120 LOAD_CONST               7 (<code object bert_tokenizer, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 14>)
+               120 LOAD_CONST               8 (<code object bert_tokenizer, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 14>)
                122 MAKE_FUNCTION            4 (annotations)
                124 STORE_NAME              13 (bert_tokenizer)
    
-    36         126 LOAD_CONST               8 ('inputstring')
+    36         126 LOAD_CONST               9 ('inputstring')
                128 LOAD_NAME               11 (str)
                130 BUILD_TUPLE              2
-               132 LOAD_CONST               9 (<code object parse_input, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 36>)
+               132 LOAD_CONST              10 (<code object parse_input, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 36>)
                134 MAKE_FUNCTION            4 (annotations)
                136 STORE_NAME              14 (parse_input)
    
-   107         138 LOAD_CONST              10 (<code object get_inference, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 107>)
+   107         138 LOAD_CONST              11 (<code object get_inference, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 107>)
                140 MAKE_FUNCTION            0
                142 STORE_NAME              15 (get_inference)
    
-   161         144 LOAD_CONST              11 (<code object run_segbot_bert, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 161>)
+   161         144 LOAD_CONST              12 (<code object run_segbot_bert, file "C:\Users\Patri\OneDrive\Documents\GitHub\patriafyp\FYP-EDU-Segmentation-final\edu_segmentation\BERTTokenClassification\run_bert.py", line 161>)
                146 MAKE_FUNCTION            0
                148 STORE_NAME              16 (run_segbot_bert)
                150 LOAD_CONST               2 (None)
                152 RETURN_VALUE
    consts
       0
       ('List',)
       None
       'ignore'
+      1
       ('TOKENIZER',)
       'text'
       'return'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
```

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.73/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/initial_dep_conda.txt` & `edu_segmentation-0.0.73/edu_segmentation/initial_dep_conda.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/main.py` & `edu_segmentation-0.0.73/edu_segmentation/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from BARTTokenClassification.run_segbot_bart import run_segbot_bart
-from BERTTokenClassification.run_bert import run_segbot_bert
+from .BARTTokenClassification.run_segbot_bart import run_segbot_bart
+from .BERTTokenClassification.run_bert import run_segbot_bert
 
 def run_segbot(sent, granularity_level="default", model="bart"):
     print("----------- EDU Segmentation with Segbot with BART model: ----------")
     results = []
 
     segbot_model = run_segbot_bart
     if model == "bert_uncased":
```

### Comparing `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/all_vocabulary.pickle` & `edu_segmentation-0.0.73/edu_segmentation/model_dependencies/all_vocabulary.pickle`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.73/edu_segmentation/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.73/edu_segmentation/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/edu_segmentation/requirements.txt` & `edu_segmentation-0.0.73/edu_segmentation/requirements.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/pyproject.toml` & `edu_segmentation-0.0.73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_segmentation"
-version = "v0.0.72"
+version = "v0.0.73"
 description = "To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset."
 authors = ["Your Name <you@example.com>"]
 readme = "readme.md"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edu_segmentation-0.0.72/readme.md` & `edu_segmentation-0.0.73/readme.md`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.72/PKG-INFO` & `edu_segmentation-0.0.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.72
+Version: 0.0.73
 Summary: To improve EDU segmentation performance using Segbot. As Segbot has an encoder-decoder model architecture, we can replace bidirectional GRU encoder with generative pretraining models such as BART and T5. Evaluate the new model using the RST dataset by using few-shot based settings (e.g. 100 examples) to train the model, instead of using the full dataset.
 Author: Your Name
 Author-email: you@example.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```


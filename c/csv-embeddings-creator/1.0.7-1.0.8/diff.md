# Comparing `tmp/csv-embeddings-creator-1.0.7.tar.gz` & `tmp/csv-embeddings-creator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-embeddings-creator-1.0.7.tar", last modified: Thu May 25 14:30:34 2023, max compression
+gzip compressed data, was "csv-embeddings-creator-1.0.8.tar", last modified: Fri May 26 03:12:05 2023, max compression
```

## Comparing `csv-embeddings-creator-1.0.7.tar` & `csv-embeddings-creator-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:30:34.639886 csv-embeddings-creator-1.0.7/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-25 14:30:34.639776 csv-embeddings-creator-1.0.7/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-25 14:30:34.639603 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3220 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/csv_embeddings_creator.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-25 14:30:34.639920 csv-embeddings-creator-1.0.7/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-25 14:30:34.000000 csv-embeddings-creator-1.0.7/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 03:12:05.078931 csv-embeddings-creator-1.0.8/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 03:12:05.078821 csv-embeddings-creator-1.0.8/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 03:12:05.078636 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3544 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-26 03:12:05.078963 csv-embeddings-creator-1.0.8/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/setup.py
```

### Comparing `csv-embeddings-creator-1.0.7/PKG-INFO` & `csv-embeddings-creator-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.7
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
 
 這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
@@ -79,9 +75,7 @@
 ### Q: 句子嵌入的尺寸是多少？
 
 A: 使用 `paraphrase-multilingual-MiniLM-L12-v2` 模型生成的句子嵌入的尺寸為 384。不同的 Transformer 模型可能具有不同的嵌入尺寸。
 
 ## 貢獻
 
 我們歡迎您為 `csv_embeddings_creator` 做出貢獻！如果您有任何建議、改進或修復錯誤，請在 GitHub 存儲庫中創建一個 Pull 請求。
-
-
```

### Comparing `csv-embeddings-creator-1.0.7/README.md` & `csv-embeddings-creator-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `csv-embeddings-creator-1.0.7/csv_embeddings_creator.egg-info/PKG-INFO` & `csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.7
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
 
 這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
@@ -79,9 +75,7 @@
 ### Q: 句子嵌入的尺寸是多少？
 
 A: 使用 `paraphrase-multilingual-MiniLM-L12-v2` 模型生成的句子嵌入的尺寸為 384。不同的 Transformer 模型可能具有不同的嵌入尺寸。
 
 ## 貢獻
 
 我們歡迎您為 `csv_embeddings_creator` 做出貢獻！如果您有任何建議、改進或修復錯誤，請在 GitHub 存儲庫中創建一個 Pull 請求。
-
-
```

### Comparing `csv-embeddings-creator-1.0.7/csv_embeddings_creator.py` & `csv-embeddings-creator-1.0.8/csv_embeddings_creator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 #!/usr/bin/env python
 # csv_embeddings_creator.py
 import argparse
 import csv
 import glob
 import os
 import re
+from concurrent.futures import ThreadPoolExecutor
 from time import time
 
 import torch
 from sentence_transformers import SentenceTransformer
 
+sentence_transformer = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
 
-def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False):
-    model = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
 
+def find_pattern(pattern, path):
+    match = re.search(pattern, path)
+    return match.group(0) if match else ''
+
+
+def encode_row(row, model):
+    embedding_input = '"' + '","'.join(row) + '"'
+    embeddings = model.encode(embedding_input)
+    return row, embeddings
+
+
+def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False, num_threads=10):
     os.makedirs(output_txt_folder, exist_ok=True)
     os.makedirs(output_embeddings_folder, exist_ok=True)
 
     csv_files = glob.glob(os.path.join(input_folder, '**/*.csv'), recursive=True)
     embedding_files = glob.glob(os.path.join(output_embeddings_folder, '**/*.pt'), recursive=True)
 
-    dic_doc_id = {}
-    for path in embedding_files:
-        matches = re.findall('doc-id_(.*?)_sha', path)
-        if matches:
-            doc_id = matches[0]
-            dic_doc_id[doc_id] = True
+    dic_skip_done_doc_id = {}
+    if not force:
+        for path in embedding_files:
+            dic_skip_done_doc_id[find_pattern('doc-id_(.*?)_sha', path)] = True
 
     i = 0
     for csv_file in csv_files:
-        matches = re.findall('doc-id_(.*?)_sha', path)
-        if matches:
-            doc_id = matches[0]
-            if doc_id in dic_doc_id:
-                continue
-
-        file_base_name = os.path.splitext(os.path.basename(csv_file))[0]
-        existing_txt_files = glob.glob(os.path.join(output_txt_folder, f"{file_base_name}_*.txt"))
-
-        if not force and existing_txt_files:
+        if find_pattern('doc-id_(.*?)_sha', csv_file) in dic_skip_done_doc_id:
             continue
-
+        file_base_name = os.path.splitext(os.path.basename(csv_file))[0]
         with open(csv_file, 'r', encoding='utf-8') as f:
             reader = csv.reader(f)
-            for idx, row in enumerate(reader):
-                t = time()
+
+            with ThreadPoolExecutor(max_workers=num_threads) as executor:
+                all_embeddings = list(executor.map(lambda row: encode_row(row, sentence_transformer), reader))
+
+            for idx, (row, row_embeddings) in enumerate(all_embeddings):
+                print('idx', idx)
                 i += 1
                 folder_txt = os.path.join(output_txt_folder, f"{file_base_name}")
                 os.makedirs(folder_txt, exist_ok=True)
                 txt_file = os.path.join(folder_txt, f"{file_base_name}_{idx + 1}.txt")
                 with open(txt_file, 'w', encoding='utf-8') as txt_f:
                     txt_f.write('"' + '","'.join(row) + '"')
-                embeddings = model.encode('"' + '","'.join(row) + '"')
+
                 folder_embeddings = os.path.join(output_embeddings_folder, f"{file_base_name}")
                 os.makedirs(folder_embeddings, exist_ok=True)
                 embeddings_file = os.path.join(folder_embeddings, f"{file_base_name}_{idx + 1}.pt")
-                torch.save(embeddings, embeddings_file)
-                print('csv_embeddings_creator.py,i,time:', i, time() - t)
+                torch.save(row_embeddings, embeddings_file)
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Create embeddings for text files using Hugging Face Transformers.')
     parser.add_argument('--input-folder', type=str, required=True,
                         help='Input folder containing CSV files')
     parser.add_argument('--output-txt-folder', type=str, required=True,
                         help='Output folder for the txt files')
     parser.add_argument('--embeddings-folder', type=str, required=True,
                         help='Output folder for the embeddings')
     parser.add_argument('--force', action='store_true',
                         help='Force to recreate embeddings even if they already exist')
+    parser.add_argument('--num-threads', type=int, default=10,
+                        help='Number of threads')
     return parser.parse_args()
 
 
 def main():
+    t = time()
     args = parse_arguments()
-    create_embeddings(args.input_folder, args.output_txt_folder, args.embeddings_folder, args.force)
+    create_embeddings(args.input_folder, args.output_txt_folder, args.embeddings_folder, args.force, args.num_threads)
+    print(time() - t)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `csv-embeddings-creator-1.0.7/setup.py` & `csv-embeddings-creator-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-embeddings-creator",
-    version="1.0.7",
+    version="1.0.8",
     packages=find_packages(),
     py_modules=['csv_embeddings_creator'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_embeddings_creator = csv_embeddings_creator:main',
         ],
```


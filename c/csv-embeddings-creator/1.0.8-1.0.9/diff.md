# Comparing `tmp/csv-embeddings-creator-1.0.8.tar.gz` & `tmp/csv-embeddings-creator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-embeddings-creator-1.0.8.tar", last modified: Fri May 26 03:12:05 2023, max compression
+gzip compressed data, was "csv-embeddings-creator-1.0.9.tar", last modified: Fri May 26 06:50:55 2023, max compression
```

## Comparing `csv-embeddings-creator-1.0.8.tar` & `csv-embeddings-creator-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 03:12:05.078931 csv-embeddings-creator-1.0.8/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 03:12:05.078821 csv-embeddings-creator-1.0.8/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 03:12:05.078636 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-26 03:12:05.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3544 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/csv_embeddings_creator.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-26 03:12:05.078963 csv-embeddings-creator-1.0.8/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-26 03:12:04.000000 csv-embeddings-creator-1.0.8/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 06:50:55.373906 csv-embeddings-creator-1.0.9/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 06:50:55.373753 csv-embeddings-creator-1.0.9/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-26 06:50:55.373531 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3063 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3553 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/csv_embeddings_creator.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-26 06:50:55.373950 csv-embeddings-creator-1.0.9/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-26 06:50:55.000000 csv-embeddings-creator-1.0.9/setup.py
```

### Comparing `csv-embeddings-creator-1.0.8/PKG-INFO` & `csv-embeddings-creator-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.8
+Version: 1.0.9
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
 
 這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
```

### Comparing `csv-embeddings-creator-1.0.8/README.md` & `csv-embeddings-creator-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `csv-embeddings-creator-1.0.8/csv_embeddings_creator.egg-info/PKG-INFO` & `csv-embeddings-creator-1.0.9/csv_embeddings_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.8
+Version: 1.0.9
 Description-Content-Type: text/markdown
 
 # csv_embeddings_creator v1.0.4 by Bowen Chiu
 
 這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
```

### Comparing `csv-embeddings-creator-1.0.8/csv_embeddings_creator.py` & `csv-embeddings-creator-1.0.9/csv_embeddings_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 import re
 from concurrent.futures import ThreadPoolExecutor
 from time import time
 
 import torch
 from sentence_transformers import SentenceTransformer
 
+DEFAULT_NUM_THREADS = 4
 sentence_transformer = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
 
 
 def find_pattern(pattern, path):
     match = re.search(pattern, path)
     return match.group(0) if match else ''
 
 
 def encode_row(row, model):
     embedding_input = '"' + '","'.join(row) + '"'
     embeddings = model.encode(embedding_input)
     return row, embeddings
 
 
-def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False, num_threads=10):
+def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False,
+                      num_threads=DEFAULT_NUM_THREADS):
     os.makedirs(output_txt_folder, exist_ok=True)
     os.makedirs(output_embeddings_folder, exist_ok=True)
 
     csv_files = glob.glob(os.path.join(input_folder, '**/*.csv'), recursive=True)
     embedding_files = glob.glob(os.path.join(output_embeddings_folder, '**/*.pt'), recursive=True)
 
     dic_skip_done_doc_id = {}
@@ -45,15 +47,14 @@
         with open(csv_file, 'r', encoding='utf-8') as f:
             reader = csv.reader(f)
 
             with ThreadPoolExecutor(max_workers=num_threads) as executor:
                 all_embeddings = list(executor.map(lambda row: encode_row(row, sentence_transformer), reader))
 
             for idx, (row, row_embeddings) in enumerate(all_embeddings):
-                print('idx', idx)
                 i += 1
                 folder_txt = os.path.join(output_txt_folder, f"{file_base_name}")
                 os.makedirs(folder_txt, exist_ok=True)
                 txt_file = os.path.join(folder_txt, f"{file_base_name}_{idx + 1}.txt")
                 with open(txt_file, 'w', encoding='utf-8') as txt_f:
                     txt_f.write('"' + '","'.join(row) + '"')
 
@@ -69,21 +70,19 @@
                         help='Input folder containing CSV files')
     parser.add_argument('--output-txt-folder', type=str, required=True,
                         help='Output folder for the txt files')
     parser.add_argument('--embeddings-folder', type=str, required=True,
                         help='Output folder for the embeddings')
     parser.add_argument('--force', action='store_true',
                         help='Force to recreate embeddings even if they already exist')
-    parser.add_argument('--num-threads', type=int, default=10,
+    parser.add_argument('--num-threads', type=int, default=DEFAULT_NUM_THREADS,
                         help='Number of threads')
     return parser.parse_args()
 
 
 def main():
-    t = time()
     args = parse_arguments()
     create_embeddings(args.input_folder, args.output_txt_folder, args.embeddings_folder, args.force, args.num_threads)
-    print(time() - t)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `csv-embeddings-creator-1.0.8/setup.py` & `csv-embeddings-creator-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-embeddings-creator",
-    version="1.0.8",
+    version="1.0.9",
     packages=find_packages(),
     py_modules=['csv_embeddings_creator'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_embeddings_creator = csv_embeddings_creator:main',
         ],
```


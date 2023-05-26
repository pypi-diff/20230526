# Comparing `tmp/pydoxtools-0.6.1.tar.gz` & `tmp/pydoxtools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoxtools-0.6.1.tar", max compression
+gzip compressed data, was "pydoxtools-0.6.2.tar", max compression
```

## Comparing `pydoxtools-0.6.1.tar` & `pydoxtools-0.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1072 2023-01-19 05:32:50.265107 pydoxtools-0.6.1/LICENSE
--rw-r--r--   0        0        0     8260 2023-05-25 01:08:00.818589 pydoxtools-0.6.1/README.md
--rw-r--r--   0        0        0      258 2023-05-25 06:20:55.635381 pydoxtools-0.6.1/pydoxtools/__init__.py
--rw-r--r--   0        0        0    11153 2023-05-25 00:15:16.561311 pydoxtools-0.6.1/pydoxtools/agent.py
--rw-r--r--   0        0        0     2508 2022-02-09 15:52:43.898218 pydoxtools-0.6.1/pydoxtools/class_utils.py
--rwxr-xr-x   0        0        0    30541 2023-05-09 05:49:37.140825 pydoxtools-0.6.1/pydoxtools/classifier.py
--rw-r--r--   0        0        0    29431 2022-11-12 20:39:33.790453 pydoxtools-0.6.1/pydoxtools/cluster_utils.py
--rw-r--r--   0        0        0     6047 2023-05-25 01:00:13.344389 pydoxtools-0.6.1/pydoxtools/dask_operators.py
--rw-r--r--   0        0        0    53220 2023-05-24 17:14:40.070633 pydoxtools-0.6.1/pydoxtools/document.py
--rw-r--r--   0        0        0    35071 2023-05-24 00:02:05.489329 pydoxtools-0.6.1/pydoxtools/document_base.py
--rw-r--r--   0        0        0     1673 2023-05-09 23:54:11.246379 pydoxtools-0.6.1/pydoxtools/extract_classes.py
--rw-r--r--   0        0        0        3 2023-05-02 20:33:41.756428 pydoxtools-0.6.1/pydoxtools/extract_db.py
--rw-r--r--   0        0        0     3978 2023-05-23 19:28:54.538602 pydoxtools-0.6.1/pydoxtools/extract_filesystem.py
--rw-r--r--   0        0        0    13329 2023-05-09 23:54:11.178377 pydoxtools-0.6.1/pydoxtools/extract_html.py
--rw-r--r--   0        0        0    12354 2023-05-26 17:50:33.184310 pydoxtools-0.6.1/pydoxtools/extract_index.py
--rw-r--r--   0        0        0     3177 2023-05-20 06:10:12.179526 pydoxtools-0.6.1/pydoxtools/extract_nlpchat.py
--rw-r--r--   0        0        0     2469 2023-05-09 23:54:11.186378 pydoxtools-0.6.1/pydoxtools/extract_objects.py
--rw-r--r--   0        0        0     1656 2023-05-10 07:01:17.768739 pydoxtools-0.6.1/pydoxtools/extract_ocr.py
--rw-r--r--   0        0        0     6469 2023-05-23 19:52:11.543694 pydoxtools-0.6.1/pydoxtools/extract_pandoc.py
--rw-r--r--   0        0        0     5544 2023-05-09 23:54:11.270379 pydoxtools-0.6.1/pydoxtools/extract_spacy.py
--rw-r--r--   0        0        0    43269 2023-05-20 05:43:43.697769 pydoxtools-0.6.1/pydoxtools/extract_tables.py
--rw-r--r--   0        0        0     8139 2023-05-09 23:54:11.150377 pydoxtools-0.6.1/pydoxtools/extract_textstructure.py
--rw-r--r--   0        0        0     1232 2023-04-26 22:02:00.116297 pydoxtools-0.6.1/pydoxtools/file_utils.py
--rwxr-xr-x   0        0        0     6143 2022-11-12 20:39:33.794453 pydoxtools-0.6.1/pydoxtools/html_utils.py
--rw-r--r--   0        0        0      150 2022-02-09 15:52:43.898218 pydoxtools-0.6.1/pydoxtools/initialize_library.py
--rw-r--r--   0        0        0     7077 2022-11-12 20:39:33.794453 pydoxtools-0.6.1/pydoxtools/labeling.py
--rw-r--r--   0        0        0     7364 2023-05-18 23:05:10.290935 pydoxtools-0.6.1/pydoxtools/list_utils.py
--rw-r--r--   0        0        0      371 2022-11-12 20:39:33.794453 pydoxtools-0.6.1/pydoxtools/math_utils.py
--rw-r--r--   0        0        0     2431 2022-11-12 20:39:33.794453 pydoxtools-0.6.1/pydoxtools/models.py
--rwxr-xr-x   0        0        0    18776 2023-05-06 19:40:13.998671 pydoxtools-0.6.1/pydoxtools/nlp_utils.py
--rw-r--r--   0        0        0     2502 2022-03-30 10:01:09.241031 pydoxtools-0.6.1/pydoxtools/ocr_language_mappings.py
--rw-r--r--   0        0        0     8897 2023-05-09 23:54:11.158377 pydoxtools-0.6.1/pydoxtools/operator_huggingface.py
--rw-r--r--   0        0        0     1137 2023-05-14 18:22:46.918667 pydoxtools-0.6.1/pydoxtools/operators.py
--rw-r--r--   0        0        0     7856 2023-05-22 06:53:09.989310 pydoxtools-0.6.1/pydoxtools/operators_base.py
--rwxr-xr-x   0        0        0    12146 2023-05-09 23:54:11.106376 pydoxtools-0.6.1/pydoxtools/pdf_utils.py
--rw-r--r--   0        0        0    34126 2023-03-28 06:51:36.920970 pydoxtools-0.6.1/pydoxtools/random_data_generators.py
--rwxr-xr-x   0        0        0     1332 2023-05-11 04:47:15.118352 pydoxtools-0.6.1/pydoxtools/settings.py
--rw-r--r--   0        0        0    17693 2023-05-09 05:49:37.108824 pydoxtools-0.6.1/pydoxtools/training.py
--rw-r--r--   0        0        0     3898 2022-02-09 15:52:43.898218 pydoxtools-0.6.1/pydoxtools/visual_document_analysis.py
--rw-r--r--   0        0        0     3209 2023-01-19 05:32:50.269106 pydoxtools-0.6.1/pydoxtools/webdav_utils.py
--rw-r--r--   0        0        0     5950 2023-05-26 17:54:23.694458 pydoxtools-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    11122 1970-01-01 00:00:00.000000 pydoxtools-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-19 05:32:50.265107 pydoxtools-0.6.2/LICENSE
+-rw-r--r--   0        0        0     8260 2023-05-25 01:08:00.818589 pydoxtools-0.6.2/README.md
+-rw-r--r--   0        0        0      258 2023-05-25 06:20:55.635381 pydoxtools-0.6.2/pydoxtools/__init__.py
+-rw-r--r--   0        0        0    11157 2023-05-26 18:46:19.000755 pydoxtools-0.6.2/pydoxtools/agent.py
+-rw-r--r--   0        0        0     2508 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/class_utils.py
+-rwxr-xr-x   0        0        0    30541 2023-05-09 05:49:37.140825 pydoxtools-0.6.2/pydoxtools/classifier.py
+-rw-r--r--   0        0        0    29431 2022-11-12 20:39:33.790453 pydoxtools-0.6.2/pydoxtools/cluster_utils.py
+-rw-r--r--   0        0        0     6047 2023-05-25 01:00:13.344389 pydoxtools-0.6.2/pydoxtools/dask_operators.py
+-rw-r--r--   0        0        0    53220 2023-05-24 17:14:40.070633 pydoxtools-0.6.2/pydoxtools/document.py
+-rw-r--r--   0        0        0    35071 2023-05-24 00:02:05.489329 pydoxtools-0.6.2/pydoxtools/document_base.py
+-rw-r--r--   0        0        0     1673 2023-05-09 23:54:11.246379 pydoxtools-0.6.2/pydoxtools/extract_classes.py
+-rw-r--r--   0        0        0        3 2023-05-02 20:33:41.756428 pydoxtools-0.6.2/pydoxtools/extract_db.py
+-rw-r--r--   0        0        0     3978 2023-05-23 19:28:54.538602 pydoxtools-0.6.2/pydoxtools/extract_filesystem.py
+-rw-r--r--   0        0        0    13329 2023-05-09 23:54:11.178377 pydoxtools-0.6.2/pydoxtools/extract_html.py
+-rw-r--r--   0        0        0    12566 2023-05-26 18:48:24.639525 pydoxtools-0.6.2/pydoxtools/extract_index.py
+-rw-r--r--   0        0        0     3177 2023-05-20 06:10:12.179526 pydoxtools-0.6.2/pydoxtools/extract_nlpchat.py
+-rw-r--r--   0        0        0     2469 2023-05-09 23:54:11.186378 pydoxtools-0.6.2/pydoxtools/extract_objects.py
+-rw-r--r--   0        0        0     1656 2023-05-10 07:01:17.768739 pydoxtools-0.6.2/pydoxtools/extract_ocr.py
+-rw-r--r--   0        0        0     6469 2023-05-23 19:52:11.543694 pydoxtools-0.6.2/pydoxtools/extract_pandoc.py
+-rw-r--r--   0        0        0     5544 2023-05-09 23:54:11.270379 pydoxtools-0.6.2/pydoxtools/extract_spacy.py
+-rw-r--r--   0        0        0    43269 2023-05-20 05:43:43.697769 pydoxtools-0.6.2/pydoxtools/extract_tables.py
+-rw-r--r--   0        0        0     8139 2023-05-09 23:54:11.150377 pydoxtools-0.6.2/pydoxtools/extract_textstructure.py
+-rw-r--r--   0        0        0     1232 2023-04-26 22:02:00.116297 pydoxtools-0.6.2/pydoxtools/file_utils.py
+-rwxr-xr-x   0        0        0     6143 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/html_utils.py
+-rw-r--r--   0        0        0      150 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/initialize_library.py
+-rw-r--r--   0        0        0     7077 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/labeling.py
+-rw-r--r--   0        0        0     7364 2023-05-18 23:05:10.290935 pydoxtools-0.6.2/pydoxtools/list_utils.py
+-rw-r--r--   0        0        0      371 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/math_utils.py
+-rw-r--r--   0        0        0     2431 2022-11-12 20:39:33.794453 pydoxtools-0.6.2/pydoxtools/models.py
+-rwxr-xr-x   0        0        0    18776 2023-05-06 19:40:13.998671 pydoxtools-0.6.2/pydoxtools/nlp_utils.py
+-rw-r--r--   0        0        0     2502 2022-03-30 10:01:09.241031 pydoxtools-0.6.2/pydoxtools/ocr_language_mappings.py
+-rw-r--r--   0        0        0     8897 2023-05-09 23:54:11.158377 pydoxtools-0.6.2/pydoxtools/operator_huggingface.py
+-rw-r--r--   0        0        0     1137 2023-05-14 18:22:46.918667 pydoxtools-0.6.2/pydoxtools/operators.py
+-rw-r--r--   0        0        0     7856 2023-05-22 06:53:09.989310 pydoxtools-0.6.2/pydoxtools/operators_base.py
+-rwxr-xr-x   0        0        0    12146 2023-05-09 23:54:11.106376 pydoxtools-0.6.2/pydoxtools/pdf_utils.py
+-rw-r--r--   0        0        0    34126 2023-03-28 06:51:36.920970 pydoxtools-0.6.2/pydoxtools/random_data_generators.py
+-rwxr-xr-x   0        0        0     1332 2023-05-11 04:47:15.118352 pydoxtools-0.6.2/pydoxtools/settings.py
+-rw-r--r--   0        0        0    17693 2023-05-09 05:49:37.108824 pydoxtools-0.6.2/pydoxtools/training.py
+-rw-r--r--   0        0        0     3898 2022-02-09 15:52:43.898218 pydoxtools-0.6.2/pydoxtools/visual_document_analysis.py
+-rw-r--r--   0        0        0     3209 2023-01-19 05:32:50.269106 pydoxtools-0.6.2/pydoxtools/webdav_utils.py
+-rw-r--r--   0        0        0     5950 2023-05-26 19:02:02.709630 pydoxtools-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    11122 1970-01-01 00:00:00.000000 pydoxtools-0.6.2/PKG-INFO
```

### Comparing `pydoxtools-0.6.1/LICENSE` & `pydoxtools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/README.md` & `pydoxtools-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/agent.py` & `pydoxtools-0.6.2/pydoxtools/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,17 +188,17 @@
                               format=formatting)
         msg = '\n'.join(m['content'] for m in msgs)
         logger.info(f"execute_task: {msg}")
         res = openai_chat_completion(msgs, max_tokens=max_tokens).content
         self._debug_queue.append((msgs, res))
         if formatting == "yaml":
             res = yaml_loader(res)
-        if formatting == "txt":
+        elif formatting == "txt":
             res = res
-        if formatting == "markdown":
+        elif formatting == "markdown":
             res = res
         else:
             logger.warning(f"Formatting: {formatting} is unknown!")
             pass  # do nothing ;)
         if save_task:
             self.add_task(task, str(res))
         return res
```

### Comparing `pydoxtools-0.6.1/pydoxtools/class_utils.py` & `pydoxtools-0.6.2/pydoxtools/class_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/classifier.py` & `pydoxtools-0.6.2/pydoxtools/classifier.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/cluster_utils.py` & `pydoxtools-0.6.2/pydoxtools/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/dask_operators.py` & `pydoxtools-0.6.2/pydoxtools/dask_operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/document.py` & `pydoxtools-0.6.2/pydoxtools/document.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/document_base.py` & `pydoxtools-0.6.2/pydoxtools/document_base.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_classes.py` & `pydoxtools-0.6.2/pydoxtools/extract_classes.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_filesystem.py` & `pydoxtools-0.6.2/pydoxtools/extract_filesystem.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_html.py` & `pydoxtools-0.6.2/pydoxtools/extract_html.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_index.py` & `pydoxtools-0.6.2/pydoxtools/extract_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,17 @@
             """
             This function is cached, so that we can use an in-memory database
             with the query function and keep it persistant for multiple injection
             operations with "add_to_chroma". As soon as we use dask with multiple processes, we need
             to have a persistant database though!!  make sure, we can somehow detect this...
 
             TODO: document the above a bit more prominent!!
+            TODO: we would like to cache this function locally in memory for faster
+                  access, but chromadb.conf.Settings is not hashable. so we need a different
+                  solution here...
             """
             # add items from bag to chroma piece-by-piece
             if chroma_settings:
                 chroma_client = chromadb.Client(chroma_settings)
             else:
                 chroma_client = chromadb.Client()
             collection_name = collection_name or "in_memory_default"
```

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_nlpchat.py` & `pydoxtools-0.6.2/pydoxtools/extract_nlpchat.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_objects.py` & `pydoxtools-0.6.2/pydoxtools/extract_objects.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_ocr.py` & `pydoxtools-0.6.2/pydoxtools/extract_ocr.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_pandoc.py` & `pydoxtools-0.6.2/pydoxtools/extract_pandoc.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_spacy.py` & `pydoxtools-0.6.2/pydoxtools/extract_spacy.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_tables.py` & `pydoxtools-0.6.2/pydoxtools/extract_tables.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/extract_textstructure.py` & `pydoxtools-0.6.2/pydoxtools/extract_textstructure.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/file_utils.py` & `pydoxtools-0.6.2/pydoxtools/file_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/html_utils.py` & `pydoxtools-0.6.2/pydoxtools/html_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/labeling.py` & `pydoxtools-0.6.2/pydoxtools/labeling.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/list_utils.py` & `pydoxtools-0.6.2/pydoxtools/list_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/models.py` & `pydoxtools-0.6.2/pydoxtools/models.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/nlp_utils.py` & `pydoxtools-0.6.2/pydoxtools/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/ocr_language_mappings.py` & `pydoxtools-0.6.2/pydoxtools/ocr_language_mappings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/operator_huggingface.py` & `pydoxtools-0.6.2/pydoxtools/operator_huggingface.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/operators.py` & `pydoxtools-0.6.2/pydoxtools/operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/operators_base.py` & `pydoxtools-0.6.2/pydoxtools/operators_base.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/pdf_utils.py` & `pydoxtools-0.6.2/pydoxtools/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/random_data_generators.py` & `pydoxtools-0.6.2/pydoxtools/random_data_generators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/settings.py` & `pydoxtools-0.6.2/pydoxtools/settings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/training.py` & `pydoxtools-0.6.2/pydoxtools/training.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/visual_document_analysis.py` & `pydoxtools-0.6.2/pydoxtools/visual_document_analysis.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pydoxtools/webdav_utils.py` & `pydoxtools-0.6.2/pydoxtools/webdav_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.1/pyproject.toml` & `pydoxtools-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoxtools"
-version = "0.6.1"
+version = "0.6.2"
 description = "This library contains a set of tools in order to extract and synthesize structured information from documents"
 authors = ["thomas meschede <yeusblender@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pydoxtools.xyntopia.com"
 repository = "https://github.com/xyntopia/pydoxtools"
 documentation = "https://pydoxtools.xyntopia.com"
```

### Comparing `pydoxtools-0.6.1/PKG-INFO` & `pydoxtools-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoxtools
-Version: 0.6.1
+Version: 0.6.2
 Summary: This library contains a set of tools in order to extract and synthesize structured information from documents
 Home-page: https://pydoxtools.xyntopia.com
 License: MIT
 Keywords: AI,document-analysis,LLM,NLP,ML
 Author: thomas meschede
 Author-email: yeusblender@gmail.com
 Requires-Python: >=3.10,<4.0
```


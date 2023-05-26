# Comparing `tmp/data-preprocessors-0.8.0.tar.gz` & `tmp/data-preprocessors-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-preprocessors-0.8.0.tar", max compression
+gzip compressed data, was "data-preprocessors-0.9.0.tar", max compression
```

## Comparing `data-preprocessors-0.8.0.tar` & `data-preprocessors-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      449 2022-04-16 05:15:54.586070 data-preprocessors-0.8.0/README.md
--rw-r--r--   0        0        0       22 2022-04-15 21:11:35.745537 data-preprocessors-0.8.0/data_preprocessors/__init__.py
--rw-r--r--   0        0        0     1544 2022-05-04 06:29:52.838723 data-preprocessors-0.8.0/data_preprocessors/list_process.py
--rw-r--r--   0        0        0    17393 2022-05-04 08:37:12.312739 data-preprocessors-0.8.0/data_preprocessors/text_preprocessor.py
--rw-r--r--   0        0        0     1171 2022-05-04 06:50:43.568723 data-preprocessors-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1126 2022-05-04 08:56:51.921403 data-preprocessors-0.8.0/setup.py
--rw-r--r--   0        0        0     1767 2022-05-04 08:56:51.923508 data-preprocessors-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      449 2022-04-16 05:15:54.586070 data-preprocessors-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-04-15 21:11:35.745537 data-preprocessors-0.9.0/data_preprocessors/__init__.py
+-rw-r--r--   0        0        0     1544 2022-05-04 06:29:52.838723 data-preprocessors-0.9.0/data_preprocessors/list_process.py
+-rw-r--r--   0        0        0    17579 2022-05-04 09:28:03.412739 data-preprocessors-0.9.0/data_preprocessors/text_preprocessor.py
+-rw-r--r--   0        0        0     1171 2022-05-04 09:28:39.812739 data-preprocessors-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1126 2022-05-04 09:31:08.907959 data-preprocessors-0.9.0/setup.py
+-rw-r--r--   0        0        0     1767 2022-05-04 09:31:08.908241 data-preprocessors-0.9.0/PKG-INFO
```

### Comparing `data-preprocessors-0.8.0/data_preprocessors/list_process.py` & `data-preprocessors-0.9.0/data_preprocessors/list_process.py`

 * *Files identical despite different names*

### Comparing `data-preprocessors-0.8.0/data_preprocessors/text_preprocessor.py` & `data-preprocessors-0.9.0/data_preprocessors/text_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,19 @@
         for listitem in val_data:
             val_file.write("%s\n" % listitem)
 
     with open(test_file_path, "w") as test_file:
         for listitem in test_data:
             test_file.write("%s\n" % listitem)
 
+    print("Total lines: ", len(main_data))
+    print("Train set size: ", len(train_data))
+    print("Validation set size: ", len(val_data))
+    print("Test set size: ", len(test_data))
+
 
 # =================================================
 # Add a space before and after a punctuation mark
 # =================================================
 def space_punc(line):
     """
     SPACE PUNC
```

### Comparing `data-preprocessors-0.8.0/pyproject.toml` & `data-preprocessors-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-preprocessors"
-version = "0.8.0"
+version = "0.9.0"
 description = "An easy to use tool for Data Preprocessing specially for Text Preprocessing"
 license = "MIT"
 authors = ["Md. Musfiqur Rahaman <musfiqur.rahaman@northsouth.edu>"]
 readme = "README.md"
 homepage = "https://github.com/MusfiqDehan/data-preprocessors"
 repository = "https://github.com/MusfiqDehan/data-preprocessors"
 keywords = ["nlp", "data-preprocessors", "data-preprocessing", "text-preprocessing", "data-science"]
```

### Comparing `data-preprocessors-0.8.0/setup.py` & `data-preprocessors-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['data_preprocessors']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'data-preprocessors',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'An easy to use tool for Data Preprocessing specially for Text Preprocessing',
     'long_description': '# Data-Preprocessor\nAn easy to use tool for Data Preprocessing specially for Text Preprocessing\n\n## Installation\nInstall the stable release<br>\nFor windows<br>\n`$ pip install -U data-preprocessors`\n\nFor Linux/WSL2<br>\n`$ pip3 install -U data-preprocessors`\n\n## Quick Start\n```python\nfrom data_preprocessors import text_preprocessor as tp\nsentence = "bla! bla- ?bla ?bla."\nsentence = tp.remove_punc(sentence)\nprint(sentence)\n\n>> bla bla bla bla\n```\n\n',
     'author': 'Md. Musfiqur Rahaman',
     'author_email': 'musfiqur.rahaman@northsouth.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/MusfiqDehan/data-preprocessors',
```

### Comparing `data-preprocessors-0.8.0/PKG-INFO` & `data-preprocessors-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-preprocessors
-Version: 0.8.0
+Version: 0.9.0
 Summary: An easy to use tool for Data Preprocessing specially for Text Preprocessing
 Home-page: https://github.com/MusfiqDehan/data-preprocessors
 License: MIT
 Keywords: nlp,data-preprocessors,data-preprocessing,text-preprocessing,data-science
 Author: Md. Musfiqur Rahaman
 Author-email: musfiqur.rahaman@northsouth.edu
 Requires-Python: >=3.6,<4.0
```


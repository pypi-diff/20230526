# Comparing `tmp/ssg-ada-course-search-0.0.2.tar.gz` & `tmp/ssg-ada-course-search-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssg-ada-course-search-0.0.2.tar", last modified: Thu May 25 23:25:29 2023, max compression
+gzip compressed data, was "ssg-ada-course-search-0.0.3.tar", last modified: Thu May 25 23:35:04 2023, max compression
```

## Comparing `ssg-ada-course-search-0.0.2.tar` & `ssg-ada-course-search-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880950 ssg-ada-course-search-0.0.2/
--rw-r--r--   0 loisji     (501) staff       (20)      370 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/MANIFEST.in
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:25:29.880837 ssg-ada-course-search-0.0.2/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      442 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/README.md
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.879382 ssg-ada-course-search-0.0.2/course_search/
--rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 23:24:37.000000 ssg-ada-course-search-0.0.2/course_search/VERSION
--rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/__init__.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.879723 ssg-ada-course-search-0.0.2/course_search/config/
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/config/__init__.py
--rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:54:13.000000 ssg-ada-course-search-0.0.2/course_search/config/core.py
--rw-r--r--   0 loisji     (501) staff       (20)     1800 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/course_search/course_search.py
--rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/params.yaml
--rw-r--r--   0 loisji     (501) staff       (20)     2978 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/course_search/utils.py
--rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/pyproject.toml
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.878257 ssg-ada-course-search-0.0.2/requirements/
--rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/requirements/requirements.txt
--rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 23:25:29.880985 ssg-ada-course-search-0.0.2/setup.cfg
--rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.2/setup.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880504 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/SOURCES.txt
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/dependency_links.txt
--rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/requires.txt
--rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/top_level.txt
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880649 ssg-ada-course-search-0.0.2/tests/
--rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/tests/test_course_search.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.607259 ssg-ada-course-search-0.0.3/
+-rw-r--r--   0 loisji     (501) staff       (20)      370 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.3/MANIFEST.in
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:35:04.607142 ssg-ada-course-search-0.0.3/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      442 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.3/README.md
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.605731 ssg-ada-course-search-0.0.3/course_search/
+-rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 23:32:06.000000 ssg-ada-course-search-0.0.3/course_search/VERSION
+-rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/__init__.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606017 ssg-ada-course-search-0.0.3/course_search/config/
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/config/__init__.py
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:54:13.000000 ssg-ada-course-search-0.0.3/course_search/config/core.py
+-rw-r--r--   0 loisji     (501) staff       (20)     1858 2023-05-25 23:31:01.000000 ssg-ada-course-search-0.0.3/course_search/course_search.py
+-rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/params.yaml
+-rw-r--r--   0 loisji     (501) staff       (20)     3036 2023-05-25 23:30:46.000000 ssg-ada-course-search-0.0.3/course_search/utils.py
+-rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/pyproject.toml
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.604828 ssg-ada-course-search-0.0.3/requirements/
+-rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/requirements/requirements.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 23:35:04.607295 ssg-ada-course-search-0.0.3/setup.cfg
+-rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.3/setup.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606823 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/SOURCES.txt
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/dependency_links.txt
+-rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/requires.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/top_level.txt
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606946 ssg-ada-course-search-0.0.3/tests/
+-rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/tests/test_course_search.py
```

### Comparing `ssg-ada-course-search-0.0.2/PKG-INFO` & `ssg-ada-course-search-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.2
+Version: 0.0.3
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.2/course_search/config/core.py` & `ssg-ada-course-search-0.0.3/course_search/config/core.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.2/course_search/course_search.py` & `ssg-ada-course-search-0.0.3/course_search/course_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import os
 from botocore.exceptions import NoCredentialsError
 import boto3
 import openai
 from cachetools import cached
 
 from course_search.utils import *
+from course_search.config.core import CONFIG_FILE_PATH
 
-params = yaml.safe_load(open("params.yaml"))
+params = yaml.safe_load(open(CONFIG_FILE_PATH))
 index_file = params["merge_indices"]["indexed_file_path"]
 s3_file_name = params["download"]["s3_file_name"]
 bucket_name = params["download"]["bucket_name"]
 
 api_key = os.environ.get("OPENAI_API_KEY")
 aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID")
 aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY")
```

### Comparing `ssg-ada-course-search-0.0.2/course_search/params.yaml` & `ssg-ada-course-search-0.0.3/course_search/params.yaml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.2/course_search/utils.py` & `ssg-ada-course-search-0.0.3/course_search/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import numpy as np
 from openai.embeddings_utils import get_embedding, cosine_similarity
 import yaml
 import os
+from course_search.config.core import CONFIG_FILE_PATH
 
-params = yaml.safe_load(open("params.yaml"))
+params = yaml.safe_load(open(CONFIG_FILE_PATH))
 # api_key = params["get_embeddings"]["api_token"]
 # api_key = os.environ.get("API_KEY")
 
 api_key = os.environ['OPENAI_API_KEY']
 
 
 def import_csv(file_path, use_cols=None):
```

### Comparing `ssg-ada-course-search-0.0.2/pyproject.toml` & `ssg-ada-course-search-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.2/setup.py` & `ssg-ada-course-search-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/PKG-INFO` & `ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.2
+Version: 0.0.3
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/SOURCES.txt` & `ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*


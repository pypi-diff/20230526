# Comparing `tmp/ssg-ada-course-search-0.0.1.tar.gz` & `tmp/ssg-ada-course-search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssg-ada-course-search-0.0.1.tar", last modified: Thu May 25 22:36:03 2023, max compression
+gzip compressed data, was "ssg-ada-course-search-0.0.2.tar", last modified: Thu May 25 23:25:29 2023, max compression
```

## Comparing `ssg-ada-course-search-0.0.1.tar` & `ssg-ada-course-search-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.691173 ssg-ada-course-search-0.0.1/
--rw-r--r--   0 loisji     (501) staff       (20)      339 2023-05-25 22:34:57.000000 ssg-ada-course-search-0.0.1/MANIFEST.in
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 22:36:03.691052 ssg-ada-course-search-0.0.1/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      247 2023-05-25 22:12:13.000000 ssg-ada-course-search-0.0.1/README.md
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.689611 ssg-ada-course-search-0.0.1/course_search/
--rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/VERSION
--rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/__init__.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.689875 ssg-ada-course-search-0.0.1/course_search/config/
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/config/__init__.py
--rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/config/core.py
--rw-r--r--   0 loisji     (501) staff       (20)     1785 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/course_search.py
--rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/params.yaml
--rw-r--r--   0 loisji     (501) staff       (20)     2978 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/course_search/util.py
--rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/pyproject.toml
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.688982 ssg-ada-course-search-0.0.1/requirements/
--rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/requirements/requirements.txt
--rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 22:36:03.691209 ssg-ada-course-search-0.0.1/setup.cfg
--rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.1/setup.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.690755 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 22:36:03.000000 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      518 2023-05-25 22:36:03.000000 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/SOURCES.txt
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:36:03.000000 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/dependency_links.txt
--rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 22:36:03.000000 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/requires.txt
--rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 22:36:03.000000 ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/top_level.txt
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 22:36:03.690882 ssg-ada-course-search-0.0.1/tests/
--rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.1/tests/test_course_search.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880950 ssg-ada-course-search-0.0.2/
+-rw-r--r--   0 loisji     (501) staff       (20)      370 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/MANIFEST.in
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:25:29.880837 ssg-ada-course-search-0.0.2/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      442 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/README.md
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.879382 ssg-ada-course-search-0.0.2/course_search/
+-rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 23:24:37.000000 ssg-ada-course-search-0.0.2/course_search/VERSION
+-rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/__init__.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.879723 ssg-ada-course-search-0.0.2/course_search/config/
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/config/__init__.py
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:54:13.000000 ssg-ada-course-search-0.0.2/course_search/config/core.py
+-rw-r--r--   0 loisji     (501) staff       (20)     1800 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/course_search/course_search.py
+-rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/course_search/params.yaml
+-rw-r--r--   0 loisji     (501) staff       (20)     2978 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.2/course_search/utils.py
+-rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/pyproject.toml
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.878257 ssg-ada-course-search-0.0.2/requirements/
+-rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/requirements/requirements.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 23:25:29.880985 ssg-ada-course-search-0.0.2/setup.cfg
+-rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.2/setup.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880504 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/SOURCES.txt
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/dependency_links.txt
+-rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/requires.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 23:25:29.000000 ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/top_level.txt
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:25:29.880649 ssg-ada-course-search-0.0.2/tests/
+-rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.2/tests/test_course_search.py
```

### Comparing `ssg-ada-course-search-0.0.1/PKG-INFO` & `ssg-ada-course-search-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.1
+Version: 0.0.2
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.1/course_search/config/core.py` & `ssg-ada-course-search-0.0.2/course_search/config/core.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.1/course_search/course_search.py` & `ssg-ada-course-search-0.0.2/course_search/course_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import yaml
 import os
 from botocore.exceptions import NoCredentialsError
 import boto3
 import openai
 from cachetools import cached
 
-from util import *
+from course_search.utils import *
 
 params = yaml.safe_load(open("params.yaml"))
 index_file = params["merge_indices"]["indexed_file_path"]
 s3_file_name = params["download"]["s3_file_name"]
 bucket_name = params["download"]["bucket_name"]
 
 api_key = os.environ.get("OPENAI_API_KEY")
```

### Comparing `ssg-ada-course-search-0.0.1/course_search/params.yaml` & `ssg-ada-course-search-0.0.2/course_search/params.yaml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.1/course_search/util.py` & `ssg-ada-course-search-0.0.2/course_search/utils.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.1/pyproject.toml` & `ssg-ada-course-search-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.1/setup.py` & `ssg-ada-course-search-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/PKG-INFO` & `ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.1
+Version: 0.0.2
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.1/ssg_ada_course_search.egg-info/SOURCES.txt` & `ssg-ada-course-search-0.0.2/ssg_ada_course_search.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pyproject.toml
 setup.py
 ./requirements/requirements.txt
 course_search/VERSION
 course_search/__init__.py
 course_search/course_search.py
 course_search/params.yaml
-course_search/util.py
+course_search/utils.py
 course_search/config/__init__.py
 course_search/config/core.py
 ssg_ada_course_search.egg-info/PKG-INFO
 ssg_ada_course_search.egg-info/SOURCES.txt
 ssg_ada_course_search.egg-info/dependency_links.txt
 ssg_ada_course_search.egg-info/requires.txt
 ssg_ada_course_search.egg-info/top_level.txt
```


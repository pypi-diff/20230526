# Comparing `tmp/ssg-ada-course-search-0.0.3.tar.gz` & `tmp/ssg-ada-course-search-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssg-ada-course-search-0.0.3.tar", last modified: Thu May 25 23:35:04 2023, max compression
+gzip compressed data, was "ssg-ada-course-search-0.0.4.tar", last modified: Thu May 25 23:58:51 2023, max compression
```

## Comparing `ssg-ada-course-search-0.0.3.tar` & `ssg-ada-course-search-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.607259 ssg-ada-course-search-0.0.3/
--rw-r--r--   0 loisji     (501) staff       (20)      370 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.3/MANIFEST.in
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:35:04.607142 ssg-ada-course-search-0.0.3/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      442 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.3/README.md
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.605731 ssg-ada-course-search-0.0.3/course_search/
--rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 23:32:06.000000 ssg-ada-course-search-0.0.3/course_search/VERSION
--rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/__init__.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606017 ssg-ada-course-search-0.0.3/course_search/config/
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/config/__init__.py
--rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:54:13.000000 ssg-ada-course-search-0.0.3/course_search/config/core.py
--rw-r--r--   0 loisji     (501) staff       (20)     1858 2023-05-25 23:31:01.000000 ssg-ada-course-search-0.0.3/course_search/course_search.py
--rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/course_search/params.yaml
--rw-r--r--   0 loisji     (501) staff       (20)     3036 2023-05-25 23:30:46.000000 ssg-ada-course-search-0.0.3/course_search/utils.py
--rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/pyproject.toml
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.604828 ssg-ada-course-search-0.0.3/requirements/
--rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/requirements/requirements.txt
--rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 23:35:04.607295 ssg-ada-course-search-0.0.3/setup.cfg
--rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.3/setup.py
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606823 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/
--rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/PKG-INFO
--rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/SOURCES.txt
--rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/dependency_links.txt
--rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/requires.txt
--rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 23:35:04.000000 ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/top_level.txt
-drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:35:04.606946 ssg-ada-course-search-0.0.3/tests/
--rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.3/tests/test_course_search.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.330880 ssg-ada-course-search-0.0.4/
+-rw-r--r--   0 loisji     (501) staff       (20)      370 2023-05-25 23:24:12.000000 ssg-ada-course-search-0.0.4/MANIFEST.in
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:58:51.330769 ssg-ada-course-search-0.0.4/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      531 2023-05-25 23:57:47.000000 ssg-ada-course-search-0.0.4/README.md
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.329229 ssg-ada-course-search-0.0.4/course_search/
+-rw-r--r--   0 loisji     (501) staff       (20)        5 2023-05-25 23:57:47.000000 ssg-ada-course-search-0.0.4/course_search/VERSION
+-rw-r--r--   0 loisji     (501) staff       (20)      150 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/course_search/__init__.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.329676 ssg-ada-course-search-0.0.4/course_search/config/
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/course_search/config/__init__.py
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 22:54:13.000000 ssg-ada-course-search-0.0.4/course_search/config/core.py
+-rw-r--r--   0 loisji     (501) staff       (20)     2313 2023-05-25 23:57:47.000000 ssg-ada-course-search-0.0.4/course_search/course_search.py
+-rw-r--r--   0 loisji     (501) staff       (20)      554 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/course_search/params.yaml
+-rw-r--r--   0 loisji     (501) staff       (20)     3036 2023-05-25 23:30:46.000000 ssg-ada-course-search-0.0.4/course_search/utils.py
+-rw-r--r--   0 loisji     (501) staff       (20)     1941 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/pyproject.toml
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.328398 ssg-ada-course-search-0.0.4/requirements/
+-rw-r--r--   0 loisji     (501) staff       (20)      169 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/requirements/requirements.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       38 2023-05-25 23:58:51.330916 ssg-ada-course-search-0.0.4/setup.cfg
+-rw-r--r--   0 loisji     (501) staff       (20)     2289 2023-05-25 22:35:28.000000 ssg-ada-course-search-0.0.4/setup.py
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.330433 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/
+-rw-r--r--   0 loisji     (501) staff       (20)      870 2023-05-25 23:58:51.000000 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/PKG-INFO
+-rw-r--r--   0 loisji     (501) staff       (20)      519 2023-05-25 23:58:51.000000 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/SOURCES.txt
+-rw-r--r--   0 loisji     (501) staff       (20)        1 2023-05-25 23:58:51.000000 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/dependency_links.txt
+-rw-r--r--   0 loisji     (501) staff       (20)      170 2023-05-25 23:58:51.000000 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/requires.txt
+-rw-r--r--   0 loisji     (501) staff       (20)       14 2023-05-25 23:58:51.000000 ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/top_level.txt
+drwxr-xr-x   0 loisji     (501) staff       (20)        0 2023-05-25 23:58:51.330567 ssg-ada-course-search-0.0.4/tests/
+-rw-r--r--   0 loisji     (501) staff       (20)      294 2023-05-25 22:12:57.000000 ssg-ada-course-search-0.0.4/tests/test_course_search.py
```

### Comparing `ssg-ada-course-search-0.0.3/PKG-INFO` & `ssg-ada-course-search-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.3
+Version: 0.0.4
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.3/course_search/config/core.py` & `ssg-ada-course-search-0.0.4/course_search/config/core.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.3/course_search/course_search.py` & `ssg-ada-course-search-0.0.4/course_search/course_search.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,24 @@
     catalog_df['embedding'] = catalog_df.embedding.apply(eval).apply(np.array)
     return catalog_df
 
 def file_check(index_file):
     if not os.path.exists(index_file):
         download_file(bucket_name=bucket_name, file_key=s3_file_name, local_dir=index_file)
     
-def search_for_courses(query, top_n=5, threshold=0.81, index_file=index_file):
+def search_for_courses(query, index_file, top_n=5, threshold=0.81):
+    """
+    input:
+        :query: str, search query for courses
+        :index_file: csv, collection of courses with ada gen2 embedding within
+        :top_n: int, optional param, default returns top 5 courses
+        :threshold: float, optional param, default set to 0.81 (returns courses that are at least 81% similar to search query)
+    output:
+        :result_json: json, contains course details and similarity score between search and course returned
+    """
     file_check(index_file)
     
     # Load in the course catalog with embeddings
     catalog_df = load_index(index_file=index_file)
     print("file loaded")
 
     # call util function search_courses to return top matches in json
```

### Comparing `ssg-ada-course-search-0.0.3/course_search/params.yaml` & `ssg-ada-course-search-0.0.4/course_search/params.yaml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.3/course_search/utils.py` & `ssg-ada-course-search-0.0.4/course_search/utils.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.3/pyproject.toml` & `ssg-ada-course-search-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.3/setup.py` & `ssg-ada-course-search-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/PKG-INFO` & `ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssg-ada-course-search
-Version: 0.0.3
+Version: 0.0.4
 Summary: SSG course search using OpenAI Ada Gen2 Text Embedding model
 Home-page: https://github.com/LoisTJ/ada-course-search-package
 Author: LoisJi
 Author-email: lois@dsaid.gov.sg
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssg-ada-course-search-0.0.3/ssg_ada_course_search.egg-info/SOURCES.txt` & `ssg-ada-course-search-0.0.4/ssg_ada_course_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*


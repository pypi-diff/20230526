# Comparing `tmp/pyopencga-2.8.1.tar.gz` & `tmp/pyopencga-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencga-2.8.1.tar", last modified: Thu May 11 09:36:35 2023, max compression
+gzip compressed data, was "pyopencga-2.9.0.tar", last modified: Fri May 26 18:35:57 2023, max compression
```

## Comparing `pyopencga-2.8.1.tar` & `pyopencga-2.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.872818 pyopencga-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-11 09:35:59.000000 pyopencga-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-11 09:36:35.872818 pyopencga-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-11 09:35:59.000000 pyopencga-2.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.868818 pyopencga-2.8.1/pyopencga/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/opencga_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/opencga_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.872818 pyopencga-2.8.1/pyopencga/rest_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/_parent_rest_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_clients/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/alignment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/clinical_analysis_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/clinical_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/cohort_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/disease_panel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/family_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/file_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/ga4gh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/individual_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/job_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/project_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/sample_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/study_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/user_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/variant_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-11 09:36:00.000000 pyopencga-2.8.1/pyopencga/rest_clients/variant_operation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/rest_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-11 09:35:59.000000 pyopencga-2.8.1/pyopencga/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 09:36:35.868818 pyopencga-2.8.1/pyopencga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 09:36:35.000000 pyopencga-2.8.1/pyopencga.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 09:36:35.872818 pyopencga-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-11 09:35:59.000000 pyopencga-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:35:57.618383 pyopencga-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 18:34:42.000000 pyopencga-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-26 18:35:57.618383 pyopencga-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-26 18:34:42.000000 pyopencga-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:35:57.602383 pyopencga-2.9.0/pyopencga/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 18:34:43.000000 pyopencga-2.9.0/pyopencga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-26 18:34:43.000000 pyopencga-2.9.0/pyopencga/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 18:34:43.000000 pyopencga-2.9.0/pyopencga/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-26 18:34:43.000000 pyopencga-2.9.0/pyopencga/opencga_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-26 18:34:43.000000 pyopencga-2.9.0/pyopencga/opencga_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:35:57.618383 pyopencga-2.9.0/pyopencga/rest_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/_parent_rest_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/alignment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52128 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/clinical_analysis_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52556 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/clinical_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/cohort_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/disease_panel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/family_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26628 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/file_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/ga4gh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/individual_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_clients/job_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/meta_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/sample_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/study_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/user_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/variant_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25700 2023-05-26 18:34:45.000000 pyopencga-2.9.0/pyopencga/rest_clients/variant_operation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/rest_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-26 18:34:44.000000 pyopencga-2.9.0/pyopencga/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:35:57.606383 pyopencga-2.9.0/pyopencga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-26 18:35:57.000000 pyopencga-2.9.0/pyopencga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-26 18:35:57.000000 pyopencga-2.9.0/pyopencga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:35:57.000000 pyopencga-2.9.0/pyopencga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 18:35:57.000000 pyopencga-2.9.0/pyopencga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 18:35:57.000000 pyopencga-2.9.0/pyopencga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:35:57.618383 pyopencga-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-26 18:34:42.000000 pyopencga-2.9.0/setup.py
```

### Comparing `pyopencga-2.8.1/LICENSE` & `pyopencga-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/PKG-INFO` & `pyopencga-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.8.1
+Version: 2.9.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.8.1/README.rst` & `pyopencga-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/commons.py` & `pyopencga-2.9.0/pyopencga/commons.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/opencga_client.py` & `pyopencga-2.9.0/pyopencga/opencga_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/opencga_config.py` & `pyopencga-2.9.0/pyopencga/opencga_config.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/_parent_rest_clients.py` & `pyopencga-2.9.0/pyopencga/rest_clients/_parent_rest_clients.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/admin_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/admin_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/alignment_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/alignment_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/clinical_analysis_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/clinical_analysis_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/clinical_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/clinical_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/cohort_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/cohort_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/disease_panel_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/disease_panel_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/family_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/family_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/file_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/file_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/ga4gh_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/ga4gh_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/individual_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/individual_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/job_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/job_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/meta_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/meta_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/project_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/project_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/sample_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/sample_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/study_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/study_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/user_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/user_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/variant_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/variant_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_clients/variant_operation_client.py` & `pyopencga-2.9.0/pyopencga/rest_clients/variant_operation_client.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/rest_response.py` & `pyopencga-2.9.0/pyopencga/rest_response.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga/retry.py` & `pyopencga-2.9.0/pyopencga/retry.py`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/pyopencga.egg-info/PKG-INFO` & `pyopencga-2.9.0/pyopencga.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencga
-Version: 2.8.1
+Version: 2.9.0
 Summary: A REST client for OpenCGA REST web services
 Home-page: https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
 Author: David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil
 Author-email: david.gomez@mgviz.org, pmarin@kanteron.com, dp529@cam.ac.uk
 License: Apache Software License
 Project-URL: Documentation, http://docs.opencb.org/display/opencga/Python
 Project-URL: Source, https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga
```

### Comparing `pyopencga-2.8.1/pyopencga.egg-info/SOURCES.txt` & `pyopencga-2.9.0/pyopencga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopencga-2.8.1/setup.py` & `pyopencga-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyopencga',
-    version='2.8.1',
+    version='2.9.0',
     description='A REST client for OpenCGA REST web services',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/opencb/opencga/tree/develop/opencga-client/src/main/python/pyopencga',
     packages=['pyopencga', 'pyopencga.rest_clients'],
     license='Apache Software License',
     author='David Gomez-Peregrina, Pablo Marin-Garcia, Daniel Perez-Gil',
```

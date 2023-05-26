# Comparing `tmp/flexmeasures-client-0.1.0.tar.gz` & `tmp/flexmeasures-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexmeasures-client-0.1.0.tar", last modified: Wed May 24 15:37:04 2023, max compression
+gzip compressed data, was "flexmeasures-client-0.1.1.tar", last modified: Fri May 26 13:38:46 2023, max compression
```

## Comparing `flexmeasures-client-0.1.0.tar` & `flexmeasures-client-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.588541 flexmeasures-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.560541 flexmeasures-client-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.572541 flexmeasures-client-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-24 15:37:04.588541 flexmeasures-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.580541 flexmeasures-client-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.580541 flexmeasures-client-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-24 15:37:04.588541 flexmeasures-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.564541 flexmeasures-client-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.580541 flexmeasures-client-0.1.0/src/flexmeasures_client/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/src/flexmeasures_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/src/flexmeasures_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/src/flexmeasures_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/src/flexmeasures_client/response_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.584541 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 15:37:04.000000 flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:04.588541 flexmeasures-client-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-24 15:36:21.000000 flexmeasures-client-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.250332 flexmeasures-client-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.258333 flexmeasures-client-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.262333 flexmeasures-client-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.262333 flexmeasures-client-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 13:38:46.270334 flexmeasures-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.250332 flexmeasures-client-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/src/flexmeasures_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/src/flexmeasures_client/response_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:38:45.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 13:38:46.000000 flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:38:46.266334 flexmeasures-client-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 13:38:07.000000 flexmeasures-client-0.1.1/tox.ini
```

### Comparing `flexmeasures-client-0.1.0/.coveragerc` & `flexmeasures-client-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/.github/workflows/ci.yml` & `flexmeasures-client-0.1.1/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 name: tests
 
 on:
   push:
     # Avoid using all the resources/limits available by checking only
     # relevant branches and tags. Other branches can be checked via PRs.
     branches: [main]
-    tags: 'v[0-9]+\.[0-9]+\.[0-9]'  # Match tags that resemble a version
+    tags: 'v[0-9]+\.[0-9]+\.[0-9]+'  # Match tags that resemble a version
   pull_request:  # Run in every PR
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
```

### Comparing `flexmeasures-client-0.1.0/.gitignore` & `flexmeasures-client-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/.pre-commit-config.yaml` & `flexmeasures-client-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/.readthedocs.yml` & `flexmeasures-client-0.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/CONTRIBUTING.rst` & `flexmeasures-client-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/LICENSE.txt` & `flexmeasures-client-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/PKG-INFO` & `flexmeasures-client-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async client to connect to the FlexMeasures API
 Home-page: https://github.com/FlexMeasures/flexmeasures-client
 Author: Flexmeasures
 Author-email: info@seita.nl
 License: APACHE
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flexmeasures-client-0.1.0/README.rst` & `flexmeasures-client-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/docs/Makefile` & `flexmeasures-client-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/docs/conf.py` & `flexmeasures-client-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/docs/index.rst` & `flexmeasures-client-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/setup.cfg` & `flexmeasures-client-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/setup.py` & `flexmeasures-client-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/src/flexmeasures_client/client.py` & `flexmeasures-client-0.1.1/src/flexmeasures_client/client.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/src/flexmeasures_client/response_handling.py` & `flexmeasures-client-0.1.1/src/flexmeasures_client/response_handling.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/PKG-INFO` & `flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexmeasures-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async client to connect to the FlexMeasures API
 Home-page: https://github.com/FlexMeasures/flexmeasures-client
 Author: Flexmeasures
 Author-email: info@seita.nl
 License: APACHE
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flexmeasures-client-0.1.0/src/flexmeasures_client.egg-info/SOURCES.txt` & `flexmeasures-client-0.1.1/src/flexmeasures_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/tests/test_client.py` & `flexmeasures-client-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `flexmeasures-client-0.1.0/tox.ini` & `flexmeasures-client-0.1.1/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/klops-0.0.3.tar.gz` & `tmp/klops-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klops-0.0.3.tar", last modified: Tue Sep 13 01:03:02 2022, max compression
+gzip compressed data, was "klops-0.0.4.tar", last modified: Fri May 26 10:02:12 2023, max compression
```

## Comparing `klops-0.0.3.tar` & `klops-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,78 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.384960 klops-0.0.3/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       80 2022-09-12 05:52:52.000000 klops-0.0.3/Containerfile
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      166 2022-09-13 00:09:41.000000 klops-0.0.3/HISTORY.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1207 2022-09-12 05:52:52.000000 klops-0.0.3/LICENSE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       81 2022-09-12 05:52:52.000000 klops-0.0.3/MANIFEST.in
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5404 2022-09-13 01:03:02.384960 klops-0.0.3/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5133 2022-09-13 00:09:41.000000 klops-0.0.3/README.md
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        6 2022-09-13 01:02:42.000000 klops-0.0.3/klops/VERSION
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2022-09-12 05:52:52.000000 klops-0.0.3/klops/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      287 2022-09-12 05:52:52.000000 klops-0.0.3/klops/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/experiment/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      106 2022-09-12 05:52:52.000000 klops-0.0.3/klops/experiment/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2192 2022-09-12 05:52:52.000000 klops-0.0.3/klops/experiment/exception.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    14828 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/experiment.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/experiment/runner/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      282 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/runner/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3918 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/runner/base.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2844 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/runner/basic.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3052 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/runner/gridsearch.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3739 2022-09-13 00:08:01.000000 klops-0.0.3/klops/experiment/runner/hyperopt.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/seldon_core/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      110 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/__init__.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/seldon_core/auth/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      188 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/auth/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1342 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/auth/default.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1214 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/auth/gke.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      706 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/auth/schema.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     6667 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/deployment.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      950 2022-09-12 05:52:52.000000 klops-0.0.3/klops/seldon_core/exception.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops/templates/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      575 2022-09-12 05:52:52.000000 klops-0.0.3/klops/templates/deployment_template.json
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.384960 klops-0.0.3/klops/versioning/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      124 2022-09-12 05:52:52.000000 klops-0.0.3/klops/versioning/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      596 2022-09-12 05:52:52.000000 klops-0.0.3/klops/versioning/helper.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3743 2022-09-12 05:52:52.000000 klops-0.0.3/klops/versioning/versioning.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.380959 klops-0.0.3/klops.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5404 2022-09-13 01:03:02.000000 klops-0.0.3/klops.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      946 2022-09-13 01:03:02.000000 klops-0.0.3/klops.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2022-09-13 01:03:02.000000 klops-0.0.3/klops.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      248 2022-09-13 01:03:02.000000 klops-0.0.3/klops.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        6 2022-09-13 01:03:02.000000 klops-0.0.3/klops.egg-info/top_level.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2022-09-13 01:03:02.384960 klops-0.0.3/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1404 2022-09-13 01:02:51.000000 klops-0.0.3/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.384960 klops-0.0.3/tests/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2022-09-12 05:52:52.000000 klops-0.0.3/tests/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      424 2022-09-12 05:52:52.000000 klops-0.0.3/tests/conftest.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2022-09-13 01:03:02.384960 klops-0.0.3/tests/seldon_core/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3881 2022-09-12 05:52:52.000000 klops-0.0.3/tests/seldon_core/deployment_test.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.999371 klops-0.0.4/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       80 2023-05-08 10:49:09.000000 klops-0.0.4/Containerfile
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5003 2023-05-08 10:49:09.000000 klops-0.0.4/HISTORY.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1207 2023-05-08 10:49:09.000000 klops-0.0.4/LICENSE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       81 2023-05-08 10:49:09.000000 klops-0.0.4/MANIFEST.in
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5404 2023-05-26 10:02:11.999371 klops-0.0.4/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5133 2023-05-08 10:49:09.000000 klops-0.0.4/README.md
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.983370 klops-0.0.4/klops/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        6 2023-05-26 10:02:00.000000 klops-0.0.4/klops/VERSION
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-05-08 10:49:09.000000 klops-0.0.4/klops/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-08 10:49:09.000000 klops-0.0.4/klops/__main__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.987370 klops-0.0.4/klops/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      156 2023-05-26 09:11:59.000000 klops-0.0.4/klops/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-26 09:12:57.000000 klops-0.0.4/klops/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      687 2023-05-08 10:49:09.000000 klops-0.0.4/klops/cli.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      278 2023-05-08 10:49:09.000000 klops-0.0.4/klops/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.987370 klops-0.0.4/klops/deployment/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3015 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/__init__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.991371 klops-0.0.4/klops/deployment/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2449 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5920 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/__pycache__/deployment.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1968 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/__pycache__/exception.cpython-39.pyc
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.991371 klops-0.0.4/klops/deployment/auth/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      188 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/auth/__init__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.991371 klops-0.0.4/klops/deployment/auth/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      360 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1216 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/auth/__pycache__/default.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1509 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/auth/__pycache__/gke.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3680 2023-05-26 09:12:00.000000 klops-0.0.4/klops/deployment/auth/__pycache__/schema.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      851 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/auth/default.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1099 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/auth/gke.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3444 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/auth/schema.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     6428 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/deployment.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1701 2023-05-08 10:49:09.000000 klops-0.0.4/klops/deployment/exception.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.991371 klops-0.0.4/klops/experiment/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       98 2023-05-11 14:57:33.000000 klops-0.0.4/klops/experiment/__init__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.991371 klops-0.0.4/klops/experiment/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      279 2023-05-26 09:11:59.000000 klops-0.0.4/klops/experiment/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3221 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/__pycache__/exception.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    12023 2023-05-26 09:11:59.000000 klops-0.0.4/klops/experiment/__pycache__/experiment.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2094 2023-05-08 10:49:09.000000 klops-0.0.4/klops/experiment/exception.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    14346 2023-05-11 15:03:46.000000 klops-0.0.4/klops/experiment/experiment.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/klops/experiment/runner/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      273 2023-05-08 10:49:09.000000 klops-0.0.4/klops/experiment/runner/__init__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/klops/experiment/runner/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      458 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/runner/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3832 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/runner/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3094 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/runner/__pycache__/basic.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3200 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/runner/__pycache__/gridsearch.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4566 2023-05-26 09:12:00.000000 klops-0.0.4/klops/experiment/runner/__pycache__/hyperopt.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3707 2023-05-08 10:49:09.000000 klops-0.0.4/klops/experiment/runner/base.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3056 2023-05-15 07:07:23.000000 klops-0.0.4/klops/experiment/runner/basic.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3216 2023-05-08 10:49:09.000000 klops-0.0.4/klops/experiment/runner/gridsearch.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4606 2023-05-16 10:13:56.000000 klops-0.0.4/klops/experiment/runner/hyperopt.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/klops/templates/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      575 2023-05-08 10:49:09.000000 klops-0.0.4/klops/templates/deployment_template.json
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/klops/versioning/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      115 2023-05-08 10:49:09.000000 klops-0.0.4/klops/versioning/__init__.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/klops/versioning/__pycache__/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      298 2023-05-26 09:12:56.000000 klops-0.0.4/klops/versioning/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      812 2023-05-26 09:12:57.000000 klops-0.0.4/klops/versioning/__pycache__/helper.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    14237 2023-05-26 09:12:56.000000 klops-0.0.4/klops/versioning/__pycache__/versioning.cpython-39.pyc
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      564 2023-05-08 10:49:09.000000 klops-0.0.4/klops/versioning/helper.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    13725 2023-05-08 10:49:09.000000 klops-0.0.4/klops/versioning/versioning.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.987370 klops-0.0.4/klops.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     5404 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2086 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       46 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/entry_points.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      254 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        6 2023-05-26 10:02:11.000000 klops-0.0.4/klops.egg-info/top_level.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-26 10:02:11.999371 klops-0.0.4/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1574 2023-05-26 09:50:24.000000 klops-0.0.4/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.995371 klops-0.0.4/tests/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        0 2023-05-08 10:49:09.000000 klops-0.0.4/tests/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      424 2023-05-08 10:49:09.000000 klops-0.0.4/tests/conftest.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-26 10:02:11.999371 klops-0.0.4/tests/seldon_core/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     4020 2023-05-08 10:49:09.000000 klops-0.0.4/tests/seldon_core/deployment_test.py
```

### Comparing `klops-0.0.3/LICENSE` & `klops-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `klops-0.0.3/PKG-INFO` & `klops-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Klops: Koin Machine Learning Ops
 Home-page: https://gitlab-engineering.koinworks.com/data-team/klops/
 Author: Koinworks Data Team
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -14,15 +14,15 @@
 
 <p align="center">
     <strong>Build your end-to-end machine learning projects within one tool.</strong>
 </p>
 
 <p align="center">
     <a href="#" title="PyPi Version"><img src="https://img.shields.io/badge/PyPi-v.0.4.8-blue"></a>
-    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.6%2B-green"></a>
+    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.8%2B-green"></a>
     <!-- <a href="https://www.codacy.com/gh/ml-tooling/lazydocs/dashboard" title="Codacy Analysis"><img src="https://app.codacy.com/project/badge/Grade/1c8ad486ce9547b6b713cce7ca1d1ec3"></a> -->
     <!-- <a href="" title="Build status"><img src="https://img.shields.io/github/workflow/status/ml-tooling/lazydocs/build-pipeline?style=flat"></a> -->
     <a href="#" title="Project License"><img src="https://img.shields.io/badge/License-Koinworks-red"></a>
     <!-- <a href="https://gitter.im/ml-tooling/lazydocs" title="Chat on Gitter"><img src="https://badges.gitter.im/ml-tooling/lazydocs.svg"></a> -->
     <a href="https://twitter.com/mltooling" title="ML Tooling on Twitter"><img src="https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: klops Version: 0.0.3 Summary: Klops: Koin Machine
+Metadata-Version: 2.1 Name: klops Version: 0.0.4 Summary: Klops: Koin Machine
 Learning Ops Home-page: https://gitlab-engineering.koinworks.com/data-team/
 klops/ Author: Koinworks Data Team Description-Content-Type: text/markdown
 Provides-Extra: test License-File: LICENSE
                         ****** Klops: Koin MLOps ******
        Build your end-to-end machine learning projects within one tool.
 [https://img.shields.io/badge/PyPi-v.0.4.8-blue] [https://img.shields.io/badge/
- Python-3.6%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
+ Python-3.8%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
 [https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social]
         Getting_Started â¢ Documentation â¢ Support â¢ Contribution
 Klops is an End-to-End machine learning development pipeline ops. Its build on
 top of Seldon Core, MLflow and DVC. The goal of this project is to make easier
 for Data Scientist to develop, maintain, log their experiments and deploy their
 machine learning projects. ## Prerequisites - Seldon Core Installed on your
 Kubernetes cluster. Guidance [here](https://docs.seldon.io/projects/seldon-
```

### Comparing `klops-0.0.3/README.md` & `klops-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 <p align="center">
     <strong>Build your end-to-end machine learning projects within one tool.</strong>
 </p>
 
 <p align="center">
     <a href="#" title="PyPi Version"><img src="https://img.shields.io/badge/PyPi-v.0.4.8-blue"></a>
-    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.6%2B-green"></a>
+    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.8%2B-green"></a>
     <!-- <a href="https://www.codacy.com/gh/ml-tooling/lazydocs/dashboard" title="Codacy Analysis"><img src="https://app.codacy.com/project/badge/Grade/1c8ad486ce9547b6b713cce7ca1d1ec3"></a> -->
     <!-- <a href="" title="Build status"><img src="https://img.shields.io/github/workflow/status/ml-tooling/lazydocs/build-pipeline?style=flat"></a> -->
     <a href="#" title="Project License"><img src="https://img.shields.io/badge/License-Koinworks-red"></a>
     <!-- <a href="https://gitter.im/ml-tooling/lazydocs" title="Chat on Gitter"><img src="https://badges.gitter.im/ml-tooling/lazydocs.svg"></a> -->
     <a href="https://twitter.com/mltooling" title="ML Tooling on Twitter"><img src="https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                         ****** Klops: Koin MLOps ******
        Build your end-to-end machine learning projects within one tool.
 [https://img.shields.io/badge/PyPi-v.0.4.8-blue] [https://img.shields.io/badge/
- Python-3.6%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
+ Python-3.8%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
 [https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social]
         Getting_Started â¢ Documentation â¢ Support â¢ Contribution
 Klops is an End-to-End machine learning development pipeline ops. Its build on
 top of Seldon Core, MLflow and DVC. The goal of this project is to make easier
 for Data Scientist to develop, maintain, log their experiments and deploy their
 machine learning projects. ## Prerequisites - Seldon Core Installed on your
 Kubernetes cluster. Guidance [here](https://docs.seldon.io/projects/seldon-
```

### Comparing `klops-0.0.3/klops/experiment/exception.py` & `klops-0.0.4/klops/experiment/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""_summary_ Experiment exception module.
+"""Experiment exception module.
 
 Put all the exception handlers here.
 """
 
 class ExperimentFailedException(Exception):
     """Experiment Failed Exception
 
     Raised when the experiment got failed.
     """
 
     def __init__(self, message: str, *args: object) -> None:
-        """_summary_ The Experiment Failed Constructor
+        """The Experiment Failed Constructor
 
         Message would store the root causes.
         Args:
             message (str): _description_
         """
         self.message = message
         super(ExperimentFailedException, self).__init__(*args)
 
     def __str__(self):
         return self.message
 
 
 class InvalidArgumentsException(ValueError):
-    """_summary_ Invalid Arguments Passed
+    """Invalid Arguments Passed
 
     Raised when the given arguments are invalid.
     """
 
     def __init__(self, message: str,*args: object) -> None:
-        """_summary_ The Exception Constructor
+        """The Exception Constructor
 
         Args:
-            message (str): _description_ message that would be displayed to the user.
+            message (str): message that would be displayed to the user.
         """
         self.message = message
         super(InvalidArgumentsException, self).__init__(*args)
 
     def __str__(self) -> str:
         return self.message
 
@@ -45,37 +45,37 @@
 class LogMetricException(Exception):
     """Log Metric Exception
 
     Raised when the Logging the metrics are failed.
     """
 
     def __init__(self, message: str, *args: object) -> None:
-        """_summary_ The Log Metric Exception Constructor
+        """The Log Metric Exception Constructor
 
         Message would store the root causes.
         Args:
             message (str): _description_
         """
         self.message = message
         super(LogMetricException, self).__init__(*args)
 
     def __str__(self):
         return self.message
 
 
 class UnknownExperimentTunerTypeException(ValueError):
-    """_summary_ Unknown Experiment Tunner Exception
+    """Unknown Experiment Tunner Exception
 
     Raised when the tuner is not one of `default` | `gridsearch` | `hyperopt`.
     """
 
     def __init__(self, message, *args: object) -> None:
-        """_summary_ The Exception Constructor.
+        """The Exception Constructor.
 
         Args:
-            message (_type_): _description_ The Exception message would be displayed.
+            message (_type_): The Exception message would be displayed.
         """
         self.message = message
         super(UnknownExperimentTunerTypeException, self).__init__(*args)
 
     def __str__(self) -> str:
         return self.message
```

### Comparing `klops-0.0.3/klops/experiment/experiment.py` & `klops-0.0.4/klops/experiment/experiment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Main module for Klops MLflow Experiment.
 """
 
 from __future__ import annotations
+from datetime import datetime
 import os
 from typing import Any, Dict, List, Tuple, Union
 import warnings
 
 import joblib
 
 from kubernetes.client import ApiException
@@ -15,96 +16,108 @@
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 import klops
 from klops.experiment.exception import ExperimentFailedException, \
     UnknownExperimentTunerTypeException
-from klops.seldon_core import SeldonDeployment
+from klops.experiment.runner.base import BaseRunner
+from klops.deployment import Deployment
 from klops.experiment.runner import BasicRunner, GridsearchRunner, HyperOptRunner
-from klops.seldon_core.auth.schema import AbstractKubernetesAuth
-from klops.seldon_core.exception import SeldonDeploymentException
+from klops.deployment.auth.schema import AbstractKubernetesAuth
+from klops.deployment.exception import DeploymentException
 
 KLOPS_PATH = klops.__path__[0]
 
 warnings.filterwarnings(action="ignore")
 
 
-class Experiment:
-    """_summary_
+class Experiment(MlflowClient):
+    """
     Main class for MLflow Experiment. This class would wrap the MLFlow client and \
     it's experiments features.
     """
 
+    best: Dict = {}
+    _tracking_uri: str = ""
+
     def __init__(self, name: str,
                  tracking_uri: str = os.getenv("MLFLOW_TRACKING_URI", None)) -> None:
-        """_summary_
+        """
         The Experiment class constructor. Every arguments sets here, \
         would be implemented to all experiments with the same name.
         Args:
-            name (str): _description_ The experiment name. Example: "my-classification-experiment"
-            tracking_uri (str): _description_ The MLflow experiment tracking uri. \
+            name (str): The experiment name. Example: "my-classification-experiment"
+            tracking_uri (str): The MLflow experiment tracking uri. \
                 Its our MLflow Tracking server URI. Example: "http://<your-mlflow-host>:<port>"
         """
         self.name = name
         if tracking_uri in ["", None]:
             raise ValueError("Tracking uri must be specified in the configuration.")
-        self.tracking_uri = tracking_uri
+        # self.tracking_uri = tracking_uri
         os.environ["MLFLOW_TRACKING_URI"] = tracking_uri
-        self.mlflow_client = MlflowClient()
+
 
         mlflow.set_experiment(name)
 
+    # @property
+    # def tracking_uri(self):
+    #     return self._tracking_uri
+
     def start(self,
               classifier: Any,
               x_train: Union[np.ndarray, pd.DataFrame, List[Dict]],
               y_train: Union[np.ndarray, pd.DataFrame, List],
+              save_best_fit: bool = False,
               dataset_auto_split: bool = True,
-              x_test: Union[np.ndarray, pd.DataFrame, List[Dict]] = [],
-              y_test: Union[np.ndarray, pd.DataFrame, List] = [],
+              x_test: Union[np.ndarray, pd.DataFrame, List[Dict], None] = None,
+              y_test: Union[np.ndarray, pd.DataFrame, List, None] = None,
               test_size: float = .2,
               random_state: int = 11,
               tuner: str = None,
               tuner_args: Dict = {},
               metrices: Dict = {
                   "mean_squared_error": {},
                   "root_mean_squared_error": {"squared": False}},
               **kwargs: Any) -> Experiment:
-        """_summary_
+        """
         Start the experiment with given arguments.
 
         Args:
-            classifier (Any): _description_ The classifier pointer class. \
+            classifier (Any): The classifier pointer class. \
                 Example: sklearn.naive_bayes.GaussianNB
             x_train (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
-                _description_ The input features with 2 Dimensional Array like.
+                The input features with 2 Dimensional Array like.
             y_train (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
-                _description_ The output mapping.
-            dataset_auto_split (bool):  Whether to automatically split the dataset into train-test pairs.
-            x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_ \
+                The output mapping.
+            dataset_auto_split (bool): Whether to automatically split the dataset into train-test pairs.
+            x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
                 The input test value. Only usable when the dataset_auto_split flag is False.
-            y_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_ \
+            y_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
                 The output test value. Only usable when the dataset_auto_split flag is False.
             test_size (float): The split size of the test data.
             random_state (int): The number of random state.
-            tuner (str): _description_ The tuner could be one of (default | hyperopt | gridsearch). \
+            tuner (str): The tuner could be one of (default | hyperopt | gridsearch). \
                 Defaults to None.
-            tuner_args (Dict, optional): _description_. Defaults to {}. Tunner keyworded arguments. \
+            tuner_args (Dict, optional): Defaults to {}. Tunner keyworded arguments. \
                 A Dictionary contains key-value pairs set of hyper parameters.
-            metrices (_type_, optional): _description_. Defaults to \
+            metrices (_type_, optional): Defaults to \
                 { "mean_squared_error": {}, "root_mean_squared_error": {"squared": True}}. \
                 The sklearn metrices. All metrices method name could be seen here: \
                 https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
 
         Raises:
-            ValueError: _description_ Raised when conditions are not met.
+            ValueError: Raised when conditions are not met.
 
         Returns:
-            Experiment: _description_ The Experiment instance class.
+            Experiment: The Experiment instance class.
         """
+
+        runner: BaseRunner = None
+
         try:
 
             tags = {}
             if "tags" in kwargs:
                 if isinstance(kwargs["tags"], Dict):
                     tags = kwargs["tags"]
                     del kwargs["tags"]
@@ -160,108 +173,101 @@
             else:
                 raise ValueError("Unknown Experiment tuner type exception. \
                         It should be on of: 'default'|'gridsearch'|'hyperopt'.")
         except ValueError as value_error:
             raise UnknownExperimentTunerTypeException(
                 message=str(value_error)) from value_error
 
-        runner.run(metrices, **kwargs)
+        best_result = runner.run(metrices, **kwargs)
+        self.best = best_result
+
+        if save_best_fit:
+            self.store_best_fit(classifier.__class__.__name__, best_result.get("model"))
 
         return self
 
+    def store_best_fit(self, estimator_name: str, model: Any):
+        """Save the best fit model from training phase.
+        """
+        best_running_time = datetime.now().strftime("%Y-%m-%d_%H:%M:%S")
+        self.store_artifact(
+            model, f"./{self.name}_{estimator_name}_{best_running_time}.pkl", "models/")
+
     def split_train_test(self,
                          x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                          y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                          test_size: float = .2, random_state: int = 11) -> Tuple:
-        """_summary_ Split Data Into Train - Test Pair.
+        """Split Data Into Train - Test Pair.
 
         Args:
-            x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_ The features of the training sets.
-            y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_ The target class.
-            test_size (float, optional): _description_. Defaults to .2. The test size in float.
-            random_state (int, optional): _description_. Defaults to 11. The randomize state.
+            x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): The features of the training sets.
+            y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): The target class.
+            test_size (float, optional):  Defaults to .2. The test size in float.
+            random_state (int, optional):  Defaults to 11. The randomize state.
 
         Returns:
-            Tuple: _description_ x_train, x_test, y_train, y_test pair.
+            Tuple: x_train, x_test, y_train, y_test pair.
         """
         return train_test_split(
             x_train, y_train, test_size=test_size, random_state=random_state)
 
     def store_artifact(self, model: Any, local_path: str, artifact_path: str) -> None:
-        """_summary_
+        """
         Store the artifact into a joblib file. Then upload to the artifact registry.
         Args:
-            model (Any): _description_ The model instance.
-            local_path (str): _description_ The local_path to be dump.
-            artifact_path (str): _description_ The artifact path in cloud storage.
+            model (Any): The model instance.
+            local_path (str): The local_path to be dump.
+            artifact_path (str): The artifact path in cloud storage.
         """
 
         joblib.dump(model, local_path)
 
         mlflow.log_artifact(local_path=local_path, artifact_path=artifact_path)
 
-    def log_param(self, key: str, value: str) -> None:
-        """_summary_
-        Log the parameters into the MLflow Experiment logs.
-        Args:
-            key (str): _description_ The param key.
-            value (str): _description_ The param value.
-        """
-        mlflow.log_param(key=key, value=value)
-
-    def log_metric(self, key: str, value: float) -> None:
-        """_summary_
-        Log the metric into the MLflow Experiment logs.
-        Args:
-            key (str): _description_ The metric key.
-            value (Any): _description_ The metric value.
-        """
-        mlflow.log_metric(key=key, value=value)
-
     def deploy(self,
                artifact_uri: str,
                deployment_name: str,
                model_name: str,
                authentication: AbstractKubernetesAuth,
                namespace: str = 'default',
                deployment_template: str = None) -> Dict:
-        """_summary_ Deploy experiment to Seldon Environment.
+        """Deploy experiment to Seldon Environment.
 
         This method would invoke the Deployment class and its dependencies to deploy \
         the experiment using default / user defined template.
 
         Args:
-            artifact_uri (str): _description_ The artifact URI. \
+            artifact_uri (str): The artifact URI. \
                 We could see it in the MLflow Tracking Server UI.
-            deployment_name (str): _description_ The Kubernetes deployment name.
-            model_name (str): _description_ The model name.
-            authentication (AbstractKubernetesAuth): _description_ The authentication object. \
+            deployment_name (str): The Kubernetes deployment name.
+            model_name (str): The model name.
+            authentication (AbstractKubernetesAuth): The authentication object. \
                 Currently supports for GCP and default / minikube Auth.
-            namespace (str, optional): _description_. Defaults to 'default'. \
+            namespace (str, optional):  Defaults to 'default'. \
                 The Kubernetes target namespace.
-            deployment_template (str, optional): _description_. Defaults to None. \
+            deployment_template (str, optional):  Defaults to None. \
                 Kubernetes JSON template file path. Recommended using default template.
         """
         try:
-            deployment = SeldonDeployment(
+            deployment = Deployment(
                 authentication=authentication, namespace=namespace)
             if deployment_template is None:
                 print("Klops path:", KLOPS_PATH)
                 deployment_template = os.path.join(
                     KLOPS_PATH, 'templates/deployment_template.json')
 
             config = deployment.load_deployment_configuration(
                 deployment_template)
             config["metadata"]["name"] = deployment_name
             config["spec"]["name"] = model_name
             config["spec"]["predictors"][0]["graph"]["modelUri"] = artifact_uri
 
             return deployment.deploy(config)
         except ApiException as api_exception:
-            raise SeldonDeploymentException(
+            raise DeploymentException(
                 status=api_exception.status,
                 reason=api_exception.reason,
                 http_resp="Failed to deploy.") from api_exception
         except Exception as exception:
             raise ExperimentFailedException(
                 message=str(exception)) from exception
 
@@ -269,58 +275,58 @@
 def start_experiment(
         name: str,
         tracking_uri: str,
         classifier: Any,
         x_train: Union[np.ndarray, pd.DataFrame, List[Dict]],
         y_train: Union[np.ndarray, pd.DataFrame, List[Dict]],
         dataset_auto_split: bool = True,
-        x_test: Union[np.ndarray, pd.DataFrame, List[Dict]] = [],
-        y_test: Union[np.ndarray, pd.DataFrame, List] = [],
+        x_test: Union[np.ndarray, pd.DataFrame, List[Dict], None] = None,
+        y_test: Union[np.ndarray, pd.DataFrame, List, None] = None,
         test_size: float = .2,
         random_state: int = 11,
         tuner: str = None,
         tuner_args: Dict = {},
         metrices: Dict = {
             "mean_squared_error": {},
             "root_mean_squared_error": {"squared": True}}
 ) -> Experiment:
-    """_summary_
+    """
     The function that wrap all the basic Experiment class do. This make the process more easier.
 
     Args:
-        name (str): _description_ The experiment name. Example: "my-classification-experiment"
-        tracking_uri (str): _description_ The MLflow experiment tracking uri. \
+        name (str): The experiment name. Example: "my-classification-experiment"
+        tracking_uri (str): The MLflow experiment tracking uri. \
             Its our MLflow Tracking server URI. Example: "http://<your-mlflow-host>:<port>"
-        classifier (Any): _description_ The classifier pointer class. \
+        classifier (Any): The classifier pointer class. \
             Example: sklearn.naive_bayes.GaussianNB
         x_train_data (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
-            _description_ The input features with 2 Dimensional Array like.
+            The input features with 2 Dimensional Array like.
         y_train_data (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
-            _description_ The output mapping.
+            The output mapping.
         dataset_auto_split (bool):  Whether to automatically split the dataset into train-test pairs.
-        x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_ \
+        x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
             The input test value. Only usable when the dataset_auto_split flag is False.
-        y_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_ \
+        y_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): \
             The output test value. Only usable when the dataset_auto_split flag is False.
         test_size (float): The split size of the test data.
         random_state (int): The number of random state.
-        tuner (str): _description_ The tuner could be one of (default | hyperopt | gridsearch). \
+        tuner (str): The tuner could be one of (default | hyperopt | gridsearch). \
             Defaults to None.
-        tuner_args (Dict, optional): _description_. Defaults to {}. Tunner keyworded arguments. \
+        tuner_args (Dict, optional):  Defaults to {}. Tunner keyworded arguments. \
             A Dictionary contains key-value pairs set of hyper parameters.
-        metrices (_type_, optional): _description_. Defaults to \
+        metrices (_type_, optional):  Defaults to \
             { "mean_squared_error": {}, "root_mean_squared_error": {"squared": True}}. \
             The sklearn metrices. All metrices method name could be seen here: \
             https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
 
     Raises:
-        ValueError: _description_ Raised when the input arguments has invalid value.
+        ValueError: Raised when the input arguments has invalid value.
 
     Returns:
-        Experiment: _description_ The Experiment class instance.
+        Experiment: The Experiment class instance.
     """
     experiment = Experiment(name=name, tracking_uri=tracking_uri)
     experiment = experiment.start(
         classifier=classifier, x_train=x_train,
         y_train=y_train, tuner=tuner,
         dataset_auto_split=dataset_auto_split,
         x_test=x_test, y_test=y_test,
```

### Comparing `klops-0.0.3/klops/experiment/runner/base.py` & `klops-0.0.4/klops/experiment/runner/hyperopt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,119 @@
-"""_summary_
-Base runner module.
 """
+"""
+from typing import Any, Dict, List, Union
+from datetime import datetime
 
-
-from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Tuple, Union
-
+from hyperopt import STATUS_OK, fmin, Trials, tpe
 import mlflow
 import numpy as np
 import pandas as pd
 from sklearn import metrics
-from sklearn.model_selection import train_test_split
 
-from klops.experiment.exception import InvalidArgumentsException, LogMetricException
+from klops.experiment.runner import BaseRunner
+from klops.experiment.exception import ExperimentFailedException
 
 
-class BaseRunner(ABC):
-    """_summary_
-    Abstract class as Base runner implementation.
+class HyperOptRunner(BaseRunner):
+    """The HyperOptRunner Implementation.
     """
 
-    metrices: Dict = {"mean_squared_error": {}, "root_mean_squared_error": {}}
-
     def __init__(self,
-                estimator: Any,
-                x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
-                y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
-                x_test: Union[np.ndarray, pd.DataFrame, List[Dict]],
-                y_test: Union[np.ndarray, pd.DataFrame, List],
-                tags: Dict = {}) -> None:
-        """_summary_
+                 estimator: Any,
+                 x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
+                 y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
+                 x_test: Union[np.ndarray, pd.DataFrame, List[Dict]],
+                 y_test: Union[np.ndarray, pd.DataFrame, List],
+                 search_spaces: Dict,
+                 experiment_name: str,
+                 tags: Dict = {},
+                 max_evals: int = 20) -> None:
+        """
 
         Args:
-            estimator (Any): _description_
-            x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
-            y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
-            x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_
-            y_test (Union[np.ndarray, pd.DataFrame, List]): _description_
-            tags (Dict): _description_ Defaults to {}. Additional tags for logging in Experiment.
-        """
-        self.estimator = estimator
-        self.x_test = x_test
-        self.y_test = y_test
-        self.x_train = x_train
-        self.y_train = y_train
-        self.tags = tags
-
-    @abstractmethod
-    def run(self, metrices: Dict, **kwargs: Any) -> Any:
-        """_summary_
-        The abstract method for base implementation to execute the experiment.
+            estimator (Any): The model class instance. Can be sklearn model or any of supported \
+                models by mlflow.
+            x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): The features set for training.
+            y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): The target set for training.
+            x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): The test features.
+            y_test (Union[np.ndarray, pd.DataFrame, List]): The test expected target.
+            search_spaces (Dict): Hyperparameter search space for training.
+            experiment_name (str): The experiment name. Example: "my-experiment-name".
+            max_evals (int, optional):  Defaults to 20. Maximum number of training trials.
+        """
+        self.search_spaces = search_spaces
+        self.max_evals = max_evals
+        self.experiment_name = experiment_name
+
+        super(HyperOptRunner, self).__init__(
+            estimator=estimator, x_train=x_train, y_train=y_train,
+            x_test=x_test, y_test=y_test, tags=tags)
+
+    def objective(self, hyper_parameters: Dict) -> Dict:
+        """
+        Run the experiment using hyperopt. Each experiment would generate exactly one \
+            artifact regitry in repository.
+
         Args:
-            metrices (Dict): _description_ The metrices that would be invoked as measurements.
-            **kwargs (Any): _description_ The key-word arguments hyper-parameters for the given class Model.
+            hyper_parameters (Dict): The hyper parameters for each experiment.
+
         Returns:
-            Any: _description_
+            Dict: Dictionary contains error function result.
+        """
+        run_name = self.experiment_name + "_" + datetime.now().strftime("%Y%m%d:%H%M%S")
+        with mlflow.start_run(run_name=run_name):
+            result = {"status": STATUS_OK}
+
+            mlflow.set_tags({**self.tags, "opt":"hyperopt"})
+            mlflow.log_params({
+                **hyper_parameters,
+                "estimator": self.estimator.__class__.__name__})
+
+            model = self.estimator
+            model.fit(self.x_train, self.y_train)
+            preds = model.predict(self.x_test)
+            rmse = self.call_metrices("root_mean_squared_error", self.y_test, preds)
+            for metric, arguments in self.metrices.items():
+                metric_name, score = self.call_metrices(metric, self.y_test, preds, **arguments)
+                result[metric_name] = score
+            return {**result, "loss": rmse, "model": model}
+
+    def run(self,
+            metrices: Dict = {"mean_squared_error": {},
+                              "root_mean_squared_error": {}},
+            **kwargs: Any) -> Dict[str, Any]:
         """
+        Run the experiment using hyperopt.fmin function.
 
-    def split_train_test(self,
-                         x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
-                         y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
-                         test_size: float = .2, random_state: int = 11) -> None:
-        """_summary_
-        Splits the given datasets of features and its class into train-test group pair.
         Args:
-            x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
-                The features data.
-            y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
-                The class data.
-        """
-        self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(
-            x_train, y_train, test_size=test_size, random_state=random_state)
-
-    def call_metrices(self, metric_name: str, *args: Any, **kwargs: Any) -> Tuple:
-        """_summary_
-        Call the measurement metrices (inherited from sklearn metrices), log as mlflow metric.
-        Args:
-            metric_name (str): _description_ The sklearn metrices.
-            All metrices method name could be seen here:
-            https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
+            metrices (Dict, optional):
+                Defaults to {"mean_squared_error": {}, "root_mean_squared_error": {}}. \
+                The sklearn metrices. All metrices method name could be seen here: \
+                https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
+
+        Returns:
+            Dict: The best fit hyperparams configuration and its model.
         """
         try:
-            if metric_name != "root_mean_squared_error":
 
-                metric_function = getattr(metrics, metric_name)
-                score = metric_function(*args, **kwargs)
-            else:
-                score = metrics.mean_squared_error(*args, **kwargs)
-            mlflow.log_metric(metric_name, score)
-            
-            return metric_name, score
-        except ValueError as value_error:
-            raise InvalidArgumentsException(message=str(value_error)) from value_error
+            self.metrices = metrices
+            trials = Trials()
+
+            best_fit = fmin(
+                fn=self.objective,
+                space=self.search_spaces,
+                algo=tpe.suggest,
+                max_evals=self.max_evals,
+                trials=trials,
+                **kwargs
+            )
+
+            best = trials.results[np.argmin([r['loss'] for r in trials.results])]
+            print(best)
+
+            return {"best_param": {**best_fit}, "model": best.model, "score": 1 - best.loss}
         except Exception as exception:
-            raise LogMetricException(message=str(exception)) from exception
+            raise ExperimentFailedException(
+                message=str(exception)) from exception
 
 
-__all__ = ["BaseRunner"]
+__all__ = ["HyperOptRunner"]
```

### Comparing `klops-0.0.3/klops/experiment/runner/basic.py` & `klops-0.0.4/klops/experiment/runner/basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,80 @@
-"""_summary_
+"""
 Experiment Runner Module without tuner.
 """
 
 from typing import Any, Union, List, Dict
 import mlflow
 import numpy as np
 import pandas as pd
 
 from klops.experiment.runner.base import BaseRunner
 from klops.experiment.exception import ExperimentFailedException
 
 
 class BasicRunner(BaseRunner):
-    """_summary_
+    """
     Experiment Runner Implementation Class without tuner.
     """
 
     def __init__(self,
                  estimator: Any,
                  x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                  y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                  x_test: Union[np.ndarray, pd.DataFrame, List[Dict]],
                  y_test: Union[np.ndarray, pd.DataFrame, List],
                  hyparams: Dict = {},
                  tags: Dict = {},
                  autolog_max_tunning_runs: int = None) -> None:
-        """_summary_
+        """
 
         Args:
             estimator (Any): _description_
             x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
             y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
             x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_
             y_test (Union[np.ndarray, pd.DataFrame, List]): _description_
-            hyparams (Dict, optional): _description_. Defaults to {}.
-            autolog_max_tunning_runs (int, optional): _description_. Defaults to None.
+            hyparams (Dict, optional):  Defaults to {}.
+            autolog_max_tunning_runs (int, optional):  Defaults to None.
         """
         self.hyparams = hyparams
         mlflow.sklearn.autolog(max_tuning_runs=autolog_max_tunning_runs)
         super(BasicRunner, self).__init__(
             estimator=estimator, x_train=x_train, y_train=y_train,
             x_test=x_test, y_test=y_test, tags=tags)
 
     def run(self,
             metrices: Dict = {"mean_squared_error": {},
                               "root_mean_squared_error": {}},
-            **kwargs: Any) -> Any:
-        """_summary_
+            **kwargs: Any) -> Dict[str, Any]:
+        """
         Run the experiment without any tuner.
+
         Args:
-            metrices (_type_, optional): _description_.
+            metrices (Dict, optional):
                 Defaults to {"mean_squared_error": {}, "root_mean_squared_error": {}}.
                 The sklearn metrices. All metrices method name could be seen here:
                 https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
+
+        Returns:
+            Dict: The best fit hyperparams configuration and its model.
         """
         try:
             mlflow.set_tags({**self.tags, "opt":"hyperopt"})
             mlflow.log_params(kwargs)
             model = self.estimator
 
             model.fit(self.x_train, self.y_train)
             preds = model.predict(self.x_test)
+            metric_name, score = self.call_metrices("root_mean_squared_error", self.y_test, preds)
             for metric, arguments in metrices.items():
                 self.call_metrices(metric, self.y_test, preds, **arguments)
+
             mlflow.end_run()
+
+            return {"best_param": {**self.hyparams}, "model": model, "score":  1 - score}
         except Exception as exception:
             raise ExperimentFailedException(
                 message=str(exception)) from exception
 
 
 __all__ = ["BasicRunner"]
```

### Comparing `klops-0.0.3/klops/experiment/runner/gridsearch.py` & `klops-0.0.4/klops/experiment/runner/gridsearch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,84 @@
-"""_summary_
+"""
 """
 from typing import Any, Type, Union, List, Dict
 import mlflow
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import GridSearchCV
 
 from klops.experiment.runner import BaseRunner
 from klops.experiment.exception import ExperimentFailedException
 
 
 class GridsearchRunner(BaseRunner):
-    """_summary_ GridSearchCV Runner Implementation.
+    """GridSearchCV Runner Implementation.
     """
 
     def __init__(self,
                  estimator: Type[Any],
                  x_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                  y_train: Union[pd.DataFrame, np.ndarray, List, Dict],
                  x_test: Union[np.ndarray, pd.DataFrame, List[Dict]],
                  y_test: Union[np.ndarray, pd.DataFrame, List],
                  grid_params: Dict = {},
                  tags: Dict = {},
                  autolog_max_tunning_runs: int = None) -> None:
-        """_summary_
+        """
 
         Args:
             estimator (Type[Any]): _description_
             x_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
             y_train (Union[pd.DataFrame, np.ndarray, List, Dict]): _description_
             x_test (Union[np.ndarray, pd.DataFrame, List[Dict]]): _description_
             y_test (Union[np.ndarray, pd.DataFrame, List]): _description_
-            grid_params (Dict, optional): _description_. Defaults to {}.
-            autolog_max_tunning_runs (int, optional): _description_. Defaults to None.
+            grid_params (Dict, optional):  Defaults to {}.
+            autolog_max_tunning_runs (int, optional):  Defaults to None.
         """
         self.grid_params = grid_params
         mlflow.sklearn.autolog(max_tuning_runs=autolog_max_tunning_runs)
         
         super(GridsearchRunner, self).__init__(
             estimator=estimator, x_train=x_train, 
             y_train=y_train, x_test=x_test, y_test=y_test,
             tags=tags)
 
     def run(self,
             metrices: Dict = {"mean_squared_error": {},
                               "root_mean_squared_error": {}},
-            **kwargs: Any) -> Any:
-        """_summary_
+            **kwargs: Any) -> Dict[str, Any]:
+        """
         Run the experiment using sklearn.model_selection.GridsearchCV tuner.
+
         Args:
-            metrices (_type_, optional): _description_.
+            metrices (Dict, optional):
                 Defaults to {"mean_squared_error": {}, "root_mean_squared_error": {}}.
                 The sklearn metrices. All metrices method name could be seen here:
                 https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
+
+        Returns:
+            Dict: The best fit hyperparams configuration and its model.
         """
         try:
             mlflow.set_tags({**self.tags, "opt": "gridsearch"})
 
             grid_search = GridSearchCV(
                 estimator=self.estimator,
                 param_grid=self.grid_params,
                 **kwargs
             )
-            
+
             best_fit = grid_search.fit(self.x_train, self.y_train)
             preds = best_fit.predict(self.x_test)
             for metric, arguments in metrices.items():
                 self.call_metrices(metric, self.y_test, preds, **arguments)
             mlflow.end_run()
+            return {
+                "best_param": best_fit.best_params_,
+                "model": best_fit,
+                "score": best_fit.best_score_}
         except Exception as exception:
             raise ExperimentFailedException(
                 message=str(exception)) from exception
 
 
 __all__ = ["GridsearchRunner"]
```

### Comparing `klops-0.0.3/klops/seldon_core/deployment.py` & `klops-0.0.4/klops/deployment/deployment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 """
-Deployment Module for Seldon Core.
+Deployment module implementation to deploy the machine learning models \
+    to Seldon Kubernetes Cluster.
 """
 import json
 import pathlib
 from typing import Dict
 import yaml
 
 from kubernetes import client
 
-from klops.seldon_core.auth.schema import AbstractKubernetesAuth
-from klops.seldon_core.exception import SeldonDeploymentException
+from klops.deployment.auth.schema import AbstractKubernetesAuth
+from klops.deployment.exception import DeploymentException
 
 
-class SeldonDeployment:
-    """_summary_
-    CRUD Kubernetes operation class implementation for Seldon ML Deployment.
+class Deployment:
+    """
+    CRUD Kubernetes operation class implementation for ML \
+        Deployment Using Seldon Core as its engine.
     """
 
     api: client.CustomObjectsApi = None
 
     def __init__(self,
                  authentication: AbstractKubernetesAuth,
                  namespace: str) -> None:
-        """_summary_
-        The contructor for SeldonDeployment class.
+        """
+        The contructor for Deployment class.
         Args:
-            authentication (AbstractKubernetesAuth): _description_
+            authentication (AbstractKubernetesAuth): \
                 The authentication instances. Currently only supports for local cluster or GKE.
-            namespace (str): _description_ The kubernetes namespace deployment target.
+            namespace (str): The kubernetes namespace deployment target.
         """
         self.authentication = authentication
         self.namespace = namespace
         self.connect_to_cluster()
 
     def connect_to_cluster(self) -> None:
-        """_summary_
+        """
         Connect to the kubernetes cluster given from the constructor arguments.
         """
         configuration = client.Configuration()
-        configuration.host = self.authentication.get_custer_endpoint()
+        configuration.host = self.authentication.get_cluster_endpoint
         configuration.verify_ssl = False
         configuration.api_key['authorization'] = "Bearer " + \
-            self.authentication.get_token()
+            self.authentication.get_token
 
         api_client = client.ApiClient(configuration=configuration)
         self.api = client.CustomObjectsApi(api_client=api_client)
 
-    def load_deployment_configuration(self, file_name: str):
-        """_summary_
+    def load_deployment_configuration(self, file_name: str) -> Dict:
+        """
         Load the deployment configuration file into a Python dictionary.
 
         Args:
-            file_name (str): _description_ The deployment file name.
+            file_name (str): The deployment file name. \
                 It can be Yaml file (.yml or .yaml) or JSON file.
 
         Returns:
-            deployment_config (dict): _description_ Seldon Deployment configuration dictionary.
+            deployment_config (Dict): Seldon Deployment configuration dictionary.
 
         Raises:
-            ValueError: _description_ When the file type are not yaml or json.
-            JSONDecodeError: _description_ When the JSON file contains wrong format.
-            YAMLError: _description_ When the Yaml contains wrong format.
+            ValueError: When the file type are not yaml or json.
+            JSONDecodeError: When the JSON file contains wrong format.
+            YAMLError: When the Yaml contains wrong format.
         """
         deployment_config = {}
 
         with open(file_name, "rb") as file:
             extension = pathlib.Path(file_name).suffix
             if extension == ".json":
                 deployment_config = json.load(file)
             elif extension in [".yaml", ".yml"]:
                 deployment_config = yaml.safe_load(file)
             else:
                 raise ValueError("Invalid file type.")
         return deployment_config
 
     def deploy(self, deployment_config: Dict) -> Dict:
-        """_description_
+        """
         Deploy the ML Model
 
         Args:
-            deployment_config (Union[object, Dict]): _description_
+            deployment_config (Union[object, Dict]): \
                 Deployment Configuration Object.
 
         Returns:
-            deployment_result (Dict): _description_ The deployment result metadata in a dictionary.
+            deployment_result (Dict): The deployment result metadata in a dictionary.
 
         Raises:
-            SeldonDeploymentException: _description_ Raised when the deployment failed.
+            DeploymentException: Raised when the deployment failed.
         """
         deployment_name = deployment_config["metadata"]["name"]
 
         deployment_existence = self.check_deployment_exist(
             deployment_name=deployment_name)
         if not deployment_existence:
 
@@ -107,65 +109,65 @@
                 name=deployment_name,
                 plural="seldondeployments",
                 body=deployment_config,
                 namespace=self.namespace)
         return deployment_result
 
     def check_deployment_exist(self, deployment_name: str) -> bool:
-        """ _summary_
+        """
         Check the deployment already exists.
 
         Args:
-            deployment_name (str): _description_ The deployment name, Example: iris-model
+            deployment_name (str): The deployment name, Example: iris-model
 
         Returns:
-            bool: _description_ The deployment existence.
+            bool: The deployment existence.
 
         Raises:
-            AttributeError: _description_ Raised when the key doesn't exists.
-            NoneTypeException: _description_ Raised when wrong compared with None Object.
+            AttributeError: Raised when the key doesn't exists.
+            NoneTypeException: Raised when wrong compared with None Object.
         """
         deployment_names = []
         response = self.api.list_namespaced_custom_object(
             group="machinelearning.seldon.io",
             version="v1alpha2",
             plural="seldondeployments",
             namespace=self.namespace)
         for item in response["items"]:
             deployment_names.append(item["metadata"]["name"])
         return deployment_name in deployment_names
 
     def delete_by_deployment_config(self, deployment_config: Dict) -> bool:
-        """_summary_
+        """
         Delete the deployment by its configuration.
 
         Args:
-            deployment_config (Union[object, Dict]): _description_ \
+            deployment_config (Union[object, Dict]): \
                 Deployment Configuration Object.
 
         Returns:
-            bool: _description_ Boolean result of deployment deletion.
+            bool: Boolean result of deployment deletion.
 
         Raises:
-            SeldonDeploymentException: _description_ Raised when the deployment failed.
+            DeploymentException: Raised when the deployment failed.
         """
         return self.delete(deployment_config["metadata"]["name"])
 
     def delete(self, deployment_name: str) -> bool:
-        """_summary_
-        Deploy the ML Model
+        """
+        Delete the ML Model Deployment from Kubernetes cluster by name.
 
         Args:
-            deployment_name (Union[object, Dict]): _description_ Deployment name.
+            deployment_name (Union[object, Dict]): Deployment name.
 
         Returns:
-            bool: _description_ Boolean result of deployment deletion.
+            bool: Boolean result of deployment deletion.
 
         Raises:
-            SeldonDeploymentException: _description_ Raised when the deployment failed.
+            DeploymentException: Raised when the deployment failed.
         """
         try:
             deployment_existence = self.check_deployment_exist(
                 deployment_name=deployment_name)
             if not deployment_existence:
                 return False
             else:
@@ -173,10 +175,10 @@
                     group="machinelearning.seldon.io",
                     version="v1alpha2",
                     name=deployment_name,
                     plural="seldondeployments",
                     namespace=self.namespace)
                 if deletion_result:
                     return True
-        except SeldonDeploymentException as deployment_exception:
+        except DeploymentException as deployment_exception:
             print("Deployment deletion failed,", str(deployment_exception))
             return False
```

### Comparing `klops-0.0.3/klops/seldon_core/exception.py` & `klops-0.0.4/klops/deployment/exception.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 """
 Seldon deployment exception handler module.
 """
+from typing import Any, Optional
 from kubernetes.client import ApiException
 
 
-class SeldonDeploymentException(ApiException):
+class DeploymentException(ApiException):
     """
     Seldon Deployment Exception Class Handler.
     """
 
-    def __init__(self, *, status=None, reason=None, http_resp=None):
-        """_summary_
+    def __init__(self, *,
+                 status: Optional[int] = None, reason: Optional[str] = None, http_resp=None):
+        """
         The constructor for the exception class handler.
 
         Args:
-            status (_type_, optional): _description_. Defaults to None. The exception status code.
-            reason (_type_, optional): _description_. Defaults to None. The exception elaborated reason.
-            http_resp (_type_, optional): _description_. Defaults to None. The HTTP response.
+            status (int, optional):  Defaults to None. The exception status code.
+            reason (str, optional):  Defaults to None. The exception elaborated reason.
+            http_resp (_type_, optional):  Defaults to None. The HTTP response.
         """
         self.status = status
         self.reason = reason
         self.http_resp = http_resp
         self.body = http_resp.data
         self.headers = http_resp.getheaders()
-        super(SeldonDeploymentException, self).__init__(
+        super(DeploymentException, self).__init__(
             status, reason, http_resp)
+
+
+class WriteAuthConfigException(Exception):
+    """WriteAuthConfigException. Raised when failed to write a config file.
+    """
+
+    def __init__(self, reason: Optional[str] = None, **args: Any):
+        """
+        The constructor for the exception class handler.
+
+        Args:
+            status (int, optional):  Defaults to None. The exception status code.
+            reason (str, optional):  Defaults to None. The exception elaborated reason.
+            http_resp (_type_, optional):  Defaults to None. The HTTP response.
+        """
+        self.reason = reason
+        super(WriteAuthConfigException, self).__init__(**args)
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        return self.reason
```

### Comparing `klops-0.0.3/klops/templates/deployment_template.json` & `klops-0.0.4/klops/templates/deployment_template.json`

 * *Files identical despite different names*

### Comparing `klops-0.0.3/klops/versioning/helper.py` & `klops-0.0.4/klops/versioning/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""_summary_
+"""
 """
 import subprocess
 
 from klops.config import LOGGER
 
 
 def shell_executor(command: str) -> subprocess.CompletedProcess:
-    """_summary_
+    """
     Command line executor wrapper.
     Args:
-        command (str): _description_ The shell command string.
+        command (str): The shell command string.
 
     Returns:
         subprocess.CompletedProcess: _description_
     """
     try:
         return subprocess.run(command, check=True, shell=True)
     except subprocess.CalledProcessError as called_error:
```

### Comparing `klops-0.0.3/klops.egg-info/PKG-INFO` & `klops-0.0.4/klops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klops
-Version: 0.0.3
+Version: 0.0.4
 Summary: Klops: Koin Machine Learning Ops
 Home-page: https://gitlab-engineering.koinworks.com/data-team/klops/
 Author: Koinworks Data Team
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -14,15 +14,15 @@
 
 <p align="center">
     <strong>Build your end-to-end machine learning projects within one tool.</strong>
 </p>
 
 <p align="center">
     <a href="#" title="PyPi Version"><img src="https://img.shields.io/badge/PyPi-v.0.4.8-blue"></a>
-    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.6%2B-green"></a>
+    <a href="#" title="Python Version"><img src="https://img.shields.io/badge/Python-3.8%2B-green"></a>
     <!-- <a href="https://www.codacy.com/gh/ml-tooling/lazydocs/dashboard" title="Codacy Analysis"><img src="https://app.codacy.com/project/badge/Grade/1c8ad486ce9547b6b713cce7ca1d1ec3"></a> -->
     <!-- <a href="" title="Build status"><img src="https://img.shields.io/github/workflow/status/ml-tooling/lazydocs/build-pipeline?style=flat"></a> -->
     <a href="#" title="Project License"><img src="https://img.shields.io/badge/License-Koinworks-red"></a>
     <!-- <a href="https://gitter.im/ml-tooling/lazydocs" title="Chat on Gitter"><img src="https://badges.gitter.im/ml-tooling/lazydocs.svg"></a> -->
     <a href="https://twitter.com/mltooling" title="ML Tooling on Twitter"><img src="https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: klops Version: 0.0.3 Summary: Klops: Koin Machine
+Metadata-Version: 2.1 Name: klops Version: 0.0.4 Summary: Klops: Koin Machine
 Learning Ops Home-page: https://gitlab-engineering.koinworks.com/data-team/
 klops/ Author: Koinworks Data Team Description-Content-Type: text/markdown
 Provides-Extra: test License-File: LICENSE
                         ****** Klops: Koin MLOps ******
        Build your end-to-end machine learning projects within one tool.
 [https://img.shields.io/badge/PyPi-v.0.4.8-blue] [https://img.shields.io/badge/
- Python-3.6%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
+ Python-3.8%2B-green]   [https://img.shields.io/badge/License-Koinworks-red]
 [https://img.shields.io/twitter/follow/mltooling.svg?label=follow&style=social]
         Getting_Started â¢ Documentation â¢ Support â¢ Contribution
 Klops is an End-to-End machine learning development pipeline ops. Its build on
 top of Seldon Core, MLflow and DVC. The goal of this project is to make easier
 for Data Scientist to develop, maintain, log their experiments and deploy their
 machine learning projects. ## Prerequisites - Seldon Core Installed on your
 Kubernetes cluster. Guidance [here](https://docs.seldon.io/projects/seldon-
```

### Comparing `klops-0.0.3/setup.py` & `klops-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         encoding=kwargs.get("encoding", "utf8"),
     ) as open_file:
         content = open_file.read().strip()
     return content
 
 
 requirements = [
+    "click",
     "dvc",
     "google-cloud",
     "google-cloud-container",
     "google-cloud-storage",
     "google-auth",
     "hyperopt",
     "kubernetes",
@@ -47,19 +48,25 @@
     "pytest-cov",
     "codecov",
     "mypy",
     "gitchangelog",
     "mkdocs"
 ]
 
+
 setup(
     name="klops",
     version=read("klops", "VERSION"),
     description="Klops: Koin Machine Learning Ops",
     url="https://gitlab-engineering.koinworks.com/data-team/klops/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Koinworks Data Team",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=requirements,
+    entry_points={
+        "console_scripts": ["klops = klops.__main__:main"]
+    },
     extras_require={"test": requirements_test},
+    package_data={'': ['klops/*.json']},
+    include_package_data=True
 )
```

### Comparing `klops-0.0.3/tests/seldon_core/deployment_test.py` & `klops-0.0.4/tests/seldon_core/deployment_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Unit Test for Seldon Deployment
 """
 from unittest import TestCase
 from unittest.mock import Mock, patch
-
-from klops.seldon_core import SeldonDeployment
 from kubernetes.client import CustomObjectsApi
 
+from klops.deployment import SeldonDeployment
+
 
 class TestSeldonDeployment(TestCase):
     """
     Test class for SeldonDeployment
     """
 
     def __init__(self, *args, **kwargs) -> None:
@@ -26,45 +26,51 @@
         }
 
     @patch.object(CustomObjectsApi, "create_namespaced_custom_object")
     def test_deploy_for_new_deployment(self, mocked_create_deployment):
         """
         Test deploy for new deployment.
         """
-        with patch.object(self.seldon_deployment, "check_deployment_exist", return_value=False) as mocked_check_deployment:
+        with patch.object(self.seldon_deployment,
+                          "check_deployment_exist", return_value=False) as mocked_check_deployment:
             self.seldon_deployment.deploy(
                 deployment_config=self.deployment_config)
             mocked_check_deployment.assert_called_once_with(
                 deployment_name=self.deployment_config["metadata"]["name"])
             mocked_create_deployment.assert_called_once()
 
     @patch.object(CustomObjectsApi, "patch_namespaced_custom_object")
     def test_deploy_for_existing_deployment(self, mocked_patch_deployment):
         """
         Test deploy or existing deployment.
         """
-        with patch.object(self.seldon_deployment, "check_deployment_exist", return_value=True) as mocked_check_deployment:
+        with patch.object(self.seldon_deployment,
+                          "check_deployment_exist",
+                          return_value=True) as mocked_check_deployment:
             self.seldon_deployment.deploy(
                 deployment_config=self.deployment_config)
             mocked_check_deployment.assert_called_once_with(
                 deployment_name=self.deployment_config["metadata"]["name"])
             mocked_patch_deployment.assert_called_once()
 
     @patch.object(CustomObjectsApi, "delete_namespaced_custom_object")
     def test_delete_deployment(self, mocked_delete_deployment):
         """
         Test the delete deployment
         """
-        with patch.object(self.seldon_deployment, "check_deployment_exist", return_value=True) as mocked_check_deployment:
+        with patch.object(self.seldon_deployment,
+                          "check_deployment_exist", return_value=True) as mocked_check_deployment:
             self.seldon_deployment.delete(self.deployment_config)
             mocked_check_deployment.assert_called_once_with(
                 deployment_name=self.deployment_config["metadata"]["name"])
             mocked_delete_deployment.assert_called_once()
 
-    @patch.object(CustomObjectsApi, "list_namespaced_custom_object", return_value={"items": [{"metadata": {"name": "mockedLearn"}}]})
+    @patch.object(CustomObjectsApi,
+                  "list_namespaced_custom_object",
+                  return_value={"items": [{"metadata": {"name": "mockedLearn"}}]})
     def testcheck_deployment_exist(self, mocked_list_object):
         """
         Test Check deployment exists
         """
         result = self.seldon_deployment.check_deployment_exist("mockedLearn")
         self.assertTrue(result)
         mocked_list_object.assert_called_once()
```


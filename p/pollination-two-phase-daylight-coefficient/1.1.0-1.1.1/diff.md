# Comparing `tmp/pollination-two-phase-daylight-coefficient-1.1.0.tar.gz` & `tmp/pollination-two-phase-daylight-coefficient-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.1.0.tar", last modified: Tue May 23 18:16:25 2023, max compression
+gzip compressed data, was "dist/pollination-two-phase-daylight-coefficient-1.1.1.tar", last modified: Fri May 26 11:26:47 2023, max compression
```

## Comparing `pollination-two-phase-daylight-coefficient-1.1.0.tar` & `pollination-two-phase-daylight-coefficient-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:15:37.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:16:25.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 18:15:09.000000 pollination-two-phase-daylight-coefficient-1.1.0/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:26:10.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:26:47.000000 pollination-two-phase-daylight-coefficient-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-26 11:25:12.000000 pollination-two-phase-daylight-coefficient-1.1.1/tests/validation_test.py
```

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/ci.yaml` & `pollination-two-phase-daylight-coefficient-1.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/.github/workflows/tests.yaml` & `pollination-two-phase-daylight-coefficient-1.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/LICENSE` & `pollination-two-phase-daylight-coefficient-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/_prepare_folder.py` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/_prepare_folder.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/entry.py` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination/two_phase_daylight_coefficient/two_phase/entry.py` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination/two_phase_daylight_coefficient/two_phase/entry.py`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-two-phase-daylight-coefficient
-Version: 1.1.0
+Version: 1.1.1
 Summary: Two phase daylight coefficient recipe for Pollination.
 Home-page: https://github.com/pollination/two-phase-daylight-coefficient
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mikkel, ladybug-tools
 Maintainer-email: mikkel@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt` & `pollination-two-phase-daylight-coefficient-1.1.1/pollination_two_phase_daylight_coefficient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-two-phase-daylight-coefficient-1.1.0/setup.py` & `pollination-two-phase-daylight-coefficient-1.1.1/setup.py`

 * *Files identical despite different names*


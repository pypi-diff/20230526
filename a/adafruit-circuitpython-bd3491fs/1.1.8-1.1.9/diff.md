# Comparing `tmp/adafruit-circuitpython-bd3491fs-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-bd3491fs-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bd3491fs-1.1.8.tar", last modified: Fri Feb  4 19:52:41 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bd3491fs-1.1.9.tar", last modified: Fri May 20 00:52:12 2022, max compression
```

## Comparing `adafruit-circuitpython-bd3491fs-1.1.8.tar` & `adafruit-circuitpython-bd3491fs-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.611304 adafruit-circuitpython-bd3491fs-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.615304 adafruit-circuitpython-bd3491fs-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.615304 adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.615304 adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_bd3491fs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-02-04 19:52:41.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-02-04 19:52:41.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 19:52:41.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 19:52:41.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-04 19:52:41.000000 adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/examples/bd3491fs_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 19:52:41.619304 adafruit-circuitpython-bd3491fs-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-02-04 19:52:22.000000 adafruit-circuitpython-bd3491fs-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     7228 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_bd3491fs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-05-20 00:52:12.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-05-20 00:52:12.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 00:52:12.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-05-20 00:52:12.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-20 00:52:12.000000 adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/examples/bd3491fs_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 00:52:12.925926 adafruit-circuitpython-bd3491fs-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-05-20 00:52:01.000000 adafruit-circuitpython-bd3491fs-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bd3491fs-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-bd3491fs-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bd3491fs-1.1.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/.pylintrc` & `adafruit-circuitpython-bd3491fs-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bd3491fs-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/LICENSE` & `adafruit-circuitpython-bd3491fs-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bd3491fs-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/PKG-INFO` & `adafruit-circuitpython-bd3491fs-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bd3491fs
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the Rohm BD3491FS Audio Processor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython bd3491fs audio
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bd3491fs/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/bd3491fs/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/actions/
     :alt: Build Status
 
@@ -89,20 +89,17 @@
     bd3491fs.channel_2_attenuation = 0
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bd3491fs/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/README.rst` & `adafruit-circuitpython-bd3491fs-1.1.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bd3491fs/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/bd3491fs/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/actions/
     :alt: Build Status
 
@@ -70,18 +70,15 @@
     bd3491fs.channel_2_attenuation = 0
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bd3491fs/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/adafruit_bd3491fs.py` & `adafruit-circuitpython-bd3491fs-1.1.9/adafruit_bd3491fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS.git"
 
 from micropython import const
 import adafruit_bus_device.i2c_device as i2cdevice
 from adafruit_register.i2c_struct import UnaryStruct
 
+try:
+    import typing  # pylint: disable=unused-import
+    from busio import I2C
+except ImportError:
+    pass
+
 _INPUT_SELECTOR = const(0x04)
 _INPUT_GAIN = const(0x06)
 _VOLUME_GAIN_CH1 = const(0x21)
 _VOLUME_GAIN_CH2 = const(0x22)
 _BASS_GAIN = const(0x51)
 _TREBLE_GAIN = const(0x57)
 _SURROUND_GAIN = const(0x78)
@@ -129,85 +135,100 @@
 
     _input_selector = UnaryStruct(_INPUT_SELECTOR, "<B")
     _input_gain = UnaryStruct(_INPUT_GAIN, "<B")
     _ch1_attenuation = UnaryStruct(_VOLUME_GAIN_CH1, "<B")
     _ch2_attenuation = UnaryStruct(_VOLUME_GAIN_CH2, "<B")
     _system_reset = UnaryStruct(_SYSTEM_RESET, "<B")
 
-    def __init__(self, i2c_bus):
+    def __init__(self, i2c_bus: I2C) -> None:
         self.i2c_device = i2cdevice.I2CDevice(i2c_bus, 0x41)
         self._current_active_input = 7  # mute
         self._current_input_gain = 0  # 0dB
         self._current_ch1_attenuation = 255  # muted
         self._current_ch2_attenuation = 255  # muted
         self.reset()
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset the sensor, muting the input, reducting input gain to 0dB, and the output channnel
         attenuation to maximum"""
         self._reset = 0x81
 
     @property
-    def active_input(self):
+    def active_input(self) -> int:
         """The currently selected input. Must be an ``Input``
 
         This example sets A1 and A2 to the active input pair.
+
         .. code-block:: python
-        bd3491fs.active_input = adafruit_bd3491fs.Input.A
+
+            bd3491fs.active_input = adafruit_bd3491fs.Input.A
+
         """
         return self._current_active_input
 
     @active_input.setter
-    def active_input(self, value):
+    def active_input(self, value: int) -> None:
         self._input_selector = value
         self._current_active_input = value
 
     @property
-    def input_gain(self):
-        """The gain applied to all inputs equally"
+    def input_gain(self) -> int:
+        """The gain applied to all inputs equally
+
         This example sets the input gain to 10dB.
+
         .. code-block:: python
-        bd3491fs.input_gain = adafruit_bd3491fs.Level.10_DB""
+
+            bd3491fs.input_gain = adafruit_bd3491fs.Level.10_DB
+
         """
         return self._current_input_gain
 
     @input_gain.setter
-    def input_gain(self, value):
+    def input_gain(self, value: int) -> None:
         allowed_gains = [0, 1, 2, 3, 4, 6, 8, 10]
         if not value in allowed_gains:
             raise ValueError("input gain must be one of 0, 2, 4, 6, 8, 12, 16, 20 dB")
         self._input_gain = value
         self._current_input_gain = value
 
     @property
-    def channel_1_attenuation(self):
+    def channel_1_attenuation(self) -> int:
         """The attenuation applied to channel 1 of the currently selected input pair in -dB.
-        Maximum is -87dB. To mute set to 255
+        Maximum is -87dB. To mute set to 255.
+
         This example sets the attenuation for input channel 1 to -10dB.
+
         .. code-block:: python
-        bd3491fs.channel_1_attenuation = 10""
+
+            bd3491fs.channel_1_attenuation = 10
+
         """
         return self._current_ch1_attenuation
 
     @channel_1_attenuation.setter
-    def channel_1_attenuation(self, value):
+    def channel_1_attenuation(self, value: int) -> None:
         if (value < 0) or ((value > 87) and (value != 255)):
             raise ValueError("channel 1 attenuation must be from 0-87db")
         self._ch1_attenuation = value
         self._current_ch1_attenuation = value
 
     @property
-    def channel_2_attenuation(self):
+    def channel_2_attenuation(self) -> int:
         """The attenuation applied to channel 2 of the currently selected input pair in -dB.
-        Maximum is -87dB. To mute set to 255
+        Maximum is -87dB. To mute set to 255.
+
         This example sets the attenuation for input channel 2 to -10dB.
+
         .. code-block:: python
-        bd3491fs.channel_2_attenuation = 10""
+
+            bd3491fs.channel_2_attenuation = 10
+
         """
         return self._current_ch2_attenuation
 
     @channel_2_attenuation.setter
-    def channel_2_attenuation(self, value):
+    def channel_2_attenuation(self, value: int) -> None:
         if (value < 0) or ((value > 87) and (value != 255)):
             raise ValueError("channel 2 attenuation must be from 0-87db")
         self._ch2_attenuation = value
         self._current_ch2_attenuation = value
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/PKG-INFO` & `adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bd3491fs
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the Rohm BD3491FS Audio Processor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython bd3491fs audio
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-bd3491fs/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/bd3491fs/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/actions/
     :alt: Build Status
 
@@ -89,20 +89,17 @@
     bd3491fs.channel_2_attenuation = 0
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bd3491fs/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BD3491FS/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/adafruit_circuitpython_bd3491fs.egg-info/SOURCES.txt` & `adafruit-circuitpython-bd3491fs-1.1.9/adafruit_circuitpython_bd3491fs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bd3491fs-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/docs/conf.py` & `adafruit-circuitpython-bd3491fs-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/docs/index.rst` & `adafruit-circuitpython-bd3491fs-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bd3491fs-1.1.8/setup.py` & `adafruit-circuitpython-bd3491fs-1.1.9/setup.py`

 * *Files identical despite different names*


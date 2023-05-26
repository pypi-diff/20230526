# Comparing `tmp/adafruit-circuitpython-ds2413-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-ds2413-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ds2413-1.2.8.tar", last modified: Fri Feb  4 20:09:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ds2413-1.2.9.tar", last modified: Tue Jun  7 17:06:23 2022, max compression
```

## Comparing `adafruit-circuitpython-ds2413-1.2.8.tar` & `adafruit-circuitpython-ds2413-1.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.726385 adafruit-circuitpython-ds2413-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.726385 adafruit-circuitpython-ds2413-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.726385 adafruit-circuitpython-ds2413-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.726385 adafruit-circuitpython-ds2413-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.726385 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-02-04 20:09:57.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-02-04 20:09:57.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:09:57.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-02-04 20:09:57.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:09:57.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/adafruit_ds2413.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/examples/ds2413_direct_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/examples/ds2413_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:09:57.730385 adafruit-circuitpython-ds2413-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-02-04 20:09:45.000000 adafruit-circuitpython-ds2413-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.478479 adafruit-circuitpython-ds2413-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.478479 adafruit-circuitpython-ds2413-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.478479 adafruit-circuitpython-ds2413-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.478479 adafruit-circuitpython-ds2413-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.478479 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-06-07 17:06:23.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-06-07 17:06:23.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:06:23.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-07 17:06:23.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:06:23.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/adafruit_ds2413.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5358 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/examples/ds2413_direct_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/examples/ds2413_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:06:23.482479 adafruit-circuitpython-ds2413-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-06-07 17:06:09.000000 adafruit-circuitpython-ds2413-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ds2413-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-ds2413-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-ds2413-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ds2413-1.2.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ds2413-1.2.8/.pylintrc` & `adafruit-circuitpython-ds2413-1.2.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ds2413-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/LICENSE` & `adafruit-circuitpython-ds2413-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ds2413-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ds2413-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ds2413-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/PKG-INFO` & `adafruit-circuitpython-ds2413-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ds2413
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for DS2413 1-Wire Dual Channel Addressable Switch.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DS2413
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit haptic motor controller buzzer vibration breakout hardware micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds2413/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ds2413/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/actions/
     :alt: Build Status
 
@@ -98,20 +98,17 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds2413/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS2413/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/README.rst` & `adafruit-circuitpython-ds2413-1.2.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds2413/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ds2413/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/actions/
     :alt: Build Status
 
@@ -79,18 +79,15 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds2413/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS2413/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/PKG-INFO` & `adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ds2413
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for DS2413 1-Wire Dual Channel Addressable Switch.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DS2413
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit haptic motor controller buzzer vibration breakout hardware micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds2413/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ds2413/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_DS2413/actions/
     :alt: Build Status
 
@@ -98,20 +98,17 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds2413/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS2413/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/adafruit_circuitpython_ds2413.egg-info/SOURCES.txt` & `adafruit-circuitpython-ds2413-1.2.9/adafruit_circuitpython_ds2413.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/adafruit_ds2413.py` & `adafruit-circuitpython-ds2413-1.2.9/adafruit_ds2413.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ds2413-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/docs/conf.py` & `adafruit-circuitpython-ds2413-1.2.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-ds2413-1.2.8/docs/index.rst` & `adafruit-circuitpython-ds2413-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/examples/ds2413_direct_access.py` & `adafruit-circuitpython-ds2413-1.2.9/examples/ds2413_direct_access.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/examples/ds2413_simpletest.py` & `adafruit-circuitpython-ds2413-1.2.9/examples/ds2413_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds2413-1.2.8/setup.py` & `adafruit-circuitpython-ds2413-1.2.9/setup.py`

 * *Files identical despite different names*


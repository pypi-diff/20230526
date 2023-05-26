# Comparing `tmp/adafruit-circuitpython-ble-magic-light-0.9.8.tar.gz` & `tmp/adafruit-circuitpython-ble-magic-light-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-magic-light-0.9.8.tar", last modified: Thu Sep 23 19:40:31 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-magic-light-0.9.9.tar", last modified: Mon Nov 15 18:37:49 2021, max compression
```

## Comparing `adafruit-circuitpython-ble-magic-light-0.9.8.tar` & `adafruit-circuitpython-ble-magic-light-0.9.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.407249 adafruit-circuitpython-ble-magic-light-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.407249 adafruit-circuitpython-ble-magic-light-0.9.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.407249 adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.407249 adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4962 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4131 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_ble_magic_light.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4962 2021-09-23 19:40:31.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      927 2021-09-23 19:40:31.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 19:40:31.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-09-23 19:40:31.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-09-23 19:40:31.000000 adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      274 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5508 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      976 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/examples/ble_magic_light_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-23 19:40:31.411249 adafruit-circuitpython-ble-magic-light-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-09-23 19:40:20.000000 adafruit-circuitpython-ble-magic-light-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.102158 adafruit-circuitpython-ble-magic-light-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5136 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_ble_magic_light.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5136 2021-11-15 18:37:48.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2021-11-15 18:37:49.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:37:48.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-15 18:37:48.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-11-15 18:37:48.000000 adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5508 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      976 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1686 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/examples/ble_magic_light_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:37:49.106158 adafruit-circuitpython-ble-magic-light-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2021-11-15 18:37:37.000000 adafruit-circuitpython-ble-magic-light-0.9.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-magic-light-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/build.yml`

 * *Files 15% similar despite different names*

```diff
@@ -38,17 +38,17 @@
       with:
         repository: adafruit/actions-ci-circuitpython-libs
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
-    - name: Pip install pylint, Sphinx, pre-commit
+    - name: Pip install Sphinx, pre-commit
       run: |
-        pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit
+        pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-magic-light-0.9.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-magic-light-0.9.9/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.3.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+    rev: v2.11.1
     hooks:
     -   id: pylint
         name: pylint (library code)
         types: [python]
-        exclude: "^(docs/|examples/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+        args:
+          - --disable=consider-using-f-string
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
+    -   id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
+        types: [python]
+        files: "^examples/"
+        args:
+        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+    -   id: pylint
+        name: pylint (test code)
+        description: Run pylint rules on "tests/*.py" files
+        types: [python]
+        files: "^tests/"
+        args:
+        - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/.pylintrc` & `adafruit-circuitpython-ble-magic-light-0.9.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=12
+min-similarity-lines=4
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-magic-light-0.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/LICENSE` & `adafruit-circuitpython-ble-magic-light-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-magic-light-0.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/PKG-INFO` & `adafruit-circuitpython-ble-magic-light-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-magic-light
-Version: 0.9.8
+Version: 0.9.9
 Summary: BLE service for Magic Light BLE RGB bulbs
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Magic_Light
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_magic_light ble rgb
 Platform: UNKNOWN
@@ -123,14 +123,19 @@
         i = 0
         while active_connection.connected:
             pixels[0] = colorwheel(i % 256)
             i += 1
 
         active_connection = None
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_magic_light/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Magic_Light/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/README.rst` & `adafruit-circuitpython-ble-magic-light-0.9.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -102,14 +102,19 @@
         i = 0
         while active_connection.connected:
             pixels[0] = colorwheel(i % 256)
             i += 1
 
         active_connection = None
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_magic_light/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Magic_Light/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_ble_magic_light.py` & `adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_ble_magic_light.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-magic-light
-Version: 0.9.8
+Version: 0.9.9
 Summary: BLE service for Magic Light BLE RGB bulbs
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Magic_Light
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_magic_light ble rgb
 Platform: UNKNOWN
@@ -123,14 +123,19 @@
         i = 0
         while active_connection.connected:
             pixels[0] = colorwheel(i % 256)
             i += 1
 
         active_connection = None
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_magic_light/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Magic_Light/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/adafruit_circuitpython_ble_magic_light.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-magic-light-0.9.9/adafruit_circuitpython_ble_magic_light.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ble_magic_light.py
 requirements.txt
 setup.py
@@ -24,10 +24,11 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/ble_magic_light_simpletest.py
```

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-magic-light-0.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/docs/conf.py` & `adafruit-circuitpython-ble-magic-light-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/docs/index.rst` & `adafruit-circuitpython-ble-magic-light-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/examples/ble_magic_light_simpletest.py` & `adafruit-circuitpython-ble-magic-light-0.9.9/examples/ble_magic_light_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-magic-light-0.9.8/setup.py` & `adafruit-circuitpython-ble-magic-light-0.9.9/setup.py`

 * *Files identical despite different names*


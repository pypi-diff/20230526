# Comparing `tmp/adafruit-circuitpython-ble-heart-rate-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-ble-heart-rate-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-heart-rate-1.1.8.tar", last modified: Thu Apr  8 22:04:07 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-heart-rate-1.1.9.tar", last modified: Mon Nov 15 18:35:28 2021, max compression
```

## Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8.tar` & `adafruit-circuitpython-ble-heart-rate-1.1.9.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.094134 adafruit-circuitpython-ble-heart-rate-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.098134 adafruit-circuitpython-ble-heart-rate-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.098134 adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6795 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_ble_heart_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.098134 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2021-04-08 22:04:06.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      821 2021-04-08 22:04:07.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-08 22:04:06.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-04-08 22:04:06.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-04-08 22:04:06.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5522 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/examples/ble_heart_rate_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-08 22:04:07.102134 adafruit-circuitpython-ble-heart-rate-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-04-08 22:03:53.000000 adafruit-circuitpython-ble-heart-rate-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.566563 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.566563 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.566563 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.566563 adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     6795 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_ble_heart_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.566563 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2021-11-15 18:35:28.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2021-11-15 18:35:28.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:35:28.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-15 18:35:28.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-11-15 18:35:28.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5522 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1828 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/examples/ble_heart_rate_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:35:28.570564 adafruit-circuitpython-ble-heart-rate-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-11-15 18:35:16.000000 adafruit-circuitpython-ble-heart-rate-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

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
@@ -67,7 +67,9 @@
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         pip install --upgrade setuptools wheel twine readme_renderer testresources
         python setup.py sdist
         python setup.py bdist_wheel --universal
         twine check dist/*
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-heart-rate-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-heart-rate-1.1.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/.pylintrc` & `adafruit-circuitpython-ble-heart-rate-1.1.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-heart-rate-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSE` & `adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-heart-rate-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/PKG-INFO` & `adafruit-circuitpython-ble-heart-rate-1.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,94 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-heart-rate
-Version: 1.1.8
+Version: 1.1.9
 Summary: BLE Heart Rate Service
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_heart_rate/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/actions
-            :alt: Build Status
-        
-        BLE Heart Rate Service
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        .. note:: This library is not available on PyPI yet. Install documentation is included
-           as a standard element. Stay tuned for PyPI availability!
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-ble_heart_rate/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit blinka circuitpython micropython ble_heart_rate ble heart rate
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_heart_rate/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/actions
+    :alt: Build Status
+
+BLE Heart Rate Service
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+.. note:: This library is not available on PyPI yet. Install documentation is included
+   as a standard element. Stay tuned for PyPI availability!
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-ble_heart_rate/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-ble-heart-rate
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-ble-heart-rate
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-ble-heart-rate
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/README.rst` & `adafruit-circuitpython-ble-heart-rate-1.1.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -49,18 +49,23 @@
 .. code-block:: shell
 
     mkdir project-name && cd project-name
     python3 -m venv .env
     source .env/bin/activate
     pip3 install adafruit-circuitpython-ble-heart-rate
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_ble_heart_rate.py` & `adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_ble_heart_rate.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,94 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-heart-rate
-Version: 1.1.8
+Version: 1.1.9
 Summary: BLE Heart Rate Service
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_heart_rate/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/actions
-            :alt: Build Status
-        
-        BLE Heart Rate Service
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        .. note:: This library is not available on PyPI yet. Install documentation is included
-           as a standard element. Stay tuned for PyPI availability!
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-ble_heart_rate/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-ble-heart-rate
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit blinka circuitpython micropython ble_heart_rate ble heart rate
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_heart_rate/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/actions
+    :alt: Build Status
+
+BLE Heart Rate Service
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+.. note:: This library is not available on PyPI yet. Install documentation is included
+   as a standard element. Stay tuned for PyPI availability!
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-ble_heart_rate/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-ble-heart-rate
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-ble-heart-rate
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-ble-heart-rate
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_heart_rate/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_BLE_Heart_Rate/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/adafruit_circuitpython_ble_heart_rate.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-heart-rate-1.1.9/adafruit_circuitpython_ble_heart_rate.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ble_heart_rate.py
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
+.github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ble_heart_rate.egg-info/PKG-INFO
 adafruit_circuitpython_ble_heart_rate.egg-info/SOURCES.txt
 adafruit_circuitpython_ble_heart_rate.egg-info/dependency_links.txt
@@ -22,10 +24,11 @@
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
 examples/ble_heart_rate_simpletest.py
```

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-heart-rate-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/docs/conf.py` & `adafruit-circuitpython-ble-heart-rate-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/docs/index.rst` & `adafruit-circuitpython-ble-heart-rate-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/examples/ble_heart_rate_simpletest.py` & `adafruit-circuitpython-ble-heart-rate-1.1.9/examples/ble_heart_rate_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-heart-rate-1.1.8/setup.py` & `adafruit-circuitpython-ble-heart-rate-1.1.9/setup.py`

 * *Files identical despite different names*


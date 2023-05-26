# Comparing `tmp/adafruit-circuitpython-tcs34725-3.3.8.tar.gz` & `tmp/adafruit-circuitpython-tcs34725-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tcs34725-3.3.8.tar", last modified: Thu Jul  1 21:18:44 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-tcs34725-3.3.9.tar", last modified: Mon Nov 15 18:54:29 2021, max compression
```

## Comparing `adafruit-circuitpython-tcs34725-3.3.8.tar` & `adafruit-circuitpython-tcs34725-3.3.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.432983 adafruit-circuitpython-tcs34725-3.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.424983 adafruit-circuitpython-tcs34725-3.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2021-07-01 21:18:44.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-07-01 21:18:44.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 21:18:44.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-07-01 21:18:44.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-01 21:18:44.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13634 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/adafruit_tcs34725.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5502 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 21:18:44.428983 adafruit-circuitpython-tcs34725-3.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/examples/tcs34725_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-01 21:18:44.432983 adafruit-circuitpython-tcs34725-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-07-01 21:18:33.000000 adafruit-circuitpython-tcs34725-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.369279 adafruit-circuitpython-tcs34725-3.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.369279 adafruit-circuitpython-tcs34725-3.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.369279 adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.369279 adafruit-circuitpython-tcs34725-3.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.369279 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2021-11-15 18:54:29.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-15 18:54:29.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:54:29.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 18:54:29.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-15 18:54:29.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13800 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/adafruit_tcs34725.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/examples/tcs34725_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:54:29.373279 adafruit-circuitpython-tcs34725-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-11-15 18:54:17.000000 adafruit-circuitpython-tcs34725-3.3.9/setup.py
```

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tcs34725-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-tcs34725-3.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tcs34725-3.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/.pylintrc` & `adafruit-circuitpython-tcs34725-3.3.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tcs34725-3.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/LICENSE` & `adafruit-circuitpython-tcs34725-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tcs34725-3.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tcs34725-3.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tcs34725-3.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/README.rst` & `adafruit-circuitpython-tcs34725-3.3.9/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -53,14 +53,19 @@
     pip3 install adafruit-circuitpython-tcs34725
 
 Usage Example
 =============
 
 See examples/tcs34725_simpletest.py for an example of the module's usage.
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/tcs34725/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_tcs34725/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/adafruit_circuitpython_tcs34725.egg-info/SOURCES.txt` & `adafruit-circuitpython-tcs34725-3.3.9/adafruit_circuitpython_tcs34725.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

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
 adafruit_tcs34725.py
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
 examples/tcs34725_simpletest.py
```

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/adafruit_tcs34725.py` & `adafruit-circuitpython-tcs34725-3.3.9/adafruit_tcs34725.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,23 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 import time
 
-import adafruit_bus_device.i2c_device as i2c_device
+from adafruit_bus_device import i2c_device
 from micropython import const
 
+try:
+    from typing import Tuple
+    from busio import I2C
+except ImportError:
+    pass
+
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TCS34725.git"
 
 # Register and command constants:
 _COMMAND_BIT = const(0x80)
 _REGISTER_ENABLE = const(0x00)
 _REGISTER_ATIME = const(0x01)
@@ -103,15 +109,15 @@
     """
 
     # Class-level buffer for reading and writing data with the sensor.
     # This reduces memory allocations but means the code is not re-entrant or
     # thread safe!
     _BUFFER = bytearray(3)
 
-    def __init__(self, i2c, address=0x29):
+    def __init__(self, i2c: I2C, address: int = 0x29):
         self._device = i2c_device.I2CDevice(i2c, address)
         self._active = False
         self.integration_time = 2.4
         self._glass_attenuation = None
         self.glass_attenuation = 1.0
         # Check sensor ID is expectd value.
         sensor_id = self._read_u8(_REGISTER_SENSORID)
@@ -143,20 +149,17 @@
         # A gamma correction of 2.5 is applied to each value as well, first dividing by 255,
         # since gamma is applied to values between 0 and 1
         red = int(pow((int((r / clear) * 256) / 255), 2.5) * 255)
         green = int(pow((int((g / clear) * 256) / 255), 2.5) * 255)
         blue = int(pow((int((b / clear) * 256) / 255), 2.5) * 255)
 
         # Handle possible 8-bit overflow
-        if red > 255:
-            red = 255
-        if green > 255:
-            green = 255
-        if blue > 255:
-            blue = 255
+        red = min(red, 255)
+        green = min(green, 255)
+        blue = min(blue, 255)
         return (red, green, blue)
 
     @property
     def color(self):
         """Read the RGB color detected by the sensor. Returns an int with 8 bits per channel.
         Examples: Red = 16711680 (0xff0000), Green = 65280 (0x00ff00),
         Blue = 255 (0x0000ff), SlateGray = 7372944 (0x708090)
@@ -169,15 +172,15 @@
         """The active state of the sensor.  Boolean value that will
         enable/activate the sensor with a value of True and disable with a
         value of False.
         """
         return self._active
 
     @active.setter
-    def active(self, val):
+    def active(self, val: bool):
         val = bool(val)
         if self._active == val:
             return
         self._active = val
         enable = self._read_u8(_REGISTER_ENABLE)
         if val:
             self._write_u8(_REGISTER_ENABLE, enable | _ENABLE_PON)
@@ -188,15 +191,15 @@
 
     @property
     def integration_time(self):
         """The integration time of the sensor in milliseconds."""
         return self._integration_time
 
     @integration_time.setter
-    def integration_time(self, val):
+    def integration_time(self, val: float):
         if (
             not _INTEGRATION_TIME_THRESHOLD_LOW
             <= val
             <= _INTEGRATION_TIME_THRESHOLD_HIGH
         ):
             raise ValueError(
                 "Integration Time must be between '{0}' and '{1}'".format(
@@ -213,30 +216,30 @@
     def gain(self):
         """The gain of the sensor.  Should be a value of 1, 4, 16,
         or 60.
         """
         return _GAINS[self._read_u8(_REGISTER_CONTROL)]
 
     @gain.setter
-    def gain(self, val):
+    def gain(self, val: int):
         if val not in _GAINS:
             raise ValueError(
                 "Gain should be one of the following values: {0}".format(_GAINS)
             )
         self._write_u8(_REGISTER_CONTROL, _GAINS.index(val))
 
     @property
     def interrupt(self):
         """True if the interrupt is set. Can be set to False (and only False)
         to clear the interrupt.
         """
         return bool(self._read_u8(_REGISTER_STATUS) & _ENABLE_AIEN)
 
     @interrupt.setter
-    def interrupt(self, val):
+    def interrupt(self, val: bool):
         if val:
             raise ValueError(
                 "Interrupt should be set to False in order to clear the interrupt"
             )
         with self._device:
             self._device.write(b"\xe6")
 
@@ -265,15 +268,15 @@
     def cycles(self):
         """The persistence cycles of the sensor."""
         if self._read_u8(_REGISTER_ENABLE) & _ENABLE_AIEN:
             return _CYCLES[self._read_u8(_REGISTER_APERS) & 0x0F]
         return -1
 
     @cycles.setter
-    def cycles(self, val):
+    def cycles(self, val: int):
         enable = self._read_u8(_REGISTER_ENABLE)
         if val == -1:
             self._write_u8(_REGISTER_ENABLE, enable & ~(_ENABLE_AIEN))
         else:
             if val not in _CYCLES:
                 raise ValueError(
                     "Only the following cycles are permitted: {0}".format(_CYCLES)
@@ -285,29 +288,29 @@
     def min_value(self):
         """The minimum threshold value (AILT register) of the
         sensor as a 16-bit unsigned value.
         """
         return self._read_u16(_REGISTER_AILT)
 
     @min_value.setter
-    def min_value(self, val):
+    def min_value(self, val: int):
         self._write_u16(_REGISTER_AILT, val)
 
     @property
     def max_value(self):
         """The minimum threshold value (AIHT register) of the
         sensor as a 16-bit unsigned value.
         """
         return self._read_u16(_REGISTER_AIHT)
 
     @max_value.setter
-    def max_value(self, val):
+    def max_value(self, val: int):
         self._write_u16(_REGISTER_AIHT, val)
 
-    def _temperature_and_lux_dn40(self):
+    def _temperature_and_lux_dn40(self) -> Tuple[float, float]:
         """Converts the raw R/G/B values to color temperature in degrees
         Kelvin using the algorithm described in DN40 from Taos (now AMS).
         Also computes lux. Returns tuple with both values or tuple of Nones
         if computation can not be done.
         """
         # pylint: disable=invalid-name, too-many-locals
 
@@ -363,44 +366,44 @@
         of 50% gives GA = 1 / 0.50 = 2. If no glass is present, use GA = 1.
         See Application Note: DN40-Rev 1.0 – Lux and CCT Calculations using
         ams Color Sensors for more details.
         """
         return self._glass_attenuation
 
     @glass_attenuation.setter
-    def glass_attenuation(self, value):
+    def glass_attenuation(self, value: float):
         if value < 1:
             raise ValueError("Glass attenuation factor must be at least 1.")
         self._glass_attenuation = value
 
-    def _valid(self):
+    def _valid(self) -> bool:
         # Check if the status bit is set and the chip is ready.
         return bool(self._read_u8(_REGISTER_STATUS) & 0x01)
 
-    def _read_u8(self, address):
+    def _read_u8(self, address: int) -> int:
         # Read an 8-bit unsigned value from the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = (address | _COMMAND_BIT) & 0xFF
             i2c.write_then_readinto(self._BUFFER, self._BUFFER, out_end=1, in_end=1)
         return self._BUFFER[0]
 
-    def _read_u16(self, address):
+    def _read_u16(self, address: int) -> int:
         # Read a 16-bit unsigned value from the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = (address | _COMMAND_BIT) & 0xFF
             i2c.write_then_readinto(self._BUFFER, self._BUFFER, out_end=1, in_end=2)
         return (self._BUFFER[1] << 8) | self._BUFFER[0]
 
-    def _write_u8(self, address, val):
+    def _write_u8(self, address: int, val: int):
         # Write an 8-bit unsigned value to the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = (address | _COMMAND_BIT) & 0xFF
             self._BUFFER[1] = val & 0xFF
             i2c.write(self._BUFFER, end=2)
 
-    def _write_u16(self, address, val):
+    def _write_u16(self, address: int, val: int):
         # Write a 16-bit unsigned value to the specified 8-bit address.
         with self._device as i2c:
             self._BUFFER[0] = (address | _COMMAND_BIT) & 0xFF
             self._BUFFER[1] = val & 0xFF
             self._BUFFER[2] = (val >> 8) & 0xFF
             i2c.write(self._BUFFER)
```

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tcs34725-3.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/docs/conf.py` & `adafruit-circuitpython-tcs34725-3.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/docs/index.rst` & `adafruit-circuitpython-tcs34725-3.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/examples/tcs34725_simpletest.py` & `adafruit-circuitpython-tcs34725-3.3.9/examples/tcs34725_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tcs34725-3.3.8/setup.py` & `adafruit-circuitpython-tcs34725-3.3.9/setup.py`

 * *Files identical despite different names*


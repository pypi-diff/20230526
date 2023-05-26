# Comparing `tmp/adafruit-circuitpython-fram-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-fram-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fram-1.3.8.tar", last modified: Tue Mar 16 18:54:45 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-fram-1.3.9.tar", last modified: Mon Nov 15 18:44:15 2021, max compression
```

## Comparing `adafruit-circuitpython-fram-1.3.8.tar` & `adafruit-circuitpython-fram-1.3.9.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.814303 adafruit-circuitpython-fram-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16231 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2021-03-16 18:54:45.000000 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-03-16 18:54:45.000000 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-16 18:54:45.000000 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-03-16 18:54:45.000000 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-16 18:54:45.000000 adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    13780 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/adafruit_fram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/examples/fram_i2c_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/examples/fram_spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-16 18:54:45.818303 adafruit-circuitpython-fram-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-03-16 18:54:36.000000 adafruit-circuitpython-fram-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.393546 adafruit-circuitpython-fram-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.393546 adafruit-circuitpython-fram-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.393546 adafruit-circuitpython-fram-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.393546 adafruit-circuitpython-fram-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2021-11-15 18:44:15.000000 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-11-15 18:44:15.000000 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:44:15.000000 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 18:44:15.000000 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-15 18:44:15.000000 adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13780 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/adafruit_fram.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/examples/fram_i2c_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/examples/fram_spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:44:15.397546 adafruit-circuitpython-fram-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-11-15 18:44:04.000000 adafruit-circuitpython-fram-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-fram-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-fram-1.3.9/.github/workflows/build.yml`

 * *Files 13% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
+    - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
-        python-version: 3.6
+        python-version: 3.7
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
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

### Comparing `adafruit-circuitpython-fram-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-fram-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-fram-1.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-fram-1.3.8/.pylintrc` & `adafruit-circuitpython-fram-1.3.9/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
-# jobs=1
-jobs=2
+jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
 load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
@@ -52,15 +51,15 @@
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
```

### Comparing `adafruit-circuitpython-fram-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fram-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/LICENSE` & `adafruit-circuitpython-fram-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fram-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-fram-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fram-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/PKG-INFO` & `adafruit-circuitpython-fram-1.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,97 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fram
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FRAM
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-fram/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/fram/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/actions/
-            :alt: Build Status
-        
-        CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-        
-        Installing from PyPI
-        ====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-fram/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-fram
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-fram
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-fram
-        
-        Usage Example
-        =============
-        
-        See simpletest examples in the ``/examples/`` directory.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit spi fram 12c hardware micropython circuitpython
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
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-fram/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/fram/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/actions/
+    :alt: Build Status
+
+CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+
+Installing from PyPI
+====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-fram/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-fram
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-fram
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-fram
+
+Usage Example
+=============
+
+See simpletest examples in the ``/examples/`` directory.
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/fram/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-fram-1.3.8/README.rst` & `adafruit-circuitpython-fram-1.3.9/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -52,18 +52,23 @@
     pip3 install adafruit-circuitpython-fram
 
 Usage Example
 =============
 
 See simpletest examples in the ``/examples/`` directory.
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/fram/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/PKG-INFO` & `adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,97 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fram
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FRAM
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-fram/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/fram/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/actions/
-            :alt: Build Status
-        
-        CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
-        
-        Installing from PyPI
-        ====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-fram/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-fram
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-fram
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-fram
-        
-        Usage Example
-        =============
-        
-        See simpletest examples in the ``/examples/`` directory.
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/master/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit spi fram 12c hardware micropython circuitpython
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
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-fram/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/fram/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_FRAM/actions/
+    :alt: Build Status
+
+CircuitPython/Python library to support the I2C and SPI FRAM Breakouts.
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
+
+Installing from PyPI
+====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-fram/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-fram
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-fram
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-fram
+
+Usage Example
+=============
+
+See simpletest examples in the ``/examples/`` directory.
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/fram/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_FRAM/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-fram-1.3.8/adafruit_circuitpython_fram.egg-info/SOURCES.txt` & `adafruit-circuitpython-fram-1.3.9/adafruit_circuitpython_fram.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

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
 adafruit_fram.py
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
+.github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_fram.egg-info/PKG-INFO
 adafruit_circuitpython_fram.egg-info/SOURCES.txt
 adafruit_circuitpython_fram.egg-info/dependency_links.txt
@@ -22,11 +24,12 @@
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
 examples/fram_i2c_simpletest.py
 examples/fram_spi_simpletest.py
```

### Comparing `adafruit-circuitpython-fram-1.3.8/adafruit_fram.py` & `adafruit-circuitpython-fram-1.3.9/adafruit_fram.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-fram-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/docs/conf.py` & `adafruit-circuitpython-fram-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/docs/index.rst` & `adafruit-circuitpython-fram-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/examples/fram_i2c_simpletest.py` & `adafruit-circuitpython-fram-1.3.9/examples/fram_i2c_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/examples/fram_spi_simpletest.py` & `adafruit-circuitpython-fram-1.3.9/examples/fram_spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fram-1.3.8/setup.py` & `adafruit-circuitpython-fram-1.3.9/setup.py`

 * *Files identical despite different names*


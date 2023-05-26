# Comparing `tmp/adafruit-circuitpython-ahtx0-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-ahtx0-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ahtx0-1.0.8.tar", last modified: Mon Nov 15 17:34:47 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ahtx0-1.0.9.tar", last modified: Fri Feb  4 19:46:18 2022, max compression
```

## Comparing `adafruit-circuitpython-ahtx0-1.0.8.tar` & `adafruit-circuitpython-ahtx0-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.232556 adafruit-circuitpython-ahtx0-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.232556 adafruit-circuitpython-ahtx0-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.232556 adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.232556 adafruit-circuitpython-ahtx0-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     4800 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_ahtx0.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-11-15 17:34:46.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-11-15 17:34:47.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 17:34:46.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-15 17:34:46.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-15 17:34:46.000000 adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/examples/ahtx0_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 17:34:47.236556 adafruit-circuitpython-ahtx0-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2021-11-15 17:34:32.000000 adafruit-circuitpython-ahtx0-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.682409 adafruit-circuitpython-ahtx0-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.686410 adafruit-circuitpython-ahtx0-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.686410 adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.686410 adafruit-circuitpython-ahtx0-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     4800 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_ahtx0.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.686410 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-02-04 19:46:18.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 19:46:18.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 19:46:18.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 19:46:18.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-04 19:46:18.000000 adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5636 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/examples/ahtx0_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 19:46:18.690410 adafruit-circuitpython-ahtx0-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-02-04 19:46:06.000000 adafruit-circuitpython-ahtx0-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ahtx0-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-ahtx0-1.0.9/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.6
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
@@ -63,15 +63,15 @@
     - uses: actions/checkout@v1
     - name: Check For setup.py
       id: need-pypi
       run: |
         echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
     - name: Set up Python
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ahtx0-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/.pylintrc` & `adafruit-circuitpython-ahtx0-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ahtx0-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/LICENSE` & `adafruit-circuitpython-ahtx0-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ahtx0-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ahtx0-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ahtx0-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/PKG-INFO` & `adafruit-circuitpython-ahtx0-1.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ahtx0
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for the Adafruit AHT10 Humidity and Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AHTx0
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ahtx0 aht10 humidity temperature sensor
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ahtx0/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/
+    :target: https://docs.circuitpython.org/projects/ahtx0/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/workflows/Build%20CI/badge.svg
@@ -95,15 +93,15 @@
         print("Humidity: %0.1f %%" % sensor.relative_humidity)
         time.sleep(2)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ahtx0/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/README.rst` & `adafruit-circuitpython-ahtx0-1.0.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ahtx0/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/
+    :target: https://docs.circuitpython.org/projects/ahtx0/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/workflows/Build%20CI/badge.svg
@@ -74,15 +74,15 @@
         print("Humidity: %0.1f %%" % sensor.relative_humidity)
         time.sleep(2)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ahtx0/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/adafruit_ahtx0.py` & `adafruit-circuitpython-ahtx0-1.0.9/adafruit_ahtx0.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/PKG-INFO` & `adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ahtx0
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for the Adafruit AHT10 Humidity and Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AHTx0
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ahtx0 aht10 humidity temperature sensor
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ahtx0/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/
+    :target: https://docs.circuitpython.org/projects/ahtx0/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/workflows/Build%20CI/badge.svg
@@ -95,15 +93,15 @@
         print("Humidity: %0.1f %%" % sensor.relative_humidity)
         time.sleep(2)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ahtx0/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ahtx0/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/adafruit_circuitpython_ahtx0.egg-info/SOURCES.txt` & `adafruit-circuitpython-ahtx0-1.0.9/adafruit_circuitpython_ahtx0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ahtx0-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/docs/conf.py` & `adafruit-circuitpython-ahtx0-1.0.9/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "BusDevice": (
-        "https://circuitpython.readthedocs.io/projects/busdevice/en/latest/",
+        "https://docs.circuitpython.org/projects/busdevice/en/latest/",
         None,
     ),
     "Register": (
-        "https://circuitpython.readthedocs.io/projects/register/en/latest/",
+        "https://docs.circuitpython.org/projects/register/en/latest/",
         None,
     ),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/docs/index.rst` & `adafruit-circuitpython-ahtx0-1.0.9/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Adafruit AHT20 - Temperature & Humidity Sensor Breakout Board <https://www.adafruit.com/product/4566>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_AHTx0/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ahtx0-1.0.8/setup.py` & `adafruit-circuitpython-ahtx0-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Hardware",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython ahtx0 aht10 humidity temperature "
     "sensor",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     # TODO: IF LIBRARY FILES ARE A PACKAGE FOLDER,
```


# Comparing `tmp/adafruit-circuitpython-ads1x15-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-ads1x15-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ads1x15-2.2.8.tar", last modified: Tue Mar  2 23:55:32 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ads1x15-2.2.9.tar", last modified: Thu Oct 28 15:04:20 2021, max compression
```

## Comparing `adafruit-circuitpython-ads1x15-2.2.8.tar` & `adafruit-circuitpython-ads1x15-2.2.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.154443 adafruit-circuitpython-ads1x15-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      189 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4640 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3041 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1015.py
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1115.py
--rw-r--r--   0 runner    (1001) docker     (116)     7010 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1x15.py
--rw-r--r--   0 runner    (1001) docker     (116)     1859 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/analog_in.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4640 2021-03-02 23:55:31.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      997 2021-03-02 23:55:32.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:55:31.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-02 23:55:31.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-03-02 23:55:31.000000 adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      301 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5466 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      326 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     1118 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:55:32.150443 adafruit-circuitpython-ads1x15-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      745 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_ads1115_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)     2450 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_fast_read.py
--rw-r--r--   0 runner    (1001) docker     (116)     1100 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_gain_example.py
--rw-r--r--   0 runner    (1001) docker     (116)      646 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      152 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:55:32.154443 adafruit-circuitpython-ads1x15-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1890 2021-03-02 23:55:23.000000 adafruit-circuitpython-ads1x15-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.318220 adafruit-circuitpython-ads1x15-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.326220 adafruit-circuitpython-ads1x15-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.330220 adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.330220 adafruit-circuitpython-ads1x15-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4023 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3205 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.330220 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1015.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1115.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7306 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1x15.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2004 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/analog_in.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4023 2021-10-28 15:04:19.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-10-28 15:04:20.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-28 15:04:19.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-28 15:04:19.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-28 15:04:19.000000 adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5466 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_ads1115_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_fast_read.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_gain_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-28 15:04:20.334220 adafruit-circuitpython-ads1x15-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2021-10-28 15:04:03.000000 adafruit-circuitpython-ads1x15-2.2.9/setup.py
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

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

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-ads1x15-2.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ads1x15-2.2.9/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         exclude: "^(docs/|examples/|setup.py$)"
 -   repo: local
     hooks:
     -   id: pylint_examples
         name: pylint (examples code)
         description: Run pylint rules on "examples/*.py" files
         entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
+        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name,consider-using-f-string $example; done)']
         language: system
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/.pylintrc` & `adafruit-circuitpython-ads1x15-2.2.9/.pylintrc`

 * *Files 1% similar despite different names*

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
@@ -249,15 +248,15 @@
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

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ads1x15-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/LICENSE` & `adafruit-circuitpython-ads1x15-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ads1x15-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ads1x15-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ads1x15-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/README.rst` & `adafruit-circuitpython-ads1x15-2.2.9/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -82,18 +82,23 @@
 
     print("{:>5}\t{:>5}".format('raw', 'v'))
 
     while True:
         print("{:>5}\t{:>5.3f}".format(chan.value, chan.voltage))
         time.sleep(0.5)
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ads1x15/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_CircuitPython_ADS1x15/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_CircuitPython_ADS1x15/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1015.py` & `adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1015.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,14 @@
         return r
 
     @property
     def rate_config(self):
         """Rate configuration masks."""
         return _ADS1015_CONFIG_DR
 
-    def _data_rate_default(self):
+    def _data_rate_default(self) -> int:
         return 1600
 
-    def _conversion_value(self, raw_adc):
+    def _conversion_value(self, raw_adc: int) -> int:
         raw_adc = raw_adc.to_bytes(2, "big")
         value = struct.unpack(">h", raw_adc)[0]
         return value >> 4
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1115.py` & `adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1115.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,14 @@
         return r
 
     @property
     def rate_config(self):
         """Rate configuration masks."""
         return _ADS1115_CONFIG_DR
 
-    def _data_rate_default(self):
+    def _data_rate_default(self) -> int:
         return 128
 
-    def _conversion_value(self, raw_adc):
+    def _conversion_value(self, raw_adc: int) -> int:
         raw_adc = raw_adc.to_bytes(2, "big")
         value = struct.unpack(">h", raw_adc)[0]
         return value
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/ads1x15.py` & `adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/ads1x15.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ADS1x15.git"
 
 import time
 from micropython import const
 from adafruit_bus_device.i2c_device import I2CDevice
 
+try:
+    from typing import Optional
+    from busio import I2C
+    from microcontroller import Pin
+except ImportError:
+    pass
+
 _ADS1X15_DEFAULT_ADDRESS = const(0x48)
 _ADS1X15_POINTER_CONVERSION = const(0x00)
 _ADS1X15_POINTER_CONFIG = const(0x01)
 _ADS1X15_CONFIG_OS_SINGLE = const(0x8000)
 _ADS1X15_CONFIG_MUX_OFFSET = const(12)
 _ADS1X15_CONFIG_COMP_QUE_DISABLE = const(0x0003)
 _ADS1X15_CONFIG_GAIN = {
@@ -45,19 +52,19 @@
 
 
 class ADS1x15:
     """Base functionality for ADS1x15 analog to digital converters."""
 
     def __init__(
         self,
-        i2c,
-        gain=1,
-        data_rate=None,
-        mode=Mode.SINGLE,
-        address=_ADS1X15_DEFAULT_ADDRESS,
+        i2c: I2C,
+        gain: float = 1,
+        data_rate: Optional[int] = None,
+        mode: Mode = Mode.SINGLE,
+        address: int = _ADS1X15_DEFAULT_ADDRESS,
     ):
         # pylint: disable=too-many-arguments
         self._last_pin_read = None
         self.buf = bytearray(3)
         self._data_rate = self._gain = self._mode = None
         self.gain = gain
         self.data_rate = self._data_rate_default() if data_rate is None else data_rate
@@ -66,15 +73,15 @@
 
     @property
     def data_rate(self):
         """The data rate for ADC conversion in samples per second."""
         return self._data_rate
 
     @data_rate.setter
-    def data_rate(self, rate):
+    def data_rate(self, rate: int):
         possible_rates = self.rates
         if rate not in possible_rates:
             raise ValueError("Data rate must be one of: {}".format(possible_rates))
         self._data_rate = rate
 
     @property
     def rates(self):
@@ -88,15 +95,15 @@
 
     @property
     def gain(self):
         """The ADC gain."""
         return self._gain
 
     @gain.setter
-    def gain(self, gain):
+    def gain(self, gain: float):
         possible_gains = self.gains
         if gain not in possible_gains:
             raise ValueError("Gain must be one of: {}".format(possible_gains))
         self._gain = gain
 
     @property
     def gains(self):
@@ -107,42 +114,42 @@
 
     @property
     def mode(self):
         """The ADC conversion mode."""
         return self._mode
 
     @mode.setter
-    def mode(self, mode):
+    def mode(self, mode: Mode):
         if mode not in (Mode.CONTINUOUS, Mode.SINGLE):
             raise ValueError("Unsupported mode.")
         self._mode = mode
 
-    def read(self, pin, is_differential=False):
+    def read(self, pin: Pin, is_differential: bool = False) -> int:
         """I2C Interface for ADS1x15-based ADCs reads.
 
         params:
             :param pin: individual or differential pin.
             :param bool is_differential: single-ended or differential read.
         """
         pin = pin if is_differential else pin + 0x04
         return self._read(pin)
 
-    def _data_rate_default(self):
+    def _data_rate_default(self) -> int:
         """Retrieve the default data rate for this ADC (in samples per second).
         Should be implemented by subclasses.
         """
         raise NotImplementedError("Subclasses must implement _data_rate_default!")
 
-    def _conversion_value(self, raw_adc):
+    def _conversion_value(self, raw_adc: int) -> int:
         """Subclasses should override this function that takes the 16 raw ADC
         values of a conversion result and returns a signed integer value.
         """
         raise NotImplementedError("Subclass must implement _conversion_value function!")
 
-    def _read(self, pin):
+    def _read(self, pin: Pin) -> int:
         """Perform an ADC read. Returns the signed integer result of the read."""
         # Immediately return conversion register result if in CONTINUOUS mode
         # and pin has not changed
         if self.mode == Mode.CONTINUOUS and self._last_pin_read == pin:
             return self._conversion_value(self.get_last_result(True))
 
         # Assign last pin read if in SINGLE mode or first sample in CONTINUOUS mode on this pin
@@ -170,38 +177,38 @@
         else:
             # Can't poll registers in CONTINUOUS mode
             # Wait expected time for two conversions to complete
             time.sleep(2 / self.data_rate)
 
         return self._conversion_value(self.get_last_result(False))
 
-    def _conversion_complete(self):
+    def _conversion_complete(self) -> int:
         """Return status of ADC conversion."""
         # OS is bit 15
         # OS = 0: Device is currently performing a conversion
         # OS = 1: Device is not currently performing a conversion
         return self._read_register(_ADS1X15_POINTER_CONFIG) & 0x8000
 
-    def get_last_result(self, fast=False):
+    def get_last_result(self, fast: bool = False) -> int:
         """Read the last conversion result when in continuous conversion mode.
         Will return a signed integer value. If fast is True, the register
         pointer is not updated as part of the read. This reduces I2C traffic
         and increases possible read rate.
         """
         return self._read_register(_ADS1X15_POINTER_CONVERSION, fast)
 
-    def _write_register(self, reg, value):
+    def _write_register(self, reg: int, value: int):
         """Write 16 bit value to register."""
         self.buf[0] = reg
         self.buf[1] = (value >> 8) & 0xFF
         self.buf[2] = value & 0xFF
         with self.i2c_device as i2c:
             i2c.write(self.buf)
 
-    def _read_register(self, reg, fast=False):
+    def _read_register(self, reg: int, fast: bool = False) -> int:
         """Read 16 bit register value. If fast is True, the pointer register
         is not updated.
         """
         with self.i2c_device as i2c:
             if fast:
                 i2c.readinto(self.buf, end=2)
             else:
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/adafruit_ads1x15/analog_in.py` & `adafruit-circuitpython-ads1x15-2.2.9/adafruit_ads1x15/analog_in.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,22 +7,30 @@
 ==============================
 AnalogIn for single-ended and
 differential ADC readings.
 
 * Author(s): Carter Nelson, adapted from MCP3xxx original by Brent Rubell
 """
 
+try:
+    from typing import Optional
+    from .ads1x15 import ADS1x15
+except ImportError:
+    pass
+
 _ADS1X15_DIFF_CHANNELS = {(0, 1): 0, (0, 3): 1, (1, 3): 2, (2, 3): 3}
 _ADS1X15_PGA_RANGE = {2 / 3: 6.144, 1: 4.096, 2: 2.048, 4: 1.024, 8: 0.512, 16: 0.256}
 
 
 class AnalogIn:
     """AnalogIn Mock Implementation for ADC Reads."""
 
-    def __init__(self, ads, positive_pin, negative_pin=None):
+    def __init__(
+        self, ads: ADS1x15, positive_pin: int, negative_pin: Optional[int] = None
+    ):
         """AnalogIn
 
         :param ads: The ads object.
         :param ~digitalio.DigitalInOut positive_pin: Required pin for single-ended.
         :param ~digitalio.DigitalInOut negative_pin: Optional pin for differential reads.
         """
         self._ads = ads
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/adafruit_circuitpython_ads1x15.egg-info/SOURCES.txt` & `adafruit-circuitpython-ads1x15-2.2.9/adafruit_circuitpython_ads1x15.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 .readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
+.github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_ads1x15/__init__.py
 adafruit_ads1x15/ads1015.py
 adafruit_ads1x15/ads1115.py
```

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ads1x15-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/docs/conf.py` & `adafruit-circuitpython-ads1x15-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/docs/index.rst` & `adafruit-circuitpython-ads1x15-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_ads1115_simpletest.py` & `adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_ads1115_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_fast_read.py` & `adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_fast_read.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_gain_example.py` & `adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_gain_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/examples/ads1x15_simpletest.py` & `adafruit-circuitpython-ads1x15-2.2.9/examples/ads1x15_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ads1x15-2.2.8/setup.py` & `adafruit-circuitpython-ads1x15-2.2.9/setup.py`

 * *Files identical despite different names*


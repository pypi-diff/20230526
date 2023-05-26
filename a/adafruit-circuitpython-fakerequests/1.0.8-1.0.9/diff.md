# Comparing `tmp/adafruit-circuitpython-fakerequests-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-fakerequests-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fakerequests-1.0.8.tar", last modified: Thu Jun  9 18:37:19 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-fakerequests-1.0.9.tar", last modified: Tue Aug  9 19:58:07 2022, max compression
```

## Comparing `adafruit-circuitpython-fakerequests-1.0.8.tar` & `adafruit-circuitpython-fakerequests-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.579911 adafruit-circuitpython-fakerequests-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.583911 adafruit-circuitpython-fakerequests-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.583911 adafruit-circuitpython-fakerequests-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.583911 adafruit-circuitpython-fakerequests-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-06-09 18:37:19.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-06-09 18:37:19.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:37:19.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 18:37:19.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-09 18:37:19.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/adafruit_fakerequests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5612 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_advancedtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_i2c_database.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_i2c_database.txt.license
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:37:19.587911 adafruit-circuitpython-fakerequests-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-06-09 18:37:09.000000 adafruit-circuitpython-fakerequests-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.574116 adafruit-circuitpython-fakerequests-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-08-09 19:58:07.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-09 19:58:07.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:58:07.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:58:07.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-09 19:58:07.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-09 19:57:59.000000 adafruit-circuitpython-fakerequests-1.0.9/adafruit_fakerequests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5612 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-08-09 19:57:59.000000 adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_advancedtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_i2c_database.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_i2c_database.txt.license
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-08-09 19:57:59.000000 adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-08-09 19:57:59.000000 adafruit-circuitpython-fakerequests-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:57:53.000000 adafruit-circuitpython-fakerequests-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:58:07.578116 adafruit-circuitpython-fakerequests-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fakerequests-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-fakerequests-1.0.9/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -43,28 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
+    - name: Archive bundles
+      uses: actions/upload-artifact@v2
+      with:
+        name: bundles
+        path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/.gitignore` & `adafruit-circuitpython-fakerequests-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-fakerequests-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/.pylintrc` & `adafruit-circuitpython-fakerequests-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fakerequests-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/LICENSE` & `adafruit-circuitpython-fakerequests-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fakerequests-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-fakerequests-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fakerequests-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/PKG-INFO` & `adafruit-circuitpython-fakerequests-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fakerequests
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fake Network Requests helper that retrieves data from a local file.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython fakerequests fake requests file network internet http
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests
+Keywords: adafruit,blinka,circuitpython,micropython,fakerequests,fake,requests,file,network,internet,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-fakerequests/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/fakerequests/en/latest/
@@ -66,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-fakerequests
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fakerequests
 
 Usage Example
 =============
 
 .. code:: python
 
@@ -93,9 +92,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/README.rst` & `adafruit-circuitpython-fakerequests-1.0.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     sudo pip3 install adafruit-circuitpython-fakerequests
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fakerequests
 
 Usage Example
 =============
 
 .. code:: python
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/PKG-INFO` & `adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fakerequests
-Version: 1.0.8
+Version: 1.0.9
 Summary: Fake Network Requests helper that retrieves data from a local file.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython fakerequests fake requests file network internet http
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests
+Keywords: adafruit,blinka,circuitpython,micropython,fakerequests,fake,requests,file,network,internet,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-fakerequests/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/fakerequests/en/latest/
@@ -66,16 +65,16 @@
     sudo pip3 install adafruit-circuitpython-fakerequests
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-fakerequests
 
 Usage Example
 =============
 
 .. code:: python
 
@@ -93,9 +92,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/adafruit_circuitpython_fakerequests.egg-info/SOURCES.txt` & `adafruit-circuitpython-fakerequests-1.0.9/adafruit_circuitpython_fakerequests.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_fakerequests.py
+optional_requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/adafruit_fakerequests.py` & `adafruit-circuitpython-fakerequests-1.0.9/adafruit_fakerequests.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import json
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FakeRequests.git"
 
 
 class Fake_Requests:
     """For faking 'requests' using a local file instead of the network."""
 
     def __init__(self, filename):
```

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-fakerequests-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/docs/conf.py` & `adafruit-circuitpython-fakerequests-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/docs/index.rst` & `adafruit-circuitpython-fakerequests-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_advancedtest.py` & `adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fakerequests-1.0.8/examples/fakerequests_i2c_database.txt` & `adafruit-circuitpython-fakerequests-1.0.9/examples/fakerequests_i2c_database.txt`

 * *Files identical despite different names*


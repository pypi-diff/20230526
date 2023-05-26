# Comparing `tmp/adafruit-circuitpython-neokey-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-neokey-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neokey-1.0.8.tar", last modified: Fri Jun 17 17:17:14 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-neokey-1.0.9.tar", last modified: Tue Aug  9 19:58:52 2022, max compression
```

## Comparing `adafruit-circuitpython-neokey-1.0.8.tar` & `adafruit-circuitpython-neokey-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.539350 adafruit-circuitpython-neokey-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.539350 adafruit-circuitpython-neokey-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.539350 adafruit-circuitpython-neokey-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.539350 adafruit-circuitpython-neokey-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3365 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3365 2022-06-17 17:17:14.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-06-17 17:17:14.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 17:17:14.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-17 17:17:14.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-17 17:17:14.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/adafruit_neokey/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_neokey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/adafruit_neokey/neokey1x4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5667 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/examples/neokey1x4_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/examples/neokey_1x4_multikey.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 17:17:14.543350 adafruit-circuitpython-neokey-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-06-17 17:17:04.000000 adafruit-circuitpython-neokey-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.139067 adafruit-circuitpython-neokey-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.139067 adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/neokey1x4.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5667 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/examples/neokey1x4_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/examples/neokey_1x4_multikey.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-neokey-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-neokey-1.0.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
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
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
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

### Comparing `adafruit-circuitpython-neokey-1.0.8/.gitignore` & `adafruit-circuitpython-neokey-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-neokey-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/.pylintrc` & `adafruit-circuitpython-neokey-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neokey-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/LICENSE` & `adafruit-circuitpython-neokey-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neokey-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-neokey-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neokey-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/PKG-INFO` & `adafruit-circuitpython-neokey-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neokey
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython library for using Adafruit NeoKey.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit neokey neopixel mechanical keyboard led rgbsensor hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
+Keywords: adafruit,neokey,neopixel,mechanical,keyboard,led,rgbsensor,hardware,micropython,circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-neokey/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/neokey/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 This is a library for using the Adafruit NeoKey boards with circuitpython.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-neokey
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-neokey
 
 Usage Example
 =============
 
 see examples/neokey1x4_simpletest.py for usage example
 
@@ -86,9 +89,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-neokey-1.0.8/README.rst` & `adafruit-circuitpython-neokey-1.0.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 This is a library for using the Adafruit NeoKey boards with circuitpython.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -45,16 +49,16 @@
     sudo pip3 install adafruit-circuitpython-neokey
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-neokey
 
 Usage Example
 =============
 
 see examples/neokey1x4_simpletest.py for usage example
```

### Comparing `adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/PKG-INFO` & `adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neokey
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython library for using Adafruit NeoKey.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit neokey neopixel mechanical keyboard led rgbsensor hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
+Keywords: adafruit,neokey,neopixel,mechanical,keyboard,led,rgbsensor,hardware,micropython,circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-neokey/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/neokey/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 This is a library for using the Adafruit NeoKey boards with circuitpython.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-neokey
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-neokey
 
 Usage Example
 =============
 
 see examples/neokey1x4_simpletest.py for usage example
 
@@ -86,9 +89,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_NeoKey/blob/master/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-neokey-1.0.8/adafruit_circuitpython_neokey.egg-info/SOURCES.txt` & `adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+pyproject.toml
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

### Comparing `adafruit-circuitpython-neokey-1.0.8/adafruit_neokey/neokey1x4.py` & `adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/neokey1x4.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
 # imports
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoKey.git"
 
 from micropython import const
 from adafruit_seesaw import neopixel
 from adafruit_seesaw.seesaw import Seesaw
 
 try:
```

### Comparing `adafruit-circuitpython-neokey-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/docs/conf.py` & `adafruit-circuitpython-neokey-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/docs/index.rst` & `adafruit-circuitpython-neokey-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/examples/neokey1x4_simpletest.py` & `adafruit-circuitpython-neokey-1.0.9/examples/neokey1x4_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.8/examples/neokey_1x4_multikey.py` & `adafruit-circuitpython-neokey-1.0.9/examples/neokey_1x4_multikey.py`

 * *Files identical despite different names*


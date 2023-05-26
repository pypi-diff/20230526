# Comparing `tmp/adafruit-circuitpython-mcp4725-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-mcp4725-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp4725-1.4.8.tar", last modified: Tue Aug  9 19:47:37 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp4725-1.4.9.tar", last modified: Mon Aug 22 18:43:14 2022, max compression
```

## Comparing `adafruit-circuitpython-mcp4725-1.4.8.tar` & `adafruit-circuitpython-mcp4725-1.4.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.851314 adafruit-circuitpython-mcp4725-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-08-09 19:47:37.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-09 19:47:37.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:47:37.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 19:47:37.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-09 19:47:37.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-08-09 19:47:30.000000 adafruit-circuitpython-mcp4725-1.4.8/adafruit_mcp4725.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-08-09 19:47:30.000000 adafruit-circuitpython-mcp4725-1.4.8/examples/mcp4725_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-09 19:47:30.000000 adafruit-circuitpython-mcp4725-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-09 19:47:22.000000 adafruit-circuitpython-mcp4725-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:47:37.855314 adafruit-circuitpython-mcp4725-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:14.000139 adafruit-circuitpython-mcp4725-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.992138 adafruit-circuitpython-mcp4725-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.996139 adafruit-circuitpython-mcp4725-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.996139 adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.996139 adafruit-circuitpython-mcp4725-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-08-22 18:43:14.000139 adafruit-circuitpython-mcp4725-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.996139 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-08-22 18:43:13.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-22 18:43:13.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:43:13.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:43:13.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:43:13.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-08-22 18:43:05.000000 adafruit-circuitpython-mcp4725-1.4.9/adafruit_mcp4725.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:13.996139 adafruit-circuitpython-mcp4725-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:14.000139 adafruit-circuitpython-mcp4725-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:43:14.000139 adafruit-circuitpython-mcp4725-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-08-22 18:43:05.000000 adafruit-circuitpython-mcp4725-1.4.9/examples/mcp4725_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-22 18:43:05.000000 adafruit-circuitpython-mcp4725-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:42:58.000000 adafruit-circuitpython-mcp4725-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:43:14.000139 adafruit-circuitpython-mcp4725-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp4725-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+            sed -i -e "s/0.0.0+auto.0/1.2.3/" $file;
         done;
         python -m build
         twine check dist/*
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-mcp4725-1.4.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+            sed -i -e "s/0.0.0+auto.0/${{github.event.release.tag_name}}/" $file;
         done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.gitignore` & `adafruit-circuitpython-mcp4725-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp4725-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/.pylintrc` & `adafruit-circuitpython-mcp4725-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp4725-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/LICENSE` & `adafruit-circuitpython-mcp4725-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp4725-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp4725-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp4725-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/PKG-INFO` & `adafruit-circuitpython-mcp4725-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4725
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for MCP4725 digital to analog converter.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4725
 Keywords: adafruit,mcp4725,digital,analog,converter,dac,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/README.rst` & `adafruit-circuitpython-mcp4725-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4725
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for MCP4725 digital to analog converter.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4725
 Keywords: adafruit,mcp4725,digital,analog,converter,dac,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/adafruit_circuitpython_mcp4725.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp4725-1.4.9/adafruit_circuitpython_mcp4725.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/adafruit_mcp4725.py` & `adafruit-circuitpython-mcp4725-1.4.9/adafruit_mcp4725.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 """
 import time
 from micropython import const
 from adafruit_bus_device import i2c_device
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4725.git"
 
 
 # Internal constants:
 _MCP4725_DEFAULT_ADDRESS = 0b01100010
 _MCP4725_WRITE_FAST_MODE = const(0b00000000)
 _MCP4725_WRITE_DAC_EEPROM = const(0b01100000)
```

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp4725-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/docs/conf.py` & `adafruit-circuitpython-mcp4725-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/docs/index.rst` & `adafruit-circuitpython-mcp4725-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/examples/mcp4725_simpletest.py` & `adafruit-circuitpython-mcp4725-1.4.9/examples/mcp4725_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4725-1.4.8/pyproject.toml` & `adafruit-circuitpython-mcp4725-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp4725"
 description = "CircuitPython library for MCP4725 digital to analog converter."
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4725"}
 keywords = [
     "adafruit",
```


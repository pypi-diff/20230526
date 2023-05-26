# Comparing `tmp/adafruit-circuitpython-bme680-3.4.8.tar.gz` & `tmp/adafruit-circuitpython-bme680-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bme680-3.4.8.tar", last modified: Tue Aug  9 19:34:10 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bme680-3.4.9.tar", last modified: Mon Aug 22 18:37:04 2022, max compression
```

## Comparing `adafruit-circuitpython-bme680-3.4.8.tar` & `adafruit-circuitpython-bme680-3.4.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.647823 adafruit-circuitpython-bme680-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.651824 adafruit-circuitpython-bme680-3.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.651824 adafruit-circuitpython-bme680-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    20289 2022-08-09 19:34:01.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_bme680.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-09 19:34:10.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-09 19:34:10.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:34:10.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-09 19:34:10.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:34:10.000000 adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-09 19:34:01.000000 adafruit-circuitpython-bme680-3.4.8/examples/bme680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-09 19:34:01.000000 adafruit-circuitpython-bme680-3.4.8/examples/bme680_spi.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-09 19:34:01.000000 adafruit-circuitpython-bme680-3.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-09 19:33:53.000000 adafruit-circuitpython-bme680-3.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:34:10.655824 adafruit-circuitpython-bme680-3.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.270232 adafruit-circuitpython-bme680-3.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3222 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    20289 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_bme680.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:37:04.000000 adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5189 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/examples/bme680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/examples/bme680_spi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-08-22 18:36:56.000000 adafruit-circuitpython-bme680-3.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:36:49.000000 adafruit-circuitpython-bme680-3.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:37:04.274232 adafruit-circuitpython-bme680-3.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-bme680-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bme680-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-bme680-3.4.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-bme680-3.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-bme680-3.4.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-bme680-3.4.8/.gitignore` & `adafruit-circuitpython-bme680-3.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bme680-3.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/.pylintrc` & `adafruit-circuitpython-bme680-3.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bme680-3.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/LICENSE` & `adafruit-circuitpython-bme680-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bme680-3.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bme680-3.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bme680-3.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/PKG-INFO` & `adafruit-circuitpython-bme680-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.4.8/README.rst` & `adafruit-circuitpython-bme680-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/adafruit_bme680.py` & `adafruit-circuitpython-bme680-3.4.9/adafruit_bme680.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from circuitpython_typing import ReadableBuffer
     from busio import I2C, SPI
     from digitalio import DigitalInOut
 
 except ImportError:
     pass
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BME680.git"
 
 
 #    I2C ADDRESS/BITS/SETTINGS
 #    -----------------------------------------------------------------------
 _BME680_CHIPID = const(0x61)
```

### Comparing `adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/PKG-INFO` & `adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.4.8/adafruit_circuitpython_bme680.egg-info/SOURCES.txt` & `adafruit-circuitpython-bme680-3.4.9/adafruit_circuitpython_bme680.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bme680-3.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/docs/conf.py` & `adafruit-circuitpython-bme680-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/docs/index.rst` & `adafruit-circuitpython-bme680-3.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/examples/bme680_simpletest.py` & `adafruit-circuitpython-bme680-3.4.9/examples/bme680_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/examples/bme680_spi.py` & `adafruit-circuitpython-bme680-3.4.9/examples/bme680_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.4.8/pyproject.toml` & `adafruit-circuitpython-bme680-3.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bme680"
 description = "CircuitPython driver for BME680 sensor over I2C"
-version = "3.4.8"
+version = "3.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BME680"}
 keywords = [
     "adafruit",
```


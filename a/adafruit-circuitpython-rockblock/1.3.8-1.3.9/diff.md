# Comparing `tmp/adafruit-circuitpython-rockblock-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-rockblock-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-rockblock-1.3.8.tar", last modified: Tue Aug  9 19:54:51 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-rockblock-1.3.9.tar", last modified: Mon Aug 22 18:46:41 2022, max compression
```

## Comparing `adafruit-circuitpython-rockblock-1.3.8.tar` & `adafruit-circuitpython-rockblock-1.3.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.907109 adafruit-circuitpython-rockblock-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.907109 adafruit-circuitpython-rockblock-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.907109 adafruit-circuitpython-rockblock-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.907109 adafruit-circuitpython-rockblock-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.907109 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-08-09 19:54:51.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-08-09 19:54:51.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:54:51.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:54:51.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-09 19:54:51.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16630 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/adafruit_rockblock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5414 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_feather_sense_sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_recv_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_recv_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_send_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_send_text.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-09 19:54:44.000000 adafruit-circuitpython-rockblock-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:54:37.000000 adafruit-circuitpython-rockblock-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:54:51.911109 adafruit-circuitpython-rockblock-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.365759 adafruit-circuitpython-rockblock-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.369759 adafruit-circuitpython-rockblock-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.369759 adafruit-circuitpython-rockblock-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.369759 adafruit-circuitpython-rockblock-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.369759 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-08-22 18:46:41.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-08-22 18:46:41.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:46:41.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 18:46:41.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-22 18:46:41.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16630 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/adafruit_rockblock.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5414 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_feather_sense_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_recv_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_recv_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_send_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_send_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-22 18:46:31.000000 adafruit-circuitpython-rockblock-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:46:21.000000 adafruit-circuitpython-rockblock-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:46:41.373759 adafruit-circuitpython-rockblock-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-rockblock-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-rockblock-1.3.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-rockblock-1.3.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.gitignore` & `adafruit-circuitpython-rockblock-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-rockblock-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/.pylintrc` & `adafruit-circuitpython-rockblock-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rockblock-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/LICENSE` & `adafruit-circuitpython-rockblock-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-rockblock-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-rockblock-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-rockblock-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/PKG-INFO` & `adafruit-circuitpython-rockblock-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rockblock
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython driver for Rock Seven RockBLOCK Iridium satellite modem
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_RockBlock
 Keywords: adafruit,blinka,circuitpython,micropython,rockblock,iridium,,satellite
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-rockblock-1.3.8/README.rst` & `adafruit-circuitpython-rockblock-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/PKG-INFO` & `adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rockblock
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython driver for Rock Seven RockBLOCK Iridium satellite modem
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_RockBlock
 Keywords: adafruit,blinka,circuitpython,micropython,rockblock,iridium,,satellite
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-rockblock-1.3.8/adafruit_circuitpython_rockblock.egg-info/SOURCES.txt` & `adafruit-circuitpython-rockblock-1.3.9/adafruit_circuitpython_rockblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/adafruit_rockblock.py` & `adafruit-circuitpython-rockblock-1.3.9/adafruit_rockblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """
 
 
 import time
 import struct
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RockBlock.git"
 
 
 class RockBlock:
     """Driver for RockBLOCK Iridium satellite modem."""
 
     def __init__(self, uart, baudrate=19200):
```

### Comparing `adafruit-circuitpython-rockblock-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-rockblock-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/docs/conf.py` & `adafruit-circuitpython-rockblock-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/docs/index.rst` & `adafruit-circuitpython-rockblock-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_feather_sense_sensors.py` & `adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_feather_sense_sensors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_recv_data.py` & `adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_recv_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_recv_text.py` & `adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_recv_text.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_send_data.py` & `adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_send_data.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/examples/rockblock_send_text.py` & `adafruit-circuitpython-rockblock-1.3.9/examples/rockblock_send_text.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rockblock-1.3.8/pyproject.toml` & `adafruit-circuitpython-rockblock-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-rockblock"
 description = "CircuitPython driver for Rock Seven RockBLOCK Iridium satellite modem"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_RockBlock"}
 keywords = [
     "adafruit",
```


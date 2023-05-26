# Comparing `tmp/adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8.tar.gz` & `tmp/adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8.tar", last modified: Fri Feb  4 19:54:19 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9.tar", last modified: Mon May  2 20:10:40 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8.tar` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.806604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.806604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.806604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.806604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_ble_berrymed_pulse_oximeter/
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_ble_berrymed_pulse_oximeter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_ble_berrymed_pulse_oximeter/adafruit_ble_transparent_uart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-02-04 19:54:19.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-02-04 19:54:19.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 19:54:19.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-04 19:54:19.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-04 19:54:19.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/examples/ble_berrymed_pulse_oximeter_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 19:54:19.810604 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-02-04 19:54:05.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.439916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3387 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_ble_berrymed_pulse_oximeter/
+-rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_ble_berrymed_pulse_oximeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_ble_berrymed_pulse_oximeter/adafruit_ble_transparent_uart.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3387 2022-05-02 20:10:40.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-02 20:10:40.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-02 20:10:40.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-02 20:10:40.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-05-02 20:10:40.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/examples/ble_berrymed_pulse_oximeter_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-02 20:10:40.447916 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-05-02 20:10:29.000000 adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
 -   repo: https://github.com/python/black
-    rev: 20.8b1
+    rev: 22.3.0
     hooks:
     - id: black
 -   repo: https://github.com/fsfe/reuse-tool
     rev: v0.12.1
     hooks:
     - id: reuse
 -   repo: https://github.com/pre-commit/pre-commit-hooks
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/.pylintrc` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSE` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/PKG-INFO` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-berrymed-pulse-oximeter
-Version: 2.0.8
+Version: 2.0.9
 Summary: BLE Support for BerryMed Pulse Oximeter Service
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_berrymed_pulse_oximeter ble pulse oximeter berrymed spo2
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble-berrymed_pulse_oximeter/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/actions
     :alt: Build Status
 
@@ -74,20 +74,17 @@
     pip3 install adafruit-circuitpython-ble-berrymed-pulse-oximeter
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/README.rst` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,34 @@
+Metadata-Version: 2.1
+Name: adafruit-circuitpython-ble-berrymed-pulse-oximeter
+Version: 2.0.9
+Summary: BLE Support for BerryMed Pulse Oximeter Service
+Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter
+Author: Adafruit Industries
+Author-email: circuitpython@adafruit.com
+License: MIT
+Keywords: adafruit blinka circuitpython micropython ble_berrymed_pulse_oximeter ble pulse oximeter berrymed spo2
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble-berrymed_pulse_oximeter/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/actions
     :alt: Build Status
 
@@ -55,18 +74,17 @@
     pip3 install adafruit-circuitpython-ble-berrymed-pulse-oximeter
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
 
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_ble_berrymed_pulse_oximeter/__init__.py` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_ble_berrymed_pulse_oximeter/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_ble_berrymed_pulse_oximeter/adafruit_ble_transparent_uart.py` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_ble_berrymed_pulse_oximeter/adafruit_ble_transparent_uart.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 """
 
 from adafruit_ble import Service
 from adafruit_ble.uuid import VendorUUID
 from adafruit_ble.characteristics.stream import StreamOut, StreamIn
 
+try:
+    from typing import Optional
+except ImportError:
+    pass
+from circuitpython_typing import ReadableBuffer, WriteableBuffer
+
 __version__ = "0.0.0-auto.0"
 __repo__ = (
     "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Contec_Pulse_Oximeter.git"
 )
 
 
 class TransparentUARTService(Service):
@@ -40,60 +46,62 @@
     )
     _server_rx = StreamIn(
         uuid=VendorUUID("49535343-8841-43F4-A8D4-ECBE34729BB3"),
         timeout=1.0,
         buffer_size=64,
     )
 
-    def __init__(self, service=None):
+    def __init__(self, service: Optional["TransparentUARTService"] = None):
         super().__init__(service=service)
         self.connectable = True
         if not service:
             self._rx = self._server_rx
             self._tx = self._server_tx
         else:
             # If we're a client then swap the characteristics we use.
             self._tx = self._server_rx
             self._rx = self._server_tx
 
-    def read(self, nbytes=None):
+    def read(self, nbytes: Optional[int] = None) -> Optional[bytes]:
         """
         Read characters. If ``nbytes`` is specified then read at most that many bytes.
         Otherwise, read everything that arrives until the connection times out.
         Providing the number of bytes expected is highly recommended because it will be faster.
 
         :return: Data read
         :rtype: bytes or None
         """
         return self._rx.read(nbytes)
 
-    def readinto(self, buf, nbytes=None):
+    def readinto(
+        self, buf: WriteableBuffer, nbytes: Optional[int] = None
+    ) -> Optional[int]:
         """
         Read bytes into the ``buf``. If ``nbytes`` is specified then read at most
         that many bytes. Otherwise, read at most ``len(buf)`` bytes.
 
         :return: number of bytes read and stored into ``buf``
         :rtype: int or None (on a non-blocking error)
         """
         return self._rx.readinto(buf, nbytes)
 
-    def readline(self):
+    def readline(self) -> Optional[bytes]:
         """
         Read a line, ending in a newline character.
 
         :return: the line read
         :rtype: bytes or None
         """
         return self._rx.readline()
 
     @property
-    def in_waiting(self):
+    def in_waiting(self) -> int:
         """The number of bytes in the input buffer, available to be read."""
         return self._rx.in_waiting
 
-    def reset_input_buffer(self):
+    def reset_input_buffer(self) -> None:
         """Discard any unread characters in the input buffer."""
         self._rx.reset_input_buffer()
 
-    def write(self, buf):
+    def write(self, buf: ReadableBuffer) -> None:
         """Write a buffer of bytes."""
         self._tx.write(buf)
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,15 @@
-Metadata-Version: 2.1
-Name: adafruit-circuitpython-ble-berrymed-pulse-oximeter
-Version: 2.0.8
-Summary: BLE Support for BerryMed Pulse Oximeter Service
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
-License: MIT
-Keywords: adafruit blinka circuitpython micropython ble_berrymed_pulse_oximeter ble pulse oximeter berrymed spo2
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble-berrymed_pulse_oximeter/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/actions
     :alt: Build Status
 
@@ -74,20 +55,15 @@
     pip3 install adafruit-circuitpython-ble-berrymed-pulse-oximeter
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_berrymed_pulse_oximeter/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
-
```

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/adafruit_circuitpython_ble_berrymed_pulse_oximeter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/conf.py` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/docs/index.rst` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/examples/ble_berrymed_pulse_oximeter_simpletest.py` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/examples/ble_berrymed_pulse_oximeter_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.8/setup.py` & `adafruit-circuitpython-ble-berrymed-pulse-oximeter-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_CircuitPython_BLE_BerryMed_Pulse_Oximeter",
     # Author details
     author="Adafruit Industries",
     author_email="circuitpython@adafruit.com",
-    install_requires=["Adafruit-Blinka", "adafruit-circuitpython-ble"],
+    install_requires=["Adafruit-Blinka>=7.2.3", "adafruit-circuitpython-ble"],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
```


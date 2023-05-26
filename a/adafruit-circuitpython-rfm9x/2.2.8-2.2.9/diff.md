# Comparing `tmp/adafruit-circuitpython-rfm9x-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-rfm9x-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-rfm9x-2.2.8.tar", last modified: Wed Jul  6 18:35:27 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-rfm9x-2.2.9.tar", last modified: Sat Jul 23 04:41:58 2022, max compression
```

## Comparing `adafruit-circuitpython-rfm9x-2.2.8.tar` & `adafruit-circuitpython-rfm9x-2.2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.781104 adafruit-circuitpython-rfm9x-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.785104 adafruit-circuitpython-rfm9x-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.785104 adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16257 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.785104 adafruit-circuitpython-rfm9x-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4361 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.785104 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-07-06 18:35:27.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-07-06 18:35:27.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 18:35:27.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-06 18:35:27.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-06 18:35:27.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    38308 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/adafruit_rfm9x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1_ack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1_bonnet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node2_ack.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_rpi_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_rpi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_transmit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-06 18:35:13.000000 adafruit-circuitpython-rfm9x-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-06 18:35:27.789104 adafruit-circuitpython-rfm9x-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.198798 adafruit-circuitpython-rfm9x-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.190798 adafruit-circuitpython-rfm9x-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16257 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-07-23 04:41:58.198798 adafruit-circuitpython-rfm9x-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4363 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2022-07-23 04:41:58.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-07-23 04:41:58.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 04:41:58.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-07-23 04:41:58.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-07-23 04:41:58.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    38301 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/adafruit_rfm9x.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.194798 adafruit-circuitpython-rfm9x-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 04:41:58.198798 adafruit-circuitpython-rfm9x-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1_ack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3555 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1_bonnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node2_ack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_rpi_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_rpi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_transmit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-07-23 04:41:51.000000 adafruit-circuitpython-rfm9x-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-23 04:41:39.000000 adafruit-circuitpython-rfm9x-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-23 04:41:58.198798 adafruit-circuitpython-rfm9x-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-rfm9x-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
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
@@ -64,11 +66,12 @@
       id: need-pypi
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
         python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-rfm9x-2.2.9/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -77,9 +77,12 @@
         pip install --upgrade build twine
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+        done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.gitignore` & `adafruit-circuitpython-rfm9x-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-rfm9x-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/.pylintrc` & `adafruit-circuitpython-rfm9x-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rfm9x-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/LICENSE` & `adafruit-circuitpython-rfm9x-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-rfm9x-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-rfm9x-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-rfm9x-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/PKG-INFO` & `adafruit-circuitpython-rfm9x-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rfm9x
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for RFM95/6/7/8 LoRa 433/915mhz radio modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_RFM9x
 Keywords: adafruit,lora,radio,rfm95,rfm9x,rfm96,rfm97,rfm98,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -60,16 +60,16 @@
     sudo pip3 install adafruit-circuitpython-rfm9x
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-rfm9x
 
 Usage Example
 =============
 
 Initialization of the RFM radio requires specifying a frequency appropriate to
 your radio hardware (i.e. 868-915 or 433 MHz) and specifying the pins used in your
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/README.rst` & `adafruit-circuitpython-rfm9x-2.2.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     sudo pip3 install adafruit-circuitpython-rfm9x
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-rfm9x
 
 Usage Example
 =============
 
 Initialization of the RFM radio requires specifying a frequency appropriate to
 your radio hardware (i.e. 868-915 or 433 MHz) and specifying the pins used in your
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/PKG-INFO` & `adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rfm9x
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for RFM95/6/7/8 LoRa 433/915mhz radio modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_RFM9x
 Keywords: adafruit,lora,radio,rfm95,rfm9x,rfm96,rfm97,rfm98,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -60,16 +60,16 @@
     sudo pip3 install adafruit-circuitpython-rfm9x
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-rfm9x
 
 Usage Example
 =============
 
 Initialization of the RFM radio requires specifying a frequency appropriate to
 your radio hardware (i.e. 868-915 or 433 MHz) and specifying the pins used in your
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/adafruit_circuitpython_rfm9x.egg-info/SOURCES.txt` & `adafruit-circuitpython-rfm9x-2.2.9/adafruit_circuitpython_rfm9x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/adafruit_rfm9x.py` & `adafruit-circuitpython-rfm9x-2.2.9/adafruit_rfm9x.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         from typing import Literal
     except ImportError:
         from typing_extensions import Literal
 
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RFM9x.git"
 
 # Internal constants:
 # Register names (FSK Mode even though we use LoRa instead, from table 85)
 _RH_RF95_REG_00_FIFO = const(0x00)
 _RH_RF95_REG_01_OP_MODE = const(0x01)
 _RH_RF95_REG_06_FRF_MSB = const(0x06)
```

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-rfm9x-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/docs/conf.py` & `adafruit-circuitpython-rfm9x-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/docs/index.rst` & `adafruit-circuitpython-rfm9x-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_header.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_header.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1_ack.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1_ack.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node1_bonnet.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node1_bonnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node2.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_node2_ack.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_node2_ack.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_rpi_interrupt.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_rpi_interrupt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_rpi_simpletest.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_rpi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_simpletest.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/examples/rfm9x_transmit.py` & `adafruit-circuitpython-rfm9x-2.2.9/examples/rfm9x_transmit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rfm9x-2.2.8/pyproject.toml` & `adafruit-circuitpython-rfm9x-2.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-rfm9x"
 description = "CircuitPython library for RFM95/6/7/8 LoRa 433/915mhz radio modules."
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_RFM9x"}
 keywords = [
     "adafruit",
@@ -35,16 +36,14 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
-dynamic = ["version", "dependencies"]
+dynamic = ["dependencies"]
 
 [tool.setuptools]
 py-modules = ["adafruit_rfm9x"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
-
-[tool.setuptools_scm]
```


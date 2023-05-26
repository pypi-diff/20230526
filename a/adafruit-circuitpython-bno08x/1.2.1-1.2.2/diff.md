# Comparing `tmp/adafruit-circuitpython-bno08x-1.2.1.tar.gz` & `tmp/adafruit-circuitpython-bno08x-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.1.tar", last modified: Thu May 18 15:32:01 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bno08x-1.2.2.tar", last modified: Fri May 26 16:08:48 2023, max compression
```

## Comparing `adafruit-circuitpython-bno08x-1.2.1.tar` & `adafruit-circuitpython-bno08x-1.2.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.457520 adafruit-circuitpython-bno08x-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/
--rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:32:01.000000 adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_find_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_more_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_quaternion_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:31:53.000000 adafruit-circuitpython-bno08x-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:31:43.000000 adafruit-circuitpython-bno08x-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:32:01.461520 adafruit-circuitpython-bno08x-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.829193 adafruit-circuitpython-bno08x-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.821193 adafruit-circuitpython-bno08x-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.821193 adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/
+-rw-r--r--   0 runner    (1001) docker     (123)    38910 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:08:48.000000 adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:48.825193 adafruit-circuitpython-bno08x-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_find_heading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_more_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_quaternion_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 16:08:41.000000 adafruit-circuitpython-bno08x-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:08:31.000000 adafruit-circuitpython-bno08x-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:08:48.829193 adafruit-circuitpython-bno08x-1.2.2/setup.cfg
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bno08x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/.gitignore` & `adafruit-circuitpython-bno08x-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/.pre-commit-config.yaml` & `adafruit-circuitpython-bno08x-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/.pylintrc` & `adafruit-circuitpython-bno08x-1.2.2/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bno08x-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/LICENSE` & `adafruit-circuitpython-bno08x-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bno08x-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/LICENSES/MIT.txt` & `adafruit-circuitpython-bno08x-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bno08x-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.1
+Version: 1.2.2
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/README.rst` & `adafruit-circuitpython-bno08x-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/__init__.py` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https:# github.com/adafruit/circuitpython/releases
 
 * `Adafruit's Bus Device library <https:# github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
 """
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https:# github.com/adafruit/Adafruit_CircuitPython_BNO08x.git"
 
 from struct import unpack_from, pack_into
 from collections import namedtuple
 import time
 from micropython import const
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/debug.py` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/debug.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/i2c.py` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/spi.py` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_bno08x/uart.py` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_bno08x/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/PKG-INFO` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bno08x
-Version: 1.2.1
+Version: 1.2.2
 Summary: Helper library for the Hillcrest Laboratories BNO08x IMUs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BNO08x
 Keywords: adafruit,blinka,circuitpython,micropython,bno080,IMU,BNO055,SENSOR,FUSION,VR,MOTION,TRACK,BNO085
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt` & `adafruit-circuitpython-bno08x-1.2.2/adafruit_circuitpython_bno08x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/docs/_static/favicon.ico` & `adafruit-circuitpython-bno08x-1.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/docs/conf.py` & `adafruit-circuitpython-bno08x-1.2.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 autodoc_mock_imports = ["busio", "micropython", "struct"]
```

### Comparing `adafruit-circuitpython-bno08x-1.2.1/docs/index.rst` & `adafruit-circuitpython-bno08x-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_calibration.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_find_heading.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_find_heading.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_more_reports.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_more_reports.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_quaternion_service.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_quaternion_service.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_spi.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/examples/bno08x_simpletest_uart.py` & `adafruit-circuitpython-bno08x-1.2.2/examples/bno08x_simpletest_uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bno08x-1.2.1/pyproject.toml` & `adafruit-circuitpython-bno08x-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bno08x"
 description = "Helper library for the Hillcrest Laboratories BNO08x IMUs"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BNO08x"}
 keywords = [
     "adafruit",
```


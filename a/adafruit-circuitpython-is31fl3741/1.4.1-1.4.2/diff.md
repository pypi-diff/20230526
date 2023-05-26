# Comparing `tmp/adafruit-circuitpython-is31fl3741-1.4.1.tar.gz` & `tmp/adafruit-circuitpython-is31fl3741-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-is31fl3741-1.4.1.tar", last modified: Mon Apr 17 21:44:59 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-is31fl3741-1.4.2.tar", last modified: Fri May 26 16:26:36 2023, max compression
```

## Comparing `adafruit-circuitpython-is31fl3741-1.4.1.tar` & `adafruit-circuitpython-is31fl3741-1.4.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.020238 adafruit-circuitpython-is31fl3741-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.012237 adafruit-circuitpython-is31fl3741-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-17 21:44:59.020238 adafruit-circuitpython-is31fl3741-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-17 21:44:58.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-17 21:44:59.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 21:44:58.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 21:44:58.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 21:44:58.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/adafruit_ledglasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/adafruit_rgbmatrixqt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/is31fl3741_pixelbuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/issi_evb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/led_glasses_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/led_glasses_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.016237 adafruit-circuitpython-is31fl3741-1.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.020238 adafruit-circuitpython-is31fl3741-1.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 21:44:59.020238 adafruit-circuitpython-is31fl3741-1.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_13x9_sequential_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_glassesrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_native.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_all_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_animation_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_led_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbswirl.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/scrolly.bdf
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/examples/scrolly.bdf.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-17 21:44:51.000000 adafruit-circuitpython-is31fl3741-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 21:44:42.000000 adafruit-circuitpython-is31fl3741-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 21:44:59.020238 adafruit-circuitpython-is31fl3741-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.161524 adafruit-circuitpython-is31fl3741-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.165524 adafruit-circuitpython-is31fl3741-1.4.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.165524 adafruit-circuitpython-is31fl3741-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.165524 adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.165524 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-26 16:26:36.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-26 16:26:36.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:26:36.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-26 16:26:36.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:26:36.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/adafruit_ledglasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/adafruit_rgbmatrixqt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/is31fl3741_pixelbuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/issi_evb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/led_glasses_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/led_glasses_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_13x9_sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_glassesrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_all_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_animation_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_led_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbswirl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/scrolly.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/examples/scrolly.bdf.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-26 16:26:28.000000 adafruit-circuitpython-is31fl3741-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 16:26:18.000000 adafruit-circuitpython-is31fl3741-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:26:36.169524 adafruit-circuitpython-is31fl3741-1.4.2/setup.cfg
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-is31fl3741-1.4.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/.gitignore` & `adafruit-circuitpython-is31fl3741-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/.pre-commit-config.yaml` & `adafruit-circuitpython-is31fl3741-1.4.2/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/.pylintrc` & `adafruit-circuitpython-is31fl3741-1.4.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-is31fl3741-1.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/LICENSE` & `adafruit-circuitpython-is31fl3741-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/MIT.txt` & `adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-is31fl3741-1.4.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/PKG-INFO` & `adafruit-circuitpython-is31fl3741-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3741
-Version: 1.4.1
+Version: 1.4.2
 Summary: CircuitPython library for IS31FL3741 RGB LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3741
 Keywords: adafruit,is31fl3741,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/README.rst` & `adafruit-circuitpython-is31fl3741-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/PKG-INFO` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3741
-Version: 1.4.1
+Version: 1.4.2
 Summary: CircuitPython library for IS31FL3741 RGB LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3741
 Keywords: adafruit,is31fl3741,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_circuitpython_is31fl3741.egg-info/SOURCES.txt` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_circuitpython_is31fl3741.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/__init__.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from circuitpython_typing.pil import Image
     from circuitpython_typing import ReadableBuffer
     from adafruit_framebuf import FrameBuffer
     import busio
 except ImportError:
     pass
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3741.git"
 
 _IS3741_ADDR_DEFAULT = 0x30
 
 _IS3741_COMMANDREGISTER = 0xFD
 _IS3741_COMMANDREGISTERLOCK = 0xFE
 _IS3741_INTMASKREGISTER = 0xF0
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/adafruit_ledglasses.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/adafruit_ledglasses.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/adafruit_rgbmatrixqt.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/adafruit_rgbmatrixqt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/is31fl3741_pixelbuf.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/is31fl3741_pixelbuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import TracebackType
     import is31fl3741
     from . import IS31FL3741
 except ImportError:
     pass
 
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 # __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3741.git"
 
 
 # Pixel color order constants
 BGR = "BGR"
 """Blue Green Red"""
 RGB = "RGB"
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/issi_evb.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/issi_evb.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/led_glasses_animation.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/led_glasses_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/adafruit_is31fl3741/led_glasses_map.py` & `adafruit-circuitpython-is31fl3741-1.4.2/adafruit_is31fl3741/led_glasses_map.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/docs/_static/favicon.ico` & `adafruit-circuitpython-is31fl3741-1.4.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/docs/conf.py` & `adafruit-circuitpython-is31fl3741-1.4.2/docs/conf.py`

 * *Files 2% similar despite different names*

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
     "sphinx.ext.viewcode",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
```

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/docs/examples.rst` & `adafruit-circuitpython-is31fl3741-1.4.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/docs/index.rst` & `adafruit-circuitpython-is31fl3741-1.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_13x9_sequential_chain.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_13x9_sequential_chain.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_animation.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_glassesrings.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_glassesrings.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_native.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_native.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_all_animations.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_all_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_animation_sequence.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_animation_sequence.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbmatrix_led_animation.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbmatrix_led_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_rgbswirl.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_rgbswirl.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/is31fl3741_simpletest.py` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/is31fl3741_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/examples/scrolly.bdf` & `adafruit-circuitpython-is31fl3741-1.4.2/examples/scrolly.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3741-1.4.1/pyproject.toml` & `adafruit-circuitpython-is31fl3741-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-is31fl3741"
 description = "CircuitPython library for IS31FL3741 RGB LED matrices."
-version = "1.4.1"
+version = "1.4.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3741"}
 keywords = [
     "adafruit",
```


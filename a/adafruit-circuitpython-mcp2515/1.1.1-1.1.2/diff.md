# Comparing `tmp/adafruit-circuitpython-mcp2515-1.1.1.tar.gz` & `tmp/adafruit-circuitpython-mcp2515-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp2515-1.1.1.tar", last modified: Mon Apr 24 19:17:30 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp2515-1.1.2.tar", last modified: Fri May 26 16:06:29 2023, max compression
```

## Comparing `adafruit-circuitpython-mcp2515-1.1.1.tar` & `adafruit-circuitpython-mcp2515-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.129586 adafruit-circuitpython-mcp2515-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/
--rw-r--r--   0 runner    (1001) docker     (123)    31200 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_canio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_loopback_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_receive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_send_and_receive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.001947 adafruit-circuitpython-mcp2515-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-26 16:06:28.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 16:06:28.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:06:28.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:06:28.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:06:28.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/
+-rw-r--r--   0 runner    (1001) docker     (123)    31200 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.005946 adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/canio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_canio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_loopback_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_send_and_receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 16:06:20.000000 adafruit-circuitpython-mcp2515-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:06:09.000000 adafruit-circuitpython-mcp2515-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:06:29.009945 adafruit-circuitpython-mcp2515-1.1.2/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp2515-1.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/.gitignore` & `adafruit-circuitpython-mcp2515-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp2515-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/.pylintrc` & `adafruit-circuitpython-mcp2515-1.1.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp2515-1.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/LICENSE` & `adafruit-circuitpython-mcp2515-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp2515-1.1.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp2515-1.1.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp2515-1.1.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/PKG-INFO` & `adafruit-circuitpython-mcp2515-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp2515
-Version: 1.1.1
+Version: 1.1.2
 Summary: A CircuitPython library for working with the MCP2515 CAN bus controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP2515
 Keywords: adafruit,blinka,circuitpython,micropython,mcp2515,CAN,CANBUS,OBD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/README.rst` & `adafruit-circuitpython-mcp2515-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp2515
-Version: 1.1.1
+Version: 1.1.2
 Summary: A CircuitPython library for working with the MCP2515 CAN bus controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP2515
 Keywords: adafruit,blinka,circuitpython,micropython,mcp2515,CAN,CANBUS,OBD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp2515-1.1.2/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/__init__.py` & `adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .timer import Timer
 
 try:
     from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP2515.git"
 
 # modes
 _MODE_NORMAL = const(0x00)
 _MODE_SLEEP = const(0x20)
 _MODE_LOOPBACK = const(0x40)
 _MODE_LISTENONLY = const(0x60)
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/__init__.py` & `adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/canio/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/timer.py` & `adafruit-circuitpython-mcp2515-1.1.2/adafruit_mcp2515/timer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp2515-1.1.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/docs/conf.py` & `adafruit-circuitpython-mcp2515-1.1.2/docs/conf.py`

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
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst` & `adafruit-circuitpython-mcp2515-1.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_canio_test.py` & `adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_canio_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_loopback_test.py` & `adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_loopback_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_receive.py` & `adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_receive.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_send_and_receive.py` & `adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_send_and_receive.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_simpletest.py` & `adafruit-circuitpython-mcp2515-1.1.2/examples/mcp2515_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.1/pyproject.toml` & `adafruit-circuitpython-mcp2515-1.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp2515"
 description = "A CircuitPython library for working with the MCP2515 CAN bus controller"
-version = "1.1.1"
+version = "1.1.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP2515"}
 keywords = [
     "adafruit",
```


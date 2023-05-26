# Comparing `tmp/adafruit-circuitpython-emc2101-1.2.1.tar.gz` & `tmp/adafruit-circuitpython-emc2101-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-emc2101-1.2.1.tar", last modified: Mon Nov 28 18:13:18 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-emc2101-1.2.2.tar", last modified: Fri May 26 15:57:55 2023, max compression
```

## Comparing `adafruit-circuitpython-emc2101-1.2.1.tar` & `adafruit-circuitpython-emc2101-1.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.203998 adafruit-circuitpython-emc2101-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.207998 adafruit-circuitpython-emc2101-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.207998 adafruit-circuitpython-emc2101-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6192 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.207998 adafruit-circuitpython-emc2101-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4814 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.207998 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4814 2022-11-28 18:13:18.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2022-11-28 18:13:18.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:13:18.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:13:18.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:13:18.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/
--rw-r--r--   0 runner    (1001) docker     (122)    18710 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_enums.py
--rw-r--r--   0 runner    (1001) docker     (122)    15344 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     6749 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_fanspeed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7420 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_lut.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_regs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5987 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      906 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_lut_example.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_set_pwm_freq.py
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-11-28 18:13:09.000000 adafruit-circuitpython-emc2101-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:12:53.000000 adafruit-circuitpython-emc2101-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:13:18.211998 adafruit-circuitpython-emc2101-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.397550 adafruit-circuitpython-emc2101-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.401550 adafruit-circuitpython-emc2101-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.401550 adafruit-circuitpython-emc2101-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.401550 adafruit-circuitpython-emc2101-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.401550 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-26 15:57:55.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 15:57:55.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:55.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 15:57:55.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:57:55.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.401550 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/
+-rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_fanspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_lut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_regs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_lut_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_set_pwm_freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 15:57:48.000000 adafruit-circuitpython-emc2101-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:57:39.000000 adafruit-circuitpython-emc2101-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:55.405550 adafruit-circuitpython-emc2101-1.2.2/setup.cfg
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-emc2101-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/.gitignore` & `adafruit-circuitpython-emc2101-1.2.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/.pre-commit-config.yaml` & `adafruit-circuitpython-emc2101-1.2.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-emc2101-1.2.1/.pylintrc` & `adafruit-circuitpython-emc2101-1.2.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-emc2101-1.2.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-emc2101-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/LICENSE` & `adafruit-circuitpython-emc2101-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-emc2101-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/LICENSES/MIT.txt` & `adafruit-circuitpython-emc2101-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-emc2101-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/PKG-INFO` & `adafruit-circuitpython-emc2101-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-emc2101
-Version: 1.2.1
+Version: 1.2.2
 Summary: Brushless fan controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_EMC2101
 Keywords: adafruit,blinka,circuitpython,micropython,emc2101,Fan,Controller,RPM,Noctua,Sunon,Cooling,Thermostat,PWM,Tach
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/README.rst` & `adafruit-circuitpython-emc2101-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/PKG-INFO` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-emc2101
-Version: 1.2.1
+Version: 1.2.2
 Summary: Brushless fan controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_EMC2101
 Keywords: adafruit,blinka,circuitpython,micropython,emc2101,Fan,Controller,RPM,Noctua,Sunon,Cooling,Thermostat,PWM,Tach
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_circuitpython_emc2101.egg-info/SOURCES.txt` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_circuitpython_emc2101.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/__init__.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from adafruit_register.i2c_struct import ROUnaryStruct, UnaryStruct
 from adafruit_register.i2c_bit import RWBit
 from adafruit_register.i2c_bits import RWBits
 import adafruit_bus_device.i2c_device as i2cdevice
 
 from adafruit_emc2101 import emc2101_regs
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_EMC2101.git"
 
 
 class EMC2101:  # pylint: disable=too-many-instance-attributes
     """Basic driver for the EMC2101 Fan Controller.
 
     :param ~busio.I2C i2c_bus: The I2C bus the EMC is connected to.
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_enums.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_enums.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_ext.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_ext.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_fanspeed.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_fanspeed.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_lut.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_lut.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from adafruit_register.i2c_struct import UnaryStruct
 
 from adafruit_emc2101 import emc2101_regs
 from adafruit_emc2101.emc2101_fanspeed import FanSpeedLUT
 from adafruit_emc2101.emc2101_ext import EMC2101_EXT
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_EMC2101.git"
 
 
 class EMC2101_LUT(EMC2101_EXT):  # pylint: disable=too-many-instance-attributes
     """Driver for the EMC2101 Fan Controller, with PWM frequency and temperature
     look-up-table (LUT) control.
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/adafruit_emc2101/emc2101_regs.py` & `adafruit-circuitpython-emc2101-1.2.2/adafruit_emc2101/emc2101_regs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/docs/_static/favicon.ico` & `adafruit-circuitpython-emc2101-1.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/docs/api.rst` & `adafruit-circuitpython-emc2101-1.2.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/docs/conf.py` & `adafruit-circuitpython-emc2101-1.2.2/docs/conf.py`

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
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-emc2101-1.2.1/docs/examples.rst` & `adafruit-circuitpython-emc2101-1.2.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/docs/index.rst` & `adafruit-circuitpython-emc2101-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_lut_example.py` & `adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_lut_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_set_pwm_freq.py` & `adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_set_pwm_freq.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/examples/emc2101_simpletest.py` & `adafruit-circuitpython-emc2101-1.2.2/examples/emc2101_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-emc2101-1.2.1/pyproject.toml` & `adafruit-circuitpython-emc2101-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-emc2101"
 description = "Brushless fan controller"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_EMC2101"}
 keywords = [
     "adafruit",
```


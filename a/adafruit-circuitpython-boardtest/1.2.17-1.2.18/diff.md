# Comparing `tmp/adafruit-circuitpython-boardtest-1.2.17.tar.gz` & `tmp/adafruit-circuitpython-boardtest-1.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-boardtest-1.2.17.tar", last modified: Tue May 16 17:48:06 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-boardtest-1.2.18.tar", last modified: Fri May 26 16:08:53 2023, max compression
```

## Comparing `adafruit-circuitpython-boardtest-1.2.17.tar` & `adafruit-circuitpython-boardtest-1.2.18.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.810864 adafruit-circuitpython-boardtest-1.2.17/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_led.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_voltage_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz.license
--rw-r--r--   0 runner    (1001) docker     (123)   168217 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png.license
--rw-r--r--   0 runner    (1001) docker     (123)   149724 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/examples/boardtest_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.846222 adafruit-circuitpython-boardtest-1.2.18/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.846222 adafruit-circuitpython-boardtest-1.2.18/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.850222 adafruit-circuitpython-boardtest-1.2.18/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.850222 adafruit-circuitpython-boardtest-1.2.18/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.850222 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_sd_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_voltage_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.850222 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-26 16:08:53.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-26 16:08:53.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:08:53.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 16:08:53.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 16:08:53.000000 adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.fzz
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.fzz.license
+-rw-r--r--   0 runner    (1001) docker     (123)   168217 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)   149724 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig_bb.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/docs/test_jig_bb.png.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/examples/boardtest_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 16:08:46.000000 adafruit-circuitpython-boardtest-1.2.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:08:33.000000 adafruit-circuitpython-boardtest-1.2.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:08:53.854222 adafruit-circuitpython-boardtest-1.2.18/setup.cfg
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-boardtest-1.2.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/.gitignore` & `adafruit-circuitpython-boardtest-1.2.18/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/.pre-commit-config.yaml` & `adafruit-circuitpython-boardtest-1.2.18/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/.pylintrc` & `adafruit-circuitpython-boardtest-1.2.18/.pylintrc`

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

### Comparing `adafruit-circuitpython-boardtest-1.2.17/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-boardtest-1.2.18/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/LICENSE` & `adafruit-circuitpython-boardtest-1.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-boardtest-1.2.18/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/LICENSES/MIT.txt` & `adafruit-circuitpython-boardtest-1.2.18/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/LICENSES/Unlicense.txt` & `adafruit-circuitpython-boardtest-1.2.18/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/PKG-INFO` & `adafruit-circuitpython-boardtest-1.2.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-boardtest
-Version: 1.2.17
+Version: 1.2.18
 Summary: Helper for verifying a board definition works as expected
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BoardTest
 Keywords: adafruit,boardtest,board,test,testing,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/README.rst` & `adafruit-circuitpython-boardtest-1.2.18/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_gpio.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_gpio.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import supervisor
 
 try:
     from typing import Any, Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 LED_ON_DELAY_TIME = 0.2  # Seconds
 LED_OFF_DELAY_TIME = 0.2  # Seconds
 LED_PIN_NAMES = ["L", "LED", "RED_LED", "GREEN_LED", "BLUE_LED"]
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_i2c.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_i2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import busio
 
 try:
     from typing import Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 SDA_PIN_NAME = "SDA"
 SCL_PIN_NAME = "SCL"
 NUM_I2C_TESTS = 10  # Number of times to write and read EEPROM values
 EEPROM_I2C_MAX_ADDR = 255  # Self-imposed max memory address
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_led.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_led.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import supervisor
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 LED_ON_DELAY_TIME = 0.2  # Seconds
 LED_OFF_DELAY_TIME = 0.2  # Seconds
 LED_PIN_NAMES = ["L", "LED", "RED_LED", "YELLOW_LED", "GREEN_LED", "BLUE_LED"]
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_sd.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import storage
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 MOSI_PIN_NAME = "SD_MOSI"
 MISO_PIN_NAME = "SD_MISO"
 SCK_PIN_NAME = "SD_SCK"
 CS_PIN_NAME = "SD_CS"
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd_cd.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_sd_cd.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import digitalio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 SD_CD_PIN_NAME = "SD_CD"
 
 # Test result strings
 PASS = "PASS"
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_spi.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import busio
 
 try:
     from typing import Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 MOSI_PIN_NAME = "MOSI"
 MISO_PIN_NAME = "MISO"
 SCK_PIN_NAME = "SCK"
 CS_PIN_NAME = "D2"
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_uart.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_uart.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import busio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 TX_PIN_NAME = "TX"
 RX_PIN_NAME = "RX"
 BAUD_RATE = 9600
 NUM_UART_BYTES = 40  # Number of bytes to transmit over UART
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_voltage_monitor.py` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_boardtest/boardtest_voltage_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import analogio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.17"
+__version__ = "1.2.18"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 VOLTAGE_MONITOR_PIN_NAMES = ["VOLTAGE_MONITOR", "BATTERY"]
 ANALOG_REF = 3.3  # Reference analog voltage
 ANALOGIN_BITS = 16  # ADC resolution (bits) for CircuitPython
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/PKG-INFO` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-boardtest
-Version: 1.2.17
+Version: 1.2.18
 Summary: Helper for verifying a board definition works as expected
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BoardTest
 Keywords: adafruit,boardtest,board,test,testing,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt` & `adafruit-circuitpython-boardtest-1.2.18/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico` & `adafruit-circuitpython-boardtest-1.2.18/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/api.rst` & `adafruit-circuitpython-boardtest-1.2.18/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/conf.py` & `adafruit-circuitpython-boardtest-1.2.18/docs/conf.py`

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

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/index.rst` & `adafruit-circuitpython-boardtest-1.2.18/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz` & `adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.fzz`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png` & `adafruit-circuitpython-boardtest-1.2.18/docs/test_jig.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png` & `adafruit-circuitpython-boardtest-1.2.18/docs/test_jig_bb.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/examples/boardtest_simpletest.py` & `adafruit-circuitpython-boardtest-1.2.18/examples/boardtest_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.17/pyproject.toml` & `adafruit-circuitpython-boardtest-1.2.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-boardtest"
 description = "Helper for verifying a board definition works as expected"
-version = "1.2.17"
+version = "1.2.18"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest"}
 keywords = [
     "adafruit",
```


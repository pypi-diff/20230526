# Comparing `tmp/adafruit-circuitpython-pioasm-0.7.8.tar.gz` & `tmp/adafruit-circuitpython-pioasm-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pioasm-0.7.8.tar", last modified: Fri Aug 26 02:49:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pioasm-0.7.9.tar", last modified: Thu Oct  6 18:14:16 2022, max compression
```

## Comparing `adafruit-circuitpython-pioasm-0.7.8.tar` & `adafruit-circuitpython-pioasm-0.7.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-08-26 02:49:08.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-08-26 02:49:08.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:49:08.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:49:08.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:49:08.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12903 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/adafruit_pioasm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.225936 adafruit-circuitpython-pioasm-0.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_7seg.py
--rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_7seg_fader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_background_morse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_blink.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_hello.py
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_i2sout.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_led_brightness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_neopixel_bg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_pdm.py
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_print_c_program.py
--rw-r--r--   0 runner    (1001) docker     (121)     7569 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_pulsegroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_rotaryencoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_rxuart.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_txuart.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_wrap.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:48:52.000000 adafruit-circuitpython-pioasm-0.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:08.229936 adafruit-circuitpython-pioasm-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6489 2022-08-26 02:49:00.000000 adafruit-circuitpython-pioasm-0.7.8/tests/testpioasm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.255794 adafruit-circuitpython-pioasm-0.7.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.247794 adafruit-circuitpython-pioasm-0.7.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-10-06 18:14:16.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-10-06 18:14:16.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 18:14:16.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-06 18:14:16.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-06 18:14:16.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12903 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/adafruit_pioasm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3764 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_7seg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_7seg_fader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_background_morse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_blink.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_i2sout.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_led_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_neopixel_bg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_pdm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_print_c_program.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7569 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_pulsegroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_rotaryencoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_rxuart.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_txuart.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-06 18:13:56.000000 adafruit-circuitpython-pioasm-0.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-06 18:14:16.255794 adafruit-circuitpython-pioasm-0.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:16.251794 adafruit-circuitpython-pioasm-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6489 2022-10-06 18:14:07.000000 adafruit-circuitpython-pioasm-0.7.9/tests/testpioasm.py
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pioasm-0.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.github/workflows/build.yml` & `adafruit-circuitpython-pioasm-0.7.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.github/workflows/release.yml` & `adafruit-circuitpython-pioasm-0.7.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.gitignore` & `adafruit-circuitpython-pioasm-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pioasm-0.7.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/.pylintrc` & `adafruit-circuitpython-pioasm-0.7.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pioasm-0.7.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/LICENSE` & `adafruit-circuitpython-pioasm-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/LICENSES/BSD-3-Clause.txt` & `adafruit-circuitpython-pioasm-0.7.9/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pioasm-0.7.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pioasm-0.7.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pioasm-0.7.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/PKG-INFO` & `adafruit-circuitpython-pioasm-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pioasm
-Version: 0.7.8
+Version: 0.7.9
 Summary: Simple assembler to convert pioasm to bytes
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PIOASM
 Keywords: adafruit,blinka,circuitpython,micropython,pioasm,rp2040
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/README.rst` & `adafruit-circuitpython-pioasm-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/PKG-INFO` & `adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pioasm
-Version: 0.7.8
+Version: 0.7.9
 Summary: Simple assembler to convert pioasm to bytes
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PIOASM
 Keywords: adafruit,blinka,circuitpython,micropython,pioasm,rp2040
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt` & `adafruit-circuitpython-pioasm-0.7.9/adafruit_circuitpython_pioasm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/adafruit_pioasm.py` & `adafruit-circuitpython-pioasm-0.7.9/adafruit_pioasm.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import array
 import re
 
 splitter = re.compile(r",\s*|\s+(?:,\s*)?").split
 mov_splitter = re.compile("!|~|::").split
 
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PIOASM.git"
 
 CONDITIONS = ["", "!x", "x--", "!y", "y--", "x!=y", "pin", "!osre"]
 IN_SOURCES = ["pins", "x", "y", "null", None, None, "isr", "osr"]
 OUT_DESTINATIONS = ["pins", "x", "y", "null", "pindirs", "pc", "isr", "exec"]
 WAIT_SOURCES = ["gpio", "pin", "irq", None]
 MOV_DESTINATIONS = ["pins", "x", "y", None, "exec", "pc", "isr", "osr"]
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pioasm-0.7.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/docs/conf.py` & `adafruit-circuitpython-pioasm-0.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/docs/index.rst` & `adafruit-circuitpython-pioasm-0.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_7seg.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_7seg.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_7seg_fader.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_7seg_fader.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_background_morse.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_background_morse.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 DAH = array.array("H", [LED_ON | DAH_DURATION, LED_OFF | DIT_DURATION])
 # That is, two more DAH-length gaps for a total of three
 LETTER_SPACE = array.array("H", [LED_OFF | (2 * DAH_DURATION)])
 # That is, four more DAH-length gaps (after a letter space) for a total of seven
 WORD_SPACE = array.array("H", [LED_OFF | (4 * DIT_DURATION)])
 
 # Letters and words can be created by concatenating ("+") the elements
-E = DAH + LETTER_SPACE
+E = DIT + LETTER_SPACE
 O = DAH + DAH + DAH + LETTER_SPACE
 S = DIT + DIT + DIT + LETTER_SPACE
-T = DIT + LETTER_SPACE
+T = DAH + LETTER_SPACE
 SOS = S + O + S + WORD_SPACE
 TEST = T + E + S + T + WORD_SPACE
 
 sm = StateMachine(
     pio_code.assembled,
     frequency=1_000_000,
     first_out_pin=LED,
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_blink.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_blink.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_hello.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_hello.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_i2sout.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_i2sout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_led_brightness.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_led_brightness.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_neopixel.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_neopixel_bg.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_neopixel_bg.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_pdm.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_pdm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_print_c_program.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_print_c_program.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_pulsegroup.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_pulsegroup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_rotaryencoder.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_rotaryencoder.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_rxuart.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_rxuart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_simpletest.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/examples/pioasm_txuart.py` & `adafruit-circuitpython-pioasm-0.7.9/examples/pioasm_txuart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pioasm-0.7.8/pyproject.toml` & `adafruit-circuitpython-pioasm-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pioasm"
 description = "Simple assembler to convert pioasm to bytes"
-version = "0.7.8"
+version = "0.7.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PIOASM"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-pioasm-0.7.8/tests/testpioasm.py` & `adafruit-circuitpython-pioasm-0.7.9/tests/testpioasm.py`

 * *Files identical despite different names*


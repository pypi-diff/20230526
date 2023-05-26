# Comparing `tmp/adafruit-circuitpython-avrprog-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-avrprog-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-avrprog-1.4.8.tar", last modified: Mon Aug 22 18:56:27 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-avrprog-1.4.9.tar", last modified: Fri Aug 26 02:32:54 2022, max compression
```

## Comparing `adafruit-circuitpython-avrprog-1.4.8.tar` & `adafruit-circuitpython-avrprog-1.4.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.476637 adafruit-circuitpython-avrprog-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.476637 adafruit-circuitpython-avrprog-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.476637 adafruit-circuitpython-avrprog-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.476637 adafruit-circuitpython-avrprog-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    18236 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_avrprog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.476637 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-22 18:56:27.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-08-22 18:56:27.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:56:27.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 18:56:27.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:56:27.000000 adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5333 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/attiny13a_blink.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/attiny13a_blink.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_mega2560.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_tiny13a.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_trinket85.py
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_uno328.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_read_signature_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/optiboot_atmega328.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/optiboot_atmega328.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)    20548 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/stk500boot_v2_mega2560.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/stk500boot_v2_mega2560.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/trinket_boot.hex
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/examples/trinket_boot.hex.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-08-22 18:56:18.000000 adafruit-circuitpython-avrprog-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:56:05.000000 adafruit-circuitpython-avrprog-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:56:27.480638 adafruit-circuitpython-avrprog-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.089571 adafruit-circuitpython-avrprog-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.089571 adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    18236 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_avrprog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:32:54.000000 adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.093571 adafruit-circuitpython-avrprog-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/attiny13a_blink.hex
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/attiny13a_blink.hex.license
+-rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_mega2560.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_tiny13a.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_trinket85.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_uno328.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_read_signature_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex.license
+-rw-r--r--   0 runner    (1001) docker     (121)    20548 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex.license
+-rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex.license
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-08-26 02:32:45.000000 adafruit-circuitpython-avrprog-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:32:33.000000 adafruit-circuitpython-avrprog-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:32:54.097571 adafruit-circuitpython-avrprog-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-avrprog-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-avrprog-1.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-avrprog-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.gitignore` & `adafruit-circuitpython-avrprog-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-avrprog-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/.pylintrc` & `adafruit-circuitpython-avrprog-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-avrprog-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/LICENSE` & `adafruit-circuitpython-avrprog-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-avrprog-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-avrprog-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-avrprog-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/PKG-INFO` & `adafruit-circuitpython-avrprog-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-avrprog-1.4.8/README.rst` & `adafruit-circuitpython-avrprog-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/adafruit_avrprog.py` & `adafruit-circuitpython-avrprog-1.4.9/adafruit_avrprog.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog.git"
 
 from digitalio import Direction, DigitalInOut
 
 _SLOW_CLOCK = 100000
 _FAST_CLOCK = 1000000
```

### Comparing `adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/PKG-INFO` & `adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-avrprog
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython helper library for programming AVR chips.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AVRprog
 Keywords: adafruit,avr,spi,atmega,attiny,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-avrprog-1.4.8/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt` & `adafruit-circuitpython-avrprog-1.4.9/adafruit_circuitpython_avrprog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-avrprog-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/docs/conf.py` & `adafruit-circuitpython-avrprog-1.4.9/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -36,15 +37,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit AVRprog Library"
-copyright = "2017 ladyada"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-avrprog-1.4.8/docs/examples.rst` & `adafruit-circuitpython-avrprog-1.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/docs/index.rst` & `adafruit-circuitpython-avrprog-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_mega2560.py` & `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_mega2560.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_tiny13a.py` & `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_tiny13a.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_trinket85.py` & `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_trinket85.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_program_uno328.py` & `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_program_uno328.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/avrprog_read_signature_simpletest.py` & `adafruit-circuitpython-avrprog-1.4.9/examples/avrprog_read_signature_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/optiboot_atmega328.hex` & `adafruit-circuitpython-avrprog-1.4.9/examples/optiboot_atmega328.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/stk500boot_v2_mega2560.hex` & `adafruit-circuitpython-avrprog-1.4.9/examples/stk500boot_v2_mega2560.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/examples/trinket_boot.hex` & `adafruit-circuitpython-avrprog-1.4.9/examples/trinket_boot.hex`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-avrprog-1.4.8/pyproject.toml` & `adafruit-circuitpython-avrprog-1.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-avrprog"
 description = "CircuitPython helper library for programming AVR chips."
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AVRprog"}
 keywords = [
     "adafruit",
```


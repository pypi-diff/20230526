# Comparing `tmp/adafruit-circuitpython-register-1.9.8.tar.gz` & `tmp/adafruit-circuitpython-register-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-register-1.9.8.tar", last modified: Fri Feb  4 21:04:55 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-register-1.9.9.tar", last modified: Tue Jun  7 17:19:48 2022, max compression
```

## Comparing `adafruit-circuitpython-register-1.9.8.tar` & `adafruit-circuitpython-register-1.9.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.331485 adafruit-circuitpython-register-1.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.331485 adafruit-circuitpython-register-1.9.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.331485 adafruit-circuitpython-register-1.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.331485 adafruit-circuitpython-register-1.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8975 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8228 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8975 2022-02-04 21:04:55.000000 adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-02-04 21:04:55.000000 adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 21:04:55.000000 adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-04 21:04:55.000000 adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/adafruit_register/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bcd_alarm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bcd_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bits.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_struct.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_struct_array.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5537 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/examples/register_rwbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/examples/register_rwbits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/examples/register_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/examples/register_unarystruct.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 21:04:55.335485 adafruit-circuitpython-register-1.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1811 2022-02-04 21:04:43.000000 adafruit-circuitpython-register-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.388030 adafruit-circuitpython-register-1.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.392030 adafruit-circuitpython-register-1.9.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.392030 adafruit-circuitpython-register-1.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.392030 adafruit-circuitpython-register-1.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8250 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.392030 adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8997 2022-06-07 17:19:48.000000 adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-06-07 17:19:48.000000 adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:19:48.000000 adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-07 17:19:48.000000 adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.392030 adafruit-circuitpython-register-1.9.9/adafruit_register/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6138 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bcd_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bcd_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_struct.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_struct_array.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5537 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/examples/register_rwbit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/examples/register_rwbits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/examples/register_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/examples/register_unarystruct.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:19:48.396031 adafruit-circuitpython-register-1.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1811 2022-06-07 17:19:32.000000 adafruit-circuitpython-register-1.9.9/setup.py
```

### Comparing `adafruit-circuitpython-register-1.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-register-1.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-register-1.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-register-1.9.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-register-1.9.9/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
-    rev: 20.8b1
+  - repo: https://github.com/python/black
+    rev: 22.3.0
     hooks:
-    - id: black
--   repo: https://github.com/fsfe/reuse-tool
-    rev: v0.12.1
+      - id: black
+  - repo: https://github.com/fsfe/reuse-tool
+    rev: v0.14.0
     hooks:
-    - id: reuse
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v2.3.0
+      - id: reuse
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.2.0
     hooks:
-    -   id: check-yaml
-    -   id: end-of-file-fixer
-    -   id: trailing-whitespace
--   repo: https://github.com/pycqa/pylint
+      - id: check-yaml
+      - id: end-of-file-fixer
+      - id: trailing-whitespace
+  - repo: https://github.com/pycqa/pylint
     rev: v2.11.1
     hooks:
-    -   id: pylint
+      - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
-    -   id: pylint
+      - id: pylint
         name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
         types: [python]
         files: "^examples/"
         args:
-        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
-    -   id: pylint
+          - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+      - id: pylint
         name: pylint (test code)
         description: Run pylint rules on "tests/*.py" files
         types: [python]
         files: "^tests/"
         args:
-        - --disable=missing-docstring,consider-using-f-string,duplicate-code
+          - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-register-1.9.8/.pylintrc` & `adafruit-circuitpython-register-1.9.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-register-1.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-register-1.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/LICENSE` & `adafruit-circuitpython-register-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-register-1.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-register-1.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-register-1.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/PKG-INFO` & `adafruit-circuitpython-register-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-register
-Version: 1.9.8
+Version: 1.9.9
 Summary: CircuitPython data descriptor classes to represent hardware registers on I2C and SPI devices.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Register
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit register micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-micropython-register/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/register/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Register/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Register/actions/
     :alt: Build Status
 
@@ -212,20 +212,17 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/register/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Register/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-register-1.9.8/README.rst` & `adafruit-circuitpython-register-1.9.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-micropython-register/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/register/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Register/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Register/actions/
     :alt: Build Status
 
@@ -193,18 +193,15 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/register/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Register/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/PKG-INFO` & `adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-register
-Version: 1.9.8
+Version: 1.9.9
 Summary: CircuitPython data descriptor classes to represent hardware registers on I2C and SPI devices.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Register
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit register micropython circuitpython
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-micropython-register/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/register/en/latest/
     :alt: Documentation Status
 
-.. image :: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_Register/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_Register/actions/
     :alt: Build Status
 
@@ -212,20 +212,17 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/register/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Register/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_circuitpython_register.egg-info/SOURCES.txt` & `adafruit-circuitpython-register-1.9.9/adafruit_circuitpython_register.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bcd_alarm.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bcd_alarm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bcd_datetime.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bcd_datetime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bit.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_bits.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_bits.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_struct.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_struct.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/adafruit_register/i2c_struct_array.py` & `adafruit-circuitpython-register-1.9.9/adafruit_register/i2c_struct_array.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-register-1.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/docs/api.rst` & `adafruit-circuitpython-register-1.9.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/docs/conf.py` & `adafruit-circuitpython-register-1.9.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-register-1.9.8/docs/examples.rst` & `adafruit-circuitpython-register-1.9.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/docs/index.rst` & `adafruit-circuitpython-register-1.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/examples/register_rwbit.py` & `adafruit-circuitpython-register-1.9.9/examples/register_rwbit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/examples/register_rwbits.py` & `adafruit-circuitpython-register-1.9.9/examples/register_rwbits.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/examples/register_simpletest.py` & `adafruit-circuitpython-register-1.9.9/examples/register_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/examples/register_unarystruct.py` & `adafruit-circuitpython-register-1.9.9/examples/register_unarystruct.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-register-1.9.8/setup.py` & `adafruit-circuitpython-register-1.9.9/setup.py`

 * *Files identical despite different names*


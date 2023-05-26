# Comparing `tmp/adafruit-circuitpython-rsa-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-rsa-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-rsa-1.2.8.tar", last modified: Tue Apr 19 23:47:21 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-rsa-1.2.9.tar", last modified: Fri May 20 00:36:45 2022, max compression
```

## Comparing `adafruit-circuitpython-rsa-1.2.8.tar` & `adafruit-circuitpython-rsa-1.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.014843 adafruit-circuitpython-rsa-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.018843 adafruit-circuitpython-rsa-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.018843 adafruit-circuitpython-rsa-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.018843 adafruit-circuitpython-rsa-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.022843 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-04-19 23:47:20.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-04-19 23:47:20.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 23:47:20.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-19 23:47:20.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-19 23:47:20.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.022843 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/
--rwxr-xr-x   0 runner    (1001) docker     (121)      970 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3875 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/asn1.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4834 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2060 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/core.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    26566 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/key.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2143 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/machine_size.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3512 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/pem.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15017 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/pkcs1.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4889 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/prime.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2380 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/randnum.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6556 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/examples/rsa_sign_verify.py
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/examples/rsa_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3290 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/examples/rsa_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 23:47:21.026843 adafruit-circuitpython-rsa-1.2.8/util/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-04-19 23:47:04.000000 adafruit-circuitpython-rsa-1.2.8/util/decode_priv_key.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.640992 adafruit-circuitpython-rsa-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.644992 adafruit-circuitpython-rsa-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.644992 adafruit-circuitpython-rsa-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.644992 adafruit-circuitpython-rsa-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    10241 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.648992 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-05-20 00:36:45.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-05-20 00:36:45.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 00:36:45.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-05-20 00:36:45.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-20 00:36:45.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.648992 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      970 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3982 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/asn1.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4834 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2060 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    26672 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/key.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2249 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/machine_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3512 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/pem.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15123 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/pkcs1.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4972 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/prime.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2380 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/randnum.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6556 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/examples/rsa_sign_verify.py
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/examples/rsa_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3290 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/examples/rsa_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 00:36:45.652992 adafruit-circuitpython-rsa-1.2.9/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-05-20 00:36:32.000000 adafruit-circuitpython-rsa-1.2.9/util/decode_priv_key.py
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-rsa-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-rsa-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-rsa-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-rsa-1.2.9/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
--   repo: https://github.com/python/black
+  - repo: https://github.com/python/black
     rev: 22.3.0
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

### Comparing `adafruit-circuitpython-rsa-1.2.8/.pylintrc` & `adafruit-circuitpython-rsa-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rsa-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/LICENSE` & `adafruit-circuitpython-rsa-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/LICENSES/Apache-2.0.txt` & `adafruit-circuitpython-rsa-1.2.9/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-rsa-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-rsa-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-rsa-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/PKG-INFO` & `adafruit-circuitpython-rsa-1.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rsa
-Version: 1.2.8
+Version: 1.2.9
 Summary: RSA implementation based on python-rsa
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RSA
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython rsa rsa,encryption,cryptography
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/rsa/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/rsa/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RSA/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_RSA/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/README.rst` & `adafruit-circuitpython-rsa-1.2.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/rsa/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/rsa/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RSA/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_RSA/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/PKG-INFO` & `adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rsa
-Version: 1.2.8
+Version: 1.2.9
 Summary: RSA implementation based on python-rsa
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RSA
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython rsa rsa,encryption,cryptography
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/rsa/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/rsa/en/latest/
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/discord/327254708534116352.svg
+.. image:: https://raw.githubusercontent.com/adafruit/Adafruit_CircuitPython_Bundle/main/badges/adafruit_discord.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_RSA/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_RSA/actions/
     :alt: Build Status
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_circuitpython_rsa.egg-info/SOURCES.txt` & `adafruit-circuitpython-rsa-1.2.9/adafruit_circuitpython_rsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/__init__.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/_compat.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/_compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,24 @@
 Python compatibility wrappers.
 """
 
 import sys
 from struct import pack
 
 try:
-    from typing import Any, Literal, Tuple
+    from typing import Any, Tuple
+
+    try:
+        from typing import Literal
+    except ImportError:
+        from typing_extensions import Literal
 except ImportError:
     pass
 
+
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RSA.git"
 
 MAX_INT = sys.maxsize
 MAX_INT64 = (1 << 63) - 1
 MAX_INT32 = (1 << 31) - 1
 MAX_INT16 = (1 << 15) - 1
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/asn1.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/asn1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/common.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/common.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/core.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/core.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/key.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/key.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 import adafruit_rsa.prime
 import adafruit_rsa.pem
 import adafruit_rsa.common
 import adafruit_rsa.randnum
 import adafruit_rsa.core
 
 try:
-    from typing import Any, Tuple, Dict, Callable, Literal
+    from typing import Any, Tuple, Dict, Callable
+
+    try:
+        from typing import Literal
+    except ImportError:
+        from typing_extensions import Literal
 except ImportError:
     pass
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RSA.git"
 
 # pylint: disable=invalid-name, useless-object-inheritance, redefined-builtin, no-name-in-module, too-few-public-methods
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/machine_size.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/machine_size.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 
 Detection of 32-bit and 64-bit machines and byte alignment.
 """
 
 import sys
 
 try:
-    from typing import Literal, Tuple
+    from typing import Tuple
+
+    try:
+        from typing import Literal
+    except ImportError:
+        from typing_extensions import Literal
 except ImportError:
     pass
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RSA.git"
 
 MAX_INT = sys.maxsize
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/pem.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/pem.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/pkcs1.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/pkcs1.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,27 @@
 """
 
 import os
 import adafruit_hashlib as hashlib
 from adafruit_rsa import common, transform, core
 
 try:
-    from typing import Optional, Iterator, Union, Literal
+    from typing import Optional, Iterator, Union
     from adafruit_rsa.key import PublicKey, PrivateKey
 
     try:
         from typing import Protocol
     except ImportError:
         from typing_extensions import Protocol
 
+    try:
+        from typing import Literal
+    except ImportError:
+        from typing_extensions import Literal
+
     class _FileLikeObject(Protocol):
         """A file like object that implements the :meth:`read` method"""
 
         def read(self, blocksize: int) -> Union[bytes, str]:
             """A method that reads a given number of bytes or chracters"""
             ...
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/prime.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/prime.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 Roberto Tamassia, 2002.
 """
 # pylint: disable=invalid-name
 import adafruit_rsa.common
 import adafruit_rsa.randnum
 
 try:
-    from typing import Literal
+    try:
+        from typing import Literal
+    except ImportError:
+        from typing_extensions import Literal
 except ImportError:
     pass
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_RSA.git"
 
 __all__ = ["getprime", "are_relatively_prime"]
```

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/randnum.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/randnum.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/adafruit_rsa/transform.py` & `adafruit-circuitpython-rsa-1.2.9/adafruit_rsa/transform.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-rsa-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/docs/api.rst` & `adafruit-circuitpython-rsa-1.2.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/docs/conf.py` & `adafruit-circuitpython-rsa-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/docs/index.rst` & `adafruit-circuitpython-rsa-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/examples/rsa_sign_verify.py` & `adafruit-circuitpython-rsa-1.2.9/examples/rsa_sign_verify.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/examples/rsa_simpletest.py` & `adafruit-circuitpython-rsa-1.2.9/examples/rsa_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/examples/rsa_tests.py` & `adafruit-circuitpython-rsa-1.2.9/examples/rsa_tests.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/setup.py` & `adafruit-circuitpython-rsa-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rsa-1.2.8/util/decode_priv_key.py` & `adafruit-circuitpython-rsa-1.2.9/util/decode_priv_key.py`

 * *Files identical despite different names*


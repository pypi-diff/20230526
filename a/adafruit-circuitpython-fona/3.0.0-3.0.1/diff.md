# Comparing `tmp/adafruit-circuitpython-fona-3.0.0.tar.gz` & `tmp/adafruit-circuitpython-fona-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fona-3.0.0.tar", last modified: Thu May 11 14:24:54 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-fona-3.0.1.tar", last modified: Fri May 26 16:22:48 2023, max compression
```

## Comparing `adafruit-circuitpython-fona-3.0.0.tar` & `adafruit-circuitpython-fona-3.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.955641 adafruit-circuitpython-fona-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.955641 adafruit-circuitpython-fona-3.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.955641 adafruit-circuitpython-fona-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.955641 adafruit-circuitpython-fona-3.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.955641 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 14:24:54.000000 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-11 14:24:54.000000 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:24:54.000000 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 14:24:54.000000 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 14:24:54.000000 adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/adafruit_fona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/adafruit_fona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33787 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3362 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/adafruit_fona/fona_3g.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/examples/fona_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2407 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/examples/fona_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/examples/fona_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/examples/fona_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/examples/fona_sms_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-11 14:24:45.000000 adafruit-circuitpython-fona-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 14:24:30.000000 adafruit-circuitpython-fona-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:24:54.959641 adafruit-circuitpython-fona-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.668441 adafruit-circuitpython-fona-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.660441 adafruit-circuitpython-fona-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-26 16:22:48.668441 adafruit-circuitpython-fona-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-26 16:22:48.000000 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 16:22:48.000000 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:48.000000 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:22:48.000000 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 16:22:48.000000 adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/adafruit_fona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/adafruit_fona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33787 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3362 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10817 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/adafruit_fona/fona_3g.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.664441 adafruit-circuitpython-fona-3.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:48.668441 adafruit-circuitpython-fona-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/examples/fona_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2407 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/examples/fona_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/examples/fona_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1267 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/examples/fona_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1229 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/examples/fona_sms_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 16:22:40.000000 adafruit-circuitpython-fona-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:22:26.000000 adafruit-circuitpython-fona-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:48.668441 adafruit-circuitpython-fona-3.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-fona-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fona-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/.gitignore` & `adafruit-circuitpython-fona-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-fona-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/.pylintrc` & `adafruit-circuitpython-fona-3.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-fona-3.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fona-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/LICENSE` & `adafruit-circuitpython-fona-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fona-3.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-fona-3.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fona-3.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/PKG-INFO` & `adafruit-circuitpython-fona-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for the Adafruit FONAA
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FONA
 Keywords: adafruit,blinka,circuitpython,micropython,fona,fona,,cellular
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fona-3.0.0/README.rst` & `adafruit-circuitpython-fona-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/PKG-INFO` & `adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fona
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for the Adafruit FONAA
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FONA
 Keywords: adafruit,blinka,circuitpython,micropython,fona,fona,,cellular
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_circuitpython_fona.egg-info/SOURCES.txt` & `adafruit-circuitpython-fona-3.0.1/adafruit_circuitpython_fona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona.py` & `adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     try:
         from typing import Literal
     except ImportError:
         from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 FONA_DEFAULT_TIMEOUT_MS = 500  # TODO: Check this against arduino...
 
 # Commands
 CMD_AT = b"AT"
 # Replies
```

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona_network.py` & `adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 try:
     from typing import Optional, Tuple, Type
     from types import TracebackType
     from adafruit_fona.adafruit_fona import FONA
 except ImportError:
     pass
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 # Network types
 NET_GSM = 0x01
 NET_CDMA = 0x02
```

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_fona/adafruit_fona_socket.py` & `adafruit-circuitpython-fona-3.0.1/adafruit_fona/adafruit_fona_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/adafruit_fona/fona_3g.py` & `adafruit-circuitpython-fona-3.0.1/adafruit_fona/fona_3g.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     try:
         from typing import Literal
     except ImportError:
         from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FONA.git"
 
 FONA_MAX_SOCKETS = const(10)
 
 
 class FONA3G(FONA):
     """FONA 3G module interface.
```

### Comparing `adafruit-circuitpython-fona-3.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-fona-3.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/docs/conf.py` & `adafruit-circuitpython-fona-3.0.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-fona-3.0.0/docs/index.rst` & `adafruit-circuitpython-fona-3.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/examples/fona_aio_post.py` & `adafruit-circuitpython-fona-3.0.1/examples/fona_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/examples/fona_cheerlights.py` & `adafruit-circuitpython-fona-3.0.1/examples/fona_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/examples/fona_simpletest.py` & `adafruit-circuitpython-fona-3.0.1/examples/fona_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/examples/fona_sms.py` & `adafruit-circuitpython-fona-3.0.1/examples/fona_sms.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/examples/fona_sms_response.py` & `adafruit-circuitpython-fona-3.0.1/examples/fona_sms_response.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fona-3.0.0/pyproject.toml` & `adafruit-circuitpython-fona-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-fona"
 description = "CircuitPython library for the Adafruit FONAA"
-version = "3.0.0"
+version = "3.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_FONA"}
 keywords = [
     "adafruit",
```


# Comparing `tmp/adafruit-circuitpython-esp-atcontrol-0.9.2.tar.gz` & `tmp/adafruit-circuitpython-esp-atcontrol-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp-atcontrol-0.9.2.tar", last modified: Tue May 16 17:53:39 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-esp-atcontrol-0.9.3.tar", last modified: Fri May 26 16:10:12 2023, max compression
```

## Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2.tar` & `adafruit-circuitpython-esp-atcontrol-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.662764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.670764 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.670764 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7460 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_countviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.140020 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.140020 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-26 16:10:12.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-26 16:10:12.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:10:12.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 16:10:12.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 16:10:12.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7460 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_countviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 16:10:04.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 16:09:48.000000 adafruit-circuitpython-esp-atcontrol-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:10:12.144020 adafruit-circuitpython-esp-atcontrol-0.9.3/setup.cfg
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-esp-atcontrol-0.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/.gitignore` & `adafruit-circuitpython-esp-atcontrol-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/.pre-commit-config.yaml` & `adafruit-circuitpython-esp-atcontrol-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/.pylintrc` & `adafruit-circuitpython-esp-atcontrol-0.9.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-esp-atcontrol-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSE` & `adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/MIT.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/PKG-INFO` & `adafruit-circuitpython-esp-atcontrol-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp-atcontrol
-Version: 0.9.2
+Version: 0.9.3
 Summary: CircuitPython driver for communicating using ESP AT command set.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol
 Keywords: adafruit,software,esp,at,atcontrol,internet,communication,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst` & `adafruit-circuitpython-esp-atcontrol-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO` & `adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp-atcontrol
-Version: 0.9.2
+Version: 0.9.3
 Summary: CircuitPython driver for communicating using ESP AT command set.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol
 Keywords: adafruit,software,esp,at,atcontrol,internet,communication,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 try:
     from typing import Optional, Dict, Union, List
     import busio
 except ImportError:
     pass
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_espATcontrol.git"
 
 
 class OKError(Exception):
     """The exception thrown when we didn't get acknowledgement to an AT command"""
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_socket.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol_socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico` & `adafruit-circuitpython-esp-atcontrol-0.9.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/conf.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/docs/conf.py`

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

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst` & `adafruit-circuitpython-esp-atcontrol-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_aio_post.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_cheerlights.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_countviewer.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_countviewer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_localtime.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_simpletest.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_webclient.py` & `adafruit-circuitpython-esp-atcontrol-0.9.3/examples/esp_atcontrol_webclient.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.2/pyproject.toml` & `adafruit-circuitpython-esp-atcontrol-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp-atcontrol"
 description = "CircuitPython driver for communicating using ESP AT command set."
-version = "0.9.2"
+version = "0.9.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol"}
 keywords = [
     "adafruit",
```


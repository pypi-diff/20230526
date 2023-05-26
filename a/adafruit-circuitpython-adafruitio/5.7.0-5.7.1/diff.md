# Comparing `tmp/adafruit-circuitpython-adafruitio-5.7.0.tar.gz` & `tmp/adafruit-circuitpython-adafruitio-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-adafruitio-5.7.0.tar", last modified: Thu May 11 14:49:11 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-adafruitio-5.7.1.tar", last modified: Fri May 26 16:22:36 2023, max compression
```

## Comparing `adafruit-circuitpython-adafruitio-5.7.0.tar` & `adafruit-circuitpython-adafruitio-5.7.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.896942 adafruit-circuitpython-adafruitio-5.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.884942 adafruit-circuitpython-adafruitio-5.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.888942 adafruit-circuitpython-adafruitio-5.7.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.888942 adafruit-circuitpython-adafruitio-5.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.888942 adafruit-circuitpython-adafruitio-5.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-11 14:49:11.896942 adafruit-circuitpython-adafruitio-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.888942 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-11 14:49:11.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-11 14:49:11.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:49:11.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 14:49:11.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 14:49:11.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.888942 adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28204 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/adafruit_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/adafruit_io_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.892942 adafruit-circuitpython-adafruitio-5.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.892942 adafruit-circuitpython-adafruitio-5.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.892942 adafruit-circuitpython-adafruitio-5.7.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.896942 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_analog_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_digital_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_randomizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:11.896942 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4105 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4134 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4627 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-11 14:49:02.000000 adafruit-circuitpython-adafruitio-5.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 14:48:49.000000 adafruit-circuitpython-adafruitio-5.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:49:11.896942 adafruit-circuitpython-adafruitio-5.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.158931 adafruit-circuitpython-adafruitio-5.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27829 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_digital_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4105 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4134 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4627 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/setup.cfg
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/.gitignore` & `adafruit-circuitpython-adafruitio-5.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/.pre-commit-config.yaml` & `adafruit-circuitpython-adafruitio-5.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/.pylintrc` & `adafruit-circuitpython-adafruitio-5.7.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-adafruitio-5.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/LICENSE` & `adafruit-circuitpython-adafruitio-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/LICENSES/MIT.txt` & `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.7.0
+Version: 5.7.1
 Summary: Adafruit IO for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Keywords: adafruit,blinka,circuitpython,micropython,adafruit_io,adafruit-io,rest,api,iot,wifi
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/README.rst` & `adafruit-circuitpython-adafruitio-5.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.7.0
+Version: 5.7.1
 Summary: Adafruit IO for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Keywords: adafruit,blinka,circuitpython,micropython,adafruit_io,adafruit-io,rest,api,iot,wifi
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt` & `adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/adafruit_io.py` & `adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from adafruit_minimqtt.adafruit_minimqtt import MMQTTException
 from adafruit_io.adafruit_io_errors import (
     AdafruitIO_RequestError,
     AdafruitIO_ThrottleError,
     AdafruitIO_MQTTError,
 )
 
-__version__ = "5.7.0"
+__version__ = "5.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO.git"
 
 CLIENT_HEADERS = {"User-Agent": "AIO-CircuitPython/{0}".format(__version__)}
 
 
 def validate_feed_key(feed_key):
     """Validates a provided feed key against Adafruit IO's system rules.
@@ -248,21 +248,14 @@
         :param str shared_user: Owner of the Adafruit IO feed, required for shared feeds.
 
         Example of subscribing to an Adafruit IO Feed named 'temperature'.
 
         .. code-block:: python
 
             client.subscribe('temperature')
-
-        Example of subscribing to two Adafruit IO feeds: 'temperature'
-        and 'humidity'.
-
-        .. code-block:: python
-
-            client.subscribe([('temperature'), ('humidity')])
         """
         if shared_user is not None and feed_key is not None:
             validate_feed_key(feed_key)
             self._client.subscribe("{0}/f/{1}".format(shared_user, feed_key))
         elif group_key is not None:
             validate_feed_key(group_key)
             self._client.subscribe("{0}/g/{1}".format(self._user, group_key))
@@ -329,21 +322,14 @@
 
         Example of unsubscribing from a feed.
 
         .. code-block:: python
 
             client.unsubscribe('temperature')
 
-        Example of unsubscribing from two feeds: 'temperature'
-        and 'humidity'
-
-        .. code-block:: python
-
-            client.unsubscribe([('temperature'), ('humidity')])
-
         Example of unsubscribing from a shared feed.
 
         .. code-block:: python
 
             client.unsubscribe('temperature', shared_user='adabot')
         """
         if shared_user is not None and feed_key is not None:
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/adafruit_io/adafruit_io_errors.py` & `adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io_errors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/docs/_static/favicon.ico` & `adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/docs/conf.py` & `adafruit-circuitpython-adafruitio-5.7.1/docs/conf.py`

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
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/docs/index.rst` & `adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_analog_in.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_digital_out.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_digital_out.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_feeds.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_feeds.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_metadata.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_metadata.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_randomizer.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_randomizer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_temperature.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_temperature.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_http/adafruit_io_weather.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_weather.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_location.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_location.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_mqtt/adafruit_io_time.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_time.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/examples/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.0/pyproject.toml` & `adafruit-circuitpython-adafruitio-5.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-adafruitio"
 description = "Adafruit IO for CircuitPython"
-version = "5.7.0"
+version = "5.7.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO"}
 keywords = [
     "adafruit",
```


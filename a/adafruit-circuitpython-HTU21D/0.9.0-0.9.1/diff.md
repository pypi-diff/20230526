# Comparing `tmp/adafruit-circuitpython-HTU21D-0.9.0.tar.gz` & `tmp/adafruit-circuitpython-HTU21D-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-HTU21D-0.9.0.tar", last modified: Mon Sep 16 21:06:10 2019, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-HTU21D-0.9.1.tar", last modified: Thu Jan 23 02:54:23 2020, max compression
```

## Comparing `adafruit-circuitpython-HTU21D-0.9.0.tar` & `adafruit-circuitpython-HTU21D-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4811 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_htu21d.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      186 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/examples.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/api.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4414 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/_static/favicon.ico
--rw-rw-r--   0 travis    (2000) travis    (2000)     5368 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3042 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1910 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)      328 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/examples/htu21d_simpletest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     1481 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5829 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4737 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/adafruit_circuitpython_HTU21D.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4737 2019-09-16 21:06:10.000000 adafruit-circuitpython-HTU21D-0.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    16110 2019-09-16 21:04:51.000000 adafruit-circuitpython-HTU21D-0.9.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.460432 adafruit-circuitpython-HTU21D-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (115)       59 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     5829 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1096 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)     4186 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2651 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     4186 2020-01-23 02:54:23.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      556 2020-01-23 02:54:23.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-23 02:54:23.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-23 02:54:23.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       16 2020-01-23 02:54:23.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_circuitpython_HTU21D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)     4811 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/adafruit_htu21d.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (115)      265 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     5368 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)      186 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     1121 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (115)      328 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/examples/htu21d_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-23 02:54:23.464432 adafruit-circuitpython-HTU21D-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1910 2020-01-23 02:54:14.000000 adafruit-circuitpython-HTU21D-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/adafruit_htu21d.py` & `adafruit-circuitpython-HTU21D-0.9.1/adafruit_htu21d.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/docs/index.rst` & `adafruit-circuitpython-HTU21D-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/docs/_static/favicon.ico` & `adafruit-circuitpython-HTU21D-0.9.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/docs/conf.py` & `adafruit-circuitpython-HTU21D-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/setup.py` & `adafruit-circuitpython-HTU21D-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/LICENSE` & `adafruit-circuitpython-HTU21D-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-HTU21D-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-HTU21D-0.9.0/.pylintrc` & `adafruit-circuitpython-HTU21D-0.9.1/.pylintrc`

 * *Files identical despite different names*


# Comparing `tmp/adafruit-circuitpython-display_shapes-2.6.1.tar.gz` & `tmp/adafruit-circuitpython-display_shapes-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-display_shapes-2.6.1.tar", last modified: Tue May 16 17:49:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-display_shapes-2.6.2.tar", last modified: Fri May 26 16:09:34 2023, max compression
```

## Comparing `adafruit-circuitpython-display_shapes-2.6.1.tar` & `adafruit-circuitpython-display_shapes-2.6.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.785800 adafruit-circuitpython-display_shapes-2.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/multisparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/roundrect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_circle_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest_magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5689 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_ticks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8543 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_triple.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.965543 adafruit-circuitpython-display_shapes-2.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.965543 adafruit-circuitpython-display_shapes-2.6.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.965543 adafruit-circuitpython-display_shapes-2.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.969543 adafruit-circuitpython-display_shapes-2.6.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.969543 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-26 16:09:34.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-26 16:09:34.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:09:34.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:09:34.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 16:09:34.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.969543 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/multisparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/roundrect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_circle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_simpletest_magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5689 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_ticks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8543 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_triple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 16:09:25.000000 adafruit-circuitpython-display_shapes-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:09:14.000000 adafruit-circuitpython-display_shapes-2.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:09:34.973543 adafruit-circuitpython-display_shapes-2.6.2/setup.cfg
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-display_shapes-2.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/.gitignore` & `adafruit-circuitpython-display_shapes-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/.pre-commit-config.yaml` & `adafruit-circuitpython-display_shapes-2.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/.pylintrc` & `adafruit-circuitpython-display_shapes-2.6.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-display_shapes-2.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/LICENSE` & `adafruit-circuitpython-display_shapes-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-display_shapes-2.6.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/MIT.txt` & `adafruit-circuitpython-display_shapes-2.6.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-display_shapes-2.6.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/PKG-INFO` & `adafruit-circuitpython-display_shapes-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display_shapes
-Version: 2.6.1
+Version: 2.6.2
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/README.rst` & `adafruit-circuitpython-display_shapes-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display-shapes
-Version: 2.6.1
+Version: 2.6.2
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/circle.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.roundrect import RoundRect
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Circle(RoundRect):
     # pylint: disable=too-few-public-methods, invalid-name
     """A circle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/line.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/line.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Line(Polygon):
     # pylint: disable=too-many-arguments,invalid-name, too-few-public-methods
     """A line.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/multisparkline.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/multisparkline.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/polygon.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional, List, Tuple
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Polygon(displayio.TileGrid):
     """A polygon.
 
     :param list points: A list of (x, y) tuples of the points
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/rect.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/rect.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Rect(displayio.TileGrid):
     """A rectangle.
 
     :param int x: The x-position of the top left corner.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/roundrect.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/roundrect.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class RoundRect(displayio.TileGrid):
     # pylint: disable=too-many-arguments
     """A round-corner rectangle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/sparkline.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/sparkline.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/triangle.py` & `adafruit-circuitpython-display_shapes-2.6.2/adafruit_display_shapes/triangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.6.1"
+__version__ = "2.6.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Triangle(Polygon):
     # pylint: disable=too-many-arguments,invalid-name
     """A triangle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico` & `adafruit-circuitpython-display_shapes-2.6.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst` & `adafruit-circuitpython-display_shapes-2.6.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/docs/conf.py` & `adafruit-circuitpython-display_shapes-2.6.2/docs/conf.py`

 * *Files 0% similar despite different names*

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

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst` & `adafruit-circuitpython-display_shapes-2.6.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst` & `adafruit-circuitpython-display_shapes-2.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_circle_animation.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_circle_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest_magtag.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_simpletest_magtag.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_simpletest.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_ticks.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_ticks.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_triple.py` & `adafruit-circuitpython-display_shapes-2.6.2/examples/display_shapes_sparkline_triple.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.1/pyproject.toml` & `adafruit-circuitpython-display_shapes-2.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-display_shapes"
 description = "Various common shapes for use with displayio"
-version = "2.6.1"
+version = "2.6.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes"}
 keywords = [
     "adafruit",
```


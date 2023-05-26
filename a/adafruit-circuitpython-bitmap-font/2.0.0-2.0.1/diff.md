# Comparing `tmp/adafruit-circuitpython-bitmap_font-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-bitmap_font-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bitmap_font-2.0.0.tar", last modified: Thu May 11 18:21:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bitmap_font-2.0.1.tar", last modified: Fri May 26 16:23:08 2023, max compression
```

## Comparing `adafruit-circuitpython-bitmap_font-2.0.0.tar` & `adafruit-circuitpython-bitmap_font-2.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.228215 adafruit-circuitpython-bitmap_font-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.216215 adafruit-circuitpython-bitmap_font-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.216215 adafruit-circuitpython-bitmap_font-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.220215 adafruit-circuitpython-bitmap_font-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.220215 adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/OFL-1.1-RFN.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-11 18:21:25.228215 adafruit-circuitpython-bitmap_font-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.220215 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/bitmap_font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/glyph_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/pcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/ttf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.220215 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-11 18:21:25.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-11 18:21:25.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:21:25.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 18:21:25.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 18:21:25.000000 adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.224215 adafruit-circuitpython-bitmap_font-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.224215 adafruit-circuitpython-bitmap_font-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.224215 adafruit-circuitpython-bitmap_font-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_displayio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_forkawesome_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_forkawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_magtag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.228215 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    62897 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.bdf
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.bdf.license
--rw-r--r--   0 runner    (1001) docker     (123)   163036 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.pcf
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.pcf.license
--rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/LeagueSpartan-Bold-16.bdf
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/LeagueSpartan-Bold-16.bdf.license
--rw-r--r--   0 runner    (1001) docker     (123)   477640 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/forkawesome-42.pcf
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/forkawesome-42.pcf.license
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-11 18:20:59.000000 adafruit-circuitpython-bitmap_font-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:21:25.228215 adafruit-circuitpython-bitmap_font-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:21:25.228215 adafruit-circuitpython-bitmap_font-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/test/displayio.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-11 18:21:15.000000 adafruit-circuitpython-bitmap_font-2.0.0/test/fontio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.232674 adafruit-circuitpython-bitmap_font-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.236674 adafruit-circuitpython-bitmap_font-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.236674 adafruit-circuitpython-bitmap_font-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.236674 adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/OFL-1.1-RFN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.240674 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/bitmap_font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/glyph_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/pcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/ttf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.240674 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-26 16:23:08.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-26 16:23:08.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:08.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 16:23:08.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:23:08.000000 adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.240674 adafruit-circuitpython-bitmap_font-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.240674 adafruit-circuitpython-bitmap_font-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_displayio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_forkawesome_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_forkawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_magtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    62897 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.bdf.license
+-rw-r--r--   0 runner    (1001) docker     (123)   163036 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.pcf
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (123)    86848 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/LeagueSpartan-Bold-16.bdf
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/LeagueSpartan-Bold-16.bdf.license
+-rw-r--r--   0 runner    (1001) docker     (123)   477640 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/forkawesome-42.pcf
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/forkawesome-42.pcf.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 16:22:47.000000 adafruit-circuitpython-bitmap_font-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:08.244674 adafruit-circuitpython-bitmap_font-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/test/displayio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-26 16:22:59.000000 adafruit-circuitpython-bitmap_font-2.0.1/test/fontio.py
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bitmap_font-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/.gitignore` & `adafruit-circuitpython-bitmap_font-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-bitmap_font-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/.pylintrc` & `adafruit-circuitpython-bitmap_font-2.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bitmap_font-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/LICENSE` & `adafruit-circuitpython-bitmap_font-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/OFL-1.1-RFN.txt` & `adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/OFL-1.1-RFN.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bitmap_font-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/PKG-INFO` & `adafruit-circuitpython-bitmap_font-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmap_font
-Version: 2.0.0
+Version: 2.0.1
 Summary: Loads bitmap fonts into CircuitPython displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
 Keywords: adafruit,blinka,circuitpython,micropython,font,text,displayio,bitmap
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/README.rst` & `adafruit-circuitpython-bitmap_font-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/bdf.py` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/bdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     pass
 
 import gc
 from fontio import Glyph
 from .glyph_cache import GlyphCache
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 class BDF(GlyphCache):
     """Loads glyphs from a BDF file in the given bitmap_class."""
 
     def __init__(self, f: FileIO, bitmap_class: Bitmap) -> None:
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/bitmap_font.py` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/bitmap_font.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from displayio import Bitmap
     from . import bdf
     from . import pcf
     from . import ttf
 except ImportError:
     pass
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 def load_font(
     filename: str, bitmap: Optional[Bitmap] = None
 ) -> Union[bdf.BDF, pcf.PCF, ttf.TTF]:
     """Loads a font file. Returns None if unsupported."""
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/glyph_cache.py` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/glyph_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from typing import Union, Iterable
     from fontio import Glyph
 except ImportError:
     pass
 
 import gc
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font.git"
 
 
 class GlyphCache:
     """Caches glyphs loaded by a subclass."""
 
     def __init__(self) -> None:
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/pcf.py` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/pcf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_bitmap_font/ttf.py` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_bitmap_font/ttf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bitmap-font
-Version: 2.0.0
+Version: 2.0.1
 Summary: Loads bitmap fonts into CircuitPython displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font
 Keywords: adafruit,blinka,circuitpython,micropython,font,text,displayio,bitmap
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt` & `adafruit-circuitpython-bitmap_font-2.0.1/adafruit_circuitpython_bitmap_font.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-bitmap_font-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/docs/api.rst` & `adafruit-circuitpython-bitmap_font-2.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/docs/conf.py` & `adafruit-circuitpython-bitmap_font-2.0.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/docs/examples.rst` & `adafruit-circuitpython-bitmap_font-2.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/docs/index.rst` & `adafruit-circuitpython-bitmap_font-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_displayio_simpletest.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_displayio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_forkawesome_icons.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_forkawesome_icons.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_forkawesome.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_forkawesome.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_magtag.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_magtag.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_label_simpletest.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_label_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/bitmap_font_simpletest.py` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/bitmap_font_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.bdf` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/Junction-regular-24.pcf` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/Junction-regular-24.pcf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/LeagueSpartan-Bold-16.bdf` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/LeagueSpartan-Bold-16.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/examples/fonts/forkawesome-42.pcf` & `adafruit-circuitpython-bitmap_font-2.0.1/examples/fonts/forkawesome-42.pcf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/pyproject.toml` & `adafruit-circuitpython-bitmap_font-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bitmap_font"
 description = "Loads bitmap fonts into CircuitPython displayio."
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-bitmap_font-2.0.0/test/displayio.py` & `adafruit-circuitpython-bitmap_font-2.0.1/test/displayio.py`

 * *Files identical despite different names*


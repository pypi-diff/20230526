# Comparing `tmp/adafruit-circuitpython-displayio-flipclock-1.0.1.tar.gz` & `tmp/adafruit-circuitpython-displayio-flipclock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-flipclock-1.0.1.tar", last modified: Mon Oct 24 00:10:27 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-flipclock-1.0.2.tar", last modified: Fri May 26 15:51:40 2023, max compression
```

## Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1.tar` & `adafruit-circuitpython-displayio-flipclock-1.0.2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.020074 adafruit-circuitpython-displayio-flipclock-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.008073 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.012074 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.012074 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.012074 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/OFL-1.1-RFN.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2022-10-24 00:10:27.020074 adafruit-circuitpython-displayio-flipclock-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.012074 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2022-10-24 00:10:26.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-10-24 00:10:27.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 00:10:26.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-10-24 00:10:26.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-24 00:10:26.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.012074 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10470 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/flip_clock.py
--rw-r--r--   0 runner    (1001) docker     (121)    11940 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/flip_digit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.016074 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.016074 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.020074 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   121162 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_5frames.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_5frames.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    39562 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_small_5frames.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_small_5frames.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_flipdigit_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_hours_and_minutes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_ntp_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3188 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2799 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipdigit_smaller_pyportal.py
--rw-r--r--   0 runner    (1001) docker     (121)   241162 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_bottom_animation_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_bottom_animation_sheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)   241162 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_top_animation_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_top_animation_sheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)   202762 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_bottom_animation_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_bottom_animation_sheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    49462 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_static_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_static_sheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)   202762 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_top_animation_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_top_animation_sheet.bmp.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 00:10:27.020074 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/
--rw-r--r--   0 runner    (1001) docker     (121)    69548 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/LeagueSpartan-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/LeagueSpartan-Regular.ttf.license
--rw-r--r--   0 runner    (1001) docker     (121)    68436 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/ParchmentMf.ttf
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/ParchmentMf.ttf.license
--rw-r--r--   0 runner    (1001) docker     (121)    17699 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/make_sprites_flip_animations.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    58678 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    19510 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet_small.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet_small.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)   121162 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_5frames.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_5frames.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    39562 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_small_5frames.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_small_5frames.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-10-24 00:10:18.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-10-24 00:10:10.000000 adafruit-circuitpython-displayio-flipclock-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 00:10:27.020074 adafruit-circuitpython-displayio-flipclock-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.886220 adafruit-circuitpython-displayio-flipclock-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.874220 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.878220 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.878220 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.878220 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/OFL-1.1-RFN.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-26 15:51:40.886220 adafruit-circuitpython-displayio-flipclock-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.878220 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-26 15:51:40.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-26 15:51:40.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:51:40.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 15:51:40.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 15:51:40.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.878220 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/flip_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/flip_digit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.882220 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.882220 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.886220 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   121162 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_5frames.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_5frames.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    39562 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_small_5frames.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_small_5frames.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_flipdigit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_hours_and_minutes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_ntp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipdigit_smaller_pyportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241162 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_bottom_animation_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_bottom_animation_sheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   241162 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_top_animation_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_top_animation_sheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   202762 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_bottom_animation_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_bottom_animation_sheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    49462 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_static_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_static_sheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   202762 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_top_animation_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_top_animation_sheet.bmp.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.886220 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)    69548 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/LeagueSpartan-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/LeagueSpartan-Regular.ttf.license
+-rw-r--r--   0 runner    (1001) docker     (123)    68436 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/ParchmentMf.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/ParchmentMf.ttf.license
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/make_sprites_flip_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    58678 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet_small.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet_small.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)   121162 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_5frames.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_5frames.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    39562 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_small_5frames.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_small_5frames.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-26 15:51:32.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-26 15:51:19.000000 adafruit-circuitpython-displayio-flipclock-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:51:40.886220 adafruit-circuitpython-displayio-flipclock-1.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-flipclock-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/.gitignore` & `adafruit-circuitpython-displayio-flipclock-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-flipclock-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/.pylintrc` & `adafruit-circuitpython-displayio-flipclock-1.0.2/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -429,8 +429,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-flipclock-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSE` & `adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/OFL-1.1-RFN.txt` & `adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/OFL-1.1-RFN.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-flipclock-1.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/PKG-INFO` & `adafruit-circuitpython-displayio-flipclock-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-flipclock
-Version: 1.0.1
+Version: 1.0.2
 Summary: DisplayIO widgets for showing flip clock style animattions changing from one number to another.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_FlipClock
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_flipclock,displayio,clock,time,flipclock,display,lcd,widget,ui,number
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/README.rst` & `adafruit-circuitpython-displayio-flipclock-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-flipclock
-Version: 1.0.1
+Version: 1.0.2
 Summary: DisplayIO widgets for showing flip clock style animattions changing from one number to another.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_FlipClock
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_flipclock,displayio,clock,time,flipclock,display,lcd,widget,ui,number
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_circuitpython_displayio_flipclock.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_circuitpython_displayio_flipclock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/OFL-1.1-RFN.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_displayio_flipclock.egg-info/PKG-INFO
 adafruit_circuitpython_displayio_flipclock.egg-info/SOURCES.txt
 adafruit_circuitpython_displayio_flipclock.egg-info/dependency_links.txt
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/__init__.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
 # imports
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_FlipClock.git"
```

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/flip_clock.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/flip_clock.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/adafruit_displayio_flipclock/flip_digit.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/adafruit_displayio_flipclock/flip_digit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-flipclock-1.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/docs/conf.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/docs/index.rst` & `adafruit-circuitpython-displayio-flipclock-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_5frames.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_5frames.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/bottom_animation_sheet_small_5frames.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/bottom_animation_sheet_small_5frames.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_flipdigit_test.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_flipdigit_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_hours_and_minutes.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_hours_and_minutes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_ntp_test.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_ntp_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipclock_simpletest.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipclock_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/displayio_flipdigit_smaller_pyportal.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/displayio_flipdigit_smaller_pyportal.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_bottom_animation_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_bottom_animation_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/grey_top_animation_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/grey_top_animation_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_bottom_animation_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_bottom_animation_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_static_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_static_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/parchment_top_animation_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/parchment_top_animation_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/LeagueSpartan-Regular.ttf` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/LeagueSpartan-Regular.ttf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/ParchmentMf.ttf` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/ParchmentMf.ttf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/spritesheet_generator/make_sprites_flip_animations.py` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/spritesheet_generator/make_sprites_flip_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/static_sheet_small.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/static_sheet_small.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_5frames.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_5frames.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/examples/top_animation_sheet_small_5frames.bmp` & `adafruit-circuitpython-displayio-flipclock-1.0.2/examples/top_animation_sheet_small_5frames.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-flipclock-1.0.1/pyproject.toml` & `adafruit-circuitpython-displayio-flipclock-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-flipclock"
 description = "DisplayIO widgets for showing flip clock style animattions changing from one number to another."
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_FlipClock"}
 keywords = [
     "adafruit",
```


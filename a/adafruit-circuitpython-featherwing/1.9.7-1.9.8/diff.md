# Comparing `tmp/adafruit-circuitpython-featherwing-1.9.7.tar.gz` & `tmp/adafruit-circuitpython-featherwing-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-featherwing-1.9.7.tar", last modified: Thu Feb 13 19:06:46 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-featherwing-1.9.8.tar", last modified: Wed Feb 26 21:43:56 2020, max compression
```

## Comparing `adafruit-circuitpython-featherwing-1.9.7.tar` & `adafruit-circuitpython-featherwing-1.9.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.380813 adafruit-circuitpython-featherwing-1.9.7/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.368813 adafruit-circuitpython-featherwing-1.9.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.368813 adafruit-circuitpython-featherwing-1.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (115)       85 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (115)       59 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (115)     3228 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (115)     1110 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)     4430 2020-02-13 19:06:46.380813 adafruit-circuitpython-featherwing-1.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2919 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.368813 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     4430 2020-02-13 19:06:46.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2057 2020-02-13 19:06:46.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-02-13 19:06:46.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      354 2020-02-13 19:06:46.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       21 2020-02-13 19:06:46.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.372813 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     2070 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/alphanum_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     2330 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/dotstar_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (115)     5678 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/gps_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (115)     4591 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/ina219_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (115)     9066 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/joy_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     3577 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/led_segments.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     5469 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/matrix_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     4366 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/minitft_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     4190 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/neopixel_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     7097 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/pixelmatrix.py
--rwxr-xr-x   0 runner    (1001) docker     (115)    10164 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/rtc_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     2073 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/sevensegment_featherwing.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     4061 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/tempmotion_featherwing.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.372813 adafruit-circuitpython-featherwing-1.9.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.372813 adafruit-circuitpython-featherwing-1.9.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.372813 adafruit-circuitpython-featherwing-1.9.7/docs/_static/ina219_featherwing/
--rw-r--r--   0 runner    (1001) docker     (115)   214537 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/ina219_featherwing/ina219_featherwing.jpg
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.376813 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/
--rw-r--r--   0 runner    (1001) docker     (115)   936845 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_a.jpg
--rw-r--r--   0 runner    (1001) docker     (115)   935494 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_b.jpg
--rw-r--r--   0 runner    (1001) docker     (115)   930279 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_joystick.jpg
--rw-r--r--   0 runner    (1001) docker     (115)   936445 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_select.jpg
--rw-r--r--   0 runner    (1001) docker     (115)   935430 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_x.jpg
--rw-r--r--   0 runner    (1001) docker     (115)   937839 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_y.jpg
--rw-r--r--   0 runner    (1001) docker     (115)      778 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (115)     5402 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)     1916 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (115)      972 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-13 19:06:46.380813 adafruit-circuitpython-featherwing-1.9.7/examples/
--rwxr-xr-x   0 runner    (1001) docker     (115)      931 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_alphanum_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)     1497 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_dotstar_palette_example.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     1678 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_dotstar_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)     2854 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_gps_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (115)      465 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_ina219_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)      655 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_joy_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)     1337 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_matrix_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (115)      641 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_minitft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)     1509 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_neopixel_palette_example.py
--rw-r--r--   0 runner    (1001) docker     (115)     1747 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_neopixel_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (115)     1496 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_rtc_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)     1054 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_sevensegment_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)      425 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_tempmotion_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)      354 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-02-13 19:06:46.380813 adafruit-circuitpython-featherwing-1.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     2431 2020-02-13 19:06:32.000000 adafruit-circuitpython-featherwing-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.599228 adafruit-circuitpython-featherwing-1.9.8/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.579228 adafruit-circuitpython-featherwing-1.9.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.583228 adafruit-circuitpython-featherwing-1.9.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (115)       85 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (115)       59 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     3228 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1110 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)     4430 2020-02-26 21:43:56.599228 adafruit-circuitpython-featherwing-1.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2919 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.583228 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     4430 2020-02-26 21:43:56.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2057 2020-02-26 21:43:56.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-02-26 21:43:56.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      354 2020-02-26 21:43:56.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       21 2020-02-26 21:43:56.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.587228 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     2070 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/alphanum_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     2330 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/dotstar_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5678 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/gps_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4591 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/ina219_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9066 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/joy_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     3577 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/led_segments.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     5469 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/matrix_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     4366 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/minitft_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     4190 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/neopixel_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     7097 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/pixelmatrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)    10164 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/rtc_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     2073 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/sevensegment_featherwing.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     4061 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/tempmotion_featherwing.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.587228 adafruit-circuitpython-featherwing-1.9.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.587228 adafruit-circuitpython-featherwing-1.9.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.587228 adafruit-circuitpython-featherwing-1.9.8/docs/_static/ina219_featherwing/
+-rw-r--r--   0 runner    (1001) docker     (115)   214537 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/ina219_featherwing/ina219_featherwing.jpg
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.595228 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/
+-rw-r--r--   0 runner    (1001) docker     (115)   936845 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_a.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)   935494 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_b.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)   930279 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_joystick.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)   936445 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_select.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)   935430 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_x.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)   937839 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_y.jpg
+-rw-r--r--   0 runner    (1001) docker     (115)      778 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     5402 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1916 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (115)      972 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-26 21:43:56.599228 adafruit-circuitpython-featherwing-1.9.8/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (115)      931 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_alphanum_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1497 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_dotstar_palette_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     1678 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_dotstar_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2854 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_gps_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)      465 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_ina219_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)      655 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_joy_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1337 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_matrix_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)      641 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_minitft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1509 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_neopixel_palette_example.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1747 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_neopixel_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (115)     1496 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_rtc_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1054 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_sevensegment_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)      425 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_tempmotion_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)      354 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-02-26 21:43:56.599228 adafruit-circuitpython-featherwing-1.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     2431 2020-02-26 21:43:47.000000 adafruit-circuitpython-featherwing-1.9.8/setup.py
```

### Comparing `adafruit-circuitpython-featherwing-1.9.7/.github/workflows/build.yml` & `adafruit-circuitpython-featherwing-1.9.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/.github/workflows/release.yml` & `adafruit-circuitpython-featherwing-1.9.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/.pylintrc` & `adafruit-circuitpython-featherwing-1.9.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-featherwing-1.9.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/LICENSE` & `adafruit-circuitpython-featherwing-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/PKG-INFO` & `adafruit-circuitpython-featherwing-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-featherwing
-Version: 1.9.7
+Version: 1.9.8
 Summary: CircuitPython library that provides FeatherWing specific classes for those that require a significant amount of initialization.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FeatherWing
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-featherwing-1.9.7/README.rst` & `adafruit-circuitpython-featherwing-1.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/PKG-INFO` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-featherwing
-Version: 1.9.7
+Version: 1.9.8
 Summary: CircuitPython library that provides FeatherWing specific classes for those that require a significant amount of initialization.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_FeatherWing
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_circuitpython_featherwing.egg-info/SOURCES.txt` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_circuitpython_featherwing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/alphanum_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/alphanum_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/dotstar_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/dotstar_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/gps_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/gps_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/ina219_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/ina219_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/joy_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/joy_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/led_segments.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/led_segments.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/matrix_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/matrix_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/minitft_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/minitft_featherwing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,22 +71,22 @@
         if spi is None:
             spi = board.SPI()
         if cs is None:
             cs = board.D5
         if dc is None:
             dc = board.D6
         self._ss = Seesaw(i2c, address)
-        self._backlight = PWMOut(self._ss, 5)
-        self._backlight.duty_cycle = 0
+        self._ss.pin_mode_bulk(self._button_mask, self._ss.INPUT_PULLUP)
         self._ss.pin_mode(8, self._ss.OUTPUT)
         self._ss.digital_write(8, True)  # Reset the Display via Seesaw
+        self._backlight = PWMOut(self._ss, 5)
+        self._backlight.duty_cycle = 0
         display_bus = displayio.FourWire(spi, command=dc, chip_select=cs)
         self.display = ST7735R(display_bus, width=160, height=80, colstart=24,
                                rotation=270, bgr=True)
-        self._ss.pin_mode_bulk(self._button_mask, self._ss.INPUT_PULLUP)
     #pylint: enable-msg=too-many-arguments
 
     @property
     def backlight(self):
         """
         Return the current backlight duty cycle value
         """
```

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/neopixel_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/neopixel_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/pixelmatrix.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/pixelmatrix.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/rtc_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/rtc_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/sevensegment_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/sevensegment_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/adafruit_featherwing/tempmotion_featherwing.py` & `adafruit-circuitpython-featherwing-1.9.8/adafruit_featherwing/tempmotion_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/favicon.ico` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/ina219_featherwing/ina219_featherwing.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/ina219_featherwing/ina219_featherwing.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_a.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_a.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_b.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_b.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_joystick.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_joystick.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_select.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_select.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_x.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_x.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/_static/joy_featherwing/joy_featherwing_y.jpg` & `adafruit-circuitpython-featherwing-1.9.8/docs/_static/joy_featherwing/joy_featherwing_y.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/api.rst` & `adafruit-circuitpython-featherwing-1.9.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/conf.py` & `adafruit-circuitpython-featherwing-1.9.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/examples.rst` & `adafruit-circuitpython-featherwing-1.9.8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/docs/index.rst` & `adafruit-circuitpython-featherwing-1.9.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_alphanum_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_alphanum_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_dotstar_palette_example.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_dotstar_palette_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_dotstar_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_dotstar_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_gps_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_gps_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_joy_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_joy_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_matrix_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_matrix_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_minitft_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_minitft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_neopixel_palette_example.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_neopixel_palette_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_neopixel_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_neopixel_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_rtc_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_rtc_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/examples/featherwing_sevensegment_simpletest.py` & `adafruit-circuitpython-featherwing-1.9.8/examples/featherwing_sevensegment_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-featherwing-1.9.7/setup.py` & `adafruit-circuitpython-featherwing-1.9.8/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/adafruit-circuitpython-slideshow-1.7.8.tar.gz` & `tmp/adafruit-circuitpython-slideshow-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-slideshow-1.7.8.tar", last modified: Tue Aug  9 19:39:25 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-slideshow-1.7.9.tar", last modified: Mon Aug 22 19:02:16 2022, max compression
```

## Comparing `adafruit-circuitpython-slideshow-1.7.8.tar` & `adafruit-circuitpython-slideshow-1.7.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.572482 adafruit-circuitpython-slideshow-1.7.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.564482 adafruit-circuitpython-slideshow-1.7.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-09 19:39:25.572482 adafruit-circuitpython-slideshow-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-09 19:39:25.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-08-09 19:39:25.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:39:25.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-09 19:39:25.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-09 19:39:25.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    17883 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/adafruit_slideshow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.568482 adafruit-circuitpython-slideshow-1.7.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5738 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.572482 adafruit-circuitpython-slideshow-1.7.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:39:25.572482 adafruit-circuitpython-slideshow-1.7.8/examples/images/
--rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/blue_rectangle.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/blue_rectangle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/green_circle.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/green_circle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/purple_oval.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/purple_oval.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/sample_text_slide.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/sample_text_slide.json.license
--rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/yellow_square.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/examples/images/yellow_square.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_alignment_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_tft_gizmo.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_touch.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-08-09 19:39:17.000000 adafruit-circuitpython-slideshow-1.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-09 19:39:09.000000 adafruit-circuitpython-slideshow-1.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:39:25.572482 adafruit-circuitpython-slideshow-1.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.417160 adafruit-circuitpython-slideshow-1.7.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.417160 adafruit-circuitpython-slideshow-1.7.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3687 2022-08-22 19:02:16.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-08-22 19:02:16.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 19:02:16.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 19:02:16.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-22 19:02:16.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17883 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/adafruit_slideshow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5738 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/blue_rectangle.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/blue_rectangle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/green_circle.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/green_circle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/purple_oval.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/purple_oval.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/sample_text_slide.json
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/sample_text_slide.json.license
+-rw-r--r--   0 runner    (1001) docker     (121)    17462 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/yellow_square.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/examples/images/yellow_square.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_alignment_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_tft_gizmo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_touch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-08-22 19:02:08.000000 adafruit-circuitpython-slideshow-1.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 19:02:01.000000 adafruit-circuitpython-slideshow-1.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 19:02:16.421160 adafruit-circuitpython-slideshow-1.7.9/setup.cfg
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-slideshow-1.7.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.github/workflows/build.yml` & `adafruit-circuitpython-slideshow-1.7.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+            sed -i -e "s/0.0.0+auto.0/1.2.3/" $file;
         done;
         python -m build
         twine check dist/*
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.github/workflows/release.yml` & `adafruit-circuitpython-slideshow-1.7.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+            sed -i -e "s/0.0.0+auto.0/${{github.event.release.tag_name}}/" $file;
         done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.gitignore` & `adafruit-circuitpython-slideshow-1.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.pre-commit-config.yaml` & `adafruit-circuitpython-slideshow-1.7.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/.pylintrc` & `adafruit-circuitpython-slideshow-1.7.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-slideshow-1.7.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/LICENSE` & `adafruit-circuitpython-slideshow-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-slideshow-1.7.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/LICENSES/MIT.txt` & `adafruit-circuitpython-slideshow-1.7.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-slideshow-1.7.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/PKG-INFO` & `adafruit-circuitpython-slideshow-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-slideshow
-Version: 1.7.8
+Version: 1.7.9
 Summary: CircuitPython helper library for displaying a slideshow of images on a display.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Slideshow
 Keywords: adafruit,software,slideshow,image,display,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/README.rst` & `adafruit-circuitpython-slideshow-1.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/PKG-INFO` & `adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-slideshow
-Version: 1.7.8
+Version: 1.7.9
 Summary: CircuitPython helper library for displaying a slideshow of images on a display.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Slideshow
 Keywords: adafruit,software,slideshow,image,display,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/adafruit_circuitpython_slideshow.egg-info/SOURCES.txt` & `adafruit-circuitpython-slideshow-1.7.9/adafruit_circuitpython_slideshow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/adafruit_slideshow.py` & `adafruit-circuitpython-slideshow-1.7.9/adafruit_slideshow.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 try:
     from typing import Optional
     from pwmio import PWMOut
 except ImportError:
     pass
 
-__version__ = "1.7.8"
+__version__ = "1.7.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Slideshow.git"
 
 
 class HorizontalAlignment:
     """Defines possible horizontal alignment orders."""
 
     # pylint: disable=too-few-public-methods
```

### Comparing `adafruit-circuitpython-slideshow-1.7.8/docs/_static/favicon.ico` & `adafruit-circuitpython-slideshow-1.7.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/docs/conf.py` & `adafruit-circuitpython-slideshow-1.7.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/docs/index.rst` & `adafruit-circuitpython-slideshow-1.7.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/images/blue_rectangle.bmp` & `adafruit-circuitpython-slideshow-1.7.9/examples/images/blue_rectangle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/images/green_circle.bmp` & `adafruit-circuitpython-slideshow-1.7.9/examples/images/green_circle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/images/purple_oval.bmp` & `adafruit-circuitpython-slideshow-1.7.9/examples/images/purple_oval.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/images/yellow_square.bmp` & `adafruit-circuitpython-slideshow-1.7.9/examples/images/yellow_square.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_alignment_test.py` & `adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_alignment_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_simpletest.py` & `adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_tft_gizmo.py` & `adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_tft_gizmo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/examples/slideshow_touch.py` & `adafruit-circuitpython-slideshow-1.7.9/examples/slideshow_touch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-slideshow-1.7.8/pyproject.toml` & `adafruit-circuitpython-slideshow-1.7.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-slideshow"
 description = "CircuitPython helper library for displaying a slideshow of images on a display."
-version = "1.7.8"
+version = "1.7.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Slideshow"}
 keywords = [
     "adafruit",
```


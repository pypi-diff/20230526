# Comparing `tmp/adafruit-circuitpython-PYOA-2.5.8.tar.gz` & `tmp/adafruit-circuitpython-PYOA-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-PYOA-2.5.8.tar", last modified: Tue Aug  9 19:35:54 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-PYOA-2.5.9.tar", last modified: Mon Aug 15 21:19:12 2022, max compression
```

## Comparing `adafruit-circuitpython-PYOA-2.5.8.tar` & `adafruit-circuitpython-PYOA-2.5.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.048332 adafruit-circuitpython-PYOA-2.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.020331 adafruit-circuitpython-PYOA-2.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16293 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-09 19:35:54.048332 adafruit-circuitpython-PYOA-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-09 19:35:53.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-08-09 19:35:54.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:35:53.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-08-09 19:35:53.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-09 19:35:53.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    17855 2022-08-09 19:35:45.000000 adafruit-circuitpython-PYOA-2.5.8/adafruit_pyoa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.024331 adafruit-circuitpython-PYOA-2.5.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.028331 adafruit-circuitpython-PYOA-2.5.8/examples/cave/
--rw-r--r--   0 runner    (1001) docker     (121)   655612 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/cave.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/cave.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)   487840 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/creak.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/creak.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/cyoa.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/cyoa.json.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.028331 adafruit-circuitpython-PYOA-2.5.8/examples/cave/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (121)    41772 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/fonts/Arial-Bold-12.bdf
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/fonts/Arial-Bold-12.bdf.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/page01.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/page01.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)   831966 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/pub.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/pub.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)   155992 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/scream.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cave/scream.wav.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.036331 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/
--rw-r--r--   0 runner    (1001) docker     (121)  1385600 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/Mystery.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/Mystery.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     2540 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/cyoa.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/cyoa.json.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.036331 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (121)    41772 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/fonts/Arial-Bold-12.bdf
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/fonts/Arial-Bold-12.bdf.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   227092 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happy_ending.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happy_ending.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happyending.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happyending.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/help.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/help.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   332668 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page01.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page01.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page02.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page02.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page03.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page03.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page04.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page04.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    42654 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_01.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_01.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    31056 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_03.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_03.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   602532 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_04.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_04.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    86828 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.wav.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.044331 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/
--rwxr-xr-x   0 runner    (1001) docker     (121)  1385600 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/Mystery.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/Mystery.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     2498 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/cyoa.json
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/cyoa.json.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:35:54.048332 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   232575 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/fonts/Arial-Bold-18.bdf
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/fonts/Arial-Bold-18.bdf.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   227092 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happy_ending.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happy_ending.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happyending.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happyending.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/help.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/help.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   460856 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   332668 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    19264 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page01.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page01.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page02.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page02.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page03.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page03.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page04.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page04.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    42654 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_01.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_01.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    31056 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_03.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_03.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   602532 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_04.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_04.wav.license
--rwxr-xr-x   0 runner    (1001) docker     (121)   460856 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.bmp.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    86828 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.wav
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.wav.license
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-09 19:35:45.000000 adafruit-circuitpython-PYOA-2.5.8/examples/pyoa_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-08-09 19:35:45.000000 adafruit-circuitpython-PYOA-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-08-09 19:35:36.000000 adafruit-circuitpython-PYOA-2.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:35:54.048332 adafruit-circuitpython-PYOA-2.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.998154 adafruit-circuitpython-PYOA-2.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.974153 adafruit-circuitpython-PYOA-2.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.974153 adafruit-circuitpython-PYOA-2.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.974153 adafruit-circuitpython-PYOA-2.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16293 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.974153 adafruit-circuitpython-PYOA-2.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-15 21:19:11.994154 adafruit-circuitpython-PYOA-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.978153 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2022-08-15 21:19:11.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-08-15 21:19:11.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 21:19:11.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-08-15 21:19:11.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-15 21:19:11.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17920 2022-08-15 21:19:04.000000 adafruit-circuitpython-PYOA-2.5.9/adafruit_pyoa.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.978153 adafruit-circuitpython-PYOA-2.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.978153 adafruit-circuitpython-PYOA-2.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.978153 adafruit-circuitpython-PYOA-2.5.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.982154 adafruit-circuitpython-PYOA-2.5.9/examples/cave/
+-rw-r--r--   0 runner    (1001) docker     (121)   655612 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/cave.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/cave.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)   487840 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/creak.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/creak.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)     6510 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/cyoa.json
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/cyoa.json.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.982154 adafruit-circuitpython-PYOA-2.5.9/examples/cave/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    41772 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/fonts/Arial-Bold-12.bdf
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/fonts/Arial-Bold-12.bdf.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/page01.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/page01.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)   831966 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/pub.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/pub.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)   155992 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/scream.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cave/scream.wav.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.986153 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/
+-rw-r--r--   0 runner    (1001) docker     (121)  1385600 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/Mystery.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/Mystery.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2540 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/cyoa.json
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/cyoa.json.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.986153 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    41772 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/fonts/Arial-Bold-12.bdf
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/fonts/Arial-Bold-12.bdf.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   227092 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happy_ending.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happy_ending.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happyending.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happyending.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/help.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/help.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   332668 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9662 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page01.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page01.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page02.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page02.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page03.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page03.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page04.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page04.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    42654 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_01.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_01.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    31056 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_03.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_03.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   602532 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_04.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_04.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   153656 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    86828 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.wav.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.994154 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/
+-rwxr-xr-x   0 runner    (1001) docker     (121)  1385600 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/Mystery.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/Mystery.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2498 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/cyoa.json
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/cyoa.json.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 21:19:11.994154 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)   232575 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/fonts/Arial-Bold-18.bdf
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/fonts/Arial-Bold-18.bdf.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   227092 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happy_ending.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happy_ending.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happyending.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happyending.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/help.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/help.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   460856 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   332668 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    19264 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page01.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page01.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page02.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page02.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page03.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page03.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   307256 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page04.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page04.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    42654 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_01.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_01.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    31056 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_03.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_03.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   602532 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_04.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_04.wav.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)   460856 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.bmp.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    86828 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.wav
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.wav.license
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-15 21:19:04.000000 adafruit-circuitpython-PYOA-2.5.9/examples/pyoa_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-08-15 21:19:04.000000 adafruit-circuitpython-PYOA-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-08-15 21:18:57.000000 adafruit-circuitpython-PYOA-2.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-15 21:19:11.998154 adafruit-circuitpython-PYOA-2.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-PYOA-2.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-PYOA-2.5.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.github/workflows/release.yml` & `adafruit-circuitpython-PYOA-2.5.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.gitignore` & `adafruit-circuitpython-PYOA-2.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-PYOA-2.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/.pylintrc` & `adafruit-circuitpython-PYOA-2.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-PYOA-2.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/LICENSE` & `adafruit-circuitpython-PYOA-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-PYOA-2.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-PYOA-2.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-PYOA-2.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/PKG-INFO` & `adafruit-circuitpython-PYOA-2.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-PYOA
-Version: 2.5.8
+Version: 2.5.9
 Summary: Python your own Adventure - card & button game
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pyoa,text,adventure,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-PYOA-2.5.8/README.rst` & `adafruit-circuitpython-PYOA-2.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/PKG-INFO` & `adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-PYOA
-Version: 2.5.8
+Version: 2.5.9
 Summary: Python your own Adventure - card & button game
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_REPLACE
 Keywords: adafruit,pyoa,text,adventure,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-PYOA-2.5.8/adafruit_circuitpython_PYOA.egg-info/SOURCES.txt` & `adafruit-circuitpython-PYOA-2.5.9/adafruit_circuitpython_PYOA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/adafruit_pyoa.py` & `adafruit-circuitpython-PYOA-2.5.9/adafruit_pyoa.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 import terminalio
 
 try:
     from typing import Dict, Optional, List
 except ImportError:
     pass
 
-__version__ = "2.5.8"
+__version__ = "2.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PYOA.git"
 
 
 class PYOA_Graphics:
     # pylint: disable=too-many-instance-attributes
     """A choose your own adventure game framework."""
 
@@ -83,15 +83,18 @@
             self.audio = audioio.AudioOut(board.SPEAKER)
         else:
             raise AttributeError("Board does not have an audio output!")
 
         self._background_file = None
         self._wavfile = None
 
-        self._display.auto_brightness = False
+        try:
+            self._display.auto_brightness = False
+        except AttributeError:
+            pass
         self.backlight_fade(0)
         self._display.show(self.root_group)
         self.touchscreen = None
         self.mouse_cursor = None
         if hasattr(board, "TOUCH_XL"):
             self.touchscreen = adafruit_touchscreen.Touchscreen(
                 board.TOUCH_XL,
```

### Comparing `adafruit-circuitpython-PYOA-2.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-PYOA-2.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/docs/conf.py` & `adafruit-circuitpython-PYOA-2.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/docs/index.rst` & `adafruit-circuitpython-PYOA-2.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/cave.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/cave.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/creak.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/creak.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/cyoa.json` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/cyoa.json`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/fonts/Arial-Bold-12.bdf` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/fonts/Arial-Bold-12.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/page01.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/page01.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/pub.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/pub.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cave/scream.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cave/scream.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/Mystery.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/Mystery.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/cyoa.json` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/cyoa.json`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/fonts/Arial-Bold-12.bdf` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/fonts/Arial-Bold-12.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happy_ending.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happy_ending.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/happyending.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/happyending.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/help.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/help.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/home.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/home.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page01.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page01.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page02.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page02.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page03.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page03.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/page04.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/page04.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_01.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_01.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_03.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_03.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/sound_04.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/sound_04.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa/startup.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa/startup.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/Mystery.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/Mystery.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/cyoa.json` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/cyoa.json`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/fonts/Arial-Bold-18.bdf` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/fonts/Arial-Bold-18.bdf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happy_ending.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happy_ending.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/happyending.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/happyending.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/help.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/help.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/home.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/home.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page01.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page01.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page02.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page02.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page03.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page03.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/page04.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/page04.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_01.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_01.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_03.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_03.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/sound_04.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/sound_04.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.bmp` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/cyoa_titano/startup.wav` & `adafruit-circuitpython-PYOA-2.5.9/examples/cyoa_titano/startup.wav`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/examples/pyoa_simpletest.py` & `adafruit-circuitpython-PYOA-2.5.9/examples/pyoa_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-PYOA-2.5.8/pyproject.toml` & `adafruit-circuitpython-PYOA-2.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-PYOA"
 description = "Python your own Adventure - card & button game"
-version = "2.5.8"
+version = "2.5.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_REPLACE"}
 keywords = [
     "adafruit",
```


# Comparing `tmp/adafruit-circuitpython-motorkit-1.6.8.tar.gz` & `tmp/adafruit-circuitpython-motorkit-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-motorkit-1.6.8.tar", last modified: Thu Jun  9 18:43:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-motorkit-1.6.9.tar", last modified: Tue Aug  9 19:40:01 2022, max compression
```

## Comparing `adafruit-circuitpython-motorkit-1.6.8.tar` & `adafruit-circuitpython-motorkit-1.6.9.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.380325 adafruit-circuitpython-motorkit-1.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.368325 adafruit-circuitpython-motorkit-1.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.368325 adafruit-circuitpython-motorkit-1.6.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.368325 adafruit-circuitpython-motorkit-1.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.372325 adafruit-circuitpython-motorkit-1.6.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17967 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-06-09 18:43:36.380325 adafruit-circuitpython-motorkit-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.372325 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-06-09 18:43:36.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-06-09 18:43:36.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:43:36.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-09 18:43:36.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-09 18:43:36.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10984 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/adafruit_motorkit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.372325 adafruit-circuitpython-motorkit-1.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.372325 adafruit-circuitpython-motorkit-1.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/favicon.ico.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.380325 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/
--rw-r--r--   0 runner    (1001) docker     (121)   670981 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m1.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)   671127 2022-06-09 18:43:22.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m2.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)   671456 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m3.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m3.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)   672245 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m4.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m4.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)   672587 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper1.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)   672078 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper2.jpg.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:36.380325 adafruit-circuitpython-motorkit-1.6.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_dc_motor_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1012 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_dc_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_dual_stepper_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_robot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_robot_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_stepper_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1219 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_stepper_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:43:36.380325 adafruit-circuitpython-motorkit-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-06-09 18:43:23.000000 adafruit-circuitpython-motorkit-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.642287 adafruit-circuitpython-motorkit-1.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.630286 adafruit-circuitpython-motorkit-1.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17967 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-08-09 19:40:01.642287 adafruit-circuitpython-motorkit-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3194 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-08-09 19:40:01.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-08-09 19:40:01.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:40:01.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-09 19:40:01.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-09 19:40:01.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10977 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/adafruit_motorkit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.634286 adafruit-circuitpython-motorkit-1.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/favicon.ico.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.642287 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/
+-rw-r--r--   0 runner    (1001) docker     (121)   670981 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m1.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m1.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)   671127 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m2.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m2.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)   671456 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m3.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m3.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)   672245 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m4.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m4.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)   672587 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper1.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper1.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)   672078 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper2.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper2.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5648 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:01.642287 adafruit-circuitpython-motorkit-1.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_dc_motor_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1012 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_dc_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_dual_stepper_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_robot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_robot_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_stepper_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1219 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_stepper_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-08-09 19:39:53.000000 adafruit-circuitpython-motorkit-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-08-09 19:39:42.000000 adafruit-circuitpython-motorkit-1.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:40:01.642287 adafruit-circuitpython-motorkit-1.6.9/setup.cfg
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-motorkit-1.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/.github/workflows/build.yml` & `adafruit-circuitpython-motorkit-1.6.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/.gitignore` & `adafruit-circuitpython-motorkit-1.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/.pre-commit-config.yaml` & `adafruit-circuitpython-motorkit-1.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/.pylintrc` & `adafruit-circuitpython-motorkit-1.6.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-motorkit-1.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/LICENSE` & `adafruit-circuitpython-motorkit-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-motorkit-1.6.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-motorkit-1.6.9/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/LICENSES/MIT.txt` & `adafruit-circuitpython-motorkit-1.6.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-motorkit-1.6.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/PKG-INFO` & `adafruit-circuitpython-motorkit-1.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-motorkit
-Version: 1.6.8
+Version: 1.6.9
 Summary: CircuitPython helper library for DC & Stepper Motor FeatherWing, Shield, and Pi Hat kits.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit motor pca9685 featherwing pi shield motorkit kit i2c hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MotorKit
+Keywords: adafruit,motor,pca9685,featherwing,pi,shield,motorkit,kit,i2c,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-motorkit/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/motorkit/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython helper library for the DC & Stepper Motor FeatherWing, Shield and Pi Hat kits.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -65,16 +68,16 @@
     sudo pip3 install adafruit-circuitpython-motorkit
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-motorkit
 
 Usage Example
 =============
 
 DC motor example:
 
@@ -110,9 +113,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/README.rst` & `adafruit-circuitpython-motorkit-1.6.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython helper library for the DC & Stepper Motor FeatherWing, Shield and Pi Hat kits.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -46,16 +50,16 @@
     sudo pip3 install adafruit-circuitpython-motorkit
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-motorkit
 
 Usage Example
 =============
 
 DC motor example:
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/PKG-INFO` & `adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-motorkit
-Version: 1.6.8
+Version: 1.6.9
 Summary: CircuitPython helper library for DC & Stepper Motor FeatherWing, Shield, and Pi Hat kits.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit motor pca9685 featherwing pi shield motorkit kit i2c hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MotorKit
+Keywords: adafruit,motor,pca9685,featherwing,pi,shield,motorkit,kit,i2c,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-motorkit/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/motorkit/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 CircuitPython helper library for the DC & Stepper Motor FeatherWing, Shield and Pi Hat kits.
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
@@ -65,16 +68,16 @@
     sudo pip3 install adafruit-circuitpython-motorkit
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-motorkit
 
 Usage Example
 =============
 
 DC motor example:
 
@@ -110,9 +113,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_MotorKit/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/adafruit_circuitpython_motorkit.egg-info/SOURCES.txt` & `adafruit-circuitpython-motorkit-1.6.9/adafruit_circuitpython_motorkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_motorkit.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/MIT.txt
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/adafruit_motorkit.py` & `adafruit-circuitpython-motorkit-1.6.9/adafruit_motorkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     from typing import Optional, Tuple
     from busio import I2C
     import adafruit_motor.motor
     import adafruit_motor.stepper
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.6.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MotorKit.git"
 
 
 class MotorKit:
     """Class representing an Adafruit DC & Stepper Motor FeatherWing, Shield or Pi Hat kit.
 
     :param int address: I2C address of PCA9685 PWM controller. Default address is ``0x60``.
```

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/favicon.ico` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m1.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m1.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m2.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m2.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m3.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m3.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/m4.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/m4.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper1.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper1.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/_static/motor_featherwing/stepper2.jpg` & `adafruit-circuitpython-motorkit-1.6.9/docs/_static/motor_featherwing/stepper2.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/conf.py` & `adafruit-circuitpython-motorkit-1.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/docs/index.rst` & `adafruit-circuitpython-motorkit-1.6.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_dc_test.py` & `adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_dc_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_dual_stepper_test.py` & `adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_dual_stepper_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_robot.py` & `adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_robot.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_robot_test.py` & `adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_robot_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-motorkit-1.6.8/examples/motorkit_stepper_test.py` & `adafruit-circuitpython-motorkit-1.6.9/examples/motorkit_stepper_test.py`

 * *Files identical despite different names*


# Comparing `tmp/adafruit-circuitpython-ble-ibbq-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-ble-ibbq-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-ibbq-1.2.8.tar", last modified: Fri May 20 20:42:26 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-ibbq-1.2.9.tar", last modified: Tue Jun  7 17:24:02 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-ibbq-1.2.8.tar` & `adafruit-circuitpython-ble-ibbq-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.190157 adafruit-circuitpython-ble-ibbq-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_ble_ibbq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-05-20 20:42:26.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-05-20 20:42:26.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 20:42:26.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-20 20:42:26.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-20 20:42:26.000000 adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/examples/ble_ibbq_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 20:42:26.194157 adafruit-circuitpython-ble-ibbq-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-05-20 20:42:15.000000 adafruit-circuitpython-ble-ibbq-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.540086 adafruit-circuitpython-ble-ibbq-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     6412 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_ble_ibbq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-06-07 17:24:02.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-06-07 17:24:02.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:24:02.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-07 17:24:02.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-07 17:24:02.000000 adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:24:02.536086 adafruit-circuitpython-ble-ibbq-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/examples/ble_ibbq_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:24:02.540086 adafruit-circuitpython-ble-ibbq-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-06-07 17:23:50.000000 adafruit-circuitpython-ble-ibbq-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-ibbq-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-ibbq-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.gitignore` & `adafruit-circuitpython-ble-ibbq-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-ibbq-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/.pylintrc` & `adafruit-circuitpython-ble-ibbq-1.2.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
 # run arbitrary code
 extension-pkg-whitelist=
 
-# Add files or directories to the blacklist. They should be base names, not
+# Add files or directories to the ignore-list. They should be base names, not
 # paths.
 ignore=CVS
 
-# Add files or directories matching the regex patterns to the blacklist. The
+# Add files or directories matching the regex patterns to the ignore-list. The
 # regex matches against base names, not paths.
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-ibbq-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/LICENSE` & `adafruit-circuitpython-ble-ibbq-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-ibbq-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/PKG-INFO` & `adafruit-circuitpython-ble-ibbq-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-ibbq
-Version: 1.2.8
+Version: 1.2.9
 Summary: BLE support for iBBQ thermometers
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_iBBQ
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_ibbq ble ibbq thermometer
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/README.rst` & `adafruit-circuitpython-ble-ibbq-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_ble_ibbq.py` & `adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_ble_ibbq.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-ibbq
-Version: 1.2.8
+Version: 1.2.9
 Summary: BLE support for iBBQ thermometers
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_iBBQ
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_ibbq ble ibbq thermometer
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/adafruit_circuitpython_ble_ibbq.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-ibbq-1.2.9/adafruit_circuitpython_ble_ibbq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-ibbq-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/docs/conf.py` & `adafruit-circuitpython-ble-ibbq-1.2.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 release = "1.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "CODE_OF_CONDUCT.md"]
 
 # The reST default role (used for this markup: `text`) to use for all
```

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/docs/index.rst` & `adafruit-circuitpython-ble-ibbq-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/examples/ble_ibbq_simpletest.py` & `adafruit-circuitpython-ble-ibbq-1.2.9/examples/ble_ibbq_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-ibbq-1.2.8/setup.py` & `adafruit-circuitpython-ble-ibbq-1.2.9/setup.py`

 * *Files identical despite different names*


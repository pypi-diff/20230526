# Comparing `tmp/adafruit-circuitpython-dotstar-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-dotstar-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dotstar-2.2.8.tar", last modified: Thu May 18 15:35:31 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-dotstar-2.2.9.tar", last modified: Fri May 26 16:18:34 2023, max compression
```

## Comparing `adafruit-circuitpython-dotstar-2.2.8.tar` & `adafruit-circuitpython-dotstar-2.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.942410 adafruit-circuitpython-dotstar-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:35:31.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/adafruit_dotstar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.946410 adafruit-circuitpython-dotstar-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_pov.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/examples/hello.png
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/examples/hello.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-18 15:35:24.000000 adafruit-circuitpython-dotstar-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 15:35:11.000000 adafruit-circuitpython-dotstar-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:35:31.950410 adafruit-circuitpython-dotstar-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.288295 adafruit-circuitpython-dotstar-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.292296 adafruit-circuitpython-dotstar-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.292296 adafruit-circuitpython-dotstar-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.292296 adafruit-circuitpython-dotstar-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.292296 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-26 16:18:34.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:18:34.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:18:34.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 16:18:34.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:18:34.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2023-05-26 16:18:25.000000 adafruit-circuitpython-dotstar-2.2.9/adafruit_dotstar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-26 16:18:25.000000 adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_image_paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-26 16:18:25.000000 adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_image_pov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 16:18:25.000000 adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/examples/hello.png
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/examples/hello.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-26 16:18:25.000000 adafruit-circuitpython-dotstar-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 16:18:13.000000 adafruit-circuitpython-dotstar-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:18:34.296296 adafruit-circuitpython-dotstar-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-dotstar-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dotstar-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/.gitignore` & `adafruit-circuitpython-dotstar-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-dotstar-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/.pylintrc` & `adafruit-circuitpython-dotstar-2.2.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-dotstar-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dotstar-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/LICENSE` & `adafruit-circuitpython-dotstar-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dotstar-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-dotstar-2.2.9/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-dotstar-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dotstar-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/PKG-INFO` & `adafruit-circuitpython-dotstar-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dotstar
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for DotStar LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DotStar
 Keywords: adafruit,dotstar,leds,rgb,spi,addressable,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dotstar-2.2.8/README.rst` & `adafruit-circuitpython-dotstar-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/PKG-INFO` & `adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dotstar
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for DotStar LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DotStar
 Keywords: adafruit,dotstar,leds,rgb,spi,addressable,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dotstar-2.2.8/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt` & `adafruit-circuitpython-dotstar-2.2.9/adafruit_circuitpython_dotstar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/adafruit_dotstar.py` & `adafruit-circuitpython-dotstar-2.2.9/adafruit_dotstar.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from typing import Optional, Type
     from types import TracebackType
     from circuitpython_typing import ReadableBuffer
     from microcontroller import Pin
 except ImportError:
     pass
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DotStar.git"
 
 START_HEADER_SIZE = 4
 
 # Pixel color order constants
 RBG = "PRBG"
 """Red Blue Green"""
```

### Comparing `adafruit-circuitpython-dotstar-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-dotstar-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/docs/conf.py` & `adafruit-circuitpython-dotstar-2.2.9/docs/conf.py`

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
     "sphinx.ext.viewcode",
 ]
 
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 intersphinx_mapping = {
```

### Comparing `adafruit-circuitpython-dotstar-2.2.8/docs/index.rst` & `adafruit-circuitpython-dotstar-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_paint.py` & `adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_image_paint.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_image_pov.py` & `adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_image_pov.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/examples/dotstar_simpletest.py` & `adafruit-circuitpython-dotstar-2.2.9/examples/dotstar_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/examples/hello.png` & `adafruit-circuitpython-dotstar-2.2.9/examples/hello.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dotstar-2.2.8/pyproject.toml` & `adafruit-circuitpython-dotstar-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dotstar"
 description = "CircuitPython library for DotStar LEDs."
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DotStar"}
 keywords = [
     "adafruit",
```


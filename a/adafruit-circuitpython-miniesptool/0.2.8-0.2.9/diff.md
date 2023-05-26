# Comparing `tmp/adafruit-circuitpython-miniesptool-0.2.8.tar.gz` & `tmp/adafruit-circuitpython-miniesptool-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-miniesptool-0.2.8.tar", last modified: Wed Feb 10 22:18:50 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-miniesptool-0.2.9.tar", last modified: Tue Mar  2 23:49:31 2021, max compression
```

## Comparing `adafruit-circuitpython-miniesptool-0.2.8.tar` & `adafruit-circuitpython-miniesptool-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.492550 adafruit-circuitpython-miniesptool-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.492550 adafruit-circuitpython-miniesptool-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      189 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      441 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16230 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1098 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.492550 adafruit-circuitpython-miniesptool-0.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4180 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2709 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.492550 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4180 2021-02-10 22:18:50.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      913 2021-02-10 22:18:50.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-10 22:18:50.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-02-10 22:18:50.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-02-10 22:18:50.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    17056 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/adafruit_miniesptool.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      270 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5464 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      204 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)      906 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2936 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp32argon.py
--rw-r--r--   0 runner    (1001) docker     (116)     2949 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp32multifile.py
--rw-r--r--   0 runner    (1001) docker     (116)      945 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp8266program.py
--rw-r--r--   0 runner    (1001) docker     (116)     1138 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      128 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-10 22:18:50.496550 adafruit-circuitpython-miniesptool-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1954 2021-02-10 22:18:41.000000 adafruit-circuitpython-miniesptool-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.626246 adafruit-circuitpython-miniesptool-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.618246 adafruit-circuitpython-miniesptool-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.622246 adafruit-circuitpython-miniesptool-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1098 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.622246 adafruit-circuitpython-miniesptool-0.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     4180 2021-03-02 23:49:31.626246 adafruit-circuitpython-miniesptool-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2709 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.622246 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4180 2021-03-02 23:49:31.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      913 2021-03-02 23:49:31.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:49:31.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2021-03-02 23:49:31.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2021-03-02 23:49:31.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    17056 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/adafruit_miniesptool.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.622246 adafruit-circuitpython-miniesptool-0.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.622246 adafruit-circuitpython-miniesptool-0.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (116)      270 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)     5464 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      204 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)      906 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:49:31.626246 adafruit-circuitpython-miniesptool-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)     2936 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp32argon.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2949 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp32multifile.py
+-rw-r--r--   0 runner    (1001) docker     (116)      945 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp8266program.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1138 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      128 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:49:31.626246 adafruit-circuitpython-miniesptool-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1954 2021-03-02 23:49:20.000000 adafruit-circuitpython-miniesptool-0.2.9/setup.py
```

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-miniesptool-0.2.9/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -46,18 +46,14 @@
       run: |
         pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
-    - name: PyLint
-      run: |
-        pylint $( find . -path './adafruit*.py' )
-        ([[ ! -d "examples" ]] || pylint --disable=missing-docstring,invalid-name,bad-whitespace $( find . -path "./examples/*.py" ))
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
```

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-miniesptool-0.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/.pylintrc` & `adafruit-circuitpython-miniesptool-0.2.9/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 # Ignore comments when computing similarities.
 ignore-comments=yes
 
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
-ignore-imports=no
+ignore-imports=yes
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [BASIC]
```

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-miniesptool-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/LICENSE` & `adafruit-circuitpython-miniesptool-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-miniesptool-0.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-miniesptool-0.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-miniesptool-0.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/PKG-INFO` & `adafruit-circuitpython-miniesptool-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniesptool
-Version: 0.2.8
+Version: 0.2.9
 Summary: CircuitPython ROM loader for ESP chips, works with ESP8266 or ESP32.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_miniesptool
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/README.rst` & `adafruit-circuitpython-miniesptool-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/PKG-INFO` & `adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniesptool
-Version: 0.2.8
+Version: 0.2.9
 Summary: CircuitPython ROM loader for ESP chips, works with ESP8266 or ESP32.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_miniesptool
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/adafruit_circuitpython_miniesptool.egg-info/SOURCES.txt` & `adafruit-circuitpython-miniesptool-0.2.9/adafruit_circuitpython_miniesptool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/adafruit_miniesptool.py` & `adafruit-circuitpython-miniesptool-0.2.9/adafruit_miniesptool.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-miniesptool-0.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/docs/conf.py` & `adafruit-circuitpython-miniesptool-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/docs/index.rst` & `adafruit-circuitpython-miniesptool-0.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp32argon.py` & `adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp32argon.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp32multifile.py` & `adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp32multifile.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_esp8266program.py` & `adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_esp8266program.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/examples/miniesptool_simpletest.py` & `adafruit-circuitpython-miniesptool-0.2.9/examples/miniesptool_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniesptool-0.2.8/setup.py` & `adafruit-circuitpython-miniesptool-0.2.9/setup.py`

 * *Files identical despite different names*


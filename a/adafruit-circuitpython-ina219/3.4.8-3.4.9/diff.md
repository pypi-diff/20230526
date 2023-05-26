# Comparing `tmp/adafruit-circuitpython-ina219-3.4.8.tar.gz` & `tmp/adafruit-circuitpython-ina219-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ina219-3.4.8.tar", last modified: Wed Feb 10 22:38:05 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ina219-3.4.9.tar", last modified: Wed Mar  3 00:01:44 2021, max compression
```

## Comparing `adafruit-circuitpython-ina219-3.4.8.tar` & `adafruit-circuitpython-ina219-3.4.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.666781 adafruit-circuitpython-ina219-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.670781 adafruit-circuitpython-ina219-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      189 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      441 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16230 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.670781 adafruit-circuitpython-ina219-3.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3860 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2443 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3860 2021-02-10 22:38:05.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      765 2021-02-10 22:38:05.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-10 22:38:05.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-02-10 22:38:05.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-02-10 22:38:05.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    20419 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/adafruit_ina219.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      125 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5484 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      186 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     1069 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2010 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/examples/ina219_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      184 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-10 22:38:05.674781 adafruit-circuitpython-ina219-3.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-02-10 22:37:55.000000 adafruit-circuitpython-ina219-3.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.025426 adafruit-circuitpython-ina219-3.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      189 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     3860 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2443 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3860 2021-03-03 00:01:43.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      765 2021-03-03 00:01:43.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-03 00:01:43.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2021-03-03 00:01:43.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2021-03-03 00:01:43.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    20419 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/adafruit_ina219.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)     5484 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      186 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)     1069 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)     2010 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/examples/ina219_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      184 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-03 00:01:44.029426 adafruit-circuitpython-ina219-3.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-03-03 00:01:33.000000 adafruit-circuitpython-ina219-3.4.9/setup.py
```

### Comparing `adafruit-circuitpython-ina219-3.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-ina219-3.4.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-ina219-3.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-ina219-3.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/.pylintrc` & `adafruit-circuitpython-ina219-3.4.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-ina219-3.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ina219-3.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/LICENSE` & `adafruit-circuitpython-ina219-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ina219-3.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ina219-3.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ina219-3.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/PKG-INFO` & `adafruit-circuitpython-ina219-3.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ina219
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython library for INA219 high side DC current sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_INA219
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-ina219-3.4.8/README.rst` & `adafruit-circuitpython-ina219-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/PKG-INFO` & `adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ina219
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython library for INA219 high side DC current sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_INA219
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-ina219-3.4.8/adafruit_circuitpython_ina219.egg-info/SOURCES.txt` & `adafruit-circuitpython-ina219-3.4.9/adafruit_circuitpython_ina219.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/adafruit_ina219.py` & `adafruit-circuitpython-ina219-3.4.9/adafruit_ina219.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ina219-3.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/docs/conf.py` & `adafruit-circuitpython-ina219-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/docs/index.rst` & `adafruit-circuitpython-ina219-3.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/examples/ina219_simpletest.py` & `adafruit-circuitpython-ina219-3.4.9/examples/ina219_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina219-3.4.8/setup.py` & `adafruit-circuitpython-ina219-3.4.9/setup.py`

 * *Files identical despite different names*


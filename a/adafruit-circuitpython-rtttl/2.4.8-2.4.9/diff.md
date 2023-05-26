# Comparing `tmp/adafruit-circuitpython-rtttl-2.4.8.tar.gz` & `tmp/adafruit-circuitpython-rtttl-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-rtttl-2.4.8.tar", last modified: Fri Nov 19 20:09:12 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-rtttl-2.4.9.tar", last modified: Tue Dec  7 20:29:25 2021, max compression
```

## Comparing `adafruit-circuitpython-rtttl-2.4.8.tar` & `adafruit-circuitpython-rtttl-2.4.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.954980 adafruit-circuitpython-rtttl-2.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-11-19 20:09:12.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-11-19 20:09:12.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-19 20:09:12.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-11-19 20:09:12.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-19 20:09:12.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5737 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/adafruit_rtttl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5148 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/examples/rtttl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-19 20:09:12.958980 adafruit-circuitpython-rtttl-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2021-11-19 20:09:01.000000 adafruit-circuitpython-rtttl-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.074947 adafruit-circuitpython-rtttl-2.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-12-07 20:29:24.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-12-07 20:29:24.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 20:29:24.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-07 20:29:24.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-07 20:29:24.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5737 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/adafruit_rtttl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5148 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/examples/rtttl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-07 20:29:25.078947 adafruit-circuitpython-rtttl-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2021-12-07 20:29:12.000000 adafruit-circuitpython-rtttl-2.4.9/setup.py
```

### Comparing `adafruit-circuitpython-rtttl-2.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-rtttl-2.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-rtttl-2.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-rtttl-2.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-rtttl-2.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/.pylintrc` & `adafruit-circuitpython-rtttl-2.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rtttl-2.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/LICENSE` & `adafruit-circuitpython-rtttl-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-rtttl-2.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-rtttl-2.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-rtttl-2.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/PKG-INFO` & `adafruit-circuitpython-rtttl-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rtttl
-Version: 2.4.8
+Version: 2.4.9
 Summary: CircuitPython library for playing RTTTL melodies.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RTTTL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit rtttl tones melodies hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-rtttl-2.4.8/README.rst` & `adafruit-circuitpython-rtttl-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/PKG-INFO` & `adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rtttl
-Version: 2.4.8
+Version: 2.4.9
 Summary: CircuitPython library for playing RTTTL melodies.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RTTTL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit rtttl tones melodies hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-rtttl-2.4.8/adafruit_circuitpython_rtttl.egg-info/SOURCES.txt` & `adafruit-circuitpython-rtttl-2.4.9/adafruit_circuitpython_rtttl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/adafruit_rtttl.py` & `adafruit-circuitpython-rtttl-2.4.9/adafruit_rtttl.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         time.sleep(0.02)
 
 
 # pylint: disable-msg=too-many-arguments
 def play(
     pin,
     rtttl: str,
-    octave: int = Optional[None],
+    octave: Optional[int] = None,
     duration: Optional[int] = None,
     tempo: Optional[int] = None,
 ) -> None:
     """Play notes to a digialio pin using ring tone text transfer language (rtttl).
     :param ~digitalio.DigitalInOut pin: the speaker pin
     :param str rtttl: string containing rtttl
     :param int octave: represents octave number (default 6 starts at middle c)
```

### Comparing `adafruit-circuitpython-rtttl-2.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-rtttl-2.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/docs/conf.py` & `adafruit-circuitpython-rtttl-2.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/docs/index.rst` & `adafruit-circuitpython-rtttl-2.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/examples/rtttl_simpletest.py` & `adafruit-circuitpython-rtttl-2.4.9/examples/rtttl_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rtttl-2.4.8/setup.py` & `adafruit-circuitpython-rtttl-2.4.9/setup.py`

 * *Files identical despite different names*


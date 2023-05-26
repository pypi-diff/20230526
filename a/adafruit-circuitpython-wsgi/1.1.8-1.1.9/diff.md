# Comparing `tmp/adafruit-circuitpython-wsgi-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-wsgi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wsgi-1.1.8.tar", last modified: Fri Feb  4 21:08:29 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-wsgi-1.1.9.tar", last modified: Thu Mar 17 12:52:22 2022, max compression
```

## Comparing `adafruit-circuitpython-wsgi-1.1.8.tar` & `adafruit-circuitpython-wsgi-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.358144 adafruit-circuitpython-wsgi-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.358144 adafruit-circuitpython-wsgi-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.358144 adafruit-circuitpython-wsgi-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.358144 adafruit-circuitpython-wsgi-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-02-04 21:08:29.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-02-04 21:08:29.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 21:08:29.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 21:08:29.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-04 21:08:29.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/wsgi_app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/examples/wsgi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 21:08:29.362144 adafruit-circuitpython-wsgi-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-02-04 21:08:11.000000 adafruit-circuitpython-wsgi-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.217512 adafruit-circuitpython-wsgi-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.221511 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3862 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-17 12:52:22.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4218 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/wsgi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/examples/wsgi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-17 12:52:22.225511 adafruit-circuitpython-wsgi-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-03-17 12:52:09.000000 adafruit-circuitpython-wsgi-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-wsgi-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wsgi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-wsgi-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-wsgi-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-wsgi-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/.pylintrc` & `adafruit-circuitpython-wsgi-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wsgi-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/LICENSE` & `adafruit-circuitpython-wsgi-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wsgi-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-wsgi-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wsgi-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/PKG-INFO` & `adafruit-circuitpython-wsgi-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wsgi
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython framework for creating WSGI compatible web server applications.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WSGI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython wsgi web server webserver app webapp framework http https flask
 Platform: UNKNOWN
@@ -74,14 +74,16 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_WSGI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-wsgi-1.1.8/README.rst` & `adafruit-circuitpython-wsgi-1.1.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_WSGI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/PKG-INFO` & `adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wsgi
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython framework for creating WSGI compatible web server applications.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_WSGI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython wsgi web server webserver app webapp framework http https flask
 Platform: UNKNOWN
@@ -74,14 +74,16 @@
 
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/wsgi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_WSGI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-wsgi-1.1.8/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt` & `adafruit-circuitpython-wsgi-1.1.9/adafruit_circuitpython_wsgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/request.py` & `adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/adafruit_wsgi/wsgi_app.py` & `adafruit-circuitpython-wsgi-1.1.9/adafruit_wsgi/wsgi_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,16 +62,22 @@
 
         request = Request(environ)
 
         match = self._match_route(request.path, request.method.upper())
 
         if match:
             args, route = match
-            status, headers, resp_data = route["func"](request, *args)
-
+            try:
+                status, headers, resp_data = route["func"](request, *args)
+            except (ValueError, TypeError) as err:
+                raise RuntimeError(
+                    "Proper HTTP response return not given for request handler '{}'".format(
+                        route["func"].__name__
+                    )
+                ) from err
         start_response(status, headers)
         return resp_data
 
     def on_request(self, methods: List[str], rule: str, request_handler: Callable):
         """
         Register a Request Handler for a particular HTTP method and path.
         request_handler will be called whenever a matching HTTP request is received.
```

### Comparing `adafruit-circuitpython-wsgi-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-wsgi-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/docs/conf.py` & `adafruit-circuitpython-wsgi-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/docs/index.rst` & `adafruit-circuitpython-wsgi-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/examples/wsgi_simpletest.py` & `adafruit-circuitpython-wsgi-1.1.9/examples/wsgi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wsgi-1.1.8/setup.py` & `adafruit-circuitpython-wsgi-1.1.9/setup.py`

 * *Files identical despite different names*


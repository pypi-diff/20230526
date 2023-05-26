# Comparing `tmp/clams-python-0.6.3.tar.gz` & `tmp/clams-python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-0.6.3.tar", last modified: Sun May 21 00:24:36 2023, max compression
+gzip compressed data, was "clams-python-1.0.0.tar", last modified: Fri May 26 02:07:14 2023, max compression
```

## Comparing `clams-python-0.6.3.tar` & `clams-python-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-21 00:24:01.000000 clams-python-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-21 00:24:01.000000 clams-python-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 00:24:36.184832 clams-python-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-21 00:24:01.000000 clams-python-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:24:02.000000 clams-python-0.6.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.176832 clams-python-0.6.3/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/CLAMS-generic-readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/app/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/github/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/develop/templates/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-apps-project.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-assign.yml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/issue-close.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/develop/templates/github/workflows/publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/source/
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-05-21 00:24:01.000000 clams-python-0.6.3/clams/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.180832 clams-python-0.6.3/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:24:36.000000 clams-python-0.6.3/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 00:24:01.000000 clams-python-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:24:36.184832 clams-python-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-21 00:24:01.000000 clams-python-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:24:36.184832 clams-python-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-21 00:24:01.000000 clams-python-0.6.3/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-21 00:24:01.000000 clams-python-0.6.3/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.337439 clams-python-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 02:06:44.000000 clams-python-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 02:06:44.000000 clams-python-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-26 02:07:14.337439 clams-python-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-26 02:06:44.000000 clams-python-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 02:06:44.000000 clams-python-1.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.329439 clams-python-1.0.0/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/app/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/gha/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/gha/workflows/issue-apps-project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/gha/workflows/issue-assign.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/gha/workflows/issue-close.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/develop/templates/gha/workflows/publish.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-26 02:06:44.000000 clams-python-1.0.0/clams/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.333439 clams-python-1.0.0/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.337439 clams-python-1.0.0/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 02:07:14.000000 clams-python-1.0.0/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 02:06:44.000000 clams-python-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:07:14.337439 clams-python-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-26 02:06:44.000000 clams-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:07:14.337439 clams-python-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-26 02:06:44.000000 clams-python-1.0.0/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-26 02:06:44.000000 clams-python-1.0.0/tests/test_clamscli.py
```

### Comparing `clams-python-0.6.3/LICENSE` & `clams-python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/PKG-INFO` & `clams-python-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.3
+Version: 1.0.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.3/README.md` & `clams-python-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/__init__.py` & `clams-python-1.0.0/clams/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import sys
 
 from mmif import __specver__
 
-from clams import source
 from clams import develop
+from clams import source
 from clams.app import *
 from clams.app import __all__ as app_all
 from clams.appmetadata import AppMetadata
 from clams.restify import Restifier
-from clams.source import WorkflowSource
-from clams.develop import CookieCutter
 from clams.ver import __version__
 
-__all__ = [AppMetadata, Restifier, WorkflowSource] + app_all
+__all__ = [AppMetadata, Restifier] + app_all
 version_template = "{} (based on MMIF spec: {})"
 
 
 def prep_argparser():
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -24,15 +22,19 @@
         action='version',
         version=version_template.format(__version__, __specver__)
     )
     subparsers = parser.add_subparsers(title='sub-command', dest='subcmd')
     for subcmd_module in [source, develop]:
         subcmd_name = subcmd_module.__name__.rsplit('.')[-1]
         subcmd_parser = subcmd_module.prep_argparser(add_help=False)
-        subparsers.add_parser(subcmd_name, parents=[subcmd_parser], help=subcmd_module.prep_argparser.__doc__)
+        subparsers.add_parser(subcmd_name, parents=[subcmd_parser], 
+                              help=subcmd_module.describe_argparser()[0],
+                              description=subcmd_module.describe_argparser()[1],
+                              formatter_class=argparse.RawDescriptionHelpFormatter,
+                              )
     return parser
 
 
 def cli():
     parser = prep_argparser()
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
```

### Comparing `clams-python-0.6.3/clams/app/__init__.py` & `clams-python-1.0.0/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/appmetadata/__init__.py` & `clams-python-1.0.0/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/app/.gitignore` & `clams-python-1.0.0/clams/develop/templates/app/.gitignore`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/app/Containerfile` & `clams-python-1.0.0/clams/develop/templates/app/Containerfile`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/app/README.md` & `clams-python-1.0.0/clams/develop/templates/app/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -3,29 +3,35 @@
 Delete this section of the document once the app development is done, before publishing the repository. 
 
 ---
 This skeleton code is a scaffolding for Python-based CLAMS app development. Specifically, it contains 
 
 1. `app.py` and `metadata.py` to write the app 
 1. `requirements.txt` to specify python dependencies
-1. `.gitignore` file listing common ignored files
 1. `Containerfile` to containerize the app and specify system dependencies
+1. `.gitignore` and `.dorckrignore` files listing commonly ignored files
 1. an empty `LICENSE` file to replace with an actual license information of the app
 1. `CLAMS-generic-readme.md` file with basic instructions of app installation and execution
 1. This `README.md` file for additional information not specified in the generic readme file. 
-1. (optional) some GH actions workflow for issue/bug-report management
-1. (optional) a GH actions workflow to build and upload app images upon any push of a git tag
+1. A number of GitHub Actions workflows for issue/bug-report management 
+1. A GHA workflow to publish app images upon any push of a git tag
+   * **NOTE**: All GHA workflows included are designed to only work in repositories under `clamsproject` organization.
 
-Use the following section to document any additional information specific to this app. If your app works significantly 
-different from what's described in the generic readme file, be as specific as possible. 
+Before pushing your first commit, please make sure to delete this section of the document.
+
+Then use the following section to document any additional information specific to this app. If your app works significantly different from what's described in the generic readme file, be as specific as possible. 
 
 ---
 
 ## User instruction
 
+General user instruction for CLAMS apps is available at [CLAMS Apps documentation](https://apps.clams.ai/clamsapp/).
+
+Below is a list of additional information specific to this app.
+
 ### System requirments
 
 (Any system-level software required to run this app)
 
 ### Configurable runtime parameter
 
 (Parameters should be already well-described in the app metadata. But you can use this space to show examples, for instance.)
```

### Comparing `clams-python-0.6.3/clams/develop/templates/app/app.py` & `clams-python-1.0.0/clams/develop/templates/app/app.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/app/metadata.py` & `clams-python-1.0.0/clams/develop/templates/app/metadata.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/github/README.md` & `clams-python-1.0.0/clams/develop/templates/gha/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/develop/templates/github/workflows/publish.yml` & `clams-python-1.0.0/clams/develop/templates/gha/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/restify/__init__.py` & `clams-python-1.0.0/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/clams/source/__init__.py` & `clams-python-1.0.0/clams/source/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import itertools
 import json
 import sys
+import textwrap
 from os import path
 from typing import Union, Generator, List, Optional, Iterable
 
 from mmif import Mmif, Document, DocumentTypes, __specver__
 from mmif.serialize.mmif import MmifMetadata
 
 __all__ = ['WorkflowSource']
@@ -211,19 +212,28 @@
             mime=mime,
             location=location
         )
         pl.add_document(doc)
     return pl.produce().serialize(pretty=True)
 
 
-def prep_argparser(**kwargs):
+def describe_argparser():
     """
-    provides CLI to create a "source" MMIF json. A source MMIF is a MMIF with a list of source documents but empty views. It can be used as a starting point for a CLAMS workflow. 
+    returns two strings: one-line description of the argparser, and addition material, 
+    which will be shown in `clams --help` and `clams <subcmd> --help`, respectively.
     """
-    parser = argparse.ArgumentParser(**kwargs)
+    oneliner = 'provides CLI to create a "source" MMIF json.'
+    additional = textwrap.dedent("""
+    A source MMIF is a MMIF with a list of source documents but empty views. 
+    It can be used as a starting point for a CLAMS workflow. """)
+    return oneliner, oneliner + '\n\n' + additional
+
+
+def prep_argparser(**kwargs):
+    parser = argparse.ArgumentParser(description=describe_argparser()[1], formatter_class=argparse.RawDescriptionHelpFormatter, **kwargs)
     parser.add_argument(
         'documents',
         default=None,
         action='store',
         nargs='+',
         help="This list of documents should be colon-joined pairs of document types and file paths. A document type "
              "can be one of ``audio``, ``video``, ``text``, ``image``, or a MIME type string (such as video/mp4). The "
```

### Comparing `clams-python-0.6.3/clams_python.egg-info/PKG-INFO` & `clams-python-1.0.0/clams_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 0.6.3
+Version: 1.0.0
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-0.6.3/clams_python.egg-info/SOURCES.txt` & `clams-python-1.0.0/clams_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 ./requirements.txt
 clams/__init__.py
 clams/app/__init__.py
 clams/appmetadata/__init__.py
 clams/develop/__init__.py
 clams/develop/templates/app/.dockerignore
 clams/develop/templates/app/.gitignore
-clams/develop/templates/app/CLAMS-generic-readme.md
 clams/develop/templates/app/Containerfile
 clams/develop/templates/app/LICENSE
 clams/develop/templates/app/README.md
 clams/develop/templates/app/app.py
 clams/develop/templates/app/metadata.py
 clams/develop/templates/app/requirements.txt
-clams/develop/templates/github/README.md
-clams/develop/templates/github/workflows/issue-apps-project.yml
-clams/develop/templates/github/workflows/issue-assign.yml
-clams/develop/templates/github/workflows/issue-close.yml
-clams/develop/templates/github/workflows/publish.yml
+clams/develop/templates/gha/README.md
+clams/develop/templates/gha/workflows/issue-apps-project.yml
+clams/develop/templates/gha/workflows/issue-assign.yml
+clams/develop/templates/gha/workflows/issue-close.yml
+clams/develop/templates/gha/workflows/publish.yml
 clams/restify/__init__.py
 clams/serve/__init__.py
 clams/source/__init__.py
 clams/ver/__init__.py
 clams_python.egg-info/PKG-INFO
 clams_python.egg-info/SOURCES.txt
 clams_python.egg-info/dependency_links.txt
```

### Comparing `clams-python-0.6.3/setup.py` & `clams-python-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/tests/test_clamsapp.py` & `clams-python-1.0.0/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-0.6.3/tests/test_clamscli.py` & `clams-python-1.0.0/tests/test_clamscli.py`

 * *Files identical despite different names*


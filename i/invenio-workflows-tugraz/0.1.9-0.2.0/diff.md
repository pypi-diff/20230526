# Comparing `tmp/invenio-workflows-tugraz-0.1.9.tar.gz` & `tmp/invenio-workflows-tugraz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-workflows-tugraz-0.1.9.tar", last modified: Wed May 10 09:58:40 2023, max compression
+gzip compressed data, was "invenio-workflows-tugraz-0.2.0.tar", last modified: Fri May 26 07:21:10 2023, max compression
```

## Comparing `invenio-workflows-tugraz-0.1.9.tar` & `invenio-workflows-tugraz-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.736153 invenio-workflows-tugraz-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/
--rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/iso6393.json
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/theses.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.740153 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 09:58:40.000000 invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      437 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-10 09:58:40.748153 invenio-workflows-tugraz-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:58:40.744153 invenio-workflows-tugraz-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 09:58:34.000000 invenio-workflows-tugraz-0.1.9/tests/test_invenio_workflows_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.270400 invenio-workflows-tugraz-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.274400 invenio-workflows-tugraz-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.274400 invenio-workflows-tugraz-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.278400 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.278400 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   939307 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/data/iso6393.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-26 07:21:01.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/theses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.278400 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 07:21:10.000000 invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:21:10.282400 invenio-workflows-tugraz-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-26 07:21:02.000000 invenio-workflows-tugraz-0.2.0/tests/test_invenio_workflows_tugraz.py
```

### Comparing `invenio-workflows-tugraz-0.1.9/.editorconfig` & `invenio-workflows-tugraz-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/.github/workflows/tests.yml` & `invenio-workflows-tugraz-0.2.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/CONTRIBUTING.rst` & `invenio-workflows-tugraz-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/LICENSE` & `invenio-workflows-tugraz-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/MANIFEST.in` & `invenio-workflows-tugraz-0.2.0/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 recursive-include invenio_workflows_tugraz/translations *.po *.pot *.mo
 
 # added by check-manifest
 include *.md
 include *.rst
 include *.sh
 include *.txt
+include *.toml
 include babel.ini
 include pytest.ini
 recursive-include docs *.bat
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
```

### Comparing `invenio-workflows-tugraz-0.1.9/PKG-INFO` & `invenio-workflows-tugraz-0.2.0/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,85 @@
-Metadata-Version: 2.1
-Name: invenio-workflows-tugraz
-Version: 0.1.9
-Summary: "This package serves as a place for the workflows of the repository of the TU Graz."
-Home-page: https://github.com/tu-graz-library/invenio-workflows-tugraz
-Author: Graz University of Technology
-Author-email: info@tugraz.at
-License: MIT
-Keywords: invenio workflows TUGraz
-Platform: any
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Provides-Extra: tests
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-# invenio-workflows-tugraz
-Implements TU Graz specific workflows
-
 ..
     Copyright (C) 2022 Graz University of Technology.
 
     invenio-workflows-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.2.0 (release 2023-05-26)
+
+- fix: use data instead of metadata
+- fix: tests
+- fix: 971 not used all additions
+- theses: rewrite access in update func
+- theses: add update_func to the workflow
+- theses: add embargo on creation
+- theses: remove locked generator
+- setup: migrate to ruff
+
+
+Version v0.1.19 (release 2023-05-17)
+
+- fix: apply requested changes for field 008
+
+
+Version v0.1.18 (release 2023-05-12)
+
+- fix: position 19 was the wrong value
+- fix: keyw was not processed
+- theses: change visitor api
+- theses: implement sorting for 971 fields
+- fix: revert back change of 007 field
+- fix: 245 field missed author
+
+
+Version v0.1.17 (release 2023-05-11)
+
+- fix: errors
+
+
+Version v0.1.16 (release 2023-05-11)
+
+- fix: int not serializable
+
+
+Version v0.1.15 (release 2023-05-11)
+
+- theses: fix german language code
+
+
+Version v0.1.14 (release 2023-05-11)
+
+
+
+
+Version v0.1.13 (release 2023-05-10)
+
+- theses: apply requested marc21 field changes
+- fix: date for status
+
+
+Version v0.1.12 (release 2023-05-10)
+
+- fix: the crap from last commit
+
+
+Version v0.1.11 (release 2023-05-10)
+
+- fix: date and format where not compatible
+
+
+Version v0.1.10 (release 2023-05-10)
+
+- fix: used wrong date format
+
+
 Version v0.1.9 (release 2023-05-10)
 
 - theses: apply marc21 request changes
 
 
 Version v0.1.8 (release 2023-04-25)
 
@@ -78,9 +124,7 @@
 
 
 Version v0.1.0 (release 2023-01-18)
 
 
 
 
-
-
```

### Comparing `invenio-workflows-tugraz-0.1.9/babel.ini` & `invenio-workflows-tugraz-0.2.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/docs/Makefile` & `invenio-workflows-tugraz-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/docs/conf.py` & `invenio-workflows-tugraz-0.2.0/docs/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 project = "invenio-workflows-tugraz"
 copyright = "2022, Graz University of Technology"
 author = "Graz University of Technology"
 
 nitpick_ignore = [
     ("py:class", "invenio_campusonline.types.CampusOnlineConfigs"),
     ("py:class", "invenio_pure.types.PureConfigs"),
+    ("py:class", "flask.app.Flask"),
+    ("py:class", "invenio_records_marc21.services.services.Marc21RecordService"),
+    ("py:class", "invenio_alma.services.sru.AlmaSRUService"),
+    ("py:class", "flask_principal.Identity"),
+    ("py:class", "collections.abc.Callable"),
+    ("py:class", "invenio_records_resources.services.records.results.RecordItem"),
 ]
 
 # -- General configuration ---------------------------------------------------
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.coverage",
```

### Comparing `invenio-workflows-tugraz-0.1.9/docs/index.rst` & `invenio-workflows-tugraz-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/docs/make.bat` & `invenio-workflows-tugraz-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/data/iso6393.json` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/data/iso6393.json`

 * *Files identical despite different names*

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/ext.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/ext.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,43 +2,48 @@
 #
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
-"""This package serves as a place for the workflows of the repository of the TU Graz."""
+"""Initialize the package."""
+
+from flask import Flask
 
 from . import config
 
 
 class InvenioWorkflowsTugraz:
     """invenio-workflows-tugraz extension."""
 
-    def __init__(self, app=None):
+    def __init__(self, app: Flask = None) -> None:
         """Extension initialization."""
         if app:
             self.init_app(app)
 
-    def init_app(self, app):
+    def init_app(self, app: Flask) -> None:
         """Flask application initialization."""
         self.init_config(app)
         app.extensions["invenio-workflows-tugraz"] = self
 
-    def init_config(self, app):
+    def init_config(self, app: Flask) -> None:
         """Initialize configuration."""
         app.config.setdefault("ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATORS", [])
         app.config.setdefault("ALMA_ALMA_RECORDS_CREATE_AGGREGATORS", [])
         app.config.setdefault("CAMPUSONLINE_THESES_FILTERS", [])
 
         for k in dir(config):
             if k == "WORKFLOW_ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATORS":
                 app.config["ALMA_REPOSITORY_RECORDS_UPDATE_AGGREGATORS"] += getattr(
-                    config, k
+                    config,
+                    k,
                 )
+            elif k == "WORKFLOW_ALMA_REPOSITORY_RECORDS_UPDATE_FUNC":
+                app.config["ALMA_REPOSITORY_RECORDS_UPDATE_FUNC"] = getattr(config, k)
 
             elif k == "WORKFLOW_ALMA_ALMA_RECORDS_CREATE_AGGREGATORS":
                 app.config["ALMA_ALMA_RECORDS_CREATE_AGGREGATORS"] += getattr(config, k)
 
             elif k == "WORKFLOW_CAMPUSONLINE_THESES_FILTERS":
                 app.config["CAMPUSONLINE_THESES_FILTERS"] += getattr(config, k)
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/convert.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,206 +1,219 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Open Access Workflow."""
 
 from json import load
-from os.path import dirname, join
+from pathlib import Path
 
 from invenio_records_marc21 import Marc21Metadata
 
 
 class Converter:
     """Converter base class to convert one format into another."""
 
-    def __init__(self):
-        """Default Constructor of the class."""
+    def __init__(self) -> None:
+        """Construct of the class."""
         # Cache iso639-3 language codes to dict
         self.languages = self.initialize_languages()
 
     def initialize_languages(self) -> dict:
         """Initialize language cache dictionary."""
-        path = join(dirname(__file__), "../data", "iso6393.json")
+        path = Path(__file__).parent / "../data/iso6393.json"
 
-        with open(path) as fp:
+        with Path(path).open() as fp:
             languages = filter(lambda obj: "iso6393" in obj, load(fp))
 
         return {language["name"]: language["iso6393"] for language in languages}
 
-    def convert(self, value: object, record: Marc21Metadata):
+    def convert(self, value: object, record: Marc21Metadata) -> None:
         """Convert record from Pure JSON format to MARC21XML."""
-        for attribute, value in value.items():
-            self.convert_attribute(attribute, value, record)
+        for attribute, val in value.items():
+            self.convert_attribute(attribute, val, record)
 
-    def convert_attribute(self, attribute: str, value: object, record: Marc21Metadata):
-        """Traverse first level elements of dictionary and extract necessary attributes."""
-        convert_function = getattr(self, f"convert_{attribute}", lambda *args: None)
+    def convert_attribute(
+        self,
+        attribute: str,
+        value: object,
+        record: Marc21Metadata,
+    ) -> None:
+        """Traverse first level elements of dictionary and extract attributes."""
+        convert_function = getattr(self, f"convert_{attribute}", lambda _: None)
         convert_function(value, record)
 
 
 class Pure2Marc21(Converter):
     """Pure to marc21 converter class."""
 
-    def convert_abstract(self, value: dict, record: Marc21Metadata):
+    def convert_abstract(self, value: dict, record: Marc21Metadata) -> None:
         """Add the abstract to the Marc21Metadata."""
         for abstract in value["text"]:
             record.emplace_field("520...", value=abstract["value"])
 
-    def convert_additionalLinks(self, value: list, record: Marc21Metadata):
+    def convert_additionalLinks(self, value: list, record: Marc21Metadata) -> None:
         """Add the additionalLinks attribute to the Marc21Metadata."""
         for link in value:
             if "url" in link:
                 record.emplace_field("856.4.1.u", value=link["url"])
 
-    def convert_bibliographicalNote(self, value: dict, record: Marc21Metadata):
+    def convert_bibliographicalNote(self, value: dict, record: Marc21Metadata) -> None:
         """Add the bibliographicalNote attribute to the Marc21Metadata."""
         for text in value["text"]:
             record.emplace_field("500...", value=text["value"])
 
-    def convert_edition(self, value: str, record: Marc21Metadata):
+    def convert_edition(self, value: str, record: Marc21Metadata) -> None:
         """Add the edition attribute to the Marc21Metadata."""
         record.emplace_field("250...", value=value)
 
-    def convert_electronicIsbns(self, value: list, record: Marc21Metadata):
+    def convert_electronicIsbns(self, value: list, record: Marc21Metadata) -> None:
         """Add the electronicIsbns attribute to the Marc21Metadata."""
         record.emplace_field("020...", value=str(value[0]).strip())
 
-    def convert_event(self, value: dict, record: Marc21Metadata):
+    def convert_event(self, value: dict, record: Marc21Metadata) -> None:
         """Add the event attribute to the Marc21Metadata."""
         for event_name in value["name"]["text"]:
             record.emplace_field("711.2..", value=event_name["value"])
 
-    def convert_isbns(self, value: list, record: Marc21Metadata):
+    def convert_isbns(self, value: list, record: Marc21Metadata) -> None:
         """Add the isbns attribute to the Marc21Metadata."""
         for isbn in value:
             record.emplace_field("020...", value=isbn)
 
-    def convert_journalAssociation(self, value: dict, record: Marc21Metadata):
+    def convert_journalAssociation(self, value: dict, record: Marc21Metadata) -> None:
         """Add the journalAssociation attribute to the Marc21Metadata."""
         value = value["title"]["value"]
         record.emplace_field("773.0.8.t", value=value)
 
-    def convert_journalNumber(self, value: str, record: Marc21Metadata):
+    def convert_journalNumber(self, value: str, record: Marc21Metadata) -> None:
         """Add the journalNumber attribute to the Marc21Metadata."""
         record.emplace_field("773.0.8.g", value=value)
 
-    def convert_keywordGroups(self, value: list, record: Marc21Metadata):
+    def convert_keywordGroups(self, value: list, record: Marc21Metadata) -> None:
         """Add the keywordGroups attribute to the Marc21Metadata."""
         for item in value:
             keyword_group = KeywordGroup()
             keyword_group.convert(item, record)
 
-    def convert_language(self, value: dict, record: Marc21Metadata):
+    def convert_language(self, value: dict, record: Marc21Metadata) -> None:
         """Add the language attribute to the Marc21Metadata."""
         for locale in value["term"]["text"]:
             language = locale["value"]
             language_iso6393 = self.languages[language]
             record.emplace_field("041...", value=language_iso6393)
 
-    def convert_managingOrganisationalUnit(self, value: dict, record: Marc21Metadata):
+    def convert_managingOrganisationalUnit(
+        self,
+        value: dict,
+        record: Marc21Metadata,
+    ) -> None:
         """Add the managingOrganisationalUnit attribute to the Marc21Metadata."""
         for locale in value["name"]["text"]:
             record.emplace_unique_field("100.1..u", value=locale["value"])
             record.emplace_unique_field("700.1..u", value=locale["value"])
 
-    def convert_numberOfPages(self, value: int, record: Marc21Metadata):
+    def convert_numberOfPages(self, value: int, record: Marc21Metadata) -> None:
         """Add the numberOfPages attribute to the Marc21Metadata."""
         record.emplace_field("300...", value=str(value))
 
-    def convert_organisationalUnits(self, value: list, record: Marc21Metadata):
+    def convert_organisationalUnits(self, value: list, record: Marc21Metadata) -> None:
         """Add the organisationalUnits attribute to the Marc21Metadata."""
         for o_unit in value:
             for locale in o_unit["name"]["text"]:
                 record.emplace_unique_field("100.1..u", value=locale["value"])
                 record.emplace_unique_field("700.1..u", value=locale["value"])
 
-    def convert_pages(self, value: str, record: Marc21Metadata):
+    def convert_pages(self, value: str, record: Marc21Metadata) -> None:
         """Add the pages attriute to the Marc21Metadata."""
         pages = value
         record.emplace_field("300...", value=pages)
 
-    def convert_patentNumber(self, value: str, record: Marc21Metadata):
+    def convert_patentNumber(self, value: str, record: Marc21Metadata) -> None:
         """Add the patentNumber attribute to the Marc21Metadata."""
         record.emplace_field("013...", value=value)
 
-    def convert_peerReview(self, value: bool, record: Marc21Metadata):
+    def convert_peerReview(
+        self,
+        value: bool,  # noqa: FBT001
+        record: Marc21Metadata,
+    ) -> None:
         """Add the peerReview attribute to the Marc21Metadata."""
         if value:
             status = "Refereed/Peer-reviewed"
             record.emplace_field("500...", value=status)
 
-    def convert_placeOfPublication(self, value: str, record: Marc21Metadata):
+    def convert_placeOfPublication(self, value: str, record: Marc21Metadata) -> None:
         """Add the placeOfPublication attribute to the Marc21Metadata."""
         record.emplace_field("264...", value=value)
 
-    def convert_publicationSeries(self, value: list, record: Marc21Metadata):
+    def convert_publicationSeries(self, value: list, record: Marc21Metadata) -> None:
         """Add the publicationSeries attribute to the Marc21Metadata."""
         for series in value:
             record.emplace_field("490.0..", value=series["name"])
 
-    def convert_publicationStatuses(self, value: list, record: Marc21Metadata):
+    def convert_publicationStatuses(self, value: list, record: Marc21Metadata) -> None:
         """Add the publicationStatuses attribute to the Marc21Metadata."""
         for entry in value:
             publication_status = PublicationStatus()
             publication_status.convert(entry, record)
 
-    def convert_publisher(self, value: dict, record: Marc21Metadata):
+    def convert_publisher(self, value: dict, record: Marc21Metadata) -> None:
         """Add the publisher attribute to the Marc21Metadata."""
         for text in value["name"]["text"]:
             record.emplace_field("264...b", value=text["value"])
 
-    def convert_relatedProjects(self, value: list, record: Marc21Metadata):
+    def convert_relatedProjects(self, value: list, record: Marc21Metadata) -> None:
         """Add the relatedProjects attribute to the Marc21Metadata."""
         for entry in value:
             for locale in entry["name"]["text"]:
                 record.emplace_field("536...", value=locale["value"])
 
-    def convert_subTitle(self, value: dict, record: Marc21Metadata):
+    def convert_subTitle(self, value: dict, record: Marc21Metadata) -> None:
         """Add the subTitle attribute to the Marc21Metadata."""
         record.emplace_field("245.1.0.b", value=value["value"])
 
-    def convert_title(self, value: dict, record: Marc21Metadata):
+    def convert_title(self, value: dict, record: Marc21Metadata) -> None:
         """Add the title attribute to the Marc21Metadata."""
         record.emplace_field("245.1.0.", value=value["value"])
 
-    def convert_volume(self, value: str, record: Marc21Metadata):
+    def convert_volume(self, value: str, record: Marc21Metadata) -> None:
         """Add the volume attribute to the Marc21Metadata."""
         record.emplace_field("490.0..", value=value)
         record.emplace_field("773.0.8.g", value=value)
 
 
 class KeywordGroup(Converter):
     """Class to convert the keywordgroup attribute."""
 
-    def convert_keywordContainers(self, value: list, record: Marc21Metadata):
+    def convert_keywordContainers(self, value: list, record: Marc21Metadata) -> None:
         """Add keywords."""
         for item in value:
             self.convert(item, record)
 
-    def convert_freeKeywords(self, value: list, record: Marc21Metadata):
+    def convert_freeKeywords(self, value: list, record: Marc21Metadata) -> None:
         """Add free keywords."""
         for free_keyword in value:
             for word in free_keyword["freeKeywords"]:
                 record.emplace_field("650..4.g", value=word)
 
-    def convert_structuredKeyword(self, value: dict, record: Marc21Metadata):
+    def convert_structuredKeyword(self, value: dict, record: Marc21Metadata) -> None:
         """Add free keywords."""
         for word in value["term"]["text"]:
             record.emplace_field("650..4.", value=word["value"])
 
 
 class PublicationStatus(Converter):
     """Class to convert publication status."""
 
-    def convert_publicationDate(self, value: dict, record: Marc21Metadata):
+    def convert_publicationDate(self, value: dict, record: Marc21Metadata) -> None:
         """Add the publication date to the Marc21Metadata."""
         record.emplace_field("264...c", value=value["year"])
 
-    def convert_publicationStatus(self, value: dict, record: Marc21Metadata):
+    def convert_publicationStatus(self, value: dict, record: Marc21Metadata) -> None:
         """Add the publication status to the Marc21Metadata."""
         for text in value["term"]["text"]:
             record.emplace_field("250...", value=text["value"])
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/utils.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Openaccess Workflow utils."""
 
 from invenio_pure import URL, PureID, PureRecord, PureRuntimeError
 from invenio_records_marc21 import check_about_duplicate
 
 from .types import PureId
 
 
 @check_about_duplicate.register
-def _(value: PureId):
+def _(value: PureId) -> None:
     """Check about double pure id."""
     check_about_duplicate(str(value), value.category)
 
 
 def access_type(electronic_version: dict) -> str:
     """Get Access type."""
     try:
@@ -48,18 +48,18 @@
     """Extract pure id."""
     return pure_record["pureId"]
 
 
 def extract_file_url(pure_record: PureRecord) -> URL:
     """Extract file url."""
 
-    def condition(item):
-        return access_type(item) in ["Open", "Offen"] and license_type(item).startswith(
-            "CC BY"
-        )
+    def condition(item: dict) -> bool:
+        condition_1 = access_type(item) in ["Open", "Offen"]
+        condition_2 = license_type(item).startswith("CC BY")
+        return condition_1 and condition_2
 
     file_urls = []
     for electronic_version in pure_record["electronicVersions"]:
         try:
             file_url = electronic_version["file"]["fileURL"]
             if condition(electronic_version):
                 file_urls.append(file_url)
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/openaccess/workflow.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/openaccess/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # Copyright (C) 2022 Graz University of Technology.
 #
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Open Access Workflow."""
-from typing import Callable
+from collections.abc import Callable
 
 from invenio_config_tugraz import get_identity_from_user_by_email
 from invenio_pure import PureConfigs, PureRecord
 from invenio_records_marc21 import (
     DuplicateRecordError,
     Marc21Metadata,
     check_about_duplicate,
     create_record,
     current_records_marc21,
 )
+from invenio_records_resources.services.records.results import RecordItem
 
 from .convert import Pure2Marc21
 from .types import PureId
 from .utils import (
     access_type,
     extract_file_url,
     extract_pure_id,
@@ -30,23 +31,26 @@
 )
 
 
 def pure_import_func(
     pure_record: PureRecord,
     configs: PureConfigs,
     download_file: Callable,
-) -> None:
+) -> RecordItem:
     """Import record from pure into the repository."""
     pure_id = extract_pure_id(pure_record)
     file_urls = extract_file_url(pure_record)
 
     file_paths = []
     for i, file_url in enumerate(file_urls):
         file_path = download_file(
-            f"{pure_id}-{i}", file_url, configs.pure_username, configs.pure_password
+            f"{pure_id}-{i}",
+            file_url,
+            configs.pure_username,
+            configs.pure_password,
         )
         file_paths.append(file_path)
 
     marc21_record = Marc21Metadata()
     convert = Pure2Marc21()
     convert.convert(pure_record, marc21_record)
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/convert.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,242 +5,290 @@
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Convert from CampusOnline to Marc21."""
 
 from datetime import datetime
+from operator import itemgetter
 from re import split
 from xml.etree.ElementTree import Element
 
 from invenio_records_marc21.services.record.metadata import Marc21Metadata, QName
 
 
-def construct_name(name):
+def construct_name(name: dict[str, str]) -> str:
     """Construct name."""
     return f"{name['ln']}, {name['fn']}"
 
 
-def language_decode(lang):
+def language_decode(lang: str) -> str:
     """Language decode."""
     languages = {
-        "DE": "deu",
+        "DE": "ger",
         "EN": "eng",
     }
     return languages.get(lang, "PLATZHALTER")
 
 
 class Visitor:
     """Visitor base class."""
 
-    def process(self, node: Element, record: Marc21Metadata):
+    def process(self, node: Element, record: Marc21Metadata) -> None:
         """Execute the corresponding method to the tag name."""
 
-        def func_not_found(*args, **kwargs):
+        def func_not_found(*_: dict, **__: dict) -> None:
             localname = QName(node).localname
             namespace = QName(node).namespace
-            raise ValueError(f"NO visitor node: '{localname}' ns: '{namespace}'")
+            msg = f"NO visitor node: '{localname}' ns: '{namespace}'"
+            raise ValueError(msg)
 
         tag_name = QName(node).localname
         visit_func = getattr(self, f"visit_{tag_name}", func_not_found)
-        result = visit_func(node, record)
-        return result
+        return visit_func(node, record)
 
-    def visit_attr(self, node, record: Marc21Metadata):
-        """Base function for attr."""
+    def visit(self, node: Element, record: Marc21Metadata) -> None:
+        """Entry point for visitor."""
+        for child in node:
+            self.process(child, record)
+
+    def visit_attr(self, node: Element, record: Marc21Metadata) -> None:
+        """Run attr function."""
         key = node.attrib["key"]
 
-        def func_not_found(*args, **kwargs):
-            raise ValueError(f"NO visitor node: '{key}'")
+        def func_not_found(*_: dict, **__: dict) -> None:
+            msg = f"NO visitor node: '{key}'"
+            raise ValueError(msg)
 
         visit_func = getattr(self, f"visit_{key}", func_not_found)
-        result = visit_func(node, record)
-        return result
+        visit_func(node, record)
 
-    def visit(self, node, record: Marc21Metadata):
-        """Entry point for visitor."""
-        for child in node:
-            self.process(child, record)
+    def convert(self, node: Element, record: Marc21Metadata) -> None:
+        """Convert."""
+        self.visit(node, record)
+
+
+class ThesesLocalField:
+    """Class to handle the various local fields."""
+
+    def __init__(self) -> None:
+        """Construct class."""
+        self.theses_local_field = {}
+
+    def add(self, key: str, value: dict) -> None:
+        """Add key value pair."""
+        if key not in self.theses_local_field:
+            self.theses_local_field[key] = []
+
+        if value not in self.theses_local_field[key]:
+            self.theses_local_field[key].append(value)
+
+    def items(self) -> tuple:
+        """Return list of tuples."""
+        for key, values in self.theses_local_field.items():
+            for subfs in values:
+                yield (key, subfs)
 
 
 class CampusOnlineToMarc21(Visitor):
     """Convertor from CampusOnline to Marc21."""
 
-    def __init__(self, record: Marc21Metadata):
-        """Constructor."""
+    def __init__(self, record: Marc21Metadata) -> None:
+        """Construct."""
         super().__init__()
         self.author_name = "N/A"
         self.state = ""
         self.metaclass_name = ""
+        self.theses_local_field = ThesesLocalField()
 
         record.emplace_leader("07878nam a2200421 c 4500")
         record.emplace_controlfield("007", "cr#|||||||||||")
-        record.emplace_controlfield("008", "230501s########   #a###om####000#0#eng c")
+        record.emplace_controlfield("008", "230501s????####   #####om####|||#|#### c")
         record.emplace_datafield(
-            "040...", subfs={"a": "AT-UBTUG", "b": "ger", "d": "AT-UBTUG", "e": "rda"}
+            "040...",
+            subfs={"a": "AT-UBTUG", "b": "ger", "d": "AT-UBTUG", "e": "rda"},
         )
         record.emplace_datafield("044...", subfs={"c": "XA-AT"})
         record.emplace_datafield("264..1.", subfs={"a": "Graz", "c": "DATUM"})
         record.emplace_datafield(
-            "300...", subfs={"a": "1 Online-Ressource ( Seiten )", "b": "ill"}
+            "300...",
+            subfs={"a": "1 Online-Ressource (Seiten)", "b": "ill"},
         )
         record.emplace_datafield("336...", subfs={"b": "txt"})
         record.emplace_datafield("337...", subfs={"b": "c"})
         record.emplace_datafield("338...", subfs={"b": "cr"})
         record.emplace_datafield("347...", subfs={"a": "Textdatei", "b": "PDF"})
         record.emplace_datafield(
-            "506.0..", subfs={"2": "star", "f": "Unrestricted online access"}
+            "506.0..",
+            subfs={"2": "star", "f": "Unrestricted online access"},
         )
         record.emplace_datafield("546...", subfs={"a": "Zusammenfassung in"})
         record.emplace_datafield(
             "655..7.",
             subfs={
                 "a": "Hochschulschrift",
                 "0": "(DE-588)4113937-9",
                 "2": "gnd-content",
             },
         )
-        # TODO: find out what in 008 should be
 
-    def visit(self, node, record: Marc21Metadata):
-        """Override visit."""
-        super().visit(node, record)
+    def convert(self, node: Element, record: Marc21Metadata) -> None:
+        """Override convert."""
+        super().convert(node, record)
+        for key, subfs in sorted(self.theses_local_field.items(), key=itemgetter(0)):
+            record.emplace_datafield(key, subfs=subfs)
 
-    def visit_ID(self, node, record: Marc21Metadata):
+    def visit_ID(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ID."""
         record.emplace_datafield(
-            "995...", subfs={"i": "TUGRAZonline", "a": node.text, "9": "local"}
+            "995...",
+            subfs={"i": "TUGRAZonline", "a": str(node.text), "9": "local"},
         )
 
-    def visit_PAG(self, node, record: Marc21Metadata):
+    def visit_PAG(self, node: Element, record: Marc21Metadata) -> None:
         """Visit PAG."""
 
-    def visit_CO(self, node: Element, record: Marc21Metadata):
+    def visit_CO(self, node: Element, record: Marc21Metadata) -> None:
         """Visit CO."""
 
-    def visit_CHD(self, node: Element, record: Marc21Metadata):
+    def visit_CHD(self, node: Element, record: Marc21Metadata) -> None:
         """Visit CHD."""
 
-    def visit_EJAHR(self, node: Element, record: Marc21Metadata):
+    def visit_EJAHR(self, node: Element, record: Marc21Metadata) -> None:
         """Visit EJAHR."""
 
-    def visit_ARCHD(self, node: Element, record: Marc21Metadata):
+    def visit_ARCHD(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ARCHD."""
 
-    def visit_PUBD(self, node: Element, record: Marc21Metadata):
+    def visit_PUBD(self, node: Element, record: Marc21Metadata) -> None:
         """Visit PUBD."""
 
-    def visit_PUBLIC(self, node: Element, record: Marc21Metadata):
+    def visit_PUBLIC(self, node: Element, record: Marc21Metadata) -> None:
         """Visit PUBLIC."""
 
-    def visit_STATUS(self, node: Element, record: Marc21Metadata):
+    def visit_STATUS(self, node: Element, record: Marc21Metadata) -> None:
         """Visit status."""
 
-    def visit_STATUSD(self, node: Element, record: Marc21Metadata):
+    def visit_STATUSD(self, node: Element, _: Marc21Metadata) -> None:
         """Visit Status date."""
         try:
-            self.year = datetime.strptime(node.text, "%Y-%M-%D %H:%M:%S").year
+            year = datetime.strptime(node.text, "%Y-%m-%d %H:%M:%S").year
         except ValueError:
-            self.year = "JAHR"
+            year = "JAHR"
+        self.year = str(year)
 
-    def visit_ORG(self, node: Element, record: Marc21Metadata):
+    def visit_ORG(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_ORGP(self, node: Element, record: Marc21Metadata):
+    def visit_ORGP(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         orgp = node.text.split("&gt;")
 
         faculty = orgp[1] if len(orgp) > 1 else ""
-        institute = orgp[2] if len(orgp) > 2 else ""
+        institute = orgp[2] if len(orgp) > 2 else ""  # noqa: PLR2004
 
-        record.emplace_datafield(
+        self.theses_local_field.add(
             "971.5..",
-            subfs={"a": "Technische Universität Graz", "b": faculty, "c": institute},
+            {
+                "a": "Technische Universität Graz",
+                "b": faculty.strip(),
+                "c": institute.strip(),
+                "d": "NUMMER",
+            },
         )
 
-    def visit_TYPKB(self, node: Element, record: Marc21Metadata):
+    def visit_TYPKB(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         value = "HS-DISS" if node.text == "DISS" else "HS-MASTER"
         record.emplace_datafield("970.2..", subfs={"d": value})
 
-    def visit_TYP(self, node: Element, record: Marc21Metadata):
+    def visit_TYP(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         if self.state == "metaobj":
             self.typ = node.text
             return
 
         record.emplace_datafield(
             "502...",
-            subfs={"b": node.text, "c": "Technische Universität Graz", "d": self.year},
+            subfs={
+                "b": node.text,
+                "c": "Technische Universität Graz",
+                "d": str(self.year),
+            },
         )
 
-    def visit_ZUGKB(self, node: Element, record: Marc21Metadata):
+    def visit_ZUGKB(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_ZUG(self, node: Element, record: Marc21Metadata):
+    def visit_ZUG(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_SPSTAT(self, node: Element, record: Marc21Metadata):
+    def visit_SPSTAT(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_SPVON(self, node: Element, record: Marc21Metadata):
+    def visit_SPVON(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         text = node.text
-        self.spvon = text.split(" ")[0] if text else ""
+        self.spvon = text if text else ""
 
-    def visit_SPBIS(self, node: Element, record: Marc21Metadata):
+    def visit_SPBIS(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         text = node.text
-        in_format = "%Y-%M-%D %H:%M:%S"
-        out_format = "%D-%M-%Y"
+
+        if not text:
+            return
+
+        in_format = "%Y-%m-%d %H:%M:%S"
+        out_format = "%d.%m.%Y"
+
         spvon = datetime.strptime(self.spvon, in_format).strftime(out_format)
-        spbis = datetime.strptime(text.split(" ")[0], in_format).strftime(out_format)
+        spbis = datetime.strptime(text, in_format).strftime(out_format)
 
-        if text:
-            record.emplace_datafield(
-                "971.7..",
-                subfs={"a": "gesperrt", "b": spvon, "c": spbis},
-            )
+        self.theses_local_field.add(
+            "971.7..",
+            {"a": "gesperrt", "b": spvon, "c": spbis},
+        )
 
-    def visit_SPBGR(self, node: Element, record: Marc21Metadata):
+    def visit_SPBGR(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_OLANG(self, node: Element, record: Marc21Metadata):
+    def visit_OLANG(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         self.object_language = node.text
         record.emplace_datafield("041...a", value=language_decode(node.text))
 
-    def visit_TLANGS(self, node: Element, record: Marc21Metadata):
+    def visit_TLANGS(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_VOLLTEXT(self, node: Element, record: Marc21Metadata):
+    def visit_VOLLTEXT(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_metaclass(self, node: Element, record: Marc21Metadata):
+    def visit_metaclass(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         self.visit(node, record)
 
-    def visit_name(self, node: Element, record: Marc21Metadata):
+    def visit_name(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         self.metaclass_name = node.text
 
-    def visit_metaobj(self, node: Element, record: Marc21Metadata):
+    def visit_metaobj(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         if self.metaclass_name not in ["AUTHOR", "TEXT", "SUPERVISOR"]:
             return
 
         self.state = "metaobj"
         self.name = {"fn": "", "ln": ""}
 
         self.visit(node, record)
 
         if self.metaclass_name == "AUTHOR":
-            self.author_name = construct_name(self.name)
+            self.author_name = self.name
             record.emplace_datafield(
-                "100.1..", subfs={"a": self.author_name, "4": "aut"}
+                "100.1..",
+                subfs={"a": construct_name(self.author_name), "4": "aut"},
             )
 
         if self.metaclass_name == "SUPERVISOR":
             types = {
                 "BTEXT": "0",
                 "BTTUG": "0",
                 "MBTUG": "2",
@@ -249,72 +297,75 @@
                 "2BUTUG": "1",
                 "3BUTUG": "1",
                 "4BUTUG": "1",
                 "5BUTUG": "1",
                 "6BUTUG": "1",
             }
             ind1 = types.get(self.typ, "")
-            record.emplace_datafield(f"971.{ind1}..a", value=construct_name(self.name))
+            self.theses_local_field.add(
+                f"971.{ind1}..",
+                {"a": construct_name(self.name)},
+            )
 
         self.state = ""
 
-    def visit_FN(self, node: Element, record: Marc21Metadata):
+    def visit_FN(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         self.name["fn"] = node.text
 
-    def visit_LN(self, node: Element, record: Marc21Metadata):
+    def visit_LN(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         self.name["ln"] = node.text
 
-    def visit_FNLN(self, node: Element, record: Marc21Metadata):
+    def visit_FNLN(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_AKK(self, node: Element, record: Marc21Metadata):
+    def visit_AKK(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_MNR(self, node: Element, record: Marc21Metadata):
+    def visit_MNR(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_STRI(self, node: Element, record: Marc21Metadata):
+    def visit_STRI(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_STKZ(self, node: Element, record: Marc21Metadata):
+    def visit_STKZ(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_ORIG(self, node: Element, record: Marc21Metadata):
+    def visit_ORIG(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_INTERN(self, node: Element, record: Marc21Metadata):
+    def visit_INTERN(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
 
-    def visit_TIT(self, node: Element, record: Marc21Metadata):
+    def visit_TIT(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
+        text = node.text.replace("\n", " ")
+        author = f"{self.author_name['fn']} {self.author_name['ln']}"
+
         if self.state == "metaobj" and self.language == self.object_language:
-            record.emplace_datafield(
-                "245.1.0.",
-                subfs={"a": node.text, "c": f"{self.name.fn} {self.name.ln}"},
-            )
+            record.emplace_datafield("245.1.0.", subfs={"a": text, "c": author})
 
         if self.state == "metaobj" and self.language != self.object_language:
-            record.emplace_datafield(
-                "246.1..", subfs={"i": "TUGRAZonline", "a": node.text}
-            )
+            record.emplace_datafield("246.1..", subfs={"i": "TUGRAZonline", "a": text})
 
-    def visit_ABS(self, node: Element, record: Marc21Metadata):
+    def visit_ABS(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
         record.emplace_datafield("520...", value=node.text)
 
-    def visit_KEYW(self, node: Element, record: Marc21Metadata):
+    def visit_KEYW(self, node: Element, record: Marc21Metadata) -> None:
         """Visit ."""
-        if not node:
+        text = node.text
+        if not text:
             return
 
         subjects = filter(
             lambda s: len(s) > 0,
-            [s.strip() for s in split(r";|,", node.text)],
+            [s.strip() for s in split(r";|,", text)],
         )
+
         for subject in subjects:
             record.emplace_datafield("653...", value=subject)
 
-    def visit_LANG(self, node: Element, record: Marc21Metadata):
+    def visit_LANG(self, node: Element, _: Marc21Metadata) -> None:
         """Visit ."""
         self.language = node.text
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/decorators.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,53 +5,57 @@
 # invenio-workflows-tugraz is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 
 """Decorator functions for theses views."""
 
+from collections.abc import Callable
 from functools import wraps
+from typing import Any
 
 from flask import abort, g
 from invenio_records_marc21.proxies import current_records_marc21
 from invenio_search import RecordsSearch
 from invenio_search.engine import dsl
 from sqlalchemy.exc import NoResultFound
 
 
-def pass_record_from_pid(f):
+def pass_record_from_pid(f: Callable) -> Callable:
     """Decorate a view to pass the record from a pid."""
 
     @wraps(f)
-    def view(*args, **kwargs):
+    def view(*_: dict, **kwargs: dict) -> Any:  # noqa: ANN401
         pid_value = kwargs.get("pid_value")
 
         search = RecordsSearch(index="marc21records")
         query = {
             "filter": [
                 {"match_all": {}},
                 {"match_phrase": {"metadata.fields.995.subfields.d": pid_value}},
                 {"match_phrase": {"metadata.fields.995.subfields.i": "TUGRAZonline"}},
-            ]
+            ],
         }
 
         search.query = dsl.Q("bool", **query)
         search = search.params(size=1)
         result = search.execute()
         if len(result["hits"]["hits"]) == 0:
             abort(404)
         hits = result["hits"]["hits"][0]["_source"]
         hits = hits.to_dict()
 
         try:
             record = current_records_marc21.records_service.read_draft(
-                id_=hits["id"], identity=g.identity
+                id_=hits["id"],
+                identity=g.identity,
             )
-        except NoResultFound as e:
+        except NoResultFound:
             record = current_records_marc21.records_service.read(
-                id_=hits["id"], identity=g.identity
+                id_=hits["id"],
+                identity=g.identity,
             )
 
         kwargs["record"] = record.to_dict()
         return f(**kwargs)
 
     return view
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz/theses/views.py` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz/theses/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # Invenio-Records-Marc21 is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 
 """Blueprint definitions."""
 
-from flask import Blueprint, redirect
+from flask import Blueprint, Flask, redirect
+from werkzeug.wrappers import Response as BaseResponse
 
 from .decorators import pass_record_from_pid
 
 
 @pass_record_from_pid
-def record_from_pid(record=None, **kwargs):
+def record_from_pid(record: dict = None, **__: dict) -> BaseResponse:
     """Redirect to record's latest version page."""
     return redirect(record["links"]["self_html"], code=301)
 
 
-def create_blueprint(app):
+def create_blueprint(_: Flask) -> Blueprint:
     """Register blueprint routes on app."""
     blueprint = Blueprint(
         "invenio_workflows_tugraz_theses",
         __name__,
         url_prefix="/theses",
     )
```

### Comparing `invenio-workflows-tugraz-0.1.9/invenio_workflows_tugraz.egg-info/SOURCES.txt` & `invenio-workflows-tugraz-0.2.0/invenio_workflows_tugraz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .dockerignore
 .editorconfig
+.ruff.toml
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `invenio-workflows-tugraz-0.1.9/setup.cfg` & `invenio-workflows-tugraz-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = invenio-workflows-tugraz
 version = attr: invenio_workflows_tugraz.__version__
-description = "This package serves as a place for the workflows of the repository of the TU Graz."
+description = "Package serves as a place for the workflows of the repository of the TU Graz."
 long_description = file: README.rst, CHANGES.rst
 keywords = invenio workflows TUGraz
 license = MIT
 author = Graz University of Technology
 author_email = info@tugraz.at
 platforms = any
 url = https://github.com/tu-graz-library/invenio-workflows-tugraz
@@ -26,14 +26,15 @@
 tests = 
 	pytest-black>=0.3.0
 	pytest-invenio>=1.4.0
 	invenio-search[opensearch2]>=2.1.0
 	invenio-alma>=0.7.1
 	invenio-campusonline>=0.1.1
 	invenio-pure>=0.1.1
+	ruff>=0.0.263
 	sphinx>=4.5
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_workflows_tugraz = invenio_workflows_tugraz:InvenioWorkflowsTugraz
 invenio_base.blueprints = 
 	invenio_workflows_tugraz_theses = invenio_workflows_tugraz.theses:create_blueprint
@@ -44,25 +45,22 @@
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
-[pydocstyle]
-add_ignore = D401
-
 [isort]
 profile = black
 
 [check-manifest]
 ignore = 
 	*-requirements.txt
 
 [tool:pytest]
-addopts = --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=invenio_workflows_tugraz --cov-report=term-missing
+addopts = --black --doctest-glob="*.rst" --doctest-modules --cov=invenio_workflows_tugraz --cov-report=term-missing
 testpaths = docs tests invenio_workflows_tugraz
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `invenio-workflows-tugraz-0.1.9/tests/conftest.py` & `invenio-workflows-tugraz-0.2.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,33 +9,26 @@
 """Pytest configuration.
 
 See https://pytest-invenio.readthedocs.io/ for documentation on which test
 fixtures are available.
 """
 
 
+from collections.abc import Callable
+
 import pytest
 from flask import Flask
 
 from invenio_workflows_tugraz import InvenioWorkflowsTugraz
 
 
 @pytest.fixture(scope="module")
-def celery_config():
-    """Override pytest-invenio fixture.
-
-    TODO: Remove this fixture if you add Celery support.
-    """
-    return {}
-
-
-@pytest.fixture(scope="module")
-def create_app(instance_path):
+def create_app(instance_path: str) -> Callable:
     """Application factory fixture."""
 
-    def factory(**config):
+    def factory(**config: dict) -> Flask:
         app = Flask("testapp", instance_path=instance_path)
         app.config.update(**config)
         InvenioWorkflowsTugraz(app)
         return app
 
     return factory
```

### Comparing `invenio-workflows-tugraz-0.1.9/tests/test_invenio_workflows_tugraz.py` & `invenio-workflows-tugraz-0.2.0/tests/test_invenio_workflows_tugraz.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Module tests."""
 
 from flask import Flask
 
-from invenio_workflows_tugraz import InvenioWorkflowsTugraz
+from invenio_workflows_tugraz import InvenioWorkflowsTugraz, __version__
 
 
-def test_version():
+def test_version() -> None:
     """Test version import."""
-    from invenio_workflows_tugraz import __version__
-
     assert __version__
 
 
-def test_init():
+def test_init() -> None:
     """Test extension initialization."""
     app = Flask("testapp")
     ext = InvenioWorkflowsTugraz(app)
     assert "invenio-workflows-tugraz" in app.extensions
 
     app = Flask("testapp")
     ext = InvenioWorkflowsTugraz()
```


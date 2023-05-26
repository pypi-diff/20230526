# Comparing `tmp/invenio-alma-0.8.2.tar.gz` & `tmp/invenio-alma-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-alma-0.8.2.tar", last modified: Mon May  1 09:39:37 2023, max compression
+gzip compressed data, was "invenio-alma-0.9.0.tar", last modified: Fri May 26 09:10:31 2023, max compression
```

## Comparing `invenio-alma-0.8.2.tar` & `invenio-alma-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.072981 invenio-alma-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/click_param_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma/services/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/invenio_alma/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/invenio_alma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 09:39:37.000000 invenio-alma-0.8.2/invenio_alma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:39:37.076981 invenio-alma-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/test_invenio_alma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-01 09:39:29.000000 invenio-alma-0.8.2/tests/test_invenio_alma_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/click_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/invenio_alma/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/invenio_alma/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.772546 invenio-alma-0.9.0/invenio_alma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 09:10:31.000000 invenio-alma-0.9.0/invenio_alma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:10:31.776546 invenio-alma-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/test_invenio_alma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 09:10:22.000000 invenio-alma-0.9.0/tests/test_invenio_alma_service.py
```

### Comparing `invenio-alma-0.8.2/.editorconfig` & `invenio-alma-0.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/CHANGES.rst` & `invenio-alma-0.9.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-05-26)
+
+- ruff: add to ignore
+- cli: make update func customizable
+
+
 Version v0.8.2 (release 2023-05-01)
 
 - ext: revert last change
 
 
 Version v0.8.1 (release 2023-05-01)
```

### Comparing `invenio-alma-0.8.2/CONTRIBUTING.rst` & `invenio-alma-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/LICENSE` & `invenio-alma-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/MANIFEST.in` & `invenio-alma-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/PKG-INFO` & `invenio-alma-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.2
+Version: 0.9.0
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-05-26)
+
+- ruff: add to ignore
+- cli: make update func customizable
+
+
 Version v0.8.2 (release 2023-05-01)
 
 - ext: revert last change
 
 
 Version v0.8.1 (release 2023-05-01)
```

### Comparing `invenio-alma-0.8.2/README.rst` & `invenio-alma-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/docs/Makefile` & `invenio-alma-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/docs/conf.py` & `invenio-alma-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
 from invenio_alma import __version__
@@ -13,14 +13,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 nitpick_ignore = [
     ("py:class", "Flask"),
     ("py:class", "flask.blueprints.Blueprint"),
+    ("py:class", "flask.app.Flask"),
     ("py:class", "invenio_alma.resources.resources.AlmaResource"),
     ("py:class", "invenio_alma.services.rest.AlmaRESTService"),
     ("py:class", "AlmaResource"),
     ("py:class", "AlmaResourceMock"),
 ]
```

### Comparing `invenio-alma-0.8.2/docs/index.rst` & `invenio-alma-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/docs/make.bat` & `invenio-alma-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/api.py` & `invenio-alma-0.9.0/invenio_alma/api.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/cli.py` & `invenio-alma-0.9.0/invenio_alma/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Command line interface to interact with the Alma-Connector module."""
 
 import click
 from click_option_group import RequiredMutuallyExclusiveOptionGroup, optgroup
+from flask import current_app
 from flask.cli import with_appcontext
 from invenio_config_tugraz import get_identity_from_user_by_email
 
 from .api import (
     create_alma_record,
     import_list_of_records,
     import_record,
     update_repository_record,
 )
 from .click_param_type import CSV
 from .proxies import current_alma
 from .services import AlmaSRUService
+from .services.config import AlmaRESTConfig, AlmaSRUConfig
 from .utils import preliminaries
 
 
 @click.group()
 def alma() -> None:
     """Alma CLI."""
 
@@ -111,51 +113,70 @@
     """Alma update group."""
 
 
 @update.command("repository-record")
 @with_appcontext
 @click.option("--marc-id", type=click.STRING, required=True)
 @click.option("--user-email", type=click.STRING, default="alma@tugraz.at")
-@click.option("--api-key", type=click.STRING, required=True)
+@optgroup.group("Alma REST config")
+@optgroup.option("--api-key", type=click.STRING)
+@optgroup.option("--api-host", type=click.STRING)
+@optgroup.group("Alma SRU config")
+@optgroup.option("--search-key", type=click.STRING)
+@optgroup.option("--domain", type=click.STRING)
+@optgroup.option("--institution-code", type=click.STRING)
 @optgroup.group("Alma identifier", cls=RequiredMutuallyExclusiveOptionGroup)
 @optgroup.option("--mms-id", type=click.STRING, help="mms-id", default=None)
 @optgroup.option("--thesis-id", type=click.STRING, help="thesis-id", default=None)
 def cli_update_repository_record(
     marc_id: str,
     user_email: str,
     api_key: str,
+    api_host: str,
+    search_key: str,
+    domain: str,
+    institution_code: str,
     mms_id: str,
     thesis_id: str,
 ) -> None:
     """Update Repository record."""
+    use_rest = False
+    use_sru = False
+
     if mms_id:
         use_rest = True
         alma_thesis_id = mms_id
+        config = AlmaRESTConfig(api_key, api_host)
     elif thesis_id:
         use_sru = True
         alma_thesis_id = thesis_id
+        config = AlmaSRUConfig(search_key, domain, institution_code)
     else:
         msg = "Neither of mms_id and thesis_id were given."
         raise RuntimeError(msg)
 
+    update_func = current_app.config.get("ALMA_REPOSITORY_RECORDS_UPDATE_FUNC", None)
+
     records_service, alma_service, identity = preliminaries(
         user_email,
+        config,
         use_rest=use_rest,
         use_sru=use_sru,
     )
 
-    alma_service.config.api_key = api_key
-
-    update_repository_record(
-        records_service,
-        alma_service,
-        marc_id,
-        identity,
-        alma_thesis_id,
-    )
+    if update_func:
+        update_func(records_service, alma_service, marc_id, thesis_id, identity)
+    else:
+        update_repository_record(
+            records_service,
+            alma_service,
+            marc_id,
+            identity,
+            alma_thesis_id,
+        )
 
 
 @update.command("url-in-alma")
 @with_appcontext
 @click.option(
     "--csv-file",
     type=CSV(header="mms_id,new_url"),
```

### Comparing `invenio-alma-0.8.2/invenio_alma/click_param_type.py` & `invenio-alma-0.9.0/invenio_alma/click_param_type.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/config.py` & `invenio-alma-0.9.0/invenio_alma/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/ext.py` & `invenio-alma-0.9.0/invenio_alma/ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to connect InvenioRDM to Alma."""
 
 from __future__ import annotations
 
-import typing as t
-
-if t.TYPE_CHECKING:
-    from flask import Flask
-
 from dataclasses import dataclass
 
-from flask import Blueprint, current_app
+from flask import Blueprint, Flask, current_app
 
 from .resources import AlmaResource, AlmaResourceConfig
 from .services import AlmaRESTService, AlmaSRUService
+from .services.config import AlmaRESTConfig, AlmaSRUConfig
 
 
 @dataclass(frozen=True)
 class AlmaResourceMock:
     """Alma Resource Mock class. It is used if the alma resource is not initialized."""
 
     def as_blueprint(self) -> Blueprint:
@@ -43,15 +39,16 @@
             self.init_app(app)
 
     @property
     def alma_rest_service(self) -> AlmaRESTService:
         """Return the alma rest service."""
         if not self._alma_rest_service:
             current_app.logger.warn("AlmaRESTService was not initialized correctly.")
-            return AlmaRESTService.build("", "")
+            config = AlmaRESTConfig("", "")
+            return AlmaRESTService.build(config)
 
         return self._alma_rest_service
 
     @property
     def alma_resource(self) -> AlmaResource | AlmaResourceMock:
         """Return the alma resource."""
         if not self._alma_resource:
@@ -66,20 +63,22 @@
         self.init_resources(app)
         app.extensions["invenio-alma"] = self
 
     def init_services(self, app: Flask) -> None:
         """Initialize service."""
         api_key = app.config.get("ALMA_API_KEY", "")
         api_host = app.config.get("ALMA_API_HOST", "")
+        config = AlmaRESTConfig(api_key, api_host)
 
-        self._alma_rest_service = AlmaRESTService.build(api_key, api_host)
+        self._alma_rest_service = AlmaRESTService.build(config)
 
     def init_resources(self, app: Flask) -> None:
         """Initialize resources."""
         search_key = "local_control_field_009"  # ac_number
         domain = app.config.get("ALMA_SRU_DOMAIN")
         institution_code = app.config.get("ALMA_SRU_INSTITUTION_CODE")
+        config = AlmaSRUConfig(search_key, domain, institution_code)
 
         self._alma_resource = AlmaResource(
-            service=AlmaSRUService.build(search_key, domain, institution_code),
+            service=AlmaSRUService.build(config),
             config=AlmaResourceConfig,
         )
```

### Comparing `invenio-alma-0.8.2/invenio_alma/resources/config.py` & `invenio-alma-0.9.0/invenio_alma/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/resources/resources.py` & `invenio-alma-0.9.0/invenio_alma/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/services/base.py` & `invenio-alma-0.9.0/invenio_alma/services/base.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/services/config.py` & `invenio-alma-0.9.0/invenio_alma/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/services/errors.py` & `invenio-alma-0.9.0/invenio_alma/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/services/rest.py` & `invenio-alma-0.9.0/invenio_alma/services/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,24 +119,19 @@
         self.config = config
         self.urls = urls
         self.service = service
 
     @classmethod
     def build(  # noqa: ANN206
         cls,
-        api_key: str,
-        api_host: str,
-        config: AlmaRESTConfig = None,
-        urls: AlmaRESTUrls = None,
-        service: AlmaREST = None,
+        config: AlmaRESTConfig,
     ):  # -> Self >=python3.11 necessary
         """Build method."""
-        config = config if config else AlmaRESTConfig(api_key, api_host)
-        urls = urls if urls else AlmaRESTUrls(config)
-        service = service if service else AlmaREST()
+        urls = AlmaRESTUrls(config)
+        service = AlmaREST()
         return cls(config, urls, service)
 
     def get_record(self, mms_id: str) -> list[Element]:
         """Get Record from alma."""
         api_url = self.urls.url_get(mms_id)
         return self.service.get(api_url)  # return etree
```

### Comparing `invenio-alma-0.8.2/invenio_alma/services/sru.py` & `invenio-alma-0.9.0/invenio_alma/services/sru.py`

 * *Files 26% similar despite different names*

```diff
@@ -70,26 +70,18 @@
         self.config = config
         self.urls = urls
         self.service = service
 
     @classmethod
     def build(  # noqa: ANN206
         cls,
-        search_key: str,
-        domain: str,
-        institution_code: str,
-        config: AlmaSRUConfig = None,
-        urls: AlmaSRUUrls = None,
-        service: AlmaSRU = None,
+        config: AlmaSRUConfig,
     ):
         """Build sru service."""
-        config = (
-            config if config else AlmaSRUConfig(search_key, domain, institution_code)
-        )
-        urls = urls if urls else AlmaSRUUrls(config)
-        service = service if service else AlmaSRU()
+        urls = AlmaSRUUrls(config)
+        service = AlmaSRU()
         return cls(config, urls, service)
 
     def get_record(self, ac_number: str, search_key: str = None) -> list[Element]:
         """Get the record."""
         url = self.urls.url(ac_number, search_key)
         return self.service.get(url)
```

### Comparing `invenio-alma-0.8.2/invenio_alma/tasks.py` & `invenio-alma-0.9.0/invenio_alma/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma/utils.py` & `invenio-alma-0.9.0/invenio_alma/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021-2022 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-alma is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Utils."""
 
 from __future__ import annotations
 
 import functools
-import typing as t
+from collections.abc import Callable
 
 from flask import current_app
 from invenio_config_tugraz import get_identity_from_user_by_email
 from invenio_records_marc21 import current_records_marc21
 
-from .proxies import current_alma
+from .services import AlmaRESTService, AlmaSRUService
+from .services.config import AlmaRESTConfig, AlmaSRUConfig
 from .services.errors import AlmaAPIError
-from .services.sru import AlmaSRUService
-
-if t.TYPE_CHECKING:
-    from collections.abc import Callable
 
 
 def is_duplicate_in_alma(cms_id: str) -> None:
     """Check if there is already a record in alma."""
     search_key = "local_field_995"
     domain = current_app.config["ALMA_SRU_DOMAIN"]
     institution_code = current_app.config["ALMA_SRU_INSTITUTION_CODE"]
-    sru_service = AlmaSRUService.build(search_key, domain, institution_code)
+    config = AlmaSRUConfig(search_key, domain, institution_code)
+    sru_service = AlmaSRUService.build(config)
 
     try:
         record = sru_service.get_record(cms_id)
         return len(record) > 0
     except AlmaAPIError:
         return False
 
 
 def preliminaries(
     user_email: str,
+    config: AlmaRESTConfig | AlmaSRUConfig = None,
     *,
     use_rest: bool = False,
     use_sru: bool = False,
 ) -> tuple:
     """Preliminaries to interact with the repository."""
     records_service = current_records_marc21.records_service
+
     if use_rest:
-        alma_service = current_alma.alma_rest_service
+        alma_service = AlmaRESTService.build(config)
     elif use_sru:
-        search_key = "local_field_995"
-        domain = current_app.config["ALMA_SRU_DOMAIN"]
-        institution_code = current_app.config["ALMA_SRU_INSTITUTION_CODE"]
-        alma_service = AlmaSRUService(search_key, domain, institution_code)
+        alma_service = AlmaSRUService.build(config)
     else:
         msg = "choose between using rest or sru."
         raise RuntimeError(msg)
 
     identity = get_identity_from_user_by_email(email=user_email)
 
     return records_service, alma_service, identity
```

### Comparing `invenio-alma-0.8.2/invenio_alma/views.py` & `invenio-alma-0.9.0/invenio_alma/views.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/invenio_alma.egg-info/PKG-INFO` & `invenio-alma-0.9.0/invenio_alma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-alma
-Version: 0.8.2
+Version: 0.9.0
 Summary: "Provides API for Alma."
 Home-page: https://github.com/tu-graz-library/invenio-alma
 Author: Graz University of Technology.
 Author-email: info@inveniosoftware.org
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
 
     invenio-alma is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-05-26)
+
+- ruff: add to ignore
+- cli: make update func customizable
+
+
 Version v0.8.2 (release 2023-05-01)
 
 - ext: revert last change
 
 
 Version v0.8.1 (release 2023-05-01)
```

### Comparing `invenio-alma-0.8.2/invenio_alma.egg-info/SOURCES.txt` & `invenio-alma-0.9.0/invenio_alma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/run-tests.sh` & `invenio-alma-0.9.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/setup.cfg` & `invenio-alma-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/tests/conftest.py` & `invenio-alma-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/tests/test_invenio_alma.py` & `invenio-alma-0.9.0/tests/test_invenio_alma.py`

 * *Files identical despite different names*

### Comparing `invenio-alma-0.8.2/tests/test_invenio_alma_service.py` & `invenio-alma-0.9.0/tests/test_invenio_alma_service.py`

 * *Files identical despite different names*


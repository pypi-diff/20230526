# Comparing `tmp/invenio-config-tuw-2023.2.2.tar.gz` & `tmp/invenio-config-tuw-2023.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.2.tar", last modified: Wed May 17 17:46:27 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.3.tar", last modified: Fri May 26 10:08:54 2023, max compression
```

## Comparing `invenio-config-tuw-2023.2.2.tar` & `invenio-config-tuw-2023.2.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.695176 invenio-config-tuw-2023.2.2/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.675175 invenio-config-tuw-2023.2.2/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2363 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.2/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5300 2023-05-17 17:46:27.695176 invenio-config-tuw-2023.2.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.2/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.683175 invenio-config-tuw-2023.2.2/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.687176 invenio-config-tuw-2023.2.2/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.691176 invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7840 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1104 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.691176 invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.691176 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5300 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-05-17 17:46:27.000000 invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-05-17 17:46:27.695176 invenio-config-tuw-2023.2.2/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.2/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-17 17:46:27.695176 invenio-config-tuw-2023.2.2/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.2/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.610253 invenio-config-tuw-2023.2.3/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2428 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5365 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.618253 invenio-config-tuw-2023.2.3/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7792 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1162 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5365 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.2/.editorconfig` & `invenio-config-tuw-2023.2.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/.tx/config` & `invenio-config-tuw-2023.2.3/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/CHANGES.rst` & `invenio-config-tuw-2023.2.3/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-04-27)
+Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
+- Add a null check for the current_user in the logging formatter
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.2/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/LICENSE` & `invenio-config-tuw-2023.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/MANIFEST.in` & `invenio-config-tuw-2023.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/PKG-INFO` & `invenio-config-tuw-2023.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.2
+Version: 2023.2.3
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,19 +94,20 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-04-27)
+Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
+- Add a null check for the current_user in the logging formatter
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.2/README.rst` & `invenio-config-tuw-2023.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/babel.ini` & `invenio-config-tuw-2023.2.3/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/docs/Makefile` & `invenio-config-tuw-2023.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/docs/conf.py` & `invenio-config-tuw-2023.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/docs/index.rst` & `invenio-config-tuw-2023.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/docs/make.bat` & `invenio-config-tuw-2023.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         }
     ],
     "publisher": "TU Wien",
     "resource_type": {
         "id": "dataset",
     },
     "version": "1.0.0",
-    "description": "<h2>A primer on your dataset's description (to be edited)</h2><p>The influence of proper documentation on the reusability for research data should not be underestimated!<br>In order to help others understand how to interpret and reuse your data, we provide you with a few questions to help you structure your dataset's description (though please don't feel obligated to stick to them):</p><h3>Context and methodology</h3><ul><li>What is the research domain or project in which this dataset was created?</li><li>Which purpose does this dataset serve?</li><li>How was this dataset created?</li></ul><h3>Technical details</h3><ul><li>What is the structure of this dataset? Do the folders and files follow a certain naming convention?</li><li>Is any specific software required to open and work with this dataset? Does it only work on certain operating systems?</li><li>Are there any additional resources available regarding the dataset, e.g. documentation, source code, etc.?</li></ul><h3>Further details</h3><ul><li>Is there anything else that other people may need to know when they want to reuse the dataset?</li></ul>",
+    "description": "<h2>A primer on your dataset's description (to be edited)</h2><p>The influence of proper documentation on the reusability for research data should not be underestimated!<br>In order to help others understand how to interpret and reuse your data, we provide you with a few questions to help you structure your dataset's description (though please don't feel obligated to stick to them):</p><h3>Context and methodology</h3><ul><li>What is the research domain or project in which this dataset was created?</li><li>Which purpose does this dataset serve?</li><li>How was this dataset created?</li></ul><h3>Technical details</h3><ul><li>What is the structure of this dataset? Do the folders and files follow a certain naming convention?</li><li>Is any specific software required to open and work with this dataset?</li><li>Are there any additional resources available regarding the dataset, e.g. documentation, source code, etc.?</li></ul><h3>Further details</h3><ul><li>Is there anything else that other people may need to know when they want to reuse the dataset?</li></ul>",
 }
 
 RDM_CITATION_STYLES = [
     ("apa", _("APA")),
     ("bibtex", _("BibTeX")),
     ("ieee", _("IEEE")),
 ]
```

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/formatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,14 @@
 class CustomFormatter(Formatter):
     """Custom logging formatter that provides more details."""
 
     def __init__(self, fmt=custom_format, **kwargs):
         super(CustomFormatter, self).__init__(fmt=fmt, **kwargs)
 
     def format(self, record):
-        record.user_id = (
-            current_user.id if current_user.is_authenticated else "Anonymous"
-        )
+        user_id = "Anonymous"
+        if current_user is not None and current_user.is_authenticated:
+            user_id = current_user.id
+
+        record.user_id = user_id
         record.request_url = request.base_url
         return super(CustomFormatter, self).format(record)
```

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.3/invenio_config_tuw/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.2
+Version: 2023.2.3
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,19 +94,20 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-04-27)
+Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
+- Add a null check for the current_user in the logging formatter
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.2/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/setup.cfg` & `invenio-config-tuw-2023.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/tests/conftest.py` & `invenio-config-tuw-2023.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.2/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.3/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*


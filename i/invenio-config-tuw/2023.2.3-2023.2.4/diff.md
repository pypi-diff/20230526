# Comparing `tmp/invenio-config-tuw-2023.2.3.tar.gz` & `tmp/invenio-config-tuw-2023.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.3.tar", last modified: Fri May 26 10:08:54 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.4.tar", last modified: Fri May 26 12:35:41 2023, max compression
```

## Comparing `invenio-config-tuw-2023.2.3.tar` & `invenio-config-tuw-2023.2.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.610253 invenio-config-tuw-2023.2.3/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2428 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5365 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.618253 invenio-config-tuw-2023.2.3/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7792 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1162 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.622253 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5365 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-05-26 10:08:54.000000 invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.3/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 10:08:54.626253 invenio-config-tuw-2023.2.3/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.3/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.823966 invenio-config-tuw-2023.2.4/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2505 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5442 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.827966 invenio-config-tuw-2023.2.4/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.831966 invenio-config-tuw-2023.2.4/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.835966 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7792 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.835966 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.831966 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5442 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.3/.editorconfig` & `invenio-config-tuw-2023.2.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/.tx/config` & `invenio-config-tuw-2023.2.4/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/CHANGES.rst` & `invenio-config-tuw-2023.2.4/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
+- Prevent the logging formatter from blowing up outside of a request context
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.3/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/LICENSE` & `invenio-config-tuw-2023.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/MANIFEST.in` & `invenio-config-tuw-2023.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/PKG-INFO` & `invenio-config-tuw-2023.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.3
+Version: 2023.2.4
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -100,14 +100,15 @@
 
 Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
+- Prevent the logging formatter from blowing up outside of a request context
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.3/README.rst` & `invenio-config-tuw-2023.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/babel.ini` & `invenio-config-tuw-2023.2.4/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/docs/Makefile` & `invenio-config-tuw-2023.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/docs/conf.py` & `invenio-config-tuw-2023.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/docs/index.rst` & `invenio-config-tuw-2023.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/docs/make.bat` & `invenio-config-tuw-2023.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/formatters.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,17 +28,24 @@
 """
 
 
 class CustomFormatter(Formatter):
     """Custom logging formatter that provides more details."""
 
     def __init__(self, fmt=custom_format, **kwargs):
-        super(CustomFormatter, self).__init__(fmt=fmt, **kwargs)
+        super().__init__(fmt=fmt, **kwargs)
 
     def format(self, record):
-        user_id = "Anonymous"
-        if current_user is not None and current_user.is_authenticated:
-            user_id = current_user.id
+        try:
+            user_id = "Anonymous"
+            if current_user and current_user.is_authenticated:
+                user_id = current_user.id
+
+            record.user_id = user_id
+            record.request_url = request.base_url
+
+        except RuntimeError:
+            # this happens when we're working outside a request context
+            record.user_id = None
+            record.request_url = None
 
-        record.user_id = user_id
-        record.request_url = request.base_url
         return super(CustomFormatter, self).format(record)
```

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.4/invenio_config_tuw/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.3
+Version: 2023.2.4
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -100,14 +100,15 @@
 
 Version 2023.2 (released 2023-04-24, updated 2023-05-26)
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
+- Prevent the logging formatter from blowing up outside of a request context
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.3/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/setup.cfg` & `invenio-config-tuw-2023.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/tests/conftest.py` & `invenio-config-tuw-2023.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.3/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.4/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*


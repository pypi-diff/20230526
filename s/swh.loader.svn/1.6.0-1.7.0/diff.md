# Comparing `tmp/swh.loader.svn-1.6.0.tar.gz` & `tmp/swh.loader.svn-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.svn-1.6.0.tar", last modified: Mon Mar  6 13:05:01 2023, max compression
+gzip compressed data, was "dist/swh.loader.svn-1.7.0.tar", last modified: Fri May 26 14:57:02 2023, max compression
```

## Comparing `swh.loader.svn-1.6.0.tar` & `swh.loader.svn-1.7.0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      130 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1755 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      827 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/bin/init-svn-repository.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/bin/swh-svn
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/docs/swh-loader-svn.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/install/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/install/install-pysvn.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/install/install-subvertpy.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/resources/svn.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2330 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/setup.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/svn-lib-client-analysis.org
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh/loader/svn/
--rw-r--r--   0 jenkins    (115) docker     (999)      491 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)    34162 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)    32566 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/replay.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23892 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1511 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2459 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/httthttt.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
--rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    56688 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_externals.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_loader.org
--rw-r--r--   0 jenkins    (115) docker     (999)    78976 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3260 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2471 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_task.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20617 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/tests/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15926 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/swh/loader/svn/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1755 2023-03-06 13:05:00.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2254 2023-03-06 13:05:01.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-06 13:05:00.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-03-06 13:05:00.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-03-06 13:05:00.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-06 13:05:00.000000 swh.loader.svn-1.6.0/swh.loader.svn.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-03-06 13:04:59.000000 swh.loader.svn-1.6.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1922 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      994 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/bin/init-svn-repository.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/bin/swh-svn
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/swh-loader-svn.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/install/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/install/install-pysvn.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/install/install-subvertpy.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/resources/svn.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     5522 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/setup.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/svn-lib-client-analysis.org
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/
+-rw-r--r--   0 jenkins    (115) docker     (999)      491 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9055 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.cpp
+-rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.pyi
+-rw-r--r--   0 jenkins    (115) docker     (999)    34162 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)    33820 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/replay.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    23534 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1511 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2459 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/httthttt.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    62193 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_externals.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2371 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_fast_crawler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.org
+-rw-r--r--   0 jenkins    (115) docker     (999)    79106 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3260 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2471 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    21336 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15984 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1922 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2360 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/tox.ini
```

### Comparing `swh.loader.svn-1.6.0/.pre-commit-config.yaml` & `swh.loader.svn-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/CODE_OF_CONDUCT.md` & `swh.loader.svn-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/LICENSE` & `swh.loader.svn-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/PKG-INFO` & `swh.loader.svn-1.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.6.0
+Version: 1.7.0
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -16,42 +16,41 @@
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS
 
-swh-loader-svn
-==============
+# swh-loader-svn [![Build Status](https://jenkins.softwareheritage.org/job/DLDSVN/job/master/badge/icon)](https://jenkins.softwareheritage.org/job/DLDSVN/job/master/)
 
-The Software Heritage SVN Loader is a tool and a library to walk a remote svn repository
-and inject into the SWH dataset all contained files that weren't known before.
+The Software Heritage Subversion loader is a tool and a library to walk a remote svn
+repository and inject into the Software Heritage archive all contained files, directories
+and commits that weren't known before.
 
 The main entry points are
 
-- :class:`swh.loader.svn.loader.SvnLoader` for the main svn loader which ingests content out of
+- `swh.loader.svn.loader.SvnLoader` for the main svn loader which ingests content out of
   a remote svn repository
 
-- :class:`swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
+- `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
-- :class:`swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
+- `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
-# CLI run
+## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
-```
+```yml
 storage:
   cls: remote
   args:
     url: http://localhost:5002/
 ```
 
 Run:
 
-```
-swh loader --config-file /tmp/loader_svn.yml \
-    run svn <svn-repository-url>
+```shell
+$ swh loader --config-file /tmp/loader_svn.yml run svn <svn-repository-url>
 ```
```

### Comparing `swh.loader.svn-1.6.0/bin/init-svn-repository.sh` & `swh.loader.svn-1.7.0/bin/init-svn-repository.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/bin/swh-svn` & `swh.loader.svn-1.7.0/bin/swh-svn`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/conftest.py` & `swh.loader.svn-1.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/docs/swh-loader-svn.txt` & `swh.loader.svn-1.7.0/docs/swh-loader-svn.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/install/install-pysvn.sh` & `swh.loader.svn-1.7.0/install/install-pysvn.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/resources/svn.ini` & `swh.loader.svn-1.7.0/resources/svn.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/svn-lib-client-analysis.org` & `swh.loader.svn-1.7.0/svn-lib-client-analysis.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/converters.py` & `swh.loader.svn-1.7.0/swh/loader/svn/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/exception.py` & `swh.loader.svn-1.7.0/swh/loader/svn/exception.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/loader.py` & `swh.loader.svn-1.7.0/swh/loader/svn/loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/replay.py` & `swh.loader.svn-1.7.0/swh/loader/svn/replay.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 
 from __future__ import annotations
 
 import codecs
 from collections import defaultdict
-from copy import copy
+from copy import copy, deepcopy
 from dataclasses import dataclass, field
 from distutils.dir_util import copy_tree
 from itertools import chain
 import logging
 import os
 import shutil
 import tempfile
@@ -130,15 +130,16 @@
                 overwrite=True,
             )
 
         # And now compute file's checksums
         self.directory[self.path] = from_disk.Content.from_file(path=self.fullpath)
 
 
-ExternalDefinition = Tuple[str, Optional[int], Optional[int], bool]
+# Tuple[external_url, revision, peg_revision, relative_url, set_at_revision]
+ExternalDefinition = Tuple[str, Optional[int], Optional[int], bool, int]
 
 
 @dataclass
 class DirState:
     """Persists some directory states (eg. externals) across revisions while
     replaying them."""
 
@@ -195,14 +196,15 @@
         Args:
             path: to remove from the current objects.
 
         """
         if path in self.directory:
             entry_removed = self.directory[path]
             del self.directory[path]
+            self.dir_states.pop(path, None)
             fpath = os.path.join(self.rootpath, path)
             if isinstance(entry_removed, from_disk.Directory):
                 shutil.rmtree(fpath)
             else:
                 os.remove(fpath)
 
     def open_directory(self, path: str, *args) -> DirEditor:
@@ -249,19 +251,41 @@
             self.directory[path_bytes] = from_disk.Directory.from_disk(path=fullpath)
 
             assert copyfrom_path is not None
             copyfrom_path_bytes = os.fsencode(copyfrom_path).lstrip(b"/")
             copyfrom_fullpath = os.path.join(self.rootpath, copyfrom_path_bytes)
 
             def _copy_dir_state(path: bytes, copied_path: bytes):
-                self.dir_states[path] = copy(self.dir_states[copied_path])
-                for external_path in self.dir_states[path].externals_paths:
+                copied_dir_state = self.dir_states[copied_path]
+                dir_state = self.dir_states[path] = deepcopy(copied_dir_state)
+                for ext_path, external_defs in copy(dir_state.externals).items():
+                    external_defs_copied = [
+                        copy(external_def)
+                        for external_def in external_defs
+                        # copy external definition only if copyfrom_rev is greater or equal
+                        # to the revision it was set
+                        if copyfrom_rev >= external_def[4]
+                    ]
+                    if external_defs_copied:
+                        dir_state.externals[ext_path] = external_defs_copied
+                    else:
+                        dir_state.externals.pop(ext_path)
+                        external_path_bytes = os.fsencode(ext_path)
+                        for external_path in copy(dir_state.externals_paths):
+                            if (
+                                external_path == external_path_bytes
+                                or external_path.startswith(external_path_bytes + b"/")
+                            ):
+                                dir_state.externals_paths.remove(external_path)
+
+                for external_path in dir_state.externals_paths:
                     self.editor.external_paths[os.path.join(path, external_path)] += 1
 
             _copy_dir_state(path_bytes, copyfrom_path_bytes)
+
             for root, dirs, _ in os.walk(fullpath):
                 for dir in dirs:
                     dir_fullpath = os.path.join(root, dir)
                     copied_dir_fullpath = dir_fullpath.replace(
                         fullpath, copyfrom_fullpath
                     )
                     dir_path = dir_fullpath.replace(self.rootpath, b"").lstrip(b"/")
@@ -337,29 +361,35 @@
             )
             self.externals = defaultdict(list)
             if value is not None:
                 try:
                     # externals are set on that directory path, parse and store them
                     # for later processing in the close method
                     for external in value.split("\n"):
-                        external = external.rstrip("\r")
+                        external = external.strip(" \t\r")
                         # skip empty line or comment
                         if not external or external.startswith("#"):
                             continue
                         (
                             path,
                             external_url,
                             revision,
                             peg_revision,
                             relative_url,
                         ) = parse_external_definition(
                             external, os.fsdecode(self.path), self.svnrepo.origin_url
                         )
                         self.externals[path].append(
-                            (external_url, revision, peg_revision, relative_url)
+                            (
+                                external_url,
+                                revision,
+                                peg_revision,
+                                relative_url,
+                                self.editor.revnum,
+                            )
                         )
                 except ValueError:
                     logger.debug(
                         "Failed to parse external: %s\n"
                         "Externals defined on path %s will not be processed",
                         external,
                         self.path,
@@ -423,40 +453,36 @@
             # externals definition list might have changed in the current replayed
             # revision, we need to determine if some were removed and delete the
             # associated paths
             externals = self.externals
             prev_externals_set = {
                 (path, url, rev, peg_rev)
                 for path in prev_externals.keys()
-                for (url, rev, peg_rev, _) in prev_externals[path]
+                for (url, rev, peg_rev, _, _) in prev_externals[path]
             }
             externals_set = {
                 (path, url, rev, peg_rev)
                 for path in externals.keys()
-                for (url, rev, peg_rev, _) in externals[path]
+                for (url, rev, peg_rev, _, _) in externals[path]
             }
             old_externals = prev_externals_set - externals_set
             for path, _, _, _ in old_externals:
                 self.remove_external_path(os.fsencode(path))
         else:
             # some external paths might have been removed in the current replayed
             # revision by a delete operation on an overlapping versioned path so we
             # need to restore them
             externals = prev_externals
 
         # For each external, try to export it in reconstructed filesystem
         for path, externals_def in externals.items():
             for i, external in enumerate(externals_def):
-                external_url, revision, peg_revision, relative_url = external
                 self.process_external(
                     path,
-                    external_url,
-                    revision,
-                    peg_revision,
-                    relative_url,
+                    external,
                     remove_target_path=i == 0,
                 )
 
         # backup externals in directory state
         if self.externals:
             self.dir_states[self.path].externals = self.externals
 
@@ -472,34 +498,31 @@
                     self.svnrepo.origin_url,
                     os.fsdecode(path),
                     external_path,
                     external_url,
                 )
                 for path, dir_state in self.dir_states.items()
                 for external_path in dir_state.externals.keys()
-                for (external_url, _, _, _) in dir_state.externals[external_path]
+                for (external_url, _, _, _, _) in dir_state.externals[external_path]
             )
             if self.svnrepo.has_recursive_externals:
                 # If the repository has recursive externals, we stop processing
                 # externals and remove those already exported,
                 # We will then ignore externals when exporting the revision to
                 # check for divergence with the reconstructed filesystem.
                 for external_path in list(self.editor.external_paths):
                     self.remove_external_path(external_path, force=True)
 
     def process_external(
         self,
         path: str,
-        external_url: str,
-        revision: Optional[int],
-        peg_revision: Optional[int],
-        relative_url: bool,
+        external: ExternalDefinition,
         remove_target_path: bool = True,
     ) -> None:
-        external = (external_url, revision, peg_revision, relative_url)
+        external_url, revision, peg_revision, relative_url, _ = external
         dest_path = os.fsencode(path)
         dest_fullpath = os.path.join(self.path, dest_path)
         prev_externals = self.dir_states[self.path].externals
         if (
             path in prev_externals
             and external in prev_externals[path]
             and dest_fullpath in self.directory
@@ -518,15 +541,14 @@
             external_url,
             f" at revision {revision}" if revision else "",
             f" and peg revision {peg_revision}" if peg_revision else "",
             dest_fullpath,
         )
 
         if external not in self.editor.externals_cache:
-
             try:
                 # try to export external in a temporary path, destination path could
                 # be versioned and must be overridden only if the external URL is
                 # still valid
                 temp_dir = os.fsencode(
                     tempfile.mkdtemp(dir=self.editor.externals_cache_dir)
                 )
@@ -739,15 +761,15 @@
         self.dir_states: Dict[bytes, DirState] = defaultdict(DirState)
         self.external_paths: Dict[bytes, int] = defaultdict(int)
         self.valid_externals: Dict[bytes, Tuple[str, bool]] = {}
         self.dead_externals: Set[Tuple[str, Optional[int], Optional[int]]] = set()
         self.externals_cache_dir = tempfile.mkdtemp(dir=temp_dir)
         self.externals_cache: Dict[ExternalDefinition, bytes] = {}
         self.svnrepo = svnrepo
-        self.revnum = None
+        self.revnum = -1
         self.debug = debug
 
     def set_target_revision(self, revnum) -> None:
         self.revnum = revnum
 
     def abort(self) -> None:
         pass
```

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/svn_repo.py` & `swh.loader.svn-1.7.0/swh/loader/svn/svn_repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     get_simple_prompt_provider,
     get_username_provider,
 )
 
 from swh.model.from_disk import Directory as DirectoryFromDisk
 from swh.model.model import Content, Directory, SkippedContent
 
-from . import converters, replay
+from . import converters, fast_crawler, replay
 from .svn_retry import svn_retry
 from .utils import is_recursive_external, parse_external_definition
 
 # When log message contains empty data
 DEFAULT_AUTHOR_MESSAGE = b""
 
 logger = logging.getLogger(__name__)
@@ -437,43 +437,37 @@
         # target a dump mounted on the local filesystem
         if self.replay_started and self.has_relative_externals:
             # externals detected while replaying revisions
             url = self.origin_url
         elif not self.replay_started:
             # revisions replay has not started, we need to check if svn:externals
             # properties are set and if some external URLs are relative to pick
-            # the right export URL,recursive externals are also checked
+            # the right export URL, recursive externals are also checked
 
-            # get all svn:externals properties recursively
-            if self.remote_url.startswith("file://"):
-                externals = self.propget(
-                    "svn:externals", self.remote_url, revision, revision, True
-                )
-            else:
-                # recursive propget operation is terribly slow over the network,
-                # better doing it from a freshly checked out working copy as it is faster
-                with tempfile.TemporaryDirectory(
-                    dir=self.local_dirname, prefix=f"checkout-revision-{revision}."
-                ) as co_dirname:
-
-                    self.checkout(
-                        self.remote_url, co_dirname, revision, ignore_externals=True
-                    )
-                    # get all svn:externals properties recursively
-                    externals = self.propget(
-                        "svn:externals", co_dirname, None, None, True
-                    )
+            # recursive propget operation is terribly slow over the network,
+            # so we use a much faster approach relying on a C++ extension module
+            paths = fast_crawler.crawl_repository(
+                self.remote_url,
+                revnum=revision,
+                username=self.username,
+                password=self.password,
+            )
+            externals = {
+                path: path_info["props"]["svn:externals"]
+                for path, path_info in paths.items()
+                if path_info["type"] == "dir" and "svn:externals" in path_info["props"]
+            }
 
             self.has_relative_externals = False
             self.has_recursive_externals = False
             for path, external_defs in externals.items():
                 if self.has_relative_externals or self.has_recursive_externals:
                     break
-                path = path.replace(self.remote_url.rstrip("/") + "/", "")
-                for external_def in os.fsdecode(external_defs).split("\n"):
+                for external_def in external_defs.split("\n"):
+                    external_def = external_def.strip(" \t\r")
                     # skip empty line or comment
                     if not external_def or external_def.startswith("#"):
                         continue
                     (
                         external_path,
                         external_url,
                         _,
```

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/svn_retry.py` & `swh.loader.svn-1.7.0/swh/loader/svn/svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tasks.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/conftest.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/httthttt.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/httthttt.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pkg-gourmet.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_converters.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_externals.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_externals.py`

 * *Files 2% similar despite different names*

```diff
@@ -715,14 +715,15 @@
     check_snapshot(loader.snapshot, loader.storage)
 
     assert (
         external_url,
         None,
         None,
         False,
+        2,
     ) in loader.svnrepo.swhreplay.editor.externals_cache
 
 
 def test_loader_remove_versioned_path_with_external_overlap(
     svn_loader_cls, swh_storage, repo_url, external_repo_url, tmp_path
 ):
     # first commit on external
@@ -1687,40 +1688,76 @@
                 data=b"#!/bin/bash\necho Hello World !",
             ),
         ],
     )
 
     add_commit(
         repo_url,
-        "Create repository structure, one externals directory with svn:externals"
-        "property set and one trunk directory",
+        "Create repository structure, one externals directory and one trunk directory",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="externals/",
+            ),
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/",
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Set svn:externals property on externals directory",
         [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
                 path="externals/",
                 properties={
                     "svn:externals": f'{svn_urljoin(external_repo_url, "code/hello/")} hello'  # noqa
                 },
             ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Add copy of externals directory to trunk from revision 1, svn:externals property"
+        "is not set at that revision so no externals should be exported from the copied path",
+        [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
-                path="trunk/",
+                path="trunk/externals/",
+                copyfrom_path=repo_url + "/externals",
+                copyfrom_rev=1,
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Remove trunk/externals directory.",
+        [
+            CommitChange(
+                change_type=CommitChangeType.Delete,
+                path="trunk/externals/",
             ),
         ],
     )
 
     add_commit(
         repo_url,
-        "Add copy of externals directory to trunk from revision 1.",
+        "Add copy of externals directory to trunk from revision 2 svn:externals property"
+        "is set at that revision so externals should be exported from the copy path",
         [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
                 path="trunk/externals/",
                 copyfrom_path=repo_url + "/externals",
-                copyfrom_rev=1,
+                copyfrom_rev=2,
             ),
         ],
     )
 
     add_commit(
         repo_url,
         "Unset svn:externals property on copied path",
@@ -2037,9 +2074,173 @@
     )
     assert loader.load() == {"status": "eventful"}
     assert_last_visit_matches(
         loader.storage,
         repo_url,
         status="full",
         type="svn",
+    )
+    check_snapshot(loader.snapshot, loader.storage)
+
+
+def test_loader_add_dir_with_externals_then_remove_then_readd_without_externals(
+    svn_loader_cls, swh_storage, repo_url, external_repo_url, tmp_path
+):
+
+    add_commit(
+        external_repo_url,
+        "Add foo/bar path in external",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="foo/bar",
+                data=b"bar",
+            )
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Add directory with externals",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="externals/",
+                properties={"svn:externals": f"{external_repo_url}/foo foo"},
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Remove directory with externals",
+        [
+            CommitChange(
+                change_type=CommitChangeType.Delete,
+                path="externals/",
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Re-add same directory without externals",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="externals/",
+            ),
+        ],
+    )
+
+    loader = svn_loader_cls(
+        swh_storage,
+        repo_url,
+        temp_directory=tmp_path,
+        check_revision=1,
+    )
+    assert loader.load() == {"status": "eventful"}
+    assert_last_visit_matches(
+        loader.storage,
+        repo_url,
+        status="full",
+        type="svn",
+    )
+    check_snapshot(loader.snapshot, loader.storage)
+
+
+def test_loader_quoted_external_definition(
+    svn_loader_cls, swh_storage, repo_url, external_repo_url, tmp_path
+):
+    add_commit(
+        repo_url,
+        "Add file with space in its path",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/foo bar/baz",
+                data=b"baz",
+            ),
+        ],
+    )
+
+    add_commit(
+        repo_url,
+        "Add directory with external targeting 'foo bar' directory with quoted URL",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="externals/",
+                properties={"svn:externals": "^/trunk/foo%20bar foobar"},
+            ),
+        ],
+    )
+
+    loader = svn_loader_cls(
+        swh_storage,
+        repo_url,
+        temp_directory=tmp_path,
+        check_revision=1,
+    )
+    assert loader.load() == {"status": "eventful"}
+    assert_last_visit_matches(
+        loader.storage,
+        repo_url,
+        status="full",
+        type="svn",
+    )
+    check_snapshot(loader.snapshot, loader.storage)
+
+
+def test_loader_with_externals_to_strip(
+    svn_loader_cls, swh_storage, repo_url, external_repo_url, tmp_path
+):
+    # first commit on external
+    add_commit(
+        external_repo_url,
+        "Create some directories and files in an external repository",
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="code/hello/hello-world",
+                properties={"svn:executable": "*"},
+                data=b"#!/bin/bash\necho Hello World !",
+            ),
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="code/bar/bar.sh",
+                properties={"svn:executable": "*"},
+                data=b"#!/bin/bash\necho bar",
+            ),
+        ],
+    )
+
+    # first commit
+    add_commit(
+        repo_url,
+        ("Set svn:externals property on trunk/externals path of repository to load."),
+        [
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path="trunk/externals/",
+                properties={
+                    "svn:externals": (
+                        f"  {svn_urljoin(external_repo_url, 'code/hello')} src/code/hello\t\n"
+                        f"\t{svn_urljoin(external_repo_url, 'code/bar')} src/code/bar   \n"
+                        "\t   \n"
+                    )
+                },
+            ),
+        ],
+    )
+
+    loader = svn_loader_cls(
+        swh_storage, repo_url, temp_directory=tmp_path, check_revision=1, debug=True
+    )
+    assert loader.load() == {"status": "eventful"}
+    assert_last_visit_matches(
+        loader.storage,
+        repo_url,
+        status="full",
+        type="svn",
     )
     check_snapshot(loader.snapshot, loader.storage)
```

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_loader.org` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_loader.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -2236,14 +2236,17 @@
         repo_url,
         status="full",
         type="svn",
     )
 
     check_snapshot(loader.snapshot, loader.storage)
 
+    loader = svn_loader_cls(swh_storage, repo_url, temp_directory=tmp_path)
+    assert loader.load() == {"status": "uneventful"}
+
 
 def test_loader_with_special_chars_in_svn_url(repo_url, tmp_path):
     content = b"foo"
 
     filename = "".join(
         itertools.chain(
             (chr(i) for i in range(32, 127)), (chr(i) for i in range(161, 256))
```

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_svn_repo.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_repo.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_svn_retry.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_task.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/test_utils.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,51 +405,63 @@
         # subversion >= 1.6
         (
             'http://svn.thirdparty.com/repos/My%20Project "My Project"',
             "trunk/externals",
             "http://svn.example.org/repos/test",
             (
                 "My Project",
-                "http://svn.thirdparty.com/repos/My%20Project",
+                "http://svn.thirdparty.com/repos/My Project",
+                None,
+                None,
+                False,
+            ),
+        ),
+        (
+            "http://svn.thirdparty.com/repos/My%20Project 'My Project'",
+            "trunk/externals",
+            "http://svn.example.org/repos/test",
+            (
+                "My Project",
+                "http://svn.thirdparty.com/repos/My Project",
                 None,
                 None,
                 False,
             ),
         ),
         (
             'http://svn.thirdparty.com/repos/My%20%20%20Project "My   Project"',
             "trunk/externals",
             "http://svn.example.org/repos/test",
             (
                 "My   Project",
-                "http://svn.thirdparty.com/repos/My%20%20%20Project",
+                "http://svn.thirdparty.com/repos/My   Project",
                 None,
                 None,
                 False,
             ),
         ),
         (
             'http://svn.thirdparty.com/repos/%22Quotes%20Too%22 \\"Quotes\\ Too\\"',
             "trunk/externals",
             "http://svn.example.org/repos/test",
             (
                 '"Quotes Too"',
-                "http://svn.thirdparty.com/repos/%22Quotes%20Too%22",
+                'http://svn.thirdparty.com/repos/"Quotes Too"',
                 None,
                 None,
                 False,
             ),
         ),
         (
             'http://svn.thirdparty.com/repos/%22Quotes%20%20%20Too%22 \\"Quotes\\ \\ \\ Too\\"',  # noqa
             "trunk/externals",
             "http://svn.example.org/repos/test",
             (
                 '"Quotes   Too"',
-                "http://svn.thirdparty.com/repos/%22Quotes%20%20%20Too%22",
+                'http://svn.thirdparty.com/repos/"Quotes   Too"',
                 None,
                 None,
                 False,
             ),
         ),
         # edge cases
         (
@@ -544,14 +556,26 @@
                 "third-party/sounds",
                 "http://svn.example.com/repos/sounds",
                 123,
                 150,
                 False,
             ),
         ),
+        (
+            "-r 123 http://svn.example.com/repos/some%20sounds@150 third-party/sounds",
+            "trunk/externals",
+            "http://svn.example.org/repos/test",
+            (
+                "third-party/sounds",
+                "http://svn.example.com/repos/some sounds",
+                123,
+                150,
+                False,
+            ),
+        ),
     ],
 )
 def test_parse_external_definition(external, dir_path, repo_url, expected_result):
     assert (
         utils.parse_external_definition(external, dir_path, repo_url) == expected_result
     )
```

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/tests/utils.py` & `swh.loader.svn-1.7.0/swh/loader/svn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.6.0/swh/loader/svn/utils.py` & `swh.loader.svn-1.7.0/swh/loader/svn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 import os
 import re
 import shutil
 from subprocess import PIPE, Popen, call, run
 import tempfile
 from typing import Optional, Tuple
-from urllib.parse import quote, urlparse, urlunparse
+from urllib.parse import quote, unquote, urlparse, urlunparse
 
 import iso8601
 from subvertpy import SubversionException
 
 logger = logging.getLogger(__name__)
 
 
@@ -292,19 +292,19 @@
                 e.replace("\\ ", " ")
                 for e in external_split
                 if e.startswith(external_part[2:])
             ][0]
             path = f'"{path}"'
         elif external_part.endswith('\\"'):
             continue
-        elif external_part.startswith('"'):
-            external_split = external.split('"')
-            path_prefix = external_part.strip('"')
+        elif external_part.startswith(('"', "'")):
+            external_split = external.split(external_part[0])
+            path_prefix = external_part.strip(external_part[0])
             path = next(iter([e for e in external_split if e.startswith(path_prefix)]))
-        elif external_part.endswith('"'):
+        elif external_part.endswith(('"', "'")):
             continue
         elif not external_part.startswith("\\") and external_part != "-r":
             # path of the external relative to dir_path
             path = external_part.replace("\\\\", "\\")
             if path == external_part:
                 path = external_part.replace("\\", "")
             if path.startswith("./"):
@@ -335,15 +335,15 @@
                     # revision it will detect it at next origin visit and perform a full reload.
                     logger.debug(e)
                     pass
 
     if not external_url or not path:
         raise ValueError(f"Failed to parse external definition '{external}'")
 
-    return path.rstrip("/"), external_url, revision, peg_revision, relative_url
+    return path.rstrip("/"), unquote(external_url), revision, peg_revision, relative_url
 
 
 def is_recursive_external(
     origin_url: str, dir_path: str, external_path: str, external_url: str
 ) -> bool:
     """
     Check if an external definition can lead to a recursive subversion export
```

### Comparing `swh.loader.svn-1.6.0/swh.loader.svn.egg-info/PKG-INFO` & `swh.loader.svn-1.7.0/swh.loader.svn.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.6.0
+Version: 1.7.0
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -16,42 +16,41 @@
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 License-File: AUTHORS
 
-swh-loader-svn
-==============
+# swh-loader-svn [![Build Status](https://jenkins.softwareheritage.org/job/DLDSVN/job/master/badge/icon)](https://jenkins.softwareheritage.org/job/DLDSVN/job/master/)
 
-The Software Heritage SVN Loader is a tool and a library to walk a remote svn repository
-and inject into the SWH dataset all contained files that weren't known before.
+The Software Heritage Subversion loader is a tool and a library to walk a remote svn
+repository and inject into the Software Heritage archive all contained files, directories
+and commits that weren't known before.
 
 The main entry points are
 
-- :class:`swh.loader.svn.loader.SvnLoader` for the main svn loader which ingests content out of
+- `swh.loader.svn.loader.SvnLoader` for the main svn loader which ingests content out of
   a remote svn repository
 
-- :class:`swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
+- `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
-- :class:`swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
+- `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
-# CLI run
+## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
-```
+```yml
 storage:
   cls: remote
   args:
     url: http://localhost:5002/
 ```
 
 Run:
 
-```
-swh loader --config-file /tmp/loader_svn.yml \
-    run svn <svn-repository-url>
+```shell
+$ swh loader --config-file /tmp/loader_svn.yml run svn <svn-repository-url>
 ```
```

### Comparing `swh.loader.svn-1.6.0/swh.loader.svn.egg-info/SOURCES.txt` & `swh.loader.svn-1.7.0/swh.loader.svn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -38,25 +38,28 @@
 swh.loader.svn.egg-info/entry_points.txt
 swh.loader.svn.egg-info/requires.txt
 swh.loader.svn.egg-info/top_level.txt
 swh/loader/__init__.py
 swh/loader/svn/__init__.py
 swh/loader/svn/converters.py
 swh/loader/svn/exception.py
+swh/loader/svn/fast_crawler.cpp
+swh/loader/svn/fast_crawler.pyi
 swh/loader/svn/loader.py
 swh/loader/svn/py.typed
 swh/loader/svn/replay.py
 swh/loader/svn/svn_repo.py
 swh/loader/svn/svn_retry.py
 swh/loader/svn/tasks.py
 swh/loader/svn/utils.py
 swh/loader/svn/tests/__init__.py
 swh/loader/svn/tests/conftest.py
 swh/loader/svn/tests/test_converters.py
 swh/loader/svn/tests/test_externals.py
+swh/loader/svn/tests/test_fast_crawler.py
 swh/loader/svn/tests/test_loader.org
 swh/loader/svn/tests/test_loader.py
 swh/loader/svn/tests/test_svn_repo.py
 swh/loader/svn/tests/test_svn_retry.py
 swh/loader/svn/tests/test_task.py
 swh/loader/svn/tests/test_utils.py
 swh/loader/svn/tests/utils.py
```

### Comparing `swh.loader.svn-1.6.0/tox.ini` & `swh.loader.svn-1.7.0/tox.ini`

 * *Files identical despite different names*


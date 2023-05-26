# Comparing `tmp/fixtures-4.0.1.tar.gz` & `tmp/fixtures-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixtures-4.0.1.tar", last modified: Fri Jul  1 18:41:56 2022, max compression
+gzip compressed data, was "fixtures-4.1.0.tar", last modified: Fri May 26 13:28:26 2023, max compression
```

## Comparing `fixtures-4.0.1.tar` & `fixtures-4.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.253736 fixtures-4.0.1/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.249736 fixtures-4.0.1/.github/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.249736 fixtures-4.0.1/.github/workflows/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2091 2022-07-01 18:40:30.000000 fixtures-4.0.1/.github/workflows/ci.yaml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      170 2022-01-28 15:37:28.000000 fixtures-4.0.1/.testr.conf
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1150 2022-07-01 18:41:56.000000 fixtures-4.0.1/AUTHORS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11358 2022-01-28 15:37:28.000000 fixtures-4.0.1/Apache-2.0
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1510 2022-01-28 15:37:28.000000 fixtures-4.0.1/BSD
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1476 2022-01-28 15:37:28.000000 fixtures-4.0.1/COPYING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    11815 2022-07-01 18:41:56.000000 fixtures-4.0.1/ChangeLog
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      821 2022-01-28 15:37:28.000000 fixtures-4.0.1/GOALS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1381 2022-01-28 15:37:28.000000 fixtures-4.0.1/HACKING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      127 2022-01-28 15:37:28.000000 fixtures-4.0.1/MANIFEST.in
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      290 2022-01-28 15:37:28.000000 fixtures-4.0.1/Makefile
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    10744 2022-07-01 18:40:30.000000 fixtures-4.0.1/NEWS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    20025 2022-07-01 18:41:56.253736 fixtures-4.0.1/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18738 2022-07-01 18:40:30.000000 fixtures-4.0.1/README.rst
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.249736 fixtures-4.0.1/fixtures/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3611 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/__init__.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.253736 fixtures-4.0.1/fixtures/_fixtures/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2296 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1987 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/environ.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4593 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/logger.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2798 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/_fixtures/mockpatch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6141 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/monkeypatch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1551 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/packagepath.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     6643 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/_fixtures/popen.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2399 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/pythonpackage.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1332 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/pythonpath.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2719 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/_fixtures/streams.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2269 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/tempdir.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1100 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/temphomedir.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2312 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/timeout.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1344 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/_fixtures/warnings.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3432 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/callmany.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15155 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/fixture.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2182 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/testcase.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.253736 fixtures-4.0.1/fixtures/tests/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1503 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/tests/__init__.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.253736 fixtures-4.0.1/fixtures/tests/_fixtures/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1290 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3132 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_environ.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     7860 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_logger.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2314 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_mockpatch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    16006 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_monkeypatch.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1718 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_packagepath.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     8642 2022-07-01 18:40:30.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_popen.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1816 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_pythonpackage.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1601 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_pythonpath.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3742 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_streams.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     3400 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_tempdir.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1534 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_temphomedir.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2334 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_timeout.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1830 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/_fixtures/test_warnings.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1254 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/helpers.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     2535 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/test_callmany.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    15259 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/test_fixture.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     4151 2022-01-28 15:37:28.000000 fixtures-4.0.1/fixtures/tests/test_testcase.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-07-01 18:41:56.249736 fixtures-4.0.1/fixtures.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    20025 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1669 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/dependency_links.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/not-zip-safe
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       46 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/pbr.json
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       72 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/requires.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        9 2022-07-01 18:41:56.000000 fixtures-4.0.1/fixtures.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      100 2022-07-01 18:40:30.000000 fixtures-4.0.1/pyproject.toml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       11 2022-07-01 18:40:30.000000 fixtures-4.0.1/requirements.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1151 2022-07-01 18:41:56.253736 fixtures-4.0.1/setup.cfg
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)      110 2022-07-01 18:40:30.000000 fixtures-4.0.1/setup.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      178 2022-07-01 18:40:30.000000 fixtures-4.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.376124 fixtures-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.356124 fixtures-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.364124 fixtures-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-26 13:28:16.000000 fixtures-4.1.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 13:28:16.000000 fixtures-4.1.0/.testr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 13:28:26.000000 fixtures-4.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 13:28:16.000000 fixtures-4.1.0/Apache-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-26 13:28:16.000000 fixtures-4.1.0/BSD
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-26 13:28:16.000000 fixtures-4.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-26 13:28:26.000000 fixtures-4.1.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-26 13:28:16.000000 fixtures-4.1.0/GOALS
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-26 13:28:16.000000 fixtures-4.1.0/HACKING
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 13:28:16.000000 fixtures-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 13:28:16.000000 fixtures-4.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-05-26 13:28:16.000000 fixtures-4.1.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-26 13:28:26.376124 fixtures-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-05-26 13:28:16.000000 fixtures-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.364124 fixtures-4.1.0/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.372124 fixtures-4.1.0/fixtures/_fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/mockpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/packagepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/pythonpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/pythonpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/temphomedir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/_fixtures/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/callmany.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.372124 fixtures-4.1.0/fixtures/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.376124 fixtures-4.1.0/fixtures/tests/_fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_mockpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_packagepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_pythonpackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_pythonpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_temphomedir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/_fixtures/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/test_callmany.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-26 13:28:16.000000 fixtures-4.1.0/fixtures/tests/test_testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:26.368124 fixtures-4.1.0/fixtures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 13:28:26.000000 fixtures-4.1.0/fixtures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 13:28:16.000000 fixtures-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 13:28:16.000000 fixtures-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-26 13:28:26.376124 fixtures-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-05-26 13:28:16.000000 fixtures-4.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 13:28:16.000000 fixtures-4.1.0/tox.ini
```

### Comparing `fixtures-4.0.1/.github/workflows/ci.yaml` & `fixtures-4.1.0/.github/workflows/ci.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -5,67 +5,67 @@
   - pull_request
 jobs:
   test:
     name: Run unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11.0-beta - 3.11", "pypy-3.7", "pypy-3.8", "pypy-3.9"]
+        python: ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy-3.7", "pypy-3.8", "pypy-3.9"]
     steps:
       - name: Checkout source code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: python -m pip install tox
       - name: Run unit tests (via tox)
         # Run tox using the version of Python in `PATH`
         run: tox -e py
   docs:
     name: Build docs
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - name: Set up Python 3.10
-        uses: actions/setup-python@v2
+      - name: Set up Python 3.11
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: python -m pip install docutils
       - name: Build docs
         run: rst2html.py README.rst README.html
       - name: Archive build results
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: html-docs-build
           path: README.html
           retention-days: 7
   release:
     name: Upload release artifacts
     runs-on: ubuntu-latest
     needs: test
     if: github.event_name == 'push'
     steps:
       - name: Checkout source code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - name: Set up Python 3.10
-        uses: actions/setup-python@v2
+      - name: Set up Python 3.11
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: python -m pip install build
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/ .
       - name: Publish distribution to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `fixtures-4.0.1/AUTHORS` & `fixtures-4.1.0/AUTHORS`

 * *Files 5% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 Joshua Harlow <harlowja@yahoo-inc.com>
 Julien Danjou <julien@danjou.info>
 Jürgen Gmach <juergen.gmach@googlemail.com>
 Martin Pool <mbp@canonical.com>
 Michał Górny <mgorny@gentoo.org>
 Robert Collins <robertc@robertcollins.net>
 Sean Dague <sean@dague.net>
+Stephen Finucane <stephen@that.guru>
 Stephen Finucane <stephenfin@redhat.com>
 Steve Kowalik <steve.kowalik@canonical.com>
 hugovk <hugovk@users.noreply.github.com>
```

### Comparing `fixtures-4.0.1/Apache-2.0` & `fixtures-4.1.0/Apache-2.0`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/BSD` & `fixtures-4.1.0/BSD`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/COPYING` & `fixtures-4.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/ChangeLog` & `fixtures-4.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 CHANGES
 =======
 
+4.1.0
+-----
+
+* Release 4.1.0
+* README: Use actual admonitions
+* README: Document missing fixtures
+* github: Update actions, switch to 3.11 by default
+* README: Trivial fixes
+* Update tox.ini
+* Add WarningsFilter fixture
+* tests: Replace hardcoded list of test modules
+* tests: Run 'warnings' tests
+* Don't explicitly build-require wheel
+* Drop support for Python 3.6
+
 4.0.1
 -----
 
 * Release 4.0.1
 * Remove testtools from requirements.txt as well
 * github: Add all pypy3 versions to test matrix
 * github: Add Python 3.11 betas to test matrix
```

### Comparing `fixtures-4.0.1/GOALS` & `fixtures-4.1.0/GOALS`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/HACKING` & `fixtures-4.1.0/HACKING`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/NEWS` & `fixtures-4.1.0/NEWS`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 ----------------------
 fixtures release notes
 ----------------------
 
 NEXT
 ~~~~
 
+4.1.0
+~~~~~
+
+* Drop support for Python 3.6 (EOL)
+  (Stephen Finucane)
+
+* Add a new ``WarningsFilter`` filter, allowing users to filter warnings as
+  part of their tests, before restoring said filters.
+  (Stephen Finucane)
+
 4.0.1
 ~~~~~
 
 * Remove ``testtools`` from ``requirements.txt`` as well.
   (Colin Watson)
 
 4.0.0
```

### Comparing `fixtures-4.0.1/PKG-INFO` & `fixtures-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,175 +1,157 @@
 Metadata-Version: 2.1
 Name: fixtures
-Version: 4.0.1
+Version: 4.1.0
 Summary: Fixtures, reusable state for writing clean tests and more.
 Home-page: https://github.com/testing-cabal/fixtures
 Author: Robert Collins
 Author-email: robertc@robertcollins.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: docs
 Provides-Extra: streams
 Provides-Extra: test
+Provides-Extra: docs
 License-File: COPYING
 
-*************************************************************
-fixtures: Fixtures with cleanups for testing and convenience.
-*************************************************************
-
-  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
-
-  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
-  license at the users choice. A copy of both licenses are available in the
-  project source as Apache-2.0 and BSD. You may not use this file except in
-  compliance with one of these two licences.
+************************************************************
+fixtures: Fixtures with cleanups for testing and convenience
+************************************************************
 
-  Unless required by applicable law or agreed to in writing, software
-  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
-  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
-  license you chose for the specific language governing permissions and
-  limitations under that license.
-
-
-Fixtures defines a Python contract for reusable state / support logic,
+*fixtures* defines a Python contract for reusable state / support logic,
 primarily for unit testing. Helper and adaption logic is included to make it
 easy to write your own fixtures using the fixtures contract. Glue code is
-provided that makes using fixtures that meet the Fixtures contract in unittest
-compatible test cases easy and straight forward.
+provided that makes using fixtures that meet the ``Fixtures`` contract in
+``unittest`` compatible test cases easy and straight forward.
 
 Dependencies
 ============
 
-* Python 3.6+
+* Python 3.7+
   This is the base language fixtures is written in and for.
 
-* pbr
+* ``pbr``
   Used for version and release management of fixtures.
 
 The ``fixtures[streams]`` extra adds:
 
-* testtools <https://launchpad.net/testtools> 0.9.22 or newer.
-  testtools provides helpful glue functions for the details API used to report
+* ``testtools`` <https://launchpad.net/testtools>
+
+  ``testtools`` provides helpful glue functions for the details API used to report
   information about a fixture (whether its used in a testing or production
   environment).
 
-For use in a unit test suite using the included glue, one of:
-
-* bzrlib.tests
-
-* Or any other test environment that supports TestCase.addCleanup.
+For use in a unit test suite using the included glue, you will need a test
+environment that supports ``TestCase.addCleanup``. Writing your own glue code
+is easy. Alternatively, you can simply use Fixtures directly without any
+support code.
 
-Writing your own glue code is easy, or you can simply use Fixtures directly
-without any support code.
-
-To run the test suite for fixtures, testtools is needed.
+To run the test suite for fixtures, ``testtools`` is needed.
 
 Why Fixtures
 ============
 
-Standard Python unittest.py provides no obvious method for making and reusing
+Standard Python ``unittest`` provides no obvious method for making and reusing
 state needed in a test case other than by adding a method on the test class.
 This scales poorly - complex helper functions propagating up a test class
-hierarchy is a regular pattern when this is done. Mocking while a great tool
+hierarchy is a regular pattern when this is done. Mocking, while a great tool,
 doesn't itself prevent this (and helpers to mock complex things can accumulate
 in the same way if placed on the test class).
 
 By defining a uniform contract where helpers have no dependency on the test
 class we permit all the regular code hygiene activities to take place without
 the distorting influence of being in a class hierarchy that is modelling an
-entirely different thing - which is what helpers on a TestCase suffer from.
+entirely different thing - which is what helpers on a ``TestCase`` suffer from.
 
 About Fixtures
 ==============
 
-A Fixture represents some state. Each fixture has attributes on it that are
+A fixture represents some state. Each fixture has attributes on it that are
 specific to the fixture. For instance, a fixture representing a directory that
-can be used for temporary files might have a attribute 'path'.
+can be used for temporary files might have a attribute ``path``.
 
 Most fixtures have complete ``pydoc`` documentation, so be sure to check
 ``pydoc fixtures`` for usage information.
 
 Creating Fixtures
 =================
 
-Minimally, subclass Fixture, define _setUp to initialize your state and schedule
-a cleanup for when cleanUp is called and you're done::
+Minimally, subclass ``Fixture``, define ``_setUp`` to initialize your state,
+schedule a cleanup for when ``cleanUp`` is called, and you're done::
 
   >>> import unittest
   >>> import fixtures
   >>> class NoddyFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.frobnozzle = 42
   ...         self.addCleanup(delattr, self, 'frobnozzle')
 
-This will initialize frobnozzle when ``setUp`` is called, and when ``cleanUp``
-is called get rid of the frobnozzle attribute. Prior to version 1.3.0 fixtures
-recommended overriding ``setUp``. This is still supported, but since it is
-harder to write leak-free fixtures in this fashion, it is not recommended.
+This will initialize ``frobnozzle`` when ``setUp`` is called, and when
+``cleanUp`` is called get rid of the ``frobnozzle`` attribute. Prior to version
+1.3.0 *fixtures* recommended overriding ``setUp``. This is still supported, but
+since it is harder to write leak-free fixtures in this fashion, it is not
+recommended.
 
 If your fixture has diagnostic data - for instance the log file of an
-application server, or log messages, it can expose that by creating a content
-object (``testtools.content.Content``) and calling ``addDetail``.
+application server, or log messages - it can expose that by creating a content
+object (``testtools.content.Content``) and calling ``addDetail``::
 
   >>> from testtools.content import text_content
   >>> class WithLog(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addDetail('message', text_content('foo bar baz'))
 
 The method ``useFixture`` will use another fixture, call ``setUp`` on it, call
 ``self.addCleanup(thefixture.cleanUp)``, attach any details from it and return
-the fixture. This allows simple composition of different fixtures.
+the fixture. This allows simple composition of different fixtures::
 
   >>> class ReusingFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.noddy = self.useFixture(NoddyFixture())
 
-There is a helper for adapting a function or function pair into Fixtures. it
-puts the result of the function in fn_result::
+There is a helper for adapting a function or function pair into Fixtures. It
+puts the result of the function in ``fn_result``::
 
   >>> import os.path
   >>> import shutil
   >>> import tempfile
   >>> def setup_function():
   ...     return tempfile.mkdtemp()
   >>> def teardown_function(fixture):
   ...     shutil.rmtree(fixture)
   >>> fixture = fixtures.FunctionFixture(setup_function, teardown_function)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-This can be expressed even more pithily:
+This can be expressed even more pithily::
 
   >>> fixture = fixtures.FunctionFixture(tempfile.mkdtemp, shutil.rmtree)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-Another variation is MethodFixture which is useful for adapting alternate
+Another variation is ``MethodFixture`` which is useful for adapting alternate
 fixture implementations to Fixture::
 
   >>> class MyServer:
   ...    def start(self):
   ...        pass
   ...    def stop(self):
   ...        pass
@@ -183,42 +165,42 @@
   >>> with noddy_with_log as x:
   ...     print (x.fixtures[0].frobnozzle)
   42
 
 The Fixture API
 ===============
 
-The example above introduces some of the Fixture API. In order to be able to
-clean up after a fixture has been used, all fixtures define a ``cleanUp``
+The example above introduces some of the ``Fixture`` API. In order to be able
+to clean up after a fixture has been used, all fixtures define a ``cleanUp``
 method which should be called when a fixture is finished with.
 
 Because it's nice to be able to build a particular set of related fixtures in
 advance of using them, fixtures also have a ``setUp`` method which should be
 called before trying to use them.
 
 One common desire with fixtures that are expensive to create is to reuse them
-in many test cases; to support this the base Fixture also defines a ``reset``
-which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
+in many test cases; to support this the base ``Fixture`` also defines a
+``reset`` which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
 efficiently make themselves reusable should override this method. This can then
 be used with multiple test state via things like ``testresources``,
 ``setUpClass``, or ``setUpModule``.
 
-When using a fixture with a test you can manually call the setUp and cleanUp
-methods. More convenient though is to use the included glue from
-``fixtures.TestWithFixtures`` which provides a mixin defining
-``useFixture`` (camel case because unittest is camel case throughout) method.
-It will call setUp on the fixture, call self.addCleanup(fixture) to schedule a
+When using a fixture with a test you can manually call the ``setUp`` and
+``cleanUp`` methods. More convenient though is to use the included glue from
+``fixtures.TestWithFixtures`` which provides a mixin defining ``useFixture``
+(camel case because ``unittest`` is camel case throughout) method. It will call
+``setUp`` on the fixture, call ``self.addCleanup(fixture)`` to schedule a
 cleanup, and return the fixture. This lets one write::
 
   >>> import testtools
   >>> import unittest
 
-Note that we use ``testtools.TestCase``. testtools has it's own implementation
-of ``useFixture`` so there is no need to use ``fixtures.TestWithFixtures`` with
-``testtools.TestCase``.
+Note that we use ``testtools.TestCase``. ``testtools`` has it's own
+implementation of ``useFixture`` so there is no need to use
+``fixtures.TestWithFixtures`` with ``testtools.TestCase``::
 
   >>> class NoddyTest(testtools.TestCase, fixtures.TestWithFixtures):
   ...     def test_example(self):
   ...         fixture = self.useFixture(NoddyFixture())
   ...         self.assertEqual(42, fixture.frobnozzle)
   >>> result = unittest.TestResult()
   >>> _ = NoddyTest('test_example').run(result)
@@ -228,16 +210,16 @@
 Fixtures implement the context protocol, so you can also use a fixture as a
 context manager::
 
   >>> with fixtures.FunctionFixture(setup_function, teardown_function) as fixture:
   ...    print (os.path.isdir(fixture.fn_result))
   True
 
-When multiple cleanups error, fixture.cleanUp() will raise a wrapper exception
-rather than choosing an arbitrary single exception to raise::
+When multiple cleanups error, ``fixture.cleanUp()`` will raise a wrapper
+exception rather than choosing an arbitrary single exception to raise::
 
   >>> import sys
   >>> from fixtures.fixture import MultipleExceptions
   >>> class BrokenFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addCleanup(lambda:1/0)
   ...         self.addCleanup(lambda:1/0)
@@ -248,39 +230,39 @@
   ... except MultipleExceptions:
   ...    exc_info = sys.exc_info()
   >>> print (exc_info[1].args[0][0].__name__)
   ZeroDivisionError
 
 Fixtures often expose diagnostic details that can be useful for tracking down
 issues. The ``getDetails`` method will return a dict of all the attached
-details, but can only be called before ``cleanUp`` is called. Each detail
-object is an instance of ``testtools.content.Content``.
+details but can only be called before ``cleanUp`` is called. Each detail
+object is an instance of ``testtools.content.Content``::
 
   >>> with WithLog() as l:
   ...     print(l.getDetails()['message'].as_text())
   foo bar baz
 
 Errors in setUp
 +++++++++++++++
 
 The examples above used ``_setUp`` rather than ``setUp`` because the base
 class implementation of ``setUp`` acts to reduce the chance of leaking
 external resources if an error is raised from ``_setUp``. Specifically,
-``setUp`` contains a try:/except: block which catches all exceptions, captures
+``setUp`` contains a try/except block which catches all exceptions, captures
 any registered detail objects, and calls ``self.cleanUp`` before propagating
 the error. As long as you take care to register any cleanups before calling
 the code that may fail, this will cause them to be cleaned up. The captured
 detail objects are provided to the args of the raised exception.
 
 If the error that occurred was a subclass of ``Exception`` then ``setUp`` will
 raise ``MultipleExceptions`` with the last element being a ``SetupError`` that
 contains the detail objects. Otherwise, to prevent causing normally
-uncatchable errors like KeyboardInterrupt being caught inappropriately in the
-calling layer, the original exception will be raised as-is and no diagnostic
-data other than that from the original exception will be available.
+uncatchable errors like ``KeyboardInterrupt`` being caught inappropriately in
+the calling layer, the original exception will be raised as-is and no
+diagnostic data other than that from the original exception will be available.
 
 Shared Dependencies
 +++++++++++++++++++
 
 A common use case within complex environments is having some fixtures shared by
 other ones.
 
@@ -326,214 +308,285 @@
 in a tempdir - on Windows this will prevent the directory being deleted).
 
 Another approach which ``fixtures`` neither helps nor hinders is to raise
 a signal of some sort for each user of a fixture before it is reset. In the
 example here, ``TempDir`` might offer a subscribers attribute that both the
 DB and web server would be registered in. Calling ``reset`` or ``cleanUp``
 on the tempdir would trigger a callback to all the subscribers; the DB and
-web server reset methods would look something like:
+web server reset methods would look something like::
 
   >>> def reset(self):
   ...     if not self._cleaned:
   ...         self._clean()
 
 (Their action on the callback from the tempdir would be to do whatever work
 was needed and set ``self._cleaned``.) This approach has the (perhaps)
 surprising effect that resetting the webserver may reset the DB - if the
 webserver were to be depending on ``tempdir.reset`` as a way to reset the
-webservers state.
+webserver's state.
 
 Another approach which is not currently implemented is to provide an object
 graph of dependencies and a reset mechanism that can traverse that, along with
 a separation between 'reset starting' and 'reset finishing' - the DB and
 webserver would both have their ``reset_starting`` methods called, then the
 tempdir would be reset, and finally the DB and webserver would have
 ``reset_finishing`` called.
 
 Stock Fixtures
 ==============
 
-In addition to the Fixture, FunctionFixture and MethodFixture classes fixtures
-includes a number of precanned fixtures. The API docs for fixtures will list
-the complete set of these, should the dcs be out of date or not to hand. For
-the complete feature set of each fixture please see the API docs.
+In addition to the ``Fixture``, ``FunctionFixture`` and ``MethodFixture``
+classes, fixtures includes a number of pre-canned fixtures. The API docs for
+fixtures will list the complete set of these, should the docs be out of date or
+not to hand. For the complete feature set of each fixture please see the API
+docs.
 
-ByteStream
-++++++++++
+``ByteStream``
+++++++++++++++
 
-Trivial adapter to make a BytesIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``BytesIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('my-content')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.something', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-EnvironmentVariable
-+++++++++++++++++++
+``EnvironmentVariable``
++++++++++++++++++++++++
 
 Isolate your code from environmental variables, delete them or set them to a
-new value.
+new value::
 
   >>> fixture = fixtures.EnvironmentVariable('HOME')
 
-FakeLogger
-++++++++++
+``FakeLogger``
+++++++++++++++
 
 Isolate your code from an external logging configuration - so that your test
-gets the output from logged messages, but they don't go to e.g. the console.
+gets the output from logged messages, but they don't go to e.g. the console::
 
   >>> fixture = fixtures.FakeLogger()
 
-FakePopen
-+++++++++
+``FakePopen``
++++++++++++++
 
 Pretend to run an external command rather than needing it to be present to run
-tests.
+tests::
 
   >>> from io import BytesIO
   >>> fixture = fixtures.FakePopen(lambda _:{'stdout': BytesIO('foobar')})
 
-MockPatchObject
-+++++++++++++++
+``LogHandler``
+++++++++++++++
 
-Adapts ``mock.patch.object`` to be used as a Fixture.
+Replace or extend a logger's handlers. The behavior of this fixture depends on
+the value of the ``nuke_handlers`` parameter: if ``true``, the logger's
+existing handlers are removed and replaced by the provided handler, while if
+``false`` the logger's set of handlers is extended by the provided handler::
+
+  >>> from logging import StreamHandler
+  >>> fixture = fixtures.LogHandler(StreamHandler())
+
+``MockPatchObject``
++++++++++++++++++++
+
+Adapts ``mock.patch.object`` to be used as a fixture::
 
   >>> class Fred:
   ...     value = 1
   >>> fixture = fixtures.MockPatchObject(Fred, 'value', 2)
   >>> with fixture:
   ...     Fred().value
   2
   >>> Fred().value
   1
 
-MockPatch
-+++++++++
+``MockPatch``
++++++++++++++
 
-Adapts ``mock.patch`` to be used as a Fixture.
+Adapts ``mock.patch`` to be used as a fixture::
 
   >>> fixture = fixtures.MockPatch('subprocess.Popen.returncode', 3)
 
-MockPatchMultiple
-+++++++++++++++++
+``MockPatchMultiple``
++++++++++++++++++++++
 
-Adapts ``mock.patch.multiple`` to be used as a Fixture.
+Adapts ``mock.patch.multiple`` to be used as a ``fixture``::
 
   >>> fixture = fixtures.MockPatchMultiple('subprocess.Popen', returncode=3)
 
-MonkeyPatch
-+++++++++++
+``MonkeyPatch``
++++++++++++++++
 
-Control the value of a named Python attribute.
+Control the value of a named Python attribute::
 
   >>> def fake_open(path, mode):
   ...     pass
   >>> fixture = fixtures.MonkeyPatch('__builtin__.open', fake_open)
 
 Note that there are some complexities when patching methods - please see the
 API documentation for details.
 
-NestedTempfile
-++++++++++++++
+``NestedTempfile``
+++++++++++++++++++
 
-Change the default directory that the tempfile module places temporary files
-and directories in. This can be useful for containing the noise created by
-code which doesn't clean up its temporary files. This does not affect
-temporary file creation where an explicit containing directory was provided.
+Change the default directory that the ``tempfile`` module places temporary
+files and directories in. This can be useful for containing the noise created
+by code which doesn't clean up its temporary files. This does not affect
+temporary file creation where an explicit containing directory was provided::
 
   >>> fixture = fixtures.NestedTempfile()
 
-PackagePathEntry
-++++++++++++++++
+``PackagePathEntry``
+++++++++++++++++++++
 
 Adds a single directory to the path for an existing Python package. This adds
-to the package.__path__ list. If the directory is already in the path, nothing
-happens, if it isn't then it is added on setUp and removed on cleanUp.
+to the ``package.__path__`` list. If the directory is already in the path,
+nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PackagePathEntry('package/name', '/foo/bar')
 
-PythonPackage
-+++++++++++++
+``PythonPackage``
++++++++++++++++++
 
 Creates a python package directory. Particularly useful for testing code that
 dynamically loads packages/modules, or for mocking out the command line entry
-points to Python programs.
+points to Python programs::
 
   >>> fixture = fixtures.PythonPackage('foo.bar', [('quux.py', '')])
 
-PythonPathEntry
-+++++++++++++++
+``PythonPathEntry``
++++++++++++++++++++
 
-Adds a single directory to sys.path. If the directory is already in the path,
-nothing happens, if it isn't then it is added on setUp and removed on cleanUp.
+Adds a single directory to ``sys.path``. If the directory is already in the
+path, nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PythonPathEntry('/foo/bar')
 
-StringStream
-++++++++++++
+``Stream``
+++++++++++
+
+Trivial adapter to expose a file-like object as a detail object, for automatic
+inclusion in test failure descriptions. ``StringStream`` and ``BytesStream``
+provided concrete users of this fixture.
+
+This requires the ``fixtures[streams]`` extra.
+
+``StringStream``
+++++++++++++++++
 
-Trivial adapter to make a StringIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``StringIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('stdout')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.stdout', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-TempDir
-+++++++
+``TempDir``
++++++++++++
 
-Create a temporary directory and clean it up later.
+Create a temporary directory and clean it up later::
 
   >>> fixture = fixtures.TempDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-TempHomeDir
-+++++++++++
+``TempHomeDir``
++++++++++++++++
 
-Create a temporary directory and set it as $HOME in the environment.
+Create a temporary directory and set it as ``$HOME`` in the environment::
 
   >>> fixture = fixtures.TempHomeDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-The environment will now have $HOME set to the same path, and the value
-will be returned to its previous value after tearDown.
+The environment will now have ``$HOME`` set to the same path, and the value
+will be returned to its previous value after ``tearDown``.
 
-Timeout
-+++++++
+``Timeout``
++++++++++++
 
 Aborts if the covered code takes more than a specified number of whole wall-clock
 seconds.
 
-There are two possibilities, controlled by the 'gentle' argument: when gentle,
+There are two possibilities, controlled by the ``gentle`` argument: when gentle,
 an exception will be raised and the test (or other covered code) will fail.
 When not gentle, the entire process will be terminated, which is less clean,
 but more likely to break hangs where no Python code is running.
 
-*Caution:* Only one timeout can be active at any time across all threads in a
-single process.  Using more than one has undefined results.  (This could be
-improved by chaining alarms.)
+.. caution::
+
+   Only one timeout can be active at any time across all threads in a single
+   process.  Using more than one has undefined results.  (This could be improved
+   by chaining alarms.)
+
+.. note::
+
+   Currently supported only on Unix because it relies on the ``alarm`` system
+   call.
 
-*Note:* Currently supported only on Unix because it relies on the ``alarm``
-system call.
+``WarningsCapture``
++++++++++++++++++++
+
+Capture warnings for later analysis::
+
+  >>> fixture = fixtures.WarningsCapture()
+
+The captured warnings are stored in the ``captures`` attribute of the fixture
+after ``setUp``.
+
+``WarningsFilter``
+++++++++++++++++++
+
+Configure warnings filters during test runs::
+
+  >>> fixture = fixtures.WarningsFilter(
+  ...     [
+  ...         {
+  ...             'action': 'ignore',
+  ...             'message': 'foo',
+  ...             'category': DeprecationWarning,
+  ...         },
+  ...     ]
+  ... )
+
+Order is important: entries closer to the front of the list override entries
+later in the list, if both match a particular warning.
 
 Contributing
 ============
 
 Fixtures has its project homepage on GitHub
 <https://github.com/testing-cabal/fixtures>.
 
+License
+=======
+
+  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
+
+  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
+  license at the users choice. A copy of both licenses are available in the
+  project source as Apache-2.0 and BSD. You may not use this file except in
+  compliance with one of these two licences.
 
+  Unless required by applicable law or agreed to in writing, software
+  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
+  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
+  license you chose for the specific language governing permissions and
+  limitations under that license.
```

### Comparing `fixtures-4.0.1/README.rst` & `fixtures-4.1.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,143 +1,127 @@
-*************************************************************
-fixtures: Fixtures with cleanups for testing and convenience.
-*************************************************************
+************************************************************
+fixtures: Fixtures with cleanups for testing and convenience
+************************************************************
 
-  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
-
-  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
-  license at the users choice. A copy of both licenses are available in the
-  project source as Apache-2.0 and BSD. You may not use this file except in
-  compliance with one of these two licences.
-
-  Unless required by applicable law or agreed to in writing, software
-  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
-  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
-  license you chose for the specific language governing permissions and
-  limitations under that license.
-
-
-Fixtures defines a Python contract for reusable state / support logic,
+*fixtures* defines a Python contract for reusable state / support logic,
 primarily for unit testing. Helper and adaption logic is included to make it
 easy to write your own fixtures using the fixtures contract. Glue code is
-provided that makes using fixtures that meet the Fixtures contract in unittest
-compatible test cases easy and straight forward.
+provided that makes using fixtures that meet the ``Fixtures`` contract in
+``unittest`` compatible test cases easy and straight forward.
 
 Dependencies
 ============
 
-* Python 3.6+
+* Python 3.7+
   This is the base language fixtures is written in and for.
 
-* pbr
+* ``pbr``
   Used for version and release management of fixtures.
 
 The ``fixtures[streams]`` extra adds:
 
-* testtools <https://launchpad.net/testtools> 0.9.22 or newer.
-  testtools provides helpful glue functions for the details API used to report
+* ``testtools`` <https://launchpad.net/testtools>
+
+  ``testtools`` provides helpful glue functions for the details API used to report
   information about a fixture (whether its used in a testing or production
   environment).
 
-For use in a unit test suite using the included glue, one of:
+For use in a unit test suite using the included glue, you will need a test
+environment that supports ``TestCase.addCleanup``. Writing your own glue code
+is easy. Alternatively, you can simply use Fixtures directly without any
+support code.
 
-* bzrlib.tests
-
-* Or any other test environment that supports TestCase.addCleanup.
-
-Writing your own glue code is easy, or you can simply use Fixtures directly
-without any support code.
-
-To run the test suite for fixtures, testtools is needed.
+To run the test suite for fixtures, ``testtools`` is needed.
 
 Why Fixtures
 ============
 
-Standard Python unittest.py provides no obvious method for making and reusing
+Standard Python ``unittest`` provides no obvious method for making and reusing
 state needed in a test case other than by adding a method on the test class.
 This scales poorly - complex helper functions propagating up a test class
-hierarchy is a regular pattern when this is done. Mocking while a great tool
+hierarchy is a regular pattern when this is done. Mocking, while a great tool,
 doesn't itself prevent this (and helpers to mock complex things can accumulate
 in the same way if placed on the test class).
 
 By defining a uniform contract where helpers have no dependency on the test
 class we permit all the regular code hygiene activities to take place without
 the distorting influence of being in a class hierarchy that is modelling an
-entirely different thing - which is what helpers on a TestCase suffer from.
+entirely different thing - which is what helpers on a ``TestCase`` suffer from.
 
 About Fixtures
 ==============
 
-A Fixture represents some state. Each fixture has attributes on it that are
+A fixture represents some state. Each fixture has attributes on it that are
 specific to the fixture. For instance, a fixture representing a directory that
-can be used for temporary files might have a attribute 'path'.
+can be used for temporary files might have a attribute ``path``.
 
 Most fixtures have complete ``pydoc`` documentation, so be sure to check
 ``pydoc fixtures`` for usage information.
 
 Creating Fixtures
 =================
 
-Minimally, subclass Fixture, define _setUp to initialize your state and schedule
-a cleanup for when cleanUp is called and you're done::
+Minimally, subclass ``Fixture``, define ``_setUp`` to initialize your state,
+schedule a cleanup for when ``cleanUp`` is called, and you're done::
 
   >>> import unittest
   >>> import fixtures
   >>> class NoddyFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.frobnozzle = 42
   ...         self.addCleanup(delattr, self, 'frobnozzle')
 
-This will initialize frobnozzle when ``setUp`` is called, and when ``cleanUp``
-is called get rid of the frobnozzle attribute. Prior to version 1.3.0 fixtures
-recommended overriding ``setUp``. This is still supported, but since it is
-harder to write leak-free fixtures in this fashion, it is not recommended.
+This will initialize ``frobnozzle`` when ``setUp`` is called, and when
+``cleanUp`` is called get rid of the ``frobnozzle`` attribute. Prior to version
+1.3.0 *fixtures* recommended overriding ``setUp``. This is still supported, but
+since it is harder to write leak-free fixtures in this fashion, it is not
+recommended.
 
 If your fixture has diagnostic data - for instance the log file of an
-application server, or log messages, it can expose that by creating a content
-object (``testtools.content.Content``) and calling ``addDetail``.
+application server, or log messages - it can expose that by creating a content
+object (``testtools.content.Content``) and calling ``addDetail``::
 
   >>> from testtools.content import text_content
   >>> class WithLog(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addDetail('message', text_content('foo bar baz'))
 
 The method ``useFixture`` will use another fixture, call ``setUp`` on it, call
 ``self.addCleanup(thefixture.cleanUp)``, attach any details from it and return
-the fixture. This allows simple composition of different fixtures.
+the fixture. This allows simple composition of different fixtures::
 
   >>> class ReusingFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.noddy = self.useFixture(NoddyFixture())
 
-There is a helper for adapting a function or function pair into Fixtures. it
-puts the result of the function in fn_result::
+There is a helper for adapting a function or function pair into Fixtures. It
+puts the result of the function in ``fn_result``::
 
   >>> import os.path
   >>> import shutil
   >>> import tempfile
   >>> def setup_function():
   ...     return tempfile.mkdtemp()
   >>> def teardown_function(fixture):
   ...     shutil.rmtree(fixture)
   >>> fixture = fixtures.FunctionFixture(setup_function, teardown_function)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-This can be expressed even more pithily:
+This can be expressed even more pithily::
 
   >>> fixture = fixtures.FunctionFixture(tempfile.mkdtemp, shutil.rmtree)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-Another variation is MethodFixture which is useful for adapting alternate
+Another variation is ``MethodFixture`` which is useful for adapting alternate
 fixture implementations to Fixture::
 
   >>> class MyServer:
   ...    def start(self):
   ...        pass
   ...    def stop(self):
   ...        pass
@@ -151,42 +135,42 @@
   >>> with noddy_with_log as x:
   ...     print (x.fixtures[0].frobnozzle)
   42
 
 The Fixture API
 ===============
 
-The example above introduces some of the Fixture API. In order to be able to
-clean up after a fixture has been used, all fixtures define a ``cleanUp``
+The example above introduces some of the ``Fixture`` API. In order to be able
+to clean up after a fixture has been used, all fixtures define a ``cleanUp``
 method which should be called when a fixture is finished with.
 
 Because it's nice to be able to build a particular set of related fixtures in
 advance of using them, fixtures also have a ``setUp`` method which should be
 called before trying to use them.
 
 One common desire with fixtures that are expensive to create is to reuse them
-in many test cases; to support this the base Fixture also defines a ``reset``
-which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
+in many test cases; to support this the base ``Fixture`` also defines a
+``reset`` which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
 efficiently make themselves reusable should override this method. This can then
 be used with multiple test state via things like ``testresources``,
 ``setUpClass``, or ``setUpModule``.
 
-When using a fixture with a test you can manually call the setUp and cleanUp
-methods. More convenient though is to use the included glue from
-``fixtures.TestWithFixtures`` which provides a mixin defining
-``useFixture`` (camel case because unittest is camel case throughout) method.
-It will call setUp on the fixture, call self.addCleanup(fixture) to schedule a
+When using a fixture with a test you can manually call the ``setUp`` and
+``cleanUp`` methods. More convenient though is to use the included glue from
+``fixtures.TestWithFixtures`` which provides a mixin defining ``useFixture``
+(camel case because ``unittest`` is camel case throughout) method. It will call
+``setUp`` on the fixture, call ``self.addCleanup(fixture)`` to schedule a
 cleanup, and return the fixture. This lets one write::
 
   >>> import testtools
   >>> import unittest
 
-Note that we use ``testtools.TestCase``. testtools has it's own implementation
-of ``useFixture`` so there is no need to use ``fixtures.TestWithFixtures`` with
-``testtools.TestCase``.
+Note that we use ``testtools.TestCase``. ``testtools`` has it's own
+implementation of ``useFixture`` so there is no need to use
+``fixtures.TestWithFixtures`` with ``testtools.TestCase``::
 
   >>> class NoddyTest(testtools.TestCase, fixtures.TestWithFixtures):
   ...     def test_example(self):
   ...         fixture = self.useFixture(NoddyFixture())
   ...         self.assertEqual(42, fixture.frobnozzle)
   >>> result = unittest.TestResult()
   >>> _ = NoddyTest('test_example').run(result)
@@ -196,16 +180,16 @@
 Fixtures implement the context protocol, so you can also use a fixture as a
 context manager::
 
   >>> with fixtures.FunctionFixture(setup_function, teardown_function) as fixture:
   ...    print (os.path.isdir(fixture.fn_result))
   True
 
-When multiple cleanups error, fixture.cleanUp() will raise a wrapper exception
-rather than choosing an arbitrary single exception to raise::
+When multiple cleanups error, ``fixture.cleanUp()`` will raise a wrapper
+exception rather than choosing an arbitrary single exception to raise::
 
   >>> import sys
   >>> from fixtures.fixture import MultipleExceptions
   >>> class BrokenFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addCleanup(lambda:1/0)
   ...         self.addCleanup(lambda:1/0)
@@ -216,39 +200,39 @@
   ... except MultipleExceptions:
   ...    exc_info = sys.exc_info()
   >>> print (exc_info[1].args[0][0].__name__)
   ZeroDivisionError
 
 Fixtures often expose diagnostic details that can be useful for tracking down
 issues. The ``getDetails`` method will return a dict of all the attached
-details, but can only be called before ``cleanUp`` is called. Each detail
-object is an instance of ``testtools.content.Content``.
+details but can only be called before ``cleanUp`` is called. Each detail
+object is an instance of ``testtools.content.Content``::
 
   >>> with WithLog() as l:
   ...     print(l.getDetails()['message'].as_text())
   foo bar baz
 
 Errors in setUp
 +++++++++++++++
 
 The examples above used ``_setUp`` rather than ``setUp`` because the base
 class implementation of ``setUp`` acts to reduce the chance of leaking
 external resources if an error is raised from ``_setUp``. Specifically,
-``setUp`` contains a try:/except: block which catches all exceptions, captures
+``setUp`` contains a try/except block which catches all exceptions, captures
 any registered detail objects, and calls ``self.cleanUp`` before propagating
 the error. As long as you take care to register any cleanups before calling
 the code that may fail, this will cause them to be cleaned up. The captured
 detail objects are provided to the args of the raised exception.
 
 If the error that occurred was a subclass of ``Exception`` then ``setUp`` will
 raise ``MultipleExceptions`` with the last element being a ``SetupError`` that
 contains the detail objects. Otherwise, to prevent causing normally
-uncatchable errors like KeyboardInterrupt being caught inappropriately in the
-calling layer, the original exception will be raised as-is and no diagnostic
-data other than that from the original exception will be available.
+uncatchable errors like ``KeyboardInterrupt`` being caught inappropriately in
+the calling layer, the original exception will be raised as-is and no
+diagnostic data other than that from the original exception will be available.
 
 Shared Dependencies
 +++++++++++++++++++
 
 A common use case within complex environments is having some fixtures shared by
 other ones.
 
@@ -294,211 +278,284 @@
 in a tempdir - on Windows this will prevent the directory being deleted).
 
 Another approach which ``fixtures`` neither helps nor hinders is to raise
 a signal of some sort for each user of a fixture before it is reset. In the
 example here, ``TempDir`` might offer a subscribers attribute that both the
 DB and web server would be registered in. Calling ``reset`` or ``cleanUp``
 on the tempdir would trigger a callback to all the subscribers; the DB and
-web server reset methods would look something like:
+web server reset methods would look something like::
 
   >>> def reset(self):
   ...     if not self._cleaned:
   ...         self._clean()
 
 (Their action on the callback from the tempdir would be to do whatever work
 was needed and set ``self._cleaned``.) This approach has the (perhaps)
 surprising effect that resetting the webserver may reset the DB - if the
 webserver were to be depending on ``tempdir.reset`` as a way to reset the
-webservers state.
+webserver's state.
 
 Another approach which is not currently implemented is to provide an object
 graph of dependencies and a reset mechanism that can traverse that, along with
 a separation between 'reset starting' and 'reset finishing' - the DB and
 webserver would both have their ``reset_starting`` methods called, then the
 tempdir would be reset, and finally the DB and webserver would have
 ``reset_finishing`` called.
 
 Stock Fixtures
 ==============
 
-In addition to the Fixture, FunctionFixture and MethodFixture classes fixtures
-includes a number of precanned fixtures. The API docs for fixtures will list
-the complete set of these, should the dcs be out of date or not to hand. For
-the complete feature set of each fixture please see the API docs.
+In addition to the ``Fixture``, ``FunctionFixture`` and ``MethodFixture``
+classes, fixtures includes a number of pre-canned fixtures. The API docs for
+fixtures will list the complete set of these, should the docs be out of date or
+not to hand. For the complete feature set of each fixture please see the API
+docs.
 
-ByteStream
-++++++++++
+``ByteStream``
+++++++++++++++
 
-Trivial adapter to make a BytesIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``BytesIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('my-content')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.something', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-EnvironmentVariable
-+++++++++++++++++++
+``EnvironmentVariable``
++++++++++++++++++++++++
 
 Isolate your code from environmental variables, delete them or set them to a
-new value.
+new value::
 
   >>> fixture = fixtures.EnvironmentVariable('HOME')
 
-FakeLogger
-++++++++++
+``FakeLogger``
+++++++++++++++
 
 Isolate your code from an external logging configuration - so that your test
-gets the output from logged messages, but they don't go to e.g. the console.
+gets the output from logged messages, but they don't go to e.g. the console::
 
   >>> fixture = fixtures.FakeLogger()
 
-FakePopen
-+++++++++
+``FakePopen``
++++++++++++++
 
 Pretend to run an external command rather than needing it to be present to run
-tests.
+tests::
 
   >>> from io import BytesIO
   >>> fixture = fixtures.FakePopen(lambda _:{'stdout': BytesIO('foobar')})
 
-MockPatchObject
-+++++++++++++++
+``LogHandler``
+++++++++++++++
+
+Replace or extend a logger's handlers. The behavior of this fixture depends on
+the value of the ``nuke_handlers`` parameter: if ``true``, the logger's
+existing handlers are removed and replaced by the provided handler, while if
+``false`` the logger's set of handlers is extended by the provided handler::
+
+  >>> from logging import StreamHandler
+  >>> fixture = fixtures.LogHandler(StreamHandler())
 
-Adapts ``mock.patch.object`` to be used as a Fixture.
+``MockPatchObject``
++++++++++++++++++++
+
+Adapts ``mock.patch.object`` to be used as a fixture::
 
   >>> class Fred:
   ...     value = 1
   >>> fixture = fixtures.MockPatchObject(Fred, 'value', 2)
   >>> with fixture:
   ...     Fred().value
   2
   >>> Fred().value
   1
 
-MockPatch
-+++++++++
+``MockPatch``
++++++++++++++
 
-Adapts ``mock.patch`` to be used as a Fixture.
+Adapts ``mock.patch`` to be used as a fixture::
 
   >>> fixture = fixtures.MockPatch('subprocess.Popen.returncode', 3)
 
-MockPatchMultiple
-+++++++++++++++++
+``MockPatchMultiple``
++++++++++++++++++++++
 
-Adapts ``mock.patch.multiple`` to be used as a Fixture.
+Adapts ``mock.patch.multiple`` to be used as a ``fixture``::
 
   >>> fixture = fixtures.MockPatchMultiple('subprocess.Popen', returncode=3)
 
-MonkeyPatch
-+++++++++++
+``MonkeyPatch``
++++++++++++++++
 
-Control the value of a named Python attribute.
+Control the value of a named Python attribute::
 
   >>> def fake_open(path, mode):
   ...     pass
   >>> fixture = fixtures.MonkeyPatch('__builtin__.open', fake_open)
 
 Note that there are some complexities when patching methods - please see the
 API documentation for details.
 
-NestedTempfile
-++++++++++++++
+``NestedTempfile``
+++++++++++++++++++
 
-Change the default directory that the tempfile module places temporary files
-and directories in. This can be useful for containing the noise created by
-code which doesn't clean up its temporary files. This does not affect
-temporary file creation where an explicit containing directory was provided.
+Change the default directory that the ``tempfile`` module places temporary
+files and directories in. This can be useful for containing the noise created
+by code which doesn't clean up its temporary files. This does not affect
+temporary file creation where an explicit containing directory was provided::
 
   >>> fixture = fixtures.NestedTempfile()
 
-PackagePathEntry
-++++++++++++++++
+``PackagePathEntry``
+++++++++++++++++++++
 
 Adds a single directory to the path for an existing Python package. This adds
-to the package.__path__ list. If the directory is already in the path, nothing
-happens, if it isn't then it is added on setUp and removed on cleanUp.
+to the ``package.__path__`` list. If the directory is already in the path,
+nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PackagePathEntry('package/name', '/foo/bar')
 
-PythonPackage
-+++++++++++++
+``PythonPackage``
++++++++++++++++++
 
 Creates a python package directory. Particularly useful for testing code that
 dynamically loads packages/modules, or for mocking out the command line entry
-points to Python programs.
+points to Python programs::
 
   >>> fixture = fixtures.PythonPackage('foo.bar', [('quux.py', '')])
 
-PythonPathEntry
-+++++++++++++++
+``PythonPathEntry``
++++++++++++++++++++
 
-Adds a single directory to sys.path. If the directory is already in the path,
-nothing happens, if it isn't then it is added on setUp and removed on cleanUp.
+Adds a single directory to ``sys.path``. If the directory is already in the
+path, nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PythonPathEntry('/foo/bar')
 
-StringStream
-++++++++++++
+``Stream``
+++++++++++
+
+Trivial adapter to expose a file-like object as a detail object, for automatic
+inclusion in test failure descriptions. ``StringStream`` and ``BytesStream``
+provided concrete users of this fixture.
+
+This requires the ``fixtures[streams]`` extra.
+
+``StringStream``
+++++++++++++++++
 
-Trivial adapter to make a StringIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``StringIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('stdout')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.stdout', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-TempDir
-+++++++
+``TempDir``
++++++++++++
 
-Create a temporary directory and clean it up later.
+Create a temporary directory and clean it up later::
 
   >>> fixture = fixtures.TempDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-TempHomeDir
-+++++++++++
+``TempHomeDir``
++++++++++++++++
 
-Create a temporary directory and set it as $HOME in the environment.
+Create a temporary directory and set it as ``$HOME`` in the environment::
 
   >>> fixture = fixtures.TempHomeDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-The environment will now have $HOME set to the same path, and the value
-will be returned to its previous value after tearDown.
+The environment will now have ``$HOME`` set to the same path, and the value
+will be returned to its previous value after ``tearDown``.
 
-Timeout
-+++++++
+``Timeout``
++++++++++++
 
 Aborts if the covered code takes more than a specified number of whole wall-clock
 seconds.
 
-There are two possibilities, controlled by the 'gentle' argument: when gentle,
+There are two possibilities, controlled by the ``gentle`` argument: when gentle,
 an exception will be raised and the test (or other covered code) will fail.
 When not gentle, the entire process will be terminated, which is less clean,
 but more likely to break hangs where no Python code is running.
 
-*Caution:* Only one timeout can be active at any time across all threads in a
-single process.  Using more than one has undefined results.  (This could be
-improved by chaining alarms.)
+.. caution::
+
+   Only one timeout can be active at any time across all threads in a single
+   process.  Using more than one has undefined results.  (This could be improved
+   by chaining alarms.)
+
+.. note::
+
+   Currently supported only on Unix because it relies on the ``alarm`` system
+   call.
+
+``WarningsCapture``
++++++++++++++++++++
+
+Capture warnings for later analysis::
+
+  >>> fixture = fixtures.WarningsCapture()
+
+The captured warnings are stored in the ``captures`` attribute of the fixture
+after ``setUp``.
 
-*Note:* Currently supported only on Unix because it relies on the ``alarm``
-system call.
+``WarningsFilter``
+++++++++++++++++++
+
+Configure warnings filters during test runs::
+
+  >>> fixture = fixtures.WarningsFilter(
+  ...     [
+  ...         {
+  ...             'action': 'ignore',
+  ...             'message': 'foo',
+  ...             'category': DeprecationWarning,
+  ...         },
+  ...     ]
+  ... )
+
+Order is important: entries closer to the front of the list override entries
+later in the list, if both match a particular warning.
 
 Contributing
 ============
 
 Fixtures has its project homepage on GitHub
 <https://github.com/testing-cabal/fixtures>.
+
+License
+=======
+
+  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
+
+  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
+  license at the users choice. A copy of both licenses are available in the
+  project source as Apache-2.0 and BSD. You may not use this file except in
+  compliance with one of these two licences.
+
+  Unless required by applicable law or agreed to in writing, software
+  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
+  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
+  license you chose for the specific language governing permissions and
+  limitations under that license.
```

### Comparing `fixtures-4.0.1/fixtures/__init__.py` & `fixtures-4.1.0/fixtures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     'StringStream',
     'TempDir',
     'TempHomeDir',
     'TestWithFixtures',
     'Timeout',
     'TimeoutException',
     'WarningsCapture',
+    'WarningsFilter',
     '__version__',
     'version',
     ]
 
 
 from fixtures.fixture import (
     CompoundFixture,
@@ -106,14 +107,15 @@
     PythonPathEntry,
     StringStream,
     TempDir,
     TempHomeDir,
     Timeout,
     TimeoutException,
     WarningsCapture,
+    WarningsFilter,
     )
 from fixtures.testcase import TestWithFixtures
 
 
 def test_suite():
     import fixtures.tests
     return fixtures.tests.test_suite()
```

### Comparing `fixtures-4.0.1/fixtures/_fixtures/__init__.py` & `fixtures-4.1.0/fixtures/_fixtures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     'PythonPathEntry',
     'StringStream',
     'TempDir',
     'TempHomeDir',
     'Timeout',
     'TimeoutException',
     'WarningsCapture',
-    ]
+    'WarningsFilter',
+]
 
 
 from fixtures._fixtures.environ import (
     EnvironmentVariable,
     EnvironmentVariableFixture,
     )
 from fixtures._fixtures.logger import (
@@ -79,8 +80,9 @@
     )
 from fixtures._fixtures.timeout import (
     Timeout,
     TimeoutException,
     )
 from fixtures._fixtures.warnings import (
     WarningsCapture,
+    WarningsFilter,
     )
```

### Comparing `fixtures-4.0.1/fixtures/_fixtures/environ.py` & `fixtures-4.1.0/fixtures/_fixtures/environ.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/logger.py` & `fixtures-4.1.0/fixtures/_fixtures/logger.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/mockpatch.py` & `fixtures-4.1.0/fixtures/_fixtures/mockpatch.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/monkeypatch.py` & `fixtures-4.1.0/fixtures/_fixtures/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/packagepath.py` & `fixtures-4.1.0/fixtures/_fixtures/packagepath.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/popen.py` & `fixtures-4.1.0/fixtures/_fixtures/popen.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/pythonpackage.py` & `fixtures-4.1.0/fixtures/_fixtures/pythonpackage.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/pythonpath.py` & `fixtures-4.1.0/fixtures/_fixtures/pythonpath.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/streams.py` & `fixtures-4.1.0/fixtures/_fixtures/streams.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/tempdir.py` & `fixtures-4.1.0/fixtures/_fixtures/tempdir.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/temphomedir.py` & `fixtures-4.1.0/fixtures/_fixtures/temphomedir.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/_fixtures/timeout.py` & `fixtures-4.1.0/fixtures/_fixtures/timeout.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/callmany.py` & `fixtures-4.1.0/fixtures/callmany.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/fixture.py` & `fixtures-4.1.0/fixtures/fixture.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/testcase.py` & `fixtures-4.1.0/fixtures/testcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import unittest
 
 from fixtures.fixture import gather_details
 
 
 class TestWithFixtures(unittest.TestCase):
     """A TestCase with a helper function to use fixtures.
-    
+
     Normally used as a mix-in class to add useFixture.
 
     Note that test classes such as testtools.TestCase which already have a
     ``useFixture`` method do not need this mixed in.
     """
 
     def useFixture(self, fixture):
```

### Comparing `fixtures-4.0.1/fixtures/tests/__init__.py` & `fixtures-4.1.0/fixtures/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/__init__.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 #  fixtures: Fixtures with cleanups for testing and convenience.
 #
 # Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
-# 
+#
 # Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
 # license at the users choice. A copy of both licenses are available in the
 # project source as Apache-2.0 and BSD. You may not use this file except in
 # compliance with one of these two licences.
-# 
+#
 # Unless required by applicable law or agreed to in writing, software
 # distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # license you chose for the specific language governing permissions and
 # limitations under that license.
 
+import os
+
+
 def load_tests(loader, standard_tests, pattern):
     test_modules = [
-        'environ',
-        'logger',
-        'mockpatch',
-        'monkeypatch',
-        'packagepath',
-        'popen',
-        'pythonpackage',
-        'pythonpath',
-        'streams',
-        'tempdir',
-        'temphomedir',
-        'timeout',
-        ]
-    prefix = "fixtures.tests._fixtures.test_"
+        os.path.splitext(path)[0]
+        for path in os.listdir(os.path.dirname(__file__))
+        if path.startswith('test_')
+    ]
+    prefix = "fixtures.tests._fixtures."
     test_mod_names = [prefix + test_module for test_module in test_modules]
     standard_tests.addTests(loader.loadTestsFromNames(test_mod_names))
     return standard_tests
```

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_environ.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_environ.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_logger.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_logger.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_mockpatch.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_mockpatch.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_monkeypatch.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_packagepath.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_packagepath.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_popen.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_popen.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_pythonpackage.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_pythonpackage.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_pythonpath.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_pythonpath.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_streams.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_streams.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_tempdir.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_temphomedir.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_temphomedir.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/_fixtures/test_timeout.py` & `fixtures-4.1.0/fixtures/tests/_fixtures/test_timeout.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/helpers.py` & `fixtures-4.1.0/fixtures/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/test_callmany.py` & `fixtures-4.1.0/fixtures/tests/test_callmany.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/test_fixture.py` & `fixtures-4.1.0/fixtures/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures/tests/test_testcase.py` & `fixtures-4.1.0/fixtures/tests/test_testcase.py`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/fixtures.egg-info/PKG-INFO` & `fixtures-4.1.0/fixtures.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,175 +1,157 @@
 Metadata-Version: 2.1
 Name: fixtures
-Version: 4.0.1
+Version: 4.1.0
 Summary: Fixtures, reusable state for writing clean tests and more.
 Home-page: https://github.com/testing-cabal/fixtures
 Author: Robert Collins
 Author-email: robertc@robertcollins.net
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Provides-Extra: docs
 Provides-Extra: streams
 Provides-Extra: test
+Provides-Extra: docs
 License-File: COPYING
 
-*************************************************************
-fixtures: Fixtures with cleanups for testing and convenience.
-*************************************************************
-
-  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
-
-  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
-  license at the users choice. A copy of both licenses are available in the
-  project source as Apache-2.0 and BSD. You may not use this file except in
-  compliance with one of these two licences.
+************************************************************
+fixtures: Fixtures with cleanups for testing and convenience
+************************************************************
 
-  Unless required by applicable law or agreed to in writing, software
-  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
-  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
-  license you chose for the specific language governing permissions and
-  limitations under that license.
-
-
-Fixtures defines a Python contract for reusable state / support logic,
+*fixtures* defines a Python contract for reusable state / support logic,
 primarily for unit testing. Helper and adaption logic is included to make it
 easy to write your own fixtures using the fixtures contract. Glue code is
-provided that makes using fixtures that meet the Fixtures contract in unittest
-compatible test cases easy and straight forward.
+provided that makes using fixtures that meet the ``Fixtures`` contract in
+``unittest`` compatible test cases easy and straight forward.
 
 Dependencies
 ============
 
-* Python 3.6+
+* Python 3.7+
   This is the base language fixtures is written in and for.
 
-* pbr
+* ``pbr``
   Used for version and release management of fixtures.
 
 The ``fixtures[streams]`` extra adds:
 
-* testtools <https://launchpad.net/testtools> 0.9.22 or newer.
-  testtools provides helpful glue functions for the details API used to report
+* ``testtools`` <https://launchpad.net/testtools>
+
+  ``testtools`` provides helpful glue functions for the details API used to report
   information about a fixture (whether its used in a testing or production
   environment).
 
-For use in a unit test suite using the included glue, one of:
-
-* bzrlib.tests
-
-* Or any other test environment that supports TestCase.addCleanup.
+For use in a unit test suite using the included glue, you will need a test
+environment that supports ``TestCase.addCleanup``. Writing your own glue code
+is easy. Alternatively, you can simply use Fixtures directly without any
+support code.
 
-Writing your own glue code is easy, or you can simply use Fixtures directly
-without any support code.
-
-To run the test suite for fixtures, testtools is needed.
+To run the test suite for fixtures, ``testtools`` is needed.
 
 Why Fixtures
 ============
 
-Standard Python unittest.py provides no obvious method for making and reusing
+Standard Python ``unittest`` provides no obvious method for making and reusing
 state needed in a test case other than by adding a method on the test class.
 This scales poorly - complex helper functions propagating up a test class
-hierarchy is a regular pattern when this is done. Mocking while a great tool
+hierarchy is a regular pattern when this is done. Mocking, while a great tool,
 doesn't itself prevent this (and helpers to mock complex things can accumulate
 in the same way if placed on the test class).
 
 By defining a uniform contract where helpers have no dependency on the test
 class we permit all the regular code hygiene activities to take place without
 the distorting influence of being in a class hierarchy that is modelling an
-entirely different thing - which is what helpers on a TestCase suffer from.
+entirely different thing - which is what helpers on a ``TestCase`` suffer from.
 
 About Fixtures
 ==============
 
-A Fixture represents some state. Each fixture has attributes on it that are
+A fixture represents some state. Each fixture has attributes on it that are
 specific to the fixture. For instance, a fixture representing a directory that
-can be used for temporary files might have a attribute 'path'.
+can be used for temporary files might have a attribute ``path``.
 
 Most fixtures have complete ``pydoc`` documentation, so be sure to check
 ``pydoc fixtures`` for usage information.
 
 Creating Fixtures
 =================
 
-Minimally, subclass Fixture, define _setUp to initialize your state and schedule
-a cleanup for when cleanUp is called and you're done::
+Minimally, subclass ``Fixture``, define ``_setUp`` to initialize your state,
+schedule a cleanup for when ``cleanUp`` is called, and you're done::
 
   >>> import unittest
   >>> import fixtures
   >>> class NoddyFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.frobnozzle = 42
   ...         self.addCleanup(delattr, self, 'frobnozzle')
 
-This will initialize frobnozzle when ``setUp`` is called, and when ``cleanUp``
-is called get rid of the frobnozzle attribute. Prior to version 1.3.0 fixtures
-recommended overriding ``setUp``. This is still supported, but since it is
-harder to write leak-free fixtures in this fashion, it is not recommended.
+This will initialize ``frobnozzle`` when ``setUp`` is called, and when
+``cleanUp`` is called get rid of the ``frobnozzle`` attribute. Prior to version
+1.3.0 *fixtures* recommended overriding ``setUp``. This is still supported, but
+since it is harder to write leak-free fixtures in this fashion, it is not
+recommended.
 
 If your fixture has diagnostic data - for instance the log file of an
-application server, or log messages, it can expose that by creating a content
-object (``testtools.content.Content``) and calling ``addDetail``.
+application server, or log messages - it can expose that by creating a content
+object (``testtools.content.Content``) and calling ``addDetail``::
 
   >>> from testtools.content import text_content
   >>> class WithLog(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addDetail('message', text_content('foo bar baz'))
 
 The method ``useFixture`` will use another fixture, call ``setUp`` on it, call
 ``self.addCleanup(thefixture.cleanUp)``, attach any details from it and return
-the fixture. This allows simple composition of different fixtures.
+the fixture. This allows simple composition of different fixtures::
 
   >>> class ReusingFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.noddy = self.useFixture(NoddyFixture())
 
-There is a helper for adapting a function or function pair into Fixtures. it
-puts the result of the function in fn_result::
+There is a helper for adapting a function or function pair into Fixtures. It
+puts the result of the function in ``fn_result``::
 
   >>> import os.path
   >>> import shutil
   >>> import tempfile
   >>> def setup_function():
   ...     return tempfile.mkdtemp()
   >>> def teardown_function(fixture):
   ...     shutil.rmtree(fixture)
   >>> fixture = fixtures.FunctionFixture(setup_function, teardown_function)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-This can be expressed even more pithily:
+This can be expressed even more pithily::
 
   >>> fixture = fixtures.FunctionFixture(tempfile.mkdtemp, shutil.rmtree)
   >>> fixture.setUp()
   >>> print (os.path.isdir(fixture.fn_result))
   True
   >>> fixture.cleanUp()
 
-Another variation is MethodFixture which is useful for adapting alternate
+Another variation is ``MethodFixture`` which is useful for adapting alternate
 fixture implementations to Fixture::
 
   >>> class MyServer:
   ...    def start(self):
   ...        pass
   ...    def stop(self):
   ...        pass
@@ -183,42 +165,42 @@
   >>> with noddy_with_log as x:
   ...     print (x.fixtures[0].frobnozzle)
   42
 
 The Fixture API
 ===============
 
-The example above introduces some of the Fixture API. In order to be able to
-clean up after a fixture has been used, all fixtures define a ``cleanUp``
+The example above introduces some of the ``Fixture`` API. In order to be able
+to clean up after a fixture has been used, all fixtures define a ``cleanUp``
 method which should be called when a fixture is finished with.
 
 Because it's nice to be able to build a particular set of related fixtures in
 advance of using them, fixtures also have a ``setUp`` method which should be
 called before trying to use them.
 
 One common desire with fixtures that are expensive to create is to reuse them
-in many test cases; to support this the base Fixture also defines a ``reset``
-which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
+in many test cases; to support this the base ``Fixture`` also defines a
+``reset`` which calls ``self.cleanUp(); self.setUp()``. Fixtures that can more
 efficiently make themselves reusable should override this method. This can then
 be used with multiple test state via things like ``testresources``,
 ``setUpClass``, or ``setUpModule``.
 
-When using a fixture with a test you can manually call the setUp and cleanUp
-methods. More convenient though is to use the included glue from
-``fixtures.TestWithFixtures`` which provides a mixin defining
-``useFixture`` (camel case because unittest is camel case throughout) method.
-It will call setUp on the fixture, call self.addCleanup(fixture) to schedule a
+When using a fixture with a test you can manually call the ``setUp`` and
+``cleanUp`` methods. More convenient though is to use the included glue from
+``fixtures.TestWithFixtures`` which provides a mixin defining ``useFixture``
+(camel case because ``unittest`` is camel case throughout) method. It will call
+``setUp`` on the fixture, call ``self.addCleanup(fixture)`` to schedule a
 cleanup, and return the fixture. This lets one write::
 
   >>> import testtools
   >>> import unittest
 
-Note that we use ``testtools.TestCase``. testtools has it's own implementation
-of ``useFixture`` so there is no need to use ``fixtures.TestWithFixtures`` with
-``testtools.TestCase``.
+Note that we use ``testtools.TestCase``. ``testtools`` has it's own
+implementation of ``useFixture`` so there is no need to use
+``fixtures.TestWithFixtures`` with ``testtools.TestCase``::
 
   >>> class NoddyTest(testtools.TestCase, fixtures.TestWithFixtures):
   ...     def test_example(self):
   ...         fixture = self.useFixture(NoddyFixture())
   ...         self.assertEqual(42, fixture.frobnozzle)
   >>> result = unittest.TestResult()
   >>> _ = NoddyTest('test_example').run(result)
@@ -228,16 +210,16 @@
 Fixtures implement the context protocol, so you can also use a fixture as a
 context manager::
 
   >>> with fixtures.FunctionFixture(setup_function, teardown_function) as fixture:
   ...    print (os.path.isdir(fixture.fn_result))
   True
 
-When multiple cleanups error, fixture.cleanUp() will raise a wrapper exception
-rather than choosing an arbitrary single exception to raise::
+When multiple cleanups error, ``fixture.cleanUp()`` will raise a wrapper
+exception rather than choosing an arbitrary single exception to raise::
 
   >>> import sys
   >>> from fixtures.fixture import MultipleExceptions
   >>> class BrokenFixture(fixtures.Fixture):
   ...     def _setUp(self):
   ...         self.addCleanup(lambda:1/0)
   ...         self.addCleanup(lambda:1/0)
@@ -248,39 +230,39 @@
   ... except MultipleExceptions:
   ...    exc_info = sys.exc_info()
   >>> print (exc_info[1].args[0][0].__name__)
   ZeroDivisionError
 
 Fixtures often expose diagnostic details that can be useful for tracking down
 issues. The ``getDetails`` method will return a dict of all the attached
-details, but can only be called before ``cleanUp`` is called. Each detail
-object is an instance of ``testtools.content.Content``.
+details but can only be called before ``cleanUp`` is called. Each detail
+object is an instance of ``testtools.content.Content``::
 
   >>> with WithLog() as l:
   ...     print(l.getDetails()['message'].as_text())
   foo bar baz
 
 Errors in setUp
 +++++++++++++++
 
 The examples above used ``_setUp`` rather than ``setUp`` because the base
 class implementation of ``setUp`` acts to reduce the chance of leaking
 external resources if an error is raised from ``_setUp``. Specifically,
-``setUp`` contains a try:/except: block which catches all exceptions, captures
+``setUp`` contains a try/except block which catches all exceptions, captures
 any registered detail objects, and calls ``self.cleanUp`` before propagating
 the error. As long as you take care to register any cleanups before calling
 the code that may fail, this will cause them to be cleaned up. The captured
 detail objects are provided to the args of the raised exception.
 
 If the error that occurred was a subclass of ``Exception`` then ``setUp`` will
 raise ``MultipleExceptions`` with the last element being a ``SetupError`` that
 contains the detail objects. Otherwise, to prevent causing normally
-uncatchable errors like KeyboardInterrupt being caught inappropriately in the
-calling layer, the original exception will be raised as-is and no diagnostic
-data other than that from the original exception will be available.
+uncatchable errors like ``KeyboardInterrupt`` being caught inappropriately in
+the calling layer, the original exception will be raised as-is and no
+diagnostic data other than that from the original exception will be available.
 
 Shared Dependencies
 +++++++++++++++++++
 
 A common use case within complex environments is having some fixtures shared by
 other ones.
 
@@ -326,214 +308,285 @@
 in a tempdir - on Windows this will prevent the directory being deleted).
 
 Another approach which ``fixtures`` neither helps nor hinders is to raise
 a signal of some sort for each user of a fixture before it is reset. In the
 example here, ``TempDir`` might offer a subscribers attribute that both the
 DB and web server would be registered in. Calling ``reset`` or ``cleanUp``
 on the tempdir would trigger a callback to all the subscribers; the DB and
-web server reset methods would look something like:
+web server reset methods would look something like::
 
   >>> def reset(self):
   ...     if not self._cleaned:
   ...         self._clean()
 
 (Their action on the callback from the tempdir would be to do whatever work
 was needed and set ``self._cleaned``.) This approach has the (perhaps)
 surprising effect that resetting the webserver may reset the DB - if the
 webserver were to be depending on ``tempdir.reset`` as a way to reset the
-webservers state.
+webserver's state.
 
 Another approach which is not currently implemented is to provide an object
 graph of dependencies and a reset mechanism that can traverse that, along with
 a separation between 'reset starting' and 'reset finishing' - the DB and
 webserver would both have their ``reset_starting`` methods called, then the
 tempdir would be reset, and finally the DB and webserver would have
 ``reset_finishing`` called.
 
 Stock Fixtures
 ==============
 
-In addition to the Fixture, FunctionFixture and MethodFixture classes fixtures
-includes a number of precanned fixtures. The API docs for fixtures will list
-the complete set of these, should the dcs be out of date or not to hand. For
-the complete feature set of each fixture please see the API docs.
+In addition to the ``Fixture``, ``FunctionFixture`` and ``MethodFixture``
+classes, fixtures includes a number of pre-canned fixtures. The API docs for
+fixtures will list the complete set of these, should the docs be out of date or
+not to hand. For the complete feature set of each fixture please see the API
+docs.
 
-ByteStream
-++++++++++
+``ByteStream``
+++++++++++++++
 
-Trivial adapter to make a BytesIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``BytesIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('my-content')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.something', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-EnvironmentVariable
-+++++++++++++++++++
+``EnvironmentVariable``
++++++++++++++++++++++++
 
 Isolate your code from environmental variables, delete them or set them to a
-new value.
+new value::
 
   >>> fixture = fixtures.EnvironmentVariable('HOME')
 
-FakeLogger
-++++++++++
+``FakeLogger``
+++++++++++++++
 
 Isolate your code from an external logging configuration - so that your test
-gets the output from logged messages, but they don't go to e.g. the console.
+gets the output from logged messages, but they don't go to e.g. the console::
 
   >>> fixture = fixtures.FakeLogger()
 
-FakePopen
-+++++++++
+``FakePopen``
++++++++++++++
 
 Pretend to run an external command rather than needing it to be present to run
-tests.
+tests::
 
   >>> from io import BytesIO
   >>> fixture = fixtures.FakePopen(lambda _:{'stdout': BytesIO('foobar')})
 
-MockPatchObject
-+++++++++++++++
+``LogHandler``
+++++++++++++++
 
-Adapts ``mock.patch.object`` to be used as a Fixture.
+Replace or extend a logger's handlers. The behavior of this fixture depends on
+the value of the ``nuke_handlers`` parameter: if ``true``, the logger's
+existing handlers are removed and replaced by the provided handler, while if
+``false`` the logger's set of handlers is extended by the provided handler::
+
+  >>> from logging import StreamHandler
+  >>> fixture = fixtures.LogHandler(StreamHandler())
+
+``MockPatchObject``
++++++++++++++++++++
+
+Adapts ``mock.patch.object`` to be used as a fixture::
 
   >>> class Fred:
   ...     value = 1
   >>> fixture = fixtures.MockPatchObject(Fred, 'value', 2)
   >>> with fixture:
   ...     Fred().value
   2
   >>> Fred().value
   1
 
-MockPatch
-+++++++++
+``MockPatch``
++++++++++++++
 
-Adapts ``mock.patch`` to be used as a Fixture.
+Adapts ``mock.patch`` to be used as a fixture::
 
   >>> fixture = fixtures.MockPatch('subprocess.Popen.returncode', 3)
 
-MockPatchMultiple
-+++++++++++++++++
+``MockPatchMultiple``
++++++++++++++++++++++
 
-Adapts ``mock.patch.multiple`` to be used as a Fixture.
+Adapts ``mock.patch.multiple`` to be used as a ``fixture``::
 
   >>> fixture = fixtures.MockPatchMultiple('subprocess.Popen', returncode=3)
 
-MonkeyPatch
-+++++++++++
+``MonkeyPatch``
++++++++++++++++
 
-Control the value of a named Python attribute.
+Control the value of a named Python attribute::
 
   >>> def fake_open(path, mode):
   ...     pass
   >>> fixture = fixtures.MonkeyPatch('__builtin__.open', fake_open)
 
 Note that there are some complexities when patching methods - please see the
 API documentation for details.
 
-NestedTempfile
-++++++++++++++
+``NestedTempfile``
+++++++++++++++++++
 
-Change the default directory that the tempfile module places temporary files
-and directories in. This can be useful for containing the noise created by
-code which doesn't clean up its temporary files. This does not affect
-temporary file creation where an explicit containing directory was provided.
+Change the default directory that the ``tempfile`` module places temporary
+files and directories in. This can be useful for containing the noise created
+by code which doesn't clean up its temporary files. This does not affect
+temporary file creation where an explicit containing directory was provided::
 
   >>> fixture = fixtures.NestedTempfile()
 
-PackagePathEntry
-++++++++++++++++
+``PackagePathEntry``
+++++++++++++++++++++
 
 Adds a single directory to the path for an existing Python package. This adds
-to the package.__path__ list. If the directory is already in the path, nothing
-happens, if it isn't then it is added on setUp and removed on cleanUp.
+to the ``package.__path__`` list. If the directory is already in the path,
+nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PackagePathEntry('package/name', '/foo/bar')
 
-PythonPackage
-+++++++++++++
+``PythonPackage``
++++++++++++++++++
 
 Creates a python package directory. Particularly useful for testing code that
 dynamically loads packages/modules, or for mocking out the command line entry
-points to Python programs.
+points to Python programs::
 
   >>> fixture = fixtures.PythonPackage('foo.bar', [('quux.py', '')])
 
-PythonPathEntry
-+++++++++++++++
+``PythonPathEntry``
++++++++++++++++++++
 
-Adds a single directory to sys.path. If the directory is already in the path,
-nothing happens, if it isn't then it is added on setUp and removed on cleanUp.
+Adds a single directory to ``sys.path``. If the directory is already in the
+path, nothing happens, if it isn't then it is added on ``setUp`` and removed on
+``cleanUp``::
 
   >>> fixture = fixtures.PythonPathEntry('/foo/bar')
 
-StringStream
-++++++++++++
+``Stream``
+++++++++++
+
+Trivial adapter to expose a file-like object as a detail object, for automatic
+inclusion in test failure descriptions. ``StringStream`` and ``BytesStream``
+provided concrete users of this fixture.
+
+This requires the ``fixtures[streams]`` extra.
+
+``StringStream``
+++++++++++++++++
 
-Trivial adapter to make a StringIO (though it may in future auto-spill to disk
-for large content) and expose that as a detail object, for automatic inclusion
-in test failure descriptions. Very useful in combination with MonkeyPatch.
+Trivial adapter to make a ``StringIO`` (though it may in future auto-spill to
+disk for large content) and expose that as a detail object, for automatic
+inclusion in test failure descriptions. Very useful in combination with
+``MonkeyPatch``::
 
   >>> fixture = fixtures.StringStream('stdout')
   >>> fixture.setUp()
   >>> with fixtures.MonkeyPatch('sys.stdout', fixture.stream):
   ...     pass
   >>> fixture.cleanUp()
 
 This requires the ``fixtures[streams]`` extra.
 
-TempDir
-+++++++
+``TempDir``
++++++++++++
 
-Create a temporary directory and clean it up later.
+Create a temporary directory and clean it up later::
 
   >>> fixture = fixtures.TempDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-TempHomeDir
-+++++++++++
+``TempHomeDir``
++++++++++++++++
 
-Create a temporary directory and set it as $HOME in the environment.
+Create a temporary directory and set it as ``$HOME`` in the environment::
 
   >>> fixture = fixtures.TempHomeDir()
 
 The created directory is stored in the ``path`` attribute of the fixture after
-setUp.
+``setUp``.
 
-The environment will now have $HOME set to the same path, and the value
-will be returned to its previous value after tearDown.
+The environment will now have ``$HOME`` set to the same path, and the value
+will be returned to its previous value after ``tearDown``.
 
-Timeout
-+++++++
+``Timeout``
++++++++++++
 
 Aborts if the covered code takes more than a specified number of whole wall-clock
 seconds.
 
-There are two possibilities, controlled by the 'gentle' argument: when gentle,
+There are two possibilities, controlled by the ``gentle`` argument: when gentle,
 an exception will be raised and the test (or other covered code) will fail.
 When not gentle, the entire process will be terminated, which is less clean,
 but more likely to break hangs where no Python code is running.
 
-*Caution:* Only one timeout can be active at any time across all threads in a
-single process.  Using more than one has undefined results.  (This could be
-improved by chaining alarms.)
+.. caution::
+
+   Only one timeout can be active at any time across all threads in a single
+   process.  Using more than one has undefined results.  (This could be improved
+   by chaining alarms.)
+
+.. note::
+
+   Currently supported only on Unix because it relies on the ``alarm`` system
+   call.
 
-*Note:* Currently supported only on Unix because it relies on the ``alarm``
-system call.
+``WarningsCapture``
++++++++++++++++++++
+
+Capture warnings for later analysis::
+
+  >>> fixture = fixtures.WarningsCapture()
+
+The captured warnings are stored in the ``captures`` attribute of the fixture
+after ``setUp``.
+
+``WarningsFilter``
+++++++++++++++++++
+
+Configure warnings filters during test runs::
+
+  >>> fixture = fixtures.WarningsFilter(
+  ...     [
+  ...         {
+  ...             'action': 'ignore',
+  ...             'message': 'foo',
+  ...             'category': DeprecationWarning,
+  ...         },
+  ...     ]
+  ... )
+
+Order is important: entries closer to the front of the list override entries
+later in the list, if both match a particular warning.
 
 Contributing
 ============
 
 Fixtures has its project homepage on GitHub
 <https://github.com/testing-cabal/fixtures>.
 
+License
+=======
+
+  Copyright (c) 2010, Robert Collins <robertc@robertcollins.net>
+
+  Licensed under either the Apache License, Version 2.0 or the BSD 3-clause
+  license at the users choice. A copy of both licenses are available in the
+  project source as Apache-2.0 and BSD. You may not use this file except in
+  compliance with one of these two licences.
 
+  Unless required by applicable law or agreed to in writing, software
+  distributed under these licenses is distributed on an "AS IS" BASIS, WITHOUT
+  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
+  license you chose for the specific language governing permissions and
+  limitations under that license.
```

### Comparing `fixtures-4.0.1/fixtures.egg-info/SOURCES.txt` & `fixtures-4.1.0/fixtures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixtures-4.0.1/setup.cfg` & `fixtures-4.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 summary = Fixtures, reusable state for writing clean tests and more.
 description_file = 
 	README.rst
 description_content_type = text/x-rst; charset=UTF-8
 author = Robert Collins
 author_email = robertc@robertcollins.net
 url = https://github.com/testing-cabal/fixtures
-python_requires = >=3.6
+python_requires = >=3.7
 classifiers = 
 	Development Status :: 6 - Mature
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development :: Quality Assurance
 	Topic :: Software Development :: Testing
 
 [files]
 packages =
```


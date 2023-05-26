# Comparing `tmp/vmklib-1.8.1.tar.gz` & `tmp/vmklib-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmklib-1.8.1.tar", last modified: Sat Apr  8 01:24:18 2023, max compression
+gzip compressed data, was "vmklib-1.8.2.tar", last modified: Fri May 26 06:27:21 2023, max compression
```

## Comparing `vmklib-1.8.1.tar` & `vmklib-1.8.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 01:22:01.000000 vmklib-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-08 01:24:18.800661 vmklib-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-08 01:22:01.000000 vmklib-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-08 01:22:01.000000 vmklib-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 01:24:18.800661 vmklib-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-08 01:22:01.000000 vmklib-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.788661 vmklib-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-08 01:22:01.000000 vmklib-1.8.1/tests/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.792661 vmklib-1.8.1/vmklib/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/conf.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/edit_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/fresh_venv.txt
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/data/header.mk
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/datazen.mk
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/functions.mk
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/grip.mk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/lib_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/lib_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-08 01:22:12.000000 vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/lib_tasks/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/build.mk
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/docs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/pypi.mk
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python/upload.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/python.mk
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/time.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/venv.mk
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/vmklib.mk
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/data/yaml.mk
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.796661 vmklib-1.8.1/vmklib/tasks/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/mixins/concrete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/vmklib/tasks/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.800661 vmklib-1.8.1/vmklib/tasks/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/datazen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/python/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-08 01:22:01.000000 vmklib-1.8.1/vmklib/tasks/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 01:24:18.792661 vmklib-1.8.1/vmklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 01:24:18.000000 vmklib-1.8.1/vmklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 06:24:48.000000 vmklib-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-26 06:27:21.115979 vmklib-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-26 06:24:48.000000 vmklib-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-26 06:24:48.000000 vmklib-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:27:21.115979 vmklib-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 06:24:48.000000 vmklib-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.111978 vmklib-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-26 06:24:48.000000 vmklib-1.8.2/tests/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.111978 vmklib-1.8.2/vmklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/conf.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/data/edit_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/data/fresh_venv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/data/header.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/datazen.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/functions.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/grip.mk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/data/lib_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/lib_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/data/lib_tasks/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-26 06:25:04.000000 vmklib-1.8.2/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/lib_tasks/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/python/build.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/python/docs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/python/pypi.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/python/upload.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/python.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/time.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/venv.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/vmklib.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/data/yaml.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/tasks/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/mixins/concrete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/tasks/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.115979 vmklib-1.8.2/vmklib/tasks/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/datazen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/python/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-26 06:24:48.000000 vmklib-1.8.2/vmklib/tasks/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:27:21.111978 vmklib-1.8.2/vmklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 06:27:21.000000 vmklib-1.8.2/vmklib.egg-info/top_level.txt
```

### Comparing `vmklib-1.8.1/LICENSE` & `vmklib-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/PKG-INFO` & `vmklib-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.1
+Version: 1.8.2
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -46,19 +46,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=86cb90c0ad730eedd704cb4110084afd
+    hash=260b3eb9b8e7e42878fb12193e72a3cd
     =====================================
 -->
 
-# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.2](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -109,34 +109,37 @@
 * [vmklib](#vmklib)
 * [yaml](#yaml)
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/mk -h
+$ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-f FILE]
-          [-c CONFIG] [-P PROJ]
-          [targets [targets ...]]
+usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
+          [-f FILE] [-c CONFIG] [-P PROJ]
+          [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
+  -D DEFAULT, --default DEFAULT
+                        default target to make if none is specified (default:
+                        'all')
   -f FILE, --file FILE  file to source user-provided recipes from (default:
                         'Makefile')
   -c CONFIG, --config CONFIG
                         file to source user-provided variable definitions,
                         ahead of loading package makefiles (default:
                         'vmklib.json')
   -P PROJ, --proj PROJ  project name for internal variable use
```

### Comparing `vmklib-1.8.1/README.md` & `vmklib-1.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=86cb90c0ad730eedd704cb4110084afd
+    hash=260b3eb9b8e7e42878fb12193e72a3cd
     =====================================
 -->
 
-# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.2](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -61,34 +61,37 @@
 * [vmklib](#vmklib)
 * [yaml](#yaml)
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/mk -h
+$ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-f FILE]
-          [-c CONFIG] [-P PROJ]
-          [targets [targets ...]]
+usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
+          [-f FILE] [-c CONFIG] [-P PROJ]
+          [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
+  -D DEFAULT, --default DEFAULT
+                        default target to make if none is specified (default:
+                        'all')
   -f FILE, --file FILE  file to source user-provided recipes from (default:
                         'Makefile')
   -c CONFIG, --config CONFIG
                         file to source user-provided variable definitions,
                         ahead of loading package makefiles (default:
                         'vmklib.json')
   -P PROJ, --proj PROJ  project name for internal variable use
```

### Comparing `vmklib-1.8.1/pyproject.toml` & `vmklib-1.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vmklib"
-version = "1.8.1"
+version = "1.8.2"
 description = "Simplify project workflows by standardizing use of GNU Make."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
   "workflow",
   "tool",
@@ -34,13 +34,20 @@
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = [
+  "pylint",
+  "flake8",
+  "black",
+  "ruff",
+  "mypy",
+  "isort",
+  "yamllint",
   "pytest-asyncio",
   "setuptools-wrapper"
 ]
 
 [project.scripts]
 mk = "vmklib.entry:main"
```

### Comparing `vmklib-1.8.1/setup.py` & `vmklib-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/tests/test_entry.py` & `vmklib-1.8.2/tests/test_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,22 +44,26 @@
             good_base_args = base_args + ["-f", get_resource("Makefile")]
             assert mk_main(good_base_args + ["test"]) == 0
             assert mk_main(good_base_args + ["--proj", "test", "test"]) == 0
             assert mk_main(good_base_args + ["-p", "prefix", "test"]) == 0
             assert mk_main(good_base_args + ["test_bad"]) != 0
             assert mk_main(good_base_args + ["--weird-option", "yo"]) != 0
             assert mk_main(base_args + ["-f", "nah"]) != 0
-            assert mk_main(base_args) == 0
+
+            assert mk_main(good_base_args) == 0
+
+            # Shouldn't be able to resolve the default target.
+            assert mk_main(base_args) != 0
 
 
 def test_package_entry():
     """Test the command-line entry through the 'python -m' invocation."""
 
     with get_args() as base_args:
-        args = [executable, "-m"] + base_args
+        args = [executable, "-m"] + base_args + ["--default", ""]
         check_output(args)
 
 
 def test_entry_proj_slug():
     """Ensure that the slug-replacement logic takes effect."""
 
     if not is_windows():
```

### Comparing `vmklib-1.8.1/vmklib/app.py` & `vmklib-1.8.2/vmklib/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,18 @@
 
     if not args.file.is_file():
         if args.file.name != str(DEFAULT_FILE):
             LOG.error("'%s' not found", args.file)
             return 1
         args.file = get_resource(os.path.join("data", "header.mk"))
 
+    # Add the default target early if nothing was specified.
+    if not args.targets and args.default:
+        args.targets.append(args.default)
+
     # load configuration data, if configuration data is found
     substitutions, targets = get_data(args.config, args.targets, args.prefix)
 
     proj = project(args.dir, args.proj)
     task_register = os.path.join("tasks", "conf.py")
 
     manager = TaskManager()
@@ -232,14 +236,23 @@
         action="store_true",
         help=(
             "whether or not to allow GNU Make "
             "target resolution (default: '%(default)s')"
         ),
     )
     parser.add_argument(
+        "-D",
+        "--default",
+        default="all",
+        help=(
+            "default target to make if none is "
+            "specified (default: '%(default)s')"
+        ),
+    )
+    parser.add_argument(
         "-f",
         "--file",
         default=DEFAULT_FILE,
         type=Path,
         help=(
             "file to source user-provided recipes from "
             "(default: '%(default)s')"
```

### Comparing `vmklib-1.8.1/vmklib/data/conf.mk` & `vmklib-1.8.2/vmklib/data/conf.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/data/header.mk` & `vmklib-1.8.2/vmklib/data/data/header.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/datazen.mk` & `vmklib-1.8.2/vmklib/data/datazen.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/functions.mk` & `vmklib-1.8.2/vmklib/data/functions.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/grip.mk` & `vmklib-1.8.2/vmklib/data/grip.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc` & `vmklib-1.8.2/vmklib/data/lib_tasks/__pycache__/conf.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Apr  8 01:22:01 2023 UTC, .py size: 2374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b9c1 3064 4609 0000  U.........0dF...
+00000000: 550d 0d0a 0000 0000 b050 7064 4609 0000  U........PpdF...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 0201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `vmklib-1.8.1/vmklib/data/lib_tasks/conf.py` & `vmklib-1.8.2/vmklib/data/lib_tasks/conf.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/python/build.mk` & `vmklib-1.8.2/vmklib/data/python/build.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/python/docs.mk` & `vmklib-1.8.2/vmklib/data/python/docs.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/python/pypi.mk` & `vmklib-1.8.2/vmklib/data/python/pypi.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/python/upload.mk` & `vmklib-1.8.2/vmklib/data/python/upload.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/python.mk` & `vmklib-1.8.2/vmklib/data/python.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/time.mk` & `vmklib-1.8.2/vmklib/data/time.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/venv.mk` & `vmklib-1.8.2/vmklib/data/venv.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/data/vmklib.mk` & `vmklib-1.8.2/vmklib/data/vmklib.mk`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/entry.py` & `vmklib-1.8.2/vmklib/entry.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/resources.py` & `vmklib-1.8.2/vmklib/resources.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/args.py` & `vmklib-1.8.2/vmklib/tasks/args.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/mixins/concrete.py` & `vmklib-1.8.2/vmklib/tasks/mixins/concrete.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/node/__init__.py` & `vmklib-1.8.2/vmklib/tasks/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/__init__.py` & `vmklib-1.8.2/vmklib/tasks/python/__init__.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/build.py` & `vmklib-1.8.2/vmklib/tasks/python/build.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/datazen.py` & `vmklib-1.8.2/vmklib/tasks/python/datazen.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/docs.py` & `vmklib-1.8.2/vmklib/tasks/python/docs.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/lint.py` & `vmklib-1.8.2/vmklib/tasks/python/lint.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/package.py` & `vmklib-1.8.2/vmklib/tasks/python/package.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/sa.py` & `vmklib-1.8.2/vmklib/tasks/python/sa.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/test.py` & `vmklib-1.8.2/vmklib/tasks/python/test.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/python/yaml.py` & `vmklib-1.8.2/vmklib/tasks/python/yaml.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib/tasks/venv.py` & `vmklib-1.8.2/vmklib/tasks/venv.py`

 * *Files identical despite different names*

### Comparing `vmklib-1.8.1/vmklib.egg-info/PKG-INFO` & `vmklib-1.8.2/vmklib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmklib
-Version: 1.8.1
+Version: 1.8.2
 Summary: Simplify project workflows by standardizing use of GNU Make.
 Home-page: https://github.com/vkottler/vmklib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 License: MIT License
         
@@ -46,19 +46,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=86cb90c0ad730eedd704cb4110084afd
+    hash=260b3eb9b8e7e42878fb12193e72a3cd
     =====================================
 -->
 
-# vmklib ([1.8.1](https://pypi.org/project/vmklib/))
+# vmklib ([1.8.2](https://pypi.org/project/vmklib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vmklib.svg)](https://pypi.org/project/vmklib/)
 ![Build Status](https://github.com/vkottler/vmklib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vmklib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vmklib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vmklib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vmklib)
 
@@ -109,34 +109,37 @@
 * [vmklib](#vmklib)
 * [yaml](#yaml)
 * [Dependency Graph](#dependency-graph)
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/mk -h
+$ ./venv3.11/bin/mk -h
 
-usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-f FILE]
-          [-c CONFIG] [-P PROJ]
-          [targets [targets ...]]
+usage: mk [-h] [--version] [-v] [-C DIR] [-p PREFIX] [-d] [-D DEFAULT]
+          [-f FILE] [-c CONFIG] [-P PROJ]
+          [targets ...]
 
 Simplify project workflows by standardizing use of GNU Make.
 
 positional arguments:
   targets               targets to execute
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
   -p PREFIX, --prefix PREFIX
                         a prefix to apply to all targets
   -d, --disable-make    whether or not to allow GNU Make target resolution
                         (default: 'False')
+  -D DEFAULT, --default DEFAULT
+                        default target to make if none is specified (default:
+                        'all')
   -f FILE, --file FILE  file to source user-provided recipes from (default:
                         'Makefile')
   -c CONFIG, --config CONFIG
                         file to source user-provided variable definitions,
                         ahead of loading package makefiles (default:
                         'vmklib.json')
   -P PROJ, --proj PROJ  project name for internal variable use
```

### Comparing `vmklib-1.8.1/vmklib.egg-info/SOURCES.txt` & `vmklib-1.8.2/vmklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


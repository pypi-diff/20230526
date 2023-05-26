# Comparing `tmp/treevalue-1.4.8.tar.gz` & `tmp/treevalue-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treevalue-1.4.8.tar", last modified: Mon Mar  6 16:34:40 2023, max compression
+gzip compressed data, was "treevalue-1.4.9.tar", last modified: Mon Mar  6 18:29:03 2023, max compression
```

## Comparing `treevalue-1.4.8.tar` & `treevalue-1.4.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.771023 treevalue-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-06 16:34:02.000000 treevalue-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-06 16:34:02.000000 treevalue-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    20434 2023-03-06 16:34:40.771023 treevalue-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19415 2023-03-06 16:34:02.000000 treevalue-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-03-06 16:34:02.000000 treevalue-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-benchmark.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-potc.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-test-extra.txt
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-06 16:34:02.000000 treevalue-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-06 16:34:40.771023 treevalue-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-03-06 16:34:02.000000 treevalue-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/entry/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/entry/cli/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/entry/script/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/entry/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/tree/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue/tree/common/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/base.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/base.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/delay.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/delay.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1655 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/storage.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    11078 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/common/storage.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.767023 treevalue-1.4.8/treevalue/tree/func/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/cfunc.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    11566 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/cfunc.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    10041 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/func.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/modes.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/func/modes.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.767023 treevalue-1.4.8/treevalue/tree/general/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/general/fast.py
--rw-r--r--   0 runner    (1001) docker     (122)    50264 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/general/general.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.767023 treevalue-1.4.8/treevalue/tree/integration/
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/base.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/base.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/cjax.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/cjax.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/ctorch.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/ctorch.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      915 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/general.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     9214 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/general.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/jax.py
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/integration/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.767023 treevalue-1.4.8/treevalue/tree/tree/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/constraint.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/constraint.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/flatten.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/flatten.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/functional.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     9418 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/functional.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     7010 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/io.py
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/service.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/service.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/structural.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    17724 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/structural.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2644 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/tree.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    39761 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/tree/tree/tree.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.767023 treevalue-1.4.8/treevalue/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15309 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/utils/formattree.py
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (122)     7371 2023-03-06 16:34:02.000000 treevalue-1.4.8/treevalue/utils/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:34:40.763023 treevalue-1.4.8/treevalue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20434 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-06 16:34:40.000000 treevalue-1.4.8/treevalue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.487417 treevalue-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-06 18:28:25.000000 treevalue-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-06 18:28:25.000000 treevalue-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20434 2023-03-06 18:29:03.487417 treevalue-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19415 2023-03-06 18:28:25.000000 treevalue-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-03-06 18:28:25.000000 treevalue-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-benchmark.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-potc.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-test-extra.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-06 18:28:25.000000 treevalue-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-06 18:29:03.487417 treevalue-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-03-06 18:28:25.000000 treevalue-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.479417 treevalue-1.4.9/treevalue/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.479417 treevalue-1.4.9/treevalue/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.479417 treevalue-1.4.9/treevalue/entry/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/entry/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6100 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2286 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/entry/script/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/entry/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/tree/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/delay.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/delay.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1655 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/storage.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    11078 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/common/storage.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/tree/func/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/cfunc.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    11566 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/cfunc.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)    10041 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/func.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/modes.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/func/modes.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/tree/general/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/general/fast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50264 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/general/general.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.483417 treevalue-1.4.9/treevalue/tree/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/cjax.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/cjax.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/ctorch.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/ctorch.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/general.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     9214 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/general.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/jax.py
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/integration/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.487417 treevalue-1.4.9/treevalue/tree/tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/constraint.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/constraint.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/flatten.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/flatten.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/functional.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     9418 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/functional.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     7010 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/service.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/service.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/structural.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    17724 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/structural.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     2644 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    40127 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/tree/tree/tree.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.487417 treevalue-1.4.9/treevalue/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15309 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4439 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/utils/formattree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7371 2023-03-06 18:28:25.000000 treevalue-1.4.9/treevalue/utils/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 18:29:03.479417 treevalue-1.4.9/treevalue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20434 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-06 18:29:03.000000 treevalue-1.4.9/treevalue.egg-info/top_level.txt
```

### Comparing `treevalue-1.4.8/LICENSE` & `treevalue-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/PKG-INFO` & `treevalue-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treevalue
-Version: 1.4.8
+Version: 1.4.9
 Summary: A flexible, generalized tree-based data structure.
 Home-page: https://github.com/HansBug/treevalue
 Author: HansBug, DI-engine's Contributors
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: treevalue Version: 1.4.8 Summary: A flexible,
+Metadata-Version: 2.1 Name: treevalue Version: 1.4.9 Summary: A flexible,
 generalized tree-based data structure. Home-page: https://github.com/HansBug/
 treevalue Author: HansBug, DI-engine's Contributors Author-email:
 hansbug@buaa.edu.cn License: Apache License, Version 2.0 Keywords: Tree-
 structured Value Management Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `treevalue-1.4.8/README.md` & `treevalue-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/pyproject.toml` & `treevalue-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/setup.py` & `treevalue-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/entry/cli/base.py` & `treevalue-1.4.9/treevalue/entry/cli/base.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/entry/cli/export.py` & `treevalue-1.4.9/treevalue/entry/cli/export.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/entry/cli/graph.py` & `treevalue-1.4.9/treevalue/entry/cli/graph.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/entry/cli/io.py` & `treevalue-1.4.9/treevalue/entry/cli/io.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/entry/cli/utils.py` & `treevalue-1.4.9/treevalue/entry/cli/utils.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/common/base.pyx` & `treevalue-1.4.9/treevalue/tree/common/base.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/common/delay.pxd` & `treevalue-1.4.9/treevalue/tree/common/delay.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/common/delay.pyx` & `treevalue-1.4.9/treevalue/tree/common/delay.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/common/storage.pxd` & `treevalue-1.4.9/treevalue/tree/common/storage.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/common/storage.pyx` & `treevalue-1.4.9/treevalue/tree/common/storage.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/func/cfunc.pxd` & `treevalue-1.4.9/treevalue/tree/func/cfunc.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/func/cfunc.pyx` & `treevalue-1.4.9/treevalue/tree/func/cfunc.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/func/func.py` & `treevalue-1.4.9/treevalue/tree/func/func.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/func/modes.pxd` & `treevalue-1.4.9/treevalue/tree/func/modes.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/func/modes.pyx` & `treevalue-1.4.9/treevalue/tree/func/modes.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/general/general.py` & `treevalue-1.4.9/treevalue/tree/general/general.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/__init__.py` & `treevalue-1.4.9/treevalue/tree/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/base.pyx` & `treevalue-1.4.9/treevalue/tree/integration/base.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/cjax.pyx` & `treevalue-1.4.9/treevalue/tree/integration/cjax.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/ctorch.pyx` & `treevalue-1.4.9/treevalue/tree/integration/ctorch.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/general.pxd` & `treevalue-1.4.9/treevalue/tree/integration/general.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/general.pyx` & `treevalue-1.4.9/treevalue/tree/integration/general.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/jax.py` & `treevalue-1.4.9/treevalue/tree/integration/jax.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/integration/torch.py` & `treevalue-1.4.9/treevalue/tree/integration/torch.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/constraint.pxd` & `treevalue-1.4.9/treevalue/tree/tree/constraint.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/constraint.pyx` & `treevalue-1.4.9/treevalue/tree/tree/constraint.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/flatten.pxd` & `treevalue-1.4.9/treevalue/tree/tree/flatten.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/flatten.pyx` & `treevalue-1.4.9/treevalue/tree/tree/flatten.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/functional.pxd` & `treevalue-1.4.9/treevalue/tree/tree/functional.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/functional.pyx` & `treevalue-1.4.9/treevalue/tree/tree/functional.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/graph.py` & `treevalue-1.4.9/treevalue/tree/tree/graph.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/io.py` & `treevalue-1.4.9/treevalue/tree/tree/io.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/service.pyx` & `treevalue-1.4.9/treevalue/tree/tree/service.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/structural.pxd` & `treevalue-1.4.9/treevalue/tree/tree/structural.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/structural.pyx` & `treevalue-1.4.9/treevalue/tree/tree/structural.pyx`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/tree.pxd` & `treevalue-1.4.9/treevalue/tree/tree/tree.pxd`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/tree/tree/tree.pyx` & `treevalue-1.4.9/treevalue/tree/tree/tree.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # distutils:language=c++
 # cython:language_level=3
 
 import os
+import shutil
 from collections.abc import Sized, Container, Reversible, Mapping
 from operator import itemgetter
 
 import cython
 from hbutils.design import SingletonMark
 
 from .constraint cimport Constraint, to_constraint, transact, _EMPTY_CONSTRAINT
@@ -66,14 +67,20 @@
         self._path = path
         self._cons = cons
 
     def __str__(self):
         return f"Validation failed on {self._cons!r} at position {self._path!r}{os.linesep}" \
                f"{type(self._error).__name__}: {self._error}"
 
+cdef inline bool _check_dot_installed():
+    if shutil.which('dot'):
+        return True
+    else:
+        return False
+
 cdef class TreeValue:
     r"""
     Overview:
         Base framework of tree value. \
         And if the fast functions and operators are what you need, \
         please use `FastTreeValue` in `treevalue.tree.general`. \
         The `TreeValue` class is a light-weight framework just for DIY.
@@ -975,23 +982,32 @@
     @cython.final
     cdef inline object _get_tree_graph(self):
         from .graph import graphics
         return graphics((self, '<root>'))
 
     @cython.binding(True)
     def _repr_svg_(self):
-        return self._get_tree_graph().pipe(format='svg', encoding='utf-8')
+        if _check_dot_installed():
+            return self._get_tree_graph().pipe(format='svg', encoding='utf-8')
+        else:
+            return None
 
     @cython.binding(True)
     def _repr_png_(self):
-        return self._get_tree_graph().pipe(format='png')
+        if _check_dot_installed():
+            return self._get_tree_graph().pipe(format='png')
+        else:
+            return None
 
     @cython.binding(True)
     def _repr_jpeg_(self):
-        return self._get_tree_graph().pipe(format='jpeg')
+        if _check_dot_installed():
+            return self._get_tree_graph().pipe(format='jpeg')
+        else:
+            return None
 
 cdef str _prefix_fix(object text, object prefix):
     cdef list lines = []
     cdef int i
     cdef str line
     cdef str white = ' ' * len(prefix)
     for i, line in enumerate(text.splitlines()):
```

### Comparing `treevalue-1.4.8/treevalue/utils/color.py` & `treevalue-1.4.9/treevalue/utils/color.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/utils/formattree.py` & `treevalue-1.4.9/treevalue/utils/formattree.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/utils/random.py` & `treevalue-1.4.9/treevalue/utils/random.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue/utils/tree.py` & `treevalue-1.4.9/treevalue/utils/tree.py`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue.egg-info/PKG-INFO` & `treevalue-1.4.9/treevalue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treevalue
-Version: 1.4.8
+Version: 1.4.9
 Summary: A flexible, generalized tree-based data structure.
 Home-page: https://github.com/HansBug/treevalue
 Author: HansBug, DI-engine's Contributors
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: treevalue Version: 1.4.8 Summary: A flexible,
+Metadata-Version: 2.1 Name: treevalue Version: 1.4.9 Summary: A flexible,
 generalized tree-based data structure. Home-page: https://github.com/HansBug/
 treevalue Author: HansBug, DI-engine's Contributors Author-email:
 hansbug@buaa.edu.cn License: Apache License, Version 2.0 Keywords: Tree-
 structured Value Management Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `treevalue-1.4.8/treevalue.egg-info/SOURCES.txt` & `treevalue-1.4.9/treevalue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `treevalue-1.4.8/treevalue.egg-info/requires.txt` & `treevalue-1.4.9/treevalue.egg-info/requires.txt`

 * *Files identical despite different names*


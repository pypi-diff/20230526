# Comparing `tmp/coconut-develop-3.0.1.post0.dev6.tar.gz` & `tmp/coconut-develop-3.0.1.post0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev6.tar", last modified: Fri May 26 01:40:47 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev7.tar", last modified: Fri May 26 05:59:54 2023, max compression
```

## Comparing `coconut-develop-3.0.1.post0.dev6.tar` & `coconut-develop-3.0.1.post0.dev7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/FAQ.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/DOCS.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)    29125 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/api.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    99362 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    92726 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-26 01:40:46.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    35944 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/FAQ.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    29312 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    99362 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    92726 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-26 05:59:52.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36035 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-26 05:59:54.000000 coconut-develop-3.0.1.post0.dev7/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-26 05:04:21.000000 coconut-develop-3.0.1.post0.dev7/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.0.1.post0.dev6/README.rst` & `coconut-develop-3.0.1.post0.dev7/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/conf.py` & `coconut-develop-3.0.1.post0.dev7/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/FAQ.md` & `coconut-develop-3.0.1.post0.dev7/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/_coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev7/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/_coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev7/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/LICENSE.txt` & `coconut-develop-3.0.1.post0.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/setup.py` & `coconut-develop-3.0.1.post0.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/xontrib/coconut.py` & `coconut-develop-3.0.1.post0.dev7/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/HELP.md` & `coconut-develop-3.0.1.post0.dev7/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/DOCS.md` & `coconut-develop-3.0.1.post0.dev7/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.pyi` & `coconut-develop-3.0.1.post0.dev7/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.py` & `coconut-develop-3.0.1.post0.dev7/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/highlighter.py` & `coconut-develop-3.0.1.post0.dev7/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/api.py` & `coconut-develop-3.0.1.post0.dev7/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/constants_test.py` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/extras.coco` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/main_test.py` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/main_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,19 +715,24 @@
             p.sendline("xontrib load coconut")
             p.expect("$")
             p.sendline("!(ls -la) |> bool")
             p.expect("True")
             p.sendline('$ENV_VAR = "ABC"')
             p.expect("$")
             p.sendline('echo f"{$ENV_VAR}"; echo f"{$ENV_VAR}"')
-            p.expect("ABC\nABC")
+            p.expect("ABC")
+            p.expect("ABC")
             p.sendline("echo 123;; 123")
             p.expect("123;; 123")
+            p.sendline('execx("10 |> print")')
+            p.expect("subprocess mode")
             p.sendline("xontrib unload coconut")
             p.expect("$")
+            p.sendline("1 |> print")
+            p.expect("subprocess mode")
             p.sendeof()
             if p.isalive():
                 p.terminate()
 
     if IPY and (not WINDOWS or PY35):
         def test_ipython_extension(self):
             call(
```

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/__main__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/tests/__init__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/convenience.pyi` & `coconut-develop-3.0.1.post0.dev7/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/convenience.py` & `coconut-develop-3.0.1.post0.dev7/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.pyi` & `coconut-develop-3.0.1.post0.dev7/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/api.pyi` & `coconut-develop-3.0.1.post0.dev7/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/root.py` & `coconut-develop-3.0.1.post0.dev7/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.1"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 6
+DEVELOP = 7
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/requirements.py` & `coconut-develop-3.0.1.post0.dev7/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/main.py` & `coconut-develop-3.0.1.post0.dev7/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/header.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/grammar.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/matching.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/compiler.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/util.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/compiler/__init__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/root.py` & `coconut-develop-3.0.1.post0.dev7/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/embed.py` & `coconut-develop-3.0.1.post0.dev7/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__main__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__init__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/mypy.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/watch.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/command.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/command.pyi` & `coconut-develop-3.0.1.post0.dev7/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/cli.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/util.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev7/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/terminal.py` & `coconut-develop-3.0.1.post0.dev7/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/exceptions.py` & `coconut-develop-3.0.1.post0.dev7/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/constants.py` & `coconut-develop-3.0.1.post0.dev7/coconut/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -885,15 +885,16 @@
         "sphinx",
         ("pygments", "mark<39"),
         ("pygments", "mark39"),
         "myst-parser",
         "pydata-sphinx-theme",
     ),
     "tests": (
-        "pytest",
+        ("pytest", "py<36"),
+        ("pytest", "py36"),
         "pexpect",
         ("numpy", "py34"),
         ("numpy", "py2;cpy"),
         ("pandas", "py36"),
     ),
 }
 
@@ -921,14 +922,15 @@
     ("typing", "py<35"): (3, 10),
     ("typing_extensions", "py37"): (4, 6),
     ("ipython", "py38"): (8,),
     ("ipykernel", "py38"): (6,),
     ("jedi", "py39"): (0, 18),
     ("pygments", "mark39"): (2, 15),
     ("xonsh", "py38"): (0, 14),
+    ("pytest", "py36"): (7,),
 
     # pinned reqs: (must be added to pinned_reqs below)
 
     # don't upgrade until myst-parser supports the new version
     "sphinx": (6,),
     # don't upgrade these; they breaks on Python 3.7
     ("ipython", "py==37"): (7, 34),
@@ -945,15 +947,15 @@
     ("jupytext", "py3"): (1, 8),
     ("jupyterlab", "py35"): (2, 2),
     ("xonsh", "py<36"): (0, 9),
     ("typing_extensions", "py==35"): (3, 10),
     # don't upgrade this to allow all versions
     ("prompt_toolkit", "mark3"): (1,),
     # don't upgrade this; it breaks on Python 2.6
-    "pytest": (3,),
+    ("pytest", "py<36"): (3,),
     # don't upgrade this; it breaks on unix
     "vprof": (0, 36),
     # don't upgrade this; it breaks on Python 3.4
     ("pygments", "mark<39"): (2, 3),
     # don't upgrade these; they break on Python 2
     ("jupyter-client", "py<35"): (5, 3),
     ("pywinpty", "py2;windows"): (0, 5),
@@ -983,15 +985,15 @@
     ("jupyter-console", "py>=35;py<37"),
     ("jupyter-client", "py==35"),
     ("jupytext", "py3"),
     ("jupyterlab", "py35"),
     ("xonsh", "py<36"),
     ("typing_extensions", "py==35"),
     ("prompt_toolkit", "mark3"),
-    "pytest",
+    ("pytest", "py<36"),
     "vprof",
     ("pygments", "mark<39"),
     ("pywinpty", "py2;windows"),
     ("jupyter-console", "py<35"),
     ("ipython", "py2"),
     ("ipykernel", "py2"),
     ("prompt_toolkit", "mark2"),
```

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/_pyparsing.py` & `coconut-develop-3.0.1.post0.dev7/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/integrations.py` & `coconut-develop-3.0.1.post0.dev7/coconut/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         self.loaded = True
 
         return self.runner.vars
 
     def unload(self, xsh):
         if not self.loaded:
             # hide imports to avoid circular dependencies
-            from coconut.exceptions import CoconutException
-            raise CoconutException("attempting to unload Coconut xontrib but it was never loaded")
+            from coconut.terminal import logger
+            logger.warn("attempting to unload Coconut xontrib but it was never loaded")
         self.loaded = False
 
 
 _load_xontrib_ = CoconutXontribLoader()
 
 _unload_xontrib_ = _load_xontrib_.unload
```

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/util.py` & `coconut-develop-3.0.1.post0.dev7/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/__main__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev7/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/PKG-INFO` & `coconut-develop-3.0.1.post0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.1.post0.dev6
+Version: 3.0.1.post0.dev7
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
```

### Comparing `coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.1.post0.dev7/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev6/CONTRIBUTING.md` & `coconut-develop-3.0.1.post0.dev7/CONTRIBUTING.md`

 * *Files identical despite different names*


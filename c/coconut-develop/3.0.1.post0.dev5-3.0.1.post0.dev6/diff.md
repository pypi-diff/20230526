# Comparing `tmp/coconut-develop-3.0.1.post0.dev5.tar.gz` & `tmp/coconut-develop-3.0.1.post0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev5.tar", last modified: Thu May 25 10:11:39 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev6.tar", last modified: Fri May 26 01:40:47 2023, max compression
```

## Comparing `coconut-develop-3.0.1.post0.dev5.tar` & `coconut-develop-3.0.1.post0.dev6.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/FAQ.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/DOCS.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/__coconut__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/api.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/__coconut__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    99362 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    92661 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-25 10:11:38.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    35759 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8404 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-25 10:11:39.000000 coconut-develop-3.0.1.post0.dev5/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-25 09:35:55.000000 coconut-develop-3.0.1.post0.dev5/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/FAQ.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    29125 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    99362 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    92726 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-26 01:40:46.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35944 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-26 01:40:47.000000 coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-26 01:07:04.000000 coconut-develop-3.0.1.post0.dev6/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.0.1.post0.dev5/README.rst` & `coconut-develop-3.0.1.post0.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/conf.py` & `coconut-develop-3.0.1.post0.dev6/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/FAQ.md` & `coconut-develop-3.0.1.post0.dev6/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/_coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev6/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/_coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev6/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/LICENSE.txt` & `coconut-develop-3.0.1.post0.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/setup.py` & `coconut-develop-3.0.1.post0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/xontrib/coconut.py` & `coconut-develop-3.0.1.post0.dev6/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/HELP.md` & `coconut-develop-3.0.1.post0.dev6/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/DOCS.md` & `coconut-develop-3.0.1.post0.dev6/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/__coconut__/__init__.pyi` & `coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/__coconut__/__init__.py` & `coconut-develop-3.0.1.post0.dev6/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/highlighter.py` & `coconut-develop-3.0.1.post0.dev6/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/api.py` & `coconut-develop-3.0.1.post0.dev6/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/constants_test.py` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/src/extras.coco` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/main_test.py` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/main_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     call_output,
     reload,
 )
 from coconut.constants import (
     WINDOWS,
     PYPY,
     IPY,
+    XONSH,
     MYPY,
     PY35,
-    PY36,
     PY38,
     PY310,
     icoconut_default_kernel_names,
     icoconut_custom_kernel_name,
     mypy_err_infixes,
     get_bool_env_var,
 )
@@ -704,24 +704,28 @@
 
     def test_import_runnable(self):
         with using_path(runnable_py):
             call_coconut([runnable_coco, runnable_py])
             for _ in range(2):  # make sure we can import it twice
                 call_python([runnable_py, "--arg"], assert_output=True, convert_to_import=True)
 
-    # not py36 is only because newer Python versions require newer xonsh
-    #  versions that aren't always installed by pip install coconut[tests]
-    if not WINDOWS and PY35 and not PY36:
+    if not WINDOWS and XONSH:
         def test_xontrib(self):
             p = spawn_cmd("xonsh")
             p.expect("$")
             p.sendline("xontrib load coconut")
             p.expect("$")
             p.sendline("!(ls -la) |> bool")
             p.expect("True")
+            p.sendline('$ENV_VAR = "ABC"')
+            p.expect("$")
+            p.sendline('echo f"{$ENV_VAR}"; echo f"{$ENV_VAR}"')
+            p.expect("ABC\nABC")
+            p.sendline("echo 123;; 123")
+            p.expect("123;; 123")
             p.sendline("xontrib unload coconut")
             p.expect("$")
             p.sendeof()
             if p.isalive():
                 p.terminate()
 
     if IPY and (not WINDOWS or PY35):
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/__main__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/tests/__init__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/convenience.pyi` & `coconut-develop-3.0.1.post0.dev6/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/convenience.py` & `coconut-develop-3.0.1.post0.dev6/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/__coconut__.pyi` & `coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/api.pyi` & `coconut-develop-3.0.1.post0.dev6/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/root.py` & `coconut-develop-3.0.1.post0.dev6/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.1"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 5
+DEVELOP = 6
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/requirements.py` & `coconut-develop-3.0.1.post0.dev6/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/main.py` & `coconut-develop-3.0.1.post0.dev6/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/__coconut__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/header.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/grammar.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -2344,14 +2344,15 @@
     parens = originalTextFor(nestedExpr("(", ")", ignoreExpr=None))
     brackets = originalTextFor(nestedExpr("[", "]", ignoreExpr=None))
     braces = originalTextFor(nestedExpr("{", "}", ignoreExpr=None))
 
     unsafe_anything_stmt = originalTextFor(regex_item("[^\n]+\n+"))
     unsafe_xonsh_command = originalTextFor(
         (Optional(at) + dollar | bang)
+        + ~(lparen + rparen | lbrack + rbrack | lbrace + rbrace)
         + (parens | brackets | braces | unsafe_name),
     )
     xonsh_parser, _anything_stmt, _xonsh_command = disable_outside(
         single_parser,
         unsafe_anything_stmt,
         unsafe_xonsh_command,
     )
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/matching.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/compiler.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/util.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/compiler/__init__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/icoconut/root.py` & `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/icoconut/embed.py` & `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/icoconut/__main__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/icoconut/__init__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/mypy.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/watch.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/command.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/command.pyi` & `coconut-develop-3.0.1.post0.dev6/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/cli.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/util.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/command/__init__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev6/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/terminal.py` & `coconut-develop-3.0.1.post0.dev6/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/exceptions.py` & `coconut-develop-3.0.1.post0.dev6/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/constants.py` & `coconut-develop-3.0.1.post0.dev6/coconut/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,15 +859,17 @@
         ("typing_extensions", "py==36"),
         ("typing_extensions", "py37"),
     ),
     "watch": (
         "watchdog",
     ),
     "xonsh": (
-        "xonsh",
+        ("xonsh", "py<36"),
+        ("xonsh", "py==37"),
+        ("xonsh", "py38"),
     ),
     "backports": (
         ("trollius", "py2;cpy"),
         ("aenum", "py<34"),
         ("dataclasses", "py==36"),
         ("typing", "py<35"),
         ("typing_extensions", "py==35"),
@@ -918,33 +920,35 @@
     ("jupyter-console", "py37"): (6, 6),
     ("typing", "py<35"): (3, 10),
     ("typing_extensions", "py37"): (4, 6),
     ("ipython", "py38"): (8,),
     ("ipykernel", "py38"): (6,),
     ("jedi", "py39"): (0, 18),
     ("pygments", "mark39"): (2, 15),
+    ("xonsh", "py38"): (0, 14),
 
     # pinned reqs: (must be added to pinned_reqs below)
 
     # don't upgrade until myst-parser supports the new version
     "sphinx": (6,),
-    # don't upgrade this; it breaks on Python 3.7
+    # don't upgrade these; they breaks on Python 3.7
     ("ipython", "py==37"): (7, 34),
-    # don't upgrade these; it breaks on Python 3.6
+    ("xonsh", "py==37"): (0, 12),
+    # don't upgrade these; they breaks on Python 3.6
     ("pandas", "py36"): (1,),
     ("jupyter-client", "py36"): (7, 1, 2),
     ("typing_extensions", "py==36"): (4, 1),
     # don't upgrade these; they break on Python 3.5
     ("ipykernel", "py3;py<38"): (5, 5),
     ("ipython", "py3;py<37"): (7, 9),
     ("jupyter-console", "py>=35;py<37"): (6, 1),
     ("jupyter-client", "py==35"): (6, 1, 12),
     ("jupytext", "py3"): (1, 8),
     ("jupyterlab", "py35"): (2, 2),
-    "xonsh": (0, 9),
+    ("xonsh", "py<36"): (0, 9),
     ("typing_extensions", "py==35"): (3, 10),
     # don't upgrade this to allow all versions
     ("prompt_toolkit", "mark3"): (1,),
     # don't upgrade this; it breaks on Python 2.6
     "pytest": (3,),
     # don't upgrade this; it breaks on unix
     "vprof": (0, 36),
@@ -965,25 +969,26 @@
     "pyparsing": (2, 4, 7),
 }
 
 # should match the reqs with comments above
 pinned_reqs = (
     "sphinx",
     ("ipython", "py==37"),
+    ("xonsh", "py==37"),
     ("pandas", "py36"),
     ("jupyter-client", "py36"),
     ("typing_extensions", "py==36"),
     ("jupyter-client", "py<35"),
     ("ipykernel", "py3;py<38"),
     ("ipython", "py3;py<37"),
     ("jupyter-console", "py>=35;py<37"),
     ("jupyter-client", "py==35"),
     ("jupytext", "py3"),
     ("jupyterlab", "py35"),
-    "xonsh",
+    ("xonsh", "py<36"),
     ("typing_extensions", "py==35"),
     ("prompt_toolkit", "mark3"),
     "pytest",
     "vprof",
     ("pygments", "mark<39"),
     ("pywinpty", "py2;windows"),
     ("jupyter-console", "py<35"),
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/_pyparsing.py` & `coconut-develop-3.0.1.post0.dev6/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/integrations.py` & `coconut-develop-3.0.1.post0.dev6/coconut/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,25 +108,25 @@
         from coconut.terminal import logger
 
         parse_start_time = get_clock_time()
         quiet, logger.quiet = logger.quiet, True
         success = False
         try:
             # .strip() outside the memoization
-            code = self.memoized_parse_xonsh(code.strip())
+            compiled = self.memoized_parse_xonsh(code.strip())
         except CoconutException as err:
             err_str = format_error(err).splitlines()[0]
-            code += "  #" + err_str
+            compiled = code + "  #" + err_str
         else:
             success = True
         finally:
             logger.quiet = quiet
             self.timing_info.append(("parse", get_clock_time() - parse_start_time))
 
-        return code, success
+        return compiled, success
 
     def new_try_subproc_toks(self, ctxtransformer, node, *args, **kwargs):
         """Version of try_subproc_toks that handles the fact that Coconut
         code may have different columns than Python code."""
         mode = ctxtransformer.mode
         if self.loaded:
             ctxtransformer.mode = "eval"
@@ -167,15 +167,17 @@
                         line = original_lines[-1]
                     if line in used_lines:
                         line = ""
                     else:
                         used_lines.add(line)
                     new_inp_lines.append(line)
                     last_ln = ln
-                inp = "\n".join(new_inp_lines) + "\n"
+                inp = "\n".join(new_inp_lines)
+
+            inp += "\n"
 
         return ctxtransformer.__class__.ctxvisit(ctxtransformer, node, inp, ctx, mode, *args, **kwargs)
 
     def __call__(self, xsh, **kwargs):
         # hide imports to avoid circular dependencies
         from coconut.util import get_clock_time
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/util.py` & `coconut-develop-3.0.1.post0.dev6/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/__main__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev6/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/PKG-INFO` & `coconut-develop-3.0.1.post0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.1.post0.dev5
+Version: 3.0.1.post0.dev6
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
```

### Comparing `coconut-develop-3.0.1.post0.dev5/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.1.post0.dev6/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev5/CONTRIBUTING.md` & `coconut-develop-3.0.1.post0.dev6/CONTRIBUTING.md`

 * *Files identical despite different names*


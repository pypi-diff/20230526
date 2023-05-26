# Comparing `tmp/yambs-1.6.0.tar.gz` & `tmp/yambs-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yambs-1.6.0.tar", last modified: Thu May 25 00:21:23 2023, max compression
+gzip compressed data, was "yambs-1.7.1.tar", last modified: Fri May 26 00:33:37 2023, max compression
```

## Comparing `yambs-1.6.0.tar` & `yambs-1.7.1.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 00:20:12.000000 yambs-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-25 00:21:23.143940 yambs-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-25 00:20:12.000000 yambs-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 00:20:12.000000 yambs-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 00:21:23.143940 yambs-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 00:20:12.000000 yambs-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 00:20:12.000000 yambs-1.6.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 00:20:12.000000 yambs-1.6.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/commands/uf2conv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/config/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/chips.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/infineon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/includes/microchip.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Architecture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Board.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Chip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/schemas/Toolchain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/all.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/architecture.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/board.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/build.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/chip.ld.j2
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/chip.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/rules.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/templates/toolchain.ninja.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/data/yambs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/chips.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/ninja.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/generate/toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/translation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.143940 yambs-1.6.0/yambs/uf2/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-25 00:20:12.000000 yambs-1.6.0/yambs/uf2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:21:23.139940 yambs-1.6.0/yambs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 00:21:23.000000 yambs-1.6.0/yambs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.775170 yambs-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 00:32:03.000000 yambs-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-26 00:33:37.775170 yambs-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-05-26 00:32:03.000000 yambs-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-26 00:32:03.000000 yambs-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:33:37.775170 yambs-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-26 00:32:03.000000 yambs-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.747170 yambs-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 00:32:03.000000 yambs-1.7.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 00:32:03.000000 yambs-1.7.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.747170 yambs-1.7.1/yambs/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.755170 yambs-1.7.1/yambs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/commands/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/commands/uf2conv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.755170 yambs-1.7.1/yambs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/config/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.755170 yambs-1.7.1/yambs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.759170 yambs-1.7.1/yambs/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/includes/chips.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/includes/infineon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/includes/microchip.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.759170 yambs-1.7.1/yambs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/schemas/Architecture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/schemas/Board.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/schemas/Chip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/schemas/Toolchain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.767170 yambs-1.7.1/yambs/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/all.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/architecture.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/board.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/build.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/chip.ld.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/chip.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/rules.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/templates/toolchain.ninja.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/data/yambs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.767170 yambs-1.7.1/yambs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.775170 yambs-1.7.1/yambs/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/boards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/chips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.775170 yambs-1.7.1/yambs/generate/ninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/ninja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/ninja/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/generate/toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.775170 yambs-1.7.1/yambs/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/translation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.775170 yambs-1.7.1/yambs/uf2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-26 00:32:03.000000 yambs-1.7.1/yambs/uf2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:33:37.751170 yambs-1.7.1/yambs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 00:33:37.000000 yambs-1.7.1/yambs.egg-info/top_level.txt
```

### Comparing `yambs-1.6.0/LICENSE` & `yambs-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/PKG-INFO` & `yambs-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.6.0
+Version: 1.7.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=aa5f774861e316a941fdf5a8220d678d
+    hash=cd7afdb31a4064e0d8f4e2e819060559
     =====================================
 -->
 
-# yambs ([1.6.0](https://pypi.org/project/yambs/))
+# yambs ([1.7.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.6.0/README.md` & `yambs-1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=aa5f774861e316a941fdf5a8220d678d
+    hash=cd7afdb31a4064e0d8f4e2e819060559
     =====================================
 -->
 
-# yambs ([1.6.0](https://pypi.org/project/yambs/))
+# yambs ([1.7.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.6.0/pyproject.toml` & `yambs-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "yambs"
-version = "1.6.0"
+version = "1.7.1"
 description = "Yet another meta build-system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `yambs-1.6.0/setup.py` & `yambs-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/tests/test_entry.py` & `yambs-1.7.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/app.py` & `yambs-1.7.1/yambs/app.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/commands/all.py` & `yambs-1.7.1/yambs/commands/all.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/commands/gen.py` & `yambs-1.7.1/yambs/commands/gen.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/commands/uf2conv.py` & `yambs-1.7.1/yambs/commands/uf2conv.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/config/__init__.py` & `yambs-1.7.1/yambs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/config/board.py` & `yambs-1.7.1/yambs/config/board.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/data/includes/chips.yaml` & `yambs-1.7.1/yambs/data/includes/chips.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/data/includes/infineon.yaml` & `yambs-1.7.1/yambs/data/includes/infineon.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/data/includes/microchip.yaml` & `yambs-1.7.1/yambs/data/includes/microchip.yaml`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/data/schemas/Chip.yaml` & `yambs-1.7.1/yambs/data/schemas/Chip.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         type: object
         additionalProperties: false
         patternProperties:
           "^[a-zA-Z0-9-_.]+$":
             type: string
 
       include:
-        default: picolibc
+        default: picolibcpp
         type: string
```

### Comparing `yambs-1.6.0/yambs/data/schemas/Config.yaml` & `yambs-1.7.1/yambs/data/schemas/Config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,22 @@
     type: string
     default: build
 
   cc:
     type: string
     default: gcc
 
+  cxx:
+    type: string
+    default: g++
+
+  ld:
+    type: string
+    default: g++
+
   common_cflags:
     type: array
     default: [-Wall, -g, -ffunction-sections]
     items:
       type: string
 
   common_ldflags:
```

### Comparing `yambs-1.6.0/yambs/data/templates/rules.ninja.j2` & `yambs-1.7.1/yambs/data/templates/rules.ninja.j2`

 * *Files 22% similar despite different names*

```diff
@@ -3,37 +3,41 @@
 
 cflags = $common_cflags $
          $board_extra_cflags $
          $chip_extra_cflags $
          $architecture_extra_cflags $
          $toolchain_cflags
 
-tool = ${toolchain_prefix}{{cc}}
-
 rule cc
   depfile = $out.d
   deps = gcc
-  command = $tool -MD -MF $out.d $cflags -c $in -o $out
+  command = ${toolchain_prefix}{{cc}} -MD -MF $out.d $cflags $
+            -std=$c_standard -c $in -o $out
+
+rule cxx
+  depfile = $out.d
+  deps = gcc
+  command = ${toolchain_prefix}{{cxx}} -MD -MF $out.d $cflags $
+            -std=$cxx_standard -c $in -o $out
 
 rule pio
   command = pioasm -o c-sdk $in $out
 
 ldflags = $board_ldflags{% for flag in common_ldflags %} {{flag}}{% endfor %}
 
 
 rule link
-  command = $tool $cflags $ldflags -Wl,-Map=$out.map $in -o $out
+  command = ${toolchain_prefix}{{ld}} $cflags $ldflags -Wl,-Map=$out.map $in -o $out
 
 rule bin
   command = ${toolchain_prefix}objcopy -O binary $in $out
 
 rule hex
   command = ${toolchain_prefix}objcopy -O ihex $in $out
 
 rule dump
   command = ${toolchain_prefix}objdump -D $in > $out
 
 rule uf2
   command = mbs uf2conv $uf2conv_args -o $out $in
 
 build_dir = {{build_root}}/$toolchain/$architecture/$cpu
-generated_dir = $src_dir/generated
```

### Comparing `yambs-1.6.0/yambs/data/uf2families.json` & `yambs-1.7.1/yambs/data/uf2families.json`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/entry.py` & `yambs-1.7.1/yambs/entry.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/generate/__init__.py` & `yambs-1.7.1/yambs/generate/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,17 +14,40 @@
 # internal
 from yambs import PKG_NAME
 from yambs.environment import BuildEnvironment
 from yambs.generate.architectures import generate as generate_architectures
 from yambs.generate.boards import generate as generate_boards
 from yambs.generate.chips import generate as generate_chips
 from yambs.generate.common import render_template
+from yambs.generate.ninja.format import write_format_target
 from yambs.generate.toolchains import generate as generate_toolchains
 
 
+def create_board_apps(env: BuildEnvironment) -> None:
+    """
+    Generate JSON metadata to give other tools a simple lookup to application
+    sources (e.g. for loading or deploying).
+    """
+
+    board_apps: Dict[str, Any] = {}
+
+    # Ensure that the build root directory is present in the full output paths
+    # for built applications.
+    for board in env.config.board_data:
+        board_apps[board.name] = {
+            short: str(env.config.build_root.joinpath(path))
+            for short, path in board.apps.items()
+        }
+
+    ARBITER.encode(
+        env.ninja_root.joinpath("board_apps.json"),
+        board_apps,
+    )
+
+
 def generate(env: BuildEnvironment) -> None:
     """Generate ninja files."""
 
     templates_dir = resource("templates", package=PKG_NAME)
     assert templates_dir is not None
 
     jinja = environment(
@@ -40,21 +63,12 @@
         generate_chips,
         generate_toolchains,
         generate_architectures,
         generate_boards,
     ]:
         gen(jinja, env)
 
-    board_apps: Dict[str, Any] = {}
+    create_board_apps(env)
 
-    # Ensure that the build root directory is present in the full output paths
-    # for built applications.
-    for board in env.config.board_data:
-        board_apps[board.name] = {
-            short: str(env.config.build_root.joinpath(path))
-            for short, path in board.apps.items()
-        }
-
-    ARBITER.encode(
-        env.ninja_root.joinpath("board_apps.json"),
-        board_apps,
-    )
+    # Create format configuration.
+    with env.ninja_root.joinpath("format.ninja").open("w") as path_fd:
+        write_format_target(path_fd, env)
```

### Comparing `yambs-1.6.0/yambs/generate/architectures.py` & `yambs-1.7.1/yambs/generate/architectures.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/generate/boards.py` & `yambs-1.7.1/yambs/generate/boards.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,33 +13,35 @@
 from vcorelib.paths import rel
 
 # internal
 from yambs.config.board import Board
 from yambs.environment import BuildEnvironment, SourceSets
 from yambs.generate.common import render_template
 from yambs.generate.ninja import write_link_lines, write_source_line
-from yambs.translation import is_source
+from yambs.translation import is_header, is_source
 
 LOG = getLogger(__name__)
 
 
 def add_dir(
     stream: TextIO,
     paths: Set[Path],
     path: Path,
     comment: str,
     base: Path,
     current_sources: Set[Path],
     board: Board,
     board_specific: bool = False,
-) -> None:
+) -> Set[Path]:
     """Add a directory to set of paths."""
 
     LOG.debug("%s: checking '%s' for sources.", comment, path)
 
+    headers = set()
+
     if path.is_dir():
         stream.write(linesep + f"# {comment}." + linesep)
         for item in path.iterdir():
             translator = is_source(item)
             if translator is not None:
                 paths.add(
                     write_source_line(
@@ -48,14 +50,18 @@
                         base,
                         current_sources,
                         board,
                         translator,
                         board_specific=board_specific,
                     )
                 )
+            elif is_header(item):
+                headers.add(item)
+
+    return headers
 
 
 def create_paths_dict(root: Path, board: Board) -> Dict[str, Any]:
     """Create paths based on common pathing conventions."""
 
     chip = board.chip
 
@@ -75,55 +81,66 @@
     env: BuildEnvironment,
 ) -> SourceSets:
     """Write the source-file manifest."""
 
     # Add regular sources.
     all_srcs: Set[Path] = set()
 
+    # Collect header files while we're doing source discovery, too.
+    headers: Set[Path] = set()
+
     for kind, path in create_paths_dict(src_root, board).items():
-        add_dir(
-            stream,
-            all_srcs,
-            path,
-            f"{kind} sources",
-            src_root,
-            env.global_sources,
-            board,
+        headers.update(
+            add_dir(
+                stream,
+                all_srcs,
+                path,
+                f"{kind} sources",
+                src_root,
+                env.global_sources,
+                board,
+            )
         )
 
     # Add any extra sources this board specified.
     for extra in board.extra_dirs:
+        # Don't keep track of external headers.
         add_dir(
             stream,
             all_srcs,
             src_root.joinpath("third-party", extra),
-            "extra sources",
+            f"Extra sources ({extra})",
             src_root,
             env.global_sources,
             board,
         )
 
     # Add application sources.
     app_srcs: Set[Path] = set()
     for kind, path in create_paths_dict(
         src_root.joinpath("apps"), board
     ).items():
-        add_dir(
-            stream,
-            app_srcs,
-            path,
-            f"{kind} application sources",
-            src_root,
-            env.global_sources,
-            board,
-            # Avoid having a redundant directory in the path when the source
-            # directory is already the board-specific one.
-            board_specific="boards" not in str(path),
+        headers.update(
+            add_dir(
+                stream,
+                app_srcs,
+                path,
+                f"{kind} application sources",
+                src_root,
+                env.global_sources,
+                board,
+                # Avoid having a redundant directory in the path when the
+                # source directory is already the board-specific one.
+                board_specific="boards" not in str(path),
+            )
         )
 
+    # Keep track of all header files.
+    env.first_party_headers.update(headers)
+
     # Populate board sources.
     return env.set_board_sources(board, all_srcs, app_srcs)
 
 
 def generate(jinja: Environment, env: BuildEnvironment) -> None:
     """Generate board-related ninja files."""
```

### Comparing `yambs-1.6.0/yambs/generate/chips.py` & `yambs-1.7.1/yambs/generate/chips.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/generate/common.py` & `yambs-1.7.1/yambs/generate/common.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/generate/ninja.py` & `yambs-1.7.1/yambs/generate/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/generate/toolchains.py` & `yambs-1.7.1/yambs/generate/toolchains.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/schemas.py` & `yambs-1.7.1/yambs/schemas.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs/translation/__init__.py` & `yambs-1.7.1/yambs/translation/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 """
 
 # built-in
 from functools import lru_cache
 from pathlib import Path
 from typing import NamedTuple, Optional
 
+HEADER_EXTENSIONS = {".h", ".hpp"}
+
 
 class SourceTranslator(NamedTuple):
     """
     A structure for keeping track of how source files become different types
     of output files.
     """
 
@@ -30,33 +32,39 @@
         executable.
         """
         return self.output_extension == ".o"
 
     @property
     def generated_header(self) -> bool:
         """Determine if this translation produces a header file."""
-        return self.output_extension == ".h"
+        return self.output_extension in HEADER_EXTENSIONS
 
 
 DEFAULT = SourceTranslator()
 
 
 SOURCES = {
     ".c": DEFAULT,
     ".S": DEFAULT,
-    ".cc": DEFAULT,
+    ".cc": SourceTranslator(rule="cxx"),
+    ".cpp": SourceTranslator(rule="cxx"),
     ".pio": SourceTranslator("pio", ".h", Path("$generated_dir")),
 }
 
 
 @lru_cache(maxsize=None)
 def is_source(path: Path) -> Optional[SourceTranslator]:
     """Determine if a file is a source file."""
     return SOURCES.get(path.suffix)
 
 
+def is_header(path: Path) -> bool:
+    """determine if a path points to a header file."""
+    return path.suffix in HEADER_EXTENSIONS
+
+
 def get_translator(path: Path) -> SourceTranslator:
     """Get the source translator for a given source."""
 
     result = is_source(path)
     assert result is not None
     return result
```

### Comparing `yambs-1.6.0/yambs/uf2/__init__.py` & `yambs-1.7.1/yambs/uf2/__init__.py`

 * *Files identical despite different names*

### Comparing `yambs-1.6.0/yambs.egg-info/PKG-INFO` & `yambs-1.7.1/yambs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yambs
-Version: 1.6.0
+Version: 1.7.1
 Summary: Yet another meta build-system.
 Home-page: https://github.com/vkottler/yambs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=aa5f774861e316a941fdf5a8220d678d
+    hash=cd7afdb31a4064e0d8f4e2e819060559
     =====================================
 -->
 
-# yambs ([1.6.0](https://pypi.org/project/yambs/))
+# yambs ([1.7.1](https://pypi.org/project/yambs/))
 
 [![python](https://img.shields.io/pypi/pyversions/yambs.svg)](https://pypi.org/project/yambs/)
 ![Build Status](https://github.com/vkottler/yambs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/yambs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/yambs)
 ![PyPI - Status](https://img.shields.io/pypi/status/yambs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/yambs)
```

### Comparing `yambs-1.6.0/yambs.egg-info/SOURCES.txt` & `yambs-1.7.1/yambs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,12 @@
 yambs/data/templates/toolchain.ninja.j2
 yambs/environment/__init__.py
 yambs/generate/__init__.py
 yambs/generate/architectures.py
 yambs/generate/boards.py
 yambs/generate/chips.py
 yambs/generate/common.py
-yambs/generate/ninja.py
 yambs/generate/toolchains.py
+yambs/generate/ninja/__init__.py
+yambs/generate/ninja/format.py
 yambs/translation/__init__.py
 yambs/uf2/__init__.py
```


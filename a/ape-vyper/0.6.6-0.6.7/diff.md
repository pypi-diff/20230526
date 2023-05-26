# Comparing `tmp/ape-vyper-0.6.6.tar.gz` & `tmp/ape-vyper-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.6.tar", last modified: Thu May 18 19:07:42 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.7.tar", last modified: Fri May 26 01:41:09 2023, max compression
```

## Comparing `ape-vyper-0.6.6.tar` & `ape-vyper-0.6.7.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-18 19:07:42.000000 ape-vyper-0.6.6/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 19:07:41.000000 ape-vyper-0.6.6/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.055631 ape-vyper-0.6.6/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/erc20.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:07:42.059631 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/interfaces/IRegistry.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/registry.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/traceback_contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-05-18 19:06:44.000000 ape-vyper-0.6.6/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 01:41:08.000000 ape-vyper-0.6.7/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_37.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IRegistry.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/registry.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/traceback_contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/release-drafter.yml` & `ape-vyper-0.6.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.7/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.7/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/workflows/publish.yaml` & `ape-vyper-0.6.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.github/workflows/test.yaml` & `ape-vyper-0.6.7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.gitignore` & `ape-vyper-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/.pre-commit-config.yaml` & `ape-vyper-0.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/CONTRIBUTING.md` & `ape-vyper-0.6.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/LICENSE` & `ape-vyper-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/PKG-INFO` & `ape-vyper-0.6.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.6
+Version: 0.6.7
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -79,22 +80,22 @@
 
 ```yaml
 # Use `voting` example contracts from Vyperlang repo.
 dependencies:
   - name: VyperVoting
     github: vyperlang/vyper
     contracts_folder: examples/voting/
-    version: v0.3.7
+    version: v0.3.8
 
 # Automatically allow importing voting contracts in your project.
 vyper:
   import_remapping:
-    - "voting=VyperVoting@v0.3.7"
+    - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.7
+# @version 0.3.8
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.6/README.md` & `ape-vyper-0.6.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
 ```yaml
 # Use `voting` example contracts from Vyperlang repo.
 dependencies:
   - name: VyperVoting
     github: vyperlang/vyper
     contracts_folder: examples/voting/
-    version: v0.3.7
+    version: v0.3.8
 
 # Automatically allow importing voting contracts in your project.
 vyper:
   import_remapping:
-    - "voting=VyperVoting@v0.3.7"
+    - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.7
+# @version 0.3.8
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.6/ape_vyper/compiler.py` & `ape-vyper-0.6.7/ape_vyper/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     VyperInstallError,
 )
 
 DEV_MSG_PATTERN = re.compile(r"#\s*(dev:.+)")
 _RETURN_OPCODES = ("RETURN", "REVERT", "STOP")
 _FUNCTION_DEF = "FunctionDef"
 _FUNCTION_AST_TYPES = (_FUNCTION_DEF, "Name", "arguments")
+_EMPTY_REVERT_OFFSET = 18
+_NON_PAYABLE_STR = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
 
 
 class VyperConfig(PluginConfig):
     evm_version: Optional[str] = None
 
     import_remapping: List[str] = []
     """
@@ -280,36 +282,32 @@
                     opcodes = bytecode["opcodes"].split(" ")
                     compressed_src_map = SourceMap(__root__=bytecode["sourceMap"])
                     src_map = list(compressed_src_map.parse())[1:]
                     pc = 0
                     pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
                     last_value = None
                     revert_pc = -1
-                    revert_pc_offset = 18
-                    if _is_nonpayable_check(opcodes):
+                    if _has_empty_revert(opcodes):
                         # Starting in vyper 0.2.14, reverts without a reason string are optimized
                         # with a jump to the "end" of the bytecode.
                         revert_pc = (
                             len(opcodes)
                             + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
-                            - revert_pc_offset
+                            - _EMPTY_REVERT_OFFSET
                         )
 
                     processed_opcodes = []
-                    last_pc = None
-                    non_payable_str = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
+
+                    # There is only 1 non-payable check and it happens early in the bytecode.
+                    non_payable_check_found = False
 
                     while src_map and opcodes:
                         src = src_map.pop(0)
                         op = opcodes.pop(0)
                         processed_opcodes.append(op)
-                        if pc not in [x[0] for x in pc_map_list]:
-                            # Track the last unused PC location.
-                            last_pc = pc
-
                         pc += 1
 
                         # Detect immutable state member load.
                         # If this is the case, ignore increasing pc by push size.
                         is_code_copy = len(opcodes) > 5 and opcodes[5] == "CODECOPY"
 
                         if not is_code_copy and opcodes and is_0x_prefixed(opcodes[0]):
@@ -320,28 +318,18 @@
 
                         # Add content PC item.
                         # Also check for compiler runtime error handling.
                         # Runtime error locations are marked in the PCMap for further analysis.
                         if src.start is not None and src.length is not None:
                             stmt = ast.get_node(src)
                             if stmt:
-                                line_nos = list(stmt.line_numbers)
-                                # Add next non-payable check.
-                                if last_pc is not None and len(function_offsets) > 0:
-                                    next_fn = function_offsets[0]
-                                    if line_nos[0] >= next_fn[0] and line_nos[2] <= next_fn[1]:
-                                        np_check = {"location": None, "dev": non_payable_str}
-                                        pc_map_list.append((last_pc, np_check))
-                                        function_offsets.pop(0)
-
                                 # Add located item.
+                                line_nos = list(stmt.line_numbers)
                                 item: Dict = {"location": line_nos}
-                                is_revert_jump = _is_revert_jump(
-                                    op, last_value, revert_pc, processed_opcodes
-                                )
+                                is_revert_jump = _is_revert_jump(op, last_value, revert_pc)
                                 if op == "REVERT" or is_revert_jump:
                                     dev = None
                                     if stmt.ast_type in ("AugAssign", "BinOp"):
                                         # SafeMath
                                         for node in stmt.children:
                                             dev = RuntimeErrorType.from_operator(node.ast_type)
                                             if dev:
@@ -355,14 +343,26 @@
                                         if is_revert_jump and len(pc_map_list) >= 1:
                                             pc_map_list[-1][1]["dev"] = val
                                         else:
                                             item["dev"] = val
 
                                 pc_map_list.append((pc, item))
 
+                        elif (
+                            not non_payable_check_found
+                            and len(opcodes) >= 3
+                            and op == "CALLVALUE"
+                            and "PUSH" in opcodes[0]
+                            and is_0x_prefixed(opcodes[1])
+                            and _is_revert_jump(opcodes[2], int(opcodes[1], 16), revert_pc)
+                        ):
+                            item = {"dev": _NON_PAYABLE_STR, "location": None}
+                            pc_map_list.append((pc, item))
+                            non_payable_check_found = True
+
                     # Find content-specified dev messages.
                     dev_messages = {}
                     for line_no, line in content.items():
                         if match := re.search(DEV_MSG_PATTERN, line):
                             dev_messages[line_no] = match.group(1).strip()
 
                     contract_type = ContractType(
@@ -491,15 +491,18 @@
         err_str = dev_message.replace("dev: ", "")
 
         if err_str in [m.value for m in RuntimeErrorType]:
             # Is a builtin compiler error.
             runtime_error_type = RuntimeErrorType(err_str)
             runtime_error_cls = RUNTIME_ERROR_MAP[runtime_error_type]
             return runtime_error_cls(
-                txn=err.txn, trace=err.trace, contract_address=err.contract_address
+                contract_address=err.contract_address,
+                source_traceback=err.source_traceback,
+                trace=err.trace,
+                txn=err.txn,
             )
 
         else:
             # Not a builtin compiler error; cannot enrich.
             return err
 
     def trace_source(
@@ -512,14 +515,15 @@
         return self._get_traceback(source_contract_type, trace, calldata)
 
     def _get_traceback(
         self, contract_src: ContractSource, trace: Iterator[TraceFrame], calldata: HexBytes
     ) -> SourceTraceback:
         traceback = SourceTraceback.parse_obj([])
         function = None
+        last_pc = None
 
         for frame in trace:
             if frame.op in CALL_OPCODES:
                 called_contract, sub_calldata = self._create_contract_from_call(frame)
                 if called_contract:
                     ext = Path(called_contract.source_id).suffix
                     if not ext.endswith(".vy"):
@@ -550,41 +554,53 @@
                 if frame.op == "RETURN" and function:
                     return_ast_result = [x for x in function.ast.children if x.ast_type == "Return"]
                     if return_ast_result:
                         # Ensure return statement added.
                         # Sometimes it is missing from the PCMap otherwise.
                         return_ast = return_ast_result[-1]
                         location = return_ast.line_numbers
-                        start = traceback.last.end_lineno + 1
-                        traceback.last.extend(location, ws_start=start)
+
+                        last_lineno = max(0, location[2] - 1)
+                        for frameset in traceback.__root__[::-1]:
+                            if frameset.end_lineno is not None:
+                                last_lineno = frameset.end_lineno
+                                break
+
+                        start = last_lineno + 1
+                        last_pcs = {last_pc + 1} if last_pc else {}
+                        traceback.last.extend(location, pcs=last_pcs, ws_start=start)
 
                 # Completed!
                 return traceback
 
             if "PUSH" in frame.op and frame.pc in contract_src.pcmap:
                 # Check if next op is SSTORE to properly use AST from push op.
                 next_frame = next(trace, None)
+                is_non_payable_hit = False
                 if next_frame and next_frame.op == "SSTORE":
                     push_location = tuple(contract_src.pcmap[frame.pc]["location"])  # type: ignore
                     pcmap = PCMap.parse_obj({next_frame.pc: {"location": push_location}})
                 else:
                     pcmap = contract_src.pcmap
+                    dev_val = str((pcmap[frame.pc].get("dev") or "")).replace("dev: ", "")
+                    is_non_payable_hit = dev_val == RuntimeErrorType.NONPAYABLE_CHECK.value
 
-                if next_frame:
+                if not is_non_payable_hit and next_frame:
                     frame = next_frame
 
             else:
                 pcmap = contract_src.pcmap
 
             if frame.pc not in pcmap:
                 continue
 
             method_id = HexBytes(calldata[:4])
             location = cast(Tuple[int, int, int, int], tuple(pcmap[frame.pc].get("location") or []))
-            dev = str(pcmap[frame.pc].get("dev", "")).replace("dev: ", "")
+            dev_item = pcmap[frame.pc].get("dev", "")
+            dev = str(dev_item).replace("dev: ", "")
             if not location and dev in [m.value for m in RuntimeErrorType]:
                 error_type = RuntimeErrorType(dev)
                 if error_type != RuntimeErrorType.NONPAYABLE_CHECK and traceback.last is not None:
                     # If the error type is not the non-payable check,
                     # it happened in the last method.
                     name = traceback.last.name
 
@@ -593,26 +609,18 @@
                     method_checked = contract_src.contract_type.methods[method_id]
                     name = method_checked.name
 
                 else:
                     # Not sure if possible to get here.
                     name = error_type.name.lower()
 
-                if (
-                    error_type == RuntimeErrorType.NONPAYABLE_CHECK
-                    and traceback.last is not None
-                    and traceback.last.closure.name == name
-                ):
-                    # Prevent weird duplicate non-payable check..
-                    # TODO: Find a better way to do this at compile time.
-                    continue
-
                 # Empty source (is builtin)
-                stmt_type = f"dev: {error_type.value}"
-                traceback.add_builtin_jump(name, stmt_type, self.name)
+                traceback.add_builtin_jump(
+                    name, dev_item, self.name, pcs={frame.pc}, source_path=contract_src.source_path
+                )
                 continue
 
             elif not location:
                 # Unknown.
                 continue
 
             function = contract_src.lookup_function(location, method_id=method_id)
@@ -629,18 +637,21 @@
                     if traceback.last and traceback.last.depth == frame.depth
                     else frame.depth
                 )
                 traceback.add_jump(
                     location,
                     function,
                     depth,
+                    pcs={frame.pc},
                     source_path=contract_src.source_path,
                 )
             else:
-                traceback.extend_last(location)
+                traceback.extend_last(location, pcs={frame.pc})
+
+            last_pc = frame.pc
 
         # Never actually hits this return.
         # See `Completed!` comment above.
         return traceback
 
 
 def _safe_append(data: Dict, version: Union[Version, NpmSpec], paths: Union[Path, Set]):
@@ -648,17 +659,15 @@
         paths = {paths}
     if version in data:
         data[version] = data[version].union(paths)
     else:
         data[version] = paths
 
 
-def _is_revert_jump(
-    op: str, value: Optional[int], revert_pc: int, processed_opcodes: List[str]
-) -> bool:
-    return op == "JUMPI" and value is not None and value == revert_pc and len(processed_opcodes) > 2
+def _is_revert_jump(op: str, value: Optional[int], revert_pc: int) -> bool:
+    return op == "JUMPI" and value is not None and value == revert_pc
 
 
-def _is_nonpayable_check(opcodes: List[str]) -> bool:
+def _has_empty_revert(opcodes: List[str]) -> bool:
     return (len(opcodes) > 12 and opcodes[-13] == "JUMPDEST" and opcodes[-9] == "REVERT") or (
         len(opcodes) > 4 and opcodes[-5] == "JUMPDEST" and opcodes[-1] == "REVERT"
     )
```

### Comparing `ape-vyper-0.6.6/ape_vyper/exceptions.py` & `ape-vyper-0.6.7/ape_vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.7/ape_vyper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.6
+Version: 0.6.7
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -79,22 +80,22 @@
 
 ```yaml
 # Use `voting` example contracts from Vyperlang repo.
 dependencies:
   - name: VyperVoting
     github: vyperlang/vyper
     contracts_folder: examples/voting/
-    version: v0.3.7
+    version: v0.3.8
 
 # Automatically allow importing voting contracts in your project.
 vyper:
   import_remapping:
-    - "voting=VyperVoting@v0.3.7"
+    - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.7
+# @version 0.3.8
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.6/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.7/ape_vyper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 tests/ape-config.yaml
 tests/conftest.py
 tests/test_compiler.py
 tests/ExampleDependency/contracts/Dependency.vy
 tests/contracts/failing_contracts/contract_undeclared_variable.vy
 tests/contracts/failing_contracts/contract_unknown_pragma.vy
 tests/contracts/passing_contracts/contract.vy
+tests/contracts/passing_contracts/contract_37.vy
 tests/contracts/passing_contracts/contract_no_pragma.vy
 tests/contracts/passing_contracts/contract_with_dev_messages.vy
 tests/contracts/passing_contracts/erc20.vy
 tests/contracts/passing_contracts/older_version.vy
 tests/contracts/passing_contracts/registry.vy
 tests/contracts/passing_contracts/traceback_contract.vy
 tests/contracts/passing_contracts/use_iface.vy
```

### Comparing `ape-vyper-0.6.6/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.7/ape_vyper.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-eth-ape<0.7,>=0.6.9
-ethpm-types
+eth-ape<0.7,>=0.6.10
+ethpm-types<0.6,>=0.5.1
 tqdm
 vvm<0.2,>=0.1.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `ape-vyper-0.6.6/pyproject.toml` & `ape-vyper-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/setup.py` & `ape-vyper-0.6.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,20 +53,20 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.9,<0.7",
-        "ethpm-types",  # Use same version as eth-ape
+        "eth-ape>=0.6.10,<0.7",
+        "ethpm-types>=0.5.1,<0.6",  # Currently bumped 1 higher than eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_vyper": ["py.typed"]},
@@ -77,9 +77,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-vyper-0.6.6/tests/conftest.py` & `ape-vyper-0.6.7/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 import ape
 import pytest
 import vvm  # type: ignore
 
 from ape_vyper.compiler import VyperCompiler
 
 # NOTE: Ensure that we don't use local paths for these
-ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
-ape.config.PROJECT_FOLDER = Path(mkdtemp()).resolve()
+DATA_FOLDER = Path(mkdtemp()).resolve()
+PROJECT_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
+ape.config.PROJECT_FOLDER = PROJECT_FOLDER
+
+# Needed for integration testing
+pytest_plugins = ["pytester"]
 
 
 @contextmanager
 def _tmp_vvm_path(monkeypatch):
     vvm_install_path = mkdtemp()
 
     monkeypatch.setenv(
@@ -59,14 +64,24 @@
     Creates a new, temporary installation path for vvm for a given test.
     """
     with _tmp_vvm_path(monkeypatch) as path:
         yield path
 
 
 @pytest.fixture
+def data_folder():
+    return DATA_FOLDER
+
+
+@pytest.fixture
+def project_folder():
+    return PROJECT_FOLDER
+
+
+@pytest.fixture
 def compiler():
     return VyperCompiler()
 
 
 @pytest.fixture
 def config():
     return ape.config
```

### Comparing `ape-vyper-0.6.6/tests/contracts/passing_contracts/contract.vy` & `ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_37.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.6.7/tests/contracts/passing_contracts/erc20.vy`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# @version ^0.3.7
+# @version ^0.3.8
 # @dev Implementation of ERC-20 token standard.
 # @author Takayuki Jimba (@yudetamago)
 # https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md
 
 from vyper.interfaces import ERC20
 from vyper.interfaces import ERC20Detailed
```

### Comparing `ape-vyper-0.6.6/tests/contracts/passing_contracts/traceback_contract.vy` & `ape-vyper-0.6.7/tests/contracts/passing_contracts/traceback_contract.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.6/tests/test_compiler.py` & `ape-vyper-0.6.7/tests/test_compiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 import pytest
 from ape.exceptions import ContractLogicError
 from semantic_version import Version  # type: ignore
 from vvm import compile_source  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.compiler import RuntimeErrorType
-from ape_vyper.exceptions import IntegerOverflowError, VyperCompileError, VyperInstallError
+from ape_vyper.exceptions import (
+    IntegerOverflowError,
+    NonPayableError,
+    VyperCompileError,
+    VyperInstallError,
+)
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
 PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 
 # Currently, this is the only version specified from a pragma spec
 OLDER_VERSION_FROM_PRAGMA = Version("0.2.8")
-VERSION_FROM_PRAGMA = Version("0.3.7")
+VERSION_37 = Version("0.3.7")
+VERSION_FROM_PRAGMA = Version("0.3.8")
 
 
 @pytest.fixture
 def dev_revert_source():
     return PASSING_BASE / "contract_with_dev_messages.vy"
 
 
@@ -72,35 +78,33 @@
 
 
 def test_get_version_map(project, compiler):
     vyper_files = [
         x for x in project.contracts_folder.iterdir() if x.is_file() and x.suffix == ".vy"
     ]
     actual = compiler.get_version_map(vyper_files)
-    expected_versions = (OLDER_VERSION_FROM_PRAGMA, VERSION_FROM_PRAGMA)
+    expected_versions = (OLDER_VERSION_FROM_PRAGMA, VERSION_FROM_PRAGMA, VERSION_37)
 
     for version, sources in actual.items():
         if version in expected_versions:
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
         fail_message = f"Unexpected version '{version}' with sources: {sources}"
         pytest.fail(fail_message)
 
     assert len(actual[OLDER_VERSION_FROM_PRAGMA]) == 1
-    assert len(actual[VERSION_FROM_PRAGMA]) == 8
+    assert len(actual[VERSION_FROM_PRAGMA]) == 6
     assert actual[OLDER_VERSION_FROM_PRAGMA] == {project.contracts_folder / "older_version.vy"}
 
     expected = (
         "contract.vy",
         "contract_no_pragma.vy",
         "contract_with_dev_messages.vy",
         "erc20.vy",
-        "registry.vy",
-        "traceback_contract.vy",
         "use_iface.vy",
         "use_iface2.vy",
     )
     names = [x.name for x in actual[VERSION_FROM_PRAGMA]]
     failures = []
     missing = []
     for ex in expected:
@@ -120,29 +124,29 @@
 
     assert not failures, "\n".join(failures)
 
 
 def test_compiler_data_in_manifest(project):
     _ = project.contracts
     manifest = project.extract_manifest()
-    assert len(manifest.compilers) == 2, manifest.compilers
+    assert len(manifest.compilers) == 3, manifest.compilers
 
-    vyper_037 = [c for c in manifest.compilers if str(c.version) == str(VERSION_FROM_PRAGMA)][0]
+    vyper_latest = [c for c in manifest.compilers if str(c.version) == str(VERSION_FROM_PRAGMA)][0]
     vyper_028 = [c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)][
         0
     ]
 
-    for compiler in (vyper_028, vyper_037):
+    for compiler in (vyper_028, vyper_latest):
         assert compiler.name == "vyper"
 
-    assert len(vyper_037.contractTypes) == 8
+    assert len(vyper_latest.contractTypes) == 6
     assert len(vyper_028.contractTypes) == 1
-    assert "contract" in vyper_037.contractTypes
+    assert "contract" in vyper_latest.contractTypes
     assert "older_version" in vyper_028.contractTypes
-    for compiler in (vyper_037, vyper_028):
+    for compiler in (vyper_latest, vyper_028):
         assert compiler.settings["evmVersion"] == "constantinople"
         assert compiler.settings["optimize"] is True
 
 
 def test_compile_parse_dev_messages(compiler, dev_revert_source):
     """
     Test parsing of dev messages in a contract. These follow the form of "#dev: ...".
@@ -179,21 +183,22 @@
     assert set(actual["contract.vy"]) == {builtin_import}
     assert len(actual["use_iface.vy"]) == 3
     assert set(actual["use_iface.vy"]) == {local_import, local_from_import, dependency_import}
     assert len(actual["use_iface2.vy"]) == 1
     assert set(actual["use_iface2.vy"]) == {local_import}
 
 
+# TODO: Test this on 0.3.8 and utilize the pcmap from the output.
 def test_pc_map(compiler, project):
     """
     Ensure we de-compress the source map correctly by comparing to the results
     from `compile_src()` which includes the uncompressed source map data.
     """
 
-    path = PASSING_BASE / "contract.vy"
+    path = PASSING_BASE / "contract_37.vy"
     result = compiler.compile([path], base_path=PASSING_BASE)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
     compile_result = compile_source(code, vyper_version="0.3.7")["<stdin>"]
     src_map = compile_result["source_map"]
     lines = code.splitlines()
 
@@ -248,15 +253,15 @@
 
     def line(cont: str) -> int:
         # A helper for getting expected line numbers
         return [i + 1 for i, x in enumerate(lines) if cont in x][0]
 
     # Verify non-payable checks.
     nonpayable_checks = _all(RuntimeErrorType.NONPAYABLE_CHECK)
-    assert len(nonpayable_checks) >= 8
+    assert len(nonpayable_checks) == 1
 
     # Verify integer overflow checks
     overflows = _all(RuntimeErrorType.INTEGER_OVERFLOW)
     overflow_no = line("return (2**127-1) + i")
     assert len(overflows) == 2
     assert overflows[0]["location"] == [overflow_no, 12, overflow_no, 20]
 
@@ -281,20 +286,26 @@
     # Verify index out of range checks
     range_checks = _all(RuntimeErrorType.INDEX_OUT_OF_RANGE)
     range_no = line("return self.dynArray[idx]")
     assert len(range_checks) == 1
     assert range_checks[0]["location"] == [range_no, 11, range_no, 24]
 
 
-def test_enrich_error(compiler, geth_provider, contract, account):
+def test_int_overflow(geth_provider, contract, account):
     int_max = 2**256 - 1
     with pytest.raises(IntegerOverflowError):
         contract.addBalance(int_max, sender=account)
 
 
+def test_non_payable_check(geth_provider, contract, account):
+    with pytest.raises(NonPayableError):
+        contract.addBalance(123, sender=account, value=1)
+
+
+# TODO: Run this test using 0.3.8 as well, once we get the PCMap working.
 def test_trace_source(account, geth_provider, project, contract):
     receipt = contract.addBalance(123, sender=account)
     actual = receipt.source_traceback
     base_folder = project.contracts_folder
     expected = rf"""
 Traceback (most recent call last)
   File {base_folder}/traceback_contract.vy, in addBalance
```


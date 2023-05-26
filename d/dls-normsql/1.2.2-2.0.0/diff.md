# Comparing `tmp/dls-normsql-1.2.2.tar.gz` & `tmp/dls-normsql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-1.2.2.tar", last modified: Wed May 10 05:53:41 2023, max compression
+gzip compressed data, was "dls-normsql-2.0.0.tar", last modified: Fri May 26 07:05:40 2023, max compression
```

## Comparing `dls-normsql-1.2.2.tar` & `dls-normsql-2.0.0.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.453551 dls-normsql-1.2.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.453551 dls-normsql-1.2.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.457551 dls-normsql-1.2.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.453551 dls-normsql-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 05:53:41.000000 dls-normsql-1.2.2/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:41.461551 dls-normsql-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-10 05:53:30.000000 dls-normsql-1.2.2/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_database.py
```

### Comparing `dls-normsql-1.2.2/.dae-devops/Makefile` & `dls-normsql-2.0.0/.dae-devops/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint 3f13d455c444ad39930aabfc68547c2c
+# dae_devops_fingerprint 62bfff1938ace30f8cb33ab30b9c60d5
```

### Comparing `dls-normsql-1.2.2/.dae-devops/docs/developing.rst` & `dls-normsql-2.0.0/.dae-devops/docs/developing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-normsql
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -18,22 +18,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-normsql
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ pip install -e .[dev]
 
 Now you may begin modifying the code.
 
 |
 
 If you plan to modify the docs, you will need to::
 
     $ pip install -e .[docs]
 
     
 
 
-.. # dae_devops_fingerprint 550d6069746935ee4e08d958dd046fa2
+.. # dae_devops_fingerprint 7b83e003f8bbbf54c27b4bd8141fb0e5
```

### Comparing `dls-normsql-1.2.2/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.0.0/.dae-devops/docs/docs_structure.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-normsql
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 68095839584c6e3455c1bd06350312f4
+.. # dae_devops_fingerprint eda941e8a0c3d217a601fb11b90f639b
```

### Comparing `dls-normsql-1.2.2/.dae-devops/docs/installing.rst` & `dls-normsql-2.0.0/.dae-devops/docs/installing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-normsql
 
 Installing
 =======================================================================
 
 
 You will need python 3.9 or later. 
@@ -22,22 +22,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
 You can now use ``pip`` to install the library and its dependencies::
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install dls-normsql
 
 If you require a feature that is not currently released you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-normsql.git
 
-The library should now be installed and the commandline interface on your path.
+The library should now be installed and the commandline should be available.
 You can check the version that has been installed by typing::
 
     $ dls-normsql --version
     $ dls-normsql --version-json
 
-.. # dae_devops_fingerprint f0f3fa3bcf53a551add4ee39538eb44a
+.. # dae_devops_fingerprint a2fe8dfbc79c151a5b899b244a529aa6
```

### Comparing `dls-normsql-1.2.2/.devcontainer/Dockerfile` & `dls-normsql-2.0.0/.devcontainer/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-normsql"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 41ae7527130d2727aa06cd91ff8e5702
+# dae_devops_fingerprint a5c05253a7982ce4ee2e60abd1a254f0
```

### Comparing `dls-normsql-1.2.2/.devcontainer/devcontainer.json` & `dls-normsql-2.0.0/.devcontainer/devcontainer.json`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name dls-normsql
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint bf6676a0739eeb0e671f3518d7739877
+// dae_devops_fingerprint 1c59c18009b5b4578be9201b399a2b6c
```

### Comparing `dls-normsql-1.2.2/.github/CONTRIBUTING.rst` & `dls-normsql-2.0.0/.github/CONTRIBUTING.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-normsql
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-normsql/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint e4fc983b36dd78a7c7fefcb6ac9fdd13
+.. # dae_devops_fingerprint 1e4da81da23bd1f1ea6d675517d6f9c5
```

### Comparing `dls-normsql-1.2.2/.github/actions/install_requirements/action.yml` & `dls-normsql-2.0.0/.github/actions/install_requirements/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint 8d7ad9a9e4bbb3b504abc3a0f33579ee
+# dae_devops_fingerprint 66e539b4856f80b66acfd95402e76d05
```

### Comparing `dls-normsql-1.2.2/.github/dependabot.yml` & `dls-normsql-2.0.0/.github/dependabot.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint b8759630d6502121150bac83a60ac05d
+# dae_devops_fingerprint 61dd9f51dc2d4a0486ac8a76be91051f
```

### Comparing `dls-normsql-1.2.2/.github/pages/make_switcher.py` & `dls-normsql-2.0.0/.github/pages/make_switcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint 321882bf975a37cedc9e7def02e120fa
+# dae_devops_fingerprint dd357c9cfe8e116f70c977b7d94d62db
```

### Comparing `dls-normsql-1.2.2/.github/workflows/code.yml` & `dls-normsql-2.0.0/.github/workflows/code.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -35,15 +35,15 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.10", "3.11"]
+        python: ["3.10"]
         install: ["-e .[dev,docs]"]
         # Make one version be non-editable to test both paths of version code
         include:
           - os: "ubuntu-latest"
             python: "3.9"
             install: ".[dev,docs]"
 
@@ -65,14 +65,18 @@
           python_version: ${{ matrix.python }}
           requirements_file: requirements-test-${{ matrix.os }}-${{ matrix.python }}.txt
           install_options: ${{ matrix.install }}
 
       - name: List dependency tree
         run: pipdeptree
 
+      # TODO: Make startup of MySQL able to be configured.
+      - name: Start up the MySQL that comes with Unbuntu
+        run: sudo /etc/init.d/mysql start
+
       - name: Run tests
         run: |
           sudo apt install environment-modules
           export MODULESHOME=/usr/share/modules
           source $MODULESHOME/init/bash
           pytest
 
@@ -208,8 +212,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 0eca35d77828ef5ba3c51d0d68628f12
+# dae_devops_fingerprint d13e8289ca6252679ab7d9ae8db75617
```

### Comparing `dls-normsql-1.2.2/.github/workflows/docs.yml` & `dls-normsql-2.0.0/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint ea6935f4eb0060233fc35dcccd2a0a36
+# dae_devops_fingerprint 0c3ce8bebad77dab099617eae89e2247
```

### Comparing `dls-normsql-1.2.2/.github/workflows/docs_clean.yml` & `dls-normsql-2.0.0/.github/workflows/docs_clean.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint 53d885e9033e0abb28bcc63d8252ca03
+# dae_devops_fingerprint b47d6e45e6ea9f929b8afe4f238d9473
```

### Comparing `dls-normsql-1.2.2/.github/workflows/linkcheck.yml` & `dls-normsql-2.0.0/.github/workflows/linkcheck.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 name: Link Check
 
 on:
   workflow_dispatch:
   schedule:
@@ -23,8 +23,8 @@
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
 
       - name: Check links
         run: tox -e docs build -- -b linkcheck
 
-# dae_devops_fingerprint f31df44c662aa0a356bb2a62fe64eade
+# dae_devops_fingerprint 674bb9fc122cc739ba92fe18045f0f1f
```

### Comparing `dls-normsql-1.2.2/.gitignore` & `dls-normsql-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/.gitlab-ci.yml` & `dls-normsql-2.0.0/.gitlab-ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 19ac89e7287f70ae7f5f96292102fde8
+# dae_devops_fingerprint f4eece0911ee4d3dbab40d858bc4962d
```

### Comparing `dls-normsql-1.2.2/.vscode/launch.json` & `dls-normsql-2.0.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/LICENSE` & `dls-normsql-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/PKG-INFO` & `dls-normsql-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 1.2.2
+Version: 2.0.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-1.2.2/README.rst` & `dls-normsql-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/docs/conf.py` & `dls-normsql-2.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 404e6b95750b57333b0799fcd1a2c408
+# dae_devops_fingerprint cd8b8b6c6077d960c9ed6af1579909b3
```

### Comparing `dls-normsql-1.2.2/docs/images/dls-favicon.ico` & `dls-normsql-2.0.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/docs/images/dls-logo.svg` & `dls-normsql-2.0.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/pyproject.toml` & `dls-normsql-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-normsql
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Normalized API over various sql libraries."
-dependencies = ["aiosqlite", "dls-utilpack"]
+dependencies = ["dls-utilpack", "aiosqlite", "aiomysql", "cryptography"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
@@ -98,8 +98,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint a8f7c8e6af4793c950a1b15a2e697dcb
+# dae_devops_fingerprint ecc6232348dbe2bd0e46bde0c1961e3b
```

### Comparing `dls-normsql-1.2.2/src/dls_normsql/__main__.py` & `dls-normsql-2.0.0/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.0.0/src/dls_normsql/aiosqlite.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # This class produces log entries.
 import logging
 import os
 import re
 import shutil
 from collections import OrderedDict
 from datetime import datetime
-from typing import Optional
 
 import aiosqlite
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain
 from dls_utilpack.isodatetime import isodatetime_filename
@@ -36,47 +35,52 @@
 # ----------------------------------------------------------------------------------------
 class Aiosqlite:
     """
     Class with coroutines for creating and querying a sqlite database.
     """
 
     # ----------------------------------------------------------------------------------------
-    def __init__(self, specification):
+    def __init__(self, specification, database_definition_object):
         """
         Construct object.  Do not connect to database.
         """
         self.__filename = require(
             f"{callsign(self)} specification", specification, "filename"
         )
 
+        # Default is an empty type_specific_tbd.
+        self.__type_specific_tbd = specification.get("type_specific_tbd", {})
+
         # Backup directory default is the path where the filename is.
         self.__backup_directory = specification.get(
             "backup_directory", os.path.dirname(self.__filename)
         )
 
         # Don't normally want to see all the debug for aiosqlite internals.
         level = specification.get("log_level", "INFO")
         logging.getLogger("aiosqlite").setLevel(level)
 
         self.__connection = None
 
+        self.__database_definition_object = database_definition_object
+
         self.__tables = {}
 
         # Deriving class has not established its latest revision?
         if not hasattr(self, "LATEST_REVISION") or self.LATEST_REVISION is None:
             # Presume it is 1.
             self.LATEST_REVISION = 1
 
         self.__backup_restore_lock = asyncio.Lock()
 
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
-    async def connect(self):
+    async def connect(self, should_drop_database=False):
         """
         Connect to database at filename given in constructor.
         """
 
         async with connect_lock:
             should_create_schemas = False
 
@@ -88,14 +92,25 @@
                 should_create_schemas = True
 
             logger.debug(f"connecting to {self.__filename}")
 
             self.__connection = await aiosqlite.connect(self.__filename)
             self.__connection.row_factory = aiosqlite.Row
 
+            # Set isolation level such that all statements which are not already in an explicit transaction
+            # are autocommitted immediately and visible on other connections.
+            # This might be less efficient?  But it's nice when monitoring a sqlite file with a management tool.
+            # TODO: Consider the ramifications of setting aiosqlite isolation_level to None.
+            # Possible values are None, '' (default), DEFERRED, and EXCLUSIVE.
+            isolation_level = self.__type_specific_tbd.get("isolation_level", None)
+            self.__connection.isolation_level = isolation_level
+            logger.debug(
+                f"isolation_level is now set to '{self.__connection.isolation_level}'"
+            )
+
             # rows = await self.query("PRAGMA journal_mode", why="query journal mode")
             # logger.debug(f"journal mode rows {json.dumps(rows)}")
 
             # rows = await self.query("PRAGMA journal_mode=OFF", why="turn OFF journal mode")
             # logger.debug(f"journal mode OFF rows {json.dumps(rows)}")
 
             # rows = await self.query("PRAGMA journal_mode", why="query journal mode")
@@ -174,14 +189,17 @@
         # Updating to revision 1 presumably means
         # this is a legacy database with no revision table in it.
         if revision == 1:
             logger.info(f"creating {Tablenames.REVISION} table")
             await self.create_table(Tablenames.REVISION)
             await self.insert(Tablenames.REVISION, [{"revision": revision}])
 
+        # Let the database definition object do its thing.
+        self.__database_definition_object.apply_revisions(self)
+
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self.__connection is not None:
             logger.debug(f"[DISSHU] {callsign(self)} disconnecting")
             await self.__connection.close()
             self.__connection = None
@@ -204,43 +222,55 @@
         self.__tables[table_definition.name] = table_definition
 
     # ----------------------------------------------------------------------------------------
     async def add_table_definitions(self):
 
         self.add_table_definition(RevisionTableDefinition(self))
 
+        # Let the database definition object do its thing.
+        await self.__database_definition_object.add_table_definitions(self)
+
+    # ----------------------------------------------------------------------------------------
+    async def begin(self):
+        """
+        Begin transaction.
+        """
+
+        await self.__connection.execute("BEGIN")
+
     # ----------------------------------------------------------------------------------------
     async def commit(self):
         """
-        Commit transaction, if any outstanding.
+        Commit transaction.
         """
 
-        if self.__connection.in_transaction:
-            await self.__connection.commit()
+        await self.__connection.commit()
 
     # ----------------------------------------------------------------------------------------
     async def rollback(self):
         """
-        Roll back transaction, if any outstanding.
+        Roll back transaction.
         """
 
-        if self.__connection.in_transaction:
-            await self.__connection.rollback()
+        await self.__connection.rollback()
 
     # ----------------------------------------------------------------------------------------
-    async def create_schemas(self, should_commit: Optional[bool] = True):
+    async def create_schemas(self):
 
-        for table in self.__tables.values():
-            await self.create_table(table, should_commit=False)
+        await self.begin()
 
-        if should_commit:
-            await self.__connection.commit()
+        try:
+            for table in self.__tables.values():
+                await self.create_table(table)
+            await self.commit()
+        except Exception:
+            await self.rollback()
 
     # ----------------------------------------------------------------------------------------
-    async def create_table(self, table, should_commit: Optional[bool] = True):
+    async def create_table(self, table):
         """
         Wipe and re-create the table in the database.
         """
 
         # If table is a string, presume it's a table name.
         if isinstance(table, str):
             table = require("table definitions", self.__tables, table)
@@ -248,40 +278,36 @@
         await self.__connection.execute("DROP TABLE IF EXISTS %s" % (table.name))
 
         fields_sql = []
         indices_sql = []
 
         for field_name in table.fields:
             field = table.fields[field_name]
-            fields_sql.append("%s %s" % (field_name, field["type"]))
+            fields_sql.append("`%s` %s" % (field_name, field["type"]))
             if field.get("index"):
                 indices_sql.append(
-                    "CREATE INDEX %s_%s ON %s(%s)"
+                    "CREATE INDEX `%s_%s` ON `%s`(`%s`)"
                     % (table.name, field_name, table.name, field_name)
                 )
 
-        sql = "CREATE TABLE %s\n(%s)" % (table.name, ",\n  ".join(fields_sql))
+        sql = "CREATE TABLE `%s`\n(%s)" % (table.name, ",\n  ".join(fields_sql))
 
         logger.debug("\n%s\n%s" % (sql, "\n".join(indices_sql)))
 
         await self.__connection.execute(sql)
 
         for sql in indices_sql:
             await self.__connection.execute(sql)
 
-        if should_commit:
-            await self.__connection.commit()
-
     # ----------------------------------------------------------------------------------------
     async def insert(
         self,
         table,
         rows,
         why=None,
-        should_commit: Optional[bool] = True,
     ) -> None:
         """
         Insert one or more rows.
         Each row is a dictionary.
         The first row is expected to define the keys for all rows inserted.
         Keys in the rows are ignored if not defined in the table schema.
         Table schema columns not specified in the first row's keys will get their sql-defined default values.
@@ -330,32 +356,28 @@
             await self.__connection.executemany(sql, values_rows)
 
             if why is None:
                 logger.debug("\n%s\n%s" % (sql, values_rows))
             else:
                 logger.debug("%s:\n%s\n%s" % (why, sql, values_rows))
 
-            if should_commit:
-                await self.__connection.commit()
-
         except aiosqlite.OperationalError:
             if why is None:
                 raise RuntimeError(f"failed to execute {sql}")
             else:
                 raise RuntimeError(f"failed to execute {why}: {sql}")
 
     # ----------------------------------------------------------------------------------------
     async def update(
         self,
         table,
         row,
         where,
         subs=None,
         why=None,
-        should_commit: Optional[bool] = True,
     ):
         """
         Update specified fields to all rows matching selection.
         """
 
         # If table is a string, presume it's a table name.
         if isinstance(table, str):
@@ -384,17 +406,14 @@
         if subs is not None:
             values_row.extend(subs)
 
         try:
             cursor = await self.__connection.execute(sql, values_row)
             rowcount = cursor.rowcount
 
-            if should_commit:
-                await self.__connection.commit()
-
             if why is None:
                 logger.debug(
                     "%d rows from:\n%s\nvalues %s" % (rowcount, sql, values_row)
                 )
             else:
                 logger.debug(
                     "%d rows from %s:\n%s\nvalues %s" % (rowcount, why, sql, values_row)
@@ -405,34 +424,29 @@
                 raise RuntimeError(f"failed to execute {sql}")
             else:
                 raise RuntimeError(f"failed to execute {why}: {sql}")
 
         return rowcount
 
     # ----------------------------------------------------------------------------------------
-    async def execute(
-        self, sql, subs=None, why=None, should_commit: Optional[bool] = True
-    ):
+    async def execute(self, sql, subs=None, why=None):
         """
         Execute a sql statement.
         If subs is a list of lists, then these are presumed the values for executemany.
         """
 
         cursor = None
         try:
             # Subs is a list of lists?
             if isinstance(subs, list) and len(subs) > 0 and isinstance(subs[0], list):
                 logger.debug(f"inserting {len(subs)} of {len(subs[0])}")
                 cursor = await self.__connection.executemany(sql, subs)
             else:
                 cursor = await self.__connection.execute(sql, subs)
 
-            if should_commit:
-                await self.__connection.commit()
-
             if why is None:
                 if cursor.rowcount > 0:
                     logger.debug(
                         f"{cursor.rowcount} records affected by\n{sql} values {subs}"
                     )
                 else:
                     logger.debug(f"{sql} values {subs}")
```

### Comparing `dls-normsql-1.2.2/src/dls_normsql/constants.py` & `dls-normsql-2.0.0/src/dls_normsql/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ----------------------------------------------------------------------------------------
 class ClassTypes:
     AIOSQLITE = "dls_normsql.aiosqlite"
+    AIOMYSQL = "dls_normsql.aiomysql"
 
 
 # ----------------------------------------------------------------------------------------
 class Tablenames:
     REVISION = "revision"
```

### Comparing `dls-normsql-1.2.2/src/dls_normsql/databases.py` & `dls-normsql-2.0.0/src/dls_normsql/databases.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 class Databases:
     """
     List of available databases.
     """
 
     # ----------------------------------------------------------------------------------------
-    def build_object(self, specification):
+    def build_object(self, specification, database_definition_object):
         """"""
 
         class_type = require("database specification", specification, "type")
         database_class = self.lookup_class(class_type)
 
         try:
-            database_object = database_class(specification)
+            database_object = database_class(specification, database_definition_object)
         except Exception as exception:
             raise RuntimeError(
                 "unable to build database object for type %s" % (database_class)
             ) from exception
 
         return database_object
 
@@ -39,8 +39,13 @@
         """"""
 
         if class_type == ClassTypes.AIOSQLITE:
             from dls_normsql.aiosqlite import Aiosqlite
 
             return Aiosqlite
 
+        if class_type == ClassTypes.AIOMYSQL:
+            from dls_normsql.aiomysql import Aiomysql
+
+            return Aiomysql
+
         raise NotFound("unable to get database class for type %s" % (class_type))
```

### Comparing `dls-normsql-1.2.2/src/dls_normsql/version.py` & `dls-normsql-2.0.0/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.0.0/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 1.2.2
+Version: 2.0.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-1.2.2/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.0.0/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 docs/api/index.rst
 docs/api/modules.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
 src/dls_normsql/__init__.py
 src/dls_normsql/__main__.py
 src/dls_normsql/_version.py
+src/dls_normsql/aiomysql.py
 src/dls_normsql/aiosqlite.py
 src/dls_normsql/constants.py
 src/dls_normsql/databases.py
 src/dls_normsql/exceptions.py
 src/dls_normsql/table_definition.py
 src/dls_normsql/version.py
 src/dls_normsql.egg-info/PKG-INFO
@@ -51,10 +52,12 @@
 src/dls_normsql.egg-info/dependency_links.txt
 src/dls_normsql.egg-info/entry_points.txt
 src/dls_normsql.egg-info/requires.txt
 src/dls_normsql.egg-info/top_level.txt
 tests/__init__.py
 tests/base_tester.py
 tests/conftest.py
+tests/my_database_definition.py
 tests/my_table_definition.py
+tests/test_aiomysql.py
 tests/test_backup_restore.py
 tests/test_database.py
```

### Comparing `dls-normsql-1.2.2/tests/base_tester.py` & `dls-normsql-2.0.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.2/tests/conftest.py` & `dls-normsql-2.0.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,20 +30,15 @@
     logging.getLogger().addHandler(logger)
 
     # Log level for all modules.
     logging.getLogger().setLevel("DEBUG")
 
     # Turn off noisy debug.
     logging.getLogger("asyncio").setLevel("WARNING")
-    logging.getLogger("pika").setLevel("WARNING")
-    logging.getLogger("stomp").setLevel("WARNING")
-    logging.getLogger("luigi-interface").setLevel("WARNING")
-    logging.getLogger("luigi.bx_scheduler").setLevel("INFO")
     logging.getLogger("urllib3.connectionpool").setLevel("INFO")
-
     logging.getLogger("dls_utilpack.things").setLevel("INFO")
 
     # Cover the version.
     # logger.info("\n%s", (json.dumps(version_meta(), indent=4)))
 
     yield None
```

### Comparing `dls-normsql-1.2.2/tests/my_table_definition.py` & `dls-normsql-2.0.0/tests/my_table_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
             "type": "TEXT PRIMARY KEY",
             "index": True,
         }
 
         self.fields[CommonFieldnames.CREATED_ON] = {"type": "TEXT", "index": True}
         self.fields["my_field"] = {"type": "TEXT", "index": True}
 
-        for i in range(200):
+        for i in range(10):
             self.fields["my_other_field_%03d" % (i)] = {"type": "TEXT", "index": True}
```

### Comparing `dls-normsql-1.2.2/tests/test_backup_restore.py` & `dls-normsql-2.0.0/tests/test_backup_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from dls_normsql.constants import ClassTypes, CommonFieldnames
 from dls_normsql.databases import Databases
 from tests.base_tester import BaseTester
-from tests.my_table_definition import MyTableDefinition
+from tests.my_database_definition import MyDatabaseDefinition
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
 class TestBackupRestore:
     def test(self, logging_setup, output_directory):
@@ -32,18 +32,21 @@
 class DatabaseTester(BaseTester):
     """
     Test direct SQL access to the database.
     """
 
     async def _main_coroutine(self, database_specification, output_directory):
         """ """
+        database_definition_object = MyDatabaseDefinition()
 
         databases = Databases()
-        database = databases.build_object(database_specification)
-        database.add_table_definition(MyTableDefinition())
+        database = databases.build_object(
+            database_specification,
+            database_definition_object,
+        )
 
         all_sql = "SELECT * FROM my_table"
 
         try:
             # Connect to database.
             await database.connect()
```


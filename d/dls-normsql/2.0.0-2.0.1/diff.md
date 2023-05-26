# Comparing `tmp/dls-normsql-2.0.0.tar.gz` & `tmp/dls-normsql-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-2.0.0.tar", last modified: Fri May 26 07:05:40 2023, max compression
+gzip compressed data, was "dls-normsql-2.0.1.tar", last modified: Fri May 26 09:35:12 2023, max compression
```

## Comparing `dls-normsql-2.0.0.tar` & `dls-normsql-2.0.1.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.481803 dls-normsql-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.485803 dls-normsql-2.0.0/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24055 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 07:05:40.000000 dls-normsql-2.0.0/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:40.489803 dls-normsql-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/my_database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 07:05:30.000000 dls-normsql-2.0.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.163949 dls-normsql-2.0.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22334 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_revision.py
```

### Comparing `dls-normsql-2.0.0/.dae-devops/Makefile` & `dls-normsql-2.0.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/conventions.rst` & `dls-normsql-2.0.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/developing.rst` & `dls-normsql-2.0.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/devops.rst` & `dls-normsql-2.0.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.0.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/installing.rst` & `dls-normsql-2.0.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/docs/testing.rst` & `dls-normsql-2.0.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.dae-devops/project.yaml` & `dls-normsql-2.0.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.devcontainer/Dockerfile` & `dls-normsql-2.0.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.devcontainer/devcontainer.json` & `dls-normsql-2.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/CONTRIBUTING.rst` & `dls-normsql-2.0.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/actions/install_requirements/action.yml` & `dls-normsql-2.0.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/dependabot.yml` & `dls-normsql-2.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/pages/make_switcher.py` & `dls-normsql-2.0.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/workflows/code.yml` & `dls-normsql-2.0.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/workflows/docs.yml` & `dls-normsql-2.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/workflows/docs_clean.yml` & `dls-normsql-2.0.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.github/workflows/linkcheck.yml` & `dls-normsql-2.0.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.gitignore` & `dls-normsql-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.gitlab-ci.yml` & `dls-normsql-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/.vscode/launch.json` & `dls-normsql-2.0.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/LICENSE` & `dls-normsql-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/PKG-INFO` & `dls-normsql-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.0.0
+Version: 2.0.1
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.0.0/README.rst` & `dls-normsql-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/docs/conf.py` & `dls-normsql-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/docs/images/dls-favicon.ico` & `dls-normsql-2.0.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/docs/images/dls-logo.svg` & `dls-normsql-2.0.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/pyproject.toml` & `dls-normsql-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/src/dls_normsql/__main__.py` & `dls-normsql-2.0.1/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/src/dls_normsql/aiomysql.py` & `dls-normsql-2.0.1/src/dls_normsql/aiomysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import asyncio
-import glob
 
 # This class produces log entries.
 import logging
 import os
-import shutil
 import warnings
 from collections import OrderedDict
 from datetime import datetime
 from typing import Any, List
 
 import aiomysql
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.envvar import Envvar
 from dls_utilpack.explain import explain
-from dls_utilpack.isodatetime import isodatetime_filename
 from dls_utilpack.require import require
 
 from dls_normsql.constants import CommonFieldnames, RevisionFieldnames, Tablenames
 from dls_normsql.table_definition import TableDefinition
 
 logger = logging.getLogger(__name__)
 
@@ -73,19 +70,14 @@
 
         self.__database_name = require(s, t, "database_name")
 
         self.__connection = None
 
         self.__tables = {}
 
-        # Deriving class has not established its latest revision?
-        if not hasattr(self, "LATEST_REVISION") or self.LATEST_REVISION is None:
-            # Presume it is 1.
-            self.LATEST_REVISION = 1
-
         self.__backup_restore_lock = asyncio.Lock()
 
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
     def __parameterize(self, sql: str, subs: List[Any]):
@@ -143,20 +135,21 @@
 
             # Let the base class contribute its table definitions to the in-memory list.
             await self.add_table_definitions()
 
             if should_create_schemas:
                 await self.create_schemas()
                 await self.insert(
-                    Tablenames.REVISION, [{"number": self.LATEST_REVISION}]
+                    Tablenames.REVISION,
+                    [{"number": self.__database_definition_object.LATEST_REVISION}],
                 )
 
             # Emit the name of the database file for positive confirmation on console.
             logger.info(
-                f"{callsign(self)} database name is {self.__database_name} code revision {self.LATEST_REVISION}"
+                f"{callsign(self)} database name is {self.__database_name} database definition revision {self.__database_definition_object.LATEST_REVISION}"
             )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revisions(self):
         """
         Apply revision updates to databse if needed.
         """
@@ -166,56 +159,61 @@
         async with apply_revisions_lock:
             try:
                 records = await self.query(
                     f"SELECT number FROM {Tablenames.REVISION}",
                     why="get database revision",
                 )
                 if len(records) == 0:
-                    old_revision = 0
+                    database_revision = 0
                 else:
-                    old_revision = records[0]["number"]
+                    database_revision = records[0]["number"]
             except Exception as exception:
                 logger.warning(
                     f"could not get revision, presuming legacy database with no table: {exception}"
                 )
-                old_revision = 0
+                database_revision = 0
 
-            if old_revision < self.LATEST_REVISION:
+            if database_revision < self.__database_definition_object.LATEST_REVISION:
                 # Backup before applying revisions.
                 logger.debug(
-                    f"[BKREVL] backing up before updating from revision {old_revision} to revision {self.LATEST_REVISION}"
+                    f"[BKREVL] backing up before updating from database revision {database_revision}"
+                    f" to definition revision {self.__database_definition_object.LATEST_REVISION}"
                 )
 
                 await self.backup()
 
-                for revision in range(old_revision, self.LATEST_REVISION):
-                    logger.debug(f"updating to revision {revision+1}")
+                for revision in range(
+                    database_revision, self.__database_definition_object.LATEST_REVISION
+                ):
                     await self.apply_revision(revision + 1)
                 await self.update(
                     Tablenames.REVISION,
-                    {"number": self.LATEST_REVISION},
+                    {"number": self.__database_definition_object.LATEST_REVISION},
                     "1 = 1",
                     why="update database revision",
                 )
             else:
                 logger.debug(
-                    f"[BKREVL] no need to update persistent revision {old_revision}"
-                    f" which matches code revision {self.LATEST_REVISION}"
+                    f"[BKREVL] no need to update database revision {database_revision}"
+                    f" which matches definition revision {self.__database_definition_object.LATEST_REVISION}"
                 )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revision(self, revision):
         logger.debug(f"updating to revision {revision}")
         # Updating to revision 1 presumably means
         # this is a legacy database with no revision table in it.
         if revision == 1:
             logger.info(f"creating {Tablenames.REVISION} table")
             await self.create_table(Tablenames.REVISION)
             await self.insert(Tablenames.REVISION, [{"revision": revision}])
 
+        # Let the database definition object do its thing.
+        await self.__database_definition_object.apply_revision(self, revision)
+
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self.__connection is not None:
             # Commit final transaction if not currently autocommitting.
             if not self.__connection.get_autocommit():
                 logger.debug(f"[DISSHU] {callsign(self)} committing final transaction")
@@ -547,86 +545,24 @@
     # ----------------------------------------------------------------------------------------
     async def backup(self):
         """
         Back up database to timestamped location.
         """
 
         async with self.__backup_restore_lock:
-            # Prune all the restores which were orphaned.
-            directory = self.__backup_directory
-            if directory is None:
-                raise RuntimeError("no backup directory supplied in confirmation")
-
-            basename, suffix = os.path.splitext(os.path.basename(self.__database_name))
-
-            filenames = glob.glob(f"{directory}/{basename}.*{suffix}")
-
-            filenames.sort(reverse=True)
-
-            for restore in range(self.__last_restore):
-                logger.debug(
-                    f"[BACKPRU] removing {restore}-th restore {filenames[restore]}"
-                )
-                os.remove(filenames[restore])
-
-            self.__last_restore = 0
-
-            timestamp = isodatetime_filename()
-            to_filename = f"{directory}/{basename}.{timestamp}{suffix}"
-
-            await self.disconnect()
-            try:
-                await self.__create_directory(to_filename)
-                shutil.copy2(self.__database_name, to_filename)
-                logger.debug(f"backed up to {to_filename}")
-            except Exception:
-                raise RuntimeError(
-                    f"copy {self.__database_name} to {to_filename} failed"
-                )
-            finally:
-                await self.connect()
+            pass
 
     # ----------------------------------------------------------------------------------------
     async def restore(self, nth):
         """
         Restore database from timestamped location.
         """
 
         async with self.__backup_restore_lock:
-            directory = self.__backup_directory
-            if directory is None:
-                raise RuntimeError("no backup directory supplied in confirmation")
-
-            basename, suffix = os.path.splitext(os.path.basename(self.__database_name))
-
-            filenames = glob.glob(f"{directory}/{basename}.*{suffix}")
-
-            filenames.sort(reverse=True)
-
-            if nth >= len(filenames):
-                raise RuntimeError(
-                    f"restoration index {nth} is more than available {len(filenames)}"
-                )
-
-            from_filename = filenames[nth]
-
-            await self.disconnect()
-            try:
-                shutil.copy2(from_filename, self.__database_name)
-                logger.debug(
-                    f"restored nth {nth} out of {len(filenames)} from {from_filename}"
-                )
-            except Exception:
-                raise RuntimeError(
-                    f"copy {from_filename} to {self.__database_name} failed"
-                )
-            finally:
-                await self.connect()
-
-            self.__last_restore = nth
+            pass
 
 
 # ----------------------------------------------------------------------------------------
 class RevisionTableDefinition(TableDefinition):
     # ----------------------------------------------------------------------------------------
     def __init__(self, database):
         TableDefinition.__init__(self, "revision")
```

### Comparing `dls-normsql-2.0.0/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.0.1/src/dls_normsql/aiosqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,14 @@
 
         self.__connection = None
 
         self.__database_definition_object = database_definition_object
 
         self.__tables = {}
 
-        # Deriving class has not established its latest revision?
-        if not hasattr(self, "LATEST_REVISION") or self.LATEST_REVISION is None:
-            # Presume it is 1.
-            self.LATEST_REVISION = 1
-
         self.__backup_restore_lock = asyncio.Lock()
 
         # Last undo position.
         self.__last_restore = 0
 
     # ----------------------------------------------------------------------------------------
     async def connect(self, should_drop_database=False):
@@ -122,22 +117,23 @@
 
             # Let the base class contribute its table definitions to the in-memory list.
             await self.add_table_definitions()
 
             if should_create_schemas:
                 await self.create_schemas()
                 await self.insert(
-                    Tablenames.REVISION, [{"number": self.LATEST_REVISION}]
+                    Tablenames.REVISION,
+                    [{"number": self.__database_definition_object.LATEST_REVISION}],
                 )
                 # TODO: Set permission on sqlite file from configuration.
                 os.chmod(self.__filename, 0o666)
 
             # Emit the name of the database file for positive confirmation on console.
             logger.info(
-                f"{callsign(self)} database file is {self.__filename} code revision {self.LATEST_REVISION}"
+                f"{callsign(self)} database file is {self.__filename} database definition revision {self.__database_definition_object.LATEST_REVISION}"
             )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revisions(self):
         """
         Apply revision updates to databse if needed.
         """
@@ -147,58 +143,60 @@
         async with apply_revisions_lock:
             try:
                 records = await self.query(
                     f"SELECT number FROM {Tablenames.REVISION}",
                     why="get database revision",
                 )
                 if len(records) == 0:
-                    old_revision = 0
+                    database_revision = 0
                 else:
-                    old_revision = records[0]["number"]
+                    database_revision = records[0]["number"]
             except Exception as exception:
                 logger.warning(
                     f"could not get revision, presuming legacy database with no table: {exception}"
                 )
-                old_revision = 0
+                database_revision = 0
 
-            if old_revision < self.LATEST_REVISION:
+            if database_revision < self.__database_definition_object.LATEST_REVISION:
                 # Backup before applying revisions.
                 logger.debug(
-                    f"[BKREVL] backing up before updating from revision {old_revision} to revision {self.LATEST_REVISION}"
+                    f"[BKREVL] backing up before updating from database revision {database_revision}"
+                    f" to definition revision {self.__database_definition_object.LATEST_REVISION}"
                 )
 
                 await self.backup()
 
-                for revision in range(old_revision, self.LATEST_REVISION):
-                    logger.debug(f"updating to revision {revision+1}")
+                for revision in range(
+                    database_revision, self.__database_definition_object.LATEST_REVISION
+                ):
                     await self.apply_revision(revision + 1)
                 await self.update(
                     Tablenames.REVISION,
-                    {"number": self.LATEST_REVISION},
+                    {"number": self.__database_definition_object.LATEST_REVISION},
                     "1 = 1",
                     why="update database revision",
                 )
             else:
                 logger.debug(
-                    f"[BKREVL] no need to update persistent revision {old_revision}"
-                    f" which matches code revision {self.LATEST_REVISION}"
+                    f"[BKREVL] no need to update database revision {database_revision}"
+                    f" which matches definition revision {self.__database_definition_object.LATEST_REVISION}"
                 )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revision(self, revision):
         logger.debug(f"updating to revision {revision}")
         # Updating to revision 1 presumably means
         # this is a legacy database with no revision table in it.
         if revision == 1:
             logger.info(f"creating {Tablenames.REVISION} table")
             await self.create_table(Tablenames.REVISION)
             await self.insert(Tablenames.REVISION, [{"revision": revision}])
 
         # Let the database definition object do its thing.
-        self.__database_definition_object.apply_revisions(self)
+        await self.__database_definition_object.apply_revision(self, revision)
 
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self.__connection is not None:
             logger.debug(f"[DISSHU] {callsign(self)} disconnecting")
             await self.__connection.close()
```

### Comparing `dls-normsql-2.0.0/src/dls_normsql/constants.py` & `dls-normsql-2.0.1/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/src/dls_normsql/databases.py` & `dls-normsql-2.0.1/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/src/dls_normsql/version.py` & `dls-normsql-2.0.1/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.0.1/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.0.0
+Version: 2.0.1
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.0.0/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.0.1/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,8 +56,9 @@
 tests/__init__.py
 tests/base_tester.py
 tests/conftest.py
 tests/my_database_definition.py
 tests/my_table_definition.py
 tests/test_aiomysql.py
 tests/test_backup_restore.py
-tests/test_database.py
+tests/test_database.py
+tests/test_revision.py
```

### Comparing `dls-normsql-2.0.0/tests/base_tester.py` & `dls-normsql-2.0.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/tests/conftest.py` & `dls-normsql-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/tests/my_database_definition.py` & `dls-normsql-2.0.1/tests/my_database_definition.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,14 +21,21 @@
         self.LATEST_REVISION = 4
 
     # ----------------------------------------------------------------------------------------
     async def apply_revision(self, database, revision):
 
         logger.debug(f"applying revision {revision}")
 
+        if revision == 4:
+            await database.execute("CREATE TABLE `my_table2` (`number` INTEGER)")
+
+            await database.execute(
+                "ALTER TABLE my_table2 ADD COLUMN string TEXT",
+            )
+
     # ----------------------------------------------------------------------------------------
     async def add_table_definitions(self, database):
         """
         Make all the table definitions.
         """
 
         # Table schemas in our database.
```

### Comparing `dls-normsql-2.0.0/tests/my_table_definition.py` & `dls-normsql-2.0.1/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/tests/test_aiomysql.py` & `dls-normsql-2.0.1/tests/test_aiomysql.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/tests/test_backup_restore.py` & `dls-normsql-2.0.1/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.0/tests/test_database.py` & `dls-normsql-2.0.1/tests/test_database.py`

 * *Files identical despite different names*


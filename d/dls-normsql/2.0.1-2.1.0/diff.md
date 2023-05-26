# Comparing `tmp/dls-normsql-2.0.1.tar.gz` & `tmp/dls-normsql-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-2.0.1.tar", last modified: Fri May 26 09:35:12 2023, max compression
+gzip compressed data, was "dls-normsql-2.1.0.tar", last modified: Fri May 26 15:09:38 2023, max compression
```

## Comparing `dls-normsql-2.0.1.tar` & `dls-normsql-2.1.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.163949 dls-normsql-2.0.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.167949 dls-normsql-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    22334 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.171949 dls-normsql-2.0.1/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 09:35:12.000000 dls-normsql-2.0.1/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:12.175949 dls-normsql-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/my_database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_aiomysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-26 09:35:02.000000 dls-normsql-2.0.1/tests/test_revision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.538672 dls-normsql-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.534671 dls-normsql-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.542672 dls-normsql-2.1.0/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 15:09:38.000000 dls-normsql-2.1.0/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:38.546672 dls-normsql-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/my_database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_aiomysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-26 15:09:29.000000 dls-normsql-2.1.0/tests/test_revision.py
```

### Comparing `dls-normsql-2.0.1/.dae-devops/Makefile` & `dls-normsql-2.1.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/conventions.rst` & `dls-normsql-2.1.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/developing.rst` & `dls-normsql-2.1.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/devops.rst` & `dls-normsql-2.1.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/docs_structure.rst` & `dls-normsql-2.1.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/installing.rst` & `dls-normsql-2.1.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/docs/testing.rst` & `dls-normsql-2.1.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.dae-devops/project.yaml` & `dls-normsql-2.1.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.devcontainer/Dockerfile` & `dls-normsql-2.1.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.devcontainer/devcontainer.json` & `dls-normsql-2.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/CONTRIBUTING.rst` & `dls-normsql-2.1.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/actions/install_requirements/action.yml` & `dls-normsql-2.1.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/dependabot.yml` & `dls-normsql-2.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/pages/make_switcher.py` & `dls-normsql-2.1.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/workflows/code.yml` & `dls-normsql-2.1.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/workflows/docs.yml` & `dls-normsql-2.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/workflows/docs_clean.yml` & `dls-normsql-2.1.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.github/workflows/linkcheck.yml` & `dls-normsql-2.1.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.gitignore` & `dls-normsql-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.gitlab-ci.yml` & `dls-normsql-2.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/.vscode/launch.json` & `dls-normsql-2.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/LICENSE` & `dls-normsql-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/PKG-INFO` & `dls-normsql-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.0.1
+Version: 2.1.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.0.1/README.rst` & `dls-normsql-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/docs/conf.py` & `dls-normsql-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/docs/images/dls-favicon.ico` & `dls-normsql-2.1.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/docs/images/dls-logo.svg` & `dls-normsql-2.1.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/pyproject.toml` & `dls-normsql-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/src/dls_normsql/__main__.py` & `dls-normsql-2.1.0/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/src/dls_normsql/aiomysql.py` & `dls-normsql-2.1.0/src/dls_normsql/aiomysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             if not envvar.is_set:
                 raise RuntimeError(
                     f"configuration error: environment variable {self.__host[1:]} is not set"
                 )
             self.__host = envvar.value
 
         self.__port = require(s, t, "port")
-        if self.__port.startswith("$"):
+        if str(self.__port).startswith("$"):
             envvar = Envvar(self.__port[1:], default=3306)
             if not envvar.is_set:
                 raise RuntimeError(
                     f"configuration error: environment variable {self.__port[1:]} is not set"
                 )
             self.__port = int(envvar.value)
```

### Comparing `dls-normsql-2.0.1/src/dls_normsql/aiosqlite.py` & `dls-normsql-2.1.0/src/dls_normsql/aiosqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,36 +87,14 @@
                 should_create_schemas = True
 
             logger.debug(f"connecting to {self.__filename}")
 
             self.__connection = await aiosqlite.connect(self.__filename)
             self.__connection.row_factory = aiosqlite.Row
 
-            # Set isolation level such that all statements which are not already in an explicit transaction
-            # are autocommitted immediately and visible on other connections.
-            # This might be less efficient?  But it's nice when monitoring a sqlite file with a management tool.
-            # TODO: Consider the ramifications of setting aiosqlite isolation_level to None.
-            # Possible values are None, '' (default), DEFERRED, and EXCLUSIVE.
-            isolation_level = self.__type_specific_tbd.get("isolation_level", None)
-            self.__connection.isolation_level = isolation_level
-            logger.debug(
-                f"isolation_level is now set to '{self.__connection.isolation_level}'"
-            )
-
-            # rows = await self.query("PRAGMA journal_mode", why="query journal mode")
-            # logger.debug(f"journal mode rows {json.dumps(rows)}")
-
-            # rows = await self.query("PRAGMA journal_mode=OFF", why="turn OFF journal mode")
-            # logger.debug(f"journal mode OFF rows {json.dumps(rows)}")
-
-            # rows = await self.query("PRAGMA journal_mode", why="query journal mode")
-            # logger.debug(f"journal mode rows {json.dumps(rows)}")
-
-            # rows = await self.query("SELECT * from mainTable", why="main table check")
-
             await self.__connection.create_function("regexp", 2, sqlite_regexp_callback)
 
             # Let the base class contribute its table definitions to the in-memory list.
             await self.add_table_definitions()
 
             if should_create_schemas:
                 await self.create_schemas()
@@ -194,14 +172,17 @@
         # Let the database definition object do its thing.
         await self.__database_definition_object.apply_revision(self, revision)
 
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self.__connection is not None:
+            # Commit any uncommitted transactions.
+            await self.commit()
+
             logger.debug(f"[DISSHU] {callsign(self)} disconnecting")
             await self.__connection.close()
             self.__connection = None
 
     # ----------------------------------------------------------------------------------------
     async def __create_directory(self, filename):
 
@@ -229,14 +210,17 @@
 
     # ----------------------------------------------------------------------------------------
     async def begin(self):
         """
         Begin transaction.
         """
 
+        # Close off any transactions underway.
+        await self.__connection.commit()
+
         await self.__connection.execute("BEGIN")
 
     # ----------------------------------------------------------------------------------------
     async def commit(self):
         """
         Commit transaction.
         """
```

### Comparing `dls-normsql-2.0.1/src/dls_normsql/constants.py` & `dls-normsql-2.1.0/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/src/dls_normsql/databases.py` & `dls-normsql-2.1.0/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/src/dls_normsql/version.py` & `dls-normsql-2.1.0/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-2.1.0/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 2.0.1
+Version: 2.1.0
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-2.0.1/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-2.1.0/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/base_tester.py` & `dls-normsql-2.1.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/conftest.py` & `dls-normsql-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/my_database_definition.py` & `dls-normsql-2.1.0/tests/my_database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/my_table_definition.py` & `dls-normsql-2.1.0/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/test_aiomysql.py` & `dls-normsql-2.1.0/tests/test_aiomysql.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/test_backup_restore.py` & `dls-normsql-2.1.0/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/test_database.py` & `dls-normsql-2.1.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-2.0.1/tests/test_revision.py` & `dls-normsql-2.1.0/tests/test_revision.py`

 * *Files identical despite different names*


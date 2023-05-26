# Comparing `tmp/dls-servbase-1.3.2.tar.gz` & `tmp/dls-servbase-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.3.2.tar", last modified: Wed May 17 17:39:37 2023, max compression
+gzip compressed data, was "dls-servbase-1.4.0.tar", last modified: Fri May 26 07:16:01 2023, max compression
```

## Comparing `dls-servbase-1.3.2.tar` & `dls-servbase-1.4.0.tar`

### file list

```diff
@@ -1,141 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.299112 dls-servbase-1.3.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.307112 dls-servbase-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.303112 dls-servbase-1.3.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/good_config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.303112 dls-servbase-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.311112 dls-servbase-1.3.2/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.315112 dls-servbase-1.3.2/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.315112 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.315112 dls-servbase-1.3.2/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.315112 dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.315112 dls-servbase-1.3.2/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 17:39:37.000000 dls-servbase-1.3.2/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.319112 dls-servbase-1.3.2/src/dls_servbase_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.319112 dls-servbase-1.3.2/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.319112 dls-servbase-1.3.2/src/dls_servbase_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.319112 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:39:37.323112 dls-servbase-1.3.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/configurations/servbase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-17 17:39:25.000000 dls-servbase-1.3.2/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/good_config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:16:01.566571 dls-servbase-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_gui.py
```

### Comparing `dls-servbase-1.3.2/.dae-devops/Makefile` & `dls-servbase-1.4.0/.dae-devops/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint dc970803af5fac409092e34299b9fa8a
+# dae_devops_fingerprint 7a40fdc6afce4991715aeda7ae70c444
```

### Comparing `dls-servbase-1.3.2/.dae-devops/docs/conventions.rst` & `dls-servbase-1.4.0/.dae-devops/docs/conventions.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint de2f9c8adee74d13de393fe798054c9a
+.. # dae_devops_fingerprint cbd0a78343b6577aa4ddb9d59a242b04
```

### Comparing `dls-servbase-1.3.2/.dae-devops/docs/developing.rst` & `dls-servbase-1.4.0/.dae-devops/docs/developing.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -18,22 +18,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-servbase
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ pip install -e .[dev]
 
 Now you may begin modifying the code.
 
 |
 
 If you plan to modify the docs, you will need to::
 
     $ pip install -e .[docs]
 
     
 
 
-.. # dae_devops_fingerprint 85a9a86c29f573bd408647f7092b6fbe
+.. # dae_devops_fingerprint ac891cf352ef89b3b20d2c601dd9ddc4
```

### Comparing `dls-servbase-1.3.2/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.4.0/.dae-devops/docs/docs_structure.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 4c487ab610c69b04a69e018d6726347d
+.. # dae_devops_fingerprint 6ef08be920f12050c1c579cf6e9d4253
```

### Comparing `dls-servbase-1.3.2/.dae-devops/docs/installing.rst` & `dls-servbase-1.4.0/.dae-devops/docs/installing.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Installing
 =======================================================================
 
 
 You will need python 3.9 or later. 
@@ -22,22 +22,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
 You can now use ``pip`` to install the library and its dependencies::
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install dls-servbase
 
 If you require a feature that is not currently released you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git
 
-The library should now be installed and the commandline interface on your path.
+The library should now be installed and the commandline should be available.
 You can check the version that has been installed by typing::
 
     $ dls-servbase --version
     $ dls-servbase --version-json
 
-.. # dae_devops_fingerprint 4595ce95067039bcca5e2ff516cd03af
+.. # dae_devops_fingerprint 64d7ae0dde8939e479b9c793df928d15
```

### Comparing `dls-servbase-1.3.2/.dae-devops/project.yaml` & `dls-servbase-1.4.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/.devcontainer/Dockerfile` & `dls-servbase-1.4.0/.devcontainer/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-servbase"]
 CMD ["--version"]
 
-# dae_devops_fingerprint d98578ac4f9faec948660e9198138f35
+# dae_devops_fingerprint 80986671f8602f6e4666f78f98141826
```

### Comparing `dls-servbase-1.3.2/.devcontainer/devcontainer.json` & `dls-servbase-1.4.0/.devcontainer/devcontainer.json`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name dls-servbase
 
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
 
-// dae_devops_fingerprint a69fcd5d4332da3e6af3b97a7f171509
+// dae_devops_fingerprint 35358278c2556f05447815a0833301dc
```

### Comparing `dls-servbase-1.3.2/.github/CONTRIBUTING.rst` & `dls-servbase-1.4.0/.github/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name dls-servbase
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-servbase/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 65b30b94836cca6d96fc062a2f20730a
+.. # dae_devops_fingerprint 0f4cbc1f77b787f03a9a4d268ed08055
```

### Comparing `dls-servbase-1.3.2/.github/actions/install_requirements/action.yml` & `dls-servbase-1.4.0/.github/actions/install_requirements/action.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
 
-# dae_devops_fingerprint c59b1a1b3a2300f4ab9f3fc9274b213c
+# dae_devops_fingerprint 492458ca501cde9a298a80a102ff22a4
```

### Comparing `dls-servbase-1.3.2/.github/dependabot.yml` & `dls-servbase-1.4.0/.github/dependabot.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint 122e34b2a7528692f5975e2fb7cc167d
+# dae_devops_fingerprint b5838c5e0d9b5041500c5cb701fb5e5b
```

### Comparing `dls-servbase-1.3.2/.github/pages/make_switcher.py` & `dls-servbase-1.4.0/.github/pages/make_switcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint fe647176edcb02077a904f8e42cf4367
+# dae_devops_fingerprint 7a1b58b851c5198d7d380e4ab78d0b49
```

### Comparing `dls-servbase-1.3.2/.github/workflows/code.yml` & `dls-servbase-1.4.0/.github/workflows/code.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint f06ae327848fe3cd45de89312a6cfadf
+# dae_devops_fingerprint 480a147d8af93a934e6ad0fd272e60e5
```

### Comparing `dls-servbase-1.3.2/.github/workflows/docs.yml` & `dls-servbase-1.4.0/.github/workflows/docs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint 7eb227aeb2a5da22835482ebc7fe11dd
+# dae_devops_fingerprint fb2dde86086783119d0b0b805151bf09
```

### Comparing `dls-servbase-1.3.2/.github/workflows/docs_clean.yml` & `dls-servbase-1.4.0/.github/workflows/docs_clean.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint cd9ac693f5bf252fbaf5c9585cb1dd76
+# dae_devops_fingerprint d46d59a6f5197bd11b1cece615feb4df
```

### Comparing `dls-servbase-1.3.2/.github/workflows/linkcheck.yml` & `dls-servbase-1.4.0/.github/workflows/linkcheck.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint dddcd5c3991c4a5f1f8ae8a99b66fbcb
+# dae_devops_fingerprint 0198bfb9fadda488379138f6b2e7f5e3
```

### Comparing `dls-servbase-1.3.2/.gitignore` & `dls-servbase-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/.gitlab-ci.yml` & `dls-servbase-1.4.0/.gitlab-ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
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
 
-# dae_devops_fingerprint e156b7559726d32f77aea7cfd628aee8
+# dae_devops_fingerprint 814043c19b1379f7f1d7b188546a7734
```

### Comparing `dls-servbase-1.3.2/.vscode/launch.json` & `dls-servbase-1.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/LICENSE` & `dls-servbase-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/PKG-INFO` & `dls-servbase-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.3.2
+Version: 1.4.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.3.2/README.rst` & `dls-servbase-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/docs/conf.py` & `dls-servbase-1.4.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 9cd088d2151788486c59b6e240be074b
+# dae_devops_fingerprint 529445ac120d879ddd71245754e51ecb
```

### Comparing `dls-servbase-1.3.2/docs/images/dls-favicon.ico` & `dls-servbase-1.4.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/docs/images/dls-logo.svg` & `dls-servbase-1.4.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/pyproject.toml` & `dls-servbase-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name dls-servbase
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -98,8 +98,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint b6059f181a9c0125cb482b270e753f4e
+# dae_devops_fingerprint ca7c759c4aa01b455a13284486cf7eaa
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.4.0/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.3.2
+Version: 1.4.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.4.0/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 src/dls_servbase.egg-info/top_level.txt
 src/dls_servbase_api/__init__.py
 src/dls_servbase_api/aiohttp_client.py
 src/dls_servbase_api/constants.py
 src/dls_servbase_api/exceptions.py
 src/dls_servbase_api/databases/__init__.py
 src/dls_servbase_api/databases/constants.py
+src/dls_servbase_api/databases/database_definition.py
+src/dls_servbase_api/databases/table_definitions.py
 src/dls_servbase_api/datafaces/__init__.py
 src/dls_servbase_api/datafaces/aiohttp.py
 src/dls_servbase_api/datafaces/constants.py
 src/dls_servbase_api/datafaces/context.py
 src/dls_servbase_api/datafaces/datafaces.py
 src/dls_servbase_cli/__init__.py
 src/dls_servbase_cli/main.py
@@ -71,24 +73,19 @@
 src/dls_servbase_lib/contexts/base.py
 src/dls_servbase_lib/contexts/classic.py
 src/dls_servbase_lib/contexts/contexts.py
 src/dls_servbase_lib/cookies/__init__.py
 src/dls_servbase_lib/cookies/base.py
 src/dls_servbase_lib/cookies/cookies.py
 src/dls_servbase_lib/cookies/dataface.py
-src/dls_servbase_lib/databases/__init__.py
-src/dls_servbase_lib/databases/aiosqlite.py
-src/dls_servbase_lib/databases/database_definition.py
-src/dls_servbase_lib/databases/databases.py
-src/dls_servbase_lib/databases/table_definitions.py
 src/dls_servbase_lib/datafaces/__init__.py
 src/dls_servbase_lib/datafaces/aiohttp.py
-src/dls_servbase_lib/datafaces/aiosqlite.py
 src/dls_servbase_lib/datafaces/context.py
 src/dls_servbase_lib/datafaces/datafaces.py
+src/dls_servbase_lib/datafaces/normsql.py
 src/dls_servbase_lib/guis/__init__.py
 src/dls_servbase_lib/guis/aiohttp.py
 src/dls_servbase_lib/guis/base.py
 src/dls_servbase_lib/guis/constants.py
 src/dls_servbase_lib/guis/context.py
 src/dls_servbase_lib/guis/guis.py
 src/dls_servbase_lib/guis/html/index.html
@@ -100,8 +97,9 @@
 tests/base_tester.py
 tests/conftest.py
 tests/test_aiohttp.py
 tests/test_database.py
 tests/test_dataface.py
 tests/test_dataface_takeover.py
 tests/test_gui.py
-tests/configurations/servbase.yaml
+tests/configurations/mysql.yaml
+tests/configurations/sqlite.yaml
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.4.0/src/dls_servbase_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_cli/main.py` & `dls-servbase-1.4.0/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_cli/subcommands/start_services.py` & `dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_cli/version.py` & `dls-servbase-1.4.0/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/contexts/base.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/contexts/classic.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/contexts/contexts.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/databases/database_definition.py` & `dls-servbase-1.4.0/src/dls_servbase_api/databases/database_definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from dls_servbase_api.databases.constants import CookieFieldnames, Tablenames
 
 # Base class for all aiosqlite database objects.
-from dls_servbase_lib.databases.table_definitions import CookiesTableDefinition
+from dls_servbase_api.databases.table_definitions import CookiesTableDefinition
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
 class DatabaseDefinition:
     """
@@ -20,31 +20,31 @@
         """
         Construct object.  Do not connect to database.
         """
 
         self.LATEST_REVISION = 2
 
     # ----------------------------------------------------------------------------------------
-    async def apply_revision(self, revision):
+    async def apply_revision(self, database, revision):
         if revision == 2:
-            await self.execute(
+            await database.execute(
                 f"ALTER TABLE {Tablenames.COOKIES} ADD COLUMN {CookieFieldnames.NAME} TEXT",
                 why=f"revision 2: add {Tablenames.COOKIES} {CookieFieldnames.NAME} column",
             )
-            await self.execute(
+            await database.execute(
                 "CREATE INDEX %s_%s ON %s(%s)"
                 % (
                     Tablenames.COOKIES,
                     CookieFieldnames.NAME,
                     Tablenames.COOKIES,
                     CookieFieldnames.NAME,
                 )
             )
 
     # ----------------------------------------------------------------------------------------
-    async def add_table_definitions(self):
+    async def add_table_definitions(self, database):
         """
         Make all the table definitions.
         """
 
         # Table schemas in our database.
-        self.add_table_definition(CookiesTableDefinition())
+        database.add_table_definition(CookiesTableDefinition())
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/databases/databases.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/guis/guis.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,42 +5,68 @@
 from dls_utilpack.things import Things
 
 # Exceptions.
 from dls_servbase_api.exceptions import NotFound
 
 logger = logging.getLogger(__name__)
 
+# -----------------------------------------------------------------------------------------
+__default_dls_servbase_gui = None
 
-class Databases(Things):
+
+def dls_servbase_guis_set_default(dls_servbase_gui):
+    global __default_dls_servbase_gui
+    __default_dls_servbase_gui = dls_servbase_gui
+
+
+def dls_servbase_guis_get_default():
+    global __default_dls_servbase_gui
+    if __default_dls_servbase_gui is None:
+        raise RuntimeError("dls_servbase_guis_get_default instance is None")
+    return __default_dls_servbase_gui
+
+
+def dls_servbase_guis_has_default():
+    global __default_dls_servbase_gui
+    return __default_dls_servbase_gui is not None
+
+
+# -----------------------------------------------------------------------------------------
+
+
+class Guis(Things):
     """
-    List of available databases.
+    List of available dls_servbase_guis.
     """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, name=None):
         Things.__init__(self, name)
 
     # ----------------------------------------------------------------------------------------
     def build_object(self, specification):
         """"""
 
-        database_class = self.lookup_class(specification["type"])
+        dls_servbase_gui_class = self.lookup_class(specification["type"])
 
         try:
-            database_object = database_class(specification)
+            dls_servbase_gui_object = dls_servbase_gui_class(specification)
         except Exception as exception:
             raise RuntimeError(
-                "unable to build database object for type %s" % (database_class)
+                "unable to build dls_servbase_gui object for type %s"
+                % (dls_servbase_gui_class)
             ) from exception
 
-        return database_object
+        return dls_servbase_gui_object
 
     # ----------------------------------------------------------------------------------------
     def lookup_class(self, class_type):
         """"""
 
-        if class_type == "dls_servbase_lib.databases.aiosqlite":
-            from dls_servbase_lib.databases.aiosqlite import Aiosqlite
+        if class_type == "dls_servbase_lib.dls_servbase_guis.aiohttp":
+            from dls_servbase_lib.guis.aiohttp import Aiohttp
 
-            return Aiosqlite
+            return Aiohttp
 
-        raise NotFound("unable to get database class for type %s" % (class_type))
+        raise NotFound(
+            "unable to get dls_servbase_gui class for type %s" % (class_type)
+        )
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/databases/table_definitions.py` & `dls-servbase-1.4.0/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/aiosqlite.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import logging
 
+# Database manager.
+from dls_normsql.databases import Databases
+
 # Base class for generic things.
 from dls_utilpack.thing import Thing
 
 from dls_servbase_api.databases.constants import Tablenames
-
-# Database manager.
-from dls_servbase_lib.databases.databases import Databases
+from dls_servbase_api.databases.database_definition import DatabaseDefinition
 
 logger = logging.getLogger(__name__)
 
-thing_type = "dls_servbase_lib.datafaces.aiosqlite"
+thing_type = "dls_servbase_lib.datafaces.normsql"
 
 
-class Aiosqlite(Thing):
+class Normsql(Thing):
     """ """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
         Thing.__init__(self, thing_type, specification)
 
+        # For testing, caller might want to drop the database on connection.
+        self.__should_drop_database = specification.get("should_drop_database")
+
         self.__database = None
 
     # ----------------------------------------------------------------------------------------
     async def start(self):
         # Connect to the database to create the schemas if they don't exist already.
         await self.establish_database_connection()
 
@@ -33,16 +37,23 @@
             await self.__database.disconnect()
             self.__database = None
 
     # ----------------------------------------------------------------------------------------
     async def establish_database_connection(self):
 
         if self.__database is None:
-            self.__database = Databases().build_object(self.specification()["database"])
-            await self.__database.connect()
+            self.__database = Databases().build_object(
+                self.specification()["database"],
+                DatabaseDefinition(),
+            )
+
+            # For testing, caller might want to drop the database on connection.
+            await self.__database.connect(
+                should_drop_database=self.__should_drop_database
+            )
 
     # ----------------------------------------------------------------------------------------
     async def reinstance(self):
         """"""
         if self.__database is None:
             return
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """"""
 
         if class_type == "dls_servbase_lib.datafaces.aiohttp":
             from dls_servbase_lib.datafaces.aiohttp import Aiohttp
 
             return Aiohttp
 
-        elif class_type == "dls_servbase_lib.datafaces.aiosqlite":
-            from dls_servbase_lib.datafaces.aiosqlite import Aiosqlite
+        elif class_type == "dls_servbase_lib.datafaces.normsql":
+            from dls_servbase_lib.datafaces.normsql import Normsql
 
-            return Aiosqlite
+            return Normsql
 
         raise NotFound(
             "unable to get dls_servbase_dataface class for type %s" % (class_type)
         )
```

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/src/dls_servbase_lib/version.py` & `dls-servbase-1.4.0/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/base.py` & `dls-servbase-1.4.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/base_context_tester.py` & `dls-servbase-1.4.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/base_specification_tester.py` & `dls-servbase-1.4.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/base_tester.py` & `dls-servbase-1.4.0/tests/base_tester.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,7 +29,37 @@
             logger.exception(
                 "unexpected exception in the test method", exc_info=exception
             )
             failure_message = str(exception)
 
         if failure_message is not None:
             pytest.fail(failure_message)
+
+
+# ----------------------------------------------------------------------------------------
+class BaseTester2:
+    """
+    Provide asyncio loop and error checking over *Tester classes.
+    """
+
+    def main(self, constants, specification, output_directory):
+        """
+        This is the main program which calls the test using asyncio.
+        """
+
+        multiprocessing.current_process().name = "main"
+
+        failure_message = None
+        try:
+            # Run main test in asyncio event loop.
+            asyncio.run(
+                self._main_coroutine(constants, specification, output_directory)
+            )
+
+        except Exception as exception:
+            logger.exception(
+                "unexpected exception in the test method", exc_info=exception
+            )
+            failure_message = str(exception)
+
+        if failure_message is not None:
+            pytest.fail(failure_message)
```

### Comparing `dls-servbase-1.3.2/tests/configurations/servbase.yaml` & `dls-servbase-1.4.0/tests/configurations/sqlite.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 type: dls_servbase_lib.dls_servbase_contexts.classic
 
-visit:
-    beamline: b29
-    year: 2022
-    visit: cy29757-3
-    directory: /dls/b29/data/2022/cy29757-3
-    # Format to make actual data_filename using data_label as token.
-    data_path_pattern: "/dls/b29/data/2022/cy29757-3/Merlin/{data_label}_data.mib"
-
 logging_settings:
     console:
         enabled: True
         verbose: True
         filters:
             markers:
                 - "[RELCOOK]"
@@ -27,44 +19,44 @@
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
     dataface_port: &DATAFACE_PORT 27520
-    dls_servbase_gui_server: &DLS_BILLY_GUI_SERVER http://*:22522
-    dls_servbase_gui_client: &DLS_BILLY_GUI_CLIENT http://127.0.0.1:22522
+    dls_servbase_gui_server: &DLS_SERVBASE_GUI_SERVER http://*:22522
+    dls_servbase_gui_client: &DLS_SERVBASE_GUI_CLIENT http://127.0.0.1:22522
 
 # The dls_servbase_dataface client/server composite.
-dls_servbase_dataface_specification: &DLS_BILLY_DATAFACE_SPECIFICATION
+dls_servbase_dataface_specification: &DLS_SERVBASE_DATAFACE_SPECIFICATION
     type: "dls_servbase_lib.datafaces.aiohttp"
     type_specific_tbd:
         # The remote dls_servbase_dataface server access.
         aiohttp_specification:
             server_host: "*"
             client_host: "127.0.0.1"
             port: *DATAFACE_PORT
         # The local implementation of the dls_servbase_dataface.
         actual_dataface_specification:
-            type: "dls_servbase_lib.datafaces.aiosqlite"
+            type: "dls_servbase_lib.datafaces.normsql"
             database:
-                type: "dls_servbase_lib.databases.aiosqlite"
+                type: "dls_normsql.aiosqlite"
                 filename: "${output_directory}/dls_servbase_dataface.sqlite"
                 log_level: "WARNING"
     context:
         start_as: process
 
 # The dls_servbase_gui specification.
 dls_servbase_gui_specification:
     type: "dls_servbase_lib.dls_servbase_guis.aiohttp"
     type_specific_tbd:
         # The remote dls_servbase_gui server access.
         aiohttp_specification:
-            server: *DLS_BILLY_GUI_SERVER
-            client: *DLS_BILLY_GUI_CLIENT
+            server: *DLS_SERVBASE_GUI_SERVER
+            client: *DLS_SERVBASE_GUI_CLIENT
             search_paths: ["examples/html"]
             cookie_specification:
                 type: "dls_servbase_lib.cookies.dataface"
                 type_specific_tbd:
-                    dataface_specification: *DLS_BILLY_DATAFACE_SPECIFICATION
+                    dataface_specification: *DLS_SERVBASE_DATAFACE_SPECIFICATION
     context:
         start_as: process
```

### Comparing `dls-servbase-1.3.2/tests/conftest.py` & `dls-servbase-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/test_aiohttp.py` & `dls-servbase-1.4.0/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.3.2/tests/test_database.py` & `dls-servbase-1.4.0/tests/test_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-import asyncio
 import logging
-import multiprocessing
 
-import pytest
+from dls_normsql.constants import ClassTypes
+from dls_normsql.databases import Databases
 
 from dls_servbase_api.databases.constants import CookieFieldnames, Tablenames
-from dls_servbase_lib.databases.databases import Databases
+from dls_servbase_api.databases.database_definition import DatabaseDefinition
+from tests.base_tester import BaseTester2
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
 class TestDatabaseSqlite:
     def test(self, constants, logging_setup, output_directory):
         """
         Tests the sqlite implementation of the Database interface.
 
         This does not use a service.
         """
 
         database_specification = {
-            "type": "dls_servbase_lib.databases.aiosqlite",
-            "filename": "%s/dls_servbase_scheduler.sqlite" % (output_directory),
+            "type": ClassTypes.AIOSQLITE,
+            "filename": "%s/dls_servbase_pytest.sqlite" % (output_directory),
         }
 
         # Test direct SQL access to the database.
-        DatabaseTesterImage().main(
+        DatabaseTester().main(
             constants,
             database_specification,
             output_directory,
         )
 
 
 # ----------------------------------------------------------------------------------------
-class _BaseTester:
-    """
-    Provide asyncio loop and error checking over *Tester classes.
-    """
-
-    def main(self, constants, specification, output_directory):
-        """
-        This is the main program which calls the test using asyncio.
+class TestDatabaseMysql:
+    def test(self, constants, logging_setup, output_directory):
         """
+        Tests the sqlite implementation of the Database interface.
 
-        multiprocessing.current_process().name = "main"
+        This does not use a service.
+        """
 
-        failure_message = None
-        try:
-            # Run main test in asyncio event loop.
-            asyncio.run(
-                self._main_coroutine(constants, specification, output_directory)
-            )
-
-        except Exception as exception:
-            logger.exception(
-                "unexpected exception in the test method", exc_info=exception
-            )
-            failure_message = str(exception)
+        database_specification = {
+            "type": ClassTypes.AIOMYSQL,
+            "type_specific_tbd": {
+                "database_name": "dls_servbase_pytest",
+                "host": "$MYSQL_HOST",
+                "port": "$MYSQL_PORT",
+                "username": "root",
+                "password": "root",
+            },
+        }
 
-        if failure_message is not None:
-            pytest.fail(failure_message)
+        # Test direct SQL access to the database.
+        DatabaseTester().main(
+            constants,
+            database_specification,
+            output_directory,
+        )
 
 
 # ----------------------------------------------------------------------------------------
-class DatabaseTesterImage(_BaseTester):
+class DatabaseTester(BaseTester2):
     """
     Test direct SQL access to the database.
     """
 
     async def _main_coroutine(
         self, constants, database_specification, output_directory
     ):
         """ """
 
         databases = Databases()
-        database = databases.build_object(database_specification)
+        database = databases.build_object(
+            database_specification,
+            DatabaseDefinition(),
+        )
 
         try:
             # Connect to database.
-            await database.connect()
+            await database.connect(should_drop_database=True)
 
             # Write one record.
             await database.insert(
                 Tablenames.COOKIES,
                 [
                     {
                         CookieFieldnames.UUID: "f0",
```

### Comparing `dls-servbase-1.3.2/tests/test_dataface.py` & `dls-servbase-1.4.0/tests/test_dataface.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,36 @@
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestDataface:
+class TestDatafaceSqlite:
     """
     Test that we can do a basic database operation through the service.
     """
 
     def test(self, constants, logging_setup, output_directory):
         """ """
 
-        configuration_file = "tests/configurations/servbase.yaml"
+        configuration_file = "tests/configurations/sqlite.yaml"
+        DatafaceTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestDatafaceMysql:
+    """
+    Test that we can do a basic database operation through the service.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+        """ """
+
+        configuration_file = "tests/configurations/mysql.yaml"
         DatafaceTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class DatafaceTester(BaseContextTester):
     """
     Class to test the dataface.
```

### Comparing `dls-servbase-1.3.2/tests/test_dataface_takeover.py` & `dls-servbase-1.4.0/tests/test_dataface_takeover.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,32 @@
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestDatafaceTakeover:
-    def test_dataface_laptop(self, constants, logging_setup, output_directory):
+class TestDatafaceTakeoverSqlite:
+    def test(self, constants, logging_setup, output_directory):
         """ """
 
-        configuration_file = "tests/configurations/servbase.yaml"
+        configuration_file = "tests/configurations/sqlite.yaml"
+        DatafaceTakeoverTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestDatafaceTakeoverMysql:
+    """
+    Test that we can do a basic database operation through the service.
+    """
+
+    def test(self, constants, logging_setup, output_directory):
+        """ """
+
+        configuration_file = "tests/configurations/mysql.yaml"
         DatafaceTakeoverTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class DatafaceTakeoverTester(BaseContextTester):
     """
     Class to test that a second instance of the dataface will cause the first one to shut down.
@@ -51,18 +64,49 @@
                     [
                         {
                             CookieFieldnames.UUID: "f0",
                             CookieFieldnames.CONTENTS: "{'a': 'f000'}",
                         }
                     ],
                 )
+                all_sql = f"SELECT * FROM {Tablenames.COOKIES}"
+                records = await dataface.query(all_sql)
 
-            # Make a new dataface context with the same specification.
+                assert len(records) == 1
+                assert records[0][CookieFieldnames.UUID] == "f0"
+                assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f000'}"
+
+            # ----------------------------------------------------------------------------
+            # Make a new dataface context with the same specification, except don't drop.
+            servbase_specification["type_specific_tbd"][
+                "actual_dataface_specification"
+            ]["should_drop_database"] = False
             dls_servbase_server_context = ServerContext(servbase_specification)
             # Activate the new dataface which should send shutdown to the old process.
             async with dls_servbase_server_context:
-                all_sql = f"SELECT * FROM {Tablenames.COOKIES}"
+                # Check the final insert made it to the database.
                 records = await dataface.query(all_sql)
-
                 assert len(records) == 1
                 assert records[0][CookieFieldnames.UUID] == "f0"
                 assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f000'}"
+
+                # Update the cookie record.
+                subs = []
+                subs.append("f0")
+                await dataface.update(
+                    Tablenames.COOKIES,
+                    {CookieFieldnames.CONTENTS: "{'a': 'f001'}"},
+                    f"{CookieFieldnames.UUID} = ?",
+                    subs=subs,
+                    why="update database revision",
+                )
+
+            # ----------------------------------------------------------------------------
+            # Make a new dataface context with the same specification, again without dropping.
+            dls_servbase_server_context = ServerContext(servbase_specification)
+            # Activate the new dataface which should send shutdown to the old process.
+            async with dls_servbase_server_context:
+                # Check the final update made it to the database.
+                records = await dataface.query(all_sql)
+                assert len(records) == 1
+                assert records[0][CookieFieldnames.UUID] == "f0"
+                assert records[0][CookieFieldnames.CONTENTS] == "{'a': 'f001'}"
```

### Comparing `dls-servbase-1.3.2/tests/test_gui.py` & `dls-servbase-1.4.0/tests/test_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     Fetch requests from the dataface similar to what javascript ajax would do.
     """
 
     def test(self, constants, logging_setup, output_directory):
         """ """
 
-        configuration_file = "tests/configurations/servbase.yaml"
+        configuration_file = "tests/configurations/sqlite.yaml"
         GuiTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class GuiTester(BaseContextTester):
     """
     Class with asyncio coroutine which does the actual test.
```


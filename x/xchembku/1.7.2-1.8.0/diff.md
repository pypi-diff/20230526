# Comparing `tmp/xchembku-1.7.2.tar.gz` & `tmp/xchembku-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.7.2.tar", last modified: Wed May 17 11:46:00 2023, max compression
+gzip compressed data, was "xchembku-1.8.0.tar", last modified: Fri May 26 10:46:39 2023, max compression
```

## Comparing `xchembku-1.7.2.tar` & `xchembku-1.8.0.tar`

### file list

```diff
@@ -1,159 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.949607 xchembku-1.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 11:45:51.000000 xchembku-1.7.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-17 11:45:51.000000 xchembku-1.7.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-17 11:45:51.000000 xchembku-1.7.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.933607 xchembku-1.7.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 11:45:51.000000 xchembku-1.7.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-17 11:45:51.000000 xchembku-1.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-17 11:45:51.000000 xchembku-1.7.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-17 11:45:51.000000 xchembku-1.7.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 11:45:51.000000 xchembku-1.7.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-17 11:45:51.000000 xchembku-1.7.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 11:45:51.000000 xchembku-1.7.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 11:45:51.000000 xchembku-1.7.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 11:45:51.000000 xchembku-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-17 11:46:00.949607 xchembku-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 11:45:51.000000 xchembku-1.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-17 11:45:51.000000 xchembku-1.7.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.933607 xchembku-1.7.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.937607 xchembku-1.7.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-17 11:45:51.000000 xchembku-1.7.2/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-17 11:45:51.000000 xchembku-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:46:00.949607 xchembku-1.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.933607 xchembku-1.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_plate_report_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.941607 xchembku-1.7.2/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 11:46:00.000000 xchembku-1.7.2/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17381 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-17 11:45:51.000000 xchembku-1.7.2/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.945607 xchembku-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:46:00.949607 xchembku-1.7.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_crystal_plate_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_crystal_well_droplocation1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_crystal_well_droplocation2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_soakdb3_crystal_well.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-17 11:45:51.000000 xchembku-1.7.2/tests/test_swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 10:46:28.000000 xchembku-1.8.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-26 10:46:28.000000 xchembku-1.8.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-26 10:46:28.000000 xchembku-1.8.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.450141 xchembku-1.8.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.458141 xchembku-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 10:46:28.000000 xchembku-1.8.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-26 10:46:28.000000 xchembku-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-26 10:46:28.000000 xchembku-1.8.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 10:46:28.000000 xchembku-1.8.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 10:46:28.000000 xchembku-1.8.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 10:46:28.000000 xchembku-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-26 10:46:39.478142 xchembku-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-26 10:46:28.000000 xchembku-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-26 10:46:28.000000 xchembku-1.8.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.450141 xchembku-1.8.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.462141 xchembku-1.8.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 10:46:28.000000 xchembku-1.8.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-26 10:46:28.000000 xchembku-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:46:39.478142 xchembku-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.454141 xchembku-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.466141 xchembku-1.8.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_plate_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.470141 xchembku-1.8.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 10:46:39.000000 xchembku-1.8.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.474141 xchembku-1.8.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17383 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-26 10:46:28.000000 xchembku-1.8.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:46:39.478142 xchembku-1.8.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/direct_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/direct_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/service_mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/configurations/service_sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_plate_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_droplocation1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_crystal_well_droplocation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_soakdb3_crystal_well.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 10:46:28.000000 xchembku-1.8.0/tests/test_swiss3.py
```

### Comparing `xchembku-1.7.2/.dae-devops/Makefile` & `xchembku-1.8.0/.dae-devops/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint 37cc3e10ff97563262222c305ac66166
+# dae_devops_fingerprint d50edec1acad9cc9284a1ec9e21055a4
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/conventions.rst` & `xchembku-1.8.0/.dae-devops/docs/conventions.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 62f9350a2bf32c116db81f845c721f6f
+.. # dae_devops_fingerprint 6447195a860d723dc42fcf539bc98512
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/developing.rst` & `xchembku-1.8.0/.dae-devops/docs/developing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
@@ -18,22 +18,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd xchembku
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ pip install -e .[dev]
 
 Now you may begin modifying the code.
 
 |
 
 If you plan to modify the docs, you will need to::
 
     $ pip install -e .[docs]
 
     
 
 
-.. # dae_devops_fingerprint e7e76b1a5311ccf929167c787da25eca
+.. # dae_devops_fingerprint b8e50fbfb03247dcba32527a1bce43ac
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/devops.rst` & `xchembku-1.8.0/.dae-devops/docs/devops.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Devops
 =======================================================================
 
-There exists a a configuration file called ``.dae-devops/project.yaml``.
+In the top level of the repository there exists a configuration file called ``.dae-devops/project.yaml``.
 
 This file defines the project information needed for CI/CD.
 
 It is parsed by the ``dae_devops.force`` command which creates these files:
 
 - pyproject.toml
+- .githib/*
 - .gitlab-ci.yml
 - .dae-devops/Makefile
 - .dae-devops/docs/*
 
 Local CI/CD execution
------------------------------------------------------------------------
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 All the CI/CD ops which are run by the git server can be run at the command line.
 
 Running these ops before pushing to the git server can make the turnaround quicker to fix things.
 
 Follow the steps in the Developing section.  Then you can run the following commands.
 
 Validation of the code::
 
     $ make -f .dae-devops/Makefile validate_pre_commit
     $ make -f .dae-devops/Makefile validate_mypy
     $ make -f .dae-devops/Makefile validate_pytest
     $ make -f .dae-devops/Makefile validate_docs
 
-Packaging:: 
+Packaging (for the Diamond intranet):: 
 
     $ make -f .dae-devops/Makefile package_pip
 
-Publishing::
+Publishing (for the Diamond intranet)::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
+The Diamond intranet commands are not used for production. The production packaging and publishing are handled in the GitHub Actions workflows mechanism.
 
-
-.. # dae_devops_fingerprint 5046f56ff14b58d97e9d1ae6c461f519
+.. # dae_devops_fingerprint ba8ae1a6737f996ecbb36c9b8517feeb
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/docs_structure.rst` & `xchembku-1.8.0/.dae-devops/docs/docs_structure.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 3991a961381331fb710f03dd96c3db0d
+.. # dae_devops_fingerprint 0de874316fdf8efc0589e4ad7854a880
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/installing.rst` & `xchembku-1.8.0/.dae-devops/docs/installing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Installing
 =======================================================================
 
 
 You will need python 3.9 or later. 
@@ -22,22 +22,21 @@
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
 You can now use ``pip`` to install the library and its dependencies::
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install xchembku
 
 If you require a feature that is not currently released you can also install
 from git::
 
     $ python3 -m pip install git+https://github.com/diamondlightsource/xchembku/xchembku.git
 
-The library should now be installed and the commandline interface on your path.
+The library should now be installed and the commandline should be available.
 You can check the version that has been installed by typing::
 
     $ xchembku --version
     $ xchembku --version-json
 
-.. # dae_devops_fingerprint e0afdddf0067db56b8f017a8b41f6d5e
+.. # dae_devops_fingerprint b0dd26d8e2897f65f63f81a16b0a8e29
```

### Comparing `xchembku-1.7.2/.dae-devops/docs/testing.rst` & `xchembku-1.8.0/.dae-devops/docs/testing.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
 If you want to run the tests, first get a copy of the code per the instructions in the Developing section.
 
 Then you can run all tests by::
 
-    $ pytest
-
-Or this, which is the command used by the CI runner.
-
-    $ make -f .dae-devops/Makefile validate_pytest
+    $ tox -q -e pytest
 
 To run a single test you can do::
 
     $ pytest tests/the_test_you_want.py
 
-If you want to see more output of the test while it's running you can do:
+If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
     /tmp/xchembku/tests/....
 
 The tests clear their directory when they start, but not when they finish.
 This allows peeking in there to see what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 0280ed9bb4b4f7b5eeb335a405be618b
+.. # dae_devops_fingerprint a8eba26c733cc75e40ad8560dd959093
```

### Comparing `xchembku-1.7.2/.dae-devops/project.yaml` & `xchembku-1.8.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/.devcontainer/Dockerfile` & `xchembku-1.8.0/.devcontainer/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["xchembku"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 680468bdc2c14f847ee259257ae283d9
+# dae_devops_fingerprint fd736af440d48fe8edef479361032684
```

### Comparing `xchembku-1.7.2/.devcontainer/devcontainer.json` & `xchembku-1.8.0/.devcontainer/devcontainer.json`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.3.
 // ********** For repository_name xchembku
 
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
 
-// dae_devops_fingerprint da0893109849a1c2b1e58165a9acf775
+// dae_devops_fingerprint 78ef5033030dfea0efccf90dd390ef9e
```

### Comparing `xchembku-1.7.2/.github/CONTRIBUTING.rst` & `xchembku-1.8.0/.github/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.3.
 .. # ********** For repository_name xchembku
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/xchembku/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 18a2f4bee481cbbd9336ca4eb826d663
+.. # dae_devops_fingerprint 4d117034a5fff6afaa2d35bb72fc9eac
```

### Comparing `xchembku-1.7.2/.github/actions/install_requirements/action.yml` & `xchembku-1.8.0/.github/actions/install_requirements/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
 
-# dae_devops_fingerprint 74117c18d48c5251cb9bcb8339f3a5d6
+# dae_devops_fingerprint 69141e6f06c677380aef16787df9b99c
```

### Comparing `xchembku-1.7.2/.github/dependabot.yml` & `xchembku-1.8.0/.github/dependabot.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint 35a240f5b9435f88aebb3cc5d4d8f23f
+# dae_devops_fingerprint cdf50e1871930e9030ec6b8a8bc08890
```

### Comparing `xchembku-1.7.2/.github/pages/make_switcher.py` & `xchembku-1.8.0/.github/pages/make_switcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint 6617b998da1ca2e997a558711603f920
+# dae_devops_fingerprint 6d3e04401582f9d0c731b00a656299ab
```

### Comparing `xchembku-1.7.2/.github/workflows/code.yml` & `xchembku-1.8.0/.github/workflows/code.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint bb3f1f5853bc4dae6aee2b49904ee5f0
+# dae_devops_fingerprint b95f4d599ba467ac167ad6ea2a446537
```

### Comparing `xchembku-1.7.2/.github/workflows/docs.yml` & `xchembku-1.8.0/.github/workflows/docs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint 90ddc5e712aa6cbe77be2950f77400f8
+# dae_devops_fingerprint 51b75f2f22704465096eb6a5556ef500
```

### Comparing `xchembku-1.7.2/.github/workflows/docs_clean.yml` & `xchembku-1.8.0/.github/workflows/docs_clean.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint 265968f295372c9fce9a5dcd7a5d61c2
+# dae_devops_fingerprint dc50d2f6b720ffa403975696c9411fee
```

### Comparing `xchembku-1.7.2/.github/workflows/linkcheck.yml` & `xchembku-1.8.0/.github/workflows/linkcheck.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint a6fb2885c8e8a2fd68b602f0deeccba1
+# dae_devops_fingerprint c821fd9c8d43265b997cf10e689ed233
```

### Comparing `xchembku-1.7.2/.gitignore` & `xchembku-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/.gitlab-ci.yml` & `xchembku-1.8.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
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
 
-# dae_devops_fingerprint 598c15acbaf37390bde200720e3166a3
+# dae_devops_fingerprint 3fd3717bf5ac6fc69f0e7e9e5e62f852
```

### Comparing `xchembku-1.7.2/.vscode/launch.json` & `xchembku-1.8.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/LICENSE` & `xchembku-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/PKG-INFO` & `xchembku-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.7.2
+Version: 1.8.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.7.2/README.rst` & `xchembku-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/configurations/development.yaml` & `xchembku-1.8.0/configurations/development.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     dataface_server: &XCHEMBKU_DATAFACE_SERVER http://*:27821
     dataface_client: &XCHEMBKU_DATAFACE_CLIENT http://localhost:27821
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
     database:
-        type: "xchembku_lib.xchembku_databases.normsql"
+        type: "dls_normsql.aiosqlite"
         filename: *DATABASE_FILENAME
         log_level: "WARNING"
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification:
     type: "xchembku_lib.xchembku_datafaces.aiohttp"
     type_specific_tbd:
```

### Comparing `xchembku-1.7.2/docs/conf.py` & `xchembku-1.8.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 84c433c63efba1181dae7d798737f15d
+# dae_devops_fingerprint 3e5f08df87ebb37ddf17572d476185a2
```

### Comparing `xchembku-1.7.2/docs/images/dls-favicon.ico` & `xchembku-1.8.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/docs/images/dls-logo.svg` & `xchembku-1.8.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/docs/index.rst` & `xchembku-1.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.8.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/docs/user/index.rst` & `xchembku-1.8.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/pyproject.toml` & `xchembku-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.3.
 # ********** For repository_name xchembku
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -99,8 +99,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 18b9ab431706150f1fba1a06f8fdb1c4
+# dae_devops_fingerprint c6a28d0d6afaffc18e6857fe4c60799f
```

### Comparing `xchembku-1.7.2/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.8.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.7.2
+Version: 1.8.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.7.2/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.8.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 src/xchembku_api/context_base.py
 src/xchembku_api/exceptions.py
 src/xchembku_api/crystal_plate_objects/__init__.py
 src/xchembku_api/crystal_plate_objects/constants.py
 src/xchembku_api/crystal_plate_objects/interface.py
 src/xchembku_api/databases/__init__.py
 src/xchembku_api/databases/constants.py
+src/xchembku_api/databases/database_definition.py
+src/xchembku_api/databases/table_definitions.py
 src/xchembku_api/datafaces/__init__.py
 src/xchembku_api/datafaces/aiohttp.py
 src/xchembku_api/datafaces/constants.py
 src/xchembku_api/datafaces/context.py
 src/xchembku_api/datafaces/datafaces.py
 src/xchembku_api/models/crystal_plate_filter_model.py
 src/xchembku_api/models/crystal_plate_model.py
@@ -85,20 +87,14 @@
 src/xchembku_lib/base_aiohttp.py
 src/xchembku_lib/envvar.py
 src/xchembku_lib/version.py
 src/xchembku_lib/contexts/__init__.py
 src/xchembku_lib/contexts/base.py
 src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
 src/xchembku_lib/crystal_plate_objects/swiss3.py
-src/xchembku_lib/databases/__init__.py
-src/xchembku_lib/databases/constants.py
-src/xchembku_lib/databases/database_definition.py
-src/xchembku_lib/databases/databases.py
-src/xchembku_lib/databases/normsql.py
-src/xchembku_lib/databases/table_definitions.py
 src/xchembku_lib/datafaces/__init__.py
 src/xchembku_lib/datafaces/aiohttp.py
 src/xchembku_lib/datafaces/context.py
 src/xchembku_lib/datafaces/datafaces.py
 src/xchembku_lib/datafaces/direct.py
 src/xchembku_lib/datafaces/direct_base.py
 src/xchembku_lib/datafaces/direct_crystal_plates.py
@@ -112,9 +108,11 @@
 tests/test_crystal_plate.py
 tests/test_crystal_plate_report.py
 tests/test_crystal_well_autolocation.py
 tests/test_crystal_well_droplocation1.py
 tests/test_crystal_well_droplocation2.py
 tests/test_soakdb3_crystal_well.py
 tests/test_swiss3.py
-tests/configurations/direct.yaml
-tests/configurations/service.yaml
+tests/configurations/direct_mysql.yaml
+tests/configurations/direct_sqlite.yaml
+tests/configurations/service_mysql.yaml
+tests/configurations/service_sqlite.yaml
```

### Comparing `xchembku-1.7.2/src/xchembku_api/context_base.py` & `xchembku-1.8.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/crystal_plate_objects/interface.py` & `xchembku-1.8.0/src/xchembku_api/crystal_plate_objects/interface.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.8.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/datafaces/context.py` & `xchembku-1.8.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.8.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/exceptions.py` & `xchembku-1.8.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_plate_filter_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_filter_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_plate_report_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_plate_report_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_well_filter_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_well_filter_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.8.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_cli/main.py` & `xchembku-1.8.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_cli/subcommands/base.py` & `xchembku-1.8.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_cli/subcommands/service.py` & `xchembku-1.8.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_cli/version.py` & `xchembku-1.8.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/__main__.py` & `xchembku-1.8.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/contexts/base.py` & `xchembku-1.8.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/crystal_plate_objects/swiss3.py` & `xchembku-1.8.0/src/xchembku_lib/crystal_plate_objects/swiss3.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.8.0/src/xchembku_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/context.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import logging
 from typing import Dict
 
+# Database manager.
+from dls_normsql.databases import Databases
 from dls_utilpack.callsign import callsign
 
 # Base class for generic things.
 from dls_utilpack.thing import Thing
 
-# Database manager.
-from xchembku_lib.databases.databases import Databases
+from xchembku_api.databases.database_definition import DatabaseDefinition
 
 logger = logging.getLogger(__name__)
 
 thing_type = "xchembku_lib.xchembku_datafaces.direct"
 
 
 class DirectBase(Thing):
     """ """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
         Thing.__init__(self, thing_type, specification)
 
+        # For testing, caller might want to drop the database on connection.
+        self.__should_drop_database = specification.get("should_drop_database")
+
+        self.__database_definition_object = DatabaseDefinition()
+
         self.__database = None
 
     # ----------------------------------------------------------------------------------------
     async def start(self):
         # Connect to the database to create the schemas if they don't exist already.
         await self.establish_database_connection()
 
@@ -41,16 +47,23 @@
 
         # TODO: Figure out a better way to disconnect the dataface mixins.
         await self.disconnect_soakdb3_crystal_wells_mixin()
 
     # ----------------------------------------------------------------------------------------
     async def establish_database_connection(self):
         if self.__database is None:
-            self.__database = Databases().build_object(self.specification()["database"])
-            await self.__database.connect()
+            self.__database = Databases().build_object(
+                self.specification()["database"],
+                self.__database_definition_object,
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

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,31 +187,36 @@
     ) -> str:
         """
         Wells need a droplocation if they have an autolocation.
         """
 
         fields = ["crystal_plates.*"]
 
+        self.__usable_unexported_count = (
+            "(COALESCE(decided_usable.count, 0) - COALESCE(exported.count, 0))"
+        )
+        self.__undecided_crystals_count = "COALESCE(undecided_crystals.count, 0)"
+
         if is_for_report:
             fields.append("COALESCE(collected.count, 0) AS collected_count")
             fields.append("COALESCE(chimped.count, 0) AS chimped_count")
             fields.append(
                 "COALESCE(chimped.count, 0) - COALESCE(decided.count, 0) AS undecided_count"
             )
             fields.append("COALESCE(decided.count, 0) AS decided_count")
             fields.append("COALESCE(decided_usable.count, 0) AS decided_usable_count")
             fields.append(
                 "COALESCE(decided.count, 0) - COALESCE(decided_usable.count, 0) AS decided_unusable_count"
             )
             fields.append("COALESCE(exported.count, 0) AS exported_count")
             fields.append(
-                "COALESCE(decided_usable.count, 0) - COALESCE(exported.count, 0) AS usable_unexported_count"
+                f"{self.__usable_unexported_count} AS usable_unexported_count"
             )
             fields.append(
-                "COALESCE(undecided_crystals.count, 0) AS undecided_crystals_count"
+                f"{self.__undecided_crystals_count} AS undecided_crystals_count"
             )
 
         return "\n  " + ",\n  ".join(fields)
 
     # ----------------------------------------------------------------------------------------
     def __build_joins(
         self,
@@ -297,18 +302,18 @@
                 sql += f"\n{where} formulatrix__plate__id > ?"
             subs.append(filter.from_formulatrix__plate__id)
             where = "AND"
 
         if filter.needing_intervention is not None:
             if filter.needing_intervention is True:
                 sql += "\n/* Those needing intervention. */"
-                sql += f"\n{where} (undecided_crystals_count > 0 OR usable_unexported_count > 0)"
+                sql += f"\n{where} ({self.__undecided_crystals_count} > 0 OR {self.__usable_unexported_count} > 0)"
             else:
                 sql += "\n/* Those NOT needing intervention. */"
-                sql += f"\n{where} (undecided_crystals_count = 0 AND usable_unexported_count = 0)"
+                sql += f"\n{where} ({self.__undecided_crystals_count} = 0 AND {self.__usable_unexported_count} = 0)"
 
         return sql
 
     # ----------------------------------------------------------------------------------------
     def __build_orderby(
         self,
         filter: CrystalPlateFilterModel,
```

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         where = "WHERE"
         sql = ""
 
         # Caller wants a glob of file?
         if filter.filename_pattern is not None:
             sql += (
                 "\n/* Just certain filenames. */"
-                f"\n{where} crystal_wells.filename GLOB ?"
+                f"\n{where} crystal_wells.filename REGEXP ?"
             )
             subs.append(filter.filename_pattern)
             where = "AND"
 
         # Caller wants specific barcode?
         if filter.barcode is not None:
             sql += (
```

### Comparing `xchembku-1.7.2/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.8.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/src/xchembku_lib/version.py` & `xchembku-1.8.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/tests/base.py` & `xchembku-1.8.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.7.2/tests/configurations/service.yaml` & `xchembku-1.8.0/tests/configurations/service_sqlite.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             - action: "regex_replace"
               pattern: "^[Cc][:]"
               replace: ""
             - action: "regex_replace"
               pattern: "^[Yy][:]"
               replace: "/dls/labxchem/"
         database:
-            type: "soakdb3_lib.databases.aiosqlite"
+            type: "dls_normsql.aiosqlite"
             filename: "set by code"
             backup_directory: "set by code"
             log_level: "WARNING"
 
 # The soakdb3 dataface via networked service.
 soakdb3_dataface_specification: &SOAKDB3_DATAFACE_SPECIFICATION
     type: "soakdb3_lib.datafaces.aiohttp"
@@ -65,15 +65,15 @@
 
 # -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
 xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
     soakdb3_dataface_specification: *SOAKDB3_DATAFACE_SPECIFICATION
     database:
-        type: "xchembku_lib.xchembku_databases.normsql"
+        type: "dls_normsql.aiosqlite"
         filename: "${output_directory}/xchembku_dataface.sqlite"
         log_level: "WARNING"
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
     type: "xchembku_lib.xchembku_datafaces.aiohttp"
     type_specific_tbd:
```

### Comparing `xchembku-1.7.2/tests/conftest.py` & `xchembku-1.8.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     logging.getLogger("xchembku_lib.things").setLevel("INFO")
 
     # Messages about starting and stopping services.
     logging.getLogger("xchembku_lib.base_aiohttp").setLevel("INFO")
 
     # All xchembku database sql commands.
-    # logging.getLogger("xchembku_lib.xchembku_databases.normsql").setLevel("INFO")
+    # logging.getLogger("dls_normsql.aiosqlite").setLevel("INFO")
 
     logging.getLogger("xchembku_lib.xchembku_contexts.classic").setLevel("INFO")
     logging.getLogger("xchembku_lib.xchembku_datafaces.context").setLevel("INFO")
 
     # Registering signal handler.
     logging.getLogger("dls_siggy_lib.signal").setLevel("INFO")
```

### Comparing `xchembku-1.7.2/tests/test_crystal_plate.py` & `xchembku-1.8.0/tests/test_crystal_plate.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,44 +23,78 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalPlateDirect:
+class TestCrystalPlateDirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         CrystalPlateTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalPlateService:
+class TestCrystalPlateDirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        CrystalPlateTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalPlateServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        CrystalPlateTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalPlateServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         CrystalPlateTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalPlateTester(Base):
     """
     Class to test the dataface droplocation-related endpoints.
```

### Comparing `xchembku-1.7.2/tests/test_crystal_plate_report.py` & `xchembku-1.8.0/tests/test_crystal_plate_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,44 +28,78 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalPlateReportDirect:
+class TestCrystalPlateReportDirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         CrystalPlateReportTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalPlateReportService:
+class TestCrystalPlateReportDirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        CrystalPlateReportTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalPlateReportServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        CrystalPlateReportTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalPlateReportServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         CrystalPlateReportTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalPlateReportTester(Base):
     """
     Class to test the dataface droplocation-related endpoints.
```

### Comparing `xchembku-1.7.2/tests/test_crystal_well_autolocation.py` & `xchembku-1.8.0/tests/test_crystal_well_autolocation.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,46 +17,84 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellAutolocationDirectPoll:
+class TestCrystalWellAutolocationDirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         CrystalWellAutolocationTester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellAutolocationService:
+class TestCrystalWellAutolocationDirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        CrystalWellAutolocationTester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellAutolocationServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        CrystalWellAutolocationTester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellAutolocationServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         CrystalWellAutolocationTester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellAutolocationTester(Base):
```

### Comparing `xchembku-1.7.2/tests/test_crystal_well_droplocation1.py` & `xchembku-1.8.0/tests/test_crystal_well_droplocation1.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,46 +28,84 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocation1Direct:
+class TestCrystalWellDroplocation1DirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         CrystalWellDroplocation1Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocation1Service:
+class TestCrystalWellDroplocation1DirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        CrystalWellDroplocation1Tester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellDroplocation1ServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        CrystalWellDroplocation1Tester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellDroplocation1ServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         CrystalWellDroplocation1Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellDroplocation1Tester(Base):
@@ -143,15 +181,15 @@
         models.append(await self.__inject(dataface, True, True))
         models.append(await self.__inject(dataface, True, False))
 
         # --------------------------------------------------------------------------
         # Query for list from filename glob.
         crystal_well_models = await self.__check(
             dataface,
-            CrystalWellFilterModel(filename_pattern="*A_1.jpg"),
+            CrystalWellFilterModel(filename_pattern=".*A_1.jpg"),
             3,
             "filename glob",
             filename="02A_1.jpg",
         )
 
         assert (
             crystal_well_models[1].filename == "03A_1.jpg"
```

### Comparing `xchembku-1.7.2/tests/test_crystal_well_droplocation2.py` & `xchembku-1.8.0/tests/test_crystal_well_droplocation2.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,46 +33,84 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocation2Direct:
+class TestCrystalWellDroplocation2DirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         CrystalWellDroplocation2Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
-class TestCrystalWellDroplocation2Service:
+class TestCrystalWellDroplocation2DirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        CrystalWellDroplocation2Tester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellDroplocation2ServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        CrystalWellDroplocation2Tester().main(
+            constants, configuration_file, output_directory
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestCrystalWellDroplocation2ServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         CrystalWellDroplocation2Tester().main(
             constants, configuration_file, output_directory
         )
 
 
 # ----------------------------------------------------------------------------------------
 class CrystalWellDroplocation2Tester(Base):
```

### Comparing `xchembku-1.7.2/tests/test_soakdb3_crystal_well.py` & `xchembku-1.8.0/tests/test_soakdb3_crystal_well.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,44 +30,78 @@
 # Server context creator.
 from xchembku_lib.datafaces.context import Context as XchembkuDatafaceServerContext
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-class TestSoakdb3CrystalWellDirect:
+class TestSoakdb3CrystalWellDirectSqlite:
     """
     Test dataface interface by direct call.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
-        configuration_file = "tests/configurations/direct.yaml"
+        configuration_file = "tests/configurations/direct_sqlite.yaml"
         Soakdb3CrystalWellTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class TestSoakdb3CrystalWellService:
+class TestSoakdb3CrystalWellDirectMysql:
+    """
+    Test dataface interface by direct call.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        configuration_file = "tests/configurations/direct_mysql.yaml"
+        Soakdb3CrystalWellTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestSoakdb3CrystalWellServiceSqlite:
+    """
+    Test dataface interface through network interface.
+    """
+
+    def test(
+        self,
+        constants,
+        logging_setup,
+        output_directory,
+    ):
+        """ """
+
+        configuration_file = "tests/configurations/service_sqlite.yaml"
+        Soakdb3CrystalWellTester().main(constants, configuration_file, output_directory)
+
+
+# ----------------------------------------------------------------------------------------
+class TestSoakdb3CrystalWellServiceMysql:
     """
     Test dataface interface through network interface.
     """
 
     def test(
         self,
         constants,
         logging_setup,
         output_directory,
     ):
         """ """
 
-        configuration_file = "tests/configurations/service.yaml"
+        configuration_file = "tests/configurations/service_mysql.yaml"
         Soakdb3CrystalWellTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
 class Soakdb3CrystalWellTester(Base):
     """
     Class to test the dataface droplocation-related endpoints.
```

### Comparing `xchembku-1.7.2/tests/test_swiss3.py` & `xchembku-1.8.0/tests/test_swiss3.py`

 * *Files identical despite different names*


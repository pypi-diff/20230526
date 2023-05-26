# Comparing `tmp/sceptre-4.1.0.tar.gz` & `tmp/sceptre-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sceptre-4.1.0.tar", last modified: Tue Apr 18 03:47:31 2023, max compression
+gzip compressed data, was "sceptre-4.2.0.tar", max compression
```

## Comparing `sceptre-4.1.0.tar` & `sceptre-4.2.0.tar`

### file list

```diff
@@ -1,231 +1,64 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31379 2023-04-18 03:45:00.000000 sceptre-4.1.0/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7802 2023-04-18 03:45:00.000000 sceptre-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 03:45:00.000000 sceptre-4.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-04-18 03:45:00.000000 sceptre-4.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-04-18 03:45:00.000000 sceptre-4.1.0/NOTICE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-04-18 03:47:31.221266 sceptre-4.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10458 2023-04-18 03:45:00.000000 sceptre-4.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/docs/_source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1794 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/about.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/docs/_source/apidoc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/modules.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.cli.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      510 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.diffing.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.hooks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      602 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.plan.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.resolvers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/conf.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/docs/_source/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/architecture.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3359 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/cli.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8177 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/faq.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5011 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/get_started.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/hooks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/install.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9931 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/permissions.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18998 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/resolvers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24147 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/stack_config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/stack_group_config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7056 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/template_handlers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8179 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/templates.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3406 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/terminology.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      656 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-04-18 03:45:00.000000 sceptre-4.1.0/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2023-04-18 03:45:00.000000 sceptre-4.1.0/requirements/prod.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/sceptre/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3188 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1877 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/create.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2115 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/describe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/diff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3297 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/drift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/dump.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/execute.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13964 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7611 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/launch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4357 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/new.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1366 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/policy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6488 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/prune.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3152 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/update.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3318 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23298 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/reader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/strategies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21662 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/connection_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4767 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/diffing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8016 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/diff_writer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18981 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/stack_differ.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4089 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7540 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2914 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3268 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/asg_scaling_processes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/cmd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/logging.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/plan/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39889 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/actions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/executor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13822 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/plan.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20784 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/environment_variable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/file_contents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1303 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/join.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/no_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3622 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/placeholders.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/select.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/split.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2074 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/stack_attr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5962 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/stack_output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/sub.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18051 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/sceptre/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_policies/unlock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2382 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_status_colourer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8848 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/sceptre/template_handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2937 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2305 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4800 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5040 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/http.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3267 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/s3.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2023-04-18 03:47:31.221266 sceptre-4.1.0/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3635 2023-04-18 03:45:00.000000 sceptre-4.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures/config/account/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/account/stack-group/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/config.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/construct_nodes.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/security_groups.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/subnets.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       91 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/top/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/top/level.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/hooks/custom_hook.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/resolvers/custom_resolver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/stack_policies/unlock.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/fixtures/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/chdir.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc_sud.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/sg.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.template
--rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.without_start_marker.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.yaml.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sgt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud_incorrect_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud_incorrect_handler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_t.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures-vpc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.189265 sceptre-4.1.0/tests/fixtures-vpc/config/account/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/config.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/top/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/top/level.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/hooks/custom_hook.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/resolvers/custom_resolver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/unlock.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures-vpc/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc_sud.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/sg.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.template
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.yaml.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sgt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud_incorrect_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud_incorrect_handler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_t.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    59434 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_actions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40000 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_cli_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7929 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_launch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7424 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_prune.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20760 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_config_reader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32490 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_connection_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3854 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_diffing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14190 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/test_diff_writer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/test_stack_differ.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6911 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5332 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_asg_scaling_processes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_cmd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3199 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2622 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_plan.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/tests/test_resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_environment_variable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_file_contents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2106 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_join.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_placeholders.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25717 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_resolver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_select.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1100 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_split.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2038 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_stack_attr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10626 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_stack_output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1624 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_sub.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12911 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_stack.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2245 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_stack_status_colourer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13844 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/tests/test_template_handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4064 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3226 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4661 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_http.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4453 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1456 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_template_handlers.py
+-rw-r--r--   0        0        0      635 2023-05-26 00:50:29.386326 sceptre-4.2.0/LICENSE
+-rw-r--r--   0        0        0    10458 2023-05-26 00:50:29.386326 sceptre-4.2.0/README.md
+-rw-r--r--   0        0        0     3116 2023-05-26 00:50:29.394327 sceptre-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/__init__.py
+-rw-r--r--   0        0        0     3188 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/__init__.py
+-rw-r--r--   0        0        0     1877 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/create.py
+-rw-r--r--   0        0        0     2115 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/delete.py
+-rw-r--r--   0        0        0     2482 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/describe.py
+-rw-r--r--   0        0        0     7349 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/diff.py
+-rw-r--r--   0        0        0     3297 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/drift.py
+-rw-r--r--   0        0        0     4307 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/dump.py
+-rw-r--r--   0        0        0     1441 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/execute.py
+-rw-r--r--   0        0        0    14253 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/helpers.py
+-rw-r--r--   0        0        0     7611 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/launch.py
+-rw-r--r--   0        0        0     4357 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/list.py
+-rw-r--r--   0        0        0     5678 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/new.py
+-rw-r--r--   0        0        0     1366 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/policy.py
+-rw-r--r--   0        0        0     6488 2023-05-26 00:50:29.394327 sceptre-4.2.0/sceptre/cli/prune.py
+-rw-r--r--   0        0        0     1162 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/cli/status.py
+-rw-r--r--   0        0        0     5293 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/cli/template.py
+-rw-r--r--   0        0        0     3152 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/cli/update.py
+-rw-r--r--   0        0        0      408 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/config/__init__.py
+-rw-r--r--   0        0        0     3318 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/config/graph.py
+-rw-r--r--   0        0        0    24130 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/config/reader.py
+-rw-r--r--   0        0        0     1450 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/config/strategies.py
+-rw-r--r--   0        0        0    21662 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/connection_manager.py
+-rw-r--r--   0        0        0     4781 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/context.py
+-rw-r--r--   0        0        0        0 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/diffing/__init__.py
+-rw-r--r--   0        0        0     8016 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/diffing/diff_writer.py
+-rw-r--r--   0        0        0    19257 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/diffing/stack_differ.py
+-rw-r--r--   0        0        0     4089 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/exceptions.py
+-rw-r--r--   0        0        0     7703 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/helpers.py
+-rw-r--r--   0        0        0     2914 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/hooks/__init__.py
+-rw-r--r--   0        0        0     3268 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/hooks/asg_scaling_processes.py
+-rw-r--r--   0        0        0      914 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/hooks/cmd.py
+-rw-r--r--   0        0        0      786 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/logging.py
+-rw-r--r--   0        0        0      408 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/plan/__init__.py
+-rw-r--r--   0        0        0    40000 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/plan/actions.py
+-rw-r--r--   0        0        0     1972 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/plan/executor.py
+-rw-r--r--   0        0        0    14157 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/plan/plan.py
+-rw-r--r--   0        0        0    20784 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/__init__.py
+-rw-r--r--   0        0        0      676 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/environment_variable.py
+-rw-r--r--   0        0        0      671 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/file_contents.py
+-rw-r--r--   0        0        0     1303 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/join.py
+-rw-r--r--   0        0        0      619 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/no_value.py
+-rw-r--r--   0        0        0     3622 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/placeholders.py
+-rw-r--r--   0        0        0     1855 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/select.py
+-rw-r--r--   0        0        0     1312 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/split.py
+-rw-r--r--   0        0        0     2074 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/stack_attr.py
+-rw-r--r--   0        0        0     5962 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/stack_output.py
+-rw-r--r--   0        0        0     1784 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/resolvers/sub.py
+-rw-r--r--   0        0        0    18185 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/stack.py
+-rw-r--r--   0        0        0      139 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/stack_policies/lock.json
+-rw-r--r--   0        0        0      140 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/stack_policies/unlock.json
+-rw-r--r--   0        0        0      539 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/stack_status.py
+-rw-r--r--   0        0        0     2419 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/stack_status_colourer.py
+-rw-r--r--   0        0        0     8848 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template.py
+-rw-r--r--   0        0        0     2937 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template_handlers/__init__.py
+-rw-r--r--   0        0        0     2305 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template_handlers/file.py
+-rw-r--r--   0        0        0     4800 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template_handlers/helper.py
+-rw-r--r--   0        0        0     5040 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template_handlers/http.py
+-rw-r--r--   0        0        0     3267 2023-05-26 00:50:29.398326 sceptre-4.2.0/sceptre/template_handlers/s3.py
+-rw-r--r--   0        0        0    13669 1970-01-01 00:00:00.000000 sceptre-4.2.0/setup.py
+-rw-r--r--   0        0        0    12622 1970-01-01 00:00:00.000000 sceptre-4.2.0/PKG-INFO
```

### Comparing `sceptre-4.1.0/LICENSE` & `sceptre-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/PKG-INFO` & `sceptre-4.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: sceptre
-Version: 4.1.0
-Summary: Cloud Provisioning Tool
-Home-page: https://github.com/Sceptre/sceptre
-Author: Cloudreach
-Author-email: sceptre@cloudreach.com
-License: Apache2
-Keywords: sceptre
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: troposphere
-License-File: LICENSE
-License-File: NOTICE
-
 # Sceptre
 
 [![CircleCI](https://img.shields.io/circleci/build/github/Sceptre/sceptre?logo=circleci)](https://app.circleci.com/pipelines/github/Sceptre)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/sceptreorg/sceptre?logo=docker&sort=semver)](https://hub.docker.com/r/sceptreorg/sceptre)
 [![PyPI](https://img.shields.io/pypi/v/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
 [![PyPI - Status](https://img.shields.io/pypi/status/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
```

### Comparing `sceptre-4.1.0/README.md` & `sceptre-4.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,58 @@
+Metadata-Version: 2.1
+Name: sceptre
+Version: 4.2.0
+Summary: An AWS Cloud Provisioning Tool
+Home-page: https://github.com/Sceptre/sceptre
+License: Apache-2.0
+Keywords: aws,cloud,devops,infrastructure,tools,cli
+Author: Sceptre
+Author-email: sceptreorg@gmail.com
+Requires-Python: >=3.7,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: docs
+Provides-Extra: troposphere
+Requires-Dist: boto3 (>=1.3.0,<2)
+Requires-Dist: cfn-flip (>=1.2.3,<2.0.0)
+Requires-Dist: click (>=7.0,<9.0)
+Requires-Dist: colorama (>=0.2.5,<0.4.4)
+Requires-Dist: deepdiff (>=5.5,<6.0)
+Requires-Dist: deprecation (>=2.0,<3.0)
+Requires-Dist: docutils (<0.17) ; extra == "docs"
+Requires-Dist: jinja2 (>=3.0,<4.0)
+Requires-Dist: jsonschema (>=3.2,<3.3)
+Requires-Dist: networkx (>=2.6,<2.7)
+Requires-Dist: packaging (>=16.8,<22.0)
+Requires-Dist: pyyaml (>=5.1,<6.0)
+Requires-Dist: sceptre-cmd-resolver (>=2.0,<3.0)
+Requires-Dist: sceptre-file-resolver (>=1.0,<2.0)
+Requires-Dist: sphinx (>=1.6.5,<=5.1.1) ; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (==1.19.2) ; extra == "docs"
+Requires-Dist: sphinx-click (>=2.0.1,<4.0.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (==0.5.2) ; extra == "docs"
+Requires-Dist: troposphere (>=4,<5) ; extra == "troposphere"
+Project-URL: Documentation, https://docs.sceptre-project.org
+Project-URL: Repository, https://github.com/Sceptre/sceptre
+Description-Content-Type: text/markdown
+
 # Sceptre
 
 [![CircleCI](https://img.shields.io/circleci/build/github/Sceptre/sceptre?logo=circleci)](https://app.circleci.com/pipelines/github/Sceptre)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/sceptreorg/sceptre?logo=docker&sort=semver)](https://hub.docker.com/r/sceptreorg/sceptre)
 [![PyPI](https://img.shields.io/pypi/v/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
 [![PyPI - Status](https://img.shields.io/pypi/status/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sceptre?logo=pypi)](https://pypi.org/project/sceptre/)
@@ -281,7 +332,8 @@
 ## Sponsors
 
 [![Sage Bionetworks](sponsors/sage_bionetworks_logo.png "Sage Bionetworks")](https://sagebionetworks.org)
 
 [![GoDaddy](sponsors/godaddy_logo.png "GoDaddy")](https://www.godaddy.com)
 
 [![Cloudreach](sponsors/cloudreach_logo.png "Cloudreach")](https://www.cloudreach.com)
+
```

### Comparing `sceptre-4.1.0/sceptre/cli/__init__.py` & `sceptre-4.2.0/sceptre/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/create.py` & `sceptre-4.2.0/sceptre/cli/create.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/delete.py` & `sceptre-4.2.0/sceptre/cli/delete.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/describe.py` & `sceptre-4.2.0/sceptre/cli/describe.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/diff.py` & `sceptre-4.2.0/sceptre/cli/diff.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/drift.py` & `sceptre-4.2.0/sceptre/cli/drift.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/dump.py` & `sceptre-4.2.0/sceptre/cli/status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,37 @@
-import logging
 import click
 
 from sceptre.context import SceptreContext
 from sceptre.cli.helpers import catch_exceptions, write
 from sceptre.plan.plan import SceptrePlan
 
-logger = logging.getLogger(__name__)
 
-
-@click.group(name="dump")
-def dump_group():
-    """
-    Commands for dumping attributes of stacks.
-    """
-    pass
-
-
-@dump_group.command(name="config")
+@click.command(name="status", short_help="Print status of stack or stack_group.")
 @click.argument("path")
 @click.pass_context
 @catch_exceptions
-def dump_config(ctx, path):
+def status_command(ctx, path):
     """
-    Dump the rendered (post-Jinja) Stack Configs.
+    Prints the stack status or the status of the stacks within a
+    stack_group for a given config PATH.
     \f
 
-    :param path: Path to execute the command on or path to stack group
+    :param path: Path to execute the command on.
+    :type path: str
     """
     context = SceptreContext(
         command_path=path,
         command_params=ctx.params,
         project_path=ctx.obj.get("project_path"),
         user_variables=ctx.obj.get("user_variables"),
-        output_format=ctx.obj.get("output_format"),
         options=ctx.obj.get("options"),
+        no_colour=ctx.obj.get("no_colour"),
+        output_format=ctx.obj.get("output_format"),
         ignore_dependencies=ctx.obj.get("ignore_dependencies"),
     )
-    plan = SceptrePlan(context)
-    responses = plan.dump_config()
-
-    output = []
-    for stack, config in responses.items():
-        if config is None:
-            logger.warning(f"{stack.external_name} does not exist")
-        else:
-            output.append({stack.external_name: config})
 
-    output_format = "json" if context.output_format == "json" else "yaml"
-
-    if len(output) == 1:
-        write(output[0][stack.external_name], output_format)
-    else:
-        for config in output:
-            write(config, output_format)
+    plan = SceptrePlan(context)
+    responses = plan.get_status()
+    message = "\n".join(
+        "{}: {}".format(stack.name, status) for stack, status in responses.items()
+    )
+    write(message, no_colour=context.no_colour)
```

### Comparing `sceptre-4.1.0/sceptre/cli/execute.py` & `sceptre-4.2.0/sceptre/cli/execute.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/helpers.py` & `sceptre-4.2.0/sceptre/cli/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import logging
 import sys
+
 from itertools import cycle
 from functools import partial, wraps
 
+from typing import Any, Optional
+from pathlib import Path
+
 import json
 import click
 import six
 import yaml
 
 from boto3.exceptions import Boto3Error
 from botocore.exceptions import BotoCoreError, ClientError
 from jinja2.exceptions import TemplateError
 
+from sceptre.helpers import logging_level
 from sceptre.exceptions import SceptreException
 from sceptre.stack_status import StackStatus
 from sceptre.stack_status_colourer import StackStatusColourer
 
+logger = logging.getLogger(__name__)
+
 
 def catch_exceptions(func):
     """
     Catches and simplifies expected errors thrown by sceptre.
 
     catch_exceptions should be used as a decorator.
 
     :param func: The function which may throw exceptions which should be
         simplified.
     :returns: The decorated function.
     """
 
-    def logging_level():
-        logger = logging.getLogger(__name__)
-        return logger.getEffectiveLevel()
-
     @wraps(func)
     def decorated(*args, **kwargs):
         """
         Invokes ``func``, catches expected errors, prints the error message and
         exits sceptre with a non-zero exit code. In debug mode, the original
         exception is re-raised to assist debugging.
         """
@@ -62,35 +65,48 @@
         if change_set:
             msg = msg + "change set '{0}' for '{1}'".format(change_set, command_path)
         else:
             msg = msg + "'{0}'".format(command_path)
         click.confirm(msg, abort=True)
 
 
-def write(var, output_format="json", no_colour=True):
+def write(
+    var: Any,
+    output_format: str = "json",
+    no_colour: bool = True,
+    file_path: Optional[Path] = None,
+) -> None:
     """
     Writes ``var`` to stdout. If output_format is set to "json" or "yaml",
     write ``var`` as a JSON or YAML string.
 
     :param var: The object to print
-    :type var: object
     :param output_format: The format to print the output as. Allowed values: \
     "text", "json", "yaml"
-    :type output_format: str
     :param no_colour: Whether to colour stack statuses
-    :type no_colour: bool
+    :param file_path: Optional path to a file to save the output
     """
     output = var
 
     if output_format == "json":
         output = _generate_json(var)
     if output_format == "yaml":
         output = _generate_yaml(var)
     if output_format == "text":
         output = _generate_text(var)
+
+    if file_path:
+        dir_path = file_path.parent
+        dir_path.mkdir(parents=True, exist_ok=True)
+
+        with open(file_path, "w") as f:
+            f.write(output)
+
+        return
+
     if not no_colour:
         stack_status_colourer = StackStatusColourer()
         output = stack_status_colourer.colour(str(output))
 
     click.echo(output)
```

### Comparing `sceptre-4.1.0/sceptre/cli/launch.py` & `sceptre-4.2.0/sceptre/cli/launch.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/list.py` & `sceptre-4.2.0/sceptre/cli/list.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/new.py` & `sceptre-4.2.0/sceptre/cli/new.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/policy.py` & `sceptre-4.2.0/sceptre/cli/policy.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/prune.py` & `sceptre-4.2.0/sceptre/cli/prune.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/cli/template.py` & `sceptre-4.2.0/sceptre/cli/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import webbrowser
-
 import click
 
+from deprecation import deprecated
+
+from sceptre import __version__
 from sceptre.cli.helpers import catch_exceptions, write
 from sceptre.context import SceptreContext
 from sceptre.helpers import null_context
 from sceptre.plan.plan import SceptrePlan
 from sceptre.resolvers.placeholders import use_resolver_placeholders_on_error
 
 logger = logging.getLogger(__name__)
@@ -61,14 +63,15 @@
     "--no-placeholders",
     is_flag=True,
     help="If True, no placeholder values will be supplied for resolvers that cannot be resolved.",
 )
 @click.argument("path")
 @click.pass_context
 @catch_exceptions
+@deprecated("4.2.0", "5.0.0", __version__, "Use dump template instead.")
 def generate_command(ctx, no_placeholders, path):
     """
     Prints the template used for stack in PATH.
     \f
 
     :param path: Path to execute the command on.
     :type path: str
```

### Comparing `sceptre-4.1.0/sceptre/cli/update.py` & `sceptre-4.2.0/sceptre/cli/update.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/config/graph.py` & `sceptre-4.2.0/sceptre/config/graph.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/config/reader.py` & `sceptre-4.2.0/sceptre/config/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import collections
 import copy
 import datetime
 import fnmatch
 import logging
 import sys
 import yaml
+import json
+import tempfile
 
 from os import environ, path, walk
 from typing import Set, Tuple
 from pathlib import Path
 from jinja2 import Environment
 from jinja2 import StrictUndefined
 from jinja2 import FileSystemLoader
@@ -28,15 +30,15 @@
 from sceptre import __version__
 from sceptre.exceptions import SceptreException
 from sceptre.exceptions import DependencyDoesNotExistError
 from sceptre.exceptions import InvalidConfigFileError
 from sceptre.exceptions import InvalidSceptreDirectoryError
 from sceptre.exceptions import VersionIncompatibleError
 from sceptre.exceptions import ConfigFileNotFoundError
-from sceptre.helpers import sceptreise_path
+from sceptre.helpers import sceptreise_path, logging_level
 from sceptre.stack import Stack
 from sceptre.config import strategies
 
 ConfigAttributes = collections.namedtuple("Attributes", "required optional")
 
 CONFIG_MERGE_STRATEGIES = {
     "dependencies": strategies.list_join,
@@ -98,22 +100,14 @@
         "sceptre_user_data",
         "stack_name",
         "stack_tags",
         "stack_timeout",
     },
 )
 
-INTERNAL_CONFIG_ATTRIBUTES = ConfigAttributes(
-    {
-        "project_path",
-        "stack_group_path",
-    },
-    {},
-)
-
 REQUIRED_KEYS = STACK_GROUP_CONFIG_ATTRIBUTES.required.union(
     STACK_CONFIG_ATTRIBUTES.required
 )
 
 
 class ConfigReader(object):
     """
@@ -247,15 +241,15 @@
             abs_path = todo.pop()
             rel_path = path.relpath(abs_path, start=self.context.full_config_path())
             directory, filename = path.split(rel_path)
 
             if directory in stack_group_configs:
                 stack_group_config = stack_group_configs[directory]
             else:
-                stack_group_config = stack_group_configs[directory] = self.read(
+                stack_group_config = stack_group_configs[directory] = self._read(
                     path.join(directory, self.context.config_file)
                 )
 
             stack = self._construct_stack(rel_path, stack_group_config)
             for dep in stack.dependencies:
                 full_dep = str(Path(self.context.full_config_path(), dep))
                 if not path.exists(full_dep):
@@ -319,15 +313,15 @@
                 # dependency ends up in the list multiple times.
                 stack.dependencies = list(set(stack.dependencies))
             else:
                 stack.dependencies = []
             stacks.add(stack)
         return stacks
 
-    def read(self, rel_path, base_config=None):
+    def _read(self, rel_path, base_config=None):
         """
         Reads in configuration from one or more YAML files
         within the Sceptre project folder.
 
         :param rel_path: Relative path to config to read.
         :type rel_path: str
         :param base_config: Base config to provide defaults.
@@ -409,14 +403,29 @@
             if value:
                 child_config[config_key] = value
 
         config.update(child_config)
 
         return config
 
+    def _write_debug_file(self, content: str, prefix: str) -> str:
+        """
+        Write some content to a temp file for debug purposes.
+
+        :param content: the file content to write.
+        :returns: the full path to the temp file.
+        """
+        with tempfile.NamedTemporaryFile(
+            mode="w", delete=False, prefix=prefix
+        ) as temp_file:
+            temp_file.write(content)
+            temp_file.flush()
+
+        return temp_file.name
+
     def _render(self, directory_path, basename, stack_group_config):
         """
         Reads a configuration file, loads the config file as a template
         and returns config loaded from the file.
 
         :param directory_path: Relative directory path to config to read.
         :type directory_path: str
@@ -425,57 +434,72 @@
         :param stack_group_config: The loaded config file for the StackGroup
         :type stack_group_config: dict
         :returns: rendered template of config file.
         :rtype: dict
         """
         config = {}
         abs_directory_path = path.join(self.full_config_path, directory_path)
-        if path.isfile(path.join(abs_directory_path, basename)):
-            default_j2_environment_config = {
-                "autoescape": select_autoescape(
-                    disabled_extensions=("yaml",),
-                    default=True,
-                ),
-                "loader": FileSystemLoader(abs_directory_path),
-                "undefined": StrictUndefined,
-            }
-            j2_environment_config = strategies.dict_merge(
-                default_j2_environment_config,
-                stack_group_config.get("j2_environment", {}),
+
+        if not path.isfile(path.join(abs_directory_path, basename)):
+            return
+
+        default_j2_environment_config = {
+            "autoescape": select_autoescape(
+                disabled_extensions=("yaml",),
+                default=True,
+            ),
+            "loader": FileSystemLoader(abs_directory_path),
+            "undefined": StrictUndefined,
+        }
+        j2_environment_config = strategies.dict_merge(
+            default_j2_environment_config,
+            stack_group_config.get("j2_environment", {}),
+        )
+        j2_environment = Environment(**j2_environment_config)
+
+        try:
+            template = j2_environment.get_template(basename)
+        except Exception as err:
+            raise SceptreException(
+                f"{Path(directory_path, basename).as_posix()} - {err}"
+            ) from err
+
+        self.templating_vars.update(stack_group_config)
+
+        try:
+            rendered_template = template.render(
+                self.templating_vars,
+                command_path=self.context.command_path.split(path.sep),
+                environment_variable=environ,
             )
-            j2_environment = Environment(**j2_environment_config)
+        except Exception as err:
+            message = f"{Path(directory_path, basename).as_posix()} - {err}"
 
-            try:
-                template = j2_environment.get_template(basename)
-            except Exception as err:
-                raise SceptreException(
-                    f"{Path(directory_path, basename).as_posix()} - {err}"
-                ) from err
-
-            self.templating_vars.update(stack_group_config)
-
-            try:
-                rendered_template = template.render(
-                    self.templating_vars,
-                    command_path=self.context.command_path.split(path.sep),
-                    environment_variable=environ,
+            if logging_level() == logging.DEBUG:
+                debug_file_path = self._write_debug_file(
+                    json.dumps(self.templating_vars), prefix="vars_"
                 )
-            except Exception as err:
-                raise SceptreException(
-                    f"{Path(directory_path, basename).as_posix()} - {err}"
-                ) from err
-
-            try:
-                config = yaml.safe_load(rendered_template)
-            except Exception as err:
-                raise ValueError(
-                    "Error parsing {}:\n{}".format(abs_directory_path, err)
+                message += f"\nTemplating vars saved to: {debug_file_path}"
+
+            raise SceptreException(message) from err
+
+        try:
+            config = yaml.safe_load(rendered_template)
+        except Exception as err:
+            message = f"Error parsing {abs_directory_path}{basename}:\n{err}"
+
+            if logging_level() == logging.DEBUG:
+                debug_file_path = self._write_debug_file(
+                    rendered_template, prefix="rendered_"
                 )
+                message += f"\nRendered template saved to: {debug_file_path}"
 
-            return config
+            raise ValueError(message)
+
+        return config
 
     @staticmethod
     def _check_valid_project_path(config_path):
         """
         Raises an InvalidSceptreDirectoryError if ``path`` is not a directory.
 
         :param path: A config directory path.
@@ -555,15 +579,15 @@
 
         directory, filename = path.split(rel_path)
         if filename == self.context.config_file:
             pass
 
         self.templating_vars["stack_group_config"] = stack_group_config
         parsed_stack_group_config = self._parsed_stack_group_config(stack_group_config)
-        config = self.read(rel_path, stack_group_config)
+        config = self._read(rel_path, stack_group_config)
         stack_name = path.splitext(rel_path)[0]
 
         # Check for missing mandatory attributes
         for required_key in REQUIRED_KEYS:
             if required_key not in config:
                 raise InvalidConfigFileError(
                     "Required attribute '{0}' not found in configuration of '{1}'.".format(
@@ -605,14 +629,15 @@
             notifications=config.get("notifications"),
             on_failure=config.get("on_failure"),
             disable_rollback=disable_rollback,
             stack_timeout=config.get("stack_timeout", 0),
             ignore=config.get("ignore", False),
             obsolete=config.get("obsolete", False),
             stack_group_config=parsed_stack_group_config,
+            config=config,
         )
 
         del self.templating_vars["stack_group_config"]
         return stack
 
     def _parsed_stack_group_config(self, stack_group_config):
         """
```

### Comparing `sceptre-4.1.0/sceptre/config/strategies.py` & `sceptre-4.2.0/sceptre/config/strategies.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/connection_manager.py` & `sceptre-4.2.0/sceptre/connection_manager.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/context.py` & `sceptre-4.2.0/sceptre/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         output_format=None,
         no_colour=False,
         ignore_dependencies=False,
         full_scan=False,
     ):
         # project_path: absolute path to the base sceptre project folder
         # e.g. absolute_path/to/sceptre_directory
-        self.project_path = normalise_path(project_path)
+        self.project_path = path.abspath(normalise_path(project_path))
 
         # config_path: holds the project stack_groups
         # e.g {project_path}/config
         self.config_path = "config"  # user definable later in v2
 
         # command_path path to either stack group or stack
         # e.g. {project_path/config_path}/command_path
```

### Comparing `sceptre-4.1.0/sceptre/diffing/diff_writer.py` & `sceptre-4.2.0/sceptre/diffing/diff_writer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/diffing/stack_differ.py` & `sceptre-4.2.0/sceptre/diffing/stack_differ.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,20 @@
         to match the what CloudFormation does on its end.
 
         :param stack: The stack to extract the parameters from
         :return: A dictionary of stack parameters to be compared.
         """
         formatted_parameters = {}
         for key, value in stack.parameters.items():
+            # When boto3 receives "None" for a cloudformation parameter, it treats it as if the
+            # value is not passed at all. To be consistent in our diffing, we need to skip Nones
+            # altogether.
+            if value is None:
+                continue
+
             if isinstance(value, list):
                 value = ",".join(item.rstrip("\n") for item in value)
             formatted_parameters[key] = value.rstrip("\n")
 
         return formatted_parameters
 
     def _create_deployed_stack_config(
@@ -215,14 +221,15 @@
 
             # If the parameter is not passed by Sceptre and the value on the deployed parameter is
             # the default value, we'll actually remove it from the deployed parameters list so it
             # doesn't show up as a false positive.
             self._remove_deployed_default_parameters_that_arent_passed(
                 deployed_template_summary, generated_config, deployed_config
             )
+
         if not self.show_no_echo:
             # We don't actually want to show parameters Sceptre is passing that the local template
             # marks as NoEcho parameters (unless show_no_echo is set to true). Therefore those
             # parameter values will be masked.
             self._mask_no_echo_parameters(generated_template_summary, generated_config)
 
     def _remove_terminating_linebreaks_from_deployed_parameters(
```

### Comparing `sceptre-4.1.0/sceptre/exceptions.py` & `sceptre-4.2.0/sceptre/exceptions.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/helpers.py` & `sceptre-4.2.0/sceptre/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,28 @@
 from contextlib import contextmanager
 from datetime import datetime
 from os import sep
 from typing import Optional, Any, List, Tuple, Union
 
 import dateutil.parser
 import deprecation
+import logging
 
 from sceptre.exceptions import PathConversionError
 from sceptre import __version__
 
 
+def logging_level():
+    """
+    Return the logging level.
+    """
+    logger = logging.getLogger(__name__)
+    return logger.getEffectiveLevel()
+
+
 def get_external_stack_name(project_code, stack_name):
     """
     Returns the name given to a stack in CloudFormation.
     :param project_code: The project code, as defined in config.yaml.
     :type project_code: str
     :param stack_name: The name of the stack.
     :type stack_name: str
```

### Comparing `sceptre-4.1.0/sceptre/hooks/__init__.py` & `sceptre-4.2.0/sceptre/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/hooks/asg_scaling_processes.py` & `sceptre-4.2.0/sceptre/hooks/asg_scaling_processes.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/hooks/cmd.py` & `sceptre-4.2.0/sceptre/hooks/cmd.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/logging.py` & `sceptre-4.2.0/sceptre/logging.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/plan/actions.py` & `sceptre-4.2.0/sceptre/plan/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,35 +8,38 @@
 """
 
 import json
 import logging
 import time
 import typing
 import urllib
-from datetime import datetime, timedelta
-from os import path
-from typing import Dict, Optional, Tuple, Union
-
 import botocore
+
+from datetime import datetime, timedelta
 from dateutil.tz import tzutc
+from os import path
+from deprecation import deprecated
 
-from sceptre.config.reader import ConfigReader
+from sceptre import __version__
 from sceptre.connection_manager import ConnectionManager
+
 from sceptre.exceptions import (
     CannotUpdateFailedStackError,
     ProtectedStackError,
     StackDoesNotExistError,
     UnknownStackChangeSetStatusError,
     UnknownStackStatusError,
 )
-from sceptre.helpers import extract_datetime_from_aws_response_headers, normalise_path
+from sceptre.helpers import extract_datetime_from_aws_response_headers
 from sceptre.hooks import add_stack_hooks
 from sceptre.stack import Stack
 from sceptre.stack_status import StackChangeSetStatus, StackStatus
 
+from typing import Dict, Optional, Tuple, Union
+
 if typing.TYPE_CHECKING:
     from sceptre.diffing.stack_differ import StackDiff, StackDiffer
 
 
 class StackActions:
     """
     StackActions stores the operations a Stack can take, such as creating or
@@ -620,20 +623,20 @@
             new_summaries.append(
                 f"https://{region}.console.aws.amazon.com/cloudformation/home?"
                 f"region={region}#/stacks/changesets/changes?{encoded}"
             )
 
         return new_summaries
 
-    @add_stack_hooks
+    @deprecated("4.2.0", "5.0.0", __version__, "Use dump template instead.")
     def generate(self):
         """
         Returns the Template for the Stack
         """
-        return self.stack.template.body
+        return self.dump_template()
 
     @add_stack_hooks
     def validate(self):
         """
         Validates the Stack's CloudFormation Template.
 
         Raises an error if the Template is invalid.
@@ -1142,13 +1145,19 @@
             is_drifted = drift["StackResourceDriftStatus"] != "IN_SYNC"
             if include_all_drift_statuses or is_drifted:
                 result["StackResourceDrifts"].append(drift)
 
         return result
 
     @add_stack_hooks
-    def dump_config(self, config_reader: ConfigReader):
+    def dump_config(self):
         """
         Dump the config for a stack.
         """
-        stack_path = normalise_path(self.stack.name + ".yaml")
-        return config_reader.read(stack_path)
+        return self.stack.config
+
+    @add_stack_hooks
+    def dump_template(self):
+        """
+        Returns the Template for the Stack
+        """
+        return self.stack.template.body
```

### Comparing `sceptre-4.1.0/sceptre/plan/executor.py` & `sceptre-4.2.0/sceptre/plan/executor.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/plan/plan.py` & `sceptre-4.2.0/sceptre/plan/plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 sceptre.plan.plan
 
 This module implements a SceptrePlan, which is responsible for holding all
 nessessary information for a command to execute.
 """
 import functools
 import itertools
+
 from os import path, walk
 from typing import Dict, List, Set, Callable, Iterable, Optional
+from deprecation import deprecated
 
 from sceptre.config.graph import StackGraph
 from sceptre.config.reader import ConfigReader
 from sceptre.context import SceptreContext
 from sceptre.diffing.stack_differ import StackDiff
 from sceptre.exceptions import ConfigFileNotFoundError
 from sceptre.helpers import sceptreise_path
 from sceptre.plan.executor import SceptrePlanExecutor
 from sceptre.stack import Stack
+from sceptre import __version__
 
 
 def require_resolved(func) -> Callable:
     @functools.wraps(func)
     def wrapped(self: "SceptrePlan", *args, **kwargs):
         if self.launch_order is None:
             raise RuntimeError(f"You cannot call {func.__name__}() before resolve().")
@@ -373,14 +376,15 @@
         :returns: A dictionary of Stacks and their estimated costs.
         :rtype: dict
         :raises: botocore.exceptions.ClientError
         """
         self.resolve(command=self.estimate_cost.__name__)
         return self._execute(*args)
 
+    @deprecated("4.2.0", "5.0.0", __version__, "Use dump template instead.")
     def generate(self, *args):
         """
         Returns a generated Template for a given Stack
 
         :returns: A dictionary of Stacks and their template body.
         :rtype: dict
         """
@@ -435,8 +439,15 @@
         return self._execute(*args)
 
     def dump_config(self, *args):
         """
         Dump the config for a stack.
         """
         self.resolve(command=self.dump_config.__name__)
-        return self._execute(self.config_reader, *args)
+        return self._execute(*args)
+
+    def dump_template(self, *args):
+        """
+        Returns a generated Template for a given Stack
+        """
+        self.resolve(command=self.dump_template.__name__)
+        return self._execute(*args)
```

### Comparing `sceptre-4.1.0/sceptre/resolvers/__init__.py` & `sceptre-4.2.0/sceptre/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/environment_variable.py` & `sceptre-4.2.0/sceptre/resolvers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/file_contents.py` & `sceptre-4.2.0/sceptre/resolvers/file_contents.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/join.py` & `sceptre-4.2.0/sceptre/resolvers/join.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/no_value.py` & `sceptre-4.2.0/sceptre/resolvers/no_value.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/placeholders.py` & `sceptre-4.2.0/sceptre/resolvers/placeholders.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/select.py` & `sceptre-4.2.0/sceptre/resolvers/select.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/split.py` & `sceptre-4.2.0/sceptre/resolvers/split.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/stack_attr.py` & `sceptre-4.2.0/sceptre/resolvers/stack_attr.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/stack_output.py` & `sceptre-4.2.0/sceptre/resolvers/stack_output.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/resolvers/sub.py` & `sceptre-4.2.0/sceptre/resolvers/sub.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/stack.py` & `sceptre-4.2.0/sceptre/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 sceptre.stack
 
 This module implements a Stack class, which stores a Stack's data.
 
 """
 
 import logging
-from typing import List, Any, Optional
 
-import deprecation
+from typing import List, Any, Optional
+from deprecation import deprecated
 
 from sceptre import __version__
 from sceptre.connection_manager import ConnectionManager
 from sceptre.exceptions import InvalidConfigFileError
 from sceptre.helpers import (
     get_external_stack_name,
     sceptreise_path,
@@ -119,14 +119,16 @@
             also be deleted if the prune command is invoked or the --prune option is used with the
             launch command.
 
     :param sceptre_role_session_duration: The session duration when Scetre assumes a role.\
            If not supplied, Sceptre uses default value (3600 seconds)
 
     :param stack_group_config: The StackGroup config for the Stack
+
+    :param config: The complete config for the stack. Used by dump config.
     """
 
     parameters = ResolvableContainerProperty("parameters")
     sceptre_user_data = ResolvableContainerProperty(
         "sceptre_user_data", PlaceholderType.alphanum
     )
     notifications = ResolvableContainerProperty("notifications")
@@ -189,15 +191,16 @@
         disable_rollback=False,
         profile: str = None,
         stack_timeout: int = 0,
         sceptre_role_session_duration: Optional[int] = None,
         iam_role_session_duration: Optional[int] = None,
         ignore=False,
         obsolete=False,
-        stack_group_config: dict = {},
+        stack_group_config: dict = None,
+        config: dict = None,
     ):
         self.logger = logging.getLogger(__name__)
 
         self.name = sceptreise_path(name)
         self.project_code = project_code
         self.region = region
         self.required_version = required_version
@@ -207,14 +210,15 @@
         self.dependencies = dependencies or []
         self.protected = protected
         self.on_failure = on_failure
         self.disable_rollback = self._ensure_boolean(
             "disable_rollback", disable_rollback
         )
         self.stack_group_config = stack_group_config or {}
+        self.config = config or {}
         self.stack_timeout = stack_timeout
         self.profile = profile
         self.template_key_prefix = template_key_prefix
         self._set_field_with_deprecated_alias(
             "sceptre_role_session_duration",
             sceptre_role_session_duration,
             "iam_role_session_duration",
@@ -379,25 +383,25 @@
                 stack_group_config=self.stack_group_config,
                 s3_details=self.s3_details,
                 connection_manager=self.connection_manager,
             )
         return self._template
 
     @property
-    @deprecation.deprecated(
+    @deprecated(
         "4.0.0", "5.0.0", __version__, "Use the template Stack Config key instead."
     )
     def template_path(self) -> str:
         """The path argument from the template_handler config. This field is deprecated as of v4.0.0
         and will be removed in v5.0.0.
         """
         return self.template_handler_config["path"]
 
     @template_path.setter
-    @deprecation.deprecated(
+    @deprecated(
         "4.0.0", "5.0.0", __version__, "Use the template Stack Config key instead."
     )
     def template_path(self, value: str):
         self.template_handler_config = {"type": "file", "path": value}
 
     def _set_field_with_deprecated_alias(
         self,
```

### Comparing `sceptre-4.1.0/sceptre/stack_status.py` & `sceptre-4.2.0/sceptre/stack_status.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/stack_status_colourer.py` & `sceptre-4.2.0/sceptre/stack_status_colourer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,27 @@
     """
     StackStatusColourer adds colours to stack statuses.
     These are documented here:
     https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-describing-stacks.html
     """
 
     STACK_STATUS_CODES = {
-        "PENDING": Fore.CYAN,
         "CREATE_COMPLETE": Fore.GREEN,
         "CREATE_FAILED": Fore.RED,
         "CREATE_IN_PROGRESS": Fore.YELLOW,
         "DELETE_COMPLETE": Fore.GREEN,
         "DELETE_FAILED": Fore.RED,
         "DELETE_IN_PROGRESS": Fore.YELLOW,
+        "DELETE_SKIPPED": Fore.CYAN,
         "IMPORT_COMPLETE": Fore.GREEN,
         "IMPORT_IN_PROGRESS": Fore.YELLOW,
         "IMPORT_ROLLBACK_COMPLETE": Fore.GREEN,
         "IMPORT_ROLLBACK_FAILED": Fore.RED,
         "IMPORT_ROLLBACK_IN_PROGRESS": Fore.YELLOW,
+        "PENDING": Fore.CYAN,
         "REVIEW_IN_PROGRESS": Fore.YELLOW,
         "ROLLBACK_COMPLETE": Fore.RED,
         "ROLLBACK_FAILED": Fore.RED,
         "ROLLBACK_IN_PROGRESS": Fore.YELLOW,
         "UPDATE_COMPLETE": Fore.GREEN,
         "UPDATE_COMPLETE_CLEANUP_IN_PROGRESS": Fore.YELLOW,
         "UPDATE_FAILED": Fore.RED,
```

### Comparing `sceptre-4.1.0/sceptre/template.py` & `sceptre-4.2.0/sceptre/template.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/template_handlers/__init__.py` & `sceptre-4.2.0/sceptre/template_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/template_handlers/file.py` & `sceptre-4.2.0/sceptre/template_handlers/file.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/template_handlers/helper.py` & `sceptre-4.2.0/sceptre/template_handlers/helper.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/template_handlers/http.py` & `sceptre-4.2.0/sceptre/template_handlers/http.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.1.0/sceptre/template_handlers/s3.py` & `sceptre-4.2.0/sceptre/template_handlers/s3.py`

 * *Files identical despite different names*


# Comparing `tmp/ReFrame-HPC-4.2.0.tar.gz` & `tmp/ReFrame-HPC-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.2.0.tar", last modified: Fri Apr 21 20:18:13 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.2.1.tar", last modified: Fri May 26 19:57:16 2023, max compression
```

## Comparing `ReFrame-HPC-4.2.0.tar` & `ReFrame-HPC-4.2.1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.558676 ReFrame-HPC-4.2.0/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.558676 ReFrame-HPC-4.2.0/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    35671 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    94467 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    55074 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 19:57:16.000000 ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.368482 ReFrame-HPC-4.2.1/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.376482 ReFrame-HPC-4.2.1/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.376482 ReFrame-HPC-4.2.1/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/launchers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94467 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.380482 ReFrame-HPC-4.2.1/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55074 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.384482 ReFrame-HPC-4.2.1/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-26 19:57:05.000000 ReFrame-HPC-4.2.1/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 19:57:16.388482 ReFrame-HPC-4.2.1/setup.cfg
```

### Comparing `ReFrame-HPC-4.2.0/LICENSE` & `ReFrame-HPC-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/PKG-INFO` & `ReFrame-HPC-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.0
+Version: 4.2.1
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.2.0/README.md` & `ReFrame-HPC-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/README_minimal.md` & `ReFrame-HPC-4.2.1/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.2.0
+Version: 4.2.1
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.2.1/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/bin/reframe` & `ReFrame-HPC-4.2.1/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/__init__.py` & `ReFrame-HPC-4.2.1/reframe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.2.0'
+VERSION = '4.2.1'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.2.0/reframe/core/backends.py` & `ReFrame-HPC-4.2.1/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/buildsystems.py` & `ReFrame-HPC-4.2.1/reframe/core/buildsystems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/builtins.py` & `ReFrame-HPC-4.2.1/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/config.py` & `ReFrame-HPC-4.2.1/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/containers.py` & `ReFrame-HPC-4.2.1/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/decorators.py` & `ReFrame-HPC-4.2.1/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/deferrable.py` & `ReFrame-HPC-4.2.1/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/environments.py` & `ReFrame-HPC-4.2.1/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/exceptions.py` & `ReFrame-HPC-4.2.1/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/fields.py` & `ReFrame-HPC-4.2.1/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/fixtures.py` & `ReFrame-HPC-4.2.1/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/hooks.py` & `ReFrame-HPC-4.2.1/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.2.1/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/launchers/local.py` & `ReFrame-HPC-4.2.1/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.2.1/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/launchers/ssh.py` & `ReFrame-HPC-4.2.1/reframe/core/launchers/ssh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/logging.py` & `ReFrame-HPC-4.2.1/reframe/core/logging.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/meta.py` & `ReFrame-HPC-4.2.1/reframe/core/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,21 @@
             '''Expose and control access to the local namespaces.
 
             Variables may only be retrieved if their value has been previously
             set. Accessing a parameter in the class body is disallowed (the
             actual test parameter is set during the class instantiation).
             '''
 
+            def _find_root(v):
+                '''Find root variable of a possibly aliased variable v'''
+                while v.is_alias():
+                    v = v._target
+
+                return v
+
             try:
                 return super().__getitem__(key)
             except KeyError as err:
                 try:
                     # Handle variable access
                     return self['_rfm_local_var_space'][key]
                 except KeyError:
@@ -133,20 +140,37 @@
                     elif key in self['_rfm_local_fixture_space']:
                         raise ReframeSyntaxError(
                             'accessing a fixture from the class body is '
                             'disallowed'
                         ) from None
                     else:
                         # As the last resource, look if key is a variable in
-                        # any of the base classes. If so, make its value
-                        # available in the current class' namespace.
+                        # any of the base classes. If so, create a shadow
+                        # (proxy) variable of it and all of its aliases in the
+                        # current namespace
                         for b in self['_rfm_bases']:
                             if key in b._rfm_var_space:
-                                v = variables.ShadowVar(b._rfm_var_space[key])
-                                self._namespace[key] = v
+                                # We suppress all warnings from the lowering
+                                # of variables here unless this is an alias
+                                v_orig = b._rfm_var_space[key]
+                                warn = False
+                                if v_orig.is_alias():
+                                    # If we need to lower an alias, we will do
+                                    # this through its root variable
+                                    v_orig = _find_root(v_orig)
+                                    warn = True
+
+                                v = variables.ShadowVar(v_orig)
+                                self._namespace[v_orig.name] = v
+                                for ref in v_orig.refs():
+                                    u = variables.ShadowVar(
+                                        ref, alias=v, warnings=warn
+                                    )
+                                    self._namespace[ref.name] = u
+
                                 return v
 
                         # If 'key' is neither a variable nor a parameter,
                         # raise the exception from the base __getitem__.
                         raise err from None
 
         def reset(self, key):
```

### Comparing `ReFrame-HPC-4.2.0/reframe/core/modules.py` & `ReFrame-HPC-4.2.1/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/namespaces.py` & `ReFrame-HPC-4.2.1/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/parameters.py` & `ReFrame-HPC-4.2.1/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/pipeline.py` & `ReFrame-HPC-4.2.1/reframe/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/runtime.py` & `ReFrame-HPC-4.2.1/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.2.1/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/settings.py` & `ReFrame-HPC-4.2.1/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/shell.py` & `ReFrame-HPC-4.2.1/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/systems.py` & `ReFrame-HPC-4.2.1/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/core/variables.py` & `ReFrame-HPC-4.2.1/reframe/core/variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     # NOTE: We can't use truly private fields in `__slots__`, because
     # `__setattr__()` will be called with their mangled name and we cannot
     # match them in the `__slots__` without making implementation-defined
     # assumptions about the mangled name. So we just add the `_p_` prefix for
     # to denote the "private" fields.
 
     __slots__ = ('_p_default_value', '_p_field',
-                 '_loggable', '_name', '_target')
+                 '_loggable', '_name', '_target', '_refs')
 
     __mutable_props = ('_default_value',)
 
     def __init__(self, *args, **kwargs):
         alias = kwargs.pop('alias', None)
         if alias is not None and 'field' in kwargs:
             raise ValueError(f"'field' cannot be set for an alias variable")
@@ -223,36 +223,58 @@
         self._loggable = kwargs.pop('loggable', False)
         if not issubclass(field_type, fields.Field):
             raise TypeError(
                 f'field {field_type!r} is not derived from '
                 f'{fields.Field.__qualname__}'
             )
 
+        self._refs = []
         if alias is not None:
             self._p_field = alias._field
+            alias.add_ref(self)
         else:
             self._p_field = field_type(*args, **kwargs)
 
         self._target = alias
 
     @classmethod
     def create_deprecated(cls, var, message,
                           kind=DEPRECATE_RDWR, from_version='0.0.0'):
         ret = TestVar.__new__(TestVar)
         ret._p_field = fields.DeprecatedField(var.field, message,
                                               kind, from_version)
         ret._p_default_value = var._default_value
         ret._loggable = var._loggable
         ret._target = var._target
+        ret._refs = var._refs
+        if var.is_alias():
+            # If we are deprecating an alias, we need to update the back
+            # reference in the target variable with the deprecated one
+            ret._target.replace_ref(var, ret)
+
         return ret
 
     def _warn_deprecation(self, kind):
         if self.is_deprecated() and self.field.op & kind:
             user_deprecation_warning(self.field.message)
 
+    def replace_ref(self, old, new):
+        for i, ref in enumerate(self._refs):
+            if ref is old:
+                break
+
+        if i < len(self._refs):
+            self._refs[i] = new
+
+    def add_ref(self, var):
+        self._refs.append(var)
+
+    def refs(self):
+        return self._refs
+
     def is_deprecated(self):
         return isinstance(self._p_field, fields.DeprecatedField)
 
     def is_loggable(self):
         return self._loggable
 
     def is_defined(self):
@@ -678,33 +700,53 @@
         self._check_is_defined()
         return math.ceil(self._default_value)
 
 
 class ShadowVar(TestVar):
     '''A shadow instance of another variable.
 
-    This is essentially a fully-fledged shallow copy of another variable. It
-    is used during the construction of the class namespace to bring in scope a
-    requested variable that is defined in a base class (see
+    This is essentially a fully-fledged copy of another variable. It is
+    practically a shallow copy of the variable except its default value, which
+    is deep copied, so that in case it is mutable to allow users to set it
+    without affecting the base classes.
+
+    The ShadowVar is used during the construction of the class namespace to
+    bring in scope a requested variable that is defined in a base class (see
     `MetaNamespace.__getitem__()`)
 
     We could not simply create a reference of the original variable in the
     current namespace, because we need a mechanism to differentiate the
-    lowered variable from any redefinition, which is illegal.
+    lowered variable from any redefinition, which is not allowed.
 
-    Also, we don't need a deep copy, since the shadow variable will replace
-    the original variable in the newly constructed `VarSpace`.
+    Also, we don't need a full deep copy, since the shadow variable will
+    replace the original variable in the newly constructed `VarSpace`.
 
     '''
 
-    def __init__(self, other):
+    def __init__(self, other, alias=None, warnings=True):
+        if alias and not isinstance(alias, ShadowVar):
+            raise TypeError(
+                'a ShadowVar can only be an alias of another ShadowVar'
+            )
+
         for name in self.__slots__:
-            setattr(self, name, getattr(other, name))
+            val = getattr(other, name)
+            if name == '_p_default_value':
+                if alias is not None:
+                    val = alias._default_value
+                else:
+                    val = copy.deepcopy(val)
 
-        self._warn_deprecation(DEPRECATE_RD)
+            setattr(self, name, val)
+
+        if alias is not None:
+            self._target = alias
+
+        if warnings:
+            self._warn_deprecation(DEPRECATE_RD)
 
     def __repr__(self):
         return super().__repr__().replace('TestVar', 'ShadowVar')
 
 
 class VarSpace(namespaces.Namespace):
     '''Variable space of a regression test.
```

### Comparing `ReFrame-HPC-4.2.0/reframe/core/warnings.py` & `ReFrame-HPC-4.2.1/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/argparse.py` & `ReFrame-HPC-4.2.1/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.2.1/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/ci.py` & `ReFrame-HPC-4.2.1/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/cli.py` & `ReFrame-HPC-4.2.1/reframe/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.2.1/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.2.1/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.2.1/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/filters.py` & `ReFrame-HPC-4.2.1/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/loader.py` & `ReFrame-HPC-4.2.1/reframe/frontend/loader.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/printer.py` & `ReFrame-HPC-4.2.1/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/runreport.py` & `ReFrame-HPC-4.2.1/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/statistics.py` & `ReFrame-HPC-4.2.1/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.2.1/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/schemas/config.json` & `ReFrame-HPC-4.2.1/reframe/schemas/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880934966257594%*

 * *Differences: {"'defaults'": "{'logging/handlers_perflog/filelog_append': True, "*

 * *               "'logging/handlers_perflog/filelog_basedir': './perflogs', "*

 * *               "'logging/handlers_perflog/graylog_extras': OrderedDict(), "*

 * *               "'logging/handlers_perflog/httpjson_extras': OrderedDict(), "*

 * *               "'logging/handlers_perflog/httpjson_ignore_keys': [], "*

 * *               "'logging/handlers_perflog/httpjson_json_formatter': None, "*

 * *               "'logging/handlers_perflog/httpjson_extra_headers': O […]*

```diff
@@ -54,35 +54,39 @@
         "logging/handlers*/*_datefmt": "%FT%T",
         "logging/handlers*/*_format": "%(message)s",
         "logging/handlers*/*_format_perfvars": "",
         "logging/handlers*/*_level": "info",
         "logging/handlers*/file_append": false,
         "logging/handlers*/file_name": "",
         "logging/handlers*/file_timestamp": false,
-        "logging/handlers*/filelog_append": true,
-        "logging/handlers*/filelog_basedir": "./perflogs",
-        "logging/handlers*/graylog_extras": {},
-        "logging/handlers*/httpjson_debug": false,
-        "logging/handlers*/httpjson_extra_headers": {},
-        "logging/handlers*/httpjson_extras": {},
-        "logging/handlers*/httpjson_ignore_keys": [],
-        "logging/handlers*/httpjson_json_formatter": null,
         "logging/handlers*/stream_name": "stdout",
         "logging/handlers*/syslog_facility": "user",
         "logging/handlers*/syslog_socktype": "udp",
         "logging/handlers_perflog": [],
+        "logging/handlers_perflog/filelog_append": true,
+        "logging/handlers_perflog/filelog_basedir": "./perflogs",
+        "logging/handlers_perflog/graylog_extras": {},
+        "logging/handlers_perflog/httpjson_debug": false,
+        "logging/handlers_perflog/httpjson_extra_headers": {},
+        "logging/handlers_perflog/httpjson_extras": {},
+        "logging/handlers_perflog/httpjson_ignore_keys": [],
+        "logging/handlers_perflog/httpjson_json_formatter": null,
         "logging/level": "undefined",
         "logging/perflog_compat": false,
         "logging/target_systems": [
             "*"
         ],
         "modes/options": [],
         "modes/target_systems": [
             "*"
         ],
+        "systems*/sched_options/ignore_reqnodenotavail": false,
+        "systems*/sched_options/job_submit_timeout": 60,
+        "systems*/sched_options/resubmit_on_errors": [],
+        "systems*/sched_options/use_nodes_option": false,
         "systems/descr": "",
         "systems/env_vars": [],
         "systems/max_local_jobs": 8,
         "systems/modules": [],
         "systems/modules_system": "nomod",
         "systems/outputdir": "",
         "systems/partitions/access": [],
@@ -104,19 +108,15 @@
         "systems/partitions/resources": [],
         "systems/partitions/resources/options": [],
         "systems/partitions/time_limit": null,
         "systems/partitions/variables": [],
         "systems/prefix": ".",
         "systems/resourcesdir": ".",
         "systems/stagedir": "",
-        "systems/variables": [],
-        "{systems,systems/partitions}/sched_options/ignore_reqnodenotavail": false,
-        "{systems,systems/partitions}/sched_options/job_submit_timeout": 60,
-        "{systems,systems/partitions}/sched_options/resubmit_on_errors": [],
-        "{systems,systems/partitions}/sched_options/use_nodes_option": false
+        "systems/variables": []
     },
     "defs": {
         "alphanum_ext_string": {
             "pattern": "([a-zA-Z_]([a-zA-Z0-9_]|-)*)",
             "type": "string"
         },
         "alphanum_string": {
@@ -692,52 +692,40 @@
                     "handlers": {
                         "items": {
                             "anyOf": [
                                 {
                                     "$ref": "#/defs/file_handler"
                                 },
                                 {
-                                    "$ref": "#/defs/filelog_handler"
-                                },
-                                {
                                     "$ref": "#/defs/graylog_handler"
                                 },
                                 {
                                     "$ref": "#/defs/stream_handler"
                                 },
                                 {
                                     "$ref": "#/defs/syslog_handler"
-                                },
-                                {
-                                    "$ref": "#/defs/httpjson_handler"
                                 }
                             ]
                         },
                         "type": "array"
                     },
                     "handlers$": {
                         "items": {
                             "anyOf": [
                                 {
                                     "$ref": "#/defs/file_handler"
                                 },
                                 {
-                                    "$ref": "#/defs/filelog_handler"
-                                },
-                                {
                                     "$ref": "#/defs/graylog_handler"
                                 },
                                 {
                                     "$ref": "#/defs/stream_handler"
                                 },
                                 {
                                     "$ref": "#/defs/syslog_handler"
-                                },
-                                {
-                                    "$ref": "#/defs/httpjson_handler"
                                 }
                             ]
                         },
                         "minItems": 1,
                         "type": "array"
                     },
                     "handlers_perflog": {
@@ -753,14 +741,17 @@
                                     "$ref": "#/defs/graylog_handler"
                                 },
                                 {
                                     "$ref": "#/defs/stream_handler"
                                 },
                                 {
                                     "$ref": "#/defs/syslog_handler"
+                                },
+                                {
+                                    "$ref": "#/defs/httpjson_handler"
                                 }
                             ]
                         },
                         "type": "array"
                     },
                     "level": {
                         "$ref": "#/defs/loglevel"
```

### Comparing `ReFrame-HPC-4.2.0/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.2.1/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/schemas/runreport.json` & `ReFrame-HPC-4.2.1/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/__init__.py` & `ReFrame-HPC-4.2.1/reframe/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/color.py` & `ReFrame-HPC-4.2.1/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.2.1/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/jsonext.py` & `ReFrame-HPC-4.2.1/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/osext.py` & `ReFrame-HPC-4.2.1/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/profile.py` & `ReFrame-HPC-4.2.1/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/sanity.py` & `ReFrame-HPC-4.2.1/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/typecheck.py` & `ReFrame-HPC-4.2.1/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/udeps.py` & `ReFrame-HPC-4.2.1/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/reframe/utility/versioning.py` & `ReFrame-HPC-4.2.1/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.2.0/setup.cfg` & `ReFrame-HPC-4.2.1/setup.cfg`

 * *Files identical despite different names*


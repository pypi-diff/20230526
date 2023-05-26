# Comparing `tmp/nextstrain-cli-6.2.1.tar.gz` & `tmp/nextstrain-cli-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain-cli-6.2.1.tar", last modified: Fri Mar 24 18:01:49 2023, max compression
+gzip compressed data, was "nextstrain-cli-7.0.0.tar", last modified: Fri May 26 20:34:09 2023, max compression
```

## Comparing `nextstrain-cli-6.2.1.tar` & `nextstrain-cli-7.0.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/LICENSE.cognito-srp
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/LICENSE.sphinx
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.696637 nextstrain-cli-6.2.1/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.700638 nextstrain-cli-6.2.1/nextstrain/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/authn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.700638 nextstrain-cli-6.2.1/nextstrain/cli/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.700638 nextstrain-cli-6.2.1/nextstrain/cli/aws/cognito/
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/aws/cognito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/aws/cognito/srp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.700638 nextstrain-cli-6.2.1/nextstrain/cli/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/check_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/init_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.700638 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/remote/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/command/whoami.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/hostenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain/cli/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/remote/nextstrain_dot_org.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/remote/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/resources/bashrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain/cli/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40176 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/rst/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain/cli/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/ambient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/runner/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/nextstrain/cli/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-24 18:01:49.000000 nextstrain-cli-6.2.1/nextstrain_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 18:01:49.704638 nextstrain-cli-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-24 18:01:37.000000 nextstrain-cli-6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE.cognito-srp
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/LICENSE.sphinx
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.730600 nextstrain-cli-7.0.0/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/authn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/srp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/check_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/init_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/remote/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15564 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/command/whoami.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/nextstrain_dot_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/remote/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.738600 nextstrain-cli-7.0.0/nextstrain/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/resources/bashrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40176 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/rst/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/ambient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17125 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/runner/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/nextstrain/cli/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 20:34:09.000000 nextstrain-cli-7.0.0/nextstrain_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:34:09.742600 nextstrain-cli-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-26 20:33:57.000000 nextstrain-cli-7.0.0/setup.py
```

### Comparing `nextstrain-cli-6.2.1/LICENSE` & `nextstrain-cli-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/LICENSE.cognito-srp` & `nextstrain-cli-7.0.0/LICENSE.cognito-srp`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/LICENSE.sphinx` & `nextstrain-cli-7.0.0/LICENSE.sphinx`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/PKG-INFO` & `nextstrain-cli-7.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 6.2.1
+Version: 7.0.0
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-6.2.1/README.md` & `nextstrain-cli-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/__main__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/argparse.py` & `nextstrain-cli-7.0.0/nextstrain/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/authn.py` & `nextstrain-cli-7.0.0/nextstrain/cli/authn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 """
 Authentication routines.
+
+
+Environment variables
+=====================
+
+.. warning::
+    For development only.  You don't need to set these during normal operation.
+
+.. envvar:: NEXTSTRAIN_COGNITO_USER_POOL_ID
+
+.. envvar:: NEXTSTRAIN_COGNITO_CLI_CLIENT_ID
 """
+import os
 from functools import partial
 from sys import stderr
 from typing import Dict, List, Optional
 
 from . import config
 from .errors import UserError
 from .aws import cognito
 
 
 # Section to use in config.SECRETS file
 CONFIG_SECTION = "authn"
 
 # Public ids.  Client id is specific to the CLI.
-COGNITO_USER_POOL_ID = "us-east-1_Cg5rcTged"
-COGNITO_CLIENT_ID    = "2vmc93kj4fiul8uv40uqge93m5"
+COGNITO_USER_POOL_ID = os.environ.get("NEXTSTRAIN_COGNITO_USER_POOL_ID") \
+                    or "us-east-1_Cg5rcTged"
+
+COGNITO_CLIENT_ID = os.environ.get("NEXTSTRAIN_COGNITO_CLI_CLIENT_ID") \
+                 or "2vmc93kj4fiul8uv40uqge93m5"
 
 CognitoSession = partial(cognito.Session, COGNITO_USER_POOL_ID, COGNITO_CLIENT_ID)
 
 
 class User:
     """
     Data class holding information about a user.
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/aws/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/aws/cognito/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/aws/cognito/srp.py` & `nextstrain-cli-7.0.0/nextstrain/cli/aws/cognito/srp.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/authorization.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/authorization.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/build.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/build.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/check_setup.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/check_setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/deploy.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/deploy.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/init_shell.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/init_shell.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/login.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/login.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/remote/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/remote/delete.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/delete.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/remote/download.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/download.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/remote/ls.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/ls.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/remote/upload.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/remote/upload.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/setup.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/setup.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/shell.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     if overlay_volumes and opts.__runner__ not in {docker, singularity}:
         raise UserError(f"""
             The {runner_name(opts.__runner__)} runtime does not support overlays (e.g. of {overlay_volumes[0].name}).
             Use the Docker or Singularity runtimes (via --docker or --singularity) if overlays are necessary.
             """)
 
-    print(colored("bold", "Entering the Nextstrain runtime"))
+    print(colored("bold", f"Entering the Nextstrain runtime ({runner_name(opts.__runner__)})"))
     print()
 
     if opts.volumes and opts.__runner__ in {docker, singularity}:
         print(colored("bold", "Mapped volumes:"))
 
         # This is more tightly coupled to the Docker/Singularity runners than
         # I'd like (i.e.  assuming /nextstrain/…), but the number of runtimes
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/update.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/update.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/version.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/version.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/view.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/view.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/command/whoami.py` & `nextstrain-cli-7.0.0/nextstrain/cli/command/whoami.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/config.py` & `nextstrain-cli-7.0.0/nextstrain/cli/config.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/console.py` & `nextstrain-cli-7.0.0/nextstrain/cli/console.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/errors.py` & `nextstrain-cli-7.0.0/nextstrain/cli/errors.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/gzip.py` & `nextstrain-cli-7.0.0/nextstrain/cli/gzip.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/hostenv.py` & `nextstrain-cli-7.0.0/nextstrain/cli/hostenv.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/markdown.py` & `nextstrain-cli-7.0.0/nextstrain/cli/markdown.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/paths.py` & `nextstrain-cli-7.0.0/nextstrain/cli/paths.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/remote/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/remote/nextstrain_dot_org.py` & `nextstrain-cli-7.0.0/nextstrain/cli/remote/nextstrain_dot_org.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/remote/s3.py` & `nextstrain-cli-7.0.0/nextstrain/cli/remote/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
     Returns a boolean.
     """
     try:
         object.load()
         return True
     except ClientError as error:
-        if 404 == int(error.response['Error']['Code']):
+        if 404 == int(error.response.get("Error", {}).get("Code", 0)):
             return False
         else:
             raise
 
 
 def guess_type(path: Path) -> Tuple[str, Optional[str]]:
     """
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/resources/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/resources/bashrc` & `nextstrain-cli-7.0.0/nextstrain/cli/resources/bashrc`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/rst/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/rst/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/rst/sphinx.py` & `nextstrain-cli-7.0.0/nextstrain/cli/rst/sphinx.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/ambient.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/ambient.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/__init__.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/jobs.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/jobs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/logs.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/logs.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/aws_batch/s3.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/aws_batch/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import fsspec
 from botocore.config import Config
 from botocore.exceptions import ClientError
 from calendar import timegm
 from os import utime
 from pathlib import Path
 from time import struct_time
-from typing import Callable, Generator, Iterable, List, Optional
+from typing import Callable, Generator, Iterable, List, Optional, Any
 from urllib.parse import urlparse
 from zipfile import ZipFile, ZipInfo
 from ...types import S3Bucket, S3Object
 from ...util import glob_matcher
 
 
 PathMatcher = Callable[[Path], bool]
@@ -61,14 +61,15 @@
 
         # Ignore Python bytecode
         "*.pyc",
         "__pycache__/",
     ])
 
     # Stream writes directly to the remote ZIP file
+    remote_file: Any
     with fsspec.open(object_url(remote_workdir), "wb", auto_mkdir = False) as remote_file:
         with ZipFile(remote_file, "w") as zipfile:
             for path in walk(workdir, excluded):
                 print("zipping:", path)
                 zipfile.write(str(path), str(path.relative_to(workdir)))
 
     return remote_workdir
@@ -104,14 +105,15 @@
 
     if patterns:
         selected = glob_matcher(patterns)
     else:
         selected = lambda path: True
 
     # Open a seekable handle to the remote ZIP file…
+    remote_file: Any
     with fsspec.open(object_url(remote_workdir)) as remote_file:
 
         # …and extract its contents to the workdir.
         with ZipFile(remote_file) as zipfile:
             for member in zipfile.infolist():
                 path = Path(member.filename)
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/conda.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/conda.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 import platform
 import re
 import requests
 import shutil
 import subprocess
 import tarfile
 import traceback
+from packaging.version import parse as parse_version
 from pathlib import Path, PurePosixPath
 from typing import Iterable, NamedTuple, Optional
 from urllib.parse import urljoin, quote as urlquote
 from ..errors import InternalError
 from ..paths import RUNTIMES
 from ..types import RunnerSetupStatus, RunnerTestResults, RunnerUpdateStatus
 from ..util import capture_output, colored, exec_or_return, runner_tests_ok, warn
@@ -539,20 +540,24 @@
 
     if not metafile:
         return None
 
     return json.loads(metafile.read_bytes())
 
 
-def package_distribution(channel: str, package: str, version: str = None) -> Optional[dict]:
+def package_distribution(channel: str, package: str, version: str = None, label: str = "main") -> Optional[dict]:
     # If *package* is a package spec, convert it just to a name.
     package = package_name(package)
 
     if version is None:
-        version = "latest"
+        version = latest_package_label_version(channel, package, label)
+        if version is None:
+            warn(f"Could not find latest version of package {package!r} with label {label!r}.",
+                 "\nUsing 'latest' version instead, which will be the latest version of the package regardless of label.")
+            version = "latest"
 
     response = requests.get(f"https://api.anaconda.org/release/{urlquote(channel)}/{urlquote(package)}/{urlquote(version)}")
     response.raise_for_status()
 
     dists = response.json().get("distributions", [])
 
     system = platform.system()
@@ -566,23 +571,35 @@
     else:
         raise InternalError(f"Unsupported system/machine: {system}/{machine}")
 
     # Releases have other attributes related to system/machine, but they're
     # informational-only and subdir is what Conda *actually* uses to
     # differentiate distributions/files/etc.  Use it too so we have the same
     # view of reality.
-    dist = next((d for d in dists if d.get("attrs", {}).get("subdir") == subdir), None)
+    subdir_dists = (d for d in dists if d.get("attrs", {}).get("subdir") == subdir)
+    dist = max(subdir_dists, default=None, key=lambda d: d.get("attrs", {}).get("build_number", 0))
 
     return dist
 
 
 def package_name(spec: str) -> str:
     return PackageSpec.parse(spec).name
 
 
+def latest_package_label_version(channel: str, package: str, label: str) -> Optional[str]:
+    response = requests.get(f"https://api.anaconda.org/package/{urlquote(channel)}/{urlquote(package)}/files")
+    response.raise_for_status()
+
+    label_files = (file for file in response.json() if label in file.get("labels", []))
+    # Default '0-dev' should be the lowest version according to PEP440
+    # See https://peps.python.org/pep-0440/#summary-of-permitted-suffixes-and-relative-ordering
+    latest_file: dict = max(label_files, default={}, key=lambda file: parse_version(file.get('version', '0-dev')))
+    return latest_file.get("version")
+
+
 class PackageSpec(NamedTuple):
     name: str
     version_spec: Optional[str] = None
     build_id: Optional[str] = None
 
     @staticmethod
     def parse(spec):
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/docker.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/docker.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/runner/singularity.py` & `nextstrain-cli-7.0.0/nextstrain/cli/runner/singularity.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 Uses the images built for the Docker runtime by automatically converting them
 to local Singularity images.  Local images are stored as files named
 :file:`~/.nextstrain/runtimes/singularity/images/{repository}/{tag}.sif`.
 """
 
 import itertools
 import os
+import re
 import shutil
 import subprocess
+from functools import lru_cache
+from packaging.version import Version, InvalidVersion
 from pathlib import Path
-from typing import Iterable, List
+from typing import Iterable, List, Optional
 from urllib.parse import urlsplit
 from .. import config, hostenv
 from ..errors import UserError
 from ..paths import RUNTIMES
 from ..types import RunnerSetupStatus, RunnerTestResults, RunnerUpdateStatus
 from ..util import capture_output, colored, exec_or_return, split_image_name, warn
 from . import docker
@@ -36,32 +39,107 @@
 # use the most recent image and not pin to "build-*" tags.
 #   (copied from ./docker.py on 5 Jan 2022)
 DEFAULT_IMAGE = os.environ.get("NEXTSTRAIN_SINGULARITY_IMAGE") \
              or config.get("singularity", "image") \
              or "docker://nextstrain/base"
 
 
+SINGULARITY_MINIMUM_VERSION = "3.0.0"
+
 SINGULARITY_CONFIG_ENV = {
     # Store image caches in our runtime root instead of ~/.singularity/…
     "SINGULARITY_CACHEDIR": str(CACHE),
+
+    # PROMPT_COMMAND is used by Singularity 3.5.3 onwards to forcibly set PS1
+    # to "Singularity> " on the first evaluation.¹  This happens *after* our
+    # bashrc is evaluated, so our Nextstrain prompt is overwritten.
+    # Singularity appends to any existing PROMPT_COMMAND value, so use a
+    # well-placed comment char (#) to avoid evaluating what it appends.
+    # Additionally unset PROMPT_COMMAND the first time it's evaluated so this
+    # silly workaround doesn't happen on every prompt.
+    #
+    # We set this via the special-cased environment passthru instead of setting
+    # it via an --env arg because --env is only first available in 3.6.0.
+    #
+    # ¹ <https://github.com/sylabs/singularity/commit/30823afc>
+    #   <https://github.com/apptainer/singularity/pull/4616>
+    #   <https://github.com/apptainer/singularity/issues/2721>
+    "SINGULARITYENV_PROMPT_COMMAND": "unset PROMPT_COMMAND; #",
 }
 
-SINGULARITY_EXEC_ARGS = [
+# Not "… = lambda: [" due to mypy.  See commit history.
+def SINGULARITY_EXEC_ARGS(): return [
     # Increase isolation.
     #
     # In the future, we may find we want to use additional related flags to
     # further increase isolation.¹  Note, however, that we'll want to think
     # about the minimum Singularity version we want to support, as many flags
     # in this area are not available on older versions.
     #
-    # ¹ e.g. <https://docs.sylabs.io/guides/latest/user-guide/singularity_and_docker.html#docker-like-compat-flag>
+    #   --compat                (available since 3.9.0; a bundle option)
+    #     --containall            (available since 2.2; a bundle option)
+    #       --contain
+    #       --cleanenv
+    #       --ipc
+    #       --pid
+    #     --writable-tmpfs        (3.0.0)
+    #     --no-init               (3.0.0)
+    #     --no-umask              (3.7.0)
+    #     --no-eval               (3.10.0)
+    #
+    # We opt not to use the --compat bundle option itself mainly for broader
+    # version compatibility but also because what it includes will likely
+    # change over time with newer Singularity releases.  We'd rather a stable,
+    # predictable set of behaviour of our choosing that maximizes
+    # compatibility.
+    #
+    # The options we use here are compatible with Singularity 2.6.0 and newer.
+    #
+    # XXX TODO: Once Singularity 4.0 is released and widely available, we *may*
+    # consider switching from --compat to --oci² for a) stronger Docker-like
+    # isolation and b) no longer having to convert our Docker (OCI) images to
+    # Singularity (SIF) images.  Alternatively, we may want to keep this
+    # runtime as a "middle ground" between the relatively strict isolation of
+    # our Docker runtime and the much looser isolation of the Conda runtime.
+    # Not sure!
+    #   -trs, 23 May 2023
+    #
+    # ¹ <https://docs.sylabs.io/guides/latest/user-guide/singularity_and_docker.html#docker-like-compat-flag>
+    # ² <https://docs.sylabs.io/guides/latest/user-guide/oci_runtime.html#oci-mode>
     "--contain",
+
+    # Don't mount anything at all at the container's value of HOME.  This is
+    # necesary because --compat includes --containall which includes --contain
+    # which makes HOME in the container an empty temporary directory.
+    # --no-home is available since 2.6.0.
     "--no-home",
+
+    # Singularity really wants to default HOME inside the container to the
+    # value from outside the container, thus ignoring the value set by the
+    # upstream Docker image which is only used as a default by the Singularity
+    # image.  Singularity forbids using --env to directly override HOME, so
+    # instead we use --home <src>:<dst> with two empty values.  <src> doesn't
+    # apply because we use --no-home, and setting <dst> to an empty value
+    # allows the container's default to apply (thus avoiding hardcoding it
+    # here).
+    "--home", ":",
+
+    # Allow writes to the image filesystem, discarded at container exit, à la
+    # Docker.  Snakemake, for example, needs to be able to write to HOME
+    # (/nextstrain).
+    "--writable-tmpfs",
+
+    # Don't copy entire host environment.  We forward our own hostenv.
     "--cleanenv",
 
+    # Don't evaluate the entrypoint command line (e.g. arguments passed via
+    # `nextstrain build`) before exec-ing the entrypoint.  It leads to unwanted
+    # substitutions that happen too early.
+    *(["--no-eval"] if singularity_version_at_least("3.10.0") else []),
+
     # Since we use --no-home above, avoid warnings about not being able to cd
     # to $HOME (the default behaviour).  run() will override this by specifying
     # --pwd again.
     "--pwd", "/",
 ]
 
 
@@ -107,15 +185,15 @@
 
         # Plus any extra environment variables provided by us
         **{f"SINGULARITYENV_{k}": v
             for k, v in extra_env.items()},
     }
 
     return exec_or_return([
-        "singularity", "run", *SINGULARITY_EXEC_ARGS,
+        "singularity", "run", *SINGULARITY_EXEC_ARGS(),
 
         # Map directories to bind mount into the container.
         *flatten(("--bind", "%s:%s:%s" % (v.src.resolve(strict = True), docker.mount_point(v), "rw" if v.writable else "ro"))
             for v in opts.volumes
              if v.src is not None),
 
         # Change the default working directory if requested
@@ -162,15 +240,15 @@
     return True
 
 
 def test_setup() -> RunnerTestResults:
     def test_run():
         try:
             capture_output([
-                "singularity", "exec", *SINGULARITY_EXEC_ARGS,
+                "singularity", "exec", *SINGULARITY_EXEC_ARGS(),
 
                 # XXX TODO: We should test --bind, as that's maybe most likely
                 # to be adminstratively disabled, but it's a bit more ceremony
                 # to arrange for a reliable dir to bind into the container.
                 # Putting it off for now…
                 #   -trs, 5 Jan 2023
 
@@ -185,14 +263,16 @@
             return False
         else:
             return True
 
     return [
         ("singularity is installed",
             shutil.which("singularity") is not None),
+        (f"singularity version {singularity_version()} ≥ {SINGULARITY_MINIMUM_VERSION}",
+            singularity_version_at_least(SINGULARITY_MINIMUM_VERSION)),
         ("singularity works",
             test_run()),
     ]
 
 
 def set_default_config() -> None:
     """
@@ -370,10 +450,38 @@
 def run_bash(script: str, image: str = DEFAULT_IMAGE) -> List[str]:
     """
     Run a Bash *script* inside of the container *image*.
 
     Returns the output of the script as a list of strings.
     """
     return capture_output([
-        "singularity", "run", *SINGULARITY_EXEC_ARGS, image_path(image),
+        "singularity", "run", *SINGULARITY_EXEC_ARGS(), image_path(image),
             "bash", "-c", script
     ])
+
+
+@lru_cache(maxsize = None)
+def singularity_version_at_least(min_version: str) -> bool:
+    version = singularity_version()
+
+    if not version:
+        return False
+
+    return version >= Version(min_version)
+
+
+@lru_cache(maxsize = None)
+def singularity_version() -> Optional[Version]:
+    try:
+        raw_version = capture_output(["singularity", "version"])[0]
+    except (OSError, subprocess.CalledProcessError):
+        return None
+
+    try:
+        return Version(raw_version)
+    except InvalidVersion:
+        # Singularity sometimes reports a version like 3.11.1-bionic with a
+        # (for Python) non-standard suffix ("-bionic"), so try stripping it.
+        try:
+            return Version(re.sub(r'-.+$', '', raw_version))
+        except InvalidVersion:
+            return None
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/types.py` & `nextstrain-cli-7.0.0/nextstrain/cli/types.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/util.py` & `nextstrain-cli-7.0.0/nextstrain/cli/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from packaging.version import parse as parse_version
 from pathlib import Path
 from shlex import quote as shquote
 from shutil import which
 from textwrap import dedent, indent
 from wcmatch.glob import globmatch, GLOBSTAR, EXTGLOB, BRACE, MATCHBASE, NEGATE
 from .__version__ import __version__
+from .debug import debug
 from .types import RunnerModule, RunnerTestResults
 
 
 def warn(*args):
     print(*args, file = sys.stderr)
 
 
@@ -272,14 +273,16 @@
     This wrapper around subprocess.run() exists because its own capture_output
     parameter wasn't added until Python 3.7 and we aim for compat with 3.6.
     When we bump our minimum Python version, we can remove this wrapper.
 
     If an *extra_env* mapping is passed, the provided keys and values are
     overlayed onto the current environment.
     """
+    debug(f"capture_output({argv!r}, {extra_env!r})")
+
     env = os.environ.copy()
 
     if extra_env:
         env.update(extra_env)
 
     result = subprocess.run(
         argv,
@@ -304,14 +307,16 @@
     signals.
 
     If an *extra_env* mapping is passed, the provided keys and values are
     overlayed onto the current environment.
 
     ¹ https://bugs.python.org/issue9148
     """
+    debug(f"exec_or_return({argv!r}, {extra_env!r})")
+
     env = os.environ.copy()
 
     if extra_env:
         env.update(extra_env)
 
     # Use a POSIX exec(3) for file descriptor and signal handling…
     if os.name == "posix":
```

### Comparing `nextstrain-cli-6.2.1/nextstrain/cli/volume.py` & `nextstrain-cli-7.0.0/nextstrain/cli/volume.py`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain_cli.egg-info/PKG-INFO` & `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-cli
-Version: 6.2.1
+Version: 7.0.0
 Summary: Nextstrain command-line tool
 Home-page: https://docs.nextstrain.org/projects/cli/
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Project-URL: Bug Reports, https://github.com/nextstrain/cli/issues
 Project-URL: Change Log, https://github.com/nextstrain/cli/blob/master/CHANGES.md
```

### Comparing `nextstrain-cli-6.2.1/nextstrain_cli.egg-info/SOURCES.txt` & `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextstrain-cli-6.2.1/nextstrain_cli.egg-info/requires.txt` & `nextstrain-cli-7.0.0/nextstrain_cli.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 pytest-forked
 recommonmark
 sphinx>=3
 sphinx-argparse~=0.3
 sphinx-autobuild
 sphinx-markdown-tables!=0.0.16
 sphinx_rtd_theme
+types-boto3
+types-botocore
 types-docutils
 types-setuptools
 
 [dev:python_version != "3.6"]
 types-requests
 
 [dev:python_version != "3.9"]
```

### Comparing `nextstrain-cli-6.2.1/setup.py` & `nextstrain-cli-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,16 @@
             "pytest-forked",
             "recommonmark",
             "sphinx>=3",
             "sphinx-argparse ~=0.3",
             "sphinx-autobuild",
             "sphinx-markdown-tables !=0.0.16",
             "sphinx_rtd_theme",
+            "types-boto3",
+            "types-botocore",
             "types-docutils",
             "types-setuptools",
             "types-requests; python_version != '3.6'",
             "types-requests <=2.28.11.12; python_version == '3.6'",
         ],
     },
 )
```


# Comparing `tmp/grayskull-2.3.0.tar.gz` & `tmp/grayskull-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grayskull-2.3.0.tar", last modified: Mon Mar 27 20:20:01 2023, max compression
+gzip compressed data, was "grayskull-2.3.1.tar", last modified: Fri May 26 20:40:27 2023, max compression
```

## Comparing `grayskull-2.3.0.tar` & `grayskull-2.3.1.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.910616 grayskull-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.902616 grayskull-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.902616 grayskull-2.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.902616 grayskull-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-27 20:19:44.000000 grayskull-2.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-27 20:19:44.000000 grayskull-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-27 20:19:44.000000 grayskull-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-03-27 20:19:44.000000 grayskull-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-27 20:19:44.000000 grayskull-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-03-27 20:20:01.910616 grayskull-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-27 20:19:44.000000 grayskull-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.902616 grayskull-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.902616 grayskull-2.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/source/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-27 20:19:44.000000 grayskull-2.3.0/docs/source/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-27 20:19:44.000000 grayskull-2.3.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.906616 grayskull-2.3.0/grayskull/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.906616 grayskull-2.3.0/grayskull/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/base/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/base/pkg_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/base/track_packages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.906616 grayskull-2.3.0/grayskull/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/cli/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.906616 grayskull-2.3.0/grayskull/license/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.910616 grayskull-2.3.0/grayskull/license/data/
--rw-r--r--   0 runner    (1001) docker     (123)    34605 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/AGPL-3.0
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/Apache-2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/BSD-2-Clause
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/BSD-3-Clause
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/BSD-4-Clause
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/CC0-1.0
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/EPL-2.0
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/GPL-2.0
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/GPL-3.0
--rw-r--r--   0 runner    (1001) docker     (123)    26568 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/LGPL-2.1
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/LGPL-3.0
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/MIT
--rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/MPL-2.0
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    62729 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/license/licence_cache.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.910616 grayskull-2.3.0/grayskull/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/abstract_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/cran.py
--rw-r--r--   0 runner    (1001) docker     (123)    31949 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/py_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/py_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/strategy/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-03-27 20:19:44.000000 grayskull-2.3.0/grayskull/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.906616 grayskull-2.3.0/grayskull.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 20:20:01.000000 grayskull-2.3.0/grayskull.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:20:01.910616 grayskull-2.3.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   598691 2023-03-27 20:19:44.000000 grayskull-2.3.0/images/cli_example_grayskull.gif
--rw-r--r--   0 runner    (1001) docker     (123)  1258428 2023-03-27 20:19:44.000000 grayskull-2.3.0/images/cli_example_grayskull_version.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-27 20:19:44.000000 grayskull-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-27 20:19:44.000000 grayskull-2.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 20:20:01.910616 grayskull-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-27 20:19:44.000000 grayskull-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.363641 grayskull-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-26 20:40:10.000000 grayskull-2.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 20:40:10.000000 grayskull-2.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-26 20:40:10.000000 grayskull-2.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-26 20:40:10.000000 grayskull-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 20:40:10.000000 grayskull-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-26 20:40:27.363641 grayskull-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-26 20:40:10.000000 grayskull-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/source/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/source/developer_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 20:40:10.000000 grayskull-2.3.1/docs/source/user_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 20:40:10.000000 grayskull-2.3.1/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/grayskull/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.359641 grayskull-2.3.1/grayskull/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/base/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/base/pkg_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/base/track_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.359641 grayskull-2.3.1/grayskull/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/cli/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.359641 grayskull-2.3.1/grayskull/license/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.359641 grayskull-2.3.1/grayskull/license/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34605 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/AGPL-3.0
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/Apache-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/BSD-2-Clause
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/BSD-3-Clause
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/BSD-4-Clause
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/CC0-1.0
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/EPL-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/GPL-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/GPL-3.0
+-rw-r--r--   0 runner    (1001) docker     (123)    26568 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/LGPL-2.1
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/LGPL-3.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/MIT
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/MPL-2.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62729 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/license/licence_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.359641 grayskull-2.3.1/grayskull/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/abstract_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/cran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31949 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/py_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/py_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/strategy/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-26 20:40:10.000000 grayskull-2.3.1/grayskull/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.355641 grayskull-2.3.1/grayskull.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 20:40:27.000000 grayskull-2.3.1/grayskull.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:40:27.363641 grayskull-2.3.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   598691 2023-05-26 20:40:10.000000 grayskull-2.3.1/images/cli_example_grayskull.gif
+-rw-r--r--   0 runner    (1001) docker     (123)  1258428 2023-05-26 20:40:10.000000 grayskull-2.3.1/images/cli_example_grayskull_version.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-26 20:40:10.000000 grayskull-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 20:40:10.000000 grayskull-2.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:40:27.363641 grayskull-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 20:40:10.000000 grayskull-2.3.1/setup.py
```

### Comparing `grayskull-2.3.0/.github/FUNDING.yml` & `grayskull-2.3.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `grayskull-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `grayskull-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/.github/workflows/codeql.yml` & `grayskull-2.3.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/.github/workflows/publish_pypi.yml` & `grayskull-2.3.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/.github/workflows/tests.yml` & `grayskull-2.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/CODE_OF_CONDUCT.md` & `grayskull-2.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/LICENSE` & `grayskull-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/PKG-INFO` & `grayskull-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: grayskull
-Version: 2.3.0
+Version: 2.3.1
 Summary: Project to generate recipes for conda packages
 Author-email: Marcelo Duarte Trevisani <marceloduartetrevisani@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/conda/grayskull
 Keywords: conda
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS
 
 # Grayskull
 -------------
 [![Tests](https://github.com/conda/grayskull/actions/workflows/tests.yml/badge.svg)](https://github.com/conda/grayskull/actions/workflows/tests.yml) [![Deployment (PyPI)](https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml)
 
@@ -31,15 +32,16 @@
 ## Introduction
 
 Grayskull is an automatic conda recipe generator. <br>
 The main goal of this project is to generate concise recipes
 for [conda-forge](https://conda-forge.org/).
 The Grayskull project was created with the intention to eventually replace `conda skeleton`. <br>
 Presently Grayskull can generate recipes for Python packages available on PyPI and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of other repositories such as CRAN and Conan etc..
+Grayskull can also generate recipes for R packages published on CRAN.
+Future versions of Grayskull will support recipe generation for packages of other repositories such as Conan and CPAN etc..
 
 ## Installation
 
 It is possible to install this project using `pip`:
 ```bash
 pip install grayskull
 ```
@@ -55,15 +57,15 @@
 cd grayskull
 pip install -e .
 ```
 
 ## Usage
 
 It is pretty simple to use `grayskull`. Just call it, pass the repository
- (just `pypi` for now) and the package name.
+ (`pypi` or `cran`) and the package name.
 
 * Example:
 ```bash
 grayskull pypi pytest
 ```
 
 After that `grayskull` will create a folder with the same name as the package
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: grayskull Version: 2.3.0 Summary: Project to
+Metadata-Version: 2.1 Name: grayskull Version: 2.3.1 Summary: Project to
 generate recipes for conda packages Author-email: Marcelo Duarte Trevisani
 gmail.com> License: Apache-2.0 Project-URL: Source, https://github.com/conda/
 grayskull Keywords: conda Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: testing License-File: LICENSE License-File:
-AUTHORS # Grayskull ------------- [![Tests](https://github.com/conda/grayskull/
-actions/workflows/tests.yml/badge.svg)](https://github.com/conda/grayskull/
-actions/workflows/tests.yml) [![Deployment (PyPI)](https://github.com/conda/
-grayskull/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/
-conda/grayskull/actions/workflows/publish_pypi.yml) [![codecov](https://
-codecov.io/gh/conda/grayskull/branch/master/graph/badge.svg)](https://
-codecov.io/gh/conda/grayskull) [![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![](https:/
-/img.shields.io/badge/python-3.8+-blue.svg) ![](https://img.shields.io/github/
-license/conda/grayskull.svg) [![PyPI version](https://badge.fury.io/py/
-grayskull.svg)](https://badge.fury.io/py/grayskull) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/grayskull.svg)](https://anaconda.org/conda-
-forge/grayskull) [![Gitter](https://badges.gitter.im/conda_grayskull/
-community.svg)](https://gitter.im/conda_grayskull/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) ------------
--
+text/markdown Provides-Extra: testing Provides-Extra: docs License-File:
+LICENSE License-File: AUTHORS # Grayskull ------------- [![Tests](https://
+github.com/conda/grayskull/actions/workflows/tests.yml/badge.svg)](https://
+github.com/conda/grayskull/actions/workflows/tests.yml) [![Deployment (PyPI)]
+(https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml/
+badge.svg)](https://github.com/conda/grayskull/actions/workflows/
+publish_pypi.yml) [![codecov](https://codecov.io/gh/conda/grayskull/branch/
+master/graph/badge.svg)](https://codecov.io/gh/conda/grayskull) [![Code style:
+black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) ![](https://img.shields.io/badge/python-3.8+-blue.svg) !
+[](https://img.shields.io/github/license/conda/grayskull.svg) [![PyPI version]
+(https://badge.fury.io/py/grayskull.svg)](https://badge.fury.io/py/grayskull)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/grayskull.svg)]
+(https://anaconda.org/conda-forge/grayskull) [![Gitter](https://
+badges.gitter.im/conda_grayskull/community.svg)](https://gitter.im/
+conda_grayskull/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-
+badge) -------------
 [https://static.wikia.nocookie.net/heman/images/3/33/Grayskull.jpg]
 "Skeletonr's main goal is to conquer the mysterious fortress of Castle
 Grayskull, from which He-Man draws his powers. If he succeeds, Skeletor would
 be able to conquer not only Eternia, but the whole universe." Adapted from
 Wikipedia. Image credits: https://he-man.fandom.com  ------------- ##
 Introduction Grayskull is an automatic conda recipe generator.
 The main goal of this project is to generate concise recipes for [conda-forge]
 (https://conda-forge.org/). The Grayskull project was created with the
 intention to eventually replace `conda skeleton`.
 Presently Grayskull can generate recipes for Python packages available on PyPI
 and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of
-other repositories such as CRAN and Conan etc.. ## Installation It is possible
-to install this project using `pip`: ```bash pip install grayskull ``` or
-`conda`, using the ``conda-forge`` channel: ```bash conda install -c conda-
-forge grayskull ``` It is also possible to clone this repo and install it using
+Grayskull can also generate recipes for R packages published on CRAN. Future
+versions of Grayskull will support recipe generation for packages of other
+repositories such as Conan and CPAN etc.. ## Installation It is possible to
+install this project using `pip`: ```bash pip install grayskull ``` or `conda`,
+using the ``conda-forge`` channel: ```bash conda install -c conda-forge
+grayskull ``` It is also possible to clone this repo and install it using
 `pip`: ```bash git clone https://github.com/conda/grayskull.git cd grayskull
 pip install -e . ``` ## Usage It is pretty simple to use `grayskull`. Just call
-it, pass the repository (just `pypi` for now) and the package name. * Example:
+it, pass the repository (`pypi` or `cran`) and the package name. * Example:
 ```bash grayskull pypi pytest ``` After that `grayskull` will create a folder
 with the same name as the package and inside this folder the generated recipe
 will be present (`meta.yaml`). * Example with `pytest` (`grayskull pypi
 pytest`): ![Grayskull CLI](https://github.com/conda/grayskull/raw/main/images/
 cli_example_grayskull.gif) If your package is a GitHub repository just replace
 the package name with the GitHub repository URL.
 For example:
```

### Comparing `grayskull-2.3.0/README.md` & `grayskull-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 ## Introduction
 
 Grayskull is an automatic conda recipe generator. <br>
 The main goal of this project is to generate concise recipes
 for [conda-forge](https://conda-forge.org/).
 The Grayskull project was created with the intention to eventually replace `conda skeleton`. <br>
 Presently Grayskull can generate recipes for Python packages available on PyPI and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of other repositories such as CRAN and Conan etc..
+Grayskull can also generate recipes for R packages published on CRAN.
+Future versions of Grayskull will support recipe generation for packages of other repositories such as Conan and CPAN etc..
 
 ## Installation
 
 It is possible to install this project using `pip`:
 ```bash
 pip install grayskull
 ```
@@ -41,15 +42,15 @@
 cd grayskull
 pip install -e .
 ```
 
 ## Usage
 
 It is pretty simple to use `grayskull`. Just call it, pass the repository
- (just `pypi` for now) and the package name.
+ (`pypi` or `cran`) and the package name.
 
 * Example:
 ```bash
 grayskull pypi pytest
 ```
 
 After that `grayskull` will create a folder with the same name as the package
```

#### html2text {}

```diff
@@ -21,22 +21,23 @@
 Wikipedia. Image credits: https://he-man.fandom.com  ------------- ##
 Introduction Grayskull is an automatic conda recipe generator.
 The main goal of this project is to generate concise recipes for [conda-forge]
 (https://conda-forge.org/). The Grayskull project was created with the
 intention to eventually replace `conda skeleton`.
 Presently Grayskull can generate recipes for Python packages available on PyPI
 and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of
-other repositories such as CRAN and Conan etc.. ## Installation It is possible
-to install this project using `pip`: ```bash pip install grayskull ``` or
-`conda`, using the ``conda-forge`` channel: ```bash conda install -c conda-
-forge grayskull ``` It is also possible to clone this repo and install it using
+Grayskull can also generate recipes for R packages published on CRAN. Future
+versions of Grayskull will support recipe generation for packages of other
+repositories such as Conan and CPAN etc.. ## Installation It is possible to
+install this project using `pip`: ```bash pip install grayskull ``` or `conda`,
+using the ``conda-forge`` channel: ```bash conda install -c conda-forge
+grayskull ``` It is also possible to clone this repo and install it using
 `pip`: ```bash git clone https://github.com/conda/grayskull.git cd grayskull
 pip install -e . ``` ## Usage It is pretty simple to use `grayskull`. Just call
-it, pass the repository (just `pypi` for now) and the package name. * Example:
+it, pass the repository (`pypi` or `cran`) and the package name. * Example:
 ```bash grayskull pypi pytest ``` After that `grayskull` will create a folder
 with the same name as the package and inside this folder the generated recipe
 will be present (`meta.yaml`). * Example with `pytest` (`grayskull pypi
 pytest`): ![Grayskull CLI](https://github.com/conda/grayskull/raw/main/images/
 cli_example_grayskull.gif) If your package is a GitHub repository just replace
 the package name with the GitHub repository URL.
 For example:
```

### Comparing `grayskull-2.3.0/docs/Makefile` & `grayskull-2.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/docs/make.bat` & `grayskull-2.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/docs/source/conf.py` & `grayskull-2.3.1/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,19 @@
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = []
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinxarg.ext",
+    "myst_parser",
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
```

### Comparing `grayskull-2.3.0/docs/source/index.rst` & `grayskull-2.3.1/docs/source/index.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-.. Grayskull documentation master file, created by
-   sphinx-quickstart on Tue Feb 15 20:08:45 2022.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
+% Grayskull documentation master file, created by
+% sphinx-quickstart on Tue Feb 15 20:08:45 2022.
+% You can adapt this file completely to your liking, but it should at least
+% contain the root `toctree` directive.
 
-Grayskull Documentation
-========================
+# Grayskull Documentation
 
-| **Grayskull** is an automatic conda recipe generator.
-| The main goal of this project is to generate concise recipes for `conda-forge <https://github.com/conda-forge>`_.
+**Grayskull**
 
-| Presently Grayskull can generate recipes for Python packages available on PyPI and also those not published on PyPI but available as GitHub repositories.
-| Future versions of Grayskull will support recipe generation for packages of other repositories such as CRAN and Conan etc..
+ is an automatic conda recipe generator.
 
-| Check out the :doc:`user_guide` section for further information, including how to :ref:`install <installation>` Grayskull.
+The main goal of this project is to generate concise recipes for [conda-forge](https://github.com/conda-forge).
 
+Presently Grayskull can generate recipes for Python packages available on PyPI and also those not published on PyPI but available as GitHub repositories. 
+Grayskull can also generate recipes for R packages published on CRAN.
 
-.. toctree::
-   :maxdepth: 1
-   :caption: Contents:
+Future versions of Grayskull will support recipe generation for packages of other repositories such as Conan, CPAN etc..
 
-   user_guide
-   developer_guide
+Check out the {doc}`user_guide` section for further information, including how
+to {ref}`install <installation>` Grayskull.
 
+```{toctree}
+:caption: 'Contents:'
+:maxdepth: 1
 
+user_guide
+cli
+developer_guide
+```
 
-.. note::
+```{note}
+This project is under active development.
+```
 
-   This project is under active development.
+# Indices and tables
 
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+- {ref}`genindex`
+- {ref}`modindex`
+- {ref}`search`
```

### Comparing `grayskull-2.3.0/grayskull/__main__.py` & `grayskull-2.3.1/grayskull/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,11 +385,7 @@
     maintainers = maintainers or [get_git_current_user()]
     if "extra" in recipe:
         recipe["extra"]["recipe-maintainers"] = maintainers
     else:
         recipe.add_section({"extra": {"recipe-maintainers": maintainers}})
     prefix = f"\n   - {Fore.LIGHTMAGENTA_EX}"
     print_msg(f"\nMaintainers:{prefix}{prefix.join(maintainers)}")
-
-
-if __name__ == "__main__":
-    main(sys.argv[1:])
```

### Comparing `grayskull-2.3.0/grayskull/base/factory.py` & `grayskull-2.3.1/grayskull/base/factory.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/base/github.py` & `grayskull-2.3.1/grayskull/base/github.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/base/pkg_info.py` & `grayskull-2.3.1/grayskull/base/pkg_info.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/base/track_packages.py` & `grayskull-2.3.1/grayskull/base/track_packages.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/cli/__init__.py` & `grayskull-2.3.1/grayskull/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/cli/parser.py` & `grayskull-2.3.1/grayskull/cli/parser.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/cli/stdout.py` & `grayskull-2.3.1/grayskull/cli/stdout.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/config.py` & `grayskull-2.3.1/grayskull/config.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/AGPL-3.0` & `grayskull-2.3.1/grayskull/license/data/AGPL-3.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/Apache-2.0` & `grayskull-2.3.1/grayskull/license/data/Apache-2.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/BSD-2-Clause` & `grayskull-2.3.1/grayskull/license/data/BSD-2-Clause`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/BSD-3-Clause` & `grayskull-2.3.1/grayskull/license/data/BSD-3-Clause`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/BSD-4-Clause` & `grayskull-2.3.1/grayskull/license/data/BSD-4-Clause`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/CC0-1.0` & `grayskull-2.3.1/grayskull/license/data/CC0-1.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/EPL-2.0` & `grayskull-2.3.1/grayskull/license/data/EPL-2.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/GPL-2.0` & `grayskull-2.3.1/grayskull/license/data/GPL-2.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/GPL-3.0` & `grayskull-2.3.1/grayskull/license/data/GPL-3.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/LGPL-2.1` & `grayskull-2.3.1/grayskull/license/data/LGPL-2.1`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/LGPL-3.0` & `grayskull-2.3.1/grayskull/license/data/LGPL-3.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/MIT` & `grayskull-2.3.1/grayskull/license/data/MIT`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/MPL-2.0` & `grayskull-2.3.1/grayskull/license/data/MPL-2.0`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/Unlicense` & `grayskull-2.3.1/grayskull/license/data/Unlicense`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/data/__init__.py` & `grayskull-2.3.1/grayskull/license/data/__init__.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/license/discovery.py` & `grayskull-2.3.1/grayskull/license/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from subprocess import check_output
 from tempfile import mkdtemp
 from typing import List, Optional, Tuple, Union
 
 import requests
 from colorama import Fore
 from rapidfuzz import process
-from rapidfuzz.fuzz import token_set_ratio, token_sort_ratio
+from rapidfuzz.distance import OSA
+from rapidfuzz.fuzz import partial_ratio, token_set_ratio, token_sort_ratio
 
 from grayskull.cli.stdout import print_msg
 from grayskull.license.data import get_all_licenses  # noqa
 
 log = logging.getLogger(__name__)
 
 
@@ -68,34 +69,44 @@
     :return: Information of the license matched
     """
     all_licenses = get_all_licenses_from_spdx()
     if not all_licenses:
         return {}
     name = re.sub(r"\s+license\s*", "", name.strip(), flags=re.IGNORECASE)
 
-    best_matches = process.extract(name, _get_all_license_choice(all_licenses))
+    best_matches = process.extract(
+        name, _get_all_license_choice(all_licenses), scorer=partial_ratio
+    )
+    best_matches = process.extract(name, [lc for lc, *_ in best_matches])
     spdx_license = best_matches[0]
-    if spdx_license[1] != 100:
+
+    if spdx_license[1] < 100:
         best_matches = [lic[0] for lic in best_matches if not lic[0].endswith("-only")]
 
         if best_matches:
-            best_matches = process.extract(name, best_matches, scorer=token_set_ratio)
+            best_matches = process.extract(
+                name, best_matches, scorer=OSA.normalized_similarity
+            )
             spdx_license = best_matches[0]
             best_matches = [lic[0] for lic in best_matches if lic[1] >= spdx_license[1]]
             if len(best_matches) > 1:
                 spdx_license = process.extractOne(
                     name, best_matches, scorer=token_sort_ratio
                 )
+    if spdx_license[1] != 100 and spdx_license[0].startswith("MIT"):
+        spdx_license = "MIT"
+    else:
+        spdx_license = spdx_license[0]
 
     log.info(
         f"Best match for license {name} was {spdx_license}.\n"
         f"Best matches: {best_matches}"
     )
 
-    return _get_license(spdx_license[0], all_licenses)
+    return _get_license(spdx_license, all_licenses)
 
 
 def get_short_license_id(name: str) -> str:
     """Get the spdx identifier for the given license name
 
     :param name: License name
     :return: short identifier (spdx) for the given license name
```

### Comparing `grayskull-2.3.0/grayskull/license/licence_cache.json` & `grayskull-2.3.1/grayskull/license/licence_cache.json`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/strategy/config.yaml` & `grayskull-2.3.1/grayskull/strategy/config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,18 @@
   conda_forge: python-cufflinks
   import_name: cufflinks
 
 dask:
   conda_forge: dask-core
   import_name: dask
 
+data-morph-ai:
+  conda_forge: data-morph-ai
+  import_name: data_morph
+
 datadotworld:
   conda_forge: datadotworld-py
   import_name: datadotworld
 
 datalad_container:
   conda_forge: datalad-container
   import_name: datalad_container
```

### Comparing `grayskull-2.3.0/grayskull/strategy/cran.py` & `grayskull-2.3.1/grayskull/strategy/cran.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/strategy/py_base.py` & `grayskull-2.3.1/grayskull/strategy/py_base.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/strategy/py_toml.py` & `grayskull-2.3.1/grayskull/strategy/py_toml.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     return semver.VersionInfo(**ver)
 
 
 def coerce_to_semver(version: str) -> str:
     """
     Coerces a version string to a semantic version.
     """
-    if semver.VersionInfo.isvalid(version):
+    if semver.VersionInfo.is_valid(version):
         return version
 
     return str(vdict_to_vinfo(parse_version(version)))
 
 
 def get_caret_ceiling(target: str) -> str:
     """
@@ -77,15 +77,15 @@
     rightmost specified digit and then coercing it to semver.
     Example: 0 => 1.0.0, 0.1 => 0.2.0, 0.1.2 => 0.1.3
 
     - If the major version is not 0, the ceiling is determined by
     coercing it to semver and then bumping the major version.
     Example: 1 => 2.0.0, 1.2 => 2.0.0, 1.2.3 => 2.0.0
     """
-    if not semver.VersionInfo.isvalid(target):
+    if not semver.VersionInfo.is_valid(target):
         target_dict = parse_version(target)
 
         if target_dict["major"] == 0:
             if target_dict["minor"] is None:
                 target_dict["major"] += 1
             elif target_dict["patch"] is None:
                 target_dict["minor"] += 1
@@ -159,16 +159,16 @@
         "Expected Poetry dependency specification to be of type str or dict, "
         f"received {type(dep_spec).__name__}"
     )
 
 
 @get_constrained_dep.register
 def __get_constrained_dep_dict(dep_spec: dict, dep_name: str):
-    conda_version = encode_poetry_version(dep_spec["version"])
-    return f"{dep_name} {conda_version}"
+    conda_version = encode_poetry_version(dep_spec.get("version", ""))
+    return f"{dep_name} {conda_version}".strip()
 
 
 @get_constrained_dep.register
 def __get_constrained_dep_str(dep_spec: str, dep_name: str):
     conda_version = encode_poetry_version(dep_spec)
     return f"{dep_name} {conda_version}"
```

### Comparing `grayskull-2.3.0/grayskull/strategy/pypi.py` & `grayskull-2.3.1/grayskull/strategy/pypi.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull/utils.py` & `grayskull-2.3.1/grayskull/utils.py`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/grayskull.egg-info/PKG-INFO` & `grayskull-2.3.1/grayskull.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: grayskull
-Version: 2.3.0
+Version: 2.3.1
 Summary: Project to generate recipes for conda packages
 Author-email: Marcelo Duarte Trevisani <marceloduartetrevisani@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/conda/grayskull
 Keywords: conda
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+Provides-Extra: docs
 License-File: LICENSE
 License-File: AUTHORS
 
 # Grayskull
 -------------
 [![Tests](https://github.com/conda/grayskull/actions/workflows/tests.yml/badge.svg)](https://github.com/conda/grayskull/actions/workflows/tests.yml) [![Deployment (PyPI)](https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml)
 
@@ -31,15 +32,16 @@
 ## Introduction
 
 Grayskull is an automatic conda recipe generator. <br>
 The main goal of this project is to generate concise recipes
 for [conda-forge](https://conda-forge.org/).
 The Grayskull project was created with the intention to eventually replace `conda skeleton`. <br>
 Presently Grayskull can generate recipes for Python packages available on PyPI and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of other repositories such as CRAN and Conan etc..
+Grayskull can also generate recipes for R packages published on CRAN.
+Future versions of Grayskull will support recipe generation for packages of other repositories such as Conan and CPAN etc..
 
 ## Installation
 
 It is possible to install this project using `pip`:
 ```bash
 pip install grayskull
 ```
@@ -55,15 +57,15 @@
 cd grayskull
 pip install -e .
 ```
 
 ## Usage
 
 It is pretty simple to use `grayskull`. Just call it, pass the repository
- (just `pypi` for now) and the package name.
+ (`pypi` or `cran`) and the package name.
 
 * Example:
 ```bash
 grayskull pypi pytest
 ```
 
 After that `grayskull` will create a folder with the same name as the package
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1 Name: grayskull Version: 2.3.0 Summary: Project to
+Metadata-Version: 2.1 Name: grayskull Version: 2.3.1 Summary: Project to
 generate recipes for conda packages Author-email: Marcelo Duarte Trevisani
 gmail.com> License: Apache-2.0 Project-URL: Source, https://github.com/conda/
 grayskull Keywords: conda Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: testing License-File: LICENSE License-File:
-AUTHORS # Grayskull ------------- [![Tests](https://github.com/conda/grayskull/
-actions/workflows/tests.yml/badge.svg)](https://github.com/conda/grayskull/
-actions/workflows/tests.yml) [![Deployment (PyPI)](https://github.com/conda/
-grayskull/actions/workflows/publish_pypi.yml/badge.svg)](https://github.com/
-conda/grayskull/actions/workflows/publish_pypi.yml) [![codecov](https://
-codecov.io/gh/conda/grayskull/branch/master/graph/badge.svg)](https://
-codecov.io/gh/conda/grayskull) [![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![](https:/
-/img.shields.io/badge/python-3.8+-blue.svg) ![](https://img.shields.io/github/
-license/conda/grayskull.svg) [![PyPI version](https://badge.fury.io/py/
-grayskull.svg)](https://badge.fury.io/py/grayskull) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/grayskull.svg)](https://anaconda.org/conda-
-forge/grayskull) [![Gitter](https://badges.gitter.im/conda_grayskull/
-community.svg)](https://gitter.im/conda_grayskull/
-community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) ------------
--
+text/markdown Provides-Extra: testing Provides-Extra: docs License-File:
+LICENSE License-File: AUTHORS # Grayskull ------------- [![Tests](https://
+github.com/conda/grayskull/actions/workflows/tests.yml/badge.svg)](https://
+github.com/conda/grayskull/actions/workflows/tests.yml) [![Deployment (PyPI)]
+(https://github.com/conda/grayskull/actions/workflows/publish_pypi.yml/
+badge.svg)](https://github.com/conda/grayskull/actions/workflows/
+publish_pypi.yml) [![codecov](https://codecov.io/gh/conda/grayskull/branch/
+master/graph/badge.svg)](https://codecov.io/gh/conda/grayskull) [![Code style:
+black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) ![](https://img.shields.io/badge/python-3.8+-blue.svg) !
+[](https://img.shields.io/github/license/conda/grayskull.svg) [![PyPI version]
+(https://badge.fury.io/py/grayskull.svg)](https://badge.fury.io/py/grayskull)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/grayskull.svg)]
+(https://anaconda.org/conda-forge/grayskull) [![Gitter](https://
+badges.gitter.im/conda_grayskull/community.svg)](https://gitter.im/
+conda_grayskull/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-
+badge) -------------
 [https://static.wikia.nocookie.net/heman/images/3/33/Grayskull.jpg]
 "Skeletonr's main goal is to conquer the mysterious fortress of Castle
 Grayskull, from which He-Man draws his powers. If he succeeds, Skeletor would
 be able to conquer not only Eternia, but the whole universe." Adapted from
 Wikipedia. Image credits: https://he-man.fandom.com  ------------- ##
 Introduction Grayskull is an automatic conda recipe generator.
 The main goal of this project is to generate concise recipes for [conda-forge]
 (https://conda-forge.org/). The Grayskull project was created with the
 intention to eventually replace `conda skeleton`.
 Presently Grayskull can generate recipes for Python packages available on PyPI
 and also those not published on PyPI but available as GitHub repositories.
-Future versions of Grayskull will support recipe generation for packages of
-other repositories such as CRAN and Conan etc.. ## Installation It is possible
-to install this project using `pip`: ```bash pip install grayskull ``` or
-`conda`, using the ``conda-forge`` channel: ```bash conda install -c conda-
-forge grayskull ``` It is also possible to clone this repo and install it using
+Grayskull can also generate recipes for R packages published on CRAN. Future
+versions of Grayskull will support recipe generation for packages of other
+repositories such as Conan and CPAN etc.. ## Installation It is possible to
+install this project using `pip`: ```bash pip install grayskull ``` or `conda`,
+using the ``conda-forge`` channel: ```bash conda install -c conda-forge
+grayskull ``` It is also possible to clone this repo and install it using
 `pip`: ```bash git clone https://github.com/conda/grayskull.git cd grayskull
 pip install -e . ``` ## Usage It is pretty simple to use `grayskull`. Just call
-it, pass the repository (just `pypi` for now) and the package name. * Example:
+it, pass the repository (`pypi` or `cran`) and the package name. * Example:
 ```bash grayskull pypi pytest ``` After that `grayskull` will create a folder
 with the same name as the package and inside this folder the generated recipe
 will be present (`meta.yaml`). * Example with `pytest` (`grayskull pypi
 pytest`): ![Grayskull CLI](https://github.com/conda/grayskull/raw/main/images/
 cli_example_grayskull.gif) If your package is a GitHub repository just replace
 the package name with the GitHub repository URL.
 For example:
```

### Comparing `grayskull-2.3.0/grayskull.egg-info/SOURCES.txt` & `grayskull-2.3.1/grayskull.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 setup.py
 .github/CODEOWNERS
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/codeql.yml
 .github/workflows/publish_pypi.yml
+.github/workflows/sphinx.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/make.bat
+docs/requirements.txt
+docs/source/cli.md
 docs/source/conf.py
-docs/source/developer_guide.rst
-docs/source/index.rst
-docs/source/user_guide.rst
+docs/source/developer_guide.md
+docs/source/index.md
+docs/source/user_guide.md
 grayskull/__init__.py
 grayskull/__main__.py
 grayskull/_version.py
 grayskull/config.py
+grayskull/main.py
 grayskull/utils.py
 grayskull.egg-info/PKG-INFO
 grayskull.egg-info/SOURCES.txt
 grayskull.egg-info/dependency_links.txt
 grayskull.egg-info/entry_points.txt
 grayskull.egg-info/requires.txt
 grayskull.egg-info/top_level.txt
```

### Comparing `grayskull-2.3.0/images/cli_example_grayskull.gif` & `grayskull-2.3.1/images/cli_example_grayskull.gif`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/images/cli_example_grayskull_version.gif` & `grayskull-2.3.1/images/cli_example_grayskull_version.gif`

 * *Files identical despite different names*

### Comparing `grayskull-2.3.0/pyproject.toml` & `grayskull-2.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 [build-system]
-requires = [
-    "setuptools >=61",
-    "setuptools_scm[toml]>=6.2",
-]
+requires = ["setuptools >=61", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "grayskull"
 authors = [
-    {name = "Marcelo Duarte Trevisani", email = "marceloduartetrevisani@gmail.com"},
+    { name = "Marcelo Duarte Trevisani", email = "marceloduartetrevisani@gmail.com" },
 ]
 description = "Project to generate recipes for conda packages"
 readme = "README.md"
 keywords = ["conda"]
-license = {text = "Apache-2.0"}
+license = { text = "Apache-2.0" }
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "beautifulsoup4",
     "colorama",
     "conda-souschef >=2.2.3",
     "packaging >=21.3",
     "pip",
     "pkginfo",
     "progressbar2 >=3.53.0",
-    "rapidfuzz >=1.7.1",
+    "rapidfuzz >=3.0.0",
     "requests",
     "ruamel.yaml >=0.16.10",
     "ruamel.yaml.jinja2",
     "setuptools >=30.3.0",
-    "semver~=2.13.0",
+    "semver~=3.0.0",
     "stdlib-list",
     "tomli",
     "tomli-w",
 ]
 
 [project.optional-dependencies]
 testing = [
@@ -41,32 +38,40 @@
     "pytest",
     "pytest-console-scripts",
     "pytest-cov",
     "pytest-mock",
     "setuptools-scm",
 ]
 
+docs = [
+    "furo",
+    "sphinx",
+    "sphinx-argparse",
+    "myst-parser",
+    "mdit-py-plugins>=0.3.0",
+]
+
 [project.scripts]
-grayskull = "grayskull.__main__:main"
-greyskull = "grayskull.__main__:main"
-conda-grayskull = "grayskull.__main__:main"
-conda-greyskull = "grayskull.__main__:main"
+grayskull = "grayskull.main:main"
+greyskull = "grayskull.main:main"
+conda-grayskull = "grayskull.main:main"
+conda-greyskull = "grayskull.main:main"
 
 [project.urls]
 Source = "https://github.com/conda/grayskull"
 
 [tool.setuptools.packages.find]
 include = ["grayskull", "grayskull.*"]
 
 [tool.setuptools_scm]
 write_to = "grayskull/_version.py"
 
 [tool.black]
-target-version=["py310"]
-exclude='''
+target-version = ["py310"]
+exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
   | \.tox
   | \.venv
```


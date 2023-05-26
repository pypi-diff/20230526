# Comparing `tmp/license-expression-30.1.0.tar.gz` & `tmp/license-expression-30.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license-expression-30.1.0.tar", last modified: Tue Jan 17 18:34:01 2023, max compression
+gzip compressed data, was "license-expression-30.1.1.tar", last modified: Fri May 26 14:52:07 2023, max compression
```

## Comparing `license-expression-30.1.0.tar` & `license-expression-30.1.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-01-17 18:33:51.000000 license-expression-30.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.389353 license-expression-30.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.389353 license-expression-30.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-01-17 18:33:51.000000 license-expression-30.1.0/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-01-17 18:33:51.000000 license-expression-30.1.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-01-17 18:33:51.000000 license-expression-30.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-01-17 18:33:51.000000 license-expression-30.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-01-17 18:33:51.000000 license-expression-30.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-01-17 18:33:51.000000 license-expression-30.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-01-17 18:33:51.000000 license-expression-30.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-01-17 18:33:51.000000 license-expression-30.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-01-17 18:33:51.000000 license-expression-30.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      733 2023-01-17 18:33:51.000000 license-expression-30.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    11746 2023-01-17 18:34:01.397353 license-expression-30.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10713 2023-01-17 18:33:51.000000 license-expression-30.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-17 18:33:51.000000 license-expression-30.1.0/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-01-17 18:33:51.000000 license-expression-30.1.0/azure-pipelines.yml
--rwxr-xr-x   0 runner    (1001) docker     (122)     6328 2023-01-17 18:33:51.000000 license-expression-30.1.0/configure
--rwxr-xr-x   0 runner    (1001) docker     (122)     6948 2023-01-17 18:33:51.000000 license-expression-30.1.0/configure.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/api/license_expression.rst
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3178 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-01-17 18:33:51.000000 license-expression-30.1.0/docs/source/readme_link.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.389353 license-expression-30.1.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.393353 license-expression-30.1.0/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     3744 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (122)     9486 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (122)     6704 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)    75931 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-01-17 18:33:51.000000 license-expression-30.1.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-01-17 18:33:51.000000 license-expression-30.1.0/license-expression.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-01-17 18:33:51.000000 license-expression-30.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 18:33:51.000000 license-expression-30.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 18:33:51.000000 license-expression-30.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-01-17 18:34:01.397353 license-expression-30.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-01-17 18:33:51.000000 license-expression-30.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.389353 license-expression-30.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/src/license_expression/
--rw-r--r--   0 runner    (1001) docker     (122)    62814 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/_pyahocorasick.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)    20579 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/_pyahocorasick.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/src/license_expression/data/
--rw-r--r--   0 runner    (1001) docker     (122)    18651 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/data/cc-by-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/data/license_key_index.json.ABOUT
--rw-r--r--   0 runner    (1001) docker     (122)   765991 2023-01-17 18:33:51.000000 license-expression-30.1.0/src/license_expression/data/scancode-licensedb-index.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/src/license_expression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11746 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-17 18:34:01.000000 license-expression-30.1.0/src/license_expression.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 18:34:01.397353 license-expression-30.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-01-17 18:33:51.000000 license-expression-30.1.0/tests/data/test_license_key_index.json
--rw-r--r--   0 runner    (1001) docker     (122)    10583 2023-01-17 18:33:51.000000 license-expression-30.1.0/tests/test__pyahocorasick.py
--rw-r--r--   0 runner    (1001) docker     (122)   100983 2023-01-17 18:33:51.000000 license-expression-30.1.0/tests/test_license_expression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-01-17 18:33:51.000000 license-expression-30.1.0/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-01-17 18:33:51.000000 license-expression-30.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.169302 license-expression-30.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-26 14:51:54.000000 license-expression-30.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.149302 license-expression-30.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.153302 license-expression-30.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-05-26 14:51:54.000000 license-expression-30.1.1/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-05-26 14:51:54.000000 license-expression-30.1.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-26 14:51:54.000000 license-expression-30.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-26 14:51:54.000000 license-expression-30.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-05-26 14:51:54.000000 license-expression-30.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-05-26 14:51:54.000000 license-expression-30.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-05-26 14:51:54.000000 license-expression-30.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-26 14:51:54.000000 license-expression-30.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-26 14:51:54.000000 license-expression-30.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-26 14:51:54.000000 license-expression-30.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    11746 2023-05-26 14:52:07.169302 license-expression-30.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10713 2023-05-26 14:51:54.000000 license-expression-30.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-26 14:51:54.000000 license-expression-30.1.1/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-26 14:51:54.000000 license-expression-30.1.1/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6328 2023-05-26 14:51:54.000000 license-expression-30.1.1/configure
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6948 2023-05-26 14:51:54.000000 license-expression-30.1.1/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.153302 license-expression-30.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.153302 license-expression-30.1.1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.157302 license-expression-30.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.157302 license-expression-30.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.157302 license-expression-30.1.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/api/license_expression.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3178 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-26 14:51:54.000000 license-expression-30.1.1/docs/source/readme_link.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.149302 license-expression-30.1.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.157302 license-expression-30.1.1/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.161302 license-expression-30.1.1/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3744 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9486 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6704 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75931 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-26 14:51:54.000000 license-expression-30.1.1/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-26 14:51:54.000000 license-expression-30.1.1/license-expression.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-05-26 14:51:54.000000 license-expression-30.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 14:51:54.000000 license-expression-30.1.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 14:51:54.000000 license-expression-30.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-05-26 14:52:07.169302 license-expression-30.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-26 14:51:54.000000 license-expression-30.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.149302 license-expression-30.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.161302 license-expression-30.1.1/src/license_expression/
+-rw-r--r--   0 runner    (1001) docker     (122)    62814 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/_pyahocorasick.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    20579 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/_pyahocorasick.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.165302 license-expression-30.1.1/src/license_expression/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    18651 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/data/cc-by-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/data/license_key_index.json.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)   802727 2023-05-26 14:51:54.000000 license-expression-30.1.1/src/license_expression/data/scancode-licensedb-index.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.165302 license-expression-30.1.1/src/license_expression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11746 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-26 14:52:07.000000 license-expression-30.1.1/src/license_expression.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.165302 license-expression-30.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 14:52:07.165302 license-expression-30.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-26 14:51:54.000000 license-expression-30.1.1/tests/data/test_license_key_index.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10583 2023-05-26 14:51:54.000000 license-expression-30.1.1/tests/test__pyahocorasick.py
+-rw-r--r--   0 runner    (1001) docker     (122)   100983 2023-05-26 14:51:54.000000 license-expression-30.1.1/tests/test_license_expression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-05-26 14:51:54.000000 license-expression-30.1.1/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-26 14:51:54.000000 license-expression-30.1.1/tox.ini
```

### Comparing `license-expression-30.1.0/.github/workflows/docs-ci.yml` & `license-expression-30.1.1/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/.github/workflows/pypi-release.yml` & `license-expression-30.1.1/.github/workflows/pypi-release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         uses: actions/upload-artifact@v3
         with:
           name: pypi_archives
           path: dist/*
 
 
   create-gh-release:
+  # Sets permissions of the GITHUB_TOKEN to allow release upload
+    permissions:
+      contents: write
     name: Create GH release
     needs:
       - build-pypi-distribs
     runs-on: ubuntu-20.04
 
     steps:
       - name: Download built archives
```

### Comparing `license-expression-30.1.0/.gitignore` & `license-expression-30.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/CHANGELOG.rst` & `license-expression-30.1.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+v30.1.1 - 2023-01-16
+----------------------
+
+This is a minor dot release without API changes
+
+- Use latest skeleton
+- Update license list to latest ScanCode and SPDX 3.20
+
 
 v30.1.0 - 2023-01-16
 ----------------------
 
 This is a minor release without API changes
 
 - Use latest skeleton (and updated configure script)
```

### Comparing `license-expression-30.1.0/CODE_OF_CONDUCT.rst` & `license-expression-30.1.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/Makefile` & `license-expression-30.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/NOTICE` & `license-expression-30.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/PKG-INFO` & `license-expression-30.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-expression
-Version: 30.1.0
+Version: 30.1.1
 Summary: license-expression is a comprehensive utility library to parse, compare, simplify and normalize license expressions (such as SPDX license expressions) using boolean logic.
 Home-page: https://github.com/nexB/license-expression
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,license expression,license,spdx,boolean,parse expression,normalize expression,compare expression,licence
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,15 +46,15 @@
 npm and Rubygems; they are important when exchanging software data (such as with
 SPDX and SBOM in general) as a way to express licensing precisely.
 
 ``license-expression`` is a comprehensive utility library to parse, compare,
 simplify and normalize these license expressions (such as SPDX license expressions)
 using boolean logic like in: `GPL-2.0-or-later WITH Classpath-exception-2.0 AND MIT`.
 
-It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.19)
+It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.20)
 and ScanCode license DB (version 21.6.7) https://scancode-licensedb.aboutcode.org/
 to get started quickly.
 
 ``license-expression`` is both powerful and simple to use and is a used as the
 license expression engine in several projects and products such as:
 
 - AboutCode-toolkit https://github.com/nexB/aboutcode-toolkit
@@ -132,15 +132,15 @@
 This supports SPDX license expressions and also accepts other license naming
 conventions and license identifiers aliases to resolve and normalize any license
 expressions.
 
 Using boolean logic, license expressions can be tested for equality, containment,
 equivalence and can be normalized or simplified.
 
-It also bundles the SPDX License list (3.19 as of now) and the ScanCode license
+It also bundles the SPDX License list (3.20 as of now) and the ScanCode license
 DB (based on latest ScanCode) to easily parse and validate expressions using
 the license symbols.
 
 
 Usage examples
 ==============
```

### Comparing `license-expression-30.1.0/README.rst` & `license-expression-30.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 npm and Rubygems; they are important when exchanging software data (such as with
 SPDX and SBOM in general) as a way to express licensing precisely.
 
 ``license-expression`` is a comprehensive utility library to parse, compare,
 simplify and normalize these license expressions (such as SPDX license expressions)
 using boolean logic like in: `GPL-2.0-or-later WITH Classpath-exception-2.0 AND MIT`.
 
-It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.19)
+It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.20)
 and ScanCode license DB (version 21.6.7) https://scancode-licensedb.aboutcode.org/
 to get started quickly.
 
 ``license-expression`` is both powerful and simple to use and is a used as the
 license expression engine in several projects and products such as:
 
 - AboutCode-toolkit https://github.com/nexB/aboutcode-toolkit
@@ -107,15 +107,15 @@
 This supports SPDX license expressions and also accepts other license naming
 conventions and license identifiers aliases to resolve and normalize any license
 expressions.
 
 Using boolean logic, license expressions can be tested for equality, containment,
 equivalence and can be normalized or simplified.
 
-It also bundles the SPDX License list (3.19 as of now) and the ScanCode license
+It also bundles the SPDX License list (3.20 as of now) and the ScanCode license
 DB (based on latest ScanCode) to easily parse and validate expressions using
 the license symbols.
 
 
 Usage examples
 ==============
```

### Comparing `license-expression-30.1.0/apache-2.0.LICENSE` & `license-expression-30.1.1/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/azure-pipelines.yml` & `license-expression-30.1.1/azure-pipelines.yml`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,14 @@
 # These jobs are using VMs with Azure-provided Python builds
 ################################################################################
 
 jobs:
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: ubuntu18_cpython
-          image_name: ubuntu-18.04
-          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
-          test_suites:
-              all: venv/bin/pytest -n 2 -vvs
-
-    - template: etc/ci/azure-posix.yml
-      parameters:
           job_name: ubuntu20_cpython
           image_name: ubuntu-20.04
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
@@ -29,22 +21,14 @@
           image_name: ubuntu-22.04
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: macos1015_cpython
-          image_name: macos-10.15
-          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
-          test_suites:
-              all: venv/bin/pytest -n 2 -vvs
-
-    - template: etc/ci/azure-posix.yml
-      parameters:
           job_name: macos11_cpython
           image_name: macos-11
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
```

### Comparing `license-expression-30.1.0/configure` & `license-expression-30.1.1/configure`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/configure.bat` & `license-expression-30.1.1/configure.bat`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/docs/Makefile` & `license-expression-30.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/docs/make.bat` & `license-expression-30.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/docs/source/_static/theme_overrides.css` & `license-expression-30.1.1/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/docs/source/conf.py` & `license-expression-30.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/azure-container-deb.yml` & `license-expression-30.1.1/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/azure-container-rpm.yml` & `license-expression-30.1.1/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/azure-posix.yml` & `license-expression-30.1.1/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/azure-win.yml` & `license-expression-30.1.1/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/macports-ci` & `license-expression-30.1.1/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/macports-ci.ABOUT` & `license-expression-30.1.1/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/ci/mit.LICENSE` & `license-expression-30.1.1/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/README.rst` & `license-expression-30.1.1/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/check_thirdparty.py` & `license-expression-30.1.1/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/fetch_thirdparty.py` & `license-expression-30.1.1/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/gen_pypi_simple.py` & `license-expression-30.1.1/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `license-expression-30.1.1/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/gen_requirements.py` & `license-expression-30.1.1/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/gen_requirements_dev.py` & `license-expression-30.1.1/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `license-expression-30.1.1/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/test_utils_pypi_supported_tags.py` & `license-expression-30.1.1/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `license-expression-30.1.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_dejacode.py` & `license-expression-30.1.1/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_pip_compatibility_tags.py` & `license-expression-30.1.1/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_pypi_supported_tags.py` & `license-expression-30.1.1/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `license-expression-30.1.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_requirements.py` & `license-expression-30.1.1/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_thirdparty.py` & `license-expression-30.1.1/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/etc/scripts/utils_thirdparty.py.ABOUT` & `license-expression-30.1.1/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/pyproject.toml` & `license-expression-30.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/setup.cfg` & `license-expression-30.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = license-expression
+version = 30.1.1
 license = Apache-2.0
 description = license-expression is a comprehensive utility library to parse, compare, simplify and normalize license expressions (such as SPDX license expressions) using boolean logic.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/nexB/license-expression
 author = nexB. Inc. and others
 author_email = info@aboutcode.org
@@ -49,15 +50,15 @@
 testing = 
 	pytest >= 6, != 7.0.0
 	pytest-xdist >= 2
 	twine
 	black
 	isort
 docs = 
-	Sphinx >= 3.3.1
+	Sphinx == 5.1.0
 	sphinx-rtd-theme >= 0.5.0
 	sphinxcontrib-apidoc >= 0.3.0
 	doc8 >= 0.8.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `license-expression-30.1.0/src/license_expression/__init__.py` & `license-expression-30.1.1/src/license_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/src/license_expression/_pyahocorasick.ABOUT` & `license-expression-30.1.1/src/license_expression/_pyahocorasick.ABOUT`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/src/license_expression/_pyahocorasick.py` & `license-expression-30.1.1/src/license_expression/_pyahocorasick.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/src/license_expression/data/cc-by-4.0.LICENSE` & `license-expression-30.1.1/src/license_expression/data/cc-by-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/src/license_expression/data/scancode-licensedb-index.json` & `license-expression-30.1.1/src/license_expression/data/scancode-licensedb-index.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9555270522388064%*

 * *Differences: {'105': "{'category': 'Proprietary Free'}",*

 * * '1082': "{'spdx_license_key': 'xlock', 'other_spdx_license_keys': ['LicenseRef-scancode-libpbm']}",*

 * * '1151': "{'spdx_license_key': 'HPND-Markus-Kuhn', 'other_spdx_license_keys': "*

 * *         "['LicenseRef-scancode-markus-kuhn-license']}",*

 * * '1152': "{'spdx_license_key': 'Martin-Birgmeier', 'other_spdx_license_keys': "*

 * *         "['LicenseRef-scancode-martin-birgmeier']}",*

 * * '1190': "{'spdx_license_key': 'MIT-Wu', 'other_spdx_license_keys': "*

 * *         "['LicenseRef-sca […]*

```diff
@@ -131,14 +131,26 @@
         "license_key": "ace-tao",
         "other_spdx_license_keys": [],
         "spdx_license_key": "DOC",
         "yaml": "ace-tao.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "acm-sla.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "acm-sla.json",
+        "license": "acm-sla.LICENSE",
+        "license_key": "acm-sla",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-acm-sla",
+        "yaml": "acm-sla.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "acroname-bdk.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "acroname-bdk.json",
         "license": "acroname-bdk.LICENSE",
         "license_key": "acroname-bdk",
         "other_spdx_license_keys": [],
@@ -197,19 +209,33 @@
         "category": "Copyleft Limited",
         "html": "ada-linking-exception.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "ada-linking-exception.json",
         "license": "ada-linking-exception.LICENSE",
         "license_key": "ada-linking-exception",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-ada-linking-exception",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-ada-linking-exception"
+        ],
+        "spdx_license_key": "GNAT-exception",
         "yaml": "ada-linking-exception.yml"
     },
     {
+        "category": "Permissive",
+        "html": "adacore-doc.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "adacore-doc.json",
+        "license": "adacore-doc.LICENSE",
+        "license_key": "adacore-doc",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "AdaCore-doc",
+        "yaml": "adacore-doc.yml"
+    },
+    {
         "category": "Copyleft",
         "html": "adapt-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "adapt-1.0.json",
         "license": "adapt-1.0.LICENSE",
         "license_key": "adapt-1.0",
@@ -765,14 +791,26 @@
         "license_key": "agpl-generic-additional-terms",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-agpl-generic-additional-terms",
         "yaml": "agpl-generic-additional-terms.yml"
     },
     {
         "category": "Permissive",
+        "html": "agtpl.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "agtpl.json",
+        "license": "agtpl.LICENSE",
+        "license_key": "agtpl",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-agtpl",
+        "yaml": "agtpl.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "aladdin-md5.html",
         "is_deprecated": true,
         "is_exception": false,
         "json": "aladdin-md5.json",
         "license": "aladdin-md5.LICENSE",
         "license_key": "aladdin-md5",
         "other_spdx_license_keys": [],
@@ -1239,15 +1277,15 @@
         "license": "apafml.LICENSE",
         "license_key": "apafml",
         "other_spdx_license_keys": [],
         "spdx_license_key": "APAFML",
         "yaml": "apafml.yml"
     },
     {
-        "category": "Copyleft Limited",
+        "category": "Proprietary Free",
         "html": "apl-1.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "apl-1.1.json",
         "license": "apl-1.1.LICENSE",
         "license_key": "apl-1.1",
         "other_spdx_license_keys": [],
@@ -1275,14 +1313,26 @@
         "license": "appfire-eula.LICENSE",
         "license_key": "appfire-eula",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-appfire-eula",
         "yaml": "appfire-eula.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "apple-academic-lisa-os-3.1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "apple-academic-lisa-os-3.1.json",
+        "license": "apple-academic-lisa-os-3.1.LICENSE",
+        "license_key": "apple-academic-lisa-os-3.1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-apple-academic-lisa-os-3.1",
+        "yaml": "apple-academic-lisa-os-3.1.yml"
+    },
+    {
         "category": "Permissive",
         "html": "apple-attribution.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "apple-attribution.json",
         "license": "apple-attribution.LICENSE",
         "license_key": "apple-attribution",
@@ -1601,14 +1651,38 @@
         "license": "artistic-perl-1.0.LICENSE",
         "license_key": "artistic-perl-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "Artistic-1.0-Perl",
         "yaml": "artistic-perl-1.0.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "ascender-eula.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ascender-eula.json",
+        "license": "ascender-eula.LICENSE",
+        "license_key": "ascender-eula",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ascender-eula",
+        "yaml": "ascender-eula.yml"
+    },
+    {
+        "category": "Commercial",
+        "html": "ascender-web-fonts.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ascender-web-fonts.json",
+        "license": "ascender-web-fonts.LICENSE",
+        "license_key": "ascender-web-fonts",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ascender-web-fonts",
+        "yaml": "ascender-web-fonts.yml"
+    },
+    {
         "category": "Free Restricted",
         "html": "aslp.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "aslp.json",
         "license": "aslp.LICENSE",
         "license_key": "aslp",
@@ -1769,14 +1843,26 @@
         "license": "attribution.LICENSE",
         "license_key": "attribution",
         "other_spdx_license_keys": [],
         "spdx_license_key": "AAL",
         "yaml": "attribution.yml"
     },
     {
+        "category": "Free Restricted",
+        "html": "authorizenet-sdk.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "authorizenet-sdk.json",
+        "license": "authorizenet-sdk.LICENSE",
+        "license_key": "authorizenet-sdk",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-authorizenet-sdk",
+        "yaml": "authorizenet-sdk.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "autoconf-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "autoconf-exception-2.0.json",
         "license": "autoconf-exception-2.0.LICENSE",
         "license_key": "autoconf-exception-2.0",
@@ -1824,16 +1910,18 @@
         "category": "Copyleft Limited",
         "html": "autoconf-simple-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "autoconf-simple-exception-2.0.json",
         "license": "autoconf-simple-exception-2.0.LICENSE",
         "license_key": "autoconf-simple-exception-2.0",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-autoconf-simple-exception-2.0",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-autoconf-simple-exception-2.0"
+        ],
+        "spdx_license_key": "Autoconf-exception-generic",
         "yaml": "autoconf-simple-exception-2.0.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "autodesk-3d-sft-3.0.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -1889,14 +1977,26 @@
         "license": "avisynth-linking-exception.LICENSE",
         "license_key": "avisynth-linking-exception",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-avisynth-linking-exception",
         "yaml": "avisynth-linking-exception.yml"
     },
     {
+        "category": "Source-available",
+        "html": "avsystem-5-clause.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "avsystem-5-clause.json",
+        "license": "avsystem-5-clause.LICENSE",
+        "license_key": "avsystem-5-clause",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-avsystem-5-clause",
+        "yaml": "avsystem-5-clause.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "bacula-exception.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "bacula-exception.json",
         "license": "bacula-exception.LICENSE",
         "license_key": "bacula-exception",
@@ -2023,14 +2123,26 @@
         "license": "beri-hw-sw-1.0.LICENSE",
         "license_key": "beri-hw-sw-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-beri-hw-sw-1.0",
         "yaml": "beri-hw-sw-1.0.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "bigcode-open-rail-m-v1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "bigcode-open-rail-m-v1.json",
+        "license": "bigcode-open-rail-m-v1.LICENSE",
+        "license_key": "bigcode-open-rail-m-v1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-bigcode-open-rail-m-v1",
+        "yaml": "bigcode-open-rail-m-v1.yml"
+    },
+    {
         "category": "Permissive",
         "html": "bigdigits.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "bigdigits.json",
         "license": "bigdigits.LICENSE",
         "license_key": "bigdigits",
@@ -2048,14 +2160,26 @@
         "license_key": "bigelow-holmes",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-bigelow-holmes",
         "yaml": "bigelow-holmes.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "bigscience-open-rail-m.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "bigscience-open-rail-m.json",
+        "license": "bigscience-open-rail-m.LICENSE",
+        "license_key": "bigscience-open-rail-m",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-bigscience-open-rail-m",
+        "yaml": "bigscience-open-rail-m.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "bigscience-rail-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "bigscience-rail-1.0.json",
         "license": "bigscience-rail-1.0.LICENSE",
         "license_key": "bigscience-rail-1.0",
         "other_spdx_license_keys": [],
@@ -2229,14 +2353,26 @@
         "license": "blas-2017.LICENSE",
         "license_key": "blas-2017",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-blas-2017",
         "yaml": "blas-2017.yml"
     },
     {
+        "category": "Copyleft",
+        "html": "blender-2010.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "blender-2010.json",
+        "license": "blender-2010.LICENSE",
+        "license_key": "blender-2010",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-blender-2010",
+        "yaml": "blender-2010.yml"
+    },
+    {
         "category": "Public Domain",
         "html": "blessing.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "blessing.json",
         "license": "blessing.LICENSE",
         "license_key": "blessing",
@@ -2447,21 +2583,23 @@
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-brian-gladman-3-clause",
         "yaml": "brian-gladman-3-clause.yml"
     },
     {
         "category": "Permissive",
         "html": "brian-gladman-dual.html",
-        "is_deprecated": true,
+        "is_deprecated": false,
         "is_exception": false,
         "json": "brian-gladman-dual.json",
         "license": "brian-gladman-dual.LICENSE",
         "license_key": "brian-gladman-dual",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": null,
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-brian-gladman-dual"
+        ],
+        "spdx_license_key": "Brian-Gladman-3-Clause",
         "yaml": "brian-gladman-dual.yml"
     },
     {
         "category": "Permissive",
         "html": "broadcom-cfe.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -2894,14 +3032,26 @@
         "license_key": "bsd-ack-carrot2",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-bsd-ack-carrot2",
         "yaml": "bsd-ack-carrot2.yml"
     },
     {
         "category": "Permissive",
+        "html": "bsd-advertising-acknowledgement.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "bsd-advertising-acknowledgement.json",
+        "license": "bsd-advertising-acknowledgement.LICENSE",
+        "license_key": "bsd-advertising-acknowledgement",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "BSD-Advertising-Acknowledgement",
+        "yaml": "bsd-advertising-acknowledgement.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "bsd-artwork.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "bsd-artwork.json",
         "license": "bsd-artwork.LICENSE",
         "license_key": "bsd-artwork",
         "other_spdx_license_keys": [],
@@ -3154,16 +3304,18 @@
         "category": "Permissive",
         "html": "bsd-original-uc-1986.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "bsd-original-uc-1986.json",
         "license": "bsd-original-uc-1986.LICENSE",
         "license_key": "bsd-original-uc-1986",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-bsd-original-uc-1986",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-bsd-original-uc-1986"
+        ],
+        "spdx_license_key": "BSD-4.3RENO",
         "yaml": "bsd-original-uc-1986.yml"
     },
     {
         "category": "Permissive",
         "html": "bsd-original-uc-1990.html",
         "is_deprecated": true,
         "is_exception": false,
@@ -3387,16 +3539,18 @@
         "category": "Permissive",
         "html": "bsla.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "bsla.json",
         "license": "bsla.LICENSE",
         "license_key": "bsla",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-bsla",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-bsla"
+        ],
+        "spdx_license_key": "BSD-4.3TAHOE",
         "yaml": "bsla.yml"
     },
     {
         "category": "Permissive",
         "html": "bsla-no-advert.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -3641,16 +3795,18 @@
         "category": "Permissive",
         "html": "carnegie-mellon-contributors.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "carnegie-mellon-contributors.json",
         "license": "carnegie-mellon-contributors.LICENSE",
         "license_key": "carnegie-mellon-contributors",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-carnegie-mellon-contributors",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-carnegie-mellon-contributors"
+        ],
+        "spdx_license_key": "CMU-Mach",
         "yaml": "carnegie-mellon-contributors.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "cavium-linux-firmware.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -4031,14 +4187,26 @@
         "license_key": "cc-by-nc-sa-2.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "CC-BY-NC-SA-2.0",
         "yaml": "cc-by-nc-sa-2.0.yml"
     },
     {
         "category": "Source-available",
+        "html": "cc-by-nc-sa-2.0-de.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "cc-by-nc-sa-2.0-de.json",
+        "license": "cc-by-nc-sa-2.0-de.LICENSE",
+        "license_key": "cc-by-nc-sa-2.0-de",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "CC-BY-NC-SA-2.0-DE",
+        "yaml": "cc-by-nc-sa-2.0-de.yml"
+    },
+    {
+        "category": "Source-available",
         "html": "cc-by-nc-sa-2.0-fr.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "cc-by-nc-sa-2.0-fr.json",
         "license": "cc-by-nc-sa-2.0-fr.LICENSE",
         "license_key": "cc-by-nc-sa-2.0-fr",
         "other_spdx_license_keys": [],
@@ -4703,14 +4871,26 @@
         "license_key": "cern-ohl-w-2.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "CERN-OHL-W-2.0",
         "yaml": "cern-ohl-w-2.0.yml"
     },
     {
         "category": "Permissive",
+        "html": "cfitsio.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "cfitsio.json",
+        "license": "cfitsio.LICENSE",
+        "license_key": "cfitsio",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "CFITSIO",
+        "yaml": "cfitsio.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "cgic.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "cgic.json",
         "license": "cgic.LICENSE",
         "license_key": "cgic",
         "other_spdx_license_keys": [],
@@ -4889,16 +5069,18 @@
         "category": "Permissive",
         "html": "clips-2017.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "clips-2017.json",
         "license": "clips-2017.LICENSE",
         "license_key": "clips-2017",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-clips-2017",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-clips-2017"
+        ],
+        "spdx_license_key": "Clips",
         "yaml": "clips-2017.yml"
     },
     {
         "category": "Copyleft Limited",
         "html": "clisp-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
@@ -4949,16 +5131,18 @@
         "category": "Permissive",
         "html": "cmu-computing-services.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "cmu-computing-services.json",
         "license": "cmu-computing-services.LICENSE",
         "license_key": "cmu-computing-services",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-cmu-computing-services",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-cmu-computing-services"
+        ],
+        "spdx_license_key": "BSD-Attribution-HPND-disclaimer",
         "yaml": "cmu-computing-services.yml"
     },
     {
         "category": "Permissive",
         "html": "cmu-mit.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -5089,26 +5273,50 @@
             "LicenseRef-scancode-cockroachdb-use-grant-for-bsl-1.1"
         ],
         "spdx_license_key": "LicenseRef-scancode-cockroachdb-use-grant-bsl-1.1",
         "yaml": "cockroachdb-use-grant-for-bsl-1.1.yml"
     },
     {
         "category": "Permissive",
+        "html": "code-credit-license-1.0-0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "code-credit-license-1.0-0.json",
+        "license": "code-credit-license-1.0-0.LICENSE",
+        "license_key": "code-credit-license-1.0-0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-code-credit-license-1.0.0",
+        "yaml": "code-credit-license-1.0-0.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "code-credit-license-1.0.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "code-credit-license-1.0.1.json",
         "license": "code-credit-license-1.0.1.LICENSE",
         "license_key": "code-credit-license-1.0.1",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-code-credit-license-1.0.1",
         "yaml": "code-credit-license-1.0.1.yml"
     },
     {
         "category": "Permissive",
+        "html": "code-credit-license-1.1.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "code-credit-license-1.1.0.json",
+        "license": "code-credit-license-1.1.0.LICENSE",
+        "license_key": "code-credit-license-1.1.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-code-credit-license-1.1.0",
+        "yaml": "code-credit-license-1.1.0.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "codeguru-permissions.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "codeguru-permissions.json",
         "license": "codeguru-permissions.LICENSE",
         "license_key": "codeguru-permissions",
         "other_spdx_license_keys": [],
@@ -5316,14 +5524,38 @@
         "license": "cooperative-non-violent-4.0.LICENSE",
         "license_key": "cooperative-non-violent-4.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-cooperative-non-violent-4.0",
         "yaml": "cooperative-non-violent-4.0.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "cooperative-non-violent-6.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "cooperative-non-violent-6.0.json",
+        "license": "cooperative-non-violent-6.0.LICENSE",
+        "license_key": "cooperative-non-violent-6.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-cooperative-non-violent-6.0",
+        "yaml": "cooperative-non-violent-6.0.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "cooperative-non-violent-7.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "cooperative-non-violent-7.0.json",
+        "license": "cooperative-non-violent-7.0.LICENSE",
+        "license_key": "cooperative-non-violent-7.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-cooperative-non-violent-7.0",
+        "yaml": "cooperative-non-violent-7.0.yml"
+    },
+    {
         "category": "Public Domain",
         "html": "copyheart.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "copyheart.json",
         "license": "copyheart.LICENSE",
         "license_key": "copyheart",
@@ -5352,14 +5584,26 @@
         "license": "copyleft-next-0.3.1.LICENSE",
         "license_key": "copyleft-next-0.3.1",
         "other_spdx_license_keys": [],
         "spdx_license_key": "copyleft-next-0.3.1",
         "yaml": "copyleft-next-0.3.1.yml"
     },
     {
+        "category": "Permissive",
+        "html": "cornell-lossless-jpeg.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "cornell-lossless-jpeg.json",
+        "license": "cornell-lossless-jpeg.LICENSE",
+        "license_key": "cornell-lossless-jpeg",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "Cornell-Lossless-JPEG",
+        "yaml": "cornell-lossless-jpeg.yml"
+    },
+    {
         "category": "Proprietary Free",
         "html": "corporate-accountability-1.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "corporate-accountability-1.1.json",
         "license": "corporate-accountability-1.1.LICENSE",
         "license_key": "corporate-accountability-1.1",
@@ -5932,14 +6176,38 @@
         "license": "dbcl-1.0.LICENSE",
         "license_key": "dbcl-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-dbcl-1.0",
         "yaml": "dbcl-1.0.yml"
     },
     {
+        "category": "Copyleft Limited",
+        "html": "dbmx-foss-exception-1.0.9.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "dbmx-foss-exception-1.0.9.json",
+        "license": "dbmx-foss-exception-1.0.9.LICENSE",
+        "license_key": "dbmx-foss-exception-1.0.9",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-dbmx-foss-exception-1.0.9",
+        "yaml": "dbmx-foss-exception-1.0.9.yml"
+    },
+    {
+        "category": "Copyleft Limited",
+        "html": "dbmx-linking-exception-1.0.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "dbmx-linking-exception-1.0.json",
+        "license": "dbmx-linking-exception-1.0.LICENSE",
+        "license_key": "dbmx-linking-exception-1.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-dbmx-linking-exception-1.0",
+        "yaml": "dbmx-linking-exception-1.0.yml"
+    },
+    {
         "category": "CLA",
         "html": "dco-1.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "dco-1.1.json",
         "license": "dco-1.1.LICENSE",
         "license_key": "dco-1.1",
@@ -6331,14 +6599,26 @@
         "license_key": "drl-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "DRL-1.0",
         "yaml": "drl-1.0.yml"
     },
     {
         "category": "Permissive",
+        "html": "drl-1.1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "drl-1.1.json",
+        "license": "drl-1.1.LICENSE",
+        "license_key": "drl-1.1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-drl-1.1",
+        "yaml": "drl-1.1.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "dropbear.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "dropbear.json",
         "license": "dropbear.LICENSE",
         "license_key": "dropbear",
         "other_spdx_license_keys": [],
@@ -6920,14 +7200,50 @@
         "license": "ellis-lab.LICENSE",
         "license_key": "ellis-lab",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ellis-lab",
         "yaml": "ellis-lab.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "embedthis-evaluation.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "embedthis-evaluation.json",
+        "license": "embedthis-evaluation.LICENSE",
+        "license_key": "embedthis-evaluation",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-embedthis-evaluation",
+        "yaml": "embedthis-evaluation.yml"
+    },
+    {
+        "category": "Free Restricted",
+        "html": "embedthis-extension.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "embedthis-extension.json",
+        "license": "embedthis-extension.LICENSE",
+        "license_key": "embedthis-extension",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-embedthis-extension",
+        "yaml": "embedthis-extension.yml"
+    },
+    {
+        "category": "Commercial",
+        "html": "embedthis-tou-2022.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "embedthis-tou-2022.json",
+        "license": "embedthis-tou-2022.LICENSE",
+        "license_key": "embedthis-tou-2022",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-embedthis-tou-2022",
+        "yaml": "embedthis-tou-2022.yml"
+    },
+    {
         "category": "Permissive",
         "html": "emit.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "emit.json",
         "license": "emit.LICENSE",
         "license_key": "emit",
@@ -7822,15 +8138,17 @@
         "category": "Permissive",
         "html": "fsf-unlimited-no-warranty.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "fsf-unlimited-no-warranty.json",
         "license": "fsf-unlimited-no-warranty.LICENSE",
         "license_key": "fsf-unlimited-no-warranty",
-        "other_spdx_license_keys": [],
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-fsf-unlimited-no-warranty"
+        ],
         "spdx_license_key": "FSFULLRWD",
         "yaml": "fsf-unlimited-no-warranty.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "ftdi.html",
         "is_deprecated": false,
@@ -7852,14 +8170,26 @@
         "license_key": "ftpbean",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ftpbean",
         "yaml": "ftpbean.yml"
     },
     {
         "category": "Permissive",
+        "html": "fujion-exception-to-apache-2.0.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "fujion-exception-to-apache-2.0.json",
+        "license": "fujion-exception-to-apache-2.0.LICENSE",
+        "license_key": "fujion-exception-to-apache-2.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-fujion-exception-to-apache-2.0",
+        "yaml": "fujion-exception-to-apache-2.0.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "gareth-mccaughan.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "gareth-mccaughan.json",
         "license": "gareth-mccaughan.LICENSE",
         "license_key": "gareth-mccaughan",
         "other_spdx_license_keys": [],
@@ -7875,14 +8205,26 @@
         "license": "gary-s-brown.LICENSE",
         "license_key": "gary-s-brown",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-gary-s-brown",
         "yaml": "gary-s-brown.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "gatling-highcharts.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gatling-highcharts.json",
+        "license": "gatling-highcharts.LICENSE",
+        "license_key": "gatling-highcharts",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gatling-highcharts",
+        "yaml": "gatling-highcharts.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "gcc-compiler-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "gcc-compiler-exception-2.0.json",
         "license": "gcc-compiler-exception-2.0.LICENSE",
         "license_key": "gcc-compiler-exception-2.0",
@@ -7995,14 +8337,26 @@
         "license": "generic-export-compliance.LICENSE",
         "license_key": "generic-export-compliance",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-generic-export-compliance",
         "yaml": "generic-export-compliance.yml"
     },
     {
+        "category": "Permissive",
+        "html": "generic-loop.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "generic-loop.json",
+        "license": "generic-loop.LICENSE",
+        "license_key": "generic-loop",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-generic-loop",
+        "yaml": "generic-loop.yml"
+    },
+    {
         "category": "Unstated License",
         "html": "generic-tos.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "generic-tos.json",
         "license": "generic-tos.LICENSE",
         "license_key": "generic-tos",
@@ -9685,23 +10039,49 @@
         "license": "gplcc-1.0.LICENSE",
         "license_key": "gplcc-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "GPL-CC-1.0",
         "yaml": "gplcc-1.0.yml"
     },
     {
+        "category": "Commercial",
+        "html": "gradle-enterprise-sla-2022-11-08.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gradle-enterprise-sla-2022-11-08.json",
+        "license": "gradle-enterprise-sla-2022-11-08.LICENSE",
+        "license_key": "gradle-enterprise-sla-2022-11-08",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gradle-enterprise-sla-2022-11-",
+        "yaml": "gradle-enterprise-sla-2022-11-08.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "gradle-tou-2022-01-13.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gradle-tou-2022-01-13.json",
+        "license": "gradle-tou-2022-01-13.LICENSE",
+        "license_key": "gradle-tou-2022-01-13",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gradle-tou-2022-01-13",
+        "yaml": "gradle-tou-2022-01-13.yml"
+    },
+    {
         "category": "Permissive",
         "html": "graphics-gems.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "graphics-gems.json",
         "license": "graphics-gems.LICENSE",
         "license_key": "graphics-gems",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-graphics-gems",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-graphics-gems"
+        ],
+        "spdx_license_key": "Graphics-Gems",
         "yaml": "graphics-gems.yml"
     },
     {
         "category": "Permissive",
         "html": "greg-roelofs.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -9781,14 +10161,50 @@
         "license": "gstreamer-exception-2008.LICENSE",
         "license_key": "gstreamer-exception-2008",
         "other_spdx_license_keys": [],
         "spdx_license_key": "GStreamer-exception-2008",
         "yaml": "gstreamer-exception-2008.yml"
     },
     {
+        "category": "Permissive",
+        "html": "gtpl-v1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gtpl-v1.json",
+        "license": "gtpl-v1.LICENSE",
+        "license_key": "gtpl-v1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gtpl-v1",
+        "yaml": "gtpl-v1.yml"
+    },
+    {
+        "category": "Permissive",
+        "html": "gtpl-v2.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gtpl-v2.json",
+        "license": "gtpl-v2.LICENSE",
+        "license_key": "gtpl-v2",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gtpl-v2",
+        "yaml": "gtpl-v2.yml"
+    },
+    {
+        "category": "Permissive",
+        "html": "gtpl-v3.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "gtpl-v3.json",
+        "license": "gtpl-v3.LICENSE",
+        "license_key": "gtpl-v3",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-gtpl-v3",
+        "yaml": "gtpl-v3.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "guile-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "guile-exception-2.0.json",
         "license": "guile-exception-2.0.LICENSE",
         "license_key": "guile-exception-2.0",
@@ -9842,14 +10258,26 @@
         "license_key": "h2-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-h2-1.0",
         "yaml": "h2-1.0.yml"
     },
     {
         "category": "Copyleft",
+        "html": "hacking-license.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "hacking-license.json",
+        "license": "hacking-license.LICENSE",
+        "license_key": "hacking-license",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-hacking-license",
+        "yaml": "hacking-license.yml"
+    },
+    {
+        "category": "Copyleft",
         "html": "hacos-1.2.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "hacos-1.2.json",
         "license": "hacos-1.2.LICENSE",
         "license_key": "hacos-1.2",
         "other_spdx_license_keys": [],
@@ -10263,14 +10691,38 @@
         "license": "hp-ux-jre.LICENSE",
         "license_key": "hp-ux-jre",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-hp-ux-jre",
         "yaml": "hp-ux-jre.yml"
     },
     {
+        "category": "Free Restricted",
+        "html": "hpnd-export-us.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "hpnd-export-us.json",
+        "license": "hpnd-export-us.LICENSE",
+        "license_key": "hpnd-export-us",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "HPND-export-US",
+        "yaml": "hpnd-export-us.yml"
+    },
+    {
+        "category": "Permissive",
+        "html": "hpnd-sell-variant-mit-disclaimer.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "hpnd-sell-variant-mit-disclaimer.json",
+        "license": "hpnd-sell-variant-mit-disclaimer.LICENSE",
+        "license_key": "hpnd-sell-variant-mit-disclaimer",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "HPND-sell-variant-MIT-disclaimer",
+        "yaml": "hpnd-sell-variant-mit-disclaimer.yml"
+    },
+    {
         "category": "Permissive",
         "html": "hs-regexp.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "hs-regexp.json",
         "license": "hs-regexp.LICENSE",
         "license_key": "hs-regexp",
@@ -10590,14 +11042,26 @@
         "license_key": "idt-notice",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-idt-notice",
         "yaml": "idt-notice.yml"
     },
     {
         "category": "Permissive",
+        "html": "iec-code-components-eula.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "iec-code-components-eula.json",
+        "license": "iec-code-components-eula.LICENSE",
+        "license_key": "iec-code-components-eula",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "IEC-Code-Components-EULA",
+        "yaml": "iec-code-components-eula.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "ietf.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ietf.json",
         "license": "ietf.LICENSE",
         "license_key": "ietf",
         "other_spdx_license_keys": [],
@@ -10626,14 +11090,26 @@
         "license_key": "ijg",
         "other_spdx_license_keys": [],
         "spdx_license_key": "IJG",
         "yaml": "ijg.yml"
     },
     {
         "category": "Permissive",
+        "html": "ijg-short.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ijg-short.json",
+        "license": "ijg-short.LICENSE",
+        "license_key": "ijg-short",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "IJG-short",
+        "yaml": "ijg-short.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "ilmid.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ilmid.json",
         "license": "ilmid.LICENSE",
         "license_key": "ilmid",
         "other_spdx_license_keys": [],
@@ -10886,16 +11362,18 @@
         "category": "Copyleft Limited",
         "html": "inria-linking-exception.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "inria-linking-exception.json",
         "license": "inria-linking-exception.LICENSE",
         "license_key": "inria-linking-exception",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-inria-linking-exception",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-inria-linking-exception"
+        ],
+        "spdx_license_key": "QPL-1.0-INRIA-2004-exception",
         "yaml": "inria-linking-exception.yml"
     },
     {
         "category": "Free Restricted",
         "html": "installsite.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -11639,14 +12117,26 @@
         "license": "josl-1.0.LICENSE",
         "license_key": "josl-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-josl-1.0",
         "yaml": "josl-1.0.yml"
     },
     {
+        "category": "Source-available",
+        "html": "jpl-image.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "jpl-image.json",
+        "license": "jpl-image.LICENSE",
+        "license_key": "jpl-image",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "JPL-image",
+        "yaml": "jpl-image.yml"
+    },
+    {
         "category": "Permissive",
         "html": "jpnic-idnkit.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "jpnic-idnkit.json",
         "license": "jpnic-idnkit.LICENSE",
         "license_key": "jpnic-idnkit",
@@ -11843,14 +12333,38 @@
         "license": "katharos-0.1.0.LICENSE",
         "license_key": "katharos-0.1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-katharos-0.1.0",
         "yaml": "katharos-0.1.0.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "katharos-0.2.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "katharos-0.2.0.json",
+        "license": "katharos-0.2.0.LICENSE",
+        "license_key": "katharos-0.2.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-katharos-0.2.0",
+        "yaml": "katharos-0.2.0.yml"
+    },
+    {
+        "category": "Permissive",
+        "html": "kazlib.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "kazlib.json",
+        "license": "kazlib.LICENSE",
+        "license_key": "kazlib",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "Kazlib",
+        "yaml": "kazlib.yml"
+    },
+    {
         "category": "Copyleft",
         "html": "kde-accepted-gpl.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "kde-accepted-gpl.json",
         "license": "kde-accepted-gpl.LICENSE",
         "license_key": "kde-accepted-gpl",
@@ -11919,14 +12433,26 @@
         "license": "kevlin-henney.LICENSE",
         "license_key": "kevlin-henney",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-kevlin-henney",
         "yaml": "kevlin-henney.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "kfgqpc-uthmanic-script-hafs.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "kfgqpc-uthmanic-script-hafs.json",
+        "license": "kfgqpc-uthmanic-script-hafs.LICENSE",
+        "license_key": "kfgqpc-uthmanic-script-hafs",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-kfgqpc-uthmanic-script-hafs",
+        "yaml": "kfgqpc-uthmanic-script-hafs.yml"
+    },
+    {
         "category": "Copyleft",
         "html": "kfqf-accepted-gpl.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "kfqf-accepted-gpl.json",
         "license": "kfqf-accepted-gpl.LICENSE",
         "license_key": "kfqf-accepted-gpl",
@@ -12611,16 +13137,18 @@
         "category": "Permissive",
         "html": "libpbm.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "libpbm.json",
         "license": "libpbm.LICENSE",
         "license_key": "libpbm",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-libpbm",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-libpbm"
+        ],
+        "spdx_license_key": "xlock",
         "yaml": "libpbm.yml"
     },
     {
         "category": "Permissive",
         "html": "libpng.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -12748,14 +13276,38 @@
         "license": "license-file-reference.LICENSE",
         "license_key": "license-file-reference",
         "other_spdx_license_keys": [],
         "spdx_license_key": null,
         "yaml": "license-file-reference.yml"
     },
     {
+        "category": "Commercial",
+        "html": "liferay-ee.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "liferay-ee.json",
+        "license": "liferay-ee.LICENSE",
+        "license_key": "liferay-ee",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-liferay-ee",
+        "yaml": "liferay-ee.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "liferay-marketplace-tos.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "liferay-marketplace-tos.json",
+        "license": "liferay-marketplace-tos.LICENSE",
+        "license_key": "liferay-marketplace-tos",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-liferay-marketplace-tos",
+        "yaml": "liferay-marketplace-tos.yml"
+    },
+    {
         "category": "Permissive",
         "html": "lil-1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "lil-1.json",
         "license": "lil-1.LICENSE",
         "license_key": "lil-1",
@@ -12954,14 +13506,26 @@
         "license": "linuxhowtos.LICENSE",
         "license_key": "linuxhowtos",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-linuxhowtos",
         "yaml": "linuxhowtos.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "llama-license-2023.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "llama-license-2023.json",
+        "license": "llama-license-2023.LICENSE",
+        "license_key": "llama-license-2023",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-llama-license-2023",
+        "yaml": "llama-license-2023.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "llgpl.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "llgpl.json",
         "license": "llgpl.LICENSE",
         "license_key": "llgpl",
@@ -13026,14 +13590,26 @@
         "license": "lontium-linux-firmware.LICENSE",
         "license_key": "lontium-linux-firmware",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-lontium-linux-firmware",
         "yaml": "lontium-linux-firmware.yml"
     },
     {
+        "category": "Permissive",
+        "html": "loop.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "loop.json",
+        "license": "loop.LICENSE",
+        "license_key": "loop",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LOOP",
+        "yaml": "loop.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "losla.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "losla.json",
         "license": "losla.LICENSE",
         "license_key": "losla",
@@ -13395,28 +13971,32 @@
         "category": "Permissive",
         "html": "markus-kuhn-license.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "markus-kuhn-license.json",
         "license": "markus-kuhn-license.LICENSE",
         "license_key": "markus-kuhn-license",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-markus-kuhn-license",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-markus-kuhn-license"
+        ],
+        "spdx_license_key": "HPND-Markus-Kuhn",
         "yaml": "markus-kuhn-license.yml"
     },
     {
         "category": "Permissive",
         "html": "martin-birgmeier.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "martin-birgmeier.json",
         "license": "martin-birgmeier.LICENSE",
         "license_key": "martin-birgmeier",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-martin-birgmeier",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-martin-birgmeier"
+        ],
+        "spdx_license_key": "Martin-Birgmeier",
         "yaml": "martin-birgmeier.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "marvell-firmware.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -13545,14 +14125,50 @@
         "license_key": "mediainfo-lib",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-mediainfo-lib",
         "yaml": "mediainfo-lib.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "mediatek-firmware.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mediatek-firmware.json",
+        "license": "mediatek-firmware.LICENSE",
+        "license_key": "mediatek-firmware",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mediatek-firmware",
+        "yaml": "mediatek-firmware.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "mediatek-no-warranty.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mediatek-no-warranty.json",
+        "license": "mediatek-no-warranty.LICENSE",
+        "license_key": "mediatek-no-warranty",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mediatek-no-warranty",
+        "yaml": "mediatek-no-warranty.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "mediatek-proprietary-2008.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mediatek-proprietary-2008.json",
+        "license": "mediatek-proprietary-2008.LICENSE",
+        "license_key": "mediatek-proprietary-2008",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mediatek-proprietary-2008",
+        "yaml": "mediatek-proprietary-2008.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "melange.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "melange.json",
         "license": "melange.LICENSE",
         "license_key": "melange",
         "other_spdx_license_keys": [],
@@ -13833,16 +14449,18 @@
         "category": "Permissive",
         "html": "mit-addition.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "mit-addition.json",
         "license": "mit-addition.LICENSE",
         "license_key": "mit-addition",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-mit-addition",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-mit-addition"
+        ],
+        "spdx_license_key": "MIT-Wu",
         "yaml": "mit-addition.yml"
     },
     {
         "category": "Permissive",
         "html": "mit-export-control.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -13850,14 +14468,26 @@
         "license": "mit-export-control.LICENSE",
         "license_key": "mit-export-control",
         "other_spdx_license_keys": [],
         "spdx_license_key": "Xerox",
         "yaml": "mit-export-control.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "mit-kyle-restrictions.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mit-kyle-restrictions.json",
+        "license": "mit-kyle-restrictions.LICENSE",
+        "license_key": "mit-kyle-restrictions",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mit-kyle-restrictions",
+        "yaml": "mit-kyle-restrictions.yml"
+    },
+    {
         "category": "Permissive",
         "html": "mit-license-1998.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "mit-license-1998.json",
         "license": "mit-license-1998.LICENSE",
         "license_key": "mit-license-1998",
@@ -14253,24 +14883,36 @@
         "spdx_license_key": "MPL-2.0",
         "yaml": "mpl-2.0.yml"
     },
     {
         "category": "Copyleft Limited",
         "html": "mpl-2.0-no-copyleft-exception.html",
         "is_deprecated": false,
-        "is_exception": false,
+        "is_exception": true,
         "json": "mpl-2.0-no-copyleft-exception.json",
         "license": "mpl-2.0-no-copyleft-exception.LICENSE",
         "license_key": "mpl-2.0-no-copyleft-exception",
         "other_spdx_license_keys": [],
         "spdx_license_key": "MPL-2.0-no-copyleft-exception",
         "yaml": "mpl-2.0-no-copyleft-exception.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "ms-api-code-pack-net.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ms-api-code-pack-net.json",
+        "license": "ms-api-code-pack-net.LICENSE",
+        "license_key": "ms-api-code-pack-net",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ms-api-code-pack-net",
+        "yaml": "ms-api-code-pack-net.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "ms-asp-net-ajax-supplemental-terms.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-asp-net-ajax-supplemental-terms.json",
         "license": "ms-asp-net-ajax-supplemental-terms.LICENSE",
         "license_key": "ms-asp-net-ajax-supplemental-terms",
         "other_spdx_license_keys": [
@@ -14422,15 +15064,15 @@
         "license": "ms-cl.LICENSE",
         "license_key": "ms-cl",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ms-cl",
         "yaml": "ms-cl.yml"
     },
     {
-        "category": "Patent License",
+        "category": "CLA",
         "html": "ms-cla.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-cla.json",
         "license": "ms-cla.LICENSE",
         "license_key": "ms-cla",
         "other_spdx_license_keys": [],
@@ -14523,26 +15165,50 @@
         "license_key": "ms-directx-sdk-eula",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ms-directx-sdk-eula",
         "yaml": "ms-directx-sdk-eula.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "ms-directx-sdk-eula-2020.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ms-directx-sdk-eula-2020.json",
+        "license": "ms-directx-sdk-eula-2020.LICENSE",
+        "license_key": "ms-directx-sdk-eula-2020",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ms-directx-sdk-eula-2020",
+        "yaml": "ms-directx-sdk-eula-2020.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "ms-dxsdk-d3dx-9.29.952.3.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-dxsdk-d3dx-9.29.952.3.json",
         "license": "ms-dxsdk-d3dx-9.29.952.3.LICENSE",
         "license_key": "ms-dxsdk-d3dx-9.29.952.3",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ms-dxsdk-d3dx-9.29.952.3",
         "yaml": "ms-dxsdk-d3dx-9.29.952.3.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "ms-edge-webview2-fixed.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ms-edge-webview2-fixed.json",
+        "license": "ms-edge-webview2-fixed.LICENSE",
+        "license_key": "ms-edge-webview2-fixed",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ms-edge-webview2-fixed",
+        "yaml": "ms-edge-webview2-fixed.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "ms-entity-framework-4.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-entity-framework-4.1.json",
         "license": "ms-entity-framework-4.1.LICENSE",
         "license_key": "ms-entity-framework-4.1",
         "other_spdx_license_keys": [],
@@ -14927,14 +15593,26 @@
         "license_key": "ms-platform-sdk",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ms-platform-sdk",
         "yaml": "ms-platform-sdk.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "ms-pre-release-sla-2023.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ms-pre-release-sla-2023.json",
+        "license": "ms-pre-release-sla-2023.LICENSE",
+        "license_key": "ms-pre-release-sla-2023",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ms-pre-release-sla-2023",
+        "yaml": "ms-pre-release-sla-2023.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "ms-programsynthesis-7.22.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-programsynthesis-7.22.0.json",
         "license": "ms-programsynthesis-7.22.0.LICENSE",
         "license_key": "ms-programsynthesis-7.22.0",
         "other_spdx_license_keys": [],
@@ -15034,14 +15712,26 @@
         "license": "ms-silverlight-3.LICENSE",
         "license_key": "ms-silverlight-3",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ms-silverlight-3",
         "yaml": "ms-silverlight-3.yml"
     },
     {
+        "category": "Free Restricted",
+        "html": "ms-specification.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ms-specification.json",
+        "license": "ms-specification.LICENSE",
+        "license_key": "ms-specification",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-ms-specification",
+        "yaml": "ms-specification.yml"
+    },
+    {
         "category": "Proprietary Free",
         "html": "ms-sql-server-compact-4.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ms-sql-server-compact-4.0.json",
         "license": "ms-sql-server-compact-4.0.LICENSE",
         "license_key": "ms-sql-server-compact-4.0",
@@ -15506,14 +16196,38 @@
         "license": "mulanpsl-2.0-en.LICENSE",
         "license_key": "mulanpsl-2.0-en",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-mulanpsl-2.0-en",
         "yaml": "mulanpsl-2.0-en.yml"
     },
     {
+        "category": "Copyleft",
+        "html": "mulanpubl-1.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mulanpubl-1.0.json",
+        "license": "mulanpubl-1.0.LICENSE",
+        "license_key": "mulanpubl-1.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mulanpubl-1.0",
+        "yaml": "mulanpubl-1.0.yml"
+    },
+    {
+        "category": "Copyleft",
+        "html": "mulanpubl-2.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mulanpubl-2.0.json",
+        "license": "mulanpubl-2.0.LICENSE",
+        "license_key": "mulanpubl-2.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mulanpubl-2.0",
+        "yaml": "mulanpubl-2.0.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "mule-source-1.1.3.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "mule-source-1.1.3.json",
         "license": "mule-source-1.1.3.LICENSE",
         "license_key": "mule-source-1.1.3",
@@ -15578,14 +16292,26 @@
         "license": "musl-exception.LICENSE",
         "license_key": "musl-exception",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-musl-exception",
         "yaml": "musl-exception.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "mut-license.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "mut-license.json",
+        "license": "mut-license.LICENSE",
+        "license_key": "mut-license",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-mut-license",
+        "yaml": "mut-license.yml"
+    },
+    {
         "category": "Free Restricted",
         "html": "mvt-1.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "mvt-1.1.json",
         "license": "mvt-1.1.LICENSE",
         "license_key": "mvt-1.1",
@@ -16136,14 +16862,26 @@
         "license": "non-violent-4.0.LICENSE",
         "license_key": "non-violent-4.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-non-violent-4.0",
         "yaml": "non-violent-4.0.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "non-violent-7.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "non-violent-7.0.json",
+        "license": "non-violent-7.0.LICENSE",
+        "license_key": "non-violent-7.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-non-violent-7.0",
+        "yaml": "non-violent-7.0.yml"
+    },
+    {
         "category": "Permissive",
         "html": "nonexclusive.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "nonexclusive.json",
         "license": "nonexclusive.LICENSE",
         "license_key": "nonexclusive",
@@ -16352,14 +17090,26 @@
         "license": "ntpl-origin.LICENSE",
         "license_key": "ntpl-origin",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ntpl-origin",
         "yaml": "ntpl-origin.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "nucleusicons-eula.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "nucleusicons-eula.json",
+        "license": "nucleusicons-eula.LICENSE",
+        "license_key": "nucleusicons-eula",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-nucleusicons-eula",
+        "yaml": "nucleusicons-eula.yml"
+    },
+    {
         "category": "Commercial",
         "html": "numerical-recipes-notice.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "numerical-recipes-notice.json",
         "license": "numerical-recipes-notice.LICENSE",
         "license_key": "numerical-recipes-notice",
@@ -16642,14 +17392,26 @@
         "license": "oasis-ws-security-spec.LICENSE",
         "license_key": "oasis-ws-security-spec",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-oasis-ws-security-spec",
         "yaml": "oasis-ws-security-spec.yml"
     },
     {
+        "category": "Permissive",
+        "html": "object-form-exception-to-mit.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "object-form-exception-to-mit.json",
+        "license": "object-form-exception-to-mit.LICENSE",
+        "license_key": "object-form-exception-to-mit",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-object-form-exception-to-mit",
+        "yaml": "object-form-exception-to-mit.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "ocaml-lgpl-linking-exception.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "ocaml-lgpl-linking-exception.json",
         "license": "ocaml-lgpl-linking-exception.LICENSE",
         "license_key": "ocaml-lgpl-linking-exception",
@@ -16849,14 +17611,26 @@
         "license_key": "odmg",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-odmg",
         "yaml": "odmg.yml"
     },
     {
         "category": "Permissive",
+        "html": "offis.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "offis.json",
+        "license": "offis.LICENSE",
+        "license_key": "offis",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "OFFIS",
+        "yaml": "offis.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "ofl-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ofl-1.0.json",
         "license": "ofl-1.0.LICENSE",
         "license_key": "ofl-1.0",
         "other_spdx_license_keys": [],
@@ -17112,15 +17886,15 @@
         "license": "oll-1.0.LICENSE",
         "license_key": "oll-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-oll-1.0",
         "yaml": "oll-1.0.yml"
     },
     {
-        "category": "Permissive",
+        "category": "Proprietary Free",
         "html": "ooura-2001.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ooura-2001.json",
         "license": "ooura-2001.LICENSE",
         "license_key": "ooura-2001",
         "other_spdx_license_keys": [],
@@ -17160,14 +17934,26 @@
         "license": "open-public.LICENSE",
         "license_key": "open-public",
         "other_spdx_license_keys": [],
         "spdx_license_key": "OPL-1.0",
         "yaml": "open-public.yml"
     },
     {
+        "category": "Commercial",
+        "html": "openai-tou-20230314.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "openai-tou-20230314.json",
+        "license": "openai-tou-20230314.LICENSE",
+        "license_key": "openai-tou-20230314",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-openai-tou-20230314",
+        "yaml": "openai-tou-20230314.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "openbd-exception-3.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "openbd-exception-3.0.json",
         "license": "openbd-exception-3.0.LICENSE",
         "license_key": "openbd-exception-3.0",
@@ -17464,14 +18250,26 @@
         "license": "openmotif-exception-2.0-plus.LICENSE",
         "license_key": "openmotif-exception-2.0-plus",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-openmotif-exception-2.0-plus",
         "yaml": "openmotif-exception-2.0-plus.yml"
     },
     {
+        "category": "Copyleft Limited",
+        "html": "openmrs-exception-to-mpl-2.0.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "openmrs-exception-to-mpl-2.0.json",
+        "license": "openmrs-exception-to-mpl-2.0.LICENSE",
+        "license_key": "openmrs-exception-to-mpl-2.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-openmrs-exception-to-mpl-2.0",
+        "yaml": "openmrs-exception-to-mpl-2.0.yml"
+    },
+    {
         "category": "Proprietary Free",
         "html": "opennetcf-shared-source.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "opennetcf-shared-source.json",
         "license": "opennetcf-shared-source.LICENSE",
         "license_key": "opennetcf-shared-source",
@@ -17495,16 +18293,18 @@
         "category": "Copyleft Limited",
         "html": "openpbs-2.3.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "openpbs-2.3.json",
         "license": "openpbs-2.3.LICENSE",
         "license_key": "openpbs-2.3",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-openpbs-2.3",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-openpbs-2.3"
+        ],
+        "spdx_license_key": "OpenPBS-2.3",
         "yaml": "openpbs-2.3.yml"
     },
     {
         "category": "Permissive",
         "html": "openpub.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -17611,15 +18411,17 @@
         "category": "Copyleft",
         "html": "openssl-exception-gpl-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "openssl-exception-gpl-2.0.json",
         "license": "openssl-exception-gpl-2.0.LICENSE",
         "license_key": "openssl-exception-gpl-2.0",
-        "other_spdx_license_keys": [],
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-openssl-exception-gpl-2.0"
+        ],
         "spdx_license_key": "x11vnc-openssl-exception",
         "yaml": "openssl-exception-gpl-2.0.yml"
     },
     {
         "category": "Copyleft",
         "html": "openssl-exception-gpl-2.0-plus.html",
         "is_deprecated": false,
@@ -18105,16 +18907,18 @@
         "category": "Permissive",
         "html": "osf-1990.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "osf-1990.json",
         "license": "osf-1990.LICENSE",
         "license_key": "osf-1990",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-osf-1990",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-osf-1990"
+        ],
+        "spdx_license_key": "HP-1986",
         "yaml": "osf-1990.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "osgi-spec-2.0.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -19062,14 +19866,26 @@
         "license": "ppp.LICENSE",
         "license_key": "ppp",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ppp",
         "yaml": "ppp.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "proconx-modbus-rev4.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "proconx-modbus-rev4.json",
+        "license": "proconx-modbus-rev4.LICENSE",
+        "license_key": "proconx-modbus-rev4",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-proconX-modbus-rev4",
+        "yaml": "proconx-modbus-rev4.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "proguard-exception-2.0.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "proguard-exception-2.0.json",
         "license": "proguard-exception-2.0.LICENSE",
         "license_key": "proguard-exception-2.0",
@@ -19427,14 +20243,26 @@
         "license": "qpl-1.0.LICENSE",
         "license_key": "qpl-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "QPL-1.0",
         "yaml": "qpl-1.0.yml"
     },
     {
+        "category": "Copyleft Limited",
+        "html": "qpl-1.0-inria-2004.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "qpl-1.0-inria-2004.json",
+        "license": "qpl-1.0-inria-2004.LICENSE",
+        "license_key": "qpl-1.0-inria-2004",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "QPL-1.0-INRIA-2004",
+        "yaml": "qpl-1.0-inria-2004.yml"
+    },
+    {
         "category": "Permissive",
         "html": "qpopper.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "qpopper.json",
         "license": "qpopper.LICENSE",
         "license_key": "qpopper",
@@ -19937,14 +20765,26 @@
         "license": "robert-hubley.LICENSE",
         "license_key": "robert-hubley",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-robert-hubley",
         "yaml": "robert-hubley.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "rockchip-proprietary-2022.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "rockchip-proprietary-2022.json",
+        "license": "rockchip-proprietary-2022.LICENSE",
+        "license_key": "rockchip-proprietary-2022",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-rockchip-proprietary-2022",
+        "yaml": "rockchip-proprietary-2022.yml"
+    },
+    {
         "category": "Commercial",
         "html": "rogue-wave.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "rogue-wave.json",
         "license": "rogue-wave.LICENSE",
         "license_key": "rogue-wave",
@@ -20515,14 +21355,26 @@
         "license": "selinux-nsa-declaration-1.0.LICENSE",
         "license_key": "selinux-nsa-declaration-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "libselinux-1.0",
         "yaml": "selinux-nsa-declaration-1.0.yml"
     },
     {
+        "category": "Source-available",
+        "html": "semgrep-registry.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "semgrep-registry.json",
+        "license": "semgrep-registry.LICENSE",
+        "license_key": "semgrep-registry",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-semgrep-registry",
+        "yaml": "semgrep-registry.yml"
+    },
+    {
         "category": "Copyleft",
         "html": "sencha-app-floss-exception.html",
         "is_deprecated": false,
         "is_exception": true,
         "json": "sencha-app-floss-exception.json",
         "license": "sencha-app-floss-exception.LICENSE",
         "license_key": "sencha-app-floss-exception",
@@ -20779,14 +21631,26 @@
         "license": "signal-gpl-3.0-exception.LICENSE",
         "license_key": "signal-gpl-3.0-exception",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-signal-gpl-3.0-exception",
         "yaml": "signal-gpl-3.0-exception.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "silicon-image-2007.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "silicon-image-2007.json",
+        "license": "silicon-image-2007.LICENSE",
+        "license_key": "silicon-image-2007",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-silicon-image-2007",
+        "yaml": "silicon-image-2007.yml"
+    },
+    {
         "category": "Permissive",
         "html": "simpl-1.1.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "simpl-1.1.json",
         "license": "simpl-1.1.LICENSE",
         "license_key": "simpl-1.1",
@@ -20966,16 +21830,18 @@
         "category": "Permissive",
         "html": "snprintf.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "snprintf.json",
         "license": "snprintf.LICENSE",
         "license_key": "snprintf",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-snprintf",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-snprintf"
+        ],
+        "spdx_license_key": "snprintf",
         "yaml": "snprintf.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "softerra-ldap-browser-eula.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -21652,14 +22518,26 @@
         "license_key": "sun-bsd-no-nuclear",
         "other_spdx_license_keys": [],
         "spdx_license_key": "BSD-3-Clause-No-Nuclear-License",
         "yaml": "sun-bsd-no-nuclear.yml"
     },
     {
         "category": "Proprietary Free",
+        "html": "sun-cc-pp-1.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "sun-cc-pp-1.0.json",
+        "license": "sun-cc-pp-1.0.LICENSE",
+        "license_key": "sun-cc-pp-1.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-sun-cc-pp-1.0",
+        "yaml": "sun-cc-pp-1.0.yml"
+    },
+    {
+        "category": "Proprietary Free",
         "html": "sun-communications-api.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "sun-communications-api.json",
         "license": "sun-communications-api.LICENSE",
         "license_key": "sun-communications-api",
         "other_spdx_license_keys": [],
@@ -21948,16 +22826,18 @@
         "category": "Permissive",
         "html": "sunpro.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "sunpro.json",
         "license": "sunpro.LICENSE",
         "license_key": "sunpro",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-sunpro",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-sunpro"
+        ],
+        "spdx_license_key": "SunPro",
         "yaml": "sunpro.yml"
     },
     {
         "category": "Permissive",
         "html": "sunsoft.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -22001,14 +22881,26 @@
         "license": "svndiff.LICENSE",
         "license_key": "svndiff",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-svndiff",
         "yaml": "svndiff.yml"
     },
     {
+        "category": "Copyleft Limited",
+        "html": "swi-exception.html",
+        "is_deprecated": false,
+        "is_exception": true,
+        "json": "swi-exception.json",
+        "license": "swi-exception.LICENSE",
+        "license_key": "swi-exception",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "SWI-exception",
+        "yaml": "swi-exception.yml"
+    },
+    {
         "category": "Permissive",
         "html": "swig.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "swig.json",
         "license": "swig.LICENSE",
         "license_key": "swig",
@@ -22037,14 +22929,26 @@
         "license": "sybase.LICENSE",
         "license_key": "sybase",
         "other_spdx_license_keys": [],
         "spdx_license_key": "Watcom-1.0",
         "yaml": "sybase.yml"
     },
     {
+        "category": "Public Domain",
+        "html": "symlinks.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "symlinks.json",
+        "license": "symlinks.LICENSE",
+        "license_key": "symlinks",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "Symlinks",
+        "yaml": "symlinks.yml"
+    },
+    {
         "category": "Permissive",
         "html": "symphonysoft.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "symphonysoft.json",
         "license": "symphonysoft.LICENSE",
         "license_key": "symphonysoft",
@@ -22097,14 +23001,134 @@
         "license": "synthesis-toolkit.LICENSE",
         "license_key": "synthesis-toolkit",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-synthesis-toolkit",
         "yaml": "synthesis-toolkit.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "t-engine-public.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-engine-public.json",
+        "license": "t-engine-public.LICENSE",
+        "license_key": "t-engine-public",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-engine-public",
+        "yaml": "t-engine-public.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-1.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-1.0.json",
+        "license": "t-license-1.0.LICENSE",
+        "license_key": "t-license-1.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-1.0",
+        "yaml": "t-license-1.0.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-2.0.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-2.0.json",
+        "license": "t-license-2.0.LICENSE",
+        "license_key": "t-license-2.0",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-2.0",
+        "yaml": "t-license-2.0.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-2.1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-2.1.json",
+        "license": "t-license-2.1.LICENSE",
+        "license_key": "t-license-2.1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-2.1",
+        "yaml": "t-license-2.1.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-2.2.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-2.2.json",
+        "license": "t-license-2.2.LICENSE",
+        "license_key": "t-license-2.2",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-2.2",
+        "yaml": "t-license-2.2.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-amp-t-kernel.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-amp-t-kernel.json",
+        "license": "t-license-amp-t-kernel.LICENSE",
+        "license_key": "t-license-amp-t-kernel",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-amp-t-kernel",
+        "yaml": "t-license-amp-t-kernel.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-amp-tkse.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-amp-tkse.json",
+        "license": "t-license-amp-tkse.LICENSE",
+        "license_key": "t-license-amp-tkse",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-amp-tkse",
+        "yaml": "t-license-amp-tkse.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-smp-t-kernel.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-smp-t-kernel.json",
+        "license": "t-license-smp-t-kernel.LICENSE",
+        "license_key": "t-license-smp-t-kernel",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-smp-t-kernel",
+        "yaml": "t-license-smp-t-kernel.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-smp-tkse.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-smp-tkse.json",
+        "license": "t-license-smp-tkse.LICENSE",
+        "license_key": "t-license-smp-tkse",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-smp-tkse",
+        "yaml": "t-license-smp-tkse.yml"
+    },
+    {
+        "category": "Proprietary Free",
+        "html": "t-license-tkse.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "t-license-tkse.json",
+        "license": "t-license-tkse.LICENSE",
+        "license_key": "t-license-tkse",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-t-license-tkse",
+        "yaml": "t-license-tkse.yml"
+    },
+    {
         "category": "Permissive",
         "html": "takao-abe.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "takao-abe.json",
         "license": "takao-abe.LICENSE",
         "license_key": "takao-abe",
@@ -22230,14 +23254,26 @@
         "license_key": "tatu-ylonen",
         "other_spdx_license_keys": [],
         "spdx_license_key": "SSH-short",
         "yaml": "tatu-ylonen.yml"
     },
     {
         "category": "Permissive",
+        "html": "tcg-spec-license-v1.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "tcg-spec-license-v1.json",
+        "license": "tcg-spec-license-v1.LICENSE",
+        "license_key": "tcg-spec-license-v1",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-tcg-spec-license-v1",
+        "yaml": "tcg-spec-license-v1.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "tcl.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "tcl.json",
         "license": "tcl.LICENSE",
         "license_key": "tcl",
         "other_spdx_license_keys": [],
@@ -22361,14 +23397,26 @@
         "license": "tfl.LICENSE",
         "license_key": "tfl",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-tfl",
         "yaml": "tfl.yml"
     },
     {
+        "category": "Permissive",
+        "html": "tgc-spec-license-v2.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "tgc-spec-license-v2.json",
+        "license": "tgc-spec-license-v2.LICENSE",
+        "license_key": "tgc-spec-license-v2",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-tcg-spec-license-v2",
+        "yaml": "tgc-spec-license-v2.yml"
+    },
+    {
         "category": "Copyleft",
         "html": "tgppl-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "tgppl-1.0.json",
         "license": "tgppl-1.0.LICENSE",
         "license_key": "tgppl-1.0",
@@ -22404,16 +23452,18 @@
         "category": "Copyleft Limited",
         "html": "thor-pl.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "thor-pl.json",
         "license": "thor-pl.LICENSE",
         "license_key": "thor-pl",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-thor-pl",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-thor-pl"
+        ],
+        "spdx_license_key": "TPL-1.0",
         "yaml": "thor-pl.yml"
     },
     {
         "category": "Proprietary Free",
         "html": "ti-broadband-apps.html",
         "is_deprecated": false,
         "is_exception": false,
@@ -22565,14 +23615,26 @@
         "license": "tosl.LICENSE",
         "license_key": "tosl",
         "other_spdx_license_keys": [],
         "spdx_license_key": "TOSL",
         "yaml": "tosl.yml"
     },
     {
+        "category": "Permissive",
+        "html": "tpdl.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "tpdl.json",
+        "license": "tpdl.LICENSE",
+        "license_key": "tpdl",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "TPDL",
+        "yaml": "tpdl.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "tpl-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "tpl-1.0.json",
         "license": "tpl-1.0.LICENSE",
         "license_key": "tpl-1.0",
@@ -22697,14 +23759,26 @@
         "license": "truecrypt-3.1.LICENSE",
         "license_key": "truecrypt-3.1",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-truecrypt-3.1",
         "yaml": "truecrypt-3.1.yml"
     },
     {
+        "category": "Proprietary Free",
+        "html": "trustonic-proprietary-2013.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "trustonic-proprietary-2013.json",
+        "license": "trustonic-proprietary-2013.LICENSE",
+        "license_key": "trustonic-proprietary-2013",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-trustonic-proprietary-2013",
+        "yaml": "trustonic-proprietary-2013.yml"
+    },
+    {
         "category": "Source-available",
         "html": "tsl-2018.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "tsl-2018.json",
         "license": "tsl-2018.LICENSE",
         "license_key": "tsl-2018",
@@ -22758,14 +23832,26 @@
         "license_key": "ttf2pt1",
         "other_spdx_license_keys": [],
         "spdx_license_key": null,
         "yaml": "ttf2pt1.yml"
     },
     {
         "category": "Permissive",
+        "html": "ttwl.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ttwl.json",
+        "license": "ttwl.LICENSE",
+        "license_key": "ttwl",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "TTWL",
+        "yaml": "ttwl.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "ttyp0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ttyp0.json",
         "license": "ttyp0.LICENSE",
         "license_key": "ttyp0",
         "other_spdx_license_keys": [],
@@ -22877,14 +23963,26 @@
         "license": "ubuntu-font-1.0.LICENSE",
         "license_key": "ubuntu-font-1.0",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-ubuntu-font-1.0",
         "yaml": "ubuntu-font-1.0.yml"
     },
     {
+        "category": "Permissive",
+        "html": "ucar.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "ucar.json",
+        "license": "ucar.LICENSE",
+        "license_key": "ucar",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "UCAR",
+        "yaml": "ucar.yml"
+    },
+    {
         "category": "Copyleft Limited",
         "html": "ucl-1.0.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "ucl-1.0.json",
         "license": "ucl-1.0.LICENSE",
         "license_key": "ucl-1.0",
@@ -23133,14 +24231,26 @@
         "license": "unrar.LICENSE",
         "license_key": "unrar",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-unrar",
         "yaml": "unrar.yml"
     },
     {
+        "category": "Source-available",
+        "html": "unrar-v3.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "unrar-v3.json",
+        "license": "unrar-v3.LICENSE",
+        "license_key": "unrar-v3",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-unrar-v3",
+        "yaml": "unrar-v3.yml"
+    },
+    {
         "category": "Free Restricted",
         "html": "unsplash.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "unsplash.json",
         "license": "unsplash.LICENSE",
         "license_key": "unsplash",
@@ -23353,14 +24463,26 @@
         "license_key": "vim",
         "other_spdx_license_keys": [],
         "spdx_license_key": "Vim",
         "yaml": "vim.yml"
     },
     {
         "category": "Permissive",
+        "html": "vince.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "vince.json",
+        "license": "vince.LICENSE",
+        "license_key": "vince",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-vince",
+        "yaml": "vince.yml"
+    },
+    {
+        "category": "Permissive",
         "html": "visual-idiot.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "visual-idiot.json",
         "license": "visual-idiot.LICENSE",
         "license_key": "visual-idiot",
         "other_spdx_license_keys": [],
@@ -23520,14 +24642,38 @@
         "license": "w3c.LICENSE",
         "license_key": "w3c",
         "other_spdx_license_keys": [],
         "spdx_license_key": "W3C",
         "yaml": "w3c.yml"
     },
     {
+        "category": "Permissive",
+        "html": "w3c-03-bsd-license.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "w3c-03-bsd-license.json",
+        "license": "w3c-03-bsd-license.LICENSE",
+        "license_key": "w3c-03-bsd-license",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-w3c-03-bsd-license",
+        "yaml": "w3c-03-bsd-license.yml"
+    },
+    {
+        "category": "CLA",
+        "html": "w3c-community-cla.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "w3c-community-cla.json",
+        "license": "w3c-community-cla.LICENSE",
+        "license_key": "w3c-community-cla",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "LicenseRef-scancode-w3c-community-cla",
+        "yaml": "w3c-community-cla.yml"
+    },
+    {
         "category": "Free Restricted",
         "html": "w3c-docs-19990405.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "w3c-docs-19990405.json",
         "license": "w3c-docs-19990405.LICENSE",
         "license_key": "w3c-docs-19990405",
@@ -23604,14 +24750,26 @@
         "license": "w3c-test-suite.LICENSE",
         "license_key": "w3c-test-suite",
         "other_spdx_license_keys": [],
         "spdx_license_key": "LicenseRef-scancode-w3c-test-suite",
         "yaml": "w3c-test-suite.yml"
     },
     {
+        "category": "Permissive",
+        "html": "w3m.html",
+        "is_deprecated": false,
+        "is_exception": false,
+        "json": "w3m.json",
+        "license": "w3m.LICENSE",
+        "license_key": "w3m",
+        "other_spdx_license_keys": [],
+        "spdx_license_key": "w3m",
+        "yaml": "w3m.yml"
+    },
+    {
         "category": "Unstated License",
         "html": "warranty-disclaimer.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "warranty-disclaimer.json",
         "license": "warranty-disclaimer.LICENSE",
         "license_key": "warranty-disclaimer",
@@ -24043,16 +25201,18 @@
         "category": "Permissive",
         "html": "x11-bitstream.html",
         "is_deprecated": false,
         "is_exception": false,
         "json": "x11-bitstream.json",
         "license": "x11-bitstream.LICENSE",
         "license_key": "x11-bitstream",
-        "other_spdx_license_keys": [],
-        "spdx_license_key": "LicenseRef-scancode-x11-bitstream",
+        "other_spdx_license_keys": [
+            "LicenseRef-scancode-x11-bitstream"
+        ],
+        "spdx_license_key": "Bitstream-Charter",
         "yaml": "x11-bitstream.yml"
     },
     {
         "category": "Permissive",
         "html": "x11-dec1.html",
         "is_deprecated": false,
         "is_exception": false,
```

### Comparing `license-expression-30.1.0/src/license_expression.egg-info/PKG-INFO` & `license-expression-30.1.1/src/license_expression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-expression
-Version: 30.1.0
+Version: 30.1.1
 Summary: license-expression is a comprehensive utility library to parse, compare, simplify and normalize license expressions (such as SPDX license expressions) using boolean logic.
 Home-page: https://github.com/nexB/license-expression
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,license expression,license,spdx,boolean,parse expression,normalize expression,compare expression,licence
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,15 +46,15 @@
 npm and Rubygems; they are important when exchanging software data (such as with
 SPDX and SBOM in general) as a way to express licensing precisely.
 
 ``license-expression`` is a comprehensive utility library to parse, compare,
 simplify and normalize these license expressions (such as SPDX license expressions)
 using boolean logic like in: `GPL-2.0-or-later WITH Classpath-exception-2.0 AND MIT`.
 
-It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.19)
+It includes the license keys from SPDX https://spdx.org/licenses/ (version 3.20)
 and ScanCode license DB (version 21.6.7) https://scancode-licensedb.aboutcode.org/
 to get started quickly.
 
 ``license-expression`` is both powerful and simple to use and is a used as the
 license expression engine in several projects and products such as:
 
 - AboutCode-toolkit https://github.com/nexB/aboutcode-toolkit
@@ -132,15 +132,15 @@
 This supports SPDX license expressions and also accepts other license naming
 conventions and license identifiers aliases to resolve and normalize any license
 expressions.
 
 Using boolean logic, license expressions can be tested for equality, containment,
 equivalence and can be normalized or simplified.
 
-It also bundles the SPDX License list (3.19 as of now) and the ScanCode license
+It also bundles the SPDX License list (3.20 as of now) and the ScanCode license
 DB (based on latest ScanCode) to easily parse and validate expressions using
 the license symbols.
 
 
 Usage examples
 ==============
```

### Comparing `license-expression-30.1.0/src/license_expression.egg-info/SOURCES.txt` & `license-expression-30.1.1/src/license_expression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/tests/data/test_license_key_index.json` & `license-expression-30.1.1/tests/data/test_license_key_index.json`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/tests/test__pyahocorasick.py` & `license-expression-30.1.1/tests/test__pyahocorasick.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/tests/test_license_expression.py` & `license-expression-30.1.1/tests/test_license_expression.py`

 * *Files identical despite different names*

### Comparing `license-expression-30.1.0/tests/test_skeleton_codestyle.py` & `license-expression-30.1.1/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*


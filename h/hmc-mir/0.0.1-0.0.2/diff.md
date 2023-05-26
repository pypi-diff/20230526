# Comparing `tmp/hmc_mir-0.0.1.tar.gz` & `tmp/hmc_mir-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmc_mir-0.0.1.tar", last modified: Thu May 25 22:20:22 2023, max compression
+gzip compressed data, was "hmc_mir-0.0.2.tar", last modified: Fri May 26 21:38:05 2023, max compression
```

## Comparing `hmc_mir-0.0.1.tar` & `hmc_mir-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/src/hmc_mir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/src/hmc_mir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-25 22:20:14.000000 hmc_mir-0.0.1/src/hmc_mir/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:20:22.096175 hmc_mir-0.0.1/src/hmc_mir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-25 22:20:22.000000 hmc_mir-0.0.1/src/hmc_mir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-25 22:20:22.000000 hmc_mir-0.0.1/src/hmc_mir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:20:22.000000 hmc_mir-0.0.1/src/hmc_mir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 22:20:22.000000 hmc_mir-0.0.1/src/hmc_mir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.373570 hmc_mir-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.373570 hmc_mir-0.0.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.373570 hmc_mir-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/src/hmc_mir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/src/hmc_mir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/src/hmc_mir/bootleg_score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/src/hmc_mir/bootleg_score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/src/hmc_mir/bootleg_score/bootleg_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/src/hmc_mir/tsm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/src/hmc_mir/tsm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-26 21:37:57.000000 hmc_mir-0.0.2/src/hmc_mir/tsm_tools/tsm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:38:05.377570 hmc_mir-0.0.2/src/hmc_mir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 21:38:05.000000 hmc_mir-0.0.2/src/hmc_mir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 21:38:05.000000 hmc_mir-0.0.2/src/hmc_mir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:38:05.000000 hmc_mir-0.0.2/src/hmc_mir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 21:38:05.000000 hmc_mir-0.0.2/src/hmc_mir.egg-info/top_level.txt
```

### Comparing `hmc_mir-0.0.1/.github/scripts/release.py` & `hmc_mir-0.0.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.0.1/LICENSE` & `hmc_mir-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.0.1/PKG-INFO` & `hmc_mir-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmc_mir
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `hmc_mir-0.0.1/setup.cfg` & `hmc_mir-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.0.1/src/hmc_mir.egg-info/PKG-INFO` & `hmc_mir-0.0.2/src/hmc_mir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmc-mir
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```


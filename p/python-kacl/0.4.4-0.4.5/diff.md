# Comparing `tmp/python-kacl-0.4.4.tar.gz` & `tmp/python-kacl-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.4.4.tar", last modified: Fri May 26 13:53:18 2023, max compression
+gzip compressed data, was "python-kacl-0.4.5.tar", last modified: Fri May 26 16:28:07 2023, max compression
```

## Comparing `python-kacl-0.4.4.tar` & `python-kacl-0.4.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.445537 python-kacl-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-26 13:53:10.000000 python-kacl-0.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-26 13:53:10.000000 python-kacl-0.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19226 2023-05-26 13:53:18.445537 python-kacl-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    18577 2023-05-26 13:53:10.000000 python-kacl-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.443537 python-kacl-0.4.4/kacl/
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/changes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.443537 python-kacl-0.4.4/kacl/config/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/config/kacl-default.yml
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/config.py
--rw-rw-rw-   0 root         (0) root         (0)    20447 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/document.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/element.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/exception.py
--rwxrwxrwx   0 root         (0) root         (0)    16280 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/kacl_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/link_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     9533 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.444537 python-kacl-0.4.4/python_kacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19226 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 13:53:18.445537 python-kacl-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-26 13:53:10.000000 python-kacl-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.445537 python-kacl-0.4.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/snapshot_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    12545 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.816015 python-kacl-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-26 16:27:59.000000 python-kacl-0.4.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-26 16:27:59.000000 python-kacl-0.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19220 2023-05-26 16:28:07.816015 python-kacl-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18571 2023-05-26 16:27:59.000000 python-kacl-0.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.814015 python-kacl-0.4.5/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.814015 python-kacl-0.4.5/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    20447 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    16280 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9533 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.815015 python-kacl-0.4.5/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19220 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 16:28:07.816015 python-kacl-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-26 16:27:59.000000 python-kacl-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.816015 python-kacl-0.4.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/test_kacl.py
```

### Comparing `python-kacl-0.4.4/LICENSE` & `python-kacl-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/PKG-INFO` & `python-kacl-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,16 +34,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
-    - [Squashing releases](#squashing-releases)
-      - [Example](#example)
+  - [Squashing releases](#squashing-releases)
+    - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -444,15 +444,15 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
-### Squashing releases
+## Squashing releases
 
 If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
 
 To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
 
 ```bash
 Usage: kacl-cli squash [OPTIONS]
@@ -465,15 +465,15 @@
                        changelog file.
   --from-version TEXT  The version to start squashing from.  [required]
   --to-version TEXT    The version to squash to. If not given, the latest
                        version will be used.
   --help               Show this message and exit.
 ```
 
-#### Example
+### Example
 
 ```bash
 kacl-cli -f CHANGELOG.md squash \
   --from-version "0.0.1" \
   --from-version "1.0.0" \
   --modify
 ```
```

### Comparing `python-kacl-0.4.4/README.md` & `python-kacl-0.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
-    - [Squashing releases](#squashing-releases)
-      - [Example](#example)
+  - [Squashing releases](#squashing-releases)
+    - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -427,15 +427,15 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
-### Squashing releases
+## Squashing releases
 
 If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
 
 To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
 
 ```bash
 Usage: kacl-cli squash [OPTIONS]
@@ -448,15 +448,15 @@
                        changelog file.
   --from-version TEXT  The version to start squashing from.  [required]
   --to-version TEXT    The version to squash to. If not given, the latest
                        version will be used.
   --help               Show this message and exit.
 ```
 
-#### Example
+### Example
 
 ```bash
 kacl-cli -f CHANGELOG.md squash \
   --from-version "0.0.1" \
   --from-version "1.0.0" \
   --modify
 ```
```

### Comparing `python-kacl-0.4.4/kacl/__init__.py` & `python-kacl-0.4.5/kacl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the python-kacl package
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 from kacl.document import KACLDocument
 from kacl.serializer import KACLMarkdownSerializer
 
 
 def load(file):
     """
```

### Comparing `python-kacl-0.4.4/kacl/changes.py` & `python-kacl-0.4.5/kacl/changes.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/config/kacl-default.yml` & `python-kacl-0.4.5/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/config.py` & `python-kacl-0.4.5/kacl/config.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/document.py` & `python-kacl-0.4.5/kacl/document.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/kacl_cli.py` & `python-kacl-0.4.5/kacl/kacl_cli.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/link_provider.py` & `python-kacl-0.4.5/kacl/link_provider.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/parser.py` & `python-kacl-0.4.5/kacl/parser.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/serializer.py` & `python-kacl-0.4.5/kacl/serializer.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/validation.py` & `python-kacl-0.4.5/kacl/validation.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/kacl/version.py` & `python-kacl-0.4.5/kacl/version.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.5/python_kacl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,16 +34,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
-    - [Squashing releases](#squashing-releases)
-      - [Example](#example)
+  - [Squashing releases](#squashing-releases)
+    - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -444,15 +444,15 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
-### Squashing releases
+## Squashing releases
 
 If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
 
 To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
 
 ```bash
 Usage: kacl-cli squash [OPTIONS]
@@ -465,15 +465,15 @@
                        changelog file.
   --from-version TEXT  The version to start squashing from.  [required]
   --to-version TEXT    The version to squash to. If not given, the latest
                        version will be used.
   --help               Show this message and exit.
 ```
 
-#### Example
+### Example
 
 ```bash
 kacl-cli -f CHANGELOG.md squash \
   --from-version "0.0.1" \
   --from-version "1.0.0" \
   --modify
 ```
```

### Comparing `python-kacl-0.4.4/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.5/python_kacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/setup.py` & `python-kacl-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.4.4"
+version = "0.4.5"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [
```

### Comparing `python-kacl-0.4.4/tests/snapshot_directory.py` & `python-kacl-0.4.5/tests/snapshot_directory.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/tests/test_cli.py` & `python-kacl-0.4.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.4/tests/test_kacl.py` & `python-kacl-0.4.5/tests/test_kacl.py`

 * *Files identical despite different names*


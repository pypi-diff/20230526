# Comparing `tmp/python-kacl-0.4.3.tar.gz` & `tmp/python-kacl-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.4.3.tar", last modified: Wed May 24 20:29:37 2023, max compression
+gzip compressed data, was "python-kacl-0.4.4.tar", last modified: Fri May 26 13:53:18 2023, max compression
```

## Comparing `python-kacl-0.4.3.tar` & `python-kacl-0.4.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:29:37.257774 python-kacl-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-24 20:29:28.000000 python-kacl-0.4.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-24 20:29:28.000000 python-kacl-0.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17899 2023-05-24 20:29:37.256774 python-kacl-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17250 2023-05-24 20:29:28.000000 python-kacl-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:29:37.254774 python-kacl-0.4.3/kacl/
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/changes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:29:37.254774 python-kacl-0.4.3/kacl/config/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/config/kacl-default.yml
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/config.py
--rw-rw-rw-   0 root         (0) root         (0)    18740 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/document.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/element.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/exception.py
--rwxrwxrwx   0 root         (0) root         (0)    14252 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/kacl_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/link_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     9139 2023-05-24 20:29:28.000000 python-kacl-0.4.3/kacl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:29:37.255774 python-kacl-0.4.3/python_kacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17899 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 20:29:37.000000 python-kacl-0.4.3/python_kacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 20:29:37.257774 python-kacl-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-24 20:29:28.000000 python-kacl-0.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 20:29:37.256774 python-kacl-0.4.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-24 20:29:28.000000 python-kacl-0.4.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-24 20:29:28.000000 python-kacl-0.4.3/tests/snapshot_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-24 20:29:28.000000 python-kacl-0.4.3/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11806 2023-05-24 20:29:28.000000 python-kacl-0.4.3/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.445537 python-kacl-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-26 13:53:10.000000 python-kacl-0.4.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-26 13:53:10.000000 python-kacl-0.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19226 2023-05-26 13:53:18.445537 python-kacl-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18577 2023-05-26 13:53:10.000000 python-kacl-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.443537 python-kacl-0.4.4/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.443537 python-kacl-0.4.4/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    20447 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    16280 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9533 2023-05-26 13:53:10.000000 python-kacl-0.4.4/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.444537 python-kacl-0.4.4/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19226 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 13:53:18.000000 python-kacl-0.4.4/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 13:53:18.445537 python-kacl-0.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-26 13:53:10.000000 python-kacl-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 13:53:18.445537 python-kacl-0.4.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-05-26 13:53:10.000000 python-kacl-0.4.4/tests/test_kacl.py
```

### Comparing `python-kacl-0.4.3/LICENSE` & `python-kacl-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/PKG-INFO` & `python-kacl-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
+    - [Squashing releases](#squashing-releases)
+      - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -442,14 +444,46 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
+### Squashing releases
+
+If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
+
+To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
+
+```bash
+Usage: kacl-cli squash [OPTIONS]
+
+  Squshes all changes from a given version into a single section. Use '--
+  modify' to directly modify the changelog file.
+
+Options:
+  -m, --modify         This option will add the changes directly into
+                       changelog file.
+  --from-version TEXT  The version to start squashing from.  [required]
+  --to-version TEXT    The version to squash to. If not given, the latest
+                       version will be used.
+  --help               Show this message and exit.
+```
+
+#### Example
+
+```bash
+kacl-cli -f CHANGELOG.md squash \
+  --from-version "0.0.1" \
+  --from-version "1.0.0" \
+  --modify
+```
+
+This example will squash all versions between `0.0.1` and `1.0.0` and move them under `1.0.0`
+
 ## Extensions
 
 ### Post-release/Hotfix
 
 > **ATTENTION:** this is not SemVer compatible and not part of the KACL standard
 
 In some situations you might come across the challenge to patch a piece of software that is already in production and you _have to_ indicate that this is a `hotfix` release. `SemVer` is not meant to support this other than incrementing the `patch` version of your project, but it is not possible to release `1.0.1-hotfix.1` after `1.0.1` as `-hotfix.1` is considered a `prerelease` version and therefore is lower in order than the `1.0.1` version.
```

### Comparing `python-kacl-0.4.3/README.md` & `python-kacl-0.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
+    - [Squashing releases](#squashing-releases)
+      - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -425,14 +427,46 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
+### Squashing releases
+
+If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
+
+To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
+
+```bash
+Usage: kacl-cli squash [OPTIONS]
+
+  Squshes all changes from a given version into a single section. Use '--
+  modify' to directly modify the changelog file.
+
+Options:
+  -m, --modify         This option will add the changes directly into
+                       changelog file.
+  --from-version TEXT  The version to start squashing from.  [required]
+  --to-version TEXT    The version to squash to. If not given, the latest
+                       version will be used.
+  --help               Show this message and exit.
+```
+
+#### Example
+
+```bash
+kacl-cli -f CHANGELOG.md squash \
+  --from-version "0.0.1" \
+  --from-version "1.0.0" \
+  --modify
+```
+
+This example will squash all versions between `0.0.1` and `1.0.0` and move them under `1.0.0`
+
 ## Extensions
 
 ### Post-release/Hotfix
 
 > **ATTENTION:** this is not SemVer compatible and not part of the KACL standard
 
 In some situations you might come across the challenge to patch a piece of software that is already in production and you _have to_ indicate that this is a `hotfix` release. `SemVer` is not meant to support this other than incrementing the `patch` version of your project, but it is not possible to release `1.0.1-hotfix.1` after `1.0.1` as `-hotfix.1` is considered a `prerelease` version and therefore is lower in order than the `1.0.1` version.
```

### Comparing `python-kacl-0.4.3/kacl/__init__.py` & `python-kacl-0.4.4/kacl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the python-kacl package
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 from kacl.document import KACLDocument
 from kacl.serializer import KACLMarkdownSerializer
 
 
 def load(file):
     """
```

### Comparing `python-kacl-0.4.3/kacl/changes.py` & `python-kacl-0.4.4/kacl/changes.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/config/kacl-default.yml` & `python-kacl-0.4.4/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/config.py` & `python-kacl-0.4.4/kacl/config.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/document.py` & `python-kacl-0.4.4/kacl/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,14 +145,57 @@
         """Checks if the current changelog is valid
         Returns:
             [bool] -- true if valid false if not
         """
         validation_results = self.validate()
         return validation_results.is_valid()
 
+    def squash(self, version_start, version_end, keep_version_info=True):
+
+        if isinstance(version_start, str):
+            version_start = semver.VersionInfo.parse(version_start)
+        if isinstance(version_end, str):
+            version_end = semver.VersionInfo.parse(version_end)
+
+        versions = self.versions()
+        versions.sort(reverse=True)
+        versions_to_squash = []
+        versions_unsquashed = []
+        for v in versions:
+            if "unreleased" in v.version().lower():
+                versions_unsquashed.append(v)
+            elif v.semver() >= version_start and v.semver() <= version_end:
+                versions_to_squash.append(v)
+            else:
+                versions_unsquashed.append(v)
+
+        # sort versions descending
+        versions_to_squash.sort(reverse=True)
+
+        # get the version that will be the new version
+        squash_version = versions_to_squash[0]
+
+        # remove version from the squashed list
+        versions_to_squash.remove(squash_version)
+
+        # add all sections from the squashed versions to the new version
+        for v in versions_to_squash:
+            for section, changes in v.sections().items():
+                for change in changes.items():
+                    if keep_version_info:
+                        if v.has_link_reference():
+                            change = f"[[{v.version()}]({v.link()})] {change}"
+                        else:
+                            change = f"[{v.version()}] {change}"
+                    squash_version.add(section, change)
+
+        versions_unsquashed.append(squash_version)
+        versions_unsquashed.sort(reverse=True)
+        self.__versions = versions_unsquashed
+
     def has_changes(self):
         unreleased_version = self.get("Unreleased")
         if not unreleased_version:
             return False
 
         sections = unreleased_version.sections()
         if not sections or len(sections) == 0:
```

### Comparing `python-kacl-0.4.3/kacl/kacl_cli.py` & `python-kacl-0.4.4/kacl/kacl_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -477,14 +477,91 @@
                         message=tag_description.format(**vcs_context),
                     )
     else:
         click.echo(kacl_changelog_content)
 
 
 @cli.command()
+@click.pass_context
+@click.option(
+    "-m",
+    "--modify",
+    is_flag=True,
+    help="This option will add the changes directly into changelog file.",
+)
+@click.option(
+    "--from-version",
+    required=True,
+    default=None,
+    type=str,
+    help="The version to start squashing from.",
+)
+@click.option(
+    "--to-version",
+    required=False,
+    default=None,
+    type=str,
+    help="The version to squash to. If not given, the latest version will be used.",
+)
+def squash(
+    ctx,
+    modify,
+    from_version,
+    to_version,
+):
+    """Squshes all changes from a given version into a single section. Use '--modify' to directly modify the changelog file."""
+
+    kacl_changelog = load_changelog(ctx)
+
+    if not kacl_changelog.is_valid():
+        click.echo(
+            click.style("Error: ", fg="red")
+            + "Changelog is not valid. Run 'kacl-cli verify' for more information."
+        )
+        sys.exit(1)
+
+    if not to_version:
+        to_version = kacl_changelog.current_version()
+    else:
+        try:
+            to_version = semver.VersionInfo.parse(to_version)
+        except Exception:
+            click.echo(
+                click.style("Error: ", fg="red")
+                + f'"{to_version}" not a valid semantic version.'
+            )
+            sys.exit(1)
+
+    try:
+        from_version = semver.VersionInfo.parse(from_version)
+    except Exception:
+        click.echo(
+            click.style("Error: ", fg="red")
+            + f'"{from_version}" not a valid semantic version.'
+        )
+        sys.exit(1)
+
+    # squash the changes
+    kacl_changelog.squash(
+        version_start=from_version, version_end=to_version, keep_version_info=True
+    )
+
+    # dump the content
+    kacl_changelog_content = kacl.dump(kacl_changelog)
+
+    # check if we should modify the file
+    if modify:
+        with open(kacl_changelog.config.changelog_file_path, "w") as f:
+            f.write(kacl_changelog_content)
+        f.close()
+    else:
+        click.echo(kacl_changelog_content)
+
+
+@cli.command()
 @click.option(
     "-o",
     "--output-file",
     required=False,
     type=click.Path(exists=False),
     help="File to write the created changelog to.",
 )
```

### Comparing `python-kacl-0.4.3/kacl/link_provider.py` & `python-kacl-0.4.4/kacl/link_provider.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/parser.py` & `python-kacl-0.4.4/kacl/parser.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/serializer.py` & `python-kacl-0.4.4/kacl/serializer.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/validation.py` & `python-kacl-0.4.4/kacl/validation.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/kacl/version.py` & `python-kacl-0.4.4/kacl/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,45 @@
         if sections is None:
             self.__sections = dict()
         else:
             self.__sections = sections
         self.__link_reference = None
         self.set_link(link)
 
+    def __lt__(self, obj):
+        if self.version().lower() == "unreleased":
+            return False
+        elif obj.version().lower() == "unreleased":
+            return False
+        else:
+            return (self.semver()) < (obj.semver())
+
+    def __eq__(self, obj):
+        return self.version() == obj.version()
+
+    def __repr__(self):
+        return self.__version
+
     def link(self):
         if self.__link_reference:
             return self.__link_reference.body()
 
     def set_link(self, link):
         if isinstance(link, KACLElement):
             self.__link_reference = link
         elif link is not None:
             self.__link_reference = KACLElement(title=self.version(), body=link)
 
     def has_link_reference(self):
         if not self.__link_reference:
             return False
         else:
-            return self.__link_reference.body() is not None and len(
-                self.__link_reference.body()
+            return bool(
+                self.__link_reference.body() is not None
+                and self.__link_reference.body()
             )
 
     def date(self):
         if not len(self.__date):
             title = self.title()
             m = re.search(r"\d\d\d\d-\d\d-\d\d", title)
             if m:
```

### Comparing `python-kacl-0.4.3/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.4/python_kacl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,16 @@
   - [Create a Changelog](#create-a-changelog)
   - [Verify a Changelog](#verify-a-changelog)
   - [Print the current release version](#print-the-current-release-version)
   - [Print a single release changelog](#print-a-single-release-changelog)
   - [Add an entry to an unreleased section](#add-an-entry-to-an-unreleased-section)
   - [Prepare a Changelog for a Release](#prepare-a-changelog-for-a-release)
   - [Link Generation](#link-generation)
+    - [Squashing releases](#squashing-releases)
+      - [Example](#example)
   - [Extensions](#extensions)
     - [Post-release/Hotfix](#post-releasehotfix)
   - [Config file](#config-file)
   - [Development](#development)
 
 ## Installation
 
@@ -442,14 +444,46 @@
         compare_versions_template: '{host}/compare/v{previous_version}...v{version}'
         unreleased_changes_template: '{host}/tree/v{latest_version}...HEAD'
         initial_version_template: '{host}/tree/v{version}'
 ```
 
 Using the python format syntax you can generate any links you want. The available replacement variables are `version`, `previous_version`, `host` and `latest_version`.
 
+### Squashing releases
+
+If you are follwing a automated versioning approach, you will often times create a number of versions that might clutter Changelog. For this purpose, `kacl-cli` provides a `squash` command that let's you squash releases into a single one without loosing valuable information.
+
+To squash the versions, you will need to specify the version range to squash by passing `--from-version` and `--to-version` to `kacl-cli squash`. Strings passed need to be valid Semantic Versions.
+
+```bash
+Usage: kacl-cli squash [OPTIONS]
+
+  Squshes all changes from a given version into a single section. Use '--
+  modify' to directly modify the changelog file.
+
+Options:
+  -m, --modify         This option will add the changes directly into
+                       changelog file.
+  --from-version TEXT  The version to start squashing from.  [required]
+  --to-version TEXT    The version to squash to. If not given, the latest
+                       version will be used.
+  --help               Show this message and exit.
+```
+
+#### Example
+
+```bash
+kacl-cli -f CHANGELOG.md squash \
+  --from-version "0.0.1" \
+  --from-version "1.0.0" \
+  --modify
+```
+
+This example will squash all versions between `0.0.1` and `1.0.0` and move them under `1.0.0`
+
 ## Extensions
 
 ### Post-release/Hotfix
 
 > **ATTENTION:** this is not SemVer compatible and not part of the KACL standard
 
 In some situations you might come across the challenge to patch a piece of software that is already in production and you _have to_ indicate that this is a `hotfix` release. `SemVer` is not meant to support this other than incrementing the `patch` version of your project, but it is not possible to release `1.0.1-hotfix.1` after `1.0.1` as `-hotfix.1` is considered a `prerelease` version and therefore is lower in order than the `1.0.1` version.
```

### Comparing `python-kacl-0.4.3/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.4/python_kacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/setup.py` & `python-kacl-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.4.3"
+version = "0.4.4"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [
```

### Comparing `python-kacl-0.4.3/tests/snapshot_directory.py` & `python-kacl-0.4.4/tests/snapshot_directory.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.3/tests/test_cli.py` & `python-kacl-0.4.4/tests/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -166,7 +166,56 @@
             "-f",
             "CHANGELOG.md",
             "verify",
         ],
         catch_exceptions=False,
     )
     assert result.exit_code != 0, result.output
+
+
+@freeze_time("2023-01-01")
+def test_squash(tmp_path, snapshot):
+    runner = CliRunner()
+    resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_keepachangelog.com.md")
+
+    with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
+        result = runner.invoke(
+            cli,
+            [
+                "-f",
+                "CHANGELOG.md",
+                "squash",
+                "--from-version",
+                "0.0.1",
+                "--to-version",
+                "0.3.0",
+                "-m",
+            ],
+            catch_exceptions=False,
+        )
+        assert result.exit_code == 0, result.output
+        snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
+
+
+def test_squash_current(tmp_path, snapshot):
+    runner = CliRunner()
+    resources_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data/")
+    changelog_file = os.path.join(resources_dir, "CHANGELOG_keepachangelog.com.md")
+
+    with runner.isolated_filesystem(temp_dir=tmp_path) as project_root_path:
+        shutil.copyfile(changelog_file, os.path.join(project_root_path, "CHANGELOG.md"))
+        result = runner.invoke(
+            cli,
+            [
+                "-f",
+                "CHANGELOG.md",
+                "squash",
+                "--from-version",
+                "0.0.1",
+                "-m",
+            ],
+            catch_exceptions=False,
+        )
+        assert result.exit_code == 0, result.output
+        snapshot_directory(snapshot=snapshot, directory_path=project_root_path)
```

### Comparing `python-kacl-0.4.3/tests/test_kacl.py` & `python-kacl-0.4.4/tests/test_kacl.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest import TestCase
 
 import yaml
 
 import kacl
 from kacl.config import KACLConfig
 from kacl.exception import KACLException
+from tests.snapshot_directory import snapshot_directory
 
 
 class TestKacl(TestCase):
     def test_load_valid(self):
         changelog_file = os.path.join(
             os.path.dirname(os.path.realpath(__file__)), "data/CHANGELOG.md"
         )
@@ -345,7 +346,28 @@
 
             changelog = kacl.load(changelog_file)
             changelog.generate_links()
 
             versions = changelog.versions()
             for v in versions:
                 self.assertIsNotNone(v.link())
+
+
+def test_squash(tmp_path, snapshot):
+    changelog_file = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)),
+        "data/CHANGELOG_keepachangelog.com.md",
+    )
+    changelog = kacl.load(changelog_file)
+    assert changelog.is_valid()
+
+    validation = changelog.validate()
+    assert len(validation.errors()) < 1
+
+    changelog.squash(version_start="0.0.1", version_end="0.3.0", keep_version_info=True)
+
+    squashed_changelog_file = os.path.join(tmp_path, "CHANGELOG.md")
+    # Open the file for writing.
+    with open(squashed_changelog_file, "w") as f:
+        f.write(kacl.dump(changelog))
+
+    snapshot_directory(snapshot=snapshot, directory_path=tmp_path)
```


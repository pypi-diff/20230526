# Comparing `tmp/sphinxcontrib_moderncmakedomain-3.25.0.tar.gz` & `tmp/sphinxcontrib_moderncmakedomain-3.26.4.tar.gz`

## Comparing `sphinxcontrib_moderncmakedomain-3.25.0.tar` & `sphinxcontrib_moderncmakedomain-3.26.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/noxfile.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/.github/dependabot.yml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/sphinxcontrib/moderncmakedomain/__init__.py
--rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/sphinxcontrib/moderncmakedomain/cmake.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/sphinxcontrib/moderncmakedomain/colors.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/tests/test_version.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/.gitignore
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/LICENSE
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/pyproject.toml
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.25.0/PKG-INFO
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/noxfile.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/sphinxcontrib/moderncmakedomain/__init__.py
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/sphinxcontrib/moderncmakedomain/cmake.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/sphinxcontrib/moderncmakedomain/colors.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/tests/test_version.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/.gitignore
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/LICENSE
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/README.md
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/pyproject.toml
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.26.4/PKG-INFO
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/.pre-commit-config.yaml` & `sphinxcontrib_moderncmakedomain-3.26.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/noxfile.py` & `sphinxcontrib_moderncmakedomain-3.26.4/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import nox
 import urllib.request
 import re
 from pathlib import Path
 
 nox.options.sessions = ["lint", "tests"]
 
-ALL_PYTHONS = ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
+ALL_PYTHONS = ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
     session.install("pre-commit")
@@ -56,9 +56,10 @@
 
 
 @nox.session(python=ALL_PYTHONS)
 def tests(session):
     """
     Run the unit and regular tests.
     """
-    session.install(".", "pytest")
+    # Setuptools is required due to sphinx installing sphinxcontrib extensions that use pkg_resources (fixed upstream but not released yet)
+    session.install(".", "pytest", "setuptools")
     session.run("pytest", *session.posargs)
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/.github/workflows/cd.yml` & `sphinxcontrib_moderncmakedomain-3.26.4/.github/workflows/cd.yml`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-      with:
-        fetch-depth: 0
 
     - name: Build SDist and wheel
       run: pipx run build
 
     - uses: actions/upload-artifact@v3
       with:
         path: dist/*
@@ -26,17 +24,20 @@
       run: pipx run twine check dist/*
 
 
   publish:
     needs: [dist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
+    environment:
+      name: pypi
+      url: https://pypi.org/p/sphinxcontrib-moderncmakedomain
+    permissions:
+      id-token: write
 
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: artifact
         path: dist
 
-    - uses: pypa/gh-action-pypi-publish@v1.5.1
-      with:
-        password: ${{ secrets.pypi_password }}
+    - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/.github/workflows/ci.yml` & `sphinxcontrib_moderncmakedomain-3.26.4/.github/workflows/ci.yml`

 * *Files 23% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 
   test:
     name: Run quick tests
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
-      - uses: wntrblm/nox@2022.8.7
+      - uses: wntrblm/nox@2023.04.22
         with:
-          python-versions: "3.6, 3.7, 3.8, 3.9, 3.10, 3.11-dev"
+          python-versions: "3.7, 3.8, 3.9, 3.10, 3.11, 3.12-dev"
       - run: nox -s tests
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/sphinxcontrib/moderncmakedomain/cmake.py` & `sphinxcontrib_moderncmakedomain-3.26.4/sphinxcontrib/moderncmakedomain/cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,7 +471,8 @@
             yield (refname, refname, type, docname, refname, 1)
 
 def setup(app):
     app.add_directive('cmake-module', CMakeModule)
     app.add_transform(CMakeTransform)
     app.add_transform(CMakeXRefTransform)
     app.add_domain(CMakeDomain)
+    return {"parallel_read_safe": True}
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/sphinxcontrib/moderncmakedomain/colors.py` & `sphinxcontrib_moderncmakedomain-3.26.4/sphinxcontrib/moderncmakedomain/colors.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/.gitignore` & `sphinxcontrib_moderncmakedomain-3.26.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/LICENSE` & `sphinxcontrib_moderncmakedomain-3.26.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/README.md` & `sphinxcontrib_moderncmakedomain-3.26.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 projects is painful otherwise. This works *exactly* in the same way as Kitware,
 so some time might be needed to study their approach to these problems.
 
 This repository is under the same License as all of CMake, which is the
 BSD-3-Clause license.
 
 🚨🚨🚨
-Any issues you run into with this plugin must be reported to [Kitware][]
+Any issues you run into with this plugin must be reported to [Kitware][],
+unless they involve the packaging itself. The Python files exactly match
+the CMake source for the released version numbers.
 🚨🚨🚨
 
 # Installation
 
 ## PyPI
 
 This domain is available via PyPI. Install it directly via `pip`:
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/pyproject.toml` & `sphinxcontrib_moderncmakedomain-3.26.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sphinxcontrib-moderncmakedomain"
 description = "Sphinx Domain for Modern CMake"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 authors = [
     { name = "Kitware" },
 ]
 keywords = [
     "cmake",
     "documentation",
     "kitware",
     "sphinx",
     "sphinxcontrib",
 ]
 classifiers = [
     "Environment :: Console",
     "Environment :: Web Environment",
+    "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Documentation",
     "Topic :: Utilities",
 ]
 dependencies = ["sphinx"]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `sphinxcontrib_moderncmakedomain-3.25.0/PKG-INFO` & `sphinxcontrib_moderncmakedomain-3.26.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-moderncmakedomain
-Version: 3.25.0
+Version: 3.26.4
 Summary: Sphinx Domain for Modern CMake
 Project-URL: Homepage, https://github.com/scikit-build/moderncmakedomain
 Author: Kitware
 License-File: LICENSE
 Keywords: cmake,documentation,kitware,sphinx,sphinxcontrib
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Requires-Dist: sphinx
 Description-Content-Type: text/markdown
 
 # Sphinx Domain for Modern CMake
 
 This is taken directly from the Kitware git repository's Utilities directory.
 The original [sphinxcontrib-cmakedomain][] has not been touched in quite some and
@@ -33,15 +34,17 @@
 projects is painful otherwise. This works *exactly* in the same way as Kitware,
 so some time might be needed to study their approach to these problems.
 
 This repository is under the same License as all of CMake, which is the
 BSD-3-Clause license.
 
 🚨🚨🚨
-Any issues you run into with this plugin must be reported to [Kitware][]
+Any issues you run into with this plugin must be reported to [Kitware][],
+unless they involve the packaging itself. The Python files exactly match
+the CMake source for the released version numbers.
 🚨🚨🚨
 
 # Installation
 
 ## PyPI
 
 This domain is available via PyPI. Install it directly via `pip`:
```


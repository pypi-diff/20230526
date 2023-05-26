# Comparing `tmp/wheeel-0.0.1.tar.gz` & `tmp/wheeel-0.0.2.tar.gz`

## Comparing `wheeel-0.0.1.tar` & `wheeel-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 wheeel-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wheeel-0.0.1/wheeel/__about__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 wheeel-0.0.1/wheeel/__init__.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheeel-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheeel-0.0.1/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 wheeel-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 wheeel-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 wheeel-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wheeel-0.0.2/wheeel/__about__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 wheeel-0.0.2/wheeel/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 wheeel-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 wheeel-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 wheeel-0.0.2/README.md
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 wheeel-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 wheeel-0.0.2/PKG-INFO
```

### Comparing `wheeel-0.0.1/LICENSE.txt` & `wheeel-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wheeel-0.0.1/pyproject.toml` & `wheeel-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [project.urls]
 Documentation = "https://github.com/graingert/wheeel#readme"
 Issues = "https://github.com/graingert/wheeel/issues"
 Source = "https://github.com/graingert/wheeel"
 
 [project.scripts]
-wheel = "wheel.cli:main"
+wheeel = "wheel.cli:main"
 
 [tool.hatch.version]
 path = "wheeel/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `wheeel-0.0.1/PKG-INFO` & `wheeel-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeel
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/graingert/wheeel#readme
 Project-URL: Issues, https://github.com/graingert/wheeel/issues
 Project-URL: Source, https://github.com/graingert/wheeel
 Author-email: Thomas Grainger <tagrain@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


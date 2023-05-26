# Comparing `tmp/swaystatus-0.3.3.tar.gz` & `tmp/swaystatus-0.3.4.tar.gz`

## Comparing `swaystatus-0.3.3.tar` & `swaystatus-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/__main__.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/cli.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/config.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/element.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/env.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/logging.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/loop.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/modules.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/subprocess.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 swaystatus-0.3.3/src/swaystatus/updater.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swaystatus-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 swaystatus-0.3.3/tests/test_element.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swaystatus-0.3.3/tests/test_modules.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 swaystatus-0.3.3/tests/test_updater.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 swaystatus-0.3.3/tests/modules/no_output.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 swaystatus-0.3.3/.gitignore
--rw-r--r--   0        0        0    34774 2020-02-02 00:00:00.000000 swaystatus-0.3.3/LICENSE.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swaystatus-0.3.3/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 swaystatus-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 swaystatus-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/__main__.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/cli.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/config.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/element.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/env.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/logging.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/loop.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/modules.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/subprocess.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 swaystatus-0.3.4/src/swaystatus/updater.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swaystatus-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 swaystatus-0.3.4/tests/test_element.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swaystatus-0.3.4/tests/test_modules.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 swaystatus-0.3.4/tests/test_updater.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 swaystatus-0.3.4/tests/modules/no_output.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 swaystatus-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 swaystatus-0.3.4/LICENSE
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 swaystatus-0.3.4/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 swaystatus-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 swaystatus-0.3.4/PKG-INFO
```

### Comparing `swaystatus-0.3.3/src/swaystatus/__init__.py` & `swaystatus-0.3.4/src/swaystatus/__init__.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/cli.py` & `swaystatus-0.3.4/src/swaystatus/cli.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/config.py` & `swaystatus-0.3.4/src/swaystatus/config.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/element.py` & `swaystatus-0.3.4/src/swaystatus/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
                     }
                 )
 
                 def create_handler(send):
                     def handler(line):
                         message = str(line, "utf-8").strip()
                         send(
-                            f"Output from module {self} button {button} handler: {message}"
+                            f"Output from module {self} "
+                            f"button {button} handler: {message}"
                         )
 
                     return handler
 
                 stdout = create_handler(logger.info)
                 stderr = create_handler(logger.error)
```

### Comparing `swaystatus-0.3.3/src/swaystatus/logging.py` & `swaystatus-0.3.4/src/swaystatus/logging.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/loop.py` & `swaystatus-0.3.4/src/swaystatus/loop.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/modules.py` & `swaystatus-0.3.4/src/swaystatus/modules.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/subprocess.py` & `swaystatus-0.3.4/src/swaystatus/subprocess.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/src/swaystatus/updater.py` & `swaystatus-0.3.4/src/swaystatus/updater.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/tests/test_element.py` & `swaystatus-0.3.4/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/tests/test_modules.py` & `swaystatus-0.3.4/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/tests/test_updater.py` & `swaystatus-0.3.4/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `swaystatus-0.3.3/pyproject.toml` & `swaystatus-0.3.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 [project]
 name = "swaystatus"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     { name="Jeremy Cantrell", email="jmcantrell@gmail.com" }
 ]
-description = "Generates a status line for swaybar"
+description = "Generate a status line for swaybar"
 readme = "README.md"
-license-files = { paths = ["LICENSE.md"] }
+license-files = { paths = ["LICENSE"] }
 requires-python = ">=3.10"
 keywords = ["sway", "wm", "status"]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
-    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "toml>=0.10",
+    "toml"
+]
+
+[project.optional-dependencies]
+dev = [
+    "black",
+    "build",
+    "pytest",
+    "ruff",
+    "twine",
 ]
 
 [project.urls]
 "Homepage" = "https://git.sr.ht/~jmcantrell/swaystatus"
 "Bug Tracker" = "https://todo.sr.ht/~jmcantrell/swaystatus"
 
 [project.scripts]
```


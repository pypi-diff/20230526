# Comparing `tmp/esp-debug-backend-1.0.2.tar.gz` & `tmp/esp-debug-backend-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-debug-backend/esp-debug-backend/dist/.tmp-9bg99a93/esp-debug-backend-1.0.2.tar", last modified: Wed Apr 19 19:12:26 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-debug-backend/esp-debug-backend/dist/.tmp-3nxg9u1c/esp-debug-backend-1.0.3.tar", last modified: Fri May 26 21:42:56 2023, max compression
```

## Comparing `esp-debug-backend-1.0.2.tar` & `esp-debug-backend-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/gdb_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/esp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/riscv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/xtensa.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/oocd.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/tests/test_gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/tests/test_oocd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30135 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/gdb_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/esp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/esp_init.gdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/riscv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/xtensa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/oocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/src/esp_debug_backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:42:56.000000 esp-debug-backend-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/tests/test_gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 21:42:36.000000 esp-debug-backend-1.0.3/tests/test_oocd.py
```

### Comparing `esp-debug-backend-1.0.2/LICENSE` & `esp-debug-backend-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/PKG-INFO` & `esp-debug-backend-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-debug-backend
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package is a library built on top of pygdbmi providing high-level API for debugging programs using GDB and OpenOCD.
 Author-email: Alexey Gerenkov <alexey.gerenkov@espressif.com>, Andrei Gramakov <andrei.gramakov@espressif.com>
 Project-URL: Homepage, https://github.com/espressif/esp-debug-backend
 Project-URL: Bug Tracker, https://github.com/espressif/esp-debug-backend/issues
 Project-URL: Documentation, https://github.com/espressif/esp-debug-backend/blob/master/README.md
 Project-URL: Changelog, https://github.com/espressif/esp-debug-backend/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
```

### Comparing `esp-debug-backend-1.0.2/pyproject.toml` & `esp-debug-backend-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "esp-debug-backend"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Alexey Gerenkov", email="alexey.gerenkov@espressif.com" },
   { name="Andrei Gramakov", email="andrei.gramakov@espressif.com" },
 ]
 description = "This package is a library built on top of pygdbmi providing high-level API for debugging programs using GDB and OpenOCD."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -24,12 +24,18 @@
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "pygdbmi>=0.9.0.0",
 ]
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+esp_debug_backend = ["hw_specific/esp_init.gdb"]
+
 [project.urls]
 "Homepage" = "https://github.com/espressif/esp-debug-backend"
 "Bug Tracker" = "https://github.com/espressif/esp-debug-backend/issues"
 "Documentation" = "https://github.com/espressif/esp-debug-backend/blob/master/README.md"
 "Changelog" = "https://github.com/espressif/esp-debug-backend/blob/master/CHANGELOG.md"
```

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/__init__.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/defs.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/defs.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/gdb.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,14 +514,28 @@
             return res_body['hw-rwpt']['number']
         elif tp == 'rw':
             if 'hw-awpt' not in res_body or 'number' not in res_body['hw-awpt']:
                 raise DebuggerError('Failed to insert AWP!')
             return res_body['hw-awpt']['number']
         return None
 
+    def add_logpoint(self, loc, argument, ignore_count=0, cond='', tmp=False):
+        # -dprintf-insert [ -t ] [ -f ] [ -d ] [ -c condition ] [ -i ignore-count ]
+        # [ -p thread-id ] [ location ] [ format ]
+        # [ argument ]
+        cmd_args = '-i %d %s %s' % (ignore_count, loc, argument)
+        if len(cond):
+            cmd_args = '-c "%s" %s' % (cond, cmd_args)
+        if tmp:
+            cmd_args = "-t " + cmd_args
+        res, res_body = self._mi_cmd_run('-dprintf-insert %s' % cmd_args)
+        if res != 'done' or not res_body or 'bkpt' not in res_body or 'number' not in res_body['bkpt']:
+            raise DebuggerError('Failed to insert logpoint!')
+        return res_body['bkpt']['number']
+
     def delete_bp(self, bp):
         # -break-delete ( breakpoint )+
         res, _ = self._mi_cmd_run('-break-delete %s' % bp)
         if res != 'done':
             raise DebuggerError('Failed to delete BP!')
 
     def monitor_run(self, cmd, tmo=None, output_type=None):
```

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/gdb_helpers.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/gdb_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/esp.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/esp.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/riscv.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/riscv.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/xtensa.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/hw_specific/xtensa.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/log.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/log.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/oocd.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/oocd.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend/utils.py` & `esp-debug-backend-1.0.3/src/esp_debug_backend/utils.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/PKG-INFO` & `esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-debug-backend
-Version: 1.0.2
+Version: 1.0.3
 Summary: This package is a library built on top of pygdbmi providing high-level API for debugging programs using GDB and OpenOCD.
 Author-email: Alexey Gerenkov <alexey.gerenkov@espressif.com>, Andrei Gramakov <andrei.gramakov@espressif.com>
 Project-URL: Homepage, https://github.com/espressif/esp-debug-backend
 Project-URL: Bug Tracker, https://github.com/espressif/esp-debug-backend/issues
 Project-URL: Documentation, https://github.com/espressif/esp-debug-backend/blob/master/README.md
 Project-URL: Changelog, https://github.com/espressif/esp-debug-backend/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
```

### Comparing `esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/SOURCES.txt` & `esp-debug-backend-1.0.3/src/esp_debug_backend.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 src/esp_debug_backend.egg-info/PKG-INFO
 src/esp_debug_backend.egg-info/SOURCES.txt
 src/esp_debug_backend.egg-info/dependency_links.txt
 src/esp_debug_backend.egg-info/requires.txt
 src/esp_debug_backend.egg-info/top_level.txt
 src/esp_debug_backend/hw_specific/__init__.py
 src/esp_debug_backend/hw_specific/esp.py
+src/esp_debug_backend/hw_specific/esp_init.gdb
 src/esp_debug_backend/hw_specific/riscv.py
 src/esp_debug_backend/hw_specific/xtensa.py
 tests/test_gdb.py
 tests/test_oocd.py
```

### Comparing `esp-debug-backend-1.0.2/tests/test_gdb.py` & `esp-debug-backend-1.0.3/tests/test_gdb.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.2/tests/test_oocd.py` & `esp-debug-backend-1.0.3/tests/test_oocd.py`

 * *Files identical despite different names*


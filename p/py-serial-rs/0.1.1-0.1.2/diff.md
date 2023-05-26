# Comparing `tmp/py_serial_rs-0.1.1.tar.gz` & `tmp/py_serial_rs-0.1.2.tar.gz`

## Comparing `py_serial_rs-0.1.1.tar` & `py_serial_rs-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000       88 2023-05-22 21:12:11.000000 py_serial_rs-0.1.1/.envrc
--rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.1/.github/workflows/rust.yml
--rw-r--r--   0     1000     1000      694 2023-05-25 20:55:00.000000 py_serial_rs-0.1.1/.gitignore
--rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.1/.readthedocs.yaml
--rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.1/LICENSE
--rw-r--r--   0     1000     1000     1580 2023-05-25 21:50:53.000000 py_serial_rs-0.1.1/Readme.rst
--rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.1/docs/Makefile
--rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.1/docs/make.bat
--rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.1/docs/source/conf.py
--rw-r--r--   0     1000     1000     1599 2023-05-25 21:50:53.000000 py_serial_rs-0.1.1/docs/source/index.rst
--rw-r--r--   0     1000     1000      374 2023-05-25 20:55:21.000000 py_serial_rs-0.1.1/pyproject.toml
--rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.1/python/demo.py
--rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.1/python/demo_threads.py
--rw-r--r--   0     1000     1000      166 2023-05-25 21:04:59.000000 py_serial_rs-0.1.1/requirements.txt
--rw-r--r--   0     1000     1000      392 2023-05-20 07:54:26.000000 py_serial_rs-0.1.1/shell.nix
--rw-r--r--   0     1000     1000     4699 2023-05-25 21:36:52.000000 py_serial_rs-0.1.1/src/lib.rs
--rw-r--r--   0     1000     1000    15416 2023-05-25 21:38:04.000000 py_serial_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      283 1970-01-01 00:00:00.000000 py_serial_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000       88 2023-05-22 21:12:11.000000 py_serial_rs-0.1.2/.envrc
+-rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.2/.github/workflows/rust.yml
+-rw-r--r--   0     1000     1000      694 2023-05-25 20:55:00.000000 py_serial_rs-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.2/.readthedocs.yaml
+-rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.2/LICENSE
+-rw-r--r--   0     1000     1000     1580 2023-05-25 21:50:53.000000 py_serial_rs-0.1.2/Readme.rst
+-rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.2/docs/Makefile
+-rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.2/docs/make.bat
+-rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.2/docs/source/conf.py
+-rw-r--r--   0     1000     1000     1599 2023-05-25 21:50:53.000000 py_serial_rs-0.1.2/docs/source/index.rst
+-rw-r--r--   0     1000     1000      794 2023-05-26 20:03:19.000000 py_serial_rs-0.1.2/pyproject.toml
+-rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.2/python/demo.py
+-rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.2/python/demo_threads.py
+-rw-r--r--   0     1000     1000      166 2023-05-25 21:04:59.000000 py_serial_rs-0.1.2/requirements.txt
+-rw-r--r--   0     1000     1000      392 2023-05-20 07:54:26.000000 py_serial_rs-0.1.2/shell.nix
+-rw-r--r--   0     1000     1000     4699 2023-05-25 21:36:52.000000 py_serial_rs-0.1.2/src/lib.rs
+-rw-r--r--   0     1000     1000    15416 2023-05-26 20:09:17.000000 py_serial_rs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 py_serial_rs-0.1.2/PKG-INFO
```

### Comparing `py_serial_rs-0.1.1/.gitignore` & `py_serial_rs-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/.readthedocs.yaml` & `py_serial_rs-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/LICENSE` & `py_serial_rs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/Readme.rst` & `py_serial_rs-0.1.2/Readme.rst`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/docs/Makefile` & `py_serial_rs-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/docs/make.bat` & `py_serial_rs-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/docs/source/conf.py` & `py_serial_rs-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/docs/source/index.rst` & `py_serial_rs-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/python/demo.py` & `py_serial_rs-0.1.2/python/demo.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/python/demo_threads.py` & `py_serial_rs-0.1.2/python/demo_threads.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/src/lib.rs` & `py_serial_rs-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.1/Cargo.lock` & `py_serial_rs-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_serial_rs"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "clippy",
  "pyo3",
  "serialport",
  "time",
 ]
```


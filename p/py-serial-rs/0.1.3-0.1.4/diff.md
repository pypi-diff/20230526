# Comparing `tmp/py_serial_rs-0.1.3.tar.gz` & `tmp/py_serial_rs-0.1.4.tar.gz`

## Comparing `py_serial_rs-0.1.3.tar` & `py_serial_rs-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.3/Cargo.toml
--rw-r--r--   0     1000     1000       88 2023-05-22 21:12:11.000000 py_serial_rs-0.1.3/.envrc
--rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.3/.github/workflows/rust.yml
--rw-r--r--   0     1000     1000      694 2023-05-25 20:55:00.000000 py_serial_rs-0.1.3/.gitignore
--rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.3/.readthedocs.yaml
--rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.3/LICENSE
--rw-r--r--   0     1000     1000     1580 2023-05-25 21:50:53.000000 py_serial_rs-0.1.3/Readme.rst
--rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.3/docs/Makefile
--rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.3/docs/make.bat
--rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.3/docs/source/conf.py
--rw-r--r--   0     1000     1000     1599 2023-05-25 21:50:53.000000 py_serial_rs-0.1.3/docs/source/index.rst
--rw-r--r--   0     1000     1000      713 2023-05-26 20:14:42.000000 py_serial_rs-0.1.3/pyproject.toml
--rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.3/python/demo.py
--rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.3/python/demo_threads.py
--rw-r--r--   0     1000     1000      166 2023-05-25 21:04:59.000000 py_serial_rs-0.1.3/requirements.txt
--rw-r--r--   0     1000     1000      392 2023-05-20 07:54:26.000000 py_serial_rs-0.1.3/shell.nix
--rw-r--r--   0     1000     1000     4699 2023-05-25 21:36:52.000000 py_serial_rs-0.1.3/src/lib.rs
--rw-r--r--   0     1000     1000    15416 2023-05-26 20:14:47.000000 py_serial_rs-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     2185 1970-01-01 00:00:00.000000 py_serial_rs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.4/Cargo.toml
+-rw-r--r--   0     1000     1000       88 2023-05-22 21:12:11.000000 py_serial_rs-0.1.4/.envrc
+-rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/.github/workflows/rust.yml
+-rw-r--r--   0     1000     1000      694 2023-05-25 20:55:00.000000 py_serial_rs-0.1.4/.gitignore
+-rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.4/.readthedocs.yaml
+-rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/LICENSE
+-rw-r--r--   0     1000     1000     1573 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/Readme.rst
+-rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.4/docs/Makefile
+-rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.4/docs/make.bat
+-rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.4/docs/source/conf.py
+-rw-r--r--   0     1000     1000     1592 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/docs/source/index.rst
+-rw-r--r--   0     1000     1000      771 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/pyproject.toml
+-rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.4/python/demo.py
+-rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.4/python/demo_threads.py
+-rw-r--r--   0     1000     1000      166 2023-05-25 21:04:59.000000 py_serial_rs-0.1.4/requirements.txt
+-rw-r--r--   0     1000     1000      392 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/shell.nix
+-rw-r--r--   0     1000     1000     4699 2023-05-25 21:36:52.000000 py_serial_rs-0.1.4/src/lib.rs
+-rw-r--r--   0     1000     1000    15416 2023-05-26 20:20:34.000000 py_serial_rs-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 py_serial_rs-0.1.4/PKG-INFO
```

### Comparing `py_serial_rs-0.1.3/.gitignore` & `py_serial_rs-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/.readthedocs.yaml` & `py_serial_rs-0.1.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/LICENSE` & `py_serial_rs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/Readme.rst` & `py_serial_rs-0.1.4/Readme.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
    contain the root `toctree` directive.
 
 py_serial_rs
 ========================================
 
 The goal of this package is to provide a fast and reliable interface to the serial ports.
 
-Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_
-crate written for Rust. This package supports threading.
+Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_ written in Rust. This package supports threading.
 
 
 ========================================
 Installation
 ========================================
 `PyO3 <https://pyo3.rs/v0.18.3/>`_ (with maturin) will build a pip package for you. For this, make
 sure that you are able to build rust packages with `cargo`. Create a virtual environment
```

### Comparing `py_serial_rs-0.1.3/docs/Makefile` & `py_serial_rs-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/docs/make.bat` & `py_serial_rs-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/docs/source/conf.py` & `py_serial_rs-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/docs/source/index.rst` & `py_serial_rs-0.1.4/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
    contain the root `toctree` directive.
 
 py_serial_rs
 ========================================
 
 The goal of this package is to provide a fast and reliable interface to the serial ports.
 
-Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_
-crate written for Rust. This package supports threading.
+Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_ written in Rust. This package supports threading.
 
 
 ========================================
 Installation
 ========================================
 `PyO3 <https://pyo3.rs/v0.18.3/>`_ (with maturin) will build a pip package for you. For this, make
 sure that you are able to build rust packages with `cargo`. Create a virtual environment
```

### Comparing `py_serial_rs-0.1.3/pyproject.toml` & `py_serial_rs-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "py_serial_rs"
 requires-python = ">=3.8"
+description = "Read and write data over the serial ports"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 readme = "Readme.rst"
 authors = [
```

### Comparing `py_serial_rs-0.1.3/python/demo.py` & `py_serial_rs-0.1.4/python/demo.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/python/demo_threads.py` & `py_serial_rs-0.1.4/python/demo_threads.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/src/lib.rs` & `py_serial_rs-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.3/Cargo.lock` & `py_serial_rs-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_serial_rs"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "clippy",
  "pyo3",
  "serialport",
  "time",
 ]
```

### Comparing `py_serial_rs-0.1.3/PKG-INFO` & `py_serial_rs-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: py_serial_rs
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
+Summary: Read and write data over the serial ports
 Author: Jürgen Hahn
 Author-email: mail.jhahn@googlemail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 Project-URL: Source Code, https://github.com/jrhahn/py_serial_rs
 Project-URL: Issues, https://github.com/jrhahn/py_serial_rs/issues
 Project-URL: Documentation, https://py-serial-rs.readthedocs.io/en/latest/
@@ -19,16 +20,15 @@
    contain the root `toctree` directive.
 
 py_serial_rs
 ========================================
 
 The goal of this package is to provide a fast and reliable interface to the serial ports.
 
-Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_
-crate written for Rust. This package supports threading.
+Instead of implementing the logic in Python, this package builds around `serialport <https://docs.rs/serialport/latest/serialport/>`_ written in Rust. This package supports threading.
 
 
 ========================================
 Installation
 ========================================
 `PyO3 <https://pyo3.rs/v0.18.3/>`_ (with maturin) will build a pip package for you. For this, make
 sure that you are able to build rust packages with `cargo`. Create a virtual environment
```


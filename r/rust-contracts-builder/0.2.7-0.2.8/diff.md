# Comparing `tmp/rust-contracts-builder-0.2.7.tar.gz` & `tmp/rust-contracts-builder-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rust-contracts-builder-0.2.7.tar", last modified: Wed May 24 11:17:29 2023, max compression
+gzip compressed data, was "rust-contracts-builder-0.2.8.tar", last modified: Fri May 26 01:44:15 2023, max compression
```

## Comparing `rust-contracts-builder-0.2.7.tar` & `rust-contracts-builder-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.252622 rust-contracts-builder-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 11:17:29.252622 rust-contracts-builder-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.248622 rust-contracts-builder-0.2.7/pysrc/
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.248622 rust-contracts-builder-0.2.7/pysrc/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.248622 rust-contracts-builder-0.2.7/pysrc/templates/abigen/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/abigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/abigen/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.248622 rust-contracts-builder-0.2.7/pysrc/templates/init/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/_Cargo.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/templates/init/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/pysrc/wasm_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:17:29.252622 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 11:17:29.000000 rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 11:17:29.252622 rust-contracts-builder-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-24 11:17:16.000000 rust-contracts-builder-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.705428 rust-contracts-builder-0.2.8/pysrc/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/templates/abigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/abigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/abigen/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/pysrc/templates/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/_Cargo.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/templates/init/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/pysrc/wasm_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 01:44:15.000000 rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 01:44:15.709428 rust-contracts-builder-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 01:44:01.000000 rust-contracts-builder-0.2.8/setup.py
```

### Comparing `rust-contracts-builder-0.2.7/LICENSE` & `rust-contracts-builder-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.7/pysrc/__init__.py` & `rust-contracts-builder-0.2.8/pysrc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import tempfile
 import toml
 import shutil
 import argparse
 from .wasm_checker import check_import_section
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 src_dir = os.path.dirname(__file__).replace('\\', '/')
 
 
 #https://stackabuse.com/how-to-print-colored-text-in-python/
 #https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal
 HEADER = '\033[95m'
@@ -131,15 +131,15 @@
 
     if result.subparser == "init":
         project_name = result.project_name
         with open(f'{src_dir}/templates/init/_Cargo.toml', 'r') as f:
             cargo_toml = f.read().replace('{{name}}', project_name)
 
         files = {}
-        for file_name in ['_Cargo.toml', '.gitignore', 'build.sh', 'lib.rs', 'test.py', 'test.sh']:
+        for file_name in ['_Cargo.toml', '.gitignore', 'build.sh', 'lib.rs', 'test.py', 'test.sh', 'pytest.ini']:
             with open(f'{src_dir}/templates/init/{file_name}', 'r') as f:
                 if file_name == '_Cargo.toml':
                     file_name = 'Cargo.toml'
                 files[file_name] = f.read().replace('{{name}}', project_name)
         try:
             os.mkdir(project_name)
             for file in files:
```

### Comparing `rust-contracts-builder-0.2.7/pysrc/templates/init/lib.rs` & `rust-contracts-builder-0.2.8/pysrc/templates/init/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #![cfg_attr(not(feature = "std"), no_std)]
+#![cfg_attr(feature = "std", allow(warnings))]
 
 #[rust_chain::contract]
 #[allow(dead_code)]
 mod {{name}} {
     use rust_chain::{
         Name,
         chain_println,
```

### Comparing `rust-contracts-builder-0.2.7/pysrc/templates/init/test.py` & `rust-contracts-builder-0.2.8/pysrc/templates/init/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,7 +73,8 @@
     r = tester.push_action('hello', 'inc', args, {'hello': 'active'})
     logger.info('++++++elapsed: %s', r['elapsed'])
     tester.produce_block()
 
     r = tester.push_action('hello', 'inc', args, {'hello': 'active'})
     logger.info('++++++elapsed: %s', r['elapsed'])
     tester.produce_block()
+    logger.info("+++++++test done!")
```

### Comparing `rust-contracts-builder-0.2.7/pysrc/wasm_checker.py` & `rust-contracts-builder-0.2.8/pysrc/wasm_checker.py`

 * *Files identical despite different names*

### Comparing `rust-contracts-builder-0.2.7/rust_contracts_builder.egg-info/SOURCES.txt` & `rust-contracts-builder-0.2.8/rust_contracts_builder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pysrc/wasm_checker.py
 pysrc/templates/abigen/Cargo.toml
 pysrc/templates/abigen/main.rs
 pysrc/templates/init/.gitignore
 pysrc/templates/init/_Cargo.toml
 pysrc/templates/init/build.sh
 pysrc/templates/init/lib.rs
+pysrc/templates/init/pytest.ini
 pysrc/templates/init/test.py
 pysrc/templates/init/test.sh
 rust_contracts_builder.egg-info/PKG-INFO
 rust_contracts_builder.egg-info/SOURCES.txt
 rust_contracts_builder.egg-info/dependency_links.txt
 rust_contracts_builder.egg-info/entry_points.txt
 rust_contracts_builder.egg-info/requires.txt
```

### Comparing `rust-contracts-builder-0.2.7/setup.py` & `rust-contracts-builder-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for f in files:
         release_files.append(os.path.join(root.replace('pysrc/', ''), f))    
 
 # print(release_files)
 
 setup(
     name="rust-contracts-builder",
-    version="0.2.7",
+    version="0.2.8",
     description="Rust Contracts Builder",
     author='The UUOSIO Team',
     license="Apache 2.0",
     url="https://github.com/uuosio/rust-contracts-builder",
     packages=['rust_contracts_builder'],
     package_dir={'rust_contracts_builder': 'pysrc'},
     package_data={
```


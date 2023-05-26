# Comparing `tmp/lib_dzne_auto_interface-0.1.1.tar.gz` & `tmp/lib-dzne-auto-interface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_dzne_auto_interface-0.1.1.tar", last modified: Sat Feb 18 09:08:43 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.2.0.tar", last modified: Fri May 26 20:42:20 2023, max compression
```

## Comparing `lib_dzne_auto_interface-0.1.1.tar` & `lib-dzne-auto-interface-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-18 09:08:43.590281 lib_dzne_auto_interface-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-17 18:31:21.000000 lib_dzne_auto_interface-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1536 2023-02-18 09:08:43.590281 lib_dzne_auto_interface-0.1.1/PKG-INFO
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-18 09:08:43.590281 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)     1637 2023-02-17 21:48:39.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface/ExecFunc.py
--rw-rw-r--   0 base      (1001) base      (1001)        0 2023-02-18 07:45:42.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     3958 2023-02-17 22:02:40.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface/cli.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-18 09:08:43.590281 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1536 2023-02-18 09:08:43.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      323 2023-02-18 09:08:43.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-18 09:08:43.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-02-18 09:08:43.000000 lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/top_level.txt
--rw-r--r--   0 base      (1001) base      (1001)      545 2023-02-18 09:08:33.000000 lib_dzne_auto_interface-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-18 09:08:43.590281 lib_dzne_auto_interface-0.1.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1538 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-25 04:55:40.000000 lib-dzne-auto-interface-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.121648 lib-dzne-auto-interface-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)     8390 2023-05-26 20:40:19.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1538 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      276 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib_dzne_auto_interface-0.1.1/LICENSE` & `lib-dzne-auto-interface-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_dzne_auto_interface-0.1.1/PKG-INFO` & `lib-dzne-auto-interface-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: lib_dzne_auto_interface
-Version: 0.1.1
-Summary: Libary for automatically created intefaces.
+Name: lib-dzne-auto-interface
+Version: 0.2.0
+Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib_dzne_auto_interface-0.1.1/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.1.1
-Summary: Libary for automatically created intefaces.
+Version: 0.2.0
+Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib_dzne_auto_interface-0.1.1/pyproject.toml` & `lib-dzne-auto-interface-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
-name = "lib_dzne_auto_interface"
-version = "0.1.1"
-description = "Libary for automatically created intefaces."
+name = "lib-dzne-auto-interface"
+version = "0.2.0"
+description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```


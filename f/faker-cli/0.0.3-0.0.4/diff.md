# Comparing `tmp/faker_cli-0.0.3.tar.gz` & `tmp/faker_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.0.3.tar", max compression
+gzip compressed data, was "faker_cli-0.0.4.tar", max compression
```

## Comparing `faker_cli-0.0.3.tar` & `faker_cli-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-25 21:52:14.055729 faker_cli-0.0.3/LICENSE
--rw-r--r--   0        0        0     2852 2023-05-25 21:52:14.055729 faker_cli-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-25 21:52:14.055729 faker_cli-0.0.3/faker_cli/__init__.py
--rw-r--r--   0        0        0     2024 2023-05-25 21:52:14.055729 faker_cli-0.0.3/faker_cli/cli.py
--rw-r--r--   0        0        0    14139 2023-05-25 21:52:14.055729 faker_cli-0.0.3/faker_cli/templates.py
--rw-r--r--   0        0        0      809 2023-05-25 21:52:14.055729 faker_cli-0.0.3/faker_cli/writer.py
--rw-r--r--   0        0        0      481 2023-05-25 21:52:33.563915 faker_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 faker_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-25 22:00:32.729052 faker_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2852 2023-05-25 22:00:32.729052 faker_cli-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/__init__.py
+-rw-r--r--   0        0        0     2024 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/cli.py
+-rw-r--r--   0        0        0    14139 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/templates.py
+-rw-r--r--   0        0        0      809 2023-05-25 22:00:32.729052 faker_cli-0.0.4/faker_cli/writer.py
+-rw-r--r--   0        0        0      461 2023-05-25 22:00:52.493226 faker_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 faker_cli-0.0.4/PKG-INFO
```

### Comparing `faker_cli-0.0.3/LICENSE` & `faker_cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.3/README.md` & `faker_cli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.3/faker_cli/cli.py` & `faker_cli-0.0.4/faker_cli/cli.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.3/faker_cli/templates.py` & `faker_cli-0.0.4/faker_cli/templates.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.3/faker_cli/writer.py` & `faker_cli-0.0.4/faker_cli/writer.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.0.3/PKG-INFO` & `faker_cli-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: faker (>=18.9.0,<19.0.0)
-Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 # Faker CLI
 
 Faker is an awesome Python library, but I often just want a simple command I can run to generate data in a variety of formats.
 
 With Faker CLI, you can easily generate CSV or JSON data with fields of your choosing.
```


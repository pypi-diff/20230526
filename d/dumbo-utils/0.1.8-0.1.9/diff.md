# Comparing `tmp/dumbo_utils-0.1.8.tar.gz` & `tmp/dumbo_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_utils-0.1.8.tar", max compression
+gzip compressed data, was "dumbo_utils-0.1.9.tar", max compression
```

## Comparing `dumbo_utils-0.1.8.tar` & `dumbo_utils-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-01-17 15:00:05.226957 dumbo_utils-0.1.8/LICENSE
--rw-r--r--   0        0        0      176 2023-02-17 13:32:21.052107 dumbo_utils-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-01-17 14:30:53.103251 dumbo_utils-0.1.8/dumbo_utils/__init__.py
--rw-r--r--   0        0        0      396 2023-01-25 11:31:11.894094 dumbo_utils-0.1.8/dumbo_utils/console.py
--rw-r--r--   0        0        0     6678 2023-01-25 11:34:14.062908 dumbo_utils-0.1.8/dumbo_utils/primitives.py
--rw-r--r--   0        0        0      889 2023-01-18 12:09:49.139316 dumbo_utils-0.1.8/dumbo_utils/validation.py
--rw-r--r--   0        0        0      527 2023-02-17 13:33:54.248164 dumbo_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 dumbo_utils-0.1.8/setup.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 dumbo_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-17 15:00:05.226957 dumbo_utils-0.1.9/LICENSE
+-rw-r--r--   0        0        0      176 2023-02-17 13:32:21.052107 dumbo_utils-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-01-17 14:30:53.103251 dumbo_utils-0.1.9/dumbo_utils/__init__.py
+-rw-r--r--   0        0        0      396 2023-01-25 11:31:11.894094 dumbo_utils-0.1.9/dumbo_utils/console.py
+-rw-r--r--   0        0        0     6678 2023-01-25 11:34:14.062908 dumbo_utils-0.1.9/dumbo_utils/primitives.py
+-rw-r--r--   0        0        0      286 2023-05-26 17:30:30.582066 dumbo_utils-0.1.9/dumbo_utils/url.py
+-rw-r--r--   0        0        0      889 2023-01-18 12:09:49.139316 dumbo_utils-0.1.9/dumbo_utils/validation.py
+-rw-r--r--   0        0        0      532 2023-05-26 17:45:17.008968 dumbo_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 dumbo_utils-0.1.9/setup.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 dumbo_utils-0.1.9/PKG-INFO
```

### Comparing `dumbo_utils-0.1.8/LICENSE` & `dumbo_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.1.8/dumbo_utils/primitives.py` & `dumbo_utils-0.1.9/dumbo_utils/primitives.py`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.1.8/dumbo_utils/validation.py` & `dumbo_utils-0.1.9/dumbo_utils/validation.py`

 * *Files identical despite different names*

### Comparing `dumbo_utils-0.1.8/pyproject.toml` & `dumbo_utils-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dumbo-utils"
-version = "0.1.8"
+version = "0.1.9"
 description = "Different utilities to be reused in other projects"
 authors = ["Mario Alviano <mario.alviano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dumbo_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.3.1"
-typer = "^0.7.0"
-typeguard = "^2.13.3"
+typer = "^0.9.0"
+typeguard = "^4.0.0"
 valid8 = "^5.1.2"
 distlib = "^0.3.6"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 coverage = "^7.1.0"
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dumbo_utils-0.1.8/setup.py` & `dumbo_utils-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['distlib>=0.3.6,<0.4.0',
  'rich>=13.3.1,<14.0.0',
- 'typeguard>=2.13.3,<3.0.0',
- 'typer>=0.7.0,<0.8.0',
+ 'typeguard>=4.0.0,<5.0.0',
+ 'typer>=0.9.0,<0.10.0',
  'valid8>=5.1.2,<6.0.0']
 
 setup_kwargs = {
     'name': 'dumbo-utils',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Different utilities to be reused in other projects',
     'long_description': '# dumbo-utils\n\nDifferent utilities to be reused in other projects\n\n\n# Prerequisites\n\n- Python 3.10+\n\n\n\n## Install\n\nAdd to your project with\n```bash\n$ poetry add dumbo-utils\n```',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dumbo_utils-0.1.8/PKG-INFO` & `dumbo_utils-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: dumbo-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: Different utilities to be reused in other projects
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: distlib (>=0.3.6,<0.4.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typeguard (>=4.0.0,<5.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: valid8 (>=5.1.2,<6.0.0)
 Description-Content-Type: text/markdown
 
 # dumbo-utils
 
 Different utilities to be reused in other projects
```


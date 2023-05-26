# Comparing `tmp/aws_lambda_layer-0.2.1.tar.gz` & `tmp/aws_lambda_layer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_layer-0.2.1.tar", last modified: Fri May 26 18:39:01 2023, max compression
+gzip compressed data, was "aws_lambda_layer-0.2.2.tar", last modified: Fri May 26 19:45:00 2023, max compression
```

## Comparing `aws_lambda_layer-0.2.1.tar` & `aws_lambda_layer-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592960 aws_lambda_layer-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 18:39:01.592814 aws_lambda_layer-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.591781 aws_lambda_layer-0.2.1/aws_lambda_layer/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 18:18:38.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11528 2023-05-26 18:36:16.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11700 2023-05-26 18:37:31.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/source.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1423 2023-05-26 17:56:52.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592433 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      569 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 16:01:05.000000 aws_lambda_layer-0.2.1/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     1531 2023-05-26 18:30:26.000000 aws_lambda_layer-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 18:39:01.592998 aws_lambda_layer-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592550 aws_lambda_layer-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670659 aws_lambda_layer-0.2.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 19:45:00.670526 aws_lambda_layer-0.2.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.669558 aws_lambda_layer-0.2.2/aws_lambda_layer/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 19:42:01.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11528 2023-05-26 18:36:16.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11700 2023-05-26 18:37:31.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/source.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1459 2023-05-26 19:44:02.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670112 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      589 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 19:42:07.000000 aws_lambda_layer-0.2.2/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1740 2023-05-26 19:44:42.000000 aws_lambda_layer-0.2.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 19:45:00.670697 aws_lambda_layer-0.2.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670362 aws_lambda_layer-0.2.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-05-26 19:43:53.000000 aws_lambda_layer-0.2.2/tests/test_utils.py
```

### Comparing `aws_lambda_layer-0.2.1/LICENSE.txt` & `aws_lambda_layer-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/PKG-INFO` & `aws_lambda_layer-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_lambda_layer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.1/README.rst` & `aws_lambda_layer-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer/build_dist.py` & `aws_lambda_layer-0.2.2/aws_lambda_layer/build_dist.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer/context.py` & `aws_lambda_layer-0.2.2/aws_lambda_layer/context.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer/layer.py` & `aws_lambda_layer-0.2.2/aws_lambda_layer/layer.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer/source.py` & `aws_lambda_layer-0.2.2/aws_lambda_layer/source.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer/utils.py` & `aws_lambda_layer-0.2.2/aws_lambda_layer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     in a sorted order, which is deterministic.
     """
     hashes = list()
 
     for path in paths:
         if path.is_dir():
             for p in sorted(path.glob("**/*"), key=lambda x: str(x)):
-                hashes.append(sha256_of_bytes(p.read_bytes()))
+                if p.is_file():
+                    hashes.append(sha256_of_bytes(p.read_bytes()))
         elif path.is_file():
             hashes.append(sha256_of_bytes(path.read_bytes()))
         else:
             pass
     return sha256_of_bytes("".join(hashes).encode("utf-8"))
```

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/PKG-INFO` & `aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-lambda-layer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/SOURCES.txt` & `aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 aws_lambda_layer/source.py
 aws_lambda_layer/utils.py
 aws_lambda_layer.egg-info/PKG-INFO
 aws_lambda_layer.egg-info/SOURCES.txt
 aws_lambda_layer.egg-info/dependency_links.txt
 aws_lambda_layer.egg-info/requires.txt
 aws_lambda_layer.egg-info/top_level.txt
-tests/test_import.py
+tests/test_import.py
+tests/test_utils.py
```

### Comparing `aws_lambda_layer-0.2.1/pyproject.toml` & `aws_lambda_layer-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_layer"
-version = "0.1.1"
+version = "0.2.2"
 description = "A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts."
 authors = ["Sanhe Hu <husanhe@gmail.com>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 boto3 = "*"
```

### Comparing `aws_lambda_layer-0.2.1/release-history.rst` & `aws_lambda_layer-0.2.2/release-history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.2 (2023-05-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that ``aws_lambda_layer.api.sha256_of_paths`` forget to ignore dir in calculation.
+
+
 0.2.1 (2023-05-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - the ``build_source_artifacts`` and ``publish_source_artifacts`` now has four options to build the source artifacts:
     - use ``python setup.py``
     - use ``python -m build ...``
```

### Comparing `aws_lambda_layer-0.2.1/setup.py` & `aws_lambda_layer-0.2.2/setup.py`

 * *Files identical despite different names*


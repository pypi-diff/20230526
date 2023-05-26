# Comparing `tmp/aws_lambda_layer-0.1.1.tar.gz` & `tmp/aws_lambda_layer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_layer-0.1.1.tar", last modified: Tue May 16 02:14:02 2023, max compression
+gzip compressed data, was "aws_lambda_layer-0.2.1.tar", last modified: Fri May 26 18:39:01 2023, max compression
```

## Comparing `aws_lambda_layer-0.1.1.tar` & `aws_lambda_layer-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-16 02:14:02.781001 aws_lambda_layer-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3995 2023-05-16 02:14:02.780867 aws_lambda_layer-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2874 2023-05-16 02:13:46.000000 aws_lambda_layer-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-16 02:14:02.779749 aws_lambda_layer-0.1.1/aws_lambda_layer/
--rw-r--r--   0 sanhehu    (501) staff       (20)      261 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-15 21:15:55.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      359 2023-05-16 01:07:12.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3892 2023-05-16 00:41:11.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11178 2023-05-16 01:10:16.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5447 2023-05-16 01:06:33.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/source.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      640 2023-05-16 00:56:15.000000 aws_lambda_layer-0.1.1/aws_lambda_layer/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-16 02:14:02.780529 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3995 2023-05-16 02:14:02.000000 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      523 2023-05-16 02:14:02.000000 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-16 02:14:02.000000 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-05-16 02:14:02.000000 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-16 02:14:02.000000 aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      608 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-16 02:14:02.781043 aws_lambda_layer-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7711 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-16 02:14:02.780653 aws_lambda_layer-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.1.1/tests/test_import.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592960 aws_lambda_layer-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 18:39:01.592814 aws_lambda_layer-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.591781 aws_lambda_layer-0.2.1/aws_lambda_layer/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 18:18:38.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11528 2023-05-26 18:36:16.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11700 2023-05-26 18:37:31.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/source.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1423 2023-05-26 17:56:52.000000 aws_lambda_layer-0.2.1/aws_lambda_layer/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592433 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      569 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 18:39:01.000000 aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 16:01:05.000000 aws_lambda_layer-0.2.1/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1531 2023-05-26 18:30:26.000000 aws_lambda_layer-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 18:39:01.592998 aws_lambda_layer-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 18:39:01.592550 aws_lambda_layer-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.1/tests/test_import.py
```

### Comparing `aws_lambda_layer-0.1.1/LICENSE.txt` & `aws_lambda_layer-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.1.1/PKG-INFO` & `aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aws_lambda_layer
-Version: 0.1.1
-Summary: Package short description.
+Name: aws-lambda-layer
+Version: 0.2.1
+Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
@@ -85,14 +84,19 @@
 A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts. It utilizes a purposefully designed S3 folder structure to store all historical versions of artifacts.
 
 Examples:
 
 - `build_layer.py <./example/build_layer.py>`_
 - `build_source.py <./example/build_source.py>`_
 
+You may need additional tools to build your source artifacts:
+
+- do ``pip install build`` to use ``python -m build``
+- do ``pip install poetry`` to use ``poetry build``
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``aws_lambda_layer`` is released on PyPI, so all you need is:
```

### Comparing `aws_lambda_layer-0.1.1/README.rst` & `aws_lambda_layer-0.2.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,19 @@
 A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts. It utilizes a purposefully designed S3 folder structure to store all historical versions of artifacts.
 
 Examples:
 
 - `build_layer.py <./example/build_layer.py>`_
 - `build_source.py <./example/build_source.py>`_
 
+You may need additional tools to build your source artifacts:
+
+- do ``pip install build`` to use ``python -m build``
+- do ``pip install poetry`` to use ``poetry build``
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``aws_lambda_layer`` is released on PyPI, so all you need is:
@@ -69,8 +74,8 @@
 
     $ pip install aws_lambda_layer
 
 To upgrade to latest version:
 
 .. code-block:: console
 
-    $ pip install --upgrade aws_lambda_layer
+    $ pip install --upgrade aws_lambda_layer
```

### Comparing `aws_lambda_layer-0.1.1/aws_lambda_layer/context.py` & `aws_lambda_layer-0.2.1/aws_lambda_layer/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 # -*- coding: utf-8 -*-
 
+"""
+This module defines the Lambda artifacts build context.
+"""
+
 import typing as T
 import dataclasses
 from pathlib import Path
 from s3pathlib import S3Path
 
 ZFILL = 6
 
 
 @dataclasses.dataclass
 class BuildContext:
+    """
+    This object defines where the lambda artifacts should locate at on local
+    laptop and on S3 bucket.
+
+    :param dir_build: the root directory of the build folder on local
+    :param s3dir_lambda: the root directory of the lambda artifacts on S3
+    """
+
     dir_build: T.Optional[Path] = dataclasses.field(default=None)
     s3dir_lambda: T.Optional[S3Path] = dataclasses.field(default=None)
 
     @classmethod
     def new(
         cls,
         dir_build: T.Optional[T.Union[str, Path]] = None,
@@ -34,15 +46,14 @@
         """
         return self.dir_build.joinpath("python")
 
     @property
     def dir_deploy(self) -> Path:
         return self.dir_build.joinpath("deploy")
 
-
     @property
     def path_source_zip(self) -> Path:
         """
         This file will be the Lambda source code zip file.
 
         example: ``${dir_build}/source.zip``
         """
```

### Comparing `aws_lambda_layer-0.1.1/aws_lambda_layer/layer.py` & `aws_lambda_layer-0.2.1/aws_lambda_layer/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         "install",
         "-r",
         f"{path_requirements}",
         "-t",
         f"{build_context.dir_python}",
     ]
     if quiet:
+        args.append("--disable-pip-version-check")
         args.append("--quiet")
     subprocess.run(args, check=True)
 
     # zip the layer file
     # some packages are pre-installed in AWS Lambda runtime, so we don't need to
     # add them to the layer
     ignore_package_list = [
@@ -281,14 +282,19 @@
 
     - :func:`get_latest_layer_version`
     - :func:`is_current_layer_the_same_as_latest_one`
     - :func:`build_layer_artifacts`
     - :func:`upload_layer_artifacts`
     - :func:`publish_layer`
 
+    This function uses requirements.txt file to determine the dependencies.
+    If you use poetry, pdm, pipenv or any other dependency management tool,
+    you should export your dependencies to requirements.txt file first.
+    I recommend poetry because the layer is supposed to be deterministic.
+
     :param bsm: boto session manager object
     :param layer_name: the lambda layer name
     :param python_version: example: ``["python3.8",]``
     :param path_requirements: example: ``/path/to/requirements.txt``
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
     :param bin_pip: example: ``/path/to/.venv/bin/pip``
```

### Comparing `aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/PKG-INFO` & `aws_lambda_layer-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: aws-lambda-layer
-Version: 0.1.1
-Summary: Package short description.
+Name: aws_lambda_layer
+Version: 0.2.1
+Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
@@ -15,15 +15,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: tests
 Provides-Extra: docs
@@ -85,14 +84,19 @@
 A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts. It utilizes a purposefully designed S3 folder structure to store all historical versions of artifacts.
 
 Examples:
 
 - `build_layer.py <./example/build_layer.py>`_
 - `build_source.py <./example/build_source.py>`_
 
+You may need additional tools to build your source artifacts:
+
+- do ``pip install build`` to use ``python -m build``
+- do ``pip install poetry`` to use ``poetry build``
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``aws_lambda_layer`` is released on PyPI, so all you need is:
```

### Comparing `aws_lambda_layer-0.1.1/aws_lambda_layer.egg-info/SOURCES.txt` & `aws_lambda_layer-0.2.1/aws_lambda_layer.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 release-history.rst
 requirements-test.txt
 requirements.txt
 setup.py
 aws_lambda_layer/__init__.py
 aws_lambda_layer/_version.py
 aws_lambda_layer/api.py
+aws_lambda_layer/build_dist.py
 aws_lambda_layer/context.py
 aws_lambda_layer/layer.py
 aws_lambda_layer/source.py
 aws_lambda_layer/utils.py
 aws_lambda_layer.egg-info/PKG-INFO
 aws_lambda_layer.egg-info/SOURCES.txt
 aws_lambda_layer.egg-info/dependency_links.txt
```

### Comparing `aws_lambda_layer-0.1.1/setup.py` & `aws_lambda_layer-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ]
     """
```


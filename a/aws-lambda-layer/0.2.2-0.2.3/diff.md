# Comparing `tmp/aws_lambda_layer-0.2.2.tar.gz` & `tmp/aws_lambda_layer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_layer-0.2.2.tar", last modified: Fri May 26 19:45:00 2023, max compression
+gzip compressed data, was "aws_lambda_layer-0.2.3.tar", last modified: Fri May 26 20:20:26 2023, max compression
```

## Comparing `aws_lambda_layer-0.2.2.tar` & `aws_lambda_layer-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670659 aws_lambda_layer-0.2.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 19:45:00.670526 aws_lambda_layer-0.2.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.669558 aws_lambda_layer-0.2.2/aws_lambda_layer/
--rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 19:42:01.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/context.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11528 2023-05-26 18:36:16.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/layer.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    11700 2023-05-26 18:37:31.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/source.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1459 2023-05-26 19:44:02.000000 aws_lambda_layer-0.2.2/aws_lambda_layer/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670112 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      589 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 19:45:00.000000 aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 19:42:07.000000 aws_lambda_layer-0.2.2/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     1740 2023-05-26 19:44:42.000000 aws_lambda_layer-0.2.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 19:45:00.670697 aws_lambda_layer-0.2.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 19:45:00.670362 aws_lambda_layer-0.2.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.2/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-05-26 19:43:53.000000 aws_lambda_layer-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780949 aws_lambda_layer-0.2.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-05-13 04:31:27.000000 aws_lambda_layer-0.2.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 20:20:26.780815 aws_lambda_layer-0.2.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3045 2023-05-26 18:33:40.000000 aws_lambda_layer-0.2.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.779864 aws_lambda_layer-0.2.3/aws_lambda_layer/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      427 2023-05-26 15:58:40.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-26 20:19:05.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      395 2023-05-26 18:27:30.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-05-26 18:14:42.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/context.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12038 2023-05-26 20:17:18.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/layer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12529 2023-05-26 20:00:24.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/source.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1459 2023-05-26 19:44:02.000000 aws_lambda_layer-0.2.3/aws_lambda_layer/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780425 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4195 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      589 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      169 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       17 2023-05-26 20:20:26.000000 aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      989 2023-05-26 20:20:04.000000 aws_lambda_layer-0.2.3/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1949 2023-05-26 20:19:50.000000 aws_lambda_layer-0.2.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-05-16 01:23:43.000000 aws_lambda_layer-0.2.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-26 20:20:26.780990 aws_lambda_layer-0.2.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7662 2023-05-26 15:59:24.000000 aws_lambda_layer-0.2.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-26 20:20:26.780656 aws_lambda_layer-0.2.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      259 2023-05-12 19:08:25.000000 aws_lambda_layer-0.2.3/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      577 2023-05-26 19:43:53.000000 aws_lambda_layer-0.2.3/tests/test_utils.py
```

### Comparing `aws_lambda_layer-0.2.2/LICENSE.txt` & `aws_lambda_layer-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/PKG-INFO` & `aws_lambda_layer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws_lambda_layer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.2/README.rst` & `aws_lambda_layer-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer/build_dist.py` & `aws_lambda_layer-0.2.3/aws_lambda_layer/build_dist.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer/context.py` & `aws_lambda_layer-0.2.3/aws_lambda_layer/context.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer/layer.py` & `aws_lambda_layer-0.2.3/aws_lambda_layer/layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 
 def build_layer_artifacts(
     path_requirements: T.Union[str, Path],
     dir_build: T.Union[str, Path],
     bin_pip: T.Union[str, Path],
     quiet: bool = False,
-):
+) -> str:
     """
     This function builds the AWS Lambda layer artifacts based on the dependencies
     specified in the ``path_requirements``. It utilizes ``bin_pip`` to install
     the dependencies into the ``${dir_build}/python`` folder. Afterward,
     it compresses the ``${dir_build}/python`` folder into ``${dir_build}/layer.zip``.
 
     Please note that this function is intended to run in an Amazon Linux-like environment,
@@ -105,14 +105,16 @@
     also uses Amazon Linux. Building the layer on Windows or Mac may result in
     compatibility issues with certain C libraries.
 
     :param path_requirements: example: ``/path/to/requirements.txt``
     :param dir_build: example: ``/path/to/build/lambda``
     :param bin_pip: example: ``/path/to/.venv/bin/pip``
     :param quiet: whether you want to suppress the output of cli commands
+
+    :return: the layer content sha256
     """
     build_context = BuildContext.new(dir_build=dir_build)
     path_requirements = Path(path_requirements).absolute()
     bin_pip = Path(bin_pip).absolute()
 
     # remove existing artifacts and temp folder
     build_context.path_layer_zip.unlink(missing_ok=True)
@@ -160,49 +162,62 @@
     # the glob command and zip command depends on the current working directory
     with utils.temp_cwd(build_context.dir_build):
         args.extend(glob.glob("*"))
         args.append("-x")
         for package in ignore_package_list:
             args.append(f"python/{package}*")
         subprocess.run(args, check=True)
+    layer_sha256 = utils.sha256_of_bytes(path_requirements.read_bytes())
+    return layer_sha256
 
 
 def upload_layer_artifacts(
     bsm: "BotoSesManager",
     path_requirements: T.Union[str, Path],
+    layer_sha256: str,
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
+    metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
 ):
     """
     Upload the recently built Lambda layer artifact from ``${dir_build}/layer.zip``
     to a temporary S3 folder. If the creation of a new layer from the temporary location
     is successful, copy it to the final location for the layer artifacts.
 
     :param bsm: boto session manager object
     :param path_requirements: example: ``/path/to/requirements.txt``
+    :param layer_sha256: layer content sha256
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
+    :param metadata: S3 object metadata
     :param tags: S3 object tags
     """
     build_context = BuildContext.new(dir_build=dir_build, s3dir_lambda=s3dir_lambda)
     path_requirements = Path(path_requirements).absolute()
 
+    if metadata is NOTHING:
+        metadata = {}
+    metadata["layer_sha256"] = layer_sha256
+
     # upload layer.zip
     extra_args = {"ContentType": "application/zip"}
+    extra_args["Metadata"] = metadata
     if tags is not NOTHING:
         extra_args["Tagging"] = urlencode(tags)
     build_context.s3path_tmp_layer_zip.upload_file(
         build_context.path_layer_zip,
         overwrite=True,
         bsm=bsm,
         extra_args=extra_args,
     )
+
     # upload requirements.txt
     extra_args = {"ContentType": "text/plain"}
+    extra_args["Metadata"] = metadata
     if tags is not NOTHING:
         extra_args["Tagging"] = urlencode(tags)
     build_context.s3path_tmp_layer_requirements_txt.upload_file(
         path_requirements,
         overwrite=True,
         bsm=bsm,
         extra_args=extra_args,
@@ -211,25 +226,23 @@
 
 def publish_layer(
     bsm: "BotoSesManager",
     layer_name: str,
     python_versions: T.List[str],
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
-    tags: T.Optional[T.Dict[str, str]] = NOTHING,
 ) -> str:
     """
     Publish a new lambda layer version from AWS S3.
 
     :param bsm: boto session manager object
     :param layer_name: the lambda layer name
     :param python_version: example: ``["python3.8",]``
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
-    :param tags: S3 object tags
 
     :return: The published lambda layer version ARN
     """
     build_context = BuildContext.new(dir_build=dir_build, s3dir_lambda=s3dir_lambda)
     # publish new layer version from temp s3 location
     response = bsm.lambda_client.publish_layer_version(
         LayerName=layer_name,
@@ -250,34 +263,33 @@
         version=layer_version,
     )
 
     # copy from tmp to the final location
     # we don't overwrite existing layer artifacts
     build_context.s3path_tmp_layer_zip.copy_to(
         s3path_layer_zip,
-        tags=tags,
         overwrite=False,
     )
     build_context.s3path_tmp_layer_requirements_txt.copy_to(
         s3path_layer_requirements_txt,
-        tags=tags,
         overwrite=False,
     )
     return layer_version_arn
 
 
 def deploy_layer(
     bsm: "BotoSesManager",
     layer_name: str,
     python_versions: T.List[str],
     path_requirements: T.Union[str, Path],
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
     bin_pip: T.Union[str, Path],
     quiet: bool = False,
+    metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
 ) -> T.Optional[str]:
     """
     Assemble the following functions together to build and deploy a new
     Lambda layer version if necessary.
 
     - :func:`get_latest_layer_version`
@@ -295,14 +307,15 @@
     :param layer_name: the lambda layer name
     :param python_version: example: ``["python3.8",]``
     :param path_requirements: example: ``/path/to/requirements.txt``
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
     :param bin_pip: example: ``/path/to/.venv/bin/pip``
     :param quiet: whether you want to suppress the output of cli commands
+    :param metadata: S3 object metadata
     :param tags: S3 object tags
 
     :return: The published lambda layer version ARN. If returns None,
         then no deployment happened.
     """
     latest_layer_version = get_latest_layer_version(bsm=bsm, layer_name=layer_name)
 
@@ -310,30 +323,31 @@
         bsm=bsm,
         latest_layer_version=latest_layer_version,
         path_requirements=path_requirements,
         s3dir_lambda=s3dir_lambda,
     ):
         return None
 
-    build_layer_artifacts(
+    layer_sha256 = build_layer_artifacts(
         path_requirements=path_requirements,
         dir_build=dir_build,
         bin_pip=bin_pip,
         quiet=quiet,
     )
 
     upload_layer_artifacts(
         bsm=bsm,
         path_requirements=path_requirements,
+        layer_sha256=layer_sha256,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
+        metadata=metadata,
         tags=tags,
     )
 
     return publish_layer(
         bsm=bsm,
         layer_name=layer_name,
         python_versions=python_versions,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
-        tags=tags,
     )
```

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer/source.py` & `aws_lambda_layer-0.2.3/aws_lambda_layer/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     path_bin_python: T.Optional[T.Union[str, Path]] = None,
     path_bin_poetry: T.Optional[T.Union[str, Path]] = None,
     use_pip: bool = False,
     use_build: bool = False,
     use_poetry: bool = False,
     use_pathlib: bool = False,
     verbose: bool = True,
-) -> Path:
+) -> T.Tuple[str, Path]:
     """
     This function builds the source artifacts for the AWS Lambda deployment package.
 
     Given the ``path_setup_py_or_pyproject_toml`` path, this function will
     locate the directory where the ``python -m build``, ``pip install`` or ``poetry build``
     command should run, build the distribution package, and then copy the
     ``path_lambda_function`` to the deploy folder in the ``dir_build`` directory,
@@ -105,15 +105,16 @@
     :param path_bin_poetry: example ``/path/to/.venv/bin/poetry`` or the global ``poetry``
     :param use_pip: do you want to use pip to build your source?
     :param use_build: do you want to use python-build to build your source?
     :param use_poetry: do you want to use python-poetry to build your source?
     :param use_pathlib: do you want to use pathlib to build your source?
     :param verbose: whether you want to suppress the output of cli commands
 
-    :return: the ``/path/to/build/lambda/source.zip`` file
+    :return: tuple of two item, first one is the code sha256 hash of the source artifacts,
+        second one is the path to the source.zip file
     """
     # validate arguments
     utils.ensure_exact_one_true(
         [
             use_pip,
             use_build,
             use_poetry,
@@ -210,44 +211,51 @@
         args.append("-q")
 
     # has to cd to the deploy dir to run the glob command
     with utils.temp_cwd(build_context.dir_deploy):
         args.extend(glob.glob("*"))
         subprocess.run(args, check=True)
 
-    return build_context.path_source_zip
+    source_sha256 = utils.sha256_of_paths([build_context.dir_deploy])
+    path_source_zip = build_context.path_source_zip
+    return source_sha256, path_source_zip
 
 
 def upload_source_artifacts(
     bsm: "BotoSesManager",
     version: str,
+    source_sha256: str,
     dir_build: T.Union[str, Path],
     s3dir_lambda: T.Union[str, S3Path],
     metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
 ) -> S3Path:
     """
     Upload the recently built Lambda source artifact from ``${dir_build}/source.zip``
     to S3 folder.
 
     :param bsm: boto session manager object
-    :param version: example: ``"0.1.1"``
+    :param version: lambda source code version, example: ``"0.1.1"``
+    :param source_sha256: sha256 hash of the source artifacts
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
+    :param metadata: S3 object metadata
     :param tags: S3 object tags
 
     :return: the S3 path of the uploaded ``source.zip`` file
     """
     build_context = BuildContext.new(dir_build=dir_build, s3dir_lambda=s3dir_lambda)
     s3dir_source = build_context.get_s3dir_source(version=version)
     s3path_source_zip = s3dir_source.joinpath("source.zip")
     # upload source.zip
     extra_args = {"ContentType": "application/zip"}
-    if metadata is not NOTHING:
-        extra_args["Metadata"] = metadata
+    if metadata is NOTHING:
+        metadata = {}
+    metadata["source_sha256"] = source_sha256
+    extra_args["Metadata"] = metadata
     if tags is not NOTHING:
         extra_args["Tagging"] = urlencode(tags)
     s3path_source_zip.upload_file(
         path=build_context.path_source_zip,
         overwrite=True,
         bsm=bsm,
         extra_args=extra_args,
@@ -268,15 +276,15 @@
     metadata: T.Optional[T.Dict[str, str]] = NOTHING,
     tags: T.Optional[T.Dict[str, str]] = NOTHING,
     use_pip: bool = False,
     use_build: bool = False,
     use_poetry: bool = False,
     use_pathlib: bool = False,
     verbose: bool = True,
-) -> S3Path:
+) -> T.Tuple[str, Path, S3Path]:
     """
     Assemble the following functions together to build and then upload the
     source artifacts to S3.
 
     - :func:`build_source_artifacts`
     - :func:`upload_source_artifacts`
 
@@ -284,42 +292,47 @@
     lazy, I recommend ``use_pathlib=True``.
 
     :param bsm: boto session manager object
     :param path_setup_py_or_pyproject_toml: example: ``/path/to/setup.py`` or
         ``/path/to/pyproject.toml``
     :param package_name: example: ``aws_lambda_layer``
     :param path_lambda_function: example: ``/path/to/lambda_function.py``
-    :param version: example: ``"0.1.1"``
+    :param version: lambda source code version, example: ``"0.1.1"``
     :param dir_build: example: ``/path/to/build/lambda``
     :param s3dir_lambda: example: ``s3://bucket/path/to/lambda/``
     :param path_bin_python: example ``/path/to/.venv/bin/python``
     :param path_bin_poetry: example ``/path/to/.venv/bin/poetry`` or the global ``poetry``
+    :param metadata: S3 object metadata
     :param tags: S3 object tags
     :param use_pip: do you want to use pip to build your source?
     :param use_build: do you want to use python-build to build your source?
     :param use_poetry: do you want to use python-poetry to build your source?
     :param use_pathlib: do you want to use pathlib to build your source?
     :param verbose: whether you want to suppress the output of cli commands
 
-    :return: the S3 path of the uploaded ``source.zip`` file
+    :return: tuple of three item, first one is the code sha256 hash of the source artifacts,
+        second one is the path to the source.zip file, the third one is the S3 path
+        of the uploaded ``source.zip`` file.
     """
-    build_source_artifacts(
+    source_sha256, path_source_zip = build_source_artifacts(
         path_setup_py_or_pyproject_toml=path_setup_py_or_pyproject_toml,
         package_name=package_name,
         path_lambda_function=path_lambda_function,
         dir_build=dir_build,
         path_bin_python=path_bin_python,
         path_bin_poetry=path_bin_poetry,
         use_pip=use_pip,
         use_build=use_build,
         use_poetry=use_poetry,
         use_pathlib=use_pathlib,
         verbose=verbose,
     )
-    return upload_source_artifacts(
+    s3path_source_zip = upload_source_artifacts(
         bsm=bsm,
         version=version,
+        source_sha256=source_sha256,
         dir_build=dir_build,
         s3dir_lambda=s3dir_lambda,
         metadata=metadata,
         tags=tags,
     )
+    return source_sha256, path_source_zip, s3path_source_zip
```

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer/utils.py` & `aws_lambda_layer-0.2.3/aws_lambda_layer/utils.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/PKG-INFO` & `aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aws-lambda-layer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts.
 Home-page: https://github.com/MacHu-GWU/aws_lambda_layer-project
-Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/aws_lambda_layer/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `aws_lambda_layer-0.2.2/aws_lambda_layer.egg-info/SOURCES.txt` & `aws_lambda_layer-0.2.3/aws_lambda_layer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/pyproject.toml` & `aws_lambda_layer-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_layer"
-version = "0.2.2"
+version = "0.2.3"
 description = "A simple tool that automates the process of building and deploying AWS Lambda layers and source artifacts."
 authors = ["Sanhe Hu <husanhe@gmail.com>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 boto3 = "*"
```

### Comparing `aws_lambda_layer-0.2.2/release-history.rst` & `aws_lambda_layer-0.2.3/release-history.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.3 (2023-05-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- also add source sha256 and layer sha256 to S3 object metadata for integrity check.
+
+
 0.2.2 (2023-05-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that ``aws_lambda_layer.api.sha256_of_paths`` forget to ignore dir in calculation.
```

### Comparing `aws_lambda_layer-0.2.2/setup.py` & `aws_lambda_layer-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_layer-0.2.2/tests/test_utils.py` & `aws_lambda_layer-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*


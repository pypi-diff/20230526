# Comparing `tmp/types-PyScreeze-0.1.0.7.tar.gz` & `tmp/types-PyScreeze-0.1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyScreeze-0.1.0.7.tar", last modified: Wed Feb 22 09:18:16 2023, max compression
+gzip compressed data, was "types-PyScreeze-0.1.0.8.tar", last modified: Fri May 26 15:14:25 2023, max compression
```

## Comparing `types-PyScreeze-0.1.0.7.tar` & `types-PyScreeze-0.1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:16.142654 types-PyScreeze-0.1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-22 09:18:15.000000 types-PyScreeze-0.1.0.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 09:18:15.000000 types-PyScreeze-0.1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-22 09:18:16.142654 types-PyScreeze-0.1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:16.142654 types-PyScreeze-0.1.0.7/pyscreeze-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-22 09:18:15.000000 types-PyScreeze-0.1.0.7/pyscreeze-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-02-22 09:17:01.000000 types-PyScreeze-0.1.0.7/pyscreeze-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:18:16.142654 types-PyScreeze-0.1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-02-22 09:18:15.000000 types-PyScreeze-0.1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:16.142654 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-02-22 09:18:16.000000 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-22 09:18:16.000000 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:18:16.000000 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 09:18:16.000000 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 09:18:16.000000 types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/pyscreeze-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/pyscreeze-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-26 15:14:05.000000 types-PyScreeze-0.1.0.8/pyscreeze-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/top_level.txt
```

### Comparing `types-PyScreeze-0.1.0.7/PKG-INFO` & `types-PyScreeze-0.1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.0.7
+Version: 0.1.0.8
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
```

### Comparing `types-PyScreeze-0.1.0.7/pyscreeze-stubs/__init__.pyi` & `types-PyScreeze-0.1.0.8/pyscreeze-stubs/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     green: int
     blue: int
 
 class PyScreezeException(Exception): ...
 class ImageNotFoundException(PyScreezeException): ...
 
 # _locateAll_opencv
-def requiresPillow(wrappedFunction: Callable[_P, _R]) -> Callable[_P, _R]: ...
+def requiresPyGetWindow(wrappedFunction: Callable[_P, _R]) -> Callable[_P, _R]: ...
 @overload
 def locate(
     needleImage: str | Image.Image | _Mat,
     haystackImage: str | Image.Image | _Mat,
     *,
     grayscale: bool | None = None,
     limit: Unused = 1,
@@ -138,14 +138,16 @@
     minSearchTime: float,
     grayscale: bool | None = None,
     limit: Unused = 1,
     region: tuple[int, int, int, int] | None = None,
     step: int = 1,
     confidence: None = None,
 ) -> Point | None: ...
+def locateOnScreenNear(image: str | Image.Image | _Mat, x: int, y: int) -> Box: ...
+def locateCenterOnScreenNear(image: str | Image.Image | _Mat, x: int, y: int) -> Point | None: ...
 
 # _locateAll_opencv
 @overload
 def locateOnWindow(
     image: str | Image.Image | _Mat,
     title: str,
     *,
@@ -172,16 +174,14 @@
 def center(coords: tuple[int, int, int, int]) -> Point: ...
 def pixelMatchesColor(
     x: int, y: int, expectedRGBColor: tuple[int, int, int] | tuple[int, int, int, int], tolerance: int = 0
 ) -> bool: ...
 def pixel(x: int, y: int) -> tuple[int, int, int]: ...
 def screenshot(imageFilename: StrOrBytesPath | None = None, region: tuple[int, int, int, int] | None = None) -> Image.Image: ...
 
-grab = screenshot
-
 # _locateAll_opencv
 @overload
 def locateAll(
     needleImage: str | Image.Image | _Mat,
     haystackImage: str | Image.Image | _Mat,
     grayscale: bool | None = None,
     limit: int = 1000,
```

### Comparing `types-PyScreeze-0.1.0.7/setup.py` & `types-PyScreeze-0.1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.1.0.7",
+      version="0.1.0.8",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md",
```

### Comparing `types-PyScreeze-0.1.0.7/types_PyScreeze.egg-info/PKG-INFO` & `types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.0.7
+Version: 0.1.0.8
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
```


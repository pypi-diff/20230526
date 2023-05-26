# Comparing `tmp/dl_fib_py-0.0.3.tar.gz` & `tmp/dl_fib_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_fib_py-0.0.3.tar", last modified: Fri May 26 15:25:38 2023, max compression
+gzip compressed data, was "dl_fib_py-0.0.4.tar", last modified: Fri May 26 15:42:41 2023, max compression
```

## Comparing `dl_fib_py-0.0.3.tar` & `dl_fib_py-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.462619 dl_fib_py-0.0.3/
--rw-r--r--   0 dimalurie   (501) staff       (20)     1067 2023-05-26 13:48:50.000000 dl_fib_py-0.0.3/LICENSE
--rw-r--r--   0 dimalurie   (501) staff       (20)      463 2023-05-26 15:25:38.462503 dl_fib_py-0.0.3/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)       41 2023-05-26 13:48:50.000000 dl_fib_py-0.0.3/README.md
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.460981 dl_fib_py-0.0.3/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)       69 2023-05-26 14:03:24.000000 dl_fib_py-0.0.3/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.461726 dl_fib_py-0.0.3/dl_fib_py/cmd/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:12:56.000000 dl_fib_py-0.0.3/dl_fib_py/cmd/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      504 2023-05-26 14:14:31.000000 dl_fib_py-0.0.3/dl_fib_py/cmd/fib_numb.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.461993 dl_fib_py-0.0.3/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:05:34.000000 dl_fib_py-0.0.3/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      302 2023-05-26 14:18:30.000000 dl_fib_py-0.0.3/dl_fib_py/fib_calcs/fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      200 2023-05-26 14:06:36.000000 dl_fib_py-0.0.3/dl_fib_py/fib_calcs/fib_numbers.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.461545 dl_fib_py-0.0.3/dl_fib_py.egg-info/
--rw-r--r--   0 dimalurie   (501) staff       (20)      463 2023-05-26 15:25:38.000000 dl_fib_py-0.0.3/dl_fib_py.egg-info/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)      526 2023-05-26 15:25:38.000000 dl_fib_py-0.0.3/dl_fib_py.egg-info/SOURCES.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)        1 2023-05-26 15:25:38.000000 dl_fib_py-0.0.3/dl_fib_py.egg-info/dependency_links.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       63 2023-05-26 15:25:38.000000 dl_fib_py-0.0.3/dl_fib_py.egg-info/entry_points.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       16 2023-05-26 15:25:38.000000 dl_fib_py-0.0.3/dl_fib_py.egg-info/top_level.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       38 2023-05-26 15:25:38.462656 dl_fib_py-0.0.3/setup.cfg
--rw-r--r--   0 dimalurie   (501) staff       (20)      854 2023-05-26 14:16:02.000000 dl_fib_py-0.0.3/setup.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.460514 dl_fib_py-0.0.3/tests/
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.462097 dl_fib_py-0.0.3/tests/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:16.000000 dl_fib_py-0.0.3/tests/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:25:38.462347 dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:34.000000 dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      660 2023-05-26 15:09:38.000000 dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/test_fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      804 2023-05-26 15:18:31.000000 dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.603314 dl_fib_py-0.0.4/
+-rw-r--r--   0 dimalurie   (501) staff       (20)     1067 2023-05-26 13:48:50.000000 dl_fib_py-0.0.4/LICENSE
+-rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 15:42:41.603189 dl_fib_py-0.0.4/PKG-INFO
+-rw-r--r--   0 dimalurie   (501) staff       (20)       41 2023-05-26 13:48:50.000000 dl_fib_py-0.0.4/README.md
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.601345 dl_fib_py-0.0.4/dl_fib_py/
+-rw-r--r--   0 dimalurie   (501) staff       (20)       69 2023-05-26 14:03:24.000000 dl_fib_py-0.0.4/dl_fib_py/__init__.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602344 dl_fib_py-0.0.4/dl_fib_py/cmd/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:12:56.000000 dl_fib_py-0.0.4/dl_fib_py/cmd/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      504 2023-05-26 14:14:31.000000 dl_fib_py-0.0.4/dl_fib_py/cmd/fib_numb.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602633 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:05:34.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      345 2023-05-26 15:38:29.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/fib_number.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      200 2023-05-26 14:06:36.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/fib_numbers.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602142 dl_fib_py-0.0.4/dl_fib_py.egg-info/
+-rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/PKG-INFO
+-rw-r--r--   0 dimalurie   (501) staff       (20)      558 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)        1 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       63 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/entry_points.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       28 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/requires.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       16 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/top_level.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       38 2023-05-26 15:42:41.603349 dl_fib_py-0.0.4/setup.cfg
+-rw-r--r--   0 dimalurie   (501) staff       (20)      914 2023-05-26 15:42:13.000000 dl_fib_py-0.0.4/setup.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.600866 dl_fib_py-0.0.4/tests/
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602737 dl_fib_py-0.0.4/tests/dl_fib_py/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:16.000000 dl_fib_py-0.0.4/tests/dl_fib_py/__init__.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.603018 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:34.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      660 2023-05-26 15:09:38.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_number.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      804 2023-05-26 15:18:31.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
```

### Comparing `dl_fib_py-0.0.3/LICENSE` & `dl_fib_py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.3/dl_fib_py.egg-info/SOURCES.txt` & `dl_fib_py-0.0.4/dl_fib_py.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 dl_fib_py/__init__.py
 dl_fib_py.egg-info/PKG-INFO
 dl_fib_py.egg-info/SOURCES.txt
 dl_fib_py.egg-info/dependency_links.txt
 dl_fib_py.egg-info/entry_points.txt
+dl_fib_py.egg-info/requires.txt
 dl_fib_py.egg-info/top_level.txt
 dl_fib_py/cmd/__init__.py
 dl_fib_py/cmd/fib_numb.py
 dl_fib_py/fib_calcs/__init__.py
 dl_fib_py/fib_calcs/fib_number.py
 dl_fib_py/fib_calcs/fib_numbers.py
 tests/dl_fib_py/__init__.py
```

### Comparing `dl_fib_py-0.0.3/setup.py` & `dl_fib_py-0.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dl_fib_py",
-    version="0.0.3",
+    version="0.0.4",
     author="Dima Lurie",
     author_email="dimalurie@gmail.com",
     description="Calculates a Fibonacci number",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dima-lurie/dl-fib-py.git",
     install_requires=[],
     packages=find_packages(exclude=("tests",)),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3",
+    extras_require={"dev": ["mypy>=1.3", "twine>=4.0"]},
+    python_requires=">=3.11",
     tests_require=["pytest"],
     entry_points={
         "console_scripts": [
             "fib-number = \
            dl_fib_py.cmd.fib_numb:fib_numb",
         ],
     },
```

### Comparing `dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/test_fib_number.py` & `dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_number.py`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.3/tests/dl_fib_py/fib_calcs/test_fib_numbers.py` & `dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_numbers.py`

 * *Files identical despite different names*


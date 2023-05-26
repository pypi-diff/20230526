# Comparing `tmp/dl_fib_py-0.0.4.tar.gz` & `tmp/dl_fib_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_fib_py-0.0.4.tar", last modified: Fri May 26 15:42:41 2023, max compression
+gzip compressed data, was "dl_fib_py-0.0.5.tar", last modified: Fri May 26 16:25:00 2023, max compression
```

## Comparing `dl_fib_py-0.0.4.tar` & `dl_fib_py-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.603314 dl_fib_py-0.0.4/
--rw-r--r--   0 dimalurie   (501) staff       (20)     1067 2023-05-26 13:48:50.000000 dl_fib_py-0.0.4/LICENSE
--rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 15:42:41.603189 dl_fib_py-0.0.4/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)       41 2023-05-26 13:48:50.000000 dl_fib_py-0.0.4/README.md
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.601345 dl_fib_py-0.0.4/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)       69 2023-05-26 14:03:24.000000 dl_fib_py-0.0.4/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602344 dl_fib_py-0.0.4/dl_fib_py/cmd/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:12:56.000000 dl_fib_py-0.0.4/dl_fib_py/cmd/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      504 2023-05-26 14:14:31.000000 dl_fib_py-0.0.4/dl_fib_py/cmd/fib_numb.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602633 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:05:34.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      345 2023-05-26 15:38:29.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      200 2023-05-26 14:06:36.000000 dl_fib_py-0.0.4/dl_fib_py/fib_calcs/fib_numbers.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602142 dl_fib_py-0.0.4/dl_fib_py.egg-info/
--rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/PKG-INFO
--rw-r--r--   0 dimalurie   (501) staff       (20)      558 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/SOURCES.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)        1 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/dependency_links.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       63 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/entry_points.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       28 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/requires.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       16 2023-05-26 15:42:41.000000 dl_fib_py-0.0.4/dl_fib_py.egg-info/top_level.txt
--rw-r--r--   0 dimalurie   (501) staff       (20)       38 2023-05-26 15:42:41.603349 dl_fib_py-0.0.4/setup.cfg
--rw-r--r--   0 dimalurie   (501) staff       (20)      914 2023-05-26 15:42:13.000000 dl_fib_py-0.0.4/setup.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.600866 dl_fib_py-0.0.4/tests/
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.602737 dl_fib_py-0.0.4/tests/dl_fib_py/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:16.000000 dl_fib_py-0.0.4/tests/dl_fib_py/__init__.py
-drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:42:41.603018 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/
--rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:34.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/__init__.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      660 2023-05-26 15:09:38.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_number.py
--rw-r--r--   0 dimalurie   (501) staff       (20)      804 2023-05-26 15:18:31.000000 dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.744532 dl_fib_py-0.0.5/
+-rw-r--r--   0 dimalurie   (501) staff       (20)     1067 2023-05-26 13:48:50.000000 dl_fib_py-0.0.5/LICENSE
+-rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 16:25:00.744298 dl_fib_py-0.0.5/PKG-INFO
+-rw-r--r--   0 dimalurie   (501) staff       (20)       41 2023-05-26 13:48:50.000000 dl_fib_py-0.0.5/README.md
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.742165 dl_fib_py-0.0.5/dl_fib_py/
+-rw-r--r--   0 dimalurie   (501) staff       (20)       69 2023-05-26 14:03:24.000000 dl_fib_py-0.0.5/dl_fib_py/__init__.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743143 dl_fib_py-0.0.5/dl_fib_py/cmd/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:12:56.000000 dl_fib_py-0.0.5/dl_fib_py/cmd/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      504 2023-05-26 14:14:31.000000 dl_fib_py-0.0.5/dl_fib_py/cmd/fib_numb.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743580 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 14:05:34.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      345 2023-05-26 15:38:29.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/fib_number.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      200 2023-05-26 14:06:36.000000 dl_fib_py-0.0.5/dl_fib_py/fib_calcs/fib_numbers.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)       15 2023-05-26 16:24:50.000000 dl_fib_py-0.0.5/dl_fib_py/version.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.742771 dl_fib_py-0.0.5/dl_fib_py.egg-info/
+-rw-r--r--   0 dimalurie   (501) staff       (20)      486 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/PKG-INFO
+-rw-r--r--   0 dimalurie   (501) staff       (20)      579 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)        1 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       63 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/entry_points.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       37 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/requires.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       16 2023-05-26 16:25:00.000000 dl_fib_py-0.0.5/dl_fib_py.egg-info/top_level.txt
+-rw-r--r--   0 dimalurie   (501) staff       (20)       38 2023-05-26 16:25:00.744571 dl_fib_py-0.0.5/setup.cfg
+-rw-r--r--   0 dimalurie   (501) staff       (20)     1099 2023-05-26 16:24:44.000000 dl_fib_py-0.0.5/setup.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.741549 dl_fib_py-0.0.5/tests/
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.743751 dl_fib_py-0.0.5/tests/dl_fib_py/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:16.000000 dl_fib_py-0.0.5/tests/dl_fib_py/__init__.py
+drwxr-xr-x   0 dimalurie   (501) staff       (20)        0 2023-05-26 16:25:00.744100 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/
+-rw-r--r--   0 dimalurie   (501) staff       (20)        0 2023-05-26 15:04:34.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/__init__.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      684 2023-05-26 15:49:50.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_number.py
+-rw-r--r--   0 dimalurie   (501) staff       (20)      804 2023-05-26 15:18:31.000000 dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_numbers.py
```

### Comparing `dl_fib_py-0.0.4/LICENSE` & `dl_fib_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_fib_py-0.0.4/dl_fib_py.egg-info/SOURCES.txt` & `dl_fib_py-0.0.5/dl_fib_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 dl_fib_py/__init__.py
+dl_fib_py/version.py
 dl_fib_py.egg-info/PKG-INFO
 dl_fib_py.egg-info/SOURCES.txt
 dl_fib_py.egg-info/dependency_links.txt
 dl_fib_py.egg-info/entry_points.txt
 dl_fib_py.egg-info/requires.txt
 dl_fib_py.egg-info/top_level.txt
 dl_fib_py/cmd/__init__.py
```

### Comparing `dl_fib_py-0.0.4/setup.py` & `dl_fib_py-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from setuptools import find_packages, setup
+import pathlib
+
+with open(
+    str(pathlib.Path(__file__).parent.absolute()) + "/dl_fib_py/version.py", "r"
+) as fh:
+    version = fh.read().split("=")[1].replace("'", "")
+
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dl_fib_py",
-    version="0.0.4",
+    version=version,
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
-    extras_require={"dev": ["mypy>=1.3", "twine>=4.0"]},
+    extras_require={"dev": ["mypy>=1.3", "twine>=4.0", "requests"]},
     python_requires=">=3.11",
     tests_require=["pytest"],
     entry_points={
         "console_scripts": [
             "fib-number = \
            dl_fib_py.cmd.fib_numb:fib_numb",
         ],
```

### Comparing `dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_number.py` & `dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_number.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 
 class RecurringFibNumberTest(TestCase):
     def test_zero(self):
         self.assertEqual(0, recurring_fibonacci_number(number=0))
 
     def test_negative(self):
-        self.assertEqual(None, recurring_fibonacci_number(number=-1))
+        with self.assertRaises(ValueError):
+            recurring_fibonacci_number(number=-1)
 
     def test_one(self):
         self.assertEqual(1, recurring_fibonacci_number(number=1))
 
     def test_two(self):
         self.assertEqual(1, recurring_fibonacci_number(number=2))
```

### Comparing `dl_fib_py-0.0.4/tests/dl_fib_py/fib_calcs/test_fib_numbers.py` & `dl_fib_py-0.0.5/tests/dl_fib_py/fib_calcs/test_fib_numbers.py`

 * *Files identical despite different names*


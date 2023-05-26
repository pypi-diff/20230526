# Comparing `tmp/pyenasolar-0.1.6.tar.gz` & `tmp/pyenasolar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenasolar-0.1.6.tar", last modified: Thu Jan 13 01:33:01 2022, max compression
+gzip compressed data, was "pyenasolar-0.2.0.tar", last modified: Fri May 26 04:48:03 2023, max compression
```

## Comparing `pyenasolar-0.1.6.tar` & `pyenasolar-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 geustace  (1000) geustace  (1000)        0 2022-01-13 01:33:01.904058 pyenasolar-0.1.6/
--rw-rw----   0 geustace  (1000) geustace  (1000)     1133 2021-08-07 04:53:03.000000 pyenasolar-0.1.6/LICENSE
--rw-r--r--   0 geustace  (1000) geustace  (1000)     1319 2022-01-13 01:33:01.904058 pyenasolar-0.1.6/PKG-INFO
--rw-rw----   0 geustace  (1000) geustace  (1000)      831 2021-09-08 21:43:39.000000 pyenasolar-0.1.6/README.md
-drwxr-xr-x   0 geustace  (1000) geustace  (1000)        0 2022-01-13 01:33:01.900058 pyenasolar-0.1.6/pyenasolar/
--rw-rw----   0 geustace  (1000) geustace  (1000)    16219 2022-01-13 01:31:47.000000 pyenasolar-0.1.6/pyenasolar/__init__.py
-drwxr-xr-x   0 geustace  (1000) geustace  (1000)        0 2022-01-13 01:33:01.904058 pyenasolar-0.1.6/pyenasolar.egg-info/
--rw-rw----   0 geustace  (1000) geustace  (1000)     1319 2022-01-13 01:33:01.000000 pyenasolar-0.1.6/pyenasolar.egg-info/PKG-INFO
--rw-rw----   0 geustace  (1000) geustace  (1000)      200 2022-01-13 01:33:01.000000 pyenasolar-0.1.6/pyenasolar.egg-info/SOURCES.txt
--rw-rw----   0 geustace  (1000) geustace  (1000)        1 2022-01-13 01:33:01.000000 pyenasolar-0.1.6/pyenasolar.egg-info/dependency_links.txt
--rw-rw----   0 geustace  (1000) geustace  (1000)       11 2022-01-13 01:33:01.000000 pyenasolar-0.1.6/pyenasolar.egg-info/top_level.txt
--rw-rw----   0 geustace  (1000) geustace  (1000)      105 2021-08-09 01:16:41.000000 pyenasolar-0.1.6/pyproject.toml
--rw-r--r--   0 geustace  (1000) geustace  (1000)       38 2022-01-13 01:33:01.904058 pyenasolar-0.1.6/setup.cfg
--rw-rw----   0 geustace  (1000) geustace  (1000)      667 2022-01-13 01:32:40.000000 pyenasolar-0.1.6/setup.py
+drwxrwx---   0 geustace   (501) staff       (20)        0 2023-05-26 04:48:03.480767 pyenasolar-0.2.0/
+-rw-rw----   0 geustace   (501) staff       (20)     1133 2021-08-07 04:53:03.000000 pyenasolar-0.2.0/LICENSE
+-rw-rw----   0 geustace   (501) staff       (20)     1319 2023-05-26 04:48:03.478767 pyenasolar-0.2.0/PKG-INFO
+-rw-rw----   0 geustace   (501) staff       (20)      831 2021-09-08 21:43:39.000000 pyenasolar-0.2.0/README.md
+drwxrwx---   0 geustace   (501) staff       (20)        0 2023-05-26 04:48:03.458767 pyenasolar-0.2.0/pyenasolar/
+-rw-rw----   0 geustace   (501) staff       (20)    15985 2023-05-26 04:30:06.000000 pyenasolar-0.2.0/pyenasolar/__init__.py
+drwxrwx---   0 geustace   (501) staff       (20)        0 2023-05-26 04:48:03.474767 pyenasolar-0.2.0/pyenasolar.egg-info/
+-rw-rw----   0 geustace   (501) staff       (20)     1319 2023-05-26 04:48:03.000000 pyenasolar-0.2.0/pyenasolar.egg-info/PKG-INFO
+-rw-rw----   0 geustace   (501) staff       (20)      200 2023-05-26 04:48:03.000000 pyenasolar-0.2.0/pyenasolar.egg-info/SOURCES.txt
+-rw-rw----   0 geustace   (501) staff       (20)        1 2023-05-26 04:48:03.000000 pyenasolar-0.2.0/pyenasolar.egg-info/dependency_links.txt
+-rw-rw----   0 geustace   (501) staff       (20)       11 2023-05-26 04:48:03.000000 pyenasolar-0.2.0/pyenasolar.egg-info/top_level.txt
+-rw-rw----   0 geustace   (501) staff       (20)      105 2021-08-09 01:16:41.000000 pyenasolar-0.2.0/pyproject.toml
+-rw-rw----   0 geustace   (501) staff       (20)       38 2023-05-26 04:48:03.481767 pyenasolar-0.2.0/setup.cfg
+-rw-rw----   0 geustace   (501) staff       (20)      667 2023-05-26 04:30:36.000000 pyenasolar-0.2.0/setup.py
```

### Comparing `pyenasolar-0.1.6/LICENSE` & `pyenasolar-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenasolar-0.1.6/PKG-INFO` & `pyenasolar-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenasolar
-Version: 0.1.6
+Version: 0.2.0
 Summary: Library to communicate with EnaSolar inverters
 Home-page: https://github.com/geustace/pyenasolar
 Author: geustace
 Author-email: glen@eustace.nz
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenasolar-0.1.6/README.md` & `pyenasolar-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenasolar-0.1.6/pyenasolar/__init__.py` & `pyenasolar-0.2.0/pyenasolar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,18 +405,14 @@
                                 continue
                             find = xml.find(sen.key)
                             if find is not None:
                                 sen.value = find.text
                                 if sen.is_hex:
                                     sen.value = int(sen.value, 16)
                                 sen.value = float(sen.value) * sen.factor
-                                if sen.unit == "h":
-                                    sen.value = "{:,d}:{:02d}".format(
-                                        *divmod(int(sen.value * 60), 60)
-                                    )
                                 sen.date = date.today()
                                 sen.enabled = True
                                 at_least_one_enabled = True
 
                             if sen.enabled:
                                 _LOGGER.debug(
                                     "Set DATA sensor %s => %s", sen.name, sen.value
```

### Comparing `pyenasolar-0.1.6/pyenasolar.egg-info/PKG-INFO` & `pyenasolar-0.2.0/pyenasolar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenasolar
-Version: 0.1.6
+Version: 0.2.0
 Summary: Library to communicate with EnaSolar inverters
 Home-page: https://github.com/geustace/pyenasolar
 Author: geustace
 Author-email: glen@eustace.nz
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyenasolar-0.1.6/setup.py` & `pyenasolar-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyenasolar",
-    version="0.1.6",
+    version="0.2.0",
     author="geustace",
     author_email="glen@eustace.nz",
     description="Library to communicate with EnaSolar inverters",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geustace/pyenasolar",
     packages=setuptools.find_packages(),
```


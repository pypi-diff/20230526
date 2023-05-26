# Comparing `tmp/evosegment-0.0.1.tar.gz` & `tmp/evosegment-0.0.2.tar.gz`

## Comparing `evosegment-0.0.1.tar` & `evosegment-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0   442945 2020-02-02 00:00:00.000000 evosegment-0.0.1/example.ipynb
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.1/data/bubble_0.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.1/data/bubble_1.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.1/data/bubble_2.tif
--rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.1/data/bubble_3.tif
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.1/evosegment/__init__.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 evosegment-0.0.1/evosegment/evoSegment.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.1/.gitignore
--rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.1/LICENSE
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 evosegment-0.0.1/README.md
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 evosegment-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 evosegment-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0   442945 2020-02-02 00:00:00.000000 evosegment-0.0.2/example.ipynb
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.2/data/bubble_0.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.2/data/bubble_1.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.2/data/bubble_2.tif
+-rw-r--r--   0        0        0  2665710 2020-02-02 00:00:00.000000 evosegment-0.0.2/data/bubble_3.tif
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 evosegment-0.0.2/evosegment/__init__.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 evosegment-0.0.2/evosegment/evoSegment.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 evosegment-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35076 2020-02-02 00:00:00.000000 evosegment-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 evosegment-0.0.2/README.md
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 evosegment-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 evosegment-0.0.2/PKG-INFO
```

### Comparing `evosegment-0.0.1/example.ipynb` & `evosegment-0.0.2/example.ipynb`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/data/bubble_0.tif` & `evosegment-0.0.2/data/bubble_0.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/data/bubble_1.tif` & `evosegment-0.0.2/data/bubble_1.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/data/bubble_2.tif` & `evosegment-0.0.2/data/bubble_2.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/data/bubble_3.tif` & `evosegment-0.0.2/data/bubble_3.tif`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/evosegment/evoSegment.py` & `evosegment-0.0.2/evosegment/evoSegment.py`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/LICENSE` & `evosegment-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/README.md` & `evosegment-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `evosegment-0.0.1/pyproject.toml` & `evosegment-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "evosegment"
-version = "0.0.1"
+version = "0.0.2"
 description = 'A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)'
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
 keywords = []
 authors = [
   { name = "Johan Hektor", email = "johan.hektor@mau.se" },
```

### Comparing `evosegment-0.0.1/PKG-INFO` & `evosegment-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evosegment
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for segmentation of grayscale evolution from 4D tomograhphy data (or other images)
 Project-URL: Documentation, https://gitlab.com/jhektor/evoSegment#readme
 Project-URL: Issues, https://gitlab.com/jhektor/evoSegment/-/issues
 Project-URL: Source, https://gitlab.com/jhektor/evoSegment
 Author-email: Johan Hektor <johan.hektor@mau.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```


# Comparing `tmp/llsd-1.2.1.tar.gz` & `tmp/llsd-1.2.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llsd-1.2.1.tar", last modified: Mon May  8 14:20:23 2023, max compression
+gzip compressed data, was "llsd-1.2.2.dev1.tar", last modified: Thu May 25 23:54:23 2023, max compression
```

## Comparing `llsd-1.2.1.tar` & `llsd-1.2.2.dev1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.969150 llsd-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/dependabot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.969150 llsd-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/bench.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 14:19:05.000000 llsd-1.2.1/.github/workflows/cla.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-08 14:19:05.000000 llsd-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 14:19:05.000000 llsd-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-08 14:19:05.000000 llsd-1.2.1/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 14:19:05.000000 llsd-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-08 14:20:23.973150 llsd-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-08 14:19:05.000000 llsd-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/llsd/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/fastest_elementtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11119 2023-05-08 14:19:05.000000 llsd-1.2.1/llsd/serde_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/llsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 14:20:23.000000 llsd-1.2.1/llsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:20:23.973150 llsd-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 14:19:05.000000 llsd-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:20:23.973150 llsd-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-05-08 14:19:05.000000 llsd-1.2.1/tests/llsd_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-08 14:19:05.000000 llsd-1.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/dependabot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/bench.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.github/workflows/cla.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.685032 llsd-1.2.2.dev1/llsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/fastest_elementtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/llsd/serde_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/llsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 23:54:23.000000 llsd-1.2.2.dev1/llsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 23:54:23.689032 llsd-1.2.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tests/llsd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 23:53:19.000000 llsd-1.2.2.dev1/tox.ini
```

### Comparing `llsd-1.2.1/.github/workflows/bench.yaml` & `llsd-1.2.2.dev1/.github/workflows/bench.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/.github/workflows/ci.yaml` & `llsd-1.2.2.dev1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/.github/workflows/cla.yaml` & `llsd-1.2.2.dev1/.github/workflows/cla.yaml`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/.gitignore` & `llsd-1.2.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/LICENSE` & `llsd-1.2.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/PKG-INFO` & `llsd-1.2.2.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.1
+Version: 1.2.2.dev1
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.1/README.md` & `llsd-1.2.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd/__init__.py` & `llsd-1.2.2.dev1/llsd/__init__.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd/base.py` & `llsd-1.2.2.dev1/llsd/base.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd/fastest_elementtree.py` & `llsd-1.2.2.dev1/llsd/fastest_elementtree.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd/serde_binary.py` & `llsd-1.2.2.dev1/llsd/serde_binary.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd/serde_notation.py` & `llsd-1.2.2.dev1/llsd/serde_notation.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/llsd.egg-info/PKG-INFO` & `llsd-1.2.2.dev1/llsd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llsd
-Version: 1.2.1
+Version: 1.2.2.dev1
 Summary: Linden Lab Structured Data (LLSD) serialization library
 Home-page: https://github.com/secondlife/python-llsd
 Author: Linden Research, Inc.
 Author-email: opensource-dev@lists.secondlife.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llsd-1.2.1/llsd.egg-info/SOURCES.txt` & `llsd-1.2.2.dev1/llsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/setup.py` & `llsd-1.2.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/tests/bench.py` & `llsd-1.2.2.dev1/tests/bench.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,14 +41,17 @@
       <uri>https://secondlife.com</uri>
       <date>2006-02-01T14:29:53Z</date>
     </array>
   </map>
 </llsd>"""
 
 _bench_data = llsd.parse_xml(BENCH_DATA_XML)
+
+    
+    
 BENCH_DATA_BINARY = llsd.format_binary(_bench_data)
 BENCH_DATA_NOTATION = llsd.format_notation(_bench_data)
 
 _tc = unittest.TestCase()
 _tc.maxDiff = 5000
 assertDictEqual =  _tc.assertDictEqual
 
@@ -74,14 +77,37 @@
 def binary_stream():
     with TemporaryFile() as f:
         d = llsd.format_binary(_bench_data)
         f.write(d)
         f.seek(0)
         yield f
 
+def build_deep_xml():
+    deep_data = {}
+    curr_data = deep_data
+    for i in range(250):
+        curr_data["curr_data"] = {}
+        curr_data["integer"] = 7
+        curr_data["string"] = "string"
+        curr_data["map"] = { "item1": 2.345, "item2": [1,2,3], "item3": {"item4": llsd.uri("http://foo.bar.com")}}
+        curr_data = curr_data["curr_data"]
+        
+    return deep_data
+_deep_bench_data = build_deep_xml()
+
+def build_wide_xml():
+    
+    wide_xml = b"""
+<?xml version="1.0" encoding="UTF-8"?><llsd><map><key>wide_array</key><array>"
+"""
+    wide_data = {}
+    for i in range(100000):
+        wide_data["item"+str(i)] = {"item1":2.345, "item2": [1,2,3], "item3": "string", "item4":{"subitem": llsd.uri("http://foo.bar.com")}}
+    return wide_data
+_wide_bench_data = build_wide_xml()
 
 def bench_stream(parse, stream):
     ret = parse(stream)
     stream.seek(0)
     return ret
 
 
@@ -121,7 +147,13 @@
 
 def test_format_notation(benchmark):
     benchmark(llsd.format_notation, _bench_data)
 
 
 def test_format_binary(benchmark):
     benchmark(llsd.format_binary, _bench_data)
+
+def test_format_xml_deep(benchmark):
+    benchmark(llsd.format_xml, _deep_bench_data)
+
+def test_format_xml_wide(benchmark):
+    benchmark(llsd.format_xml, _wide_bench_data)
```

### Comparing `llsd-1.2.1/tests/fuzz.py` & `llsd-1.2.2.dev1/tests/fuzz.py`

 * *Files identical despite different names*

### Comparing `llsd-1.2.1/tests/llsd_test.py` & `llsd-1.2.2.dev1/tests/llsd_test.py`

 * *Files identical despite different names*


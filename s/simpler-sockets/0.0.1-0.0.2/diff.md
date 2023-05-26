# Comparing `tmp/simpler_sockets-0.0.1.tar.gz` & `tmp/simpler_sockets-0.0.2.tar.gz`

## Comparing `simpler_sockets-0.0.1.tar` & `simpler_sockets-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/src/simpler_sockets/__about__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/src/simpler_sockets/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/README.md
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 simpler_sockets-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/src/simpler_sockets/__about__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/src/simpler_sockets/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/README.md
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 simpler_sockets-0.0.2/PKG-INFO
```

### Comparing `simpler_sockets-0.0.1/src/simpler_sockets/__init__.py` & `simpler_sockets-0.0.2/src/simpler_sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpler_sockets-0.0.1/LICENSE.txt` & `simpler_sockets-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simpler_sockets-0.0.1/README.md` & `simpler_sockets-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simpler_sockets-0.0.1/pyproject.toml` & `simpler_sockets-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,17 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/unknown/simpler-sockets#readme"
-Issues = "https://github.com/unknown/simpler-sockets/issues"
-Source = "https://github.com/unknown/simpler-sockets"
+Documentation = "https://github.com/StrajnarFilip/simpler-sockets"
+Issues = "https://github.com/StrajnarFilip/simpler-sockets"
+Source = "https://github.com/StrajnarFilip/simpler-sockets"
 
 [tool.hatch.version]
 path = "src/simpler_sockets/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```


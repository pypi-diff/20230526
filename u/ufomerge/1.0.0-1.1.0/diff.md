# Comparing `tmp/ufomerge-1.0.0.tar.gz` & `tmp/ufomerge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufomerge-1.0.0.tar", last modified: Thu May  4 21:39:10 2023, max compression
+gzip compressed data, was "ufomerge-1.1.0.tar", last modified: Fri May 26 06:28:05 2023, max compression
```

## Comparing `ufomerge-1.0.0.tar` & `ufomerge-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 21:39:10.832111 ufomerge-1.0.0/
--rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.0.0/AUTHORS.txt
--rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.0.0/CONTRIBUTORS.txt
--rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.0.0/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 21:39:10.827890 ufomerge-1.0.0/Lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 21:39:10.829835 ufomerge-1.0.0/Lib/ufomerge/
--rw-r--r--   0 simon      (501) staff       (20)    27599 2023-05-04 21:07:09.000000 ufomerge-1.0.0/Lib/ufomerge/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.0.0/Lib/ufomerge/__main__.py
--rw-r--r--   0 simon      (501) staff       (20)      160 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge/_version.py
--rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.0.0/Lib/ufomerge/cli.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 21:39:10.830801 ufomerge-1.0.0/Lib/ufomerge.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      433 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       47 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)       29 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-05-04 21:39:10.000000 ufomerge-1.0.0/Lib/ufomerge.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-04 21:39:10.831947 ufomerge-1.0.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.0.0/README.md
--rw-r--r--   0 simon      (501) staff       (20)      632 2023-05-04 17:05:45.000000 ufomerge-1.0.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-04 21:39:10.832150 ufomerge-1.0.0/setup.cfg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 21:39:10.831547 ufomerge-1.0.0/tests/
--rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.0.0/tests/conftest.py
--rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.0.0/tests/test_basic.py
--rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.0.0/tests/test_layout.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.964199 ufomerge-1.1.0/
+-rw-r--r--   0 simon      (501) staff       (20)      302 2023-05-04 21:34:42.000000 ufomerge-1.1.0/AUTHORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1060 2023-05-04 21:34:45.000000 ufomerge-1.1.0/CONTRIBUTORS.txt
+-rw-r--r--   0 simon      (501) staff       (20)    11358 2023-05-04 21:33:18.000000 ufomerge-1.1.0/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.959356 ufomerge-1.1.0/Lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.961735 ufomerge-1.1.0/Lib/ufomerge/
+-rw-r--r--   0 simon      (501) staff       (20)    27676 2023-05-26 06:20:31.000000 ufomerge-1.1.0/Lib/ufomerge/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)       87 2023-05-04 20:25:37.000000 ufomerge-1.1.0/Lib/ufomerge/__main__.py
+-rw-r--r--   0 simon      (501) staff       (20)      160 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge/_version.py
+-rw-r--r--   0 simon      (501) staff       (20)     4261 2023-05-04 21:10:17.000000 ufomerge-1.1.0/Lib/ufomerge/cli.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.962921 ufomerge-1.1.0/Lib/ufomerge.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      433 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       47 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)       29 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-05-26 06:28:05.000000 ufomerge-1.1.0/Lib/ufomerge.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)     2402 2023-05-26 06:28:05.964027 ufomerge-1.1.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     2073 2023-05-04 21:34:01.000000 ufomerge-1.1.0/README.md
+-rw-r--r--   0 simon      (501) staff       (20)      632 2023-05-26 06:27:42.000000 ufomerge-1.1.0/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-26 06:28:05.964239 ufomerge-1.1.0/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-26 06:28:05.963658 ufomerge-1.1.0/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     1357 2023-05-04 13:39:59.000000 ufomerge-1.1.0/tests/conftest.py
+-rw-r--r--   0 simon      (501) staff       (20)     1315 2023-05-04 13:16:44.000000 ufomerge-1.1.0/tests/test_basic.py
+-rw-r--r--   0 simon      (501) staff       (20)     2969 2023-05-04 17:05:29.000000 ufomerge-1.1.0/tests/test_layout.py
```

### Comparing `ufomerge-1.0.0/CONTRIBUTORS.txt` & `ufomerge-1.1.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/LICENSE` & `ufomerge-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/Lib/ufomerge/__init__.py` & `ufomerge-1.1.0/Lib/ufomerge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,17 @@
 
             if hasattr(st, "statements"):
                 st.statements = self.filter_layout(st.statements)
                 substantive_statements = [
                     x for x in st.statements if not isinstance(x, ast.Comment)
                 ]
                 if not substantive_statements:
-                    st.statements = [ast.Comment("lookupflag 0; #HELLO WORLD")]
+                    if isinstance(st, ast.FeatureBlock):
+                        continue
+                    st.statements = [ast.Comment("lookupflag 0;")]
                 newstatements.append(st)
                 continue
             if isinstance(st, ast.GlyphClassDefinition):
                 st.glyphs = self.filter_glyph_container(st.glyphs)
             if isinstance(
                 st,
                 (
```

### Comparing `ufomerge-1.0.0/Lib/ufomerge/cli.py` & `ufomerge-1.1.0/Lib/ufomerge/cli.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/Lib/ufomerge.egg-info/PKG-INFO` & `ufomerge-1.1.0/Lib/ufomerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.0.0
+Version: 1.1.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.0.0/PKG-INFO` & `ufomerge-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufomerge
-Version: 1.0.0
+Version: 1.1.0
 Summary: Merge together two source fonts in UFO format
 Author-email: Simon Cozens <simon@simon-cozens.org>
 Classifier: Environment :: Console
 Classifier: Topic :: Text Processing :: Fonts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.txt
```

### Comparing `ufomerge-1.0.0/README.md` & `ufomerge-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/pyproject.toml` & `ufomerge-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/tests/conftest.py` & `ufomerge-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/tests/test_basic.py` & `ufomerge-1.1.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `ufomerge-1.0.0/tests/test_layout.py` & `ufomerge-1.1.0/tests/test_layout.py`

 * *Files identical despite different names*


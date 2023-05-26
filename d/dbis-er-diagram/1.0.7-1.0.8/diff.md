# Comparing `tmp/dbis-er-diagram-1.0.7.tar.gz` & `tmp/dbis-er-diagram-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-er-diagram-1.0.7.tar", last modified: Tue May  9 14:16:37 2023, max compression
+gzip compressed data, was "dbis-er-diagram-1.0.8.tar", last modified: Fri May 26 15:58:37 2023, max compression
```

## Comparing `dbis-er-diagram-1.0.7.tar` & `dbis-er-diagram-1.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.555646 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-09 14:16:37.000000 dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/top_level.txt
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.555646 dbis-er-diagram-1.0.7/erdiagram/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/er.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    30923 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/erdiagram/grading.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/erdiagram/node_type.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/pyproject.toml
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-09 14:16:37.567646 dbis-er-diagram-1.0.7/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_adders.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_getters.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-04 14:27:55.000000 dbis-er-diagram-1.0.7/tests/test_grading_components.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_grading_diagrams.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11835 2023-05-09 14:16:07.000000 dbis-er-diagram-1.0.7/tests/test_grading_special_cases.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.7/tests/test_other_methods.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-26 15:58:37.498478 dbis-er-diagram-1.0.8/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-26 15:58:37.497478 dbis-er-diagram-1.0.8/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-26 15:58:37.491478 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-26 15:58:37.000000 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-26 15:58:37.000000 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-26 15:58:37.000000 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       55 2023-05-26 15:58:37.000000 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-26 15:58:37.000000 dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/top_level.txt
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-26 15:58:37.494478 dbis-er-diagram-1.0.8/erdiagram/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/erdiagram/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/erdiagram/drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/erdiagram/er.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    31052 2023-05-26 15:57:47.000000 dbis-er-diagram-1.0.8/erdiagram/grading.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/erdiagram/merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/erdiagram/node_type.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      888 2023-05-26 15:57:47.000000 dbis-er-diagram-1.0.8/pyproject.toml
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-26 15:58:37.498478 dbis-er-diagram-1.0.8/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-26 15:58:37.497478 dbis-er-diagram-1.0.8/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_adders.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_getters.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_grading_components.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_grading_diagrams.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11197 2023-05-26 15:57:47.000000 dbis-er-diagram-1.0.8/tests/test_grading_special_cases.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-26 15:37:53.000000 dbis-er-diagram-1.0.8/tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.7/LICENSE` & `dbis-er-diagram-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/PKG-INFO` & `dbis-er-diagram-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.7
+Version: 1.0.8
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.7/README.md` & `dbis-er-diagram-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/PKG-INFO` & `dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.7
+Version: 1.0.8
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.7/dbis_er_diagram.egg-info/SOURCES.txt` & `dbis-er-diagram-1.0.8/dbis_er_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/erdiagram/drawing.py` & `dbis-er-diagram-1.0.8/erdiagram/drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/erdiagram/er.py` & `dbis-er-diagram-1.0.8/erdiagram/er.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/erdiagram/grading.py` & `dbis-er-diagram-1.0.8/erdiagram/grading.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,30 +232,34 @@
     s = s.lower()
 
     if s.isdigit():
         # The string represents an integer
         return int(s)
     elif s.isalpha():
         # The string represents a single character string
-        return s
+        # return s
+        return "n"
     elif s.startswith("(") and s.endswith(")"):
         # The string represents a tuple of two values
         parts = s[1:-1].split(",")
         if len(parts) != 2:
             return None
         val1 = parts[0].strip()
         val2 = parts[1].strip()
         if val1.isdigit() and val2.isdigit():
             return (int(val1), int(val2))
         elif val1.isdigit() and val2.isalpha():
-            return (int(val1), val2)
+            # return (int(val1), val2)
+            return (int(val1), "n")
         elif val1.isalpha() and val2.isdigit():
-            return (val1, int(val2))
+            return ("n", int(val2))
+            # return (val1, int(val2))
         else:
-            return (val1, val2)
+            return ("n", "n")
+            # return (val1, val2)
     else:
         return None
 
 
 @typechecked
 def _grade_relation_pair(
     relation_pair: tuple[dict[str, Any], dict[str, Any]],
```

### Comparing `dbis-er-diagram-1.0.7/erdiagram/merging.py` & `dbis-er-diagram-1.0.8/erdiagram/merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/pyproject.toml` & `dbis-er-diagram-1.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-er-diagram"
-version = "1.0.7"
+version = "1.0.8"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Michal Slupczynski", email = "slupczynski@dbis.rwth-aachen.de" },
 	{ name = "Beyza Akyüz", email = "beyza.akyuez@rwth-aachen.de" },
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
@@ -13,15 +13,15 @@
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 ]
 dependencies = [
 	"networkx",
 	"graphviz",
 	"ipython",
-	"typeguard",
+	"typeguard==3.0.2",
 	"Levenshtein",
 ]
 
 [project.urls]
 "Homepage" = "https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram"
 
 [options]
```

### Comparing `dbis-er-diagram-1.0.7/tests/test_adders.py` & `dbis-er-diagram-1.0.8/tests/test_adders.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_drawing.py` & `dbis-er-diagram-1.0.8/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_getters.py` & `dbis-er-diagram-1.0.8/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_grading_components.py` & `dbis-er-diagram-1.0.8/tests/test_grading_components.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_grading_diagrams.py` & `dbis-er-diagram-1.0.8/tests/test_grading_diagrams.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_grading_special_cases.py` & `dbis-er-diagram-1.0.8/tests/test_grading_special_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,34 +53,14 @@
     submission.add_relation({"U": "(m,n) "}, "R9", {"V": "(n, m)", "W": "(n,n)"})
     submission.add_relation({"X": "(m,n)"}, "R10", {"Y": "(n,m)", "Z": "(1, m)"})
 
     score, log = grade_submission(solution, submission)
     assert score == 0
 
 
-def test_renamed_cardinality_1_n_incorrect():
-    solution = ER()
-    solution.add_relation({"A": "m"}, "R1", {"B": "n", "C": "m"})
-    submission = ER()
-    submission.add_relation({"A": "n"}, "R1", {"B": "m", "C": "m"})
-
-    score, log = grade_submission(solution, submission)
-    assert score > 0
-
-
-def test_renamed_cardinality_min_max_incorrect():
-    solution = ER()
-    solution.add_relation({"A": "(m, n)"}, "R1", {"B": "(n, m)", "C": "(m, n)"})
-    submission = ER()
-    submission.add_relation({"A": "(n, m)"}, "R1", {"B": "(m, n)", "C": "(m, n)"})
-
-    score, log = grade_submission(solution, submission)
-    assert score > 0
-
-
 def test_pk_weak_attribute_incorrect():
     solution = ER()
     solution.add_entity("A", is_weak=True)
     solution.add_attribute("A", "attr", is_pk=True, is_weak=True)
     submission = ER()
     submission.add_entity("A", is_weak=True)
     submission.add_attribute("A", "attr", is_pk=True, is_weak=False)
```

### Comparing `dbis-er-diagram-1.0.7/tests/test_merging.py` & `dbis-er-diagram-1.0.8/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.7/tests/test_other_methods.py` & `dbis-er-diagram-1.0.8/tests/test_other_methods.py`

 * *Files identical despite different names*


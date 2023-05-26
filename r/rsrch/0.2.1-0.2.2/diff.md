# Comparing `tmp/rsrch-0.2.1.tar.gz` & `tmp/rsrch-0.2.2.tar.gz`

## Comparing `rsrch-0.2.1.tar` & `rsrch-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.1/.DS_Store
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.1/examples/yitay.md
--rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.1/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.2/.DS_Store
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.2/examples/yitay.md
+-rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
 Understanding_and_Reduce_the_Spread_of_Misinformation.pdf
--rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.1/papers/Decision_Transformer:_Reinforcement
+-rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.2/papers/Decision_Transformer:_Reinforcement
 Learning_via_Sequence_Modeling.pdf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/__about__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/__init__.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/_src/labml.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/_src/notion.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.1/LICENSE
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rsrch-0.2.1/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 rsrch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/__about__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/__init__.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/_src/labml.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.2/rsrch/_src/notion.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rsrch-0.2.2/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 rsrch-0.2.2/PKG-INFO
```

### Comparing `rsrch-0.2.1/.DS_Store` & `rsrch-0.2.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/examples/yitay.md` & `rsrch-0.2.2/examples/yitay.md`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf` & `rsrch-0.2.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf` & `rsrch-0.2.2/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/rsrch/_src/labml.py` & `rsrch-0.2.2/rsrch/_src/labml.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,22 +44,15 @@
     title = title.translate(str.maketrans("", "", string.punctuation))
 
     search = arxiv.Search(
         query=title,
         max_results=10,
     )
 
-    # Storing the results in a list
-    results = list(search.results())
-
-    # Sorting the results by title match (must be exact)
-    results.sort(key=lambda r: r.title != title)
-    paper = results[0] if results[0].title == title else None
-
-    return paper
+    return next(search.results(), None)
 
 
 def popular(sort_by="weekly", num_papers=5):
     """
     Retrieves popular papers from papers.labml.ai.
 
     Parameters:
```

### Comparing `rsrch-0.2.1/rsrch/_src/notion.py` & `rsrch-0.2.2/rsrch/_src/notion.py`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/LICENSE` & `rsrch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/README.md` & `rsrch-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/pyproject.toml` & `rsrch-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.1/PKG-INFO` & `rsrch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsrch
-Version: 0.2.1
+Version: 0.2.2
 Summary: Manage your ever-growing list of research papers
 Project-URL: Homepage, https://github.com/ishan0102/rsrch
 Project-URL: Bug Tracker, https://github.com/ishan0102/rsrch/issues
 Author-email: Ishan Shah <ishan0102@utexas.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


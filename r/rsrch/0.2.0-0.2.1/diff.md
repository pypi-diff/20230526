# Comparing `tmp/rsrch-0.2.0.tar.gz` & `tmp/rsrch-0.2.1.tar.gz`

## Comparing `rsrch-0.2.0.tar` & `rsrch-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.0/.DS_Store
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.0/examples/yitay.md
--rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.0/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.1/.DS_Store
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.1/examples/yitay.md
+-rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.1/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
 Understanding_and_Reduce_the_Spread_of_Misinformation.pdf
--rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.0/papers/Decision_Transformer:_Reinforcement
+-rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.1/papers/Decision_Transformer:_Reinforcement
 Learning_via_Sequence_Modeling.pdf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/__about__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/__init__.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/_src/labml.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/_src/notion.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.0/LICENSE
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 rsrch-0.2.0/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 rsrch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/__about__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/__init__.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/_src/labml.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.1/rsrch/_src/notion.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 rsrch-0.2.1/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 rsrch-0.2.1/PKG-INFO
```

### Comparing `rsrch-0.2.0/.DS_Store` & `rsrch-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/examples/yitay.md` & `rsrch-0.2.1/examples/yitay.md`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf` & `rsrch-0.2.1/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf` & `rsrch-0.2.1/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/rsrch/_src/labml.py` & `rsrch-0.2.1/rsrch/_src/labml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import string
 import time
 
 import arxiv
 import requests
 from rich.console import Console
 from rich.table import Table
 from selenium import webdriver
@@ -36,14 +37,15 @@
 
     return authorization_token
 
 
 def fetch_paper_details(paper):
     title = paper["title"]["text"].replace("\n", " ")
     title = " ".join(title.split())
+    title = title.translate(str.maketrans("", "", string.punctuation))
 
     search = arxiv.Search(
         query=title,
         max_results=10,
     )
 
     # Storing the results in a list
@@ -119,15 +121,15 @@
                 try:
                     metadata = fetch_paper_details(paper)
                     if metadata is not None:
                         paper_data.append(metadata)
                 except Exception as e:
                     console.print(f"[bold yellow]Error occurred:[/bold yellow] {e}")
 
-            console.print()
+            console.print(f"\nFound {len(paper_data)} out of {len(papers)} paper successfully.\n")
             if len(paper_data) > 0:
                 table = Table(title="Popular Papers", header_style="bold blue")
                 table.add_column("Title")
                 table.add_column("Date")
                 table.add_column("URL")
 
                 for paper in paper_data:
```

### Comparing `rsrch-0.2.0/rsrch/_src/notion.py` & `rsrch-0.2.1/rsrch/_src/notion.py`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/LICENSE` & `rsrch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/README.md` & `rsrch-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,26 @@
 
 <p>
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/232264615-82b42d8c-ca1c-4f21-899f-439a6c8a7879.png">
 </p>
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
+### Popular
+You can get the most popular papers from this day, week, or month from the [LabML database](https://papers.labml.ai/).
+
+```python
+from rsrch import popular
+popular(sort_by="weekly", num_papers=10)
+```
+
+<p>
+    <img width="1095" alt="image" src="https://github.com/ishan0102/rsrch/assets/47067154/b99197a1-8556-4469-82f4-786a4c974447">
+</p>
+
 
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
 - To build and release this:
   - Make new code accessible in `src/__init__.py`
   - Update the version in `src/__about__.py`
```

### Comparing `rsrch-0.2.0/pyproject.toml` & `rsrch-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsrch-0.2.0/PKG-INFO` & `rsrch-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsrch
-Version: 0.2.0
+Version: 0.2.1
 Summary: Manage your ever-growing list of research papers
 Project-URL: Homepage, https://github.com/ishan0102/rsrch
 Project-URL: Bug Tracker, https://github.com/ishan0102/rsrch/issues
 Author-email: Ishan Shah <ishan0102@utexas.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -78,14 +78,26 @@
 
 <p>
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/232264615-82b42d8c-ca1c-4f21-899f-439a6c8a7879.png">
 </p>
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
+### Popular
+You can get the most popular papers from this day, week, or month from the [LabML database](https://papers.labml.ai/).
+
+```python
+from rsrch import popular
+popular(sort_by="weekly", num_papers=10)
+```
+
+<p>
+    <img width="1095" alt="image" src="https://github.com/ishan0102/rsrch/assets/47067154/b99197a1-8556-4469-82f4-786a4c974447">
+</p>
+
 
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
 - To build and release this:
   - Make new code accessible in `src/__init__.py`
   - Update the version in `src/__about__.py`
```


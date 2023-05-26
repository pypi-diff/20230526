# Comparing `tmp/raphtory-0.3.1-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.3.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2831603 bytes, number of entries: 7
--rw-r--r--  4.6 unx     9743 b- defN 23-May-10 14:05 raphtory-0.3.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-May-10 14:05 raphtory-0.3.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     2052 b- defN 23-May-10 14:05 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7531 b- defN 23-May-10 14:05 raphtory/vis.py
--rw-r--r--  4.6 unx      537 b- defN 23-May-10 14:05 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  8094720 b- defN 23-May-10 14:05 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-May-10 14:05 raphtory-0.3.1.dist-info/RECORD
-7 files, 8115210 bytes uncompressed, 2830675 bytes compressed:  65.1%
+Zip file size: 2928225 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9737 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2052 b- defN 23-May-26 16:14 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7552 b- defN 23-May-26 16:14 raphtory/vis.py
+-rw-r--r--  4.6 unx      537 b- defN 23-May-26 16:14 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  8371200 b- defN 23-May-26 16:14 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-May-26 16:14 raphtory-0.3.2.dist-info/RECORD
+7 files, 8391704 bytes uncompressed, 2927297 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.3.1.dist-info/METADATA
+Filename: raphtory-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.3.1.dist-info/WHEEL
+Filename: raphtory-0.3.2.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.3.1.dist-info/RECORD
+Filename: raphtory-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## raphtory/vis.py

```diff
@@ -74,14 +74,15 @@
     for e in graph.edges():
         weight = e.property(edge_weight) if edge_weight != None else 1
         label = e.property(edge_label) if edge_label != None else ""
         visGraph.add_edge(e.src().id(), e.dst().id(), value=weight, color=edge_color, title=label)
        
     visGraph.show_buttons(filter_=['physics'])
     visGraph.show('nx.html')
+    return visGraph
     
 r"""Draw a graph with NetworkX.
 
 .. note::
 
     Network X is a required dependency.
     If you intend to use this function make sure that
```

## Comparing `raphtory-0.3.1.dist-info/METADATA` & `raphtory-0.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3
 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
 Requires-Dist: networkx >=2.6.3 ; extra == 'vis'
 Requires-Dist: matplotlib >=3.4.3 ; extra == 'vis'
 Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis
 Summary: Python package for raphtory, a temporal graph library
 Keywords: graph,temporal-graph,temporal
 Home-Page: https://github.com/Raphtory/raphtory/
 Author: Pometry
-License: AGPL-3.0-only
+License: GPL-3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/pometry/raphtory
 Project-URL: documentation, https://docs.raphtory.com/
 Project-URL: repository, https://github.com/pometry/raphtory
 Project-URL: twitter, https://twitter.com/raphtory/
 Project-URL: slack, https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA
```

### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.3.1 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.3.2 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
 Requires-Dist: networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib
 >=3.4.3 ; extra == 'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis Summary: Python package for raphtory, a temporal graph
 library Keywords: graph,temporal-graph,temporal Home-Page: https://github.com/
-Raphtory/raphtory/ Author: Pometry License: AGPL-3.0-only Requires-Python:
->=3.7 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://github.com/pometry/raphtory Project-URL:
-documentation, https://docs.raphtory.com/ Project-URL: repository, https://
-github.com/pometry/raphtory Project-URL: twitter, https://twitter.com/raphtory/
-Project-URL: slack, https://join.slack.com/t/raphtory/shared_invite/zt-
-xbebws9j-VgPIFRleJFJBwmpf81tvxA Project-URL: youtube, https://www.youtube.com/
+Raphtory/raphtory/ Author: Pometry License: GPL-3.0 Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
+URL: homepage, https://github.com/pometry/raphtory Project-URL: documentation,
+https://docs.raphtory.com/ Project-URL: repository, https://github.com/pometry/
+raphtory Project-URL: twitter, https://twitter.com/raphtory/ Project-URL:
+slack, https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-
+VgPIFRleJFJBwmpf81tvxA Project-URL: youtube, https://www.youtube.com/
 @pometry8546/videos
                                   [Raphtory]
 [Test_and_Build] [Latest_Release] [Issues] [Crates.io] [PyPI] [Launch_Notebook]
 ð_Website   ð_Documentation   [https://user-images.githubusercontent.com/
      6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png]_Pometry  
            ð§ð»â_Tutorial   ð_Report_a_Bug   [https://user-
     images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-4dcf-be03-
```


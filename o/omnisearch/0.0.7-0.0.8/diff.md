# Comparing `tmp/omnisearch-0.0.7.tar.gz` & `tmp/omnisearch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisearch-0.0.7.tar", last modified: Fri May 26 17:21:43 2023, max compression
+gzip compressed data, was "omnisearch-0.0.8.tar", last modified: Fri May 26 17:27:59 2023, max compression
```

## Comparing `omnisearch-0.0.7.tar` & `omnisearch-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.078064 omnisearch-0.0.7/
--rw-rw-rw-   0        0        0     1095 2023-04-18 14:26:53.000000 omnisearch-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2023-05-26 17:21:43.077063 omnisearch-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-26 17:00:13.000000 omnisearch-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.047057 omnisearch-0.0.7/algorithms/
--rw-rw-rw-   0        0        0      382 2023-04-08 14:47:28.000000 omnisearch-0.0.7/algorithms/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/a_star.py
--rw-rw-rw-   0        0        0     2138 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/best_first.py
--rw-rw-rw-   0        0        0     1934 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/branch_and_bound.py
--rw-rw-rw-   0        0        0     1718 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/breadth_first.py
--rw-rw-rw-   0        0        0     1702 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/depth_first.py
--rw-rw-rw-   0        0        0     3047 2023-04-16 18:47:52.000000 omnisearch-0.0.7/algorithms/hill_climbing.py
--rw-rw-rw-   0        0        0     2746 2023-04-16 18:47:52.000000 omnisearch-0.0.7/algorithms/iterative_deepening.py
--rw-rw-rw-   0        0        0     1799 2023-04-17 16:15:55.000000 omnisearch-0.0.7/algorithms/uniform_cost.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.051057 omnisearch-0.0.7/data_structures/
--rw-rw-rw-   0        0        0       93 2023-04-18 13:51:25.000000 omnisearch-0.0.7/data_structures/__init__.py
--rw-rw-rw-   0        0        0     1435 2023-04-18 14:26:53.000000 omnisearch-0.0.7/data_structures/priority_queue.py
--rw-rw-rw-   0        0        0     1028 2023-04-18 14:26:53.000000 omnisearch-0.0.7/data_structures/queue.py
--rw-rw-rw-   0        0        0     1021 2023-04-18 14:26:53.000000 omnisearch-0.0.7/data_structures/stack.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.052059 omnisearch-0.0.7/interfaces/
--rw-rw-rw-   0        0        0       52 2023-03-22 13:45:41.000000 omnisearch-0.0.7/interfaces/__init__.py
--rw-rw-rw-   0        0        0     1746 2023-04-07 15:40:00.000000 omnisearch-0.0.7/interfaces/state_space_problem.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.072063 omnisearch-0.0.7/omnisearch.egg-info/
--rw-rw-rw-   0        0        0      766 2023-05-26 17:21:42.000000 omnisearch-0.0.7/omnisearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-05-26 17:21:42.000000 omnisearch-0.0.7/omnisearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:21:42.000000 omnisearch-0.0.7/omnisearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-26 17:21:42.000000 omnisearch-0.0.7/omnisearch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 17:21:43.076065 omnisearch-0.0.7/problems/
--rw-rw-rw-   0        0        0      142 2023-04-01 17:36:13.000000 omnisearch-0.0.7/problems/__init__.py
--rw-rw-rw-   0        0        0     2159 2023-04-08 13:18:21.000000 omnisearch-0.0.7/problems/maze.py
--rw-rw-rw-   0        0        0     2806 2023-04-19 10:31:02.000000 omnisearch-0.0.7/problems/missionaries_and_cannibals.py
--rw-rw-rw-   0        0        0     1521 2023-04-08 12:12:09.000000 omnisearch-0.0.7/problems/n_queens.py
--rw-rw-rw-   0        0        0       42 2023-05-26 17:21:43.078064 omnisearch-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-05-26 17:21:38.000000 omnisearch-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.233371 omnisearch-0.0.8/
+-rw-rw-rw-   0        0        0     1095 2023-04-18 14:26:53.000000 omnisearch-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2023-05-26 17:27:59.233371 omnisearch-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-26 17:00:13.000000 omnisearch-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.197363 omnisearch-0.0.8/omnisearch/
+-rw-rw-rw-   0        0        0      109 2023-05-26 17:27:37.000000 omnisearch-0.0.8/omnisearch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.222369 omnisearch-0.0.8/omnisearch/algorithms/
+-rw-rw-rw-   0        0        0      382 2023-04-08 14:47:28.000000 omnisearch-0.0.8/omnisearch/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     2406 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/a_star.py
+-rw-rw-rw-   0        0        0     2138 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/best_first.py
+-rw-rw-rw-   0        0        0     1934 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/branch_and_bound.py
+-rw-rw-rw-   0        0        0     1718 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/breadth_first.py
+-rw-rw-rw-   0        0        0     1702 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/depth_first.py
+-rw-rw-rw-   0        0        0     3047 2023-04-16 18:47:52.000000 omnisearch-0.0.8/omnisearch/algorithms/hill_climbing.py
+-rw-rw-rw-   0        0        0     2746 2023-04-16 18:47:52.000000 omnisearch-0.0.8/omnisearch/algorithms/iterative_deepening.py
+-rw-rw-rw-   0        0        0     1799 2023-04-17 16:15:55.000000 omnisearch-0.0.8/omnisearch/algorithms/uniform_cost.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.225370 omnisearch-0.0.8/omnisearch/data_structures/
+-rw-rw-rw-   0        0        0       93 2023-04-18 13:51:25.000000 omnisearch-0.0.8/omnisearch/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     1435 2023-04-18 14:26:53.000000 omnisearch-0.0.8/omnisearch/data_structures/priority_queue.py
+-rw-rw-rw-   0        0        0     1028 2023-04-18 14:26:53.000000 omnisearch-0.0.8/omnisearch/data_structures/queue.py
+-rw-rw-rw-   0        0        0     1021 2023-04-18 14:26:53.000000 omnisearch-0.0.8/omnisearch/data_structures/stack.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.227370 omnisearch-0.0.8/omnisearch/interfaces/
+-rw-rw-rw-   0        0        0       52 2023-03-22 13:45:41.000000 omnisearch-0.0.8/omnisearch/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-04-07 15:40:00.000000 omnisearch-0.0.8/omnisearch/interfaces/state_space_problem.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.232371 omnisearch-0.0.8/omnisearch/problems/
+-rw-rw-rw-   0        0        0      142 2023-04-01 17:36:13.000000 omnisearch-0.0.8/omnisearch/problems/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-08 13:18:21.000000 omnisearch-0.0.8/omnisearch/problems/maze.py
+-rw-rw-rw-   0        0        0     2806 2023-04-19 10:31:02.000000 omnisearch-0.0.8/omnisearch/problems/missionaries_and_cannibals.py
+-rw-rw-rw-   0        0        0     1521 2023-04-08 12:12:09.000000 omnisearch-0.0.8/omnisearch/problems/n_queens.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:27:59.212367 omnisearch-0.0.8/omnisearch.egg-info/
+-rw-rw-rw-   0        0        0      766 2023-05-26 17:27:59.000000 omnisearch-0.0.8/omnisearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-05-26 17:27:59.000000 omnisearch-0.0.8/omnisearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:27:59.000000 omnisearch-0.0.8/omnisearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 17:27:59.000000 omnisearch-0.0.8/omnisearch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:27:59.233371 omnisearch-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-05-26 17:27:53.000000 omnisearch-0.0.8/setup.py
```

### Comparing `omnisearch-0.0.7/LICENSE.txt` & `omnisearch-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/PKG-INFO` & `omnisearch-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnisearch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of state space search algorithms.
 Home-page: https://github.com/chaseburton/polysearch
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omnisearch-0.0.7/algorithms/a_star.py` & `omnisearch-0.0.8/omnisearch/algorithms/a_star.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/best_first.py` & `omnisearch-0.0.8/omnisearch/algorithms/best_first.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/branch_and_bound.py` & `omnisearch-0.0.8/omnisearch/algorithms/branch_and_bound.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/breadth_first.py` & `omnisearch-0.0.8/omnisearch/algorithms/breadth_first.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/depth_first.py` & `omnisearch-0.0.8/omnisearch/algorithms/depth_first.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/hill_climbing.py` & `omnisearch-0.0.8/omnisearch/algorithms/hill_climbing.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/iterative_deepening.py` & `omnisearch-0.0.8/omnisearch/algorithms/iterative_deepening.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/algorithms/uniform_cost.py` & `omnisearch-0.0.8/omnisearch/algorithms/uniform_cost.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/data_structures/priority_queue.py` & `omnisearch-0.0.8/omnisearch/data_structures/priority_queue.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/data_structures/queue.py` & `omnisearch-0.0.8/omnisearch/data_structures/queue.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/data_structures/stack.py` & `omnisearch-0.0.8/omnisearch/data_structures/stack.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/interfaces/state_space_problem.py` & `omnisearch-0.0.8/omnisearch/interfaces/state_space_problem.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/omnisearch.egg-info/PKG-INFO` & `omnisearch-0.0.8/omnisearch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnisearch
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of state space search algorithms.
 Home-page: https://github.com/chaseburton/polysearch
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `omnisearch-0.0.7/problems/maze.py` & `omnisearch-0.0.8/omnisearch/problems/maze.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/problems/missionaries_and_cannibals.py` & `omnisearch-0.0.8/omnisearch/problems/missionaries_and_cannibals.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/problems/n_queens.py` & `omnisearch-0.0.8/omnisearch/problems/n_queens.py`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.7/setup.py` & `omnisearch-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='omnisearch',
-    version='0.0.7',
+    version='0.0.8',
     description='A collection of state space search algorithms.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Chase Burton Taylor',
     author_email='ctaylor@citycollege.sheffield.eu',
     url='https://github.com/chaseburton/polysearch',
     packages=find_packages(),
```


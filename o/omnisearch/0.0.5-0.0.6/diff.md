# Comparing `tmp/omnisearch-0.0.5.tar.gz` & `tmp/omnisearch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisearch-0.0.5.tar", last modified: Fri May 26 17:00:15 2023, max compression
+gzip compressed data, was "omnisearch-0.0.6.tar", last modified: Fri May 26 17:01:32 2023, max compression
```

## Comparing `omnisearch-0.0.5.tar` & `omnisearch-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:00:15.258023 omnisearch-0.0.5/
--rw-rw-rw-   0        0        0     1095 2023-04-18 14:26:53.000000 omnisearch-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      766 2023-05-26 17:00:15.257023 omnisearch-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-05-26 17:00:13.000000 omnisearch-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 17:00:15.256021 omnisearch-0.0.5/omnisearch.egg-info/
--rw-rw-rw-   0        0        0      766 2023-05-26 17:00:15.000000 omnisearch-0.0.5/omnisearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-05-26 17:00:15.000000 omnisearch-0.0.5/omnisearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:00:15.000000 omnisearch-0.0.5/omnisearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:00:15.000000 omnisearch-0.0.5/omnisearch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 17:00:15.258023 omnisearch-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-05-26 16:59:34.000000 omnisearch-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:01:32.744797 omnisearch-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-04-18 14:26:53.000000 omnisearch-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      766 2023-05-26 17:01:32.744797 omnisearch-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-05-26 17:00:13.000000 omnisearch-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 17:01:32.742797 omnisearch-0.0.6/omnisearch.egg-info/
+-rw-rw-rw-   0        0        0      766 2023-05-26 17:01:32.000000 omnisearch-0.0.6/omnisearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-05-26 17:01:32.000000 omnisearch-0.0.6/omnisearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:01:32.000000 omnisearch-0.0.6/omnisearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:01:32.000000 omnisearch-0.0.6/omnisearch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:01:32.744797 omnisearch-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-05-26 17:01:30.000000 omnisearch-0.0.6/setup.py
```

### Comparing `omnisearch-0.0.5/LICENSE.txt` & `omnisearch-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omnisearch-0.0.5/PKG-INFO` & `omnisearch-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: omnisearch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of state space search algorithms.
-Home-page: https://github.com/chaseburton/omnisearch
+Home-page: https://github.com/chaseburton/polysearch
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `omnisearch-0.0.5/omnisearch.egg-info/PKG-INFO` & `omnisearch-0.0.6/omnisearch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: omnisearch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of state space search algorithms.
-Home-page: https://github.com/chaseburton/omnisearch
+Home-page: https://github.com/chaseburton/polysearch
 Author: Chase Burton Taylor
 Author-email: ctaylor@citycollege.sheffield.eu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `omnisearch-0.0.5/setup.py` & `omnisearch-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='omnisearch',
-    version='0.0.5',
+    version='0.0.6',
     description='A collection of state space search algorithms.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Chase Burton Taylor',
     author_email='ctaylor@citycollege.sheffield.eu',
-    url='https://github.com/chaseburton/omnisearch',
+    url='https://github.com/chaseburton/polysearch',
     packages=find_packages(),
     install_requires=[
         # None since heapq, abc, and time are built-in modules.
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```


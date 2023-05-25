# Comparing `tmp/gscdash-0.0.2.tar.gz` & `tmp/gscdash-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscdash-0.0.2.tar", last modified: Thu May 25 21:56:06 2023, max compression
+gzip compressed data, was "gscdash-0.0.3.tar", last modified: Thu May 25 22:05:08 2023, max compression
```

## Comparing `gscdash-0.0.2.tar` & `gscdash-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,28 @@
-drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:56:06.243268 gscdash-0.0.2/
--rw-r--r--   0 zives      (501) staff       (20)    34523 2023-04-14 14:43:14.000000 gscdash-0.0.2/LICENSE.TXT
--rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:56:06.243338 gscdash-0.0.2/PKG-INFO
--rw-r--r--   0 zives      (501) staff       (20)     4831 2023-05-25 21:44:35.000000 gscdash-0.0.2/README.md
-drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 21:56:06.243068 gscdash-0.0.2/gscdash.egg-info/
--rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/PKG-INFO
--rw-r--r--   0 zives      (501) staff       (20)      209 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/SOURCES.txt
--rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/dependency_links.txt
--rw-r--r--   0 zives      (501) staff       (20)       62 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/requires.txt
--rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 21:56:06.000000 gscdash-0.0.2/gscdash.egg-info/top_level.txt
--rw-r--r--   0 zives      (501) staff       (20)      255 2023-05-25 21:55:55.000000 gscdash-0.0.2/pyproject.toml
--rw-r--r--   0 zives      (501) staff       (20)      185 2023-05-25 21:56:06.243600 gscdash-0.0.2/setup.cfg
--rw-r--r--   0 zives      (501) staff       (20)      951 2023-05-25 21:55:51.000000 gscdash-0.0.2/setup.py
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 22:05:08.958767 gscdash-0.0.3/
+-rw-r--r--   0 zives      (501) staff       (20)    34523 2023-04-14 14:43:14.000000 gscdash-0.0.3/LICENSE.TXT
+-rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 22:05:08.958825 gscdash-0.0.3/PKG-INFO
+-rw-r--r--   0 zives      (501) staff       (20)     4831 2023-05-25 21:44:35.000000 gscdash-0.0.3/README.md
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 22:05:08.956713 gscdash-0.0.3/gscdash/
+-rw-r--r--   0 zives      (501) staff       (20)        0 2023-05-25 21:21:13.000000 gscdash-0.0.3/gscdash/__init__.py
+-rw-r--r--   0 zives      (501) staff       (20)     3398 2023-05-25 17:42:04.000000 gscdash-0.0.3/gscdash/course_info.py
+-rw-r--r--   0 zives      (501) staff       (20)     1333 2023-05-25 14:51:58.000000 gscdash-0.0.3/gscdash/export_events.py
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 22:05:08.957666 gscdash-0.0.3/gscdash/pycanvas/
+-rw-r--r--   0 zives      (501) staff       (20)     4537 2023-05-25 17:42:41.000000 gscdash-0.0.3/gscdash/pycanvas/canvas_status.py
+-rw-r--r--   0 zives      (501) staff       (20)     9784 2023-05-24 21:34:09.000000 gscdash-0.0.3/gscdash/pycanvas/pycanvas.py
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 22:05:08.958628 gscdash-0.0.3/gscdash/pyscope/
+-rw-r--r--   0 zives      (501) staff       (20)     2369 2023-05-25 14:59:19.000000 gscdash-0.0.3/gscdash/pyscope/account.py
+-rw-r--r--   0 zives      (501) staff       (20)     6182 2023-05-23 20:41:27.000000 gscdash-0.0.3/gscdash/pyscope/assignment.py
+-rw-r--r--   0 zives      (501) staff       (20)    14071 2023-05-25 18:15:17.000000 gscdash-0.0.3/gscdash/pyscope/course.py
+-rw-r--r--   0 zives      (501) staff       (20)     5708 2023-05-25 20:54:34.000000 gscdash-0.0.3/gscdash/pyscope/gs_status.py
+-rw-r--r--   0 zives      (501) staff       (20)     1230 2023-05-23 20:41:27.000000 gscdash-0.0.3/gscdash/pyscope/person.py
+-rw-r--r--   0 zives      (501) staff       (20)     7889 2023-05-25 20:52:16.000000 gscdash-0.0.3/gscdash/pyscope/pyscope.py
+-rw-r--r--   0 zives      (501) staff       (20)      733 2023-04-14 14:43:14.000000 gscdash-0.0.3/gscdash/pyscope/question.py
+drwxr-xr-x   0 zives      (501) staff       (20)        0 2023-05-25 22:05:08.957395 gscdash-0.0.3/gscdash.egg-info/
+-rw-r--r--   0 zives      (501) staff       (20)     5304 2023-05-25 22:05:08.000000 gscdash-0.0.3/gscdash.egg-info/PKG-INFO
+-rw-r--r--   0 zives      (501) staff       (20)      533 2023-05-25 22:05:08.000000 gscdash-0.0.3/gscdash.egg-info/SOURCES.txt
+-rw-r--r--   0 zives      (501) staff       (20)        1 2023-05-25 22:05:08.000000 gscdash-0.0.3/gscdash.egg-info/dependency_links.txt
+-rw-r--r--   0 zives      (501) staff       (20)       62 2023-05-25 22:05:08.000000 gscdash-0.0.3/gscdash.egg-info/requires.txt
+-rw-r--r--   0 zives      (501) staff       (20)        8 2023-05-25 22:05:08.000000 gscdash-0.0.3/gscdash.egg-info/top_level.txt
+-rw-r--r--   0 zives      (501) staff       (20)      255 2023-05-25 22:05:04.000000 gscdash-0.0.3/pyproject.toml
+-rw-r--r--   0 zives      (501) staff       (20)      185 2023-05-25 22:05:08.959054 gscdash-0.0.3/setup.cfg
+-rw-r--r--   0 zives      (501) staff       (20)      918 2023-05-25 22:04:54.000000 gscdash-0.0.3/setup.py
```

### Comparing `gscdash-0.0.2/LICENSE.TXT` & `gscdash-0.0.3/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `gscdash-0.0.2/PKG-INFO` & `gscdash-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscdash
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gradescope-Canvas Dashboard support
 Home-page: https://github.com/upenn/gradescope-canvas-dashboard
 Author: Zack Ives
 Author-email: zives@cis.upenn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `gscdash-0.0.2/README.md` & `gscdash-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gscdash-0.0.2/gscdash.egg-info/PKG-INFO` & `gscdash-0.0.3/gscdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscdash
-Version: 0.0.2
+Version: 0.0.3
 Summary: Gradescope-Canvas Dashboard support
 Home-page: https://github.com/upenn/gradescope-canvas-dashboard
 Author: Zack Ives
 Author-email: zives@cis.upenn.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `gscdash-0.0.2/setup.py` & `gscdash-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "gscdash",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Zack Ives",
     author_email = "zives@cis.upenn.edu",
     description = "Gradescope-Canvas Dashboard support",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/upenn/gradescope-canvas-dashboard",
     classifiers = [
@@ -22,11 +22,10 @@
         "html5lib",
         "beautifulsoup4",
         "canvasapi",
         "pandas",
         "pytz",
         "pyyaml",
     ],
-    package_dir = {"gscdash": "gscdash"},
-    packages = setuptools.find_packages(where="gscdash"),
+    packages = ["gscdash", "gscdash.pycanvas", "gscdash.pyscope"],
     python_requires = ">=3.9"
 )
```


# Comparing `tmp/livestream_monitor_classifier-0.0.2.tar.gz` & `tmp/livestream_monitor_classifier-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestream_monitor_classifier-0.0.2.tar", last modified: Fri May 26 20:54:19 2023, max compression
+gzip compressed data, was "livestream_monitor_classifier-0.0.3.tar", last modified: Fri May 26 20:57:25 2023, max compression
```

## Comparing `livestream_monitor_classifier-0.0.2.tar` & `livestream_monitor_classifier-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.784567 livestream_monitor_classifier-0.0.2/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1061 2023-05-26 19:34:03.000000 livestream_monitor_classifier-0.0.2/LICENSE.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      124 2023-05-26 20:15:08.000000 livestream_monitor_classifier-0.0.2/MANIFEST.in
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:54:19.784716 livestream_monitor_classifier-0.0.2/PKG-INFO
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       99 2023-05-24 20:43:52.000000 livestream_monitor_classifier-0.0.2/README.md
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.775608 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       28 2023-05-26 19:18:27.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/__init__.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.779354 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/__pycache__/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      272 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1400 2023-05-26 20:23:44.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.779715 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/data/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     6460 2023-05-26 19:13:41.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/data/stopwords-custom.txt
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.780859 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 19:18:18.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/__init__.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.781623 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/__pycache__/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      240 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     2025 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1493 2023-05-26 19:16:55.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/preprocess.py
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      896 2023-05-26 20:23:43.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/main.py
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.781999 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/model/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)   356572 2023-05-26 19:30:26.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/model/sklearn_MNB.model
-drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:54:19.778343 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:54:19.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/PKG-INFO
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      886 2023-05-26 20:54:19.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        1 2023-05-26 20:54:19.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       41 2023-05-26 20:54:19.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/requires.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       30 2023-05-26 20:54:19.000000 livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/top_level.txt
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      173 2023-05-26 20:54:19.785361 livestream_monitor_classifier-0.0.2/setup.cfg
--rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1807 2023-05-26 20:53:14.000000 livestream_monitor_classifier-0.0.2/setup.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.656480 livestream_monitor_classifier-0.0.3/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1061 2023-05-26 19:34:03.000000 livestream_monitor_classifier-0.0.3/LICENSE.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      124 2023-05-26 20:15:08.000000 livestream_monitor_classifier-0.0.3/MANIFEST.in
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:57:25.656566 livestream_monitor_classifier-0.0.3/PKG-INFO
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       99 2023-05-24 20:43:52.000000 livestream_monitor_classifier-0.0.3/README.md
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.649282 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       28 2023-05-26 19:18:27.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__init__.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.651108 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      272 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1400 2023-05-26 20:23:44.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.651631 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     6460 2023-05-26 19:13:41.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/stopwords-custom.txt
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.652191 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 19:18:18.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__init__.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.654353 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      240 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     2025 2023-05-26 20:22:47.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1493 2023-05-26 19:16:55.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/preprocess.py
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      896 2023-05-26 20:23:43.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/main.py
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.654715 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)   356572 2023-05-26 19:30:26.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/sklearn_MNB.model
+drwxr-xr-x   0 rahmadfirmansyah   (501) staff       (20)        0 2023-05-26 20:57:25.650502 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      864 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      886 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)        1 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       46 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/requires.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)       30 2023-05-26 20:57:25.000000 livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/top_level.txt
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)      173 2023-05-26 20:57:25.657003 livestream_monitor_classifier-0.0.3/setup.cfg
+-rw-r--r--   0 rahmadfirmansyah   (501) staff       (20)     1812 2023-05-26 20:56:46.000000 livestream_monitor_classifier-0.0.3/setup.py
```

### Comparing `livestream_monitor_classifier-0.0.2/LICENSE.txt` & `livestream_monitor_classifier-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/PKG-INFO` & `livestream_monitor_classifier-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: livestream_monitor_classifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Machine Learning Classifier that used to for my personal thesis project called livestream monitor
 Home-page: https://github.com/rfirmansyh/livestream_monitor_classifier
-Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.2.tar.gz
+Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz
 Author: Rahmad Firmansyah
 Author-email: rahmadfirmansyah.id@gmail.com
 License: MIT
 Keywords: rfirmansyh,livestream_monitor_classifier
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/data/stopwords-custom.txt` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/data/stopwords-custom.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/__pycache__/preprocess.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/helper/preprocess.py` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/helper/preprocess.py`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/main.py` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/main.py`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier/model/sklearn_MNB.model` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier/model/sklearn_MNB.model`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/PKG-INFO` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: livestream-monitor-classifier
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Machine Learning Classifier that used to for my personal thesis project called livestream monitor
 Home-page: https://github.com/rfirmansyh/livestream_monitor_classifier
-Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.2.tar.gz
+Download-URL: https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz
 Author: Rahmad Firmansyah
 Author-email: rahmadfirmansyah.id@gmail.com
 License: MIT
 Keywords: rfirmansyh,livestream_monitor_classifier
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `livestream_monitor_classifier-0.0.2/livestream_monitor_classifier.egg-info/SOURCES.txt` & `livestream_monitor_classifier-0.0.3/livestream_monitor_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livestream_monitor_classifier-0.0.2/setup.py` & `livestream_monitor_classifier-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from distutils.core import setup
 
 
 setup(
     name='livestream_monitor_classifier',
     packages=['livestream_monitor_classifier'],
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='A Machine Learning Classifier that used to for my personal thesis project called livestream monitor',   # Give a short description about your library
     author='Rahmad Firmansyah',                   # Type in your name
     author_email='rahmadfirmansyah.id@gmail.com',      # Type in your E-Mail
     url='https://github.com/rfirmansyh/livestream_monitor_classifier',   # Provide either the link to your github or to your website
-    download_url='https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.2.tar.gz',    # I explain this later on
+    download_url='https://github.com/rfirmansyh/livestream_monitor_classifier/archive/refs/tags/v0.0.3.tar.gz',    # I explain this later on
     keywords=['rfirmansyh', 'livestream_monitor_classifier'],   # Keywords that define your package best
     install_requires=[            # I get to this in a second
-        'sklearn',
+        'scikit-learn',
         'pandas',
         'joblib',
         'sastrawi',
         'unidecode',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```


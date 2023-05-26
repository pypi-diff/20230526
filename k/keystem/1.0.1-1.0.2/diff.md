# Comparing `tmp/keystem-1.0.1.tar.gz` & `tmp/keystem-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/naga/Documents/projects/mine/keyroot/dist/.tmp-mfccypam/keystem-1.0.1.tar", last modified: Fri May 19 06:11:19 2023, max compression
+gzip compressed data, was "/Users/naga/Documents/projects/mine/keyroot/dist/.tmp-xgrmlnem/keystem-1.0.2.tar", last modified: Fri May 26 11:12:39 2023, max compression
```

## Comparing `keystem-1.0.1.tar` & `keystem-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-19 06:11:19.000000 keystem-1.0.1/
--rw-r--r--   0 naga       (501) staff       (20)     9077 2023-05-19 06:11:19.000000 keystem-1.0.1/PKG-INFO
--rw-r--r--   0 naga       (501) staff       (20)     8499 2023-05-19 06:04:13.000000 keystem-1.0.1/README.md
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem/
--rwxrwxrwx   0 naga       (501) staff       (20)       22 2023-05-18 19:25:08.000000 keystem-1.0.1/keystem/__init__.py
--rw-r--r--   0 naga       (501) staff       (20)     1735 2023-05-18 19:02:03.000000 keystem-1.0.1/keystem/_kmeans.py
--rwxrwxrwx   0 naga       (501) staff       (20)     3080 2023-05-18 19:34:14.000000 keystem-1.0.1/keystem/keystem.py
-drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/
--rw-r--r--   0 naga       (501) staff       (20)     9077 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/PKG-INFO
--rw-r--r--   0 naga       (501) staff       (20)      290 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/SOURCES.txt
--rw-r--r--   0 naga       (501) staff       (20)        1 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/dependency_links.txt
--rw-r--r--   0 naga       (501) staff       (20)       55 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/entry_points.txt
--rw-r--r--   0 naga       (501) staff       (20)      144 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/requires.txt
--rw-r--r--   0 naga       (501) staff       (20)        8 2023-05-19 06:11:19.000000 keystem-1.0.1/keystem.egg-info/top_level.txt
--rwxrwxrwx   0 naga       (501) staff       (20)     3289 2023-05-19 05:48:17.000000 keystem-1.0.1/keystem.py
--rw-r--r--   0 naga       (501) staff       (20)     1356 2023-05-19 06:10:43.000000 keystem-1.0.1/pyproject.toml
--rw-r--r--   0 naga       (501) staff       (20)       38 2023-05-19 06:11:19.000000 keystem-1.0.1/setup.cfg
--rwxrwxrwx   0 naga       (501) staff       (20)      886 2023-05-19 06:10:17.000000 keystem-1.0.1/setup.py
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 11:12:39.000000 keystem-1.0.2/
+-rw-r--r--   0 naga       (501) staff       (20)     9077 2023-05-26 11:12:39.000000 keystem-1.0.2/PKG-INFO
+-rwxrwxrwx   0 naga       (501) staff       (20)     8499 2023-05-26 11:09:18.000000 keystem-1.0.2/README.md
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem/
+-rwxrwxrwx   0 naga       (501) staff       (20)       22 2023-05-18 19:25:08.000000 keystem-1.0.2/keystem/__init__.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     1735 2023-05-26 11:09:18.000000 keystem-1.0.2/keystem/_kmeans.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     3198 2023-05-26 11:09:18.000000 keystem-1.0.2/keystem/keystem.py
+drwxr-xr-x   0 naga       (501) staff       (20)        0 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/
+-rwxrwxrwx   0 naga       (501) staff       (20)     9077 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/PKG-INFO
+-rwxrwxrwx   0 naga       (501) staff       (20)      290 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)        1 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)       55 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/entry_points.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)      144 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/requires.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)        8 2023-05-26 11:12:39.000000 keystem-1.0.2/keystem.egg-info/top_level.txt
+-rwxrwxrwx   0 naga       (501) staff       (20)     3289 2023-05-19 05:48:17.000000 keystem-1.0.2/keystem.py
+-rwxrwxrwx   0 naga       (501) staff       (20)     1356 2023-05-26 11:09:18.000000 keystem-1.0.2/pyproject.toml
+-rw-r--r--   0 naga       (501) staff       (20)       38 2023-05-26 11:12:39.000000 keystem-1.0.2/setup.cfg
+-rwxrwxrwx   0 naga       (501) staff       (20)     1111 2023-05-26 11:09:18.000000 keystem-1.0.2/setup.py
```

### Comparing `keystem-1.0.1/PKG-INFO` & `keystem-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystem
-Version: 1.0.1
+Version: 1.0.2
 Summary: Extract the keywords from the given text and assign root of the key for each cluster keys
 Home-page: https://github.com/Nagakiran1/keystem.git
 Author: Naga
 Author-email: Naga <naga@caspai.in>
 Project-URL: Homepage, https://github.com/Nagakiran1/keystem
 Keywords: text,keywords,bert,keybert
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keystem-1.0.1/README.md` & `keystem-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `keystem-1.0.1/keystem/_kmeans.py` & `keystem-1.0.2/keystem/_kmeans.py`

 * *Files identical despite different names*

### Comparing `keystem-1.0.1/keystem/keystem.py` & `keystem-1.0.2/keystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,24 +57,28 @@
             else: 
                 tags.append(doc[i])
                 
         return tags 
 
     def get_keygroups(
         self,
-        text
+        text='',
+        keyphrase_ngram_range=(1,2),
+        keywords=[],
+        stop_words=None,
+        keyword_threshold=0.3
     ):
-        # text = rashes_text
-        sents = nltk.tokenize.sent_tokenize(text)
-
-        keywords = []
-        for sent in sents:
-            phrases = self.kw_model.extract_keywords(sent, keyphrase_ngram_range=(1, 2), stop_words=None)
-            keywords.extend([p for p in phrases if p[1]>0.3])
-
+        if text and not keywords:
+            # text = rashes_text
+            sents = nltk.tokenize.sent_tokenize(text)
+
+            keywords = []
+            for sent in sents:
+                phrases = self.kw_model.extract_keywords(sent, keyphrase_ngram_range=keyphrase_ngram_range, stop_words=stop_words)
+                keywords.extend([p for p in phrases if p[1]>keyword_threshold])
 
         res = pd.DataFrame()
         res['keywords'] = keywords
         res['text'] = [p[0] for p in res['keywords']]
 
 
         res['features'] = res['text'].apply(lambda x: self.preprocess(x, pos=False))
```

### Comparing `keystem-1.0.1/keystem.egg-info/PKG-INFO` & `keystem-1.0.2/keystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystem
-Version: 1.0.1
+Version: 1.0.2
 Summary: Extract the keywords from the given text and assign root of the key for each cluster keys
 Home-page: https://github.com/Nagakiran1/keystem.git
 Author: Naga
 Author-email: Naga <naga@caspai.in>
 Project-URL: Homepage, https://github.com/Nagakiran1/keystem
 Keywords: text,keywords,bert,keybert
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `keystem-1.0.1/keystem.py` & `keystem-1.0.2/keystem/keystem.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,28 +57,27 @@
             else: 
                 tags.append(doc[i])
                 
         return tags 
 
     def get_keygroups(
         self,
-        text='',
-        keyphrase_ngram_range=(1,2),
-        keywords=[],
-        stop_words=None,
-        keyword_threshold=0.3
+        text
     ):
-        if text and not keywords:
+        if isinstance(text, list) and text:
+            keywords = text
+        else:
             # text = rashes_text
             sents = nltk.tokenize.sent_tokenize(text)
 
             keywords = []
             for sent in sents:
-                phrases = self.kw_model.extract_keywords(sent, keyphrase_ngram_range=keyphrase_ngram_range, stop_words=stop_words)
-                keywords.extend([p for p in phrases if p[1]>keyword_threshold])
+                phrases = self.kw_model.extract_keywords(sent, keyphrase_ngram_range=(1, 2), stop_words=None)
+                keywords.extend([p for p in phrases if p[1]>0.3])
+        
 
         res = pd.DataFrame()
         res['keywords'] = keywords
         res['text'] = [p[0] for p in res['keywords']]
 
 
         res['features'] = res['text'].apply(lambda x: self.preprocess(x, pos=False))
```

### Comparing `keystem-1.0.1/pyproject.toml` & `keystem-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keystem"
-version = "1.0.1"
+version = "1.0.2"
 description = "Extract the keywords from the given text and assign root of the key for each cluster keys"
 readme = "README.md"
 authors = [{ name = "Naga", email = "naga@caspai.in" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `keystem-1.0.1/setup.py` & `keystem-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # +
 from setuptools import find_packages, setup
 
 setup(
     name = "keystem",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "Naga",
     author_email = "naga@caspai.in",
     description = "This project helps to have git version for S3 buckets."  ,
     url = "https://github.com/Nagakiran1/keystem.git",
     py_modules=['keystem.keyroots', 'keystem'],
     include_package_data=True,
     classifiers=[
@@ -24,8 +24,14 @@
         'pandas>=1.1.5',
         'numpy>=1.19.5'
         ],
     python_requires='>=3.6.0'
     
 )
 
-    # python setup.py sdist bdist_wheel
+# https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
+# python setup.py sdist bdist_wheel
+
+# to build and push library 
+# Change version in pyproject and setup
+# python3 -m build
+# twine upload --repository testpypi dist/*
```


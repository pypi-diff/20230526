# Comparing `tmp/aiogrobid-0.1.5.tar.gz` & `tmp/aiogrobid-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogrobid-0.1.5.tar", last modified: Fri May 26 07:49:29 2023, max compression
+gzip compressed data, was "aiogrobid-0.1.6.tar", last modified: Fri May 26 07:51:05 2023, max compression
```

## Comparing `aiogrobid-0.1.5.tar` & `aiogrobid-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:49:29.949994 aiogrobid-0.1.5/
--rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.5/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 07:49:29.950137 aiogrobid-0.1.5/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.5/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:49:29.947256 aiogrobid-0.1.5/aiogrobid/
--rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.5/aiogrobid/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      397 2023-05-26 07:44:21.000000 aiogrobid-0.1.5/aiogrobid/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     3669 2023-05-26 07:49:14.000000 aiogrobid-0.1.5/aiogrobid/client.py
--rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.5/aiogrobid/exceptions.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:49:29.949702 aiogrobid-0.1.5/aiogrobid.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      325 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       50 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       59 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-05-26 07:49:29.000000 aiogrobid-0.1.5/aiogrobid.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      613 2023-05-26 07:49:29.950851 aiogrobid-0.1.5/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:51:05.442025 aiogrobid-0.1.6/
+-rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.6/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 07:51:05.442130 aiogrobid-0.1.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.6/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:51:05.439622 aiogrobid-0.1.6/aiogrobid/
+-rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.6/aiogrobid/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      397 2023-05-26 07:44:21.000000 aiogrobid-0.1.6/aiogrobid/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3706 2023-05-26 07:50:40.000000 aiogrobid-0.1.6/aiogrobid/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.6/aiogrobid/exceptions.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 07:51:05.441796 aiogrobid-0.1.6/aiogrobid.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      325 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       50 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       59 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-05-26 07:51:05.000000 aiogrobid-0.1.6/aiogrobid.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      613 2023-05-26 07:51:05.442627 aiogrobid-0.1.6/setup.cfg
```

### Comparing `aiogrobid-0.1.5/LICENSE` & `aiogrobid-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.5/PKG-INFO` & `aiogrobid-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.5/README.md` & `aiogrobid-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.5/aiogrobid/client.py` & `aiogrobid-0.1.6/aiogrobid/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,18 @@
         return result.strip()
 
     def _extract_references(self, node):
         bibliography = node.find('.//{http://www.tei-c.org/ns/1.0}listBibl')
         references = []
         for bibl_struct in bibliography:
             analytic = bibl_struct.find('.//{http://www.tei-c.org/ns/1.0}analytic')
-            idno = analytic.find(".//{http://www.tei-c.org/ns/1.0}idno[@type='DOI']")
-            if idno:
-                references.append(idno.text.lower().strip())
+            if analytic:
+                idno = analytic.find(".//{http://www.tei-c.org/ns/1.0}idno[@type='DOI']")
+                if idno:
+                    references.append(idno.text.lower().strip())
         return references
 
     def _exract_authors(self, node):
         node = node.find(".//{http://www.tei-c.org/ns/1.0}sourceDesc")
         authors = []
         for author in node.findall('.//{http://www.tei-c.org/ns/1.0}author'):
             pers_name = author.find('.//{http://www.tei-c.org/ns/1.0}persName')
```

### Comparing `aiogrobid-0.1.5/aiogrobid.egg-info/PKG-INFO` & `aiogrobid-0.1.6/aiogrobid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.5
+Version: 0.1.6
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.5/setup.cfg` & `aiogrobid-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = 
 	Topic :: Utilities
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = aiogrobid
 python_requires = '>=3.8',
-version = 0.1.5
+version = 0.1.6
 url = https://github.com/izihawa/aiogrobid
 
 [options]
 packages = find:
 install_requires = 
 	aiobaseclient >= 0.2.4
 	fire >= 0.3.1
```


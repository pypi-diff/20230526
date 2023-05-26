# Comparing `tmp/askCO-0.0.8.tar.gz` & `tmp/askCO-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.8.tar", last modified: Tue May 23 23:37:07 2023, max compression
+gzip compressed data, was "askCO-0.0.9.tar", last modified: Fri May 26 02:36:15 2023, max compression
```

## Comparing `askCO-0.0.8.tar` & `askCO-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.493689 askCO-0.0.8/
--rw-rw-rw-   0        0        0     3994 2023-05-23 23:37:07.493689 askCO-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.8/README.md
--rw-rw-rw-   0        0        0      676 2023-05-23 23:36:25.000000 askCO-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 23:37:07.493689 askCO-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.462447 askCO-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.478063 askCO-0.0.8/src/askCO/
--rw-rw-rw-   0        0        0     9721 2023-05-23 23:30:08.000000 askCO-0.0.8/src/askCO/__init__.py
--rw-rw-rw-   0        0        0     2387 2023-05-23 23:35:16.000000 askCO-0.0.8/src/askCO/tryCO.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:37:07.493689 askCO-0.0.8/src/askCO.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 23:37:07.000000 askCO-0.0.8/src/askCO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:15.402690 askCO-0.0.9/
+-rw-rw-rw-   0        0        0     3994 2023-05-26 02:36:15.387066 askCO-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3424 2023-05-23 00:07:57.000000 askCO-0.0.9/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-26 02:34:44.000000 askCO-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 02:36:15.402690 askCO-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:15.355809 askCO-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:15.371429 askCO-0.0.9/src/askCO/
+-rw-rw-rw-   0        0        0     9758 2023-05-26 02:34:00.000000 askCO-0.0.9/src/askCO/__init__.py
+-rw-rw-rw-   0        0        0     2387 2023-05-23 23:35:16.000000 askCO-0.0.9/src/askCO/tryCO.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:15.387066 askCO-0.0.9/src/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3994 2023-05-26 02:36:15.000000 askCO-0.0.9/src/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-26 02:36:15.000000 askCO-0.0.9/src/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 02:36:15.000000 askCO-0.0.9/src/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 02:36:15.000000 askCO-0.0.9/src/askCO.egg-info/top_level.txt
```

### Comparing `askCO-0.0.8/PKG-INFO` & `askCO-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `askCO-0.0.8/README.md` & `askCO-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `askCO-0.0.8/pyproject.toml` & `askCO-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "askCO"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
 	{name = "Lucy Schrader", email = "lucy@schrader.nz"},
 ]
 description = "Python interface for Te Papa's collections API"
 readme = "README.md"
 keywords = ["python", "museum", "api"]
 requires-python = ">=3.7"
```

### Comparing `askCO-0.0.8/src/askCO/__init__.py` & `askCO-0.0.9/src/askCO/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,16 @@
 		# Save the result count for the search or scroll, save records
 		response_text = json.loads(self.response.text)
 		if not self.record_count:
 			self.record_count = response_text["_metadata"]["resultset"]["count"]
 			if not self.quiet:
 				print("Retrieving {} records".format(self.record_count))
 
-		self.records.extend([result for result in response_text["results"]])
+		if response_text.get("results"):
+			self.records.extend([result for result in response_text["results"]])
 
 class Search(Request):
 	def __init__(self, **kwargs):
 		Request.__init__(self, **kwargs)
 		# Build a search for a specified page of results
 		self.query_type = "search"
 		self.query = kwargs.get("query")
```

### Comparing `askCO-0.0.8/src/askCO/tryCO.py` & `askCO-0.0.9/src/askCO/tryCO.py`

 * *Files identical despite different names*

### Comparing `askCO-0.0.8/src/askCO.egg-info/PKG-INFO` & `askCO-0.0.9/src/askCO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askCO
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python interface for Te Papa's collections API
 Author-email: Lucy Schrader <lucy@schrader.nz>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucyschrader/askCO
 Keywords: python,museum,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```


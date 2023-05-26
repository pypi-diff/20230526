# Comparing `tmp/fairly-0.3.0.tar.gz` & `tmp/fairly-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairly-0.3.0.tar", last modified: Wed Mar 22 10:34:40 2023, max compression
+gzip compressed data, was "fairly-0.4.0.tar", last modified: Fri May 26 18:51:29 2023, max compression
```

## Comparing `fairly-0.3.0.tar` & `fairly-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-22 10:34:28.000000 fairly-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 10:34:28.000000 fairly-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-22 10:34:40.991628 fairly-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-22 10:34:28.000000 fairly-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-22 10:34:28.000000 fairly-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-22 10:34:40.991628 fairly-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.987628 fairly-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.987628 fairly-0.3.0/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-22 10:34:28.000000 fairly-0.3.0/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-22 10:34:28.000000 fairly-0.3.0/src/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-03-22 10:34:28.000000 fairly-0.3.0/src/cli/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.987628 fairly-0.3.0/src/fairly/
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/client/
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/client/dataverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/client/djehuty.py
--rw-r--r--   0 runner    (1001) docker     (123)    31371 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/client/figshare.py
--rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/client/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/data/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/data/languages/
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/languages/ISO-639-2_8859-1.tab
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab
--rw-r--r--   0 runner    (1001) docker     (123)   201810 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/languages/ISO-639-3_8859-1.tab
--rw-r--r--   0 runner    (1001) docker     (123)   202920 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/templates/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/templates/figshare.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/data/templates/zenodo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/dataset/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/dataset/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/file/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/file/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-03-22 10:34:28.000000 fairly-0.3.0/src/fairly/person.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/src/fairly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 10:34:40.000000 fairly-0.3.0/src/fairly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 10:34:40.991628 fairly-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-22 10:34:28.000000 fairly-0.3.0/tests/test_fairly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.852438 fairly-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 18:51:12.000000 fairly-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 18:51:12.000000 fairly-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-26 18:51:29.852438 fairly-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-26 18:51:12.000000 fairly-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 18:51:12.000000 fairly-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 18:51:29.852438 fairly-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.844437 fairly-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.844437 fairly-0.4.0/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-26 18:51:12.000000 fairly-0.4.0/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-26 18:51:12.000000 fairly-0.4.0/src/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-26 18:51:12.000000 fairly-0.4.0/src/cli/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.848438 fairly-0.4.0/src/fairly/
+-rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.848438 fairly-0.4.0/src/fairly/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/client/dataverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/client/djehuty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31371 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/client/figshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33394 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/client/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.848438 fairly-0.4.0/src/fairly/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.848438 fairly-0.4.0/src/fairly/data/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/languages/ISO-639-2_8859-1.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   201810 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/languages/ISO-639-3_8859-1.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   202920 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.852438 fairly-0.4.0/src/fairly/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/templates/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/templates/figshare.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/data/templates/zenodo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.852438 fairly-0.4.0/src/fairly/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20870 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/dataset/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/dataset/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.852438 fairly-0.4.0/src/fairly/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/file/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/file/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-05-26 18:51:12.000000 fairly-0.4.0/src/fairly/person.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.848438 fairly-0.4.0/src/fairly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 18:51:29.000000 fairly-0.4.0/src/fairly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:51:29.852438 fairly-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-26 18:51:12.000000 fairly-0.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-26 18:51:12.000000 fairly-0.4.0/tests/test_fairly.py
```

### Comparing `fairly-0.3.0/LICENSE` & `fairly-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/pyproject.toml` & `fairly-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [project]
 name = "fairly"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Serkan Girgin", email="s.girgin@utwente.nl" },
   { name="Manuel Garcia Alvarez", email="m.g.garciaalvarez@tudelft.nl" },
   { name="Jose Urra Llanusa", email="j.c.urrallanusa@tudelft.nl" }, ]
 description = "A package to create, publish, and download research datasets"
-readme = "README.md"
+readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent", ]
 dependencies = [
     "python-dateutil",
     "requests",
 		"requests_toolbelt",
-    "ruamel.yaml",
-    "typer>=0.6.1",
+    "ruamel.yaml>=0.17.26",
+    "typer>=0.9.0",
     "rich"
     ]
 keywords = ["fairly", "open science", "research data", "data management"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
-    "pytest-recording",
-    "python-dotenv",
-    "vcrpy"
+    "python-dotenv"
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/ITC-CRIB/fairly"
 "Bug Tracker" = "https://github.com/ITC-CRIB/fairly/issues"
 "Documentation" = "https://fairly.readthedocs.io/en/latest/"
 "Funding" = "https://nwo.nl/en/researchprogrammes/open-science/open-science-fund"
```

### Comparing `fairly-0.3.0/src/cli/__init__.py` & `fairly-0.4.0/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/cli/config.py` & `fairly-0.4.0/src/cli/config.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/__init__.py` & `fairly-0.4.0/src/fairly/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,18 +164,17 @@
 
                     else:
                         data[key].update(val)
 
         except FileNotFoundError:
             pass
 
-    # Update repository configuration from the environment variables if not testing
-    if not is_testing():
-        for key in data:
-            data[key].update(get_environment_config(key))
+    # Update repository configuration from the environment variables
+    for key in data:
+        data[key].update(get_environment_config(key))
 
     # Create repository dictionary
     repositories = {}
     clients = get_clients()
 
     for id, attrs in data.items():
         repository = {}
@@ -345,15 +344,14 @@
         Local dataset object
 
     Raises:
         ValueError("Invalid path"): If path is invalid.
         NotADirectoryError: If path is not a directory path.
         ValueError("Operation not permitted"): If path is an existing dataset path.
         ValueError("Invalid template name"): If template name is invalid.
-
     """
     if not os.path.exists(path):
         if create:
             os.makedirs(path)
         else:
             raise ValueError("Invalid path")
     elif not os.path.isdir(path):
@@ -407,10 +405,25 @@
         else:
             print(
                 f"{file.path}, {current_size}/{file.size}, {current_total_size}/{total_size}")
     else:
         print(f"{file.path}, {current_size}/{file.size}")
 
 
+def store(id: str, path: str=None, notify: Callable=None, extract: bool=False) -> LocalDataset:
+    """Stores remote dataset locally
+
+    Args:
+        id (str): Dataset identifier.
+        path (str): Local path to store the dataset (optional).
+        notify (Callable): Notification callback function.
+        extract (bool): Set True to extract dataset archives (default = False)
+
+    Returns:
+        Local dataset object
+    """
+    return dataset(id).store(path, notify=notify, extract=extract)
+
+
 if __name__ == "__main__":
     # TODO: CLI implementation
     raise NotImplementedError
```

### Comparing `fairly-0.3.0/src/fairly/client/__init__.py` & `fairly-0.4.0/src/fairly/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,24 +310,22 @@
 
 
     def _request(self, endpoint: str, method: str="GET", headers: dict=None, data=None, format: str=None, serialize: bool=True) -> Tuple(Any, requests.Response):
         """ Sends a HTTP request and returns the result
 
         Returns:
           Returned content and response
-
         """
 
-        if not fairly.is_testing():
-            # Patch HTTPConnection block size to improve connection speed
-            # ref: https://stackoverflow.com/questions/72977722/python-requests-post-very-slow
-            http.client.HTTPConnection.__init__.__defaults__ = tuple(
-                x if x != 8192 else self.CHUNK_SIZE
-                for x in http.client.HTTPConnection.__init__.__defaults__
-            )
+        # Patch HTTPConnection block size to improve connection speed
+        # ref: https://stackoverflow.com/questions/72977722/python-requests-post-very-slow
+        http.client.HTTPConnection.__init__.__defaults__ = tuple(
+            x if x != 8192 else self.CHUNK_SIZE
+            for x in http.client.HTTPConnection.__init__.__defaults__
+        )
 
         # Set default data format
         if not format:
             format = self.REQUEST_FORMAT
 
         # Serialize data if required
         if data is not None and serialize:
@@ -532,25 +530,40 @@
 
     @abstractmethod
     def get_files(self, id: Dict) -> List[RemoteFile]:
         raise NotImplementedError
 
 
     def download_file(self, file: RemoteFile, path: str=None, name: str=None, notify: Callable=None) -> LocalFile:
+        """Downloads a remote file.
+
+        Args:
+            file (RemoteFile): Remote file.
+            path (str): Local path of the file (optional).
+            name (str): Local name of the file (optional).
+            notify (Callable): Notification callback method (optional).
+
+        Returns:
+            Local file object.
+
+        Raises:
+            ValueError("No URL address"): If remote file has no URL address.
+            IOError("Invalid MD5 checksum"): If MD5 checksum is invalid.
+        """
         if not file.url:
             raise ValueError("No URL address")
 
         if not path:
             path = os.getcwd()
 
         if not name:
             name = file.path
             dirs = os.path.dirname(name)
             if dirs:
-                os.makedirs(dirs, exist_ok=True)
+                os.makedirs(os.path.join(path, dirs), exist_ok=True)
 
         fullpath = os.path.join(path, name)
         current_size = 0
         md5 = hashlib.md5()
         if self._session is None:
             self._session = self._create_session()
         try:
```

### Comparing `fairly-0.3.0/src/fairly/client/dataverse.py` & `fairly-0.4.0/src/fairly/client/dataverse.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/client/djehuty.py` & `fairly-0.4.0/src/fairly/client/djehuty.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,18 +45,15 @@
         Args:
             **kwargs: Dataset identifier arguments
 
         Returns:
             Standard dataset identifier
 
         Raises:
-            ValueError("Invalid id")
             ValueError("Invalid URL address")
-            ValueError("No identifier")
-            ValueError("Invalid version")
         """
         version = None
 
         if kwargs.get("uuid"):
             id = str(kwargs["uuid"])
 
         elif kwargs.get("url"):
```

### Comparing `fairly-0.3.0/src/fairly/client/figshare.py` & `fairly-0.4.0/src/fairly/client/figshare.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/client/zenodo.py` & `fairly-0.4.0/src/fairly/client/zenodo.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/config.json` & `fairly-0.4.0/src/fairly/data/config.json`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/languages/ISO-639-2_8859-1.tab` & `fairly-0.4.0/src/fairly/data/languages/ISO-639-2_8859-1.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab` & `fairly-0.4.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/languages/ISO-639-3_8859-1.tab` & `fairly-0.4.0/src/fairly/data/languages/ISO-639-3_8859-1.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab` & `fairly-0.4.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/templates/default.yaml` & `fairly-0.4.0/src/fairly/data/templates/default.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/templates/figshare.yaml` & `fairly-0.4.0/src/fairly/data/templates/figshare.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/data/templates/zenodo.yaml` & `fairly-0.4.0/src/fairly/data/templates/zenodo.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/dataset/__init__.py` & `fairly-0.4.0/src/fairly/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/dataset/local.py` & `fairly-0.4.0/src/fairly/dataset/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,26 +64,28 @@
         self._includes = None
         self._excludes = None
 
         # Load cached MD5 hashes
         self._load_md5s()
 
         self._yaml = YAML()
+        self._yaml.allow_unicode = True
+        self._yaml.encoding = "utf-8"
 
 
     def _get_manifest(self) -> Dict:
         """Retrieves dataset manifest
 
         Returns:
             Dataset manifest dictionary
         """
         # TODO: Add exception handling
         manifest = None
         if os.path.isfile(self._manifest_path):
-            with open(self._manifest_path, "r") as file:
+            with open(self._manifest_path, "r", encoding="utf-8") as file:
                 # REMARK: ruaml.yaml is used to preserve document structure
                 # https://stackoverflow.com/questions/71024653/how-to-update-yaml-file-without-loss-of-comments-and-formatting-yaml-automatic
                 manifest = self._yaml.load(file)
 
         if not manifest:
             manifest = {}
 
@@ -172,15 +174,15 @@
 
         if "files" not in manifest:
             manifest["files"] = {
                 "includes": [],
                 "excludes": [],
             }
 
-        with open(self._manifest_path, "w") as file:
+        with open(self._manifest_path, "w", encoding="utf-8") as file:
             # TODO: Exception handling
             self._yaml.dump(manifest, file)
 
 
     def _save_metadata(self) -> None:
         """Stores dataset metadata."""
         manifest = self._get_manifest()
@@ -484,19 +486,15 @@
 
         except:
             client.delete_dataset(dataset.id)
             raise
 
         # Add remote dataset id to the manifest if known repository
         if client.repository_id:
-            manifest = self._get_manifest()
-            if "remotes" not in manifest:
-                manifest["remotes"] = {}
-            manifest["remotes"][client.repository_id] = dataset.id
-            self._set_manifest(manifest)
+            self.set_remote_dataset(dataset)
 
         return dataset
 
 
     @property
     def size(self) -> int:
         """Total size of the dataset in bytes."""
@@ -555,14 +553,31 @@
 
 
     def reproduce(self) -> LocalDataset:
         """Reproduces an actual copy of the dataset."""
         return LocalDataset(self.path)
 
 
+    def set_remote_dataset(self, dataset) -> None:
+        if not isinstance(dataset, RemoteDataset):
+            dataset = fairly.dataset(dataset)
+            if not isinstance(dataset, RemoteDataset):
+                raise ValueError("Invalid remote dataset")
+
+        id = dataset.client.repository_id
+        if not id:
+            raise ValueError("No repository id")
+
+        manifest = self._get_manifest()
+        if "remotes" not in manifest:
+            manifest["remotes"] = {}
+        manifest["remotes"][id] = dataset.id
+        self._set_manifest(manifest)
+
+
     def get_remote_dataset(self, remote=None) -> RemoteDataset:
         if isinstance(remote, RemoteDataset):
             return remote
 
         elif not remote and self.metadata.get("doi"):
             return fairly.dataset(self.metadata["doi"])
```

### Comparing `fairly-0.3.0/src/fairly/dataset/remote.py` & `fairly-0.4.0/src/fairly/dataset/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,35 @@
         return self.client.get_versions(self.id)
 
 
     def _download_file(self, file: RemoteFile, path: str=None, name: str=None, notify: Callable=None) -> LocalFile:
         return self.client.download_file(file, path, name, notify)
 
 
-    def store(self, path: str, notify: Callable=None, extract: bool=False) -> LocalDataset:
+    def store(self, path: str=None, notify: Callable=None, extract: bool=False) -> LocalDataset:
+        if not path:
+            path = self.doi
+            if not path:
+                raise ValueError("Empty path.")
+            for sep in ["/", "\\"]:
+                path = path.replace(sep, "_")
+
         os.makedirs(path, exist_ok=True)
         if os.listdir(path):
             raise ValueError("Directory is not empty.")
 
-        dataset = fairly.init_dataset(path)
+        templates = fairly.metadata_templates()
+        if self.client.repository_id in templates:
+            template = self.client.repository_id
+        elif self.client.client_id in templates:
+            template = self.client.client_id
+        else:
+            template = None
+
+        dataset = fairly.init_dataset(path, template=template)
 
         # TODO: Set metadata directly without serialization
         dataset.set_metadata(**self.metadata)
         dataset.save_metadata()
 
         includes = dataset.includes
         for name, file in self.files.items():
@@ -97,14 +112,17 @@
                 files = local_file.extract(path, notify=notify)
                 includes.append({file.path: files})
                 os.remove(local_file.fullpath)
             else:
                 includes.append(file.path)
         dataset.save_files()
 
+        if self.client.repository_id:
+            dataset.set_remote_dataset(self)
+
         return dataset
 
 
     def _get_detail(self, key: str, refresh: bool=False) -> Any:
         if not self._details or key not in self._details or refresh:
             self._details = self.client.get_details(self.id)
```

### Comparing `fairly-0.3.0/src/fairly/diff.py` & `fairly-0.4.0/src/fairly/diff.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/file/__init__.py` & `fairly-0.4.0/src/fairly/file/__init__.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/file/local.py` & `fairly-0.4.0/src/fairly/file/local.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/file/remote.py` & `fairly-0.4.0/src/fairly/file/remote.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly/metadata.py` & `fairly-0.4.0/src/fairly/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import Any, Dict
 from collections.abc import MutableMapping
 
 from .person import Person, PersonList
 
 import re
 import copy
+import sys
+import ruamel.yaml
 
 class Metadata(MutableMapping):
     """Metadata class.
 
     Attributes:
         _normalize (Callable): Attribute normalization method.
         _attrs (Dict): Metadata attributes.
@@ -191,8 +193,37 @@
 
             else:
                 continue
 
             if result:
                 updated[key] = result
 
-        return updated
+        return updated
+
+
+    def _remove_comments(self, d):
+        # REMARK: https://stackoverflow.com/questions/60080325/how-to-delete-all-comments-in-ruamel-yaml
+        if isinstance(d, dict):
+            for k, v in d.items():
+                self._remove_comments(k)
+                self._remove_comments(v)
+
+        elif isinstance(d, list):
+            for elem in d:
+                self._remove_comments(elem)
+
+        try:
+             # literal scalarstring might have comment associated with them
+             attr = 'comment' if isinstance(d, ruamel.yaml.scalarstring.ScalarString) \
+                      else ruamel.yaml.comments.Comment.attrib
+             delattr(d, attr)
+        except AttributeError:
+            pass
+
+
+    def print(self):
+        yaml = ruamel.yaml.YAML()
+
+        out = self.serialize()
+        self._remove_comments(out)
+
+        yaml.dump(out, sys.stdout)
```

### Comparing `fairly-0.3.0/src/fairly/person.py` & `fairly-0.4.0/src/fairly/person.py`

 * *Files identical despite different names*

### Comparing `fairly-0.3.0/src/fairly.egg-info/SOURCES.txt` & `fairly-0.4.0/src/fairly.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.md
+README.rst
 pyproject.toml
 setup.cfg
 src/cli/__init__.py
 src/cli/config.py
 src/cli/dataset.py
 src/fairly/__init__.py
 src/fairly/diff.py
@@ -31,8 +31,9 @@
 src/fairly/data/templates/zenodo.yaml
 src/fairly/dataset/__init__.py
 src/fairly/dataset/local.py
 src/fairly/dataset/remote.py
 src/fairly/file/__init__.py
 src/fairly/file/local.py
 src/fairly/file/remote.py
+tests/test_cli.py
 tests/test_fairly.py
```


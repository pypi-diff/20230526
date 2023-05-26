# Comparing `tmp/macrometa-target-collection-0.0.61.tar.gz` & `tmp/macrometa-target-collection-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.61.tar", last modified: Fri May 26 06:41:45 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.62.tar", last modified: Fri May 26 07:05:05 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.61.tar` & `macrometa-target-collection-0.0.62.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14458 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14458 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:05:05.863687 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 07:05:05.000000 macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 07:04:39.000000 macrometa-target-collection-0.0.62/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 07:05:05.867687 macrometa-target-collection-0.0.62/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.61/LICENSE` & `macrometa-target-collection-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.61/PKG-INFO` & `macrometa-target-collection-0.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.61
+Version: 0.0.62
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.61/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.62/macrometa_target_collection/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,11 +84,14 @@
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
 
 
 def extract_gdn_host(url):
     parsed_url = urlparse(url)
-    resource_name = parsed_url.netloc.strip()
+    if parsed_url.scheme:
+        resource_name = parsed_url.netloc.strip()
+    else:
+        resource_name = parsed_url.path.strip()
     if not resource_name.startswith("api-"):
         resource_name = "api-" + resource_name
     return resource_name
```

### Comparing `macrometa-target-collection-0.0.61/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.62/macrometa_target_collection/main.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.62/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.61
+Version: 0.0.62
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.61/pyproject.toml` & `macrometa-target-collection-0.0.62/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.61"
+version = "0.0.62"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```


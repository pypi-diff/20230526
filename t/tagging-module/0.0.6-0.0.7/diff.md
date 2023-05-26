# Comparing `tmp/tagging_module-0.0.6.tar.gz` & `tmp/tagging_module-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagging_module-0.0.6.tar", last modified: Fri May 26 09:58:48 2023, max compression
+gzip compressed data, was "tagging_module-0.0.7.tar", last modified: Fri May 26 11:45:37 2023, max compression
```

## Comparing `tagging_module-0.0.6.tar` & `tagging_module-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.693390 tagging_module-0.0.6/
--rw-rw-rw-   0        0        0       42 2023-05-26 08:21:31.000000 tagging_module-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      194 2023-05-26 09:58:48.692391 tagging_module-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-05-21 13:22:58.000000 tagging_module-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 09:58:48.693390 tagging_module-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      442 2023-05-26 08:25:40.000000 tagging_module-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.681388 tagging_module-0.0.6/tagging_module/
--rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.691392 tagging_module-0.0.6/tagging_module/config/
--rw-rw-rw-   0        0        0     4001 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/config/rules.yml
--rw-rw-rw-   0        0        0      783 2023-05-26 08:25:07.000000 tagging_module-0.0.6/tagging_module/tagging_service.py
--rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/tagging_system.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.689388 tagging_module-0.0.6/tagging_module.egg-info/
--rw-rw-rw-   0        0        0      194 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.863945 tagging_module-0.0.7/
+-rw-rw-rw-   0        0        0       61 2023-05-26 11:32:18.000000 tagging_module-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2082 2023-05-26 11:45:37.862949 tagging_module-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-26 11:21:14.000000 tagging_module-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 11:45:37.863945 tagging_module-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-05-26 11:45:20.000000 tagging_module-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.852937 tagging_module-0.0.7/tagging_module/
+-rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.861947 tagging_module-0.0.7/tagging_module/config/
+-rw-rw-rw-   0        0        0     4001 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/config/rules.yml
+-rw-rw-rw-   0        0        0      783 2023-05-26 08:25:07.000000 tagging_module-0.0.7/tagging_module/tagging_service.py
+-rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.7/tagging_module/tagging_system.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:45:37.860952 tagging_module-0.0.7/tagging_module.egg-info/
+-rw-rw-rw-   0        0        0     2082 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 11:45:37.000000 tagging_module-0.0.7/tagging_module.egg-info/top_level.txt
```

### Comparing `tagging_module-0.0.6/README.md` & `tagging_module-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # Tagging Module
 A lightweight rule based tech content tagging module for Python
 
 ## Class Overview
 The `TaggingService` class is designed to provide a tagging service. It uses the `tagging_system` module to assign tags to content based on predefined rules. The tagging rules are specified in a YAML file.
 
+You may directly use it from this repo or install via Pip.
+```
+pip install tagging-module
+```
+
 ## Constructor
 ### `__init__(self, rules_path: str = None)`
 The constructor initializes a `TaggingService` object.
 
 #### Parameters
 - `rules_path` (optional): A string representing the path to the YAML file containing the tagging rules. If not provided, the default rules file path (`tagging_module/config/rules.yml`) is used.
 
 #### Exceptions
 - `FileNotFoundError`: Raised if the provided `rules_path` is not a valid file path.
 
 ### Example
 ```python
-from tagging_module.tagging_module import TaggingService
+from tagging_module.tagging_service import TaggingService
 
 # Using the default rules file path
 service = TaggingService()
 
 # Providing a custom rules file path
 service = TaggingService(rules_path="path/to/custom_rules.yml")
 ```
@@ -32,15 +37,15 @@
 #### Parameters
 - content: A string representing the content to be tagged.
 #### Returns
 A list of strings representing the assigned tags for the content.
 
 ### Example
 ```python
-from tagging_module.tagging_module import TaggingService
+from tagging_module.tagging_service import TaggingService
 
 # Assuming the rules file contains rules for tagging different types of content
 service = TaggingService()
 
 content = "This is a sample content."
 tags = service.assign_tags(content)
 print(tags)
```

### Comparing `tagging_module-0.0.6/tagging_module/config/rules.yml` & `tagging_module-0.0.7/tagging_module/config/rules.yml`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.6/tagging_module/tagging_service.py` & `tagging_module-0.0.7/tagging_module/tagging_service.py`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.6/tagging_module/tagging_system.py` & `tagging_module-0.0.7/tagging_module/tagging_system.py`

 * *Files identical despite different names*


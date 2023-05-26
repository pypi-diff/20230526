# Comparing `tmp/tagging_module-0.0.5.tar.gz` & `tmp/tagging_module-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagging_module-0.0.5.tar", last modified: Fri May 26 07:13:17 2023, max compression
+gzip compressed data, was "tagging_module-0.0.6.tar", last modified: Fri May 26 09:58:48 2023, max compression
```

## Comparing `tagging_module-0.0.5.tar` & `tagging_module-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 07:13:17.556782 tagging_module-0.0.5/
--rw-rw-rw-   0        0        0      194 2023-05-26 07:13:17.555783 tagging_module-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-05-21 13:22:58.000000 tagging_module-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 07:13:17.556782 tagging_module-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-05-26 07:12:32.000000 tagging_module-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:13:17.546773 tagging_module-0.0.5/tagging_module/
--rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.5/tagging_module/__init__.py
--rw-rw-rw-   0        0        0      656 2023-05-26 07:07:42.000000 tagging_module-0.0.5/tagging_module/tagging_service.py
--rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.5/tagging_module/tagging_system.py
-drwxrwxrwx   0        0        0        0 2023-05-26 07:13:17.554783 tagging_module-0.0.5/tagging_module.egg-info/
--rw-rw-rw-   0        0        0      194 2023-05-26 07:13:17.000000 tagging_module-0.0.5/tagging_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-05-26 07:13:17.000000 tagging_module-0.0.5/tagging_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 07:13:17.000000 tagging_module-0.0.5/tagging_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 07:13:17.000000 tagging_module-0.0.5/tagging_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 07:13:17.000000 tagging_module-0.0.5/tagging_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.693390 tagging_module-0.0.6/
+-rw-rw-rw-   0        0        0       42 2023-05-26 08:21:31.000000 tagging_module-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      194 2023-05-26 09:58:48.692391 tagging_module-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2023-05-21 13:22:58.000000 tagging_module-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 09:58:48.693390 tagging_module-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      442 2023-05-26 08:25:40.000000 tagging_module-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.681388 tagging_module-0.0.6/tagging_module/
+-rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.691392 tagging_module-0.0.6/tagging_module/config/
+-rw-rw-rw-   0        0        0     4001 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/config/rules.yml
+-rw-rw-rw-   0        0        0      783 2023-05-26 08:25:07.000000 tagging_module-0.0.6/tagging_module/tagging_service.py
+-rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.6/tagging_module/tagging_system.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:58:48.689388 tagging_module-0.0.6/tagging_module.egg-info/
+-rw-rw-rw-   0        0        0      194 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 09:58:48.000000 tagging_module-0.0.6/tagging_module.egg-info/top_level.txt
```

### Comparing `tagging_module-0.0.5/README.md` & `tagging_module-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.5/tagging_module/tagging_service.py` & `tagging_module-0.0.6/tagging_module/tagging_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from tagging_module.tagging_system import TaggingSystem
 
 class TaggingService:
     """
     A class for providing a tagging service.
     """
 
-    rules_path = "tagging_module/config/rules.yml"
+    package_dir = os.path.dirname(os.path.abspath(__file__))  # Get the absolute path of the package directory
+    rules_path = os.path.join(package_dir, 'config', 'rules.yml')
 
     def __init__(self, rules_path: str = None):
         if rules_path is None:
             rules_path = TaggingService.rules_path
         if not os.path.isfile(rules_path):
             raise FileNotFoundError(f"Rules file not found: {rules_path}")
         self.rules_path = rules_path
```

### Comparing `tagging_module-0.0.5/tagging_module/tagging_system.py` & `tagging_module-0.0.6/tagging_module/tagging_system.py`

 * *Files identical despite different names*


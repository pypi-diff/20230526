# Comparing `tmp/tagging_module-0.0.2.tar.gz` & `tmp/tagging_module-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagging_module-0.0.2.tar", last modified: Fri May 26 06:53:18 2023, max compression
+gzip compressed data, was "tagging_module-0.0.3.tar", last modified: Fri May 26 06:57:17 2023, max compression
```

## Comparing `tagging_module-0.0.2.tar` & `tagging_module-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:53:18.198997 tagging_module-0.0.2/
--rw-rw-rw-   0        0        0      194 2023-05-26 06:53:18.197996 tagging_module-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-05-21 13:22:58.000000 tagging_module-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 06:53:18.198997 tagging_module-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-05-26 06:51:00.000000 tagging_module-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:53:18.187996 tagging_module-0.0.2/tagging_module/
--rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.2/tagging_module/__init__.py
--rw-rw-rw-   0        0        0      658 2023-05-21 13:22:58.000000 tagging_module-0.0.2/tagging_module/tagging_service.py
--rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.2/tagging_module/tagging_system.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:53:18.195995 tagging_module-0.0.2/tagging_module.egg-info/
--rw-rw-rw-   0        0        0      194 2023-05-26 06:53:17.000000 tagging_module-0.0.2/tagging_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-05-26 06:53:18.000000 tagging_module-0.0.2/tagging_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:53:17.000000 tagging_module-0.0.2/tagging_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 06:53:17.000000 tagging_module-0.0.2/tagging_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 06:53:17.000000 tagging_module-0.0.2/tagging_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:17.265130 tagging_module-0.0.3/
+-rw-rw-rw-   0        0        0      194 2023-05-26 06:57:17.263129 tagging_module-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2023-05-21 13:22:58.000000 tagging_module-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:57:17.265130 tagging_module-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-05-26 06:56:40.000000 tagging_module-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:17.254129 tagging_module-0.0.3/tagging_module/
+-rw-rw-rw-   0        0        0        0 2023-05-21 13:22:58.000000 tagging_module-0.0.3/tagging_module/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-05-26 06:56:31.000000 tagging_module-0.0.3/tagging_module/tagging_service.py
+-rw-rw-rw-   0        0        0     1394 2023-05-21 13:22:58.000000 tagging_module-0.0.3/tagging_module/tagging_system.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:57:17.262133 tagging_module-0.0.3/tagging_module.egg-info/
+-rw-rw-rw-   0        0        0      194 2023-05-26 06:57:16.000000 tagging_module-0.0.3/tagging_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-05-26 06:57:17.000000 tagging_module-0.0.3/tagging_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:57:16.000000 tagging_module-0.0.3/tagging_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 06:57:17.000000 tagging_module-0.0.3/tagging_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 06:57:17.000000 tagging_module-0.0.3/tagging_module.egg-info/top_level.txt
```

### Comparing `tagging_module-0.0.2/README.md` & `tagging_module-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tagging_module-0.0.2/tagging_module/tagging_service.py` & `tagging_module-0.0.3/tagging_module/tagging_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 import os
 
-from tagging_module.tagging_module import tagging_system
+from tagging_module import tagging_system
 
 class TaggingService:
     """
     A class for providing a tagging service.
     """
 
-    rules_path = "tagging_module/config/rules.yml"
+    rules_path = "config/rules.yml"
 
     def __init__(self, rules_path: str = None):
         if rules_path is None:
             rules_path = TaggingService.rules_path
         if not os.path.isfile(rules_path):
             raise FileNotFoundError(f"Rules file not found: {rules_path}")
         self.rules_path = rules_path
```

### Comparing `tagging_module-0.0.2/tagging_module/tagging_system.py` & `tagging_module-0.0.3/tagging_module/tagging_system.py`

 * *Files identical despite different names*


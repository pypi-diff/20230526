# Comparing `tmp/domjudge_utility-0.0.7.tar.gz` & `tmp/domjudge_utility-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domjudge_utility-0.0.7.tar", max compression
+gzip compressed data, was "domjudge_utility-0.0.8.tar", max compression
```

## Comparing `domjudge_utility-0.0.7.tar` & `domjudge_utility-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-05-25 12:41:33.655414 domjudge_utility-0.0.7/LICENSE
--rw-r--r--   0        0        0      636 2023-05-25 12:41:33.655414 domjudge_utility-0.0.7/README.md
--rw-r--r--   0        0        0       47 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/__init__.py
--rw-r--r--   0        0        0    21911 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/dump.py
--rw-r--r--   0        0        0     3165 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/dump_config.py
--rw-r--r--   0        0        0      394 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/utils.py
--rw-r--r--   0        0        0       22 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/domjudge_utility/version.py
--rw-r--r--   0        0        0     1161 2023-05-25 12:41:33.659414 domjudge_utility-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/LICENSE
+-rw-r--r--   0        0        0      636 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/README.md
+-rw-r--r--   0        0        0       47 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/__init__.py
+-rw-r--r--   0        0        0    22055 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/dump.py
+-rw-r--r--   0        0        0     3329 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/dump_config.py
+-rw-r--r--   0        0        0      394 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/utils.py
+-rw-r--r--   0        0        0       22 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/domjudge_utility/version.py
+-rw-r--r--   0        0        0     1161 2023-05-26 17:15:34.605504 domjudge_utility-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 domjudge_utility-0.0.8/PKG-INFO
```

### Comparing `domjudge_utility-0.0.7/LICENSE` & `domjudge_utility-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.7/README.md` & `domjudge_utility-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `domjudge_utility-0.0.7/domjudge_utility/dump.py` & `domjudge_utility-0.0.8/domjudge_utility/dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,17 @@
         self.organizations = self.request_json_and_save(
             'organizations', 'organizations.json')
         self.problems = self.request_json_and_save('problems', 'problems.json')
         self.teams = self.request_json_and_save('teams', 'teams.json')
         self.submissions = self.request_json_and_save(
             'submissions', 'submissions.json')
 
-        self.clarifications = self.request_json_and_save(
-            'clarifications', 'clarifications.json')
+        if self.config.exported_data.domjudge_api_clarifications:
+            self.clarifications = self.request_json_and_save(
+                'clarifications', 'clarifications.json')
 
         if self.config.exported_data.event_feed:
             self.event_feed = self.request_json_and_save(
                 'event-feed', 'event-feed.ndjson', {'stream': False, 'strict': True})
 
     def dump_runs(self):
         if not self.config.exported_data.runs:
@@ -641,11 +642,12 @@
         self.dump_runs()
         self.dump_source_code()
         self.dump_images()
         self.dump_3rd_data()
 
     def load_domjudge_api(self):
         self.config.exported_data.domjudge_api = False
+        self.config.exported_data.domjudge_api_clarifications = False
 
         self.init_logging()
         self.dump_domjudge_api()
         self.process_domjudge_raw_data()
```

### Comparing `domjudge_utility-0.0.7/domjudge_utility/dump_config.py` & `domjudge_utility-0.0.8/domjudge_utility/dump_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
         return default_value
 
     class ExportedData:
         def __init__(self, exported_data_dict):
             self.domjudge_api = DumpConfig.get_config_with_default_value(
                 exported_data_dict, 'domjudge_api', True)
 
+            self.domjudge_api_clarifications = DumpConfig.get_config_with_default_value(
+                exported_data_dict, "domjudge_api_clarifications", False)
+
             # Since the export of event-feed may be a bit slow
             # we do not export by default
             self.event_feed = DumpConfig.get_config_with_default_value(
                 exported_data_dict, 'event_feed', False)
 
             self.runs = DumpConfig.get_config_with_default_value(
                 exported_data_dict, 'runs', False)
```

### Comparing `domjudge_utility-0.0.7/pyproject.toml` & `domjudge_utility-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domjudge-utility"
-version = "0.0.7"
+version = "0.0.8"
 description = "DOMjudge Utility"
 authors = ["Dup4 <lyuzhi.pan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `domjudge_utility-0.0.7/PKG-INFO` & `domjudge_utility-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domjudge-utility
-Version: 0.0.7
+Version: 0.0.8
 Summary: DOMjudge Utility
 License: MIT
 Author: Dup4
 Author-email: lyuzhi.pan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


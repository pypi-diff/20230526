# Comparing `tmp/spreadsheet-migrator-0.1.tar.gz` & `tmp/spreadsheet-migrator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spreadsheet-migrator-0.1.tar", last modified: Thu May 25 15:00:07 2023, max compression
+gzip compressed data, was "spreadsheet-migrator-0.2.tar", last modified: Thu May 25 15:22:55 2023, max compression
```

## Comparing `spreadsheet-migrator-0.1.tar` & `spreadsheet-migrator-0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:00:07.699127 spreadsheet-migrator-0.1/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1094 2023-05-25 14:35:20.000000 spreadsheet-migrator-0.1/LICENSE
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      139 2023-05-25 15:00:07.697125 spreadsheet-migrator-0.1/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     8928 2023-05-25 14:22:46.000000 spreadsheet-migrator-0.1/README.md
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-05-25 15:00:07.700125 spreadsheet-migrator-0.1/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      321 2023-05-07 19:58:28.000000 spreadsheet-migrator-0.1/setup.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:00:07.484278 spreadsheet-migrator-0.1/spreadsheet_migrator/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      387 2023-05-07 20:07:02.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:00:07.600125 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      191 2023-03-29 14:56:36.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:00:07.685126 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-07 08:40:57.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/__init__.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-20 07:50:40.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/cases_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      225 2023-04-03 13:21:26.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/parameters_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-03 13:21:36.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/plans_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      221 2023-04-03 13:21:18.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/logs/suites_logs.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12358 2023-05-25 14:47:36.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     6173 2023-05-25 13:57:04.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/service.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12695 2023-05-25 11:51:41.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      100 2023-03-16 20:10:58.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/testy_exception.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      551 2023-05-07 22:17:30.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/urls.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1931 2023-05-22 20:32:22.000000 spreadsheet-migrator-0.1/spreadsheet_migrator/views.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:00:07.536278 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      139 2023-05-25 15:00:07.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1008 2023-05-25 15:00:07.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-25 15:00:07.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        2 2023-05-07 20:03:57.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/not-zip-safe
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       16 2023-05-25 15:00:07.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/requires.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       21 2023-05-25 15:00:07.000000 spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/top_level.txt
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:22:55.248707 spreadsheet-migrator-0.2/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1094 2023-05-25 14:35:20.000000 spreadsheet-migrator-0.2/LICENSE
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     9058 2023-05-25 15:22:55.247704 spreadsheet-migrator-0.2/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     8928 2023-05-25 14:22:46.000000 spreadsheet-migrator-0.2/README.md
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-05-25 15:22:55.249704 spreadsheet-migrator-0.2/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      594 2023-05-25 15:22:34.000000 spreadsheet-migrator-0.2/setup.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:22:55.058318 spreadsheet-migrator-0.2/spreadsheet_migrator/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      387 2023-05-07 20:07:02.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:22:55.167586 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      191 2023-03-29 14:56:36.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/__init__.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:22:55.234704 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-07 08:40:57.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/__init__.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-20 07:50:40.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/cases_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      225 2023-04-03 13:21:26.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/parameters_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      220 2023-04-03 13:21:36.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/plans_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      221 2023-04-03 13:21:18.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/logs/suites_logs.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12358 2023-05-25 14:47:36.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     6173 2023-05-25 13:57:04.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/service.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)    12695 2023-05-25 11:51:41.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      100 2023-03-16 20:10:58.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/testy_exception.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      551 2023-05-07 22:17:30.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/urls.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1931 2023-05-22 20:32:22.000000 spreadsheet-migrator-0.2/spreadsheet_migrator/views.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-05-25 15:22:55.111586 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     9058 2023-05-25 15:22:54.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     1008 2023-05-25 15:22:54.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-05-25 15:22:54.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        2 2023-05-07 20:03:57.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/not-zip-safe
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       16 2023-05-25 15:22:54.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/requires.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       21 2023-05-25 15:22:54.000000 spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/top_level.txt
```

### Comparing `spreadsheet-migrator-0.1/LICENSE` & `spreadsheet-migrator-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/README.md` & `spreadsheet-migrator-0.2/README.md`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py` & `spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/parser.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/service.py` & `spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/service.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py` & `spreadsheet-migrator-0.2/spreadsheet_migrator/spreadsheet_migrator_lib/testy_creator.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator/urls.py` & `spreadsheet-migrator-0.2/spreadsheet_migrator/urls.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator/views.py` & `spreadsheet-migrator-0.2/spreadsheet_migrator/views.py`

 * *Files identical despite different names*

### Comparing `spreadsheet-migrator-0.1/spreadsheet_migrator.egg-info/SOURCES.txt` & `spreadsheet-migrator-0.2/spreadsheet_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/indecro-0.13.tar.gz` & `tmp/indecro-0.131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indecro-0.13.tar", last modified: Fri May 26 08:27:05 2023, max compression
+gzip compressed data, was "indecro-0.131.tar", last modified: Fri May 26 08:52:19 2023, max compression
```

## Comparing `indecro-0.13.tar` & `indecro-0.131.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.496592 indecro-0.13/
--rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.13/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2107 2023-05-26 08:27:05.496592 indecro-0.13/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1574 2023-05-26 04:26:38.000000 indecro-0.13/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.495592 indecro-0.13/indecro/
--rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.13/indecro/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.13/indecro/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.13/indecro/executor.py
--rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.13/indecro/job.py
--rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.13/indecro/rules.py
--rw-r--r--   0 user      (1000) user      (1000)     3450 2023-05-26 04:38:48.000000 indecro-0.13/indecro/scheduler.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.496592 indecro-0.13/indecro/storage/
--rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.13/indecro/storage/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.13/indecro/storage/base.py
--rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.13/indecro/storage/memory_storage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.495592 indecro-0.13/indecro.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2107 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:27:05.497592 indecro-0.13/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      935 2023-05-26 08:26:47.000000 indecro-0.13/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/
+-rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.131/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:52:19.155269 indecro-0.131/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1536 2023-05-26 08:51:44.000000 indecro-0.131/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.131/indecro/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.131/indecro/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.131/indecro/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.131/indecro/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.131/indecro/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     3450 2023-05-26 04:38:48.000000 indecro-0.131/indecro/scheduler.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro/storage/
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.131/indecro/storage/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.131/indecro/storage/base.py
+-rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.131/indecro/storage/memory_storage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:52:19.156269 indecro-0.131/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      936 2023-05-26 08:52:18.000000 indecro-0.131/setup.py
```

### Comparing `indecro-0.13/LICENSE` & `indecro-0.131/LICENSE`

 * *Files identical despite different names*

### Comparing `indecro-0.13/PKG-INFO` & `indecro-0.131/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.13
+Version: 0.131
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,35 +51,35 @@
     storage=MemoryStorage()
 )
 ```
 
 Schedule job using decorator-based shortcut (custom job name can be provided for compatibility)
 
 ```python
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-@scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
+@scheduler.job(rule=RunOnce(after=timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
 
 ```python
 async def some_another_job():
     print('Executing some another job..')
 
 
 scheduler.add_job(
     some_another_job,
-    rule=RunOnce(at=datetime.now() + timedelta(seconds=20))
+    rule=RunOnce(after=timedelta(seconds=20))
 )
 ```
 
 Run scheduler:
 
 ```python
 await scheduler.run()
```

### Comparing `indecro-0.13/README.md` & `indecro-0.131/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,35 +35,35 @@
     storage=MemoryStorage()
 )
 ```
 
 Schedule job using decorator-based shortcut (custom job name can be provided for compatibility)
 
 ```python
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-@scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
+@scheduler.job(rule=RunOnce(after=timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
 
 ```python
 async def some_another_job():
     print('Executing some another job..')
 
 
 scheduler.add_job(
     some_another_job,
-    rule=RunOnce(at=datetime.now() + timedelta(seconds=20))
+    rule=RunOnce(after=timedelta(seconds=20))
 )
 ```
 
 Run scheduler:
 
 ```python
 await scheduler.run()
```

### Comparing `indecro-0.13/indecro/exceptions.py` & `indecro-0.131/indecro/exceptions.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/executor.py` & `indecro-0.131/indecro/executor.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/job.py` & `indecro-0.131/indecro/job.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/rules.py` & `indecro-0.131/indecro/rules.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/scheduler.py` & `indecro-0.131/indecro/scheduler.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/storage/base.py` & `indecro-0.131/indecro/storage/base.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro/storage/memory_storage.py` & `indecro-0.131/indecro/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `indecro-0.13/indecro.egg-info/PKG-INFO` & `indecro-0.131/indecro.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.13
+Version: 0.131
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -51,35 +51,35 @@
     storage=MemoryStorage()
 )
 ```
 
 Schedule job using decorator-based shortcut (custom job name can be provided for compatibility)
 
 ```python
-from datetime import datetime, timedelta
+from datetime import timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-@scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
+@scheduler.job(rule=RunOnce(after=timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
 
 ```python
 async def some_another_job():
     print('Executing some another job..')
 
 
 scheduler.add_job(
     some_another_job,
-    rule=RunOnce(at=datetime.now() + timedelta(seconds=20))
+    rule=RunOnce(after=timedelta(seconds=20))
 )
 ```
 
 Run scheduler:
 
 ```python
 await scheduler.run()
```

### Comparing `indecro-0.13/setup.py` & `indecro-0.131/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 this_directory = path.abspath(path.dirname(__file__))
 
 setup(
     name='indecro',
     description='Python scheduler with task independency from scheduler, executor and others',
-    version='0.13',
+    version='0.131',
     url='https://github.com/TypeHintsFun/indecro',
     author='TypeHintsFun',
     author_email='typehintsfun@gmail.com',
     license='MIT',
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
```


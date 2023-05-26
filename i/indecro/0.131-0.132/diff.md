# Comparing `tmp/indecro-0.131.tar.gz` & `tmp/indecro-0.132.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indecro-0.131.tar", last modified: Fri May 26 08:52:19 2023, max compression
+gzip compressed data, was "indecro-0.132.tar", last modified: Fri May 26 08:59:40 2023, max compression
```

## Comparing `indecro-0.131.tar` & `indecro-0.132.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/
--rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.131/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:52:19.155269 indecro-0.131/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1536 2023-05-26 08:51:44.000000 indecro-0.131/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro/
--rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.131/indecro/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.131/indecro/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.131/indecro/executor.py
--rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.131/indecro/job.py
--rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.131/indecro/rules.py
--rw-r--r--   0 user      (1000) user      (1000)     3450 2023-05-26 04:38:48.000000 indecro-0.131/indecro/scheduler.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro/storage/
--rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.131/indecro/storage/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.131/indecro/storage/base.py
--rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.131/indecro/storage/memory_storage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:52:19.155269 indecro-0.131/indecro.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:52:19.000000 indecro-0.131/indecro.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:52:19.156269 indecro-0.131/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      936 2023-05-26 08:52:18.000000 indecro-0.131/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/
+-rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.132/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:59:40.899741 indecro-0.132/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1536 2023-05-26 08:51:44.000000 indecro-0.132/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.898741 indecro-0.132/indecro/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.132/indecro/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.132/indecro/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.132/indecro/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.132/indecro/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.132/indecro/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     3703 2023-05-26 08:58:07.000000 indecro-0.132/indecro/scheduler.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/indecro/storage/
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.132/indecro/storage/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.132/indecro/storage/base.py
+-rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.132/indecro/storage/memory_storage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:59:40.899741 indecro-0.132/indecro.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2070 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:59:40.000000 indecro-0.132/indecro.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:59:40.899741 indecro-0.132/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      936 2023-05-26 08:59:40.000000 indecro-0.132/setup.py
```

### Comparing `indecro-0.131/LICENSE` & `indecro-0.132/LICENSE`

 * *Files identical despite different names*

### Comparing `indecro-0.131/PKG-INFO` & `indecro-0.132/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.131
+Version: 0.132
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `indecro-0.131/README.md` & `indecro-0.132/README.md`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/exceptions.py` & `indecro-0.132/indecro/exceptions.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/executor.py` & `indecro-0.132/indecro/executor.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/job.py` & `indecro-0.132/indecro/job.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/rules.py` & `indecro-0.132/indecro/rules.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/scheduler.py` & `indecro-0.132/indecro/scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,25 @@
 from indecro.job import Job
 from indecro.api.rules import Rule
 from indecro.api.scheduler import Scheduler as SchedulerProtocol
 from indecro.api.storage import Storage, AsyncStorage
 
 
 class Scheduler(SchedulerProtocol):
-    def __init__(self, storage: Union[Storage, AsyncStorage], executor: Executor):
+    def __init__(
+            self,
+            storage: Union[Storage, AsyncStorage],
+            executor: Executor,
+            loop_delay: Union[int, float] = 1
+    ):
         self.storage = storage
         self.executor = executor
 
+        self.loop_delay = loop_delay
+
         self.running = False
 
     def job(
             self,
             rule: Rule,
 
             daemonize: RunAs = RunAs.FUNCTION,
@@ -114,8 +121,9 @@
 
                     job_executed = False
                 except CannotPredictJobSchedulingTime:  # Looks like BoolRule, we just wait
                     job_executed = False
 
                 any_job_started = job_executed or any_job_started
 
-            await asyncio.sleep(not any_job_started)
+            # Sleeping loop_delay seconds if not any job started, else sleeping 0 seconds (asyncio magic)
+            await asyncio.sleep(self.loop_delay * (not any_job_started))
```

### Comparing `indecro-0.131/indecro/storage/base.py` & `indecro-0.132/indecro/storage/base.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro/storage/memory_storage.py` & `indecro-0.132/indecro/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `indecro-0.131/indecro.egg-info/PKG-INFO` & `indecro-0.132/indecro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.131
+Version: 0.132
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `indecro-0.131/setup.py` & `indecro-0.132/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 this_directory = path.abspath(path.dirname(__file__))
 
 setup(
     name='indecro',
     description='Python scheduler with task independency from scheduler, executor and others',
-    version='0.131',
+    version='0.132',
     url='https://github.com/TypeHintsFun/indecro',
     author='TypeHintsFun',
     author_email='typehintsfun@gmail.com',
     license='MIT',
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
```


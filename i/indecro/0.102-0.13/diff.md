# Comparing `tmp/indecro-0.102.tar.gz` & `tmp/indecro-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indecro-0.102.tar", last modified: Thu May 25 06:25:20 2023, max compression
+gzip compressed data, was "indecro-0.13.tar", last modified: Fri May 26 08:27:05 2023, max compression
```

## Comparing `indecro-0.102.tar` & `indecro-0.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:25:20.719911 indecro-0.102/
--rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.102/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1944 2023-05-25 06:25:20.719911 indecro-0.102/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1410 2023-05-25 06:25:12.000000 indecro-0.102/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:25:20.719911 indecro-0.102/indecro/
--rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.102/indecro/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      672 2023-05-25 01:51:47.000000 indecro-0.102/indecro/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 04:55:40.000000 indecro-0.102/indecro/executor.py
--rw-r--r--   0 user      (1000) user      (1000)     1497 2023-05-25 02:26:06.000000 indecro-0.102/indecro/job.py
--rw-r--r--   0 user      (1000) user      (1000)     1671 2023-05-25 03:52:13.000000 indecro-0.102/indecro/rules.py
--rw-r--r--   0 user      (1000) user      (1000)     2993 2023-05-25 03:17:52.000000 indecro-0.102/indecro/scheduler.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:25:20.719911 indecro-0.102/indecro/storage/
--rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.102/indecro/storage/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.102/indecro/storage/base.py
--rw-r--r--   0 user      (1000) user      (1000)     1036 2023-05-24 05:57:31.000000 indecro-0.102/indecro/storage/memory_storage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 06:25:20.719911 indecro-0.102/indecro.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1944 2023-05-25 06:25:20.000000 indecro-0.102/indecro.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-25 06:25:20.000000 indecro-0.102/indecro.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-25 06:25:20.000000 indecro-0.102/indecro.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-25 06:25:20.000000 indecro-0.102/indecro.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-25 06:25:20.719911 indecro-0.102/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      936 2023-05-25 06:25:19.000000 indecro-0.102/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.496592 indecro-0.13/
+-rw-r--r--   0 user      (1000) user      (1000)     1069 2023-05-25 02:33:35.000000 indecro-0.13/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2107 2023-05-26 08:27:05.496592 indecro-0.13/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1574 2023-05-26 04:26:38.000000 indecro-0.13/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.495592 indecro-0.13/indecro/
+-rw-r--r--   0 user      (1000) user      (1000)       33 2023-05-25 03:11:46.000000 indecro-0.13/indecro/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      898 2023-05-26 03:50:28.000000 indecro-0.13/indecro/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     1701 2023-05-25 09:16:34.000000 indecro-0.13/indecro/executor.py
+-rw-r--r--   0 user      (1000) user      (1000)     1531 2023-05-26 03:53:49.000000 indecro-0.13/indecro/job.py
+-rw-r--r--   0 user      (1000) user      (1000)     3352 2023-05-26 06:06:40.000000 indecro-0.13/indecro/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     3450 2023-05-26 04:38:48.000000 indecro-0.13/indecro/scheduler.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.496592 indecro-0.13/indecro/storage/
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-05-25 03:46:12.000000 indecro-0.13/indecro/storage/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2126 2023-05-23 18:24:15.000000 indecro-0.13/indecro/storage/base.py
+-rw-r--r--   0 user      (1000) user      (1000)     1113 2023-05-26 04:29:00.000000 indecro-0.13/indecro/storage/memory_storage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-26 08:27:05.495592 indecro-0.13/indecro.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2107 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      361 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-26 08:27:05.000000 indecro-0.13/indecro.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       79 2023-05-26 08:27:05.497592 indecro-0.13/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      935 2023-05-26 08:26:47.000000 indecro-0.13/setup.py
```

### Comparing `indecro-0.102/LICENSE` & `indecro-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `indecro-0.102/PKG-INFO` & `indecro-0.13/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.102
+Version: 0.13
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,26 @@
 All parts are designed to be replaceable.
 
 Main ideas are:
 
 * Task creator doesn't need to know how tasks are implemented or executed
 * Persistence may be implemented
 * You can choose how jobs will be parallelized and whether they will be parallelized at all
+* Not only time-based scheduling rules! Magic filters and bool-based rules is available
 
 Currently project is in the design stage and any APIs are to be changed
 
+
+### How to install:
+
+#### Install using pip
+```bash
+pip install indecro
+```
+
 ### How to use:
 
 Create scheduler
 
 ```python
 from indecro import Scheduler
 from indecro.executor import Executor
@@ -48,16 +57,14 @@
 ```python
 from datetime import datetime, timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-
-
 @scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
```

### Comparing `indecro-0.102/README.md` & `indecro-0.13/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,26 @@
 All parts are designed to be replaceable.
 
 Main ideas are:
 
 * Task creator doesn't need to know how tasks are implemented or executed
 * Persistence may be implemented
 * You can choose how jobs will be parallelized and whether they will be parallelized at all
+* Not only time-based scheduling rules! Magic filters and bool-based rules is available
 
 Currently project is in the design stage and any APIs are to be changed
 
+
+### How to install:
+
+#### Install using pip
+```bash
+pip install indecro
+```
+
 ### How to use:
 
 Create scheduler
 
 ```python
 from indecro import Scheduler
 from indecro.executor import Executor
@@ -32,16 +41,14 @@
 ```python
 from datetime import datetime, timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-
-
 @scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
```

### Comparing `indecro-0.102/indecro/executor.py` & `indecro-0.13/indecro/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     def __init__(self):
         self.daemonized_tasks: set[asyncio.Task] = set()
 
     async def execute(self, job: Job):
         if job.is_running:
             return False
 
-        if job.daemonize == RunAs.FUNCTION:
+        if job.daemonize is RunAs.FUNCTION:
             res = self.sync_worker(job.task, job)
 
             if isinstance(res, Awaitable):
                 await res
 
         else:
-            if job.daemonize == RunAs.THREAD:
+            if job.daemonize is RunAs.THREAD:
                 res = asyncio.to_thread(functools.partial(self.sync_worker, job.task, job))
-            elif job.daemonize == RunAs.ASYNC_TASK:
+            elif job.daemonize is RunAs.ASYNC_TASK:
                 res = job.task()
 
                 if not isinstance(res, Awaitable):
                     pass
                     # TODO: Create warning message here
             else:
                 raise ValueError(f'Invalid job.daemonize value: {job.daemonize}')
```

### Comparing `indecro-0.102/indecro/job.py` & `indecro-0.13/indecro/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import asyncio
 from abc import abstractmethod
 from dataclasses import dataclass, is_dataclass
 from datetime import datetime
-from typing import Optional, Any
+from typing import Optional, Any, Union
 
 from indecro.api.executor import Executor
 from indecro.api.task import Task
-from indecro.api.rules import Rule
+from indecro.api.rules import Rule, BoolRule
 from indecro.api.scheduler import Scheduler
 from indecro.api.job import Job as JobProtocol, RunAs
 
 
 @dataclass
 class Job(JobProtocol):  # If the Job is highlighted in red, the bad work of the paycharm with dataclasses and typehints for them is to blame
     task: Task
-    rule: Rule
+    rule: Union[Rule, BoolRule]
 
     next_run_time: datetime
 
     daemonize: RunAs = RunAs.FUNCTION
 
     name: Optional[str] = None
```

### Comparing `indecro-0.102/indecro/rules.py` & `indecro-0.13/indecro/rules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,59 @@
-from abc import ABC
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime, timedelta
-from typing import Optional
+from typing import Optional, Callable, Any, Union
 
-from indecro.api.rules import Rule
+from magic_filter import MagicFilter
+
+from indecro.api.rules import Rule, BoolRule
 from indecro.exceptions import JobNeverBeScheduled
 
 
 @dataclass
-class RunRegular(Rule):
-    start: datetime
+class RunEvery(Rule):
     period: timedelta
+    after: Optional[Union[datetime, timedelta]] = None
+    before: Optional[Union[datetime, timedelta]] = None
+    repeat: Optional[int] = None
+
+    init_time: datetime = field(default_factory=datetime.now)
+
+    repeats: int = 0
 
     def get_next_schedule_time(self, *, after: datetime) -> datetime:
-        delta = after - self.start
+        # Lazy after timedelta to datetime transformation instead of __init__ redefinition
+        if isinstance(self.after, timedelta):
+            self.after = self.init_time + self.after
+
+        #similar actions for before
+        if isinstance(self.before, timedelta):
+            self.before = self.init_time + self.before
+
+        delta = after - self.init_time
         intervals = delta.total_seconds() // self.period.total_seconds() + 1
-        return self.start + intervals * self.period
+
+        next_schedule_time = self.init_time + intervals * self.period
+
+        if self.before is not None and self.before <= next_schedule_time:
+            raise JobNeverBeScheduled(after=after, by_rule=self)
+
+        if self.repeat is not None and self.repeat <= self.repeats:
+            raise JobNeverBeScheduled(after=after, by_rule=self)
+
+        if self.after is not None and self.after > next_schedule_time:
+            next_schedule_time = self.after
+            self.after = None
+
+        self.repeats += 1
+
+        return next_schedule_time
 
     def __repr__(self):
         # TODO: Remove hardcode from arguments displaying in repr
-        return f'{self.__class__.__name__}(start={repr(self.start)}, period={repr(self.period)})'
+        return f'{self.__class__.__name__}(start={repr(self.after)}, period={repr(self.period)})'
 
     def __hash__(self):
         return hash(repr(self))
 
 
 @dataclass(init=False)
 class RunOnce(Rule):
@@ -51,7 +81,26 @@
 
     def __repr__(self):
         # TODO: Remove hardcode from arguments displaying in repr
         return f'{self.__class__.__name__}(at={repr(self.at)}, after={self.after})'
 
     def __hash__(self):
         return hash(repr(self))
+
+
+@dataclass
+class RunWhen(BoolRule):
+    will: Union[MagicFilter, Callable[[], bool]]
+    subject: Union[None, Any] = None
+
+    def get_must_be_scheduled_now_flag(self):
+        if isinstance(self.will, MagicFilter):
+            return self.will.resolve(self.subject)
+        elif isinstance(self.will, Callable):
+            return self.will()
+
+    def __repr__(self):
+        # TODO: Remove hardcode from arguments displaying in repr
+        return f'{self.__class__.__name__}(at={repr(self.will)}, after={self.subject})'
+
+    def __hash__(self):
+        return hash(repr(self))
```

### Comparing `indecro-0.102/indecro/scheduler.py` & `indecro-0.13/indecro/scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import functools
 from datetime import datetime
 from typing import Optional, Union, Awaitable
 
 from indecro.api.executor import Executor
 from indecro.api.job import RunAs
 from indecro.api.task import Task
-from indecro.exceptions import JobNeverBeScheduled
+from indecro.exceptions import JobNeverBeScheduled, CannotPredictJobSchedulingTime
+from indecro.api.job import Job as JobProtocol
 from indecro.job import Job
 from indecro.api.rules import Rule
 from indecro.api.scheduler import Scheduler as SchedulerProtocol
 from indecro.api.storage import Storage, AsyncStorage
 
 
 class Scheduler(SchedulerProtocol):
@@ -50,47 +51,54 @@
             rule: Rule,
 
             daemonize: RunAs = RunAs.FUNCTION,
 
             name: Optional[str] = None,
             *args,
             **kwargs
-    ) -> Job:
+    ) -> JobProtocol:
         if isinstance(task, Job):
             job = task
         else:
+            try:
+                next_run_time = rule.get_next_schedule_time(after=datetime.now())
+            except CannotPredictJobSchedulingTime:
+                next_run_time = None
             job = Job(
                 task=functools.partial(task, *args, **kwargs),
                 rule=rule,
-                next_run_time=rule.get_next_schedule_time(after=datetime.now()),
+                next_run_time=next_run_time,
                 name=name,
                 scheduler=self,
                 executor=self.executor,
                 daemonize=daemonize
             )
 
         return self.storage.add_job(job)
 
-    async def stop(self):
+    def stop(self):
         self.running = False
 
-    async def execute_job(self, job: Job, reschedule: bool = True):
+    async def execute_job(self, job: JobProtocol, reschedule: bool = True):
         job_executed = await self.executor.execute(job)
 
         if reschedule:
             self.schedule_job(job)
 
         return job_executed
 
     @staticmethod
-    def schedule_job(job: Job):
-        job.next_run_time = job.rule.get_next_schedule_time(after=datetime.now())
-        return job.next_run_time
+    def schedule_job(job: JobProtocol):
+        try:
+            job.next_run_time = job.rule.get_next_schedule_time(after=datetime.now())
+        except CannotPredictJobSchedulingTime:
+            pass
+        return None
 
-    def remove_job(self, job: Job):
+    def remove_job(self, job: JobProtocol):
         return self.storage.remove_job(job)
 
     async def run(self):
         self.running = True
         while self.running:
             now = datetime.now()
 
@@ -101,11 +109,13 @@
                 except JobNeverBeScheduled:
                     res = self.storage.remove_job(job)
 
                     if isinstance(res, Awaitable):
                         await res
 
                     job_executed = False
+                except CannotPredictJobSchedulingTime:  # Looks like BoolRule, we just wait
+                    job_executed = False
 
                 any_job_started = job_executed or any_job_started
 
             await asyncio.sleep(not any_job_started)
```

### Comparing `indecro-0.102/indecro/storage/base.py` & `indecro-0.13/indecro/storage/base.py`

 * *Files identical despite different names*

### Comparing `indecro-0.102/indecro/storage/memory_storage.py` & `indecro-0.13/indecro/storage/memory_storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,16 +21,19 @@
             after: Optional[datetime] = None,
             before: Optional[datetime] = None,
             limit: Optional[int] = None
     ) -> Generator[Job, None, None]:
 
         a = 0
         for job in sorted(self.jobs, key=lambda job: job.next_run_time):
-            # print(f'{job=}')
-            # print(job.next_run_time > datetime.now())
-            if (
+
+            if job.next_run_time is None:
+                if job.rule.get_must_be_scheduled_now_flag():
+                    yield job
+                    a += 1
+            elif (
                     (after is not None and job.next_run_time > after) or
                     (before is not None and job.next_run_time < before)
             ) and \
                     (limit is None or a <= limit):
                 yield job
                 a += 1
```

### Comparing `indecro-0.102/indecro.egg-info/PKG-INFO` & `indecro-0.13/indecro.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indecro
-Version: 0.102
+Version: 0.13
 Summary: Python scheduler with task independency from scheduler, executor and others
 Home-page: https://github.com/TypeHintsFun/indecro
 Author: TypeHintsFun
 Author-email: typehintsfun@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -21,17 +21,26 @@
 All parts are designed to be replaceable.
 
 Main ideas are:
 
 * Task creator doesn't need to know how tasks are implemented or executed
 * Persistence may be implemented
 * You can choose how jobs will be parallelized and whether they will be parallelized at all
+* Not only time-based scheduling rules! Magic filters and bool-based rules is available
 
 Currently project is in the design stage and any APIs are to be changed
 
+
+### How to install:
+
+#### Install using pip
+```bash
+pip install indecro
+```
+
 ### How to use:
 
 Create scheduler
 
 ```python
 from indecro import Scheduler
 from indecro.executor import Executor
@@ -48,16 +57,14 @@
 ```python
 from datetime import datetime, timedelta
 
 from indecro.rules import RunOnce
 
 
 # Rule, theft control time when scheduled task would be executed
-
-
 @scheduler.job(rule=RunOnce(at=datetime.now() + timedelta(seconds=10)))
 async def some_job():
     print('Executing some job..')
 ```
 
 Schedule job using direct function
```

### Comparing `indecro-0.102/setup.py` & `indecro-0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 this_directory = path.abspath(path.dirname(__file__))
 
 setup(
     name='indecro',
     description='Python scheduler with task independency from scheduler, executor and others',
-    version='0.102',
+    version='0.13',
     url='https://github.com/TypeHintsFun/indecro',
     author='TypeHintsFun',
     author_email='typehintsfun@gmail.com',
     license='MIT',
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
```


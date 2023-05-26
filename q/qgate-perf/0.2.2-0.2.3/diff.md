# Comparing `tmp/qgate_perf-0.2.2-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 16532 bytes, number of entries: 16
+Zip file size: 17044 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    11741 b- defN 23-May-16 18:07 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    11942 b- defN 23-May-26 13:56 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-15 18:16 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-26 14:18 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
+-rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     4550 b- defN 23-May-16 18:10 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1286 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/RECORD
-16 files, 51178 bytes uncompressed, 14418 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-26 14:23 qgate_perf-0.2.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-May-26 14:23 qgate_perf-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 14:23 qgate_perf-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-26 14:23 qgate_perf-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-May-26 14:23 qgate_perf-0.2.3.dist-info/RECORD
+17 files, 52183 bytes uncompressed, 14820 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -24,26 +24,29 @@
 
 Filename: qgate_perf/version.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
+Filename: tests/test_dir.py
+Comment: 
+
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.2.dist-info/LICENSE
+Filename: qgate_perf-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.2.dist-info/METADATA
+Filename: qgate_perf-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.2.dist-info/WHEEL
+Filename: qgate_perf-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.2.dist-info/top_level.txt
+Filename: qgate_perf-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.2.dist-info/RECORD
+Filename: qgate_perf-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -1,8 +1,9 @@
 import gc
+import os.path
 from multiprocessing import Process
 import multiprocessing
 import threading
 import datetime
 import time
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
@@ -187,26 +188,33 @@
             run_setup.set_bulk(bulk[0], bulk[1])
 
             # execute
             self.run_executor(executor_list, run_setup)
             time.sleep(sleep_between_bulks)
             gc.collect()
 
+    def _open_output(self):
+        dirname = os.path.dirname(self._output_file)
+        if not os.path.exists(dirname):
+            os.makedirs(dirname)
+        return open(self._output_file, 'a')
+
+
     def run_executor(self, executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                          run_setup: RunSetup=None):
         """ Run executor sequencies
             :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
             :param run_setup:           setup of execution
         """
         file = None
         print('Execution...')
 
         try:
             if self._output_file is not None:
-                file = open(self._output_file, 'a')
+                file=self._open_output()
 
             self._print_header(file, run_setup)
 
             for executors in executor_list:
                 # execution
                 with multiprocessing.Manager() as manager:
                     return_dict = manager.dict()
@@ -234,15 +242,15 @@
             :param run_setup:       setup of execution
         """
         file = None
         print('Execution...')
 
         try:
             if self._output_file is not None:
-                file = open(self._output_file, 'a')
+                file=self._open_output()
 
             self._print_header(file, run_setup)
             # Execution
             with multiprocessing.Manager() as manager:
                 return_dict = manager.dict()
                 self._executeCore(run_setup, return_dict, processes, threads)
                 self._print_detail(file, run_setup, return_dict, processes, threads)
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.2'
+__version__ = '0.2.3'
```

## Comparing `qgate_perf-0.2.2.dist-info/LICENSE` & `qgate_perf-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.2.dist-info/METADATA` & `qgate_perf-0.2.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.2
+Version: 0.2.3
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.2.2.dist-info/RECORD` & `qgate_perf-0.2.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=_XKg0TWSwQsYdpTYv_zuk8kIRTAKFWurLMAyqp8pFbc,11741
+qgate_perf/parallel_executor.py,sha256=IWHBHNfM-LBv4vagWJjyw8BNhrlJGihIiD-0JHN3Qcg,11942
 qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
-qgate_perf/version.py,sha256=tcQaHZtXfWWYoM4ddQOuomrr-c_dFrHFTvhuwK78o-A,215
+qgate_perf/version.py,sha256=3MS6MfRSJQ_bh3YIxei2IsaVHLG-cR_Upg6CLFcE8uI,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
 tests/test_run.py,sha256=DVe9FvaPTfMU0GSRyVdy5zEUk1mzRzjzy6bM2i4uTyo,4550
-qgate_perf-0.2.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.2.2.dist-info/METADATA,sha256=EseI37FJl5_mrxdZaSJvS1zXbaCoSMMwvoUny5ga7qI,6964
-qgate_perf-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.2.2.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.2.2.dist-info/RECORD,,
+qgate_perf-0.2.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.2.3.dist-info/METADATA,sha256=5XzqBcTtRXKyzOmgBPfq4WF0RZNzcOdcDODZsvRoGSU,6964
+qgate_perf-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.2.3.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.2.3.dist-info/RECORD,,
```


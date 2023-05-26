# Comparing `tmp/qgate_perf-0.2.4-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17062 bytes, number of entries: 17
+Zip file size: 17120 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    12109 b- defN 23-May-26 17:50 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    12467 b- defN 23-May-26 18:21 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-26 18:00 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-26 18:15 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
--rw-rw-rw-  2.0 fat     4551 b- defN 23-May-26 17:50 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-26 18:02 qgate_perf-0.2.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-May-26 18:02 qgate_perf-0.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 18:02 qgate_perf-0.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-26 18:02 qgate_perf-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-May-26 18:02 qgate_perf-0.2.4.dist-info/RECORD
-17 files, 52351 bytes uncompressed, 14838 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     4587 b- defN 23-May-26 18:18 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-26 18:23 qgate_perf-0.2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-May-26 18:23 qgate_perf-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 18:23 qgate_perf-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-26 18:23 qgate_perf-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-May-26 18:23 qgate_perf-0.2.5.dist-info/RECORD
+17 files, 52745 bytes uncompressed, 14896 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.4.dist-info/LICENSE
+Filename: qgate_perf-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.4.dist-info/METADATA
+Filename: qgate_perf-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.4.dist-info/WHEEL
+Filename: qgate_perf-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.4.dist-info/top_level.txt
+Filename: qgate_perf-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.4.dist-info/RECORD
+Filename: qgate_perf-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -16,18 +16,19 @@
 from qgate_perf.run_return import RunReturn
 
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
     def __init__(self, func, label=None, detail_output=True, output_file=None):
         """ Setting of execution
-            :param func:            function for parallel run
-            :param label:           text label for parallel run
-            :param detail_output:   provide details output from executors
-            :param output_file:     output to the file, defualt is without file
+
+        :param func:            function for parallel run
+        :param label:           text label for parallel run
+        :param detail_output:   provide details output from executors
+        :param output_file:     output to the file, defualt is without file
         """
         self._func = func
         self._detail_output = detail_output
         self._label =label
         self._output_file = output_file
 
 
@@ -175,14 +176,15 @@
 
     def run_bulk_executor(self,
                               bulk_list= BundleHelper.ROW_1_COL_10_100,
                               executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                               run_setup: RunSetup=None,
                               sleep_between_bulks=0):
         """ Run cykle of bulks in cycle of sequences for function execution
+
         :param bulk_list:           list of bulks for execution in format [[rows, columns], ...]
         :param executor_list:       list of executors for execution in format [[processes, threads], ...]
         :param run_setup:           setup of execution
         :param sleep_between_bulks: sleep between bulks
         """
         for bulk in bulk_list:
             run_setup.set_bulk(bulk[0], bulk[1])
@@ -198,16 +200,17 @@
             os.makedirs(dirname)
         return open(self._output_file, 'a')
 
 
     def run_executor(self, executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                          run_setup: RunSetup=None):
         """ Run executor sequencies
-            :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
-            :param run_setup:           setup of execution
+
+        :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
+        :param run_setup:           setup of execution
         """
         file = None
         print('Execution...')
 
         try:
             if self._output_file is not None:
                 file=self._open_output()
@@ -233,17 +236,17 @@
         finally:
             if file is not None:
                 file.close()
 
     def run(self, processes=2, threads=2, run_setup: RunSetup=None):
         """ Run execution of parallel call
 
-            :param processes:       how much processes will be used
-            :param threads:         how much threads will be used
-            :param run_setup:       setup of execution
+        :param processes:       how much processes will be used
+        :param threads:         how much threads will be used
+        :param run_setup:       setup of execution
         """
         file = None
         print('Execution...')
 
         try:
             if self._output_file is not None:
                 file=self._open_output()
@@ -259,40 +262,48 @@
         except Exception as e:
             self._print(file, str(e) if e is not None else '!! Noname exception !!')
         finally:
             if file is not None:
                 file.close()
 
     def one_run(self, run_setup: RunSetup=None, parameters=None):
-        """ Run test, only one call, execution in new process, with standart write outputs """
+        """ Run test, only one call, execution in new process, with standart write outputs
+
+        :param run_setup:       setting for run
+        :param parameters:      parameters for execution, application in case the run_setup is None
+        """
 
         # setup minimalistic values
         if not run_setup:
             run_setup = RunSetup(duration_second=0, start_delay=0, parameters=parameters)
 
         # run
         self.run(processes=1,
                  threads=1,
                  run_setup=run_setup)
 
-    def test_run(self, run_setup: RunSetup=None, parameters=None):
+    def test_run(self, run_setup: RunSetup=None, parameters=None, print_output=False):
         """ Test call in current process/thread (without ability to define parallel execution and without
-         write standard outputs to file)"""
+         write standard outputs to file)
+
+        :param run_setup:       setting for run
+        :param parameters:      parameters for execution, application in case the run_setup is None
+        :return:                return output from execution
+        """
 
         # init
         key="test-no-parallel"
         dictionary={key: ""}
         run_return = RunReturn(key, dictionary)
 
         if not run_setup:
             run_setup = RunSetup(duration_second=0, start_delay=0, parameters=parameters)
         run_setup.set_start_time()
 
         # test call
         self._func(run_return, run_setup)
 
-        # show output
+        # return output
         ret=dictionary[key]
         if ret:
             print(ret.ToString())
-
-    #TODO: create dir, if not exist
+        return ret
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.4'
+__version__ = '0.2.5'
```

## tests/test_run.py

```diff
@@ -63,27 +63,27 @@
 
     def test_testrun(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file="../output/test_gil_impact_test.txt")
 
-        generator.test_run()
+        generator.test_run(print_output=True)
 
     def test_testrun_setup(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file="../output/test_gil_impact_test.txt")
 
         setting = {"aa": 10,
                    "name": "Adam"}
 
         setup=RunSetup(duration_second=0, start_delay=0, parameters=setting)
-        generator.test_run(run_setup=setup)
+        generator.test_run(run_setup=setup, print_output=True)
 
     def test_run(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file="../output/test_gil_impact_test.txt")
```

## Comparing `qgate_perf-0.2.4.dist-info/LICENSE` & `qgate_perf-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.4.dist-info/METADATA` & `qgate_perf-0.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.4
+Version: 0.2.5
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.2.4.dist-info/RECORD` & `qgate_perf-0.2.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=fSYOfms3njb44YvHtLpEhEslWTRBhZQkZvXtVXPxPjI,12109
+qgate_perf/parallel_executor.py,sha256=RP0WLTjhVCq6ig4CqN7K-t16P0Vg8Lwb9HZNnWXajxA,12467
 qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
-qgate_perf/version.py,sha256=C0QTB7gIh4T9AXgjL8MTyq66LdE1fQXmYTlIbcxC2Bo,215
+qgate_perf/version.py,sha256=qNS6AfoqsJJBmSrxNDE2feLKnZFnaPPGj9pLY0XbiBc,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
-tests/test_run.py,sha256=yjGTC_Y9kYYioZu5awQfAjkvTfA3RCNe3fq_2qfmnSQ,4551
-qgate_perf-0.2.4.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.2.4.dist-info/METADATA,sha256=gl5Ec7d-oOOcPjbxlYjRszn5QhP51Jj8fFVqJxtQQwI,6964
-qgate_perf-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.2.4.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.2.4.dist-info/RECORD,,
+tests/test_run.py,sha256=TZzHiy02r0reYxB2bfoEKsDmtwAEBBXy9ZUy2UCK_9g,4587
+qgate_perf-0.2.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.2.5.dist-info/METADATA,sha256=dclzt9nG6wl9_oex6iu7QA8oDQBnG_EDOGQrHC67ruU,6964
+qgate_perf-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.2.5.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.2.5.dist-info/RECORD,,
```


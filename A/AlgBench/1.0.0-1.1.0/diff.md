# Comparing `tmp/AlgBench-1.0.0.tar.gz` & `tmp/AlgBench-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-1.0.0.tar", last modified: Thu May 25 20:36:49 2023, max compression
+gzip compressed data, was "AlgBench-1.1.0.tar", last modified: Fri May 26 12:05:04 2023, max compression
```

## Comparing `AlgBench-1.0.0.tar` & `AlgBench-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 20:36:37.000000 AlgBench-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18870 2023-05-25 20:36:49.511835 AlgBench-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-05-25 20:36:37.000000 AlgBench-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 20:36:38.000000 AlgBench-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:36:49.511835 AlgBench-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.507835 AlgBench-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.507835 AlgBench-1.0.0/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18870 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 20:36:38.000000 AlgBench-1.0.0/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 12:04:54.000000 AlgBench-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-05-26 12:05:04.899719 AlgBench-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-05-26 12:04:54.000000 AlgBench-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 12:04:55.000000 AlgBench-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:05:04.899719 AlgBench-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.895719 AlgBench-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 12:05:04.000000 AlgBench-1.1.0/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-26 12:04:55.000000 AlgBench-1.1.0/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:05:04.899719 AlgBench-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-26 12:04:55.000000 AlgBench-1.1.0/tests/test_basics.py
```

### Comparing `AlgBench-1.0.0/LICENSE` & `AlgBench-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/PKG-INFO` & `AlgBench-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: AlgBench
-Version: 1.0.0
-Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
 
 There are a number of challenges when performing benchmarks for (long-running)
 algorithms.
 
 - Saving all information requires a lot of **boilerplate code** and often you
   forget something.
@@ -41,14 +30,41 @@
   repairing broken databases by hand
 
 There is a predecessor project, called
 [AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
 data easy, but required more boilerplate code and reading the data was more
 difficult and less efficient.
 
+## Other things you should know about for empirical/experimental evaluations
+
+The following tools I consider essential for empirical evaluations (of algorithms):
+
+* [pandas](https://pandas.pydata.org/): Simple and powerful tool for working with data tables. Do your experiments and parse the important data into a pandas DataFrame.
+* [seaborn](https://seaborn.pydata.org/) and [matplotlib](https://matplotlib.org/): Creating beautiful plots from pandas DataFrames with little work.
+* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/): Interactive Python+Markdown documents. Great for analyzing data and sharing the insights. Works great with pandas and seaborn.
+
+AlgBench essentially takes over the part of saving the information from the runs and allowing you to easily extract pandas DataFrames from it.
+For very simple studies, you could also directly save your data into a Pandas DataFrame but even for nearly every serious experiment, you run into the problems mentioned in the beginning.
+
+Note that the actual algorithms can also be writen in another, more efficient programming language.
+It is reasonably easy to create Python-bindings, e.g., for C++ with [PyBind11](https://pybind11.readthedocs.io/), or just call the binaries with Python.
+
+Publishable evaluations often require extensive experiments that are best performed on a cluster of shared workstations.
+Many institutes and companies are using [slurm](https://slurm.schedmd.com/documentation.html) to schedule and distribute the workloads.
+The data is usually shared via a network file system (NFS), for which AlgBench is designed.
+While you usually also have databases available, they are not made for just dumping all the data you may need for analyzis and potentially debugging into.
+We developed an additonal tool [slurminade](https://github.com/d-krupke/slurminade) that allows you to distribute your experiments with just a few additional lines.
+You can see this in an example: [original script](./examples/graph_coloring/02_run_benchmark.py) vs [script with slurminade](./examples/graph_coloring/02b_run_benchmark_with_slurminade.py).
+
+Let me further recommend the books [A Guide To Experimental Algorithmics by Catherine McGeoch](https://www.cambridge.org/core/books/guide-to-experimental-algorithmics/CDB0CB718F6250E0806C909E1D3D1082) here that gives a good introduction into the big picture of performing empirical evluations for algorithms.
+If you want to know more about actually implementing complex algorithms for difficult problems, I recommend to read [In Pursuit of the Traveling Salesman by Bill Cook](https://press.princeton.edu/books/paperback/9780691163529/in-pursuit-of-the-traveling-salesman) or [The Traveling Salesman Problem: A Computational Study by Appelgate et al.](https://www.math.uwaterloo.ca/tsp/book/index.html) to really go into details.
+The Traveling Salesman Problem is an excellent example for this because it is probably had gotten the most attention of any NP-hard combinatorial problems.
+However, it can also be intimidating as you probably won't have the funds to look into any problem as deep as the Travelings Salesman Problem has been looked at.
+Maybe you want to read some papers from the SIAM Symposium on Algorithm Engineering and Experiments (ALENEX) to see how smaller studies can be performed (though, for most papers you will find aspects that could be improved).
+
 ## Installation
 
 You can install AlgBench using pip
 
 ```bash
 pip install -U algbench
 ```
@@ -467,14 +483,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.1.0** Some changes for efficiency turned out to be less robust in case of, e.g., keyboard interrupt. Fixed that.
 - **1.0.0** Changing the database layout, making it more efficient (breaking
   change!).
 - **0.2.0** Changing database slightly to contain meta data and doing more
   caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
```

### Comparing `AlgBench-1.0.0/README.md` & `AlgBench-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: AlgBench
+Version: 1.1.0
+Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AlgBench: A Python-util to run benchmarks for the empirical evaluation of algorithms.
 
 There are a number of challenges when performing benchmarks for (long-running)
 algorithms.
 
 - Saving all information requires a lot of **boilerplate code** and often you
   forget something.
@@ -30,14 +41,41 @@
   repairing broken databases by hand
 
 There is a predecessor project, called
 [AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
 data easy, but required more boilerplate code and reading the data was more
 difficult and less efficient.
 
+## Other things you should know about for empirical/experimental evaluations
+
+The following tools I consider essential for empirical evaluations (of algorithms):
+
+* [pandas](https://pandas.pydata.org/): Simple and powerful tool for working with data tables. Do your experiments and parse the important data into a pandas DataFrame.
+* [seaborn](https://seaborn.pydata.org/) and [matplotlib](https://matplotlib.org/): Creating beautiful plots from pandas DataFrames with little work.
+* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/): Interactive Python+Markdown documents. Great for analyzing data and sharing the insights. Works great with pandas and seaborn.
+
+AlgBench essentially takes over the part of saving the information from the runs and allowing you to easily extract pandas DataFrames from it.
+For very simple studies, you could also directly save your data into a Pandas DataFrame but even for nearly every serious experiment, you run into the problems mentioned in the beginning.
+
+Note that the actual algorithms can also be writen in another, more efficient programming language.
+It is reasonably easy to create Python-bindings, e.g., for C++ with [PyBind11](https://pybind11.readthedocs.io/), or just call the binaries with Python.
+
+Publishable evaluations often require extensive experiments that are best performed on a cluster of shared workstations.
+Many institutes and companies are using [slurm](https://slurm.schedmd.com/documentation.html) to schedule and distribute the workloads.
+The data is usually shared via a network file system (NFS), for which AlgBench is designed.
+While you usually also have databases available, they are not made for just dumping all the data you may need for analyzis and potentially debugging into.
+We developed an additonal tool [slurminade](https://github.com/d-krupke/slurminade) that allows you to distribute your experiments with just a few additional lines.
+You can see this in an example: [original script](./examples/graph_coloring/02_run_benchmark.py) vs [script with slurminade](./examples/graph_coloring/02b_run_benchmark_with_slurminade.py).
+
+Let me further recommend the books [A Guide To Experimental Algorithmics by Catherine McGeoch](https://www.cambridge.org/core/books/guide-to-experimental-algorithmics/CDB0CB718F6250E0806C909E1D3D1082) here that gives a good introduction into the big picture of performing empirical evluations for algorithms.
+If you want to know more about actually implementing complex algorithms for difficult problems, I recommend to read [In Pursuit of the Traveling Salesman by Bill Cook](https://press.princeton.edu/books/paperback/9780691163529/in-pursuit-of-the-traveling-salesman) or [The Traveling Salesman Problem: A Computational Study by Appelgate et al.](https://www.math.uwaterloo.ca/tsp/book/index.html) to really go into details.
+The Traveling Salesman Problem is an excellent example for this because it is probably had gotten the most attention of any NP-hard combinatorial problems.
+However, it can also be intimidating as you probably won't have the funds to look into any problem as deep as the Travelings Salesman Problem has been looked at.
+Maybe you want to read some papers from the SIAM Symposium on Algorithm Engineering and Experiments (ALENEX) to see how smaller studies can be performed (though, for most papers you will find aspects that could be improved).
+
 ## Installation
 
 You can install AlgBench using pip
 
 ```bash
 pip install -U algbench
 ```
@@ -456,14 +494,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.1.0** Some changes for efficiency turned out to be less robust in case of, e.g., keyboard interrupt. Fixed that.
 - **1.0.0** Changing the database layout, making it more efficient (breaking
   change!).
 - **0.2.0** Changing database slightly to contain meta data and doing more
   caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
```

### Comparing `AlgBench-1.0.0/pyproject.toml` & `AlgBench-1.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "AlgBench"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name = "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)", email = "krupke@ibr.cs.tu-bs.de" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `AlgBench-1.0.0/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-1.1.0/src/AlgBench.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 1.0.0
+Version: 1.1.0
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,14 +41,41 @@
   repairing broken databases by hand
 
 There is a predecessor project, called
 [AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
 data easy, but required more boilerplate code and reading the data was more
 difficult and less efficient.
 
+## Other things you should know about for empirical/experimental evaluations
+
+The following tools I consider essential for empirical evaluations (of algorithms):
+
+* [pandas](https://pandas.pydata.org/): Simple and powerful tool for working with data tables. Do your experiments and parse the important data into a pandas DataFrame.
+* [seaborn](https://seaborn.pydata.org/) and [matplotlib](https://matplotlib.org/): Creating beautiful plots from pandas DataFrames with little work.
+* [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/): Interactive Python+Markdown documents. Great for analyzing data and sharing the insights. Works great with pandas and seaborn.
+
+AlgBench essentially takes over the part of saving the information from the runs and allowing you to easily extract pandas DataFrames from it.
+For very simple studies, you could also directly save your data into a Pandas DataFrame but even for nearly every serious experiment, you run into the problems mentioned in the beginning.
+
+Note that the actual algorithms can also be writen in another, more efficient programming language.
+It is reasonably easy to create Python-bindings, e.g., for C++ with [PyBind11](https://pybind11.readthedocs.io/), or just call the binaries with Python.
+
+Publishable evaluations often require extensive experiments that are best performed on a cluster of shared workstations.
+Many institutes and companies are using [slurm](https://slurm.schedmd.com/documentation.html) to schedule and distribute the workloads.
+The data is usually shared via a network file system (NFS), for which AlgBench is designed.
+While you usually also have databases available, they are not made for just dumping all the data you may need for analyzis and potentially debugging into.
+We developed an additonal tool [slurminade](https://github.com/d-krupke/slurminade) that allows you to distribute your experiments with just a few additional lines.
+You can see this in an example: [original script](./examples/graph_coloring/02_run_benchmark.py) vs [script with slurminade](./examples/graph_coloring/02b_run_benchmark_with_slurminade.py).
+
+Let me further recommend the books [A Guide To Experimental Algorithmics by Catherine McGeoch](https://www.cambridge.org/core/books/guide-to-experimental-algorithmics/CDB0CB718F6250E0806C909E1D3D1082) here that gives a good introduction into the big picture of performing empirical evluations for algorithms.
+If you want to know more about actually implementing complex algorithms for difficult problems, I recommend to read [In Pursuit of the Traveling Salesman by Bill Cook](https://press.princeton.edu/books/paperback/9780691163529/in-pursuit-of-the-traveling-salesman) or [The Traveling Salesman Problem: A Computational Study by Appelgate et al.](https://www.math.uwaterloo.ca/tsp/book/index.html) to really go into details.
+The Traveling Salesman Problem is an excellent example for this because it is probably had gotten the most attention of any NP-hard combinatorial problems.
+However, it can also be intimidating as you probably won't have the funds to look into any problem as deep as the Travelings Salesman Problem has been looked at.
+Maybe you want to read some papers from the SIAM Symposium on Algorithm Engineering and Experiments (ALENEX) to see how smaller studies can be performed (though, for most papers you will find aspects that could be improved).
+
 ## Installation
 
 You can install AlgBench using pip
 
 ```bash
 pip install -U algbench
 ```
@@ -467,14 +494,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.1.0** Some changes for efficiency turned out to be less robust in case of, e.g., keyboard interrupt. Fixed that.
 - **1.0.0** Changing the database layout, making it more efficient (breaking
   change!).
 - **0.2.0** Changing database slightly to contain meta data and doing more
   caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
```

### Comparing `AlgBench-1.0.0/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-1.1.0/src/AlgBench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/__init__.py` & `AlgBench-1.1.0/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/benchmark.py` & `AlgBench-1.1.0/src/algbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/benchmark_db.py` & `AlgBench-1.1.0/src/algbench/benchmark_db.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,18 @@
 
     def get_env_info(self, env_fingerprint):
         return self._env_data[env_fingerprint]
 
     def __iter__(self):
         for entry in self._data:
             entry = entry.copy()
-            entry["env"] = self.get_env_info(entry["env_fingerprint"])
-            yield entry
+            try:
+                entry["env"] = self.get_env_info(entry["env_fingerprint"])
+                yield entry
+            except KeyError:
+                pass
 
     def front(self) -> typing.Optional[typing.Dict]:
         try:
             return next(self.__iter__())
         except StopIteration:
             return None
```

### Comparing `AlgBench-1.0.0/src/algbench/db/json_serializer.py` & `AlgBench-1.1.0/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/db/nfs_json_dict.py` & `AlgBench-1.1.0/src/algbench/db/nfs_json_dict.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,23 +30,20 @@
 
     def __setitem__(self, key: str, value):
         key = str(key)
         value = to_json(value)
         if key in self._values:
             if _equal(self._values[key], value):
                 return
-        self._db.append({key: value}, flush=False)
+        self._db.append({key: value})
         self._values[key] = value
 
     def __getitem__(self, key: str):
         return self._values[key]
 
-    def flush(self):
-        self._db.flush()
-
     def get(self, *args, **kwargs):
         return self._values.get(*args, **kwargs)
 
     def update(self, *args, **kwargs):
         return self._values.update(*args, **kwargs)
 
     def items(self):
```

### Comparing `AlgBench-1.0.0/src/algbench/db/nfs_json_list.py` & `AlgBench-1.1.0/src/algbench/db/nfs_json_list.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/db/nfs_json_set.py` & `AlgBench-1.1.0/src/algbench/db/nfs_json_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __contains__(self, item):
         return item in self._values
 
     def add(self, item):
         item = to_json(item)
         if item not in self._values:
-            self._db.append([item], flush=False)
+            self._db.append([item])
             self._values.add(item)
         return item
 
     def update(self, items):
         for item in items:
             self.add(item)
 
@@ -40,12 +40,9 @@
         self._db.append(list(self._values))
         self._db.compress()
 
     def clear(self):
         self._db.clear()
         self._values.clear()
 
-    def flush(self):
-        self._db.flush()
-
     def delete(self):
         self._db.delete()
```

### Comparing `AlgBench-1.0.0/src/algbench/environment.py` & `AlgBench-1.1.0/src/algbench/environment.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/pandas.py` & `AlgBench-1.1.0/src/algbench/pandas.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/src/algbench/utils/timer.py` & `AlgBench-1.1.0/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-1.0.0/tests/test_basics.py` & `AlgBench-1.1.0/tests/test_basics.py`

 * *Files identical despite different names*


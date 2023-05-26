# Comparing `tmp/Pint-Pandas-0.3.tar.gz` & `tmp/Pint-Pandas-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pint-Pandas-0.3.tar", last modified: Tue Nov 15 00:42:45 2022, max compression
+gzip compressed data, was "Pint-Pandas-0.4.tar", last modified: Fri May 26 21:01:02 2023, max compression
```

## Comparing `Pint-Pandas-0.3.tar` & `Pint-Pandas-0.4.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.831066 Pint-Pandas-0.3/
--rw-r--r--   0 grecco   (11832)    32000       38 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/.coveragerc
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.802452 Pint-Pandas-0.3/.github/
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.810413 Pint-Pandas-0.3/.github/workflows/
--rw-r--r--   0 grecco   (11832)    32000     2600 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/.github/workflows/ci.yml
--rw-r--r--   0 grecco   (11832)    32000      336 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/.github/workflows/lint.yml
--rw-r--r--   0 grecco   (11832)    32000      310 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/.gitignore
--rw-r--r--   0 grecco   (11832)    32000      278 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/.pre-commit-config.yaml
--rw-r--r--   0 grecco   (11832)    32000      317 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/AUTHORS
--rw-r--r--   0 grecco   (11832)    32000     1697 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/CHANGES
--rw-r--r--   0 grecco   (11832)    32000     1584 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/LICENSE
--rw-r--r--   0 grecco   (11832)    32000      438 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/MANIFEST.in
--rw-r--r--   0 grecco   (11832)    32000     3045 2022-11-15 00:42:45.831234 Pint-Pandas-0.3/PKG-INFO
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.824331 Pint-Pandas-0.3/Pint_Pandas.egg-info/
--rw-r--r--   0 grecco   (11832)    32000     3045 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/PKG-INFO
--rw-r--r--   0 grecco   (11832)    32000      695 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/SOURCES.txt
--rw-r--r--   0 grecco   (11832)    32000        1 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/dependency_links.txt
--rw-r--r--   0 grecco   (11832)    32000      110 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/requires.txt
--rw-r--r--   0 grecco   (11832)    32000       12 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/top_level.txt
--rw-r--r--   0 grecco   (11832)    32000        1 2022-11-15 00:42:45.000000 Pint-Pandas-0.3/Pint_Pandas.egg-info/zip-safe
--rw-r--r--   0 grecco   (11832)    32000     2046 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/README.rst
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.825583 Pint-Pandas-0.3/notebooks/
--rw-r--r--   0 grecco   (11832)    32000      170 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/notebooks/pandas_test.csv
--rw-r--r--   0 grecco   (11832)    32000   143276 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/notebooks/pint-pandas.ipynb
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.827319 Pint-Pandas-0.3/pint_pandas/
--rw-r--r--   0 grecco   (11832)    32000      699 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/__init__.py
--rw-r--r--   0 grecco   (11832)    32000    31740 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/pint_array.py
-drwxr-xr-x   0 grecco   (11832)    32000        0 2022-11-15 00:42:45.830636 Pint-Pandas-0.3/pint_pandas/testsuite/
--rw-r--r--   0 grecco   (11832)    32000        0 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/testsuite/__init__.py
--rw-r--r--   0 grecco   (11832)    32000      201 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/testsuite/pandas_test.csv
--rw-r--r--   0 grecco   (11832)    32000     3355 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/testsuite/test_issues.py
--rw-r--r--   0 grecco   (11832)    32000    19703 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/testsuite/test_pandas_extensiontests.py
--rw-r--r--   0 grecco   (11832)    32000    12731 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pint_pandas/testsuite/test_pandas_interface.py
--rw-r--r--   0 grecco   (11832)    32000      512 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/pyproject.toml
--rw-r--r--   0 grecco   (11832)    32000     1617 2022-11-15 00:42:45.833565 Pint-Pandas-0.3/setup.cfg
--rw-r--r--   0 grecco   (11832)    32000      112 2022-11-15 00:42:43.000000 Pint-Pandas-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.951306 Pint-Pandas-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.943306 Pint-Pandas-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.947306 Pint-Pandas-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/ci-pint-master.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/ci-pint-pre.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/lint-autoupdate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-26 21:01:02.951306 Pint-Pandas-0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.947306 Pint-Pandas-0.4/Pint_Pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-26 21:01:02.000000 Pint-Pandas-0.4/Pint_Pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 21:01:02.000000 Pint-Pandas-0.4/Pint_Pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:01:02.000000 Pint-Pandas-0.4/Pint_Pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 21:01:02.000000 Pint-Pandas-0.4/Pint_Pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 21:01:02.000000 Pint-Pandas-0.4/Pint_Pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.947306 Pint-Pandas-0.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/notebooks/pandas_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/notebooks/pint-pandas.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.947306 Pint-Pandas-0.4/pint_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33808 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/pint_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:01:02.947306 Pint-Pandas-0.4/pint_pandas/testsuite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/testsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/testsuite/pandas_test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/testsuite/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/testsuite/test_pandas_extensiontests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pint_pandas/testsuite/test_pandas_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-26 21:00:53.000000 Pint-Pandas-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:01:02.951306 Pint-Pandas-0.4/setup.cfg
```

### Comparing `Pint-Pandas-0.3/.github/workflows/ci.yml` & `Pint-Pandas-0.4/.github/workflows/ci-pint-pre.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-name: CI
+name: CI-pint-pre
 
 on: [push, pull_request]
 
 jobs:
   test:
     strategy:
       matrix:
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [3.9, "3.10", "3.11"]
         numpy: ["numpy>=1.20.3,<2.0.0"]
-        pandas: ["git+https://github.com/andrewgsavage/pandas.git@assert_1_5", 
-        "git+https://github.com/andrewgsavage/pandas.git@assert_almost_equal", ]
+        pandas: ["pandas==1.5.2", ]
         pint: ["pint>=0.20.1"]
 
     runs-on: ubuntu-latest
 
     env:
       TEST_OPTS: "-rfsxEX -s --cov=pint_pandas --cov-config=.coveragerc"
 
@@ -26,14 +25,17 @@
         run: git fetch --depth=1 origin +refs/tags/*:refs/tags/*
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
+      - name: Install pint
+        run: python -m pip install --pre pint
+
       - name: Get pip cache dir
         id: pip-cache
         run: echo "::set-output name=dir::$(pip cache dir)"
 
       - name: Setup caching
         uses: actions/cache@v2
         with:
@@ -42,18 +44,14 @@
           restore-keys: |
             pip-${{ matrix.python-version }}
 
       - name: Install numpy
         if: ${{ matrix.numpy != null }}
         run: pip install "${{matrix.numpy}}"
 
-      - name: Install pint
-        if: ${{ matrix.pint != null }}
-        run: pip install "${{matrix.pint}}"
-
       - name: Install dependencies
         run: |
           pip install .[test]
 
       - name: Install pandas
         if: ${{ matrix.pandas != null }}
         run: pip install "${{matrix.pandas}}"
```

### Comparing `Pint-Pandas-0.3/CHANGES` & `Pint-Pandas-0.4/CHANGES`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 pint-pandas Changelog
 =====================
 
+0.4 (2023-05-26)
+----------------
+
+- Upgraded pint-pandas infrastructure.
+- Support for <NA> values in columns with integer magnitudes
+- Support for magnitudes of any type, such as complex128 or tuples #146
+- Support for Pint 0.21 #168, #179
+- Cast to `numpy.ndarray` in `PintArray._reduce` if needed to use `nanops` functions
+- Minimum Pint version: 0.21+
+- Better testing.
+
 0.3 (2022-11-14)
 ----------------
 
 - Support for pandas 1.5, with a significant uplift in capability. Many operations that gave results with object
   dtype now give PintArrays. #133
 - Fixed a bug which caused the creation of PintArray (and even more so all binary mathematical operations)
   to convert input arrays to lists of Quantity, thereby causing a huge slowdown. #80
```

### Comparing `Pint-Pandas-0.3/LICENSE` & `Pint-Pandas-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Pint-Pandas-0.3/PKG-INFO` & `Pint-Pandas-0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: Pint-Pandas
-Version: 0.3
-Summary: Physical quantities module
-Home-page: https://github.com/hgrecco/pint-pandas
-Author: Hernan E. Grecco
-Author-email: hernan.grecco@gmail.com
+Version: 0.4
+Summary: Extend Pandas Dataframe with Physical quantities module
+Author-email: "Hernan E. Grecco" <hernan.grecco@gmail.com>
 License: BSD
-Keywords: physical,quantities,unit,conversion,science
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/hgrecco/pint-pandas
+Keywords: physical,quantities,unit,conversion,science,pandas,dataframe
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 .. image:: https://img.shields.io/pypi/v/pint-pandas.svg
     :target: https://pypi.python.org/pypi/pint-pandas
     :alt: Latest Version
@@ -71,15 +70,15 @@
     >>> df['power'] = df['torque'] * df['angular_velocity']
     >>> df.dtypes
     torque                                       pint[foot * force_pound]
     angular_velocity                         pint[revolutions_per_minute]
     power               pint[foot * force_pound * revolutions_per_minute]
     dtype: object
 
-More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb 
+More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb
 
 
 Quick Installation
 ------------------
 
 To install Pint-Pandas, simply:
 
@@ -90,10 +89,7 @@
 or utilizing conda, with the conda-forge channel:
 
 .. code-block:: bash
 
     $ conda install -c conda-forge pint-pandas
 
 and then simply enjoy it!
-
-
-
```

### Comparing `Pint-Pandas-0.3/Pint_Pandas.egg-info/PKG-INFO` & `Pint-Pandas-0.4/Pint_Pandas.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: Pint-Pandas
-Version: 0.3
-Summary: Physical quantities module
-Home-page: https://github.com/hgrecco/pint-pandas
-Author: Hernan E. Grecco
-Author-email: hernan.grecco@gmail.com
+Version: 0.4
+Summary: Extend Pandas Dataframe with Physical quantities module
+Author-email: "Hernan E. Grecco" <hernan.grecco@gmail.com>
 License: BSD
-Keywords: physical,quantities,unit,conversion,science
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/hgrecco/pint-pandas
+Keywords: physical,quantities,unit,conversion,science,pandas,dataframe
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 .. image:: https://img.shields.io/pypi/v/pint-pandas.svg
     :target: https://pypi.python.org/pypi/pint-pandas
     :alt: Latest Version
@@ -71,15 +70,15 @@
     >>> df['power'] = df['torque'] * df['angular_velocity']
     >>> df.dtypes
     torque                                       pint[foot * force_pound]
     angular_velocity                         pint[revolutions_per_minute]
     power               pint[foot * force_pound * revolutions_per_minute]
     dtype: object
 
-More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb 
+More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb
 
 
 Quick Installation
 ------------------
 
 To install Pint-Pandas, simply:
 
@@ -90,10 +89,7 @@
 or utilizing conda, with the conda-forge channel:
 
 .. code-block:: bash
 
     $ conda install -c conda-forge pint-pandas
 
 and then simply enjoy it!
-
-
-
```

### Comparing `Pint-Pandas-0.3/Pint_Pandas.egg-info/SOURCES.txt` & `Pint-Pandas-0.4/Pint_Pandas.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 .pre-commit-config.yaml
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
+.github/workflows/ci-pint-master.yml
+.github/workflows/ci-pint-pre.yml
 .github/workflows/ci.yml
+.github/workflows/lint-autoupdate.yml
 .github/workflows/lint.yml
+.github/workflows/publish.yml
 Pint_Pandas.egg-info/PKG-INFO
 Pint_Pandas.egg-info/SOURCES.txt
 Pint_Pandas.egg-info/dependency_links.txt
 Pint_Pandas.egg-info/requires.txt
 Pint_Pandas.egg-info/top_level.txt
-Pint_Pandas.egg-info/zip-safe
 notebooks/pandas_test.csv
 notebooks/pint-pandas.ipynb
 pint_pandas/__init__.py
 pint_pandas/pint_array.py
+pint_pandas/py.typed
 pint_pandas/testsuite/__init__.py
 pint_pandas/testsuite/pandas_test.csv
 pint_pandas/testsuite/test_issues.py
 pint_pandas/testsuite/test_pandas_extensiontests.py
 pint_pandas/testsuite/test_pandas_interface.py
```

### Comparing `Pint-Pandas-0.3/README.rst` & `Pint-Pandas-0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     >>> df['power'] = df['torque'] * df['angular_velocity']
     >>> df.dtypes
     torque                                       pint[foot * force_pound]
     angular_velocity                         pint[revolutions_per_minute]
     power               pint[foot * force_pound * revolutions_per_minute]
     dtype: object
 
-More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb 
+More examples are shown in the example notebook https://github.com/hgrecco/pint-pandas/blob/master/notebooks/pint-pandas.ipynb
 
 
 Quick Installation
 ------------------
 
 To install Pint-Pandas, simply:
 
@@ -62,8 +62,7 @@
 or utilizing conda, with the conda-forge channel:
 
 .. code-block:: bash
 
     $ conda install -c conda-forge pint-pandas
 
 and then simply enjoy it!
-
```

### Comparing `Pint-Pandas-0.3/pint_pandas/__init__.py` & `Pint-Pandas-0.4/pint_pandas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     # so the reported version will be unknown
     __version__ = "unknown"
 
 __all__ = ["PintArray", "PintType", "__version__"]
 
 
 def show_versions():
-
     deps = [
         "pint_pandas",
         "pint",
         "pandas",
         "numpy",
     ]
```

### Comparing `Pint-Pandas-0.3/pint_pandas/pint_array.py` & `Pint-Pandas-0.4/pint_pandas/pint_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,31 @@
         Invoked by unicode(df) in py2 only. Yields a Unicode String in both
         py2/py3.
         """
 
         return self.name
 
 
+dtypemap = {
+    int: pd.Int64Dtype(),
+    np.int64: pd.Int64Dtype(),
+    np.int32: pd.Int32Dtype(),
+    np.int16: pd.Int16Dtype(),
+    np.int8: pd.Int8Dtype(),
+    # np.float128: pd.Float128Dtype(),
+    float: pd.Float64Dtype(),
+    np.float64: pd.Float64Dtype(),
+    np.float32: pd.Float32Dtype(),
+    np.complex128: pd.core.dtypes.dtypes.PandasDtype("complex128"),
+    np.complex64: pd.core.dtypes.dtypes.PandasDtype("complex64"),
+    # np.float16: pd.Float16Dtype(),
+}
+dtypeunmap = {v: k for k, v in dtypemap.items()}
+
+
 class PintArray(ExtensionArray, ExtensionOpsMixin):
     """Implements a class to describe an array of physical quantities:
     the product of an array of numerical values and a unit of measurement.
 
     Parameters
     ----------
     values : pint.Quantity or array-like
@@ -205,34 +222,38 @@
     """
 
     _data = np.array([])
     context_name = None
     context_units = None
 
     def __init__(self, values, dtype=None, copy=False):
-        if dtype is None and isinstance(values, _Quantity):
-            dtype = values.units
+        if dtype is None:
+            if isinstance(values, _Quantity):
+                dtype = values.units
+            elif isinstance(values, PintArray):
+                dtype = values._dtype
         if dtype is None:
             raise NotImplementedError
 
         if not isinstance(dtype, PintType):
             dtype = PintType(dtype)
         self._dtype = dtype
 
         if isinstance(values, _Quantity):
             values = values.to(dtype.units).magnitude
-        if not isinstance(values, np.ndarray):
-            values = np.array(values, copy=copy)
+        elif isinstance(values, PintArray):
+            values = values._data
+        if isinstance(values, np.ndarray):
+            dtype = values.dtype
+            if dtype in dtypemap:
+                dtype = dtypemap[dtype]
+            values = pd.array(values, copy=copy, dtype=dtype)
             copy = False
-        if not np.issubdtype(values.dtype, np.floating):
-            warnings.warn(
-                f"pint-pandas does not support magnitudes of {values.dtype}. Converting magnitudes to float.",
-                category=RuntimeWarning,
-            )
-            values = values.astype(float)
+        elif not isinstance(values, pd.core.arrays.numeric.NumericArray):
+            values = pd.array(values, copy=copy)
             copy = False
         if copy:
             values = values.copy()
         self._data = values
         self._Q = self.dtype.ureg.Quantity
 
     def __getstate__(self):
@@ -325,29 +346,32 @@
             ``boxed=True``.
         """
         float_format = pint.formatting.remove_custom_flags(
             self.dtype.ureg.default_format
         )
 
         def formatting_function(quantity):
-            return "{:{float_format}}".format(
-                quantity.magnitude, float_format=float_format
-            )
+            if isinstance(quantity.magnitude, float):
+                return "{:{float_format}}".format(
+                    quantity.magnitude, float_format=float_format
+                )
+            else:
+                return str(quantity.magnitude)
 
         return formatting_function
 
     def isna(self):
         # type: () -> np.ndarray
         """Return a Boolean NumPy array indicating if each value is missing.
 
         Returns
         -------
         missing : np.array
         """
-        return np.isnan(self._data)
+        return self._data.isna()
 
     def astype(self, dtype, copy=True):
         """Cast to a NumPy array with 'dtype'.
 
         Parameters
         ----------
         dtype : str or dtype
@@ -382,15 +406,15 @@
 
     @property
     def units(self):
         return self._dtype.units
 
     @property
     def quantity(self):
-        return self._Q(self.data, self._dtype.units)
+        return self._Q(self.numpy_data, self._dtype.units)
 
     def take(self, indices, allow_fill=False, fill_value=None):
         """Take elements from an array.
 
         # type: (Sequence[int], bool, Optional[Any]) -> PintArray
 
         Parameters
@@ -492,30 +516,32 @@
         def quantify_nan(item):
             if type(item) is float:
                 return item * dtype.units
             return item
 
         if isinstance(master_scalar, _Quantity):
             scalars = [quantify_nan(item) for item in scalars]
-            scalars = [item.to(dtype.units).magnitude for item in scalars]
+            scalars = [
+                (item.to(dtype.units).magnitude if hasattr(item, "to") else item)
+                for item in scalars
+            ]
         return cls(scalars, dtype=dtype, copy=copy)
 
     @classmethod
     def _from_sequence_of_strings(cls, scalars, dtype=None, copy=False):
         if not dtype:
             dtype = PintType.construct_from_quantity_string(scalars[0])
         return cls._from_sequence([dtype.ureg.Quantity(x) for x in scalars])
 
     @classmethod
     def _from_factorized(cls, values, original):
         return cls(values, dtype=original.dtype)
 
     def _values_for_factorize(self):
-        arr = self._data
-        return arr, np.NaN
+        return self._data._values_for_factorize()
 
     def value_counts(self, dropna=True):
         """
         Returns a Series containing counts of each category.
 
         Every category will have an entry, even those with a count of 0.
 
@@ -533,21 +559,25 @@
         Series.value_counts
         """
 
         from pandas import Series
 
         # compute counts on the data with no nans
         data = self._data
-        if dropna:
-            data = data[~np.isnan(data)]
+        nafilt = np.isnan(data)
+        data = data[~nafilt]
 
         data_list = data.tolist()
         index = list(set(data))
         array = [data_list.count(item) for item in index]
 
+        if not dropna:
+            index.append(np.nan)
+            array.append(nafilt.sum())
+
         return Series(array, index=index)
 
     def unique(self):
         """Compute the PintArray of unique values.
 
         Returns
         -------
@@ -566,14 +596,28 @@
             return super().__contains__(item)
 
     @property
     def data(self):
         return self._data
 
     @property
+    def numpy_data(self):
+        data = self.data
+        if data.dtype in dtypeunmap:
+            try:
+                data = data.astype(dtypeunmap[data.dtype])
+            except Exception:
+                # We might get here for integer arrays with <NA> values
+                # In that case, the returned quantity will have dtype=O, which is less useful.
+                pass
+        if hasattr(data, "to_numpy"):
+            data = data.to_numpy()
+        return data
+
+    @property
     def nbytes(self):
         return self._data.nbytes
 
     # The _can_hold_na attribute is set to True so that pandas internals
     # will use the ExtensionDtype.na_value as the NA value in operations
     # such as take(), reindex(), shift(), etc.  In addition, those results
     # will then be of the ExtensionArray subclass rather than an array
@@ -687,15 +731,18 @@
         if dtype is None or is_object_dtype(dtype):
             return self._to_array_of_quantity(copy=copy)
         if is_string_dtype(dtype):
             return np.array([str(x) for x in self.quantity], dtype=str)
         return np.array(self._data, dtype=dtype, copy=copy)
 
     def _to_array_of_quantity(self, copy=False):
-        qtys = [self._Q(item, self._dtype.units) for item in self._data]
+        qtys = [
+            self._Q(item, self._dtype.units) if not pd.isna(item) else item
+            for item in self._data
+        ]
         with warnings.catch_warnings(record=True):
             return np.array(qtys, dtype="object", copy=copy)
 
     def searchsorted(self, value, side="left", sorter=None):
         """
         Find indices where elements should be inserted to maintain order.
 
@@ -785,15 +832,20 @@
             "sem": nanops.nansem,
             "kurt": nanops.nankurt,
             "skew": nanops.nanskew,
         }
         if name not in functions:
             raise TypeError(f"cannot perform {name} with type {self.dtype}")
 
-        result = functions[name](self._data, **kwds)
+        if isinstance(self._data, ExtensionArray):
+            try:
+                result = self._data._reduce(name, **kwds)
+            except NotImplementedError:
+                result = functions[name](self.numpy_data, **kwds)
+
         if name in {"all", "any", "kurt", "skew"}:
             return result
         if name == "var":
             return self._Q(result, self.units**2)
         return self._Q(result, self.units)
 
 
@@ -988,8 +1040,15 @@
     t = getattr(obj, "dtype", obj)
     try:
         return isinstance(t, PintType) or issubclass(t, PintType)
     except Exception:
         return False
 
 
-compat.upcast_types.append(PintArray)
+try:
+    # for pint < 0.21 we need to explicitly register
+    compat.upcast_types.append(PintArray)
+except AttributeError:
+    # for pint = 0.21 we need to add the full names of PintArray and DataFrame,
+    # which is to be added in pint > 0.21
+    compat.upcast_type_map.setdefault("pint_pandas.pint_array.PintArray", PintArray)
+    compat.upcast_type_map.setdefault("pandas.core.frame.DataFrame", DataFrame)
```

### Comparing `Pint-Pandas-0.3/pint_pandas/testsuite/test_issues.py` & `Pint-Pandas-0.4/pint_pandas/testsuite/test_issues.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,27 @@
         )
         self.assert_equal(result, expected)
 
         # issue #141
         print(PintArray(q_a))
 
 
+class TestIssue68(BaseExtensionTests):
+    def test_assignment_add_empty(self):
+        # GH 68
+        data = PintArray.from_1darray_quantity(
+            np.arange(start=1.0, stop=101.0, dtype=float) * ureg.nm
+        )
+
+        result = pd.Series(data)
+        result[[]] += data[0]
+        expected = pd.Series(data)
+        self.assert_series_equal(result, expected)
+
+
 class TestIssue80:
     @staticmethod
     def _timeit(fun, n_runs=5):
         run_time = []
         for k in range(n_runs):
             t_start = time.monotonic_ns()
             fun()
```

### Comparing `Pint-Pandas-0.3/pint_pandas/testsuite/test_pandas_extensiontests.py` & `Pint-Pandas-0.4/pint_pandas/testsuite/test_pandas_extensiontests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """
 This file contains the tests required by pandas for an ExtensionArray and ExtensionType.
 """
-import itertools
 import warnings
 
 import numpy as np
 import pandas as pd
 import pandas._testing as tm
 import pytest
 from pandas.core import ops
-from pandas.core.dtypes.dtypes import (
-    DatetimeTZDtype,
-    IntervalDtype,
-    PandasDtype,
-    PeriodDtype,
-)
 from pandas.tests.extension import base
-from pandas.tests.extension.conftest import (  # noqa: F401
-    as_array,
-    as_frame,
-    as_series,
-    fillna_method,
-    groupby_apply_op,
-    use_numpy,
+from pandas.tests.extension.conftest import (
+    as_frame,  # noqa: F401
+    as_array,  # noqa: F401,
+    as_series,  # noqa: F401
+    fillna_method,  # noqa: F401
+    groupby_apply_op,  # noqa: F401
+    use_numpy,  # noqa: F401
 )
+
+
 from pint.errors import DimensionalityError
 
 from pint_pandas import PintArray, PintType
+from pint_pandas.pint_array import dtypemap
 
 ureg = PintType.ureg
 
 
 @pytest.fixture(params=[True, False])
 def box_in_series(request):
     """Whether to box the data in a Series"""
@@ -38,44 +34,60 @@
 
 
 @pytest.fixture
 def dtype():
     return PintType("pint[meter]")
 
 
+_base_numeric_dtypes = [float, int]
+_all_numeric_dtypes = _base_numeric_dtypes + [np.complex128]
+
+
+@pytest.fixture(params=_all_numeric_dtypes)
+def numeric_dtype(request):
+    return request.param
+
+
 @pytest.fixture
-def data():
-    return PintArray.from_1darray_quantity(np.arange(start=1.0, stop=101.0) * ureg.nm)
+def data(request, numeric_dtype):
+    return PintArray.from_1darray_quantity(
+        np.arange(start=1.0, stop=101.0, dtype=numeric_dtype) * ureg.nm
+    )
 
 
 @pytest.fixture
-def data_missing():
-    return PintArray.from_1darray_quantity([np.nan, 1.0] * ureg.meter)
+def data_missing(numeric_dtype):
+    numeric_dtype = dtypemap.get(numeric_dtype, numeric_dtype)
+    return PintArray.from_1darray_quantity(
+        ureg.Quantity(pd.array([np.nan, 1], dtype=numeric_dtype), ureg.meter)
+    )
 
 
 @pytest.fixture
-def data_for_twos():
+def data_for_twos(numeric_dtype):
     x = [
         2.0,
     ] * 100
-    return PintArray.from_1darray_quantity(x * ureg.meter)
+    return PintArray.from_1darray_quantity(
+        pd.array(x, dtype=numeric_dtype) * ureg.meter
+    )
 
 
 @pytest.fixture(params=["data", "data_missing"])
 def all_data(request, data, data_missing):
     if request.param == "data":
         return data
     elif request.param == "data_missing":
         return data_missing
 
 
 @pytest.fixture
 def data_repeated(data):
     """Return different versions of data for count times"""
-    # no idea what I'm meant to put here, try just copying from https://github.com/pandas-dev/pandas/blob/master/pandas/tests/extension/integer/test_integer.py
+
     def gen(count):
         for _ in range(count):
             yield data
 
     yield gen
 
 
@@ -85,46 +97,53 @@
     Simple fixture for testing keys in sorting methods.
     Tests None (no key) and the identity key.
     """
     return request.param
 
 
 @pytest.fixture
-def data_for_sorting():
-    return PintArray.from_1darray_quantity([0.3, 10.0, -50.0] * ureg.centimeter)
-    # should probably get more sophisticated and do something like
-    # [1 * ureg.meter, 3 * ureg.meter, 10 * ureg.centimeter]
+def data_for_sorting(numeric_dtype):
+    return PintArray.from_1darray_quantity(
+        pd.array([0.3, 10.0, -50.0], numeric_dtype) * ureg.centimeter
+    )
 
 
 @pytest.fixture
-def data_missing_for_sorting():
-    return PintArray.from_1darray_quantity([4.0, np.nan, -5.0] * ureg.centimeter)
-    # should probably get more sophisticated and do something like
-    # [4 * ureg.meter, np.nan, 10 * ureg.centimeter]
+def data_missing_for_sorting(numeric_dtype):
+    numeric_dtype = dtypemap.get(numeric_dtype, numeric_dtype)
+    return PintArray.from_1darray_quantity(
+        ureg.Quantity(
+            pd.array([4.0, np.nan, -5.0], dtype=numeric_dtype), ureg.centimeter
+        )
+    )
 
 
 @pytest.fixture
 def na_cmp():
     """Binary operator for comparing NA values."""
-    return lambda x, y: bool(np.isnan(x.magnitude)) & bool(np.isnan(y.magnitude))
+    return lambda x, y: bool(pd.isna(x.magnitude)) & bool(pd.isna(y.magnitude))
 
 
 @pytest.fixture
-def na_value():
+def na_value(numeric_dtype):
     return PintType("meter").na_value
 
 
 @pytest.fixture
-def data_for_grouping():
-    # should probably get more sophisticated here and use units on all these
-    # quantities
+def data_for_grouping(numeric_dtype):
     a = 1.0
     b = 2.0**32 + 1
     c = 2.0**32 + 10
-    return PintArray.from_1darray_quantity([b, b, np.nan, np.nan, a, a, b, c] * ureg.m)
+
+    numeric_dtype = dtypemap.get(numeric_dtype, numeric_dtype)
+    return PintArray.from_1darray_quantity(
+        ureg.Quantity(
+            pd.array([b, b, np.nan, np.nan, a, a, b, c], dtype=numeric_dtype), ureg.m
+        )
+    )
 
 
 # === missing from pandas extension docs about what has to be included in tests ===
 # copied from pandas/pandas/conftest.py
 _all_arithmetic_operators = [
     "__add__",
     "__radd__",
@@ -227,15 +246,15 @@
 
 
 class TestGetitem(base.BaseGetitemTests):
     pass
 
 
 class TestGroupby(base.BaseGroupbyTests):
-    # @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
+    @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
     def test_groupby_apply_identity(self, data_for_grouping):
         df = pd.DataFrame({"A": [1, 1, 2, 2, 3, 3, 1, 4], "B": data_for_grouping})
         result = df.groupby("A").B.apply(lambda x: x.array)
         expected = pd.Series(
             [
                 df.B.iloc[[0, 1, 6]].array,
                 df.B.iloc[[2, 3]].array,
@@ -243,15 +262,15 @@
                 df.B.iloc[[7]].array,
             ],
             index=pd.Index([1, 2, 3, 4], name="A"),
             name="B",
         )
         self.assert_series_equal(result, expected)
 
-    # @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
+    @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
     @pytest.mark.parametrize("as_index", [True, False])
     def test_groupby_extension_agg(self, as_index, data_for_grouping):
         df = pd.DataFrame({"A": [1, 1, 2, 2, 3, 3, 1, 4], "B": data_for_grouping})
         result = df.groupby("B", as_index=as_index).A.mean()
         _, uniques = pd.factorize(data_for_grouping, sort=True)
 
         if as_index:
@@ -268,22 +287,19 @@
                 "A": [1, 1, 2, 2, 3, 3, 1, 4],
                 "B": data_for_grouping,
                 "C": [1, 1, 1, 1, 1, 1, 1, 1],
             }
         )
         result = df.groupby("A").sum().columns
 
-        if data_for_grouping.dtype._is_numeric:
-            expected = pd.Index(["B", "C"])
-        else:
-            expected = pd.Index(["C"])
+        expected = pd.Index(["B", "C"])
 
         tm.assert_index_equal(result, expected)
 
-    # @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
+    @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
     def test_groupby_extension_no_sort(self, data_for_grouping):
         df = pd.DataFrame({"A": [1, 1, 2, 2, 3, 3, 1, 4], "B": data_for_grouping})
         result = df.groupby("B", sort=False).A.mean()
         _, index = pd.factorize(data_for_grouping, sort=False)
 
         index = pd.Index._with_infer(index, name="B")
         expected = pd.Series([1.0, 3.0, 4.0], index=index, name="A")
@@ -291,59 +307,17 @@
 
 
 class TestInterface(base.BaseInterfaceTests):
     pass
 
 
 class TestMethods(base.BaseMethodsTests):
-    # @pytest.mark.xfail(
-    #     run=True, reason="TypeError: 'float' object is not subscriptable"
-    # )
-    def test_where_series(self, data, na_value, as_frame):  # noqa: F811
-        assert data[0] != data[1]
-        cls = type(data)
-        a, b = data[:2]
-
-        orig = pd.Series(cls._from_sequence([a, a, b, b], dtype=data.dtype))
-        ser = orig.copy()
-        cond = np.array([True, True, False, False])
-
-        if as_frame:
-            ser = ser.to_frame(name="a")
-            cond = cond.reshape(-1, 1)
-
-        result = ser.where(cond)
-        expected = pd.Series(
-            cls._from_sequence([a, a, na_value, na_value], dtype=data.dtype)
-        )
-
-        if as_frame:
-            expected = expected.to_frame(name="a")
-        self.assert_equal(result, expected)
-
-        ser.mask(~cond, inplace=True)
-        self.assert_equal(ser, expected)
-
-        # array other
-        ser = orig.copy()
-        if as_frame:
-            ser = ser.to_frame(name="a")
-        cond = np.array([True, False, True, True])
-        other = cls._from_sequence([a, b, a, b], dtype=data.dtype)
-        if as_frame:
-            other = pd.DataFrame({"a": other})
-            cond = pd.DataFrame({"a": cond})
-        result = ser.where(cond, other)
-        expected = pd.Series(cls._from_sequence([a, b, b, b], dtype=data.dtype))
-        if as_frame:
-            expected = expected.to_frame(name="a")
-        self.assert_equal(result, expected)
-
-        ser.mask(~cond, other, inplace=True)
-        self.assert_equal(ser, expected)
+    @pytest.mark.skip("All values are valid as magnitudes")
+    def test_insert_invalid(self):
+        pass
 
 
 class TestArithmeticOps(base.BaseArithmeticOpsTests):
     def _check_divmod_op(self, s, op, other, exc=None):
         # divmod has multiple return values, so check separately
         if exc is None:
             result_div, result_mod = op(s, other)
@@ -354,20 +328,29 @@
             self.assert_series_equal(result_div, expected_div)
             self.assert_series_equal(result_mod, expected_mod)
         else:
             with pytest.raises(exc):
                 divmod(s, other)
 
     def _get_exception(self, data, op_name):
+        if data.data.dtype == pd.core.dtypes.dtypes.PandasDtype("complex128"):
+            if op_name in ["__floordiv__", "__rfloordiv__", "__mod__", "__rmod__"]:
+                return op_name, TypeError
         if op_name in ["__pow__", "__rpow__"]:
             return op_name, DimensionalityError
-        else:
-            return op_name, None
+
+        return op_name, None
+
+    @pytest.mark.parametrize("numeric_dtype", _base_numeric_dtypes, indirect=True)
+    def test_divmod_series_array(self, data, data_for_twos):
+        base.BaseArithmeticOpsTests.test_divmod_series_array(self, data, data_for_twos)
 
     def test_arith_series_with_scalar(self, data, all_arithmetic_operators):
+        # With Pint 0.21, series and scalar need to have compatible units for
+        # the arithmetic to work
         # series & scalar
         op_name, exc = self._get_exception(data, all_arithmetic_operators)
         s = pd.Series(data)
         self.check_opname(s, op_name, s.iloc[0], exc=exc)
 
     def test_arith_series_with_array(self, data, all_arithmetic_operators):
         # ndarray & other series
@@ -378,39 +361,20 @@
     def test_arith_frame_with_scalar(self, data, all_arithmetic_operators):
         # frame & scalar
         op_name, exc = self._get_exception(data, all_arithmetic_operators)
         df = pd.DataFrame({"A": data})
         self.check_opname(df, op_name, data[0], exc=exc)
 
     # parameterise this to try divisor not equal to 1
+    @pytest.mark.parametrize("numeric_dtype", _base_numeric_dtypes, indirect=True)
     def test_divmod(self, data):
         s = pd.Series(data)
         self._check_divmod_op(s, divmod, 1 * ureg.Mm)
         self._check_divmod_op(1 * ureg.Mm, ops.rdivmod, s)
 
-    @pytest.mark.parametrize("box", [pd.Series, pd.DataFrame])
-    def test_direct_arith_with_ndframe_returns_not_implemented(self, data, box):
-        # EAs should return NotImplemented for ops with Series/DataFrame
-        # Pandas takes care of unboxing the series and calling the EA's op.
-        other = pd.Series(data)
-        if box is pd.DataFrame:
-            other = other.to_frame()
-        if hasattr(data, "__add__"):
-            result = data.__add__(other)
-            assert result is NotImplemented
-        else:
-            raise pytest.skip(f"{type(data).__name__} does not implement add")
-
-    def test_assignment_add_empty(self, data):
-        # GH 68
-        result = pd.Series(data)
-        result[[]] += data[0]
-        expected = pd.Series(data)
-        self.assert_series_equal(result, expected)
-
 
 class TestComparisonOps(base.BaseComparisonOpsTests):
     def _compare_other(self, s, data, op_name, other):
         op = self.get_op_from_name(op_name)
 
         result = op(s, other)
         expected = op(s.values.quantity, other)
@@ -426,39 +390,20 @@
         # nb this compares an quantity containing array
         # eg Q_([1,2],"m")
         op_name = all_compare_operators
         s = pd.Series(data)
         other = data
         self._compare_other(s, data, op_name, other)
 
-    @pytest.mark.parametrize("box", [pd.Series, pd.DataFrame])
-    def test_direct_arith_with_ndframe_returns_not_implemented(self, data, box):
-        # EAs should return NotImplemented for ops with Series/DataFrame
-        # Pandas takes care of unboxing the series and calling the EA's op.
-        other = pd.Series(data)
-        if box is pd.DataFrame:
-            other = other.to_frame()
-
-        if hasattr(data, "__eq__"):
-            result = data.__eq__(other)
-            assert result is NotImplemented
-        else:
-            raise pytest.skip(f"{type(data).__name__} does not implement __eq__")
-
-        if hasattr(data, "__ne__"):
-            result = data.__ne__(other)
-            assert result is NotImplemented
-        else:
-            raise pytest.skip(f"{type(data).__name__} does not implement __ne__")
-
 
 class TestOpsUtil(base.BaseOpsUtil):
     pass
 
 
+@pytest.mark.parametrize("numeric_dtype", _base_numeric_dtypes, indirect=True)
 class TestParsing(base.BaseParsingTests):
     pass
 
 
 class TestPrinting(base.BasePrintingTests):
     pass
 
@@ -518,15 +463,15 @@
         expected = getattr(pd.Series(s.values.quantity._magnitude), op_name)(
             skipna=skipna
         )
         assert result == expected
 
 
 class TestReshaping(base.BaseReshapingTests):
-    # @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
+    @pytest.mark.xfail(run=True, reason="assert_frame_equal issue")
     @pytest.mark.parametrize(
         "index",
         [
             # Two levels, uniform.
             pd.MultiIndex.from_product(([["A", "B"], ["a", "b"]]), names=["a", "b"]),
             # non-uniform
             pd.MultiIndex.from_tuples([("A", "a"), ("A", "b"), ("B", "b")]),
@@ -541,85 +486,14 @@
                     ("B", "c", 1),
                 ]
             ),
         ],
     )
     @pytest.mark.parametrize("obj", ["series", "frame"])
     def test_unstack(self, data, index, obj):
-        data = data[: len(index)]
-        if obj == "series":
-            ser = pd.Series(data, index=index)
-        else:
-            ser = pd.DataFrame({"A": data, "B": data}, index=index)
-
-        n = index.nlevels
-        levels = list(range(n))
-        # [0, 1, 2]
-        # [(0,), (1,), (2,), (0, 1), (0, 2), (1, 0), (1, 2), (2, 0), (2, 1)]
-        combinations = itertools.chain.from_iterable(
-            itertools.permutations(levels, i) for i in range(1, n)
-        )
-
-        for level in combinations:
-            result = ser.unstack(level=level)
-            assert all(
-                isinstance(result[col].array, type(data)) for col in result.columns
-            )
-
-            if obj == "series":
-                # We should get the same result with to_frame+unstack+droplevel
-                df = ser.to_frame()
-
-                alt = df.unstack(level=level).droplevel(0, axis=1)
-                self.assert_frame_equal(result, alt)
-
-            expected = ser.astype(object).unstack(level=level)
-            result = result.astype(object)
-
-            self.assert_frame_equal(result, expected)
+        base.TestReshaping.test_unstack(self, data, index, obj)
 
 
 class TestSetitem(base.BaseSetitemTests):
-    # @pytest.mark.xfail(run=True, reason="excess warnings, needs debugging")
-    def test_setitem_frame_2d_values(self, data):
-        # GH#44514
-        df = pd.DataFrame({"A": data})
-
-        # These dtypes have non-broken implementations of _can_hold_element
-        has_can_hold_element = isinstance(
-            data.dtype, (PandasDtype, PeriodDtype, IntervalDtype, DatetimeTZDtype)
-        )
-
-        # Avoiding using_array_manager fixture
-        #  https://github.com/pandas-dev/pandas/pull/44514#discussion_r754002410
-        using_array_manager = isinstance(df._mgr, pd.core.internals.ArrayManager)
-
-        blk_data = df._mgr.arrays[0]
-
-        orig = df.copy()
-
-        msg = "will attempt to set the values inplace instead"
-        warn = None
-        if has_can_hold_element and not isinstance(data.dtype, PandasDtype):
-            # PandasDtype excluded because it isn't *really* supported.
-            warn = FutureWarning
-
-        with tm.assert_produces_warning(warn, match=msg):
-            df.iloc[:] = df
-        self.assert_frame_equal(df, orig)
-
-        df.iloc[:-1] = df.iloc[:-1]
-        self.assert_frame_equal(df, orig)
-
-        if isinstance(data.dtype, DatetimeTZDtype):
-            # no warning bc df.values casts to object dtype
-            warn = None
-        with tm.assert_produces_warning(warn, match=msg):
-            df.iloc[:] = df.values
-        self.assert_frame_equal(df, orig)
-        if not using_array_manager:
-            # GH#33457 Check that this setting occurred in-place
-            # FIXME(ArrayManager): this should work there too
-            assert df._mgr.arrays[0] is blk_data
-
-        df.iloc[:-1] = df.values[:-1]
-        self.assert_frame_equal(df, orig)
+    @pytest.mark.parametrize("numeric_dtype", _base_numeric_dtypes, indirect=True)
+    def test_setitem_scalar_key_sequence_raise(self, data):
+        base.BaseSetitemTests.test_setitem_scalar_key_sequence_raise(self, data)
```

### Comparing `Pint-Pandas-0.3/pint_pandas/testsuite/test_pandas_interface.py` & `Pint-Pandas-0.4/pint_pandas/testsuite/test_pandas_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import operator
 from os.path import dirname, join
 
 import numpy as np
 import pandas as pd
 import pytest
-from pandas.tests.extension.conftest import (  # noqa: F401
-    as_array,
-    as_frame,
-    as_series,
-    fillna_method,
-    groupby_apply_op,
-    use_numpy,
+from pandas.tests.extension.conftest import (
+    as_array,  # noqa: F401
+    as_frame,  # noqa: F401
+    as_series,  # noqa: F401
+    fillna_method,  # noqa: F401
+    groupby_apply_op,  # noqa: F401
+    use_numpy,  # noqa: F401
 )
 from pint.testsuite import QuantityTestCase, helpers
 
 from pint_pandas import PintArray, PintType
 
 ureg = PintType.ureg
 
@@ -97,20 +97,23 @@
                     [1.0, 2.0, 2.0, 3.0], dtype="pint[lbf ft]"
                 ),
             }
         )
         expected = pd.DataFrame(
             {
                 ("no_unit_column", "No Unit"): {0: 0.0, 1: 1.0, 2: 2.0, 3: 3.0},
-                ("pintarray_column", "foot * force_pound"): {
-                    0: 1.0,
-                    1: 2.0,
-                    2: 2.0,
-                    3: 3.0,
-                },
+                ("pintarray_column", "foot * force_pound"): pd.Series(
+                    {
+                        0: 1.0,
+                        1: 2.0,
+                        2: 2.0,
+                        3: 3.0,
+                    },
+                    dtype=pd.Float64Dtype(),
+                ),
             }
         )
         expected.columns.names = [None, "unit"]
 
         result = df.pint.dequantify()
         pd.testing.assert_frame_equal(result, expected)
```


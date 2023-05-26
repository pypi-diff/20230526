# Comparing `tmp/py-dot-0.5.1.tar.gz` & `tmp/py_dot-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-dot-0.5.1.tar", last modified: Wed Feb  8 08:32:11 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `py-dot-0.5.1.tar` & `py_dot-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.528602 py-dot-0.5.1/
--rw-rw-rw-   0        0        0      432 2023-02-08 08:32:11.527601 py-dot-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-02-08 08:18:05.000000 py-dot-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.490072 py-dot-0.5.1/py_dot/
--rw-rw-rw-   0        0        0        0 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.507071 py-dot-0.5.1/py_dot/core/
--rw-rw-rw-   0        0        0     1201 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.508582 py-dot-0.5.1/py_dot/core/date/
--rw-rw-rw-   0        0        0     5827 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/date/__init__.py
--rw-rw-rw-   0        0        0       99 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/date/modify.py
--rw-rw-rw-   0        0        0     2011 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/dicts.py
--rw-rw-rw-   0        0        0     1008 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/jsons.py
--rw-rw-rw-   0        0        0      322 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/lists.py
--rw-rw-rw-   0        0        0     1181 2023-02-06 04:54:13.000000 py-dot-0.5.1/py_dot/core/objects.py
--rw-rw-rw-   0        0        0      425 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/operator.py
--rw-rw-rw-   0        0        0      384 2022-12-14 08:32:36.000000 py-dot-0.5.1/py_dot/core/paths.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.509584 py-dot-0.5.1/py_dot/core/regex/
--rw-rw-rw-   0        0        0      201 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/regex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.511586 py-dot-0.5.1/py_dot/core/route/
--rw-rw-rw-   0        0        0     2658 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/route/__init__.py
--rw-rw-rw-   0        0        0      876 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/route/route.py
--rw-rw-rw-   0        0        0     2186 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/strings.py
--rw-rw-rw-   0        0        0      966 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/syntax.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.515590 py-dot-0.5.1/py_dot/core/tests/
--rw-rw-rw-   0        0        0        0 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/__init__.py
--rw-rw-rw-   0        0        0      971 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/test_core.py
--rw-rw-rw-   0        0        0      997 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/test_dicts.py
--rw-rw-rw-   0        0        0      595 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/test_lists.py
--rw-rw-rw-   0        0        0     1446 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/test_route.py
--rw-rw-rw-   0        0        0      394 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/tests/test_strings.py
--rw-rw-rw-   0        0        0     2292 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/core/timer.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.518592 py-dot-0.5.1/py_dot/data/
--rw-rw-rw-   0        0        0     9080 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/__init__.py
--rw-rw-rw-   0        0        0     3084 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/frame.py
--rw-rw-rw-   0        0        0      179 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/summary_time_unit.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.520594 py-dot-0.5.1/py_dot/data/tests/
--rw-rw-rw-   0        0        0        0 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/tests/__init__.py
--rw-rw-rw-   0        0        0      677 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/tests/test_data.py
--rw-rw-rw-   0        0        0     1701 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/data/tests/test_frame.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.521595 py-dot-0.5.1/py_dot/prompt/
--rw-rw-rw-   0        0        0     1441 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/prompt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.522596 py-dot-0.5.1/py_dot/store/
--rw-rw-rw-   0        0        0        0 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/__init__.py
--rw-rw-rw-   0        0        0     3405 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/arrange.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.525598 py-dot-0.5.1/py_dot/store/sqlalchemies/
--rw-rw-rw-   0        0        0     1039 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/sqlalchemies/__init__.py
--rw-rw-rw-   0        0        0     4976 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/sqlalchemies/filter_from_query_string.py
--rw-rw-rw-   0        0        0     5837 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/sqlalchemies/filter_from_string.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.526600 py-dot-0.5.1/py_dot/store/tests/
--rw-rw-rw-   0        0        0        0 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/tests/__init__.py
--rw-rw-rw-   0        0        0     3384 2022-12-14 08:32:37.000000 py-dot-0.5.1/py_dot/store/tests/test_arrange.py
-drwxrwxrwx   0        0        0        0 2023-02-08 08:32:11.500064 py-dot-0.5.1/py_dot.egg-info/
--rw-rw-rw-   0        0        0      432 2023-02-08 08:32:11.000000 py-dot-0.5.1/py_dot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2023-02-08 08:32:11.000000 py-dot-0.5.1/py_dot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 08:32:11.000000 py-dot-0.5.1/py_dot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-08 08:32:11.000000 py-dot-0.5.1/py_dot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-08 08:32:11.528602 py-dot-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-02-08 08:29:49.000000 py-dot-0.5.1/setup.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 py_dot-0.6.0/BUILD.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 py_dot-0.6.0/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/__init__.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/__init__.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/dicts.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/jsons.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/lists.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/objects.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/operator.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/paths.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/strings.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/syntax.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/timer.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/date/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/date/modify.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/regex/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/route/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/route/route.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/__init__.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_core.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_dicts.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_lists.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_route.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/core/tests/test_strings.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/frame.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/summary_time_unit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/test_data.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/data/tests/test_frame.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/prompt/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/prompt/tests/prompt_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/__init__.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/arrange.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/__init__.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_query_string.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_string.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/tests/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 py_dot-0.6.0/py_dot/store/tests/test_arrange.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 py_dot-0.6.0/.gitignore
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 py_dot-0.6.0/README.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 py_dot-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 py_dot-0.6.0/PKG-INFO
```

### Comparing `py-dot-0.5.1/py_dot/core/__init__.py` & `py_dot-0.6.0/py_dot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/date/__init__.py` & `py_dot-0.6.0/py_dot/core/date/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/dicts.py` & `py_dot-0.6.0/py_dot/core/dicts.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/jsons.py` & `py_dot-0.6.0/py_dot/core/jsons.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/objects.py` & `py_dot-0.6.0/py_dot/core/objects.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/route/__init__.py` & `py_dot-0.6.0/py_dot/core/route/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/route/route.py` & `py_dot-0.6.0/py_dot/core/route/route.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/strings.py` & `py_dot-0.6.0/py_dot/core/strings.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/syntax.py` & `py_dot-0.6.0/py_dot/core/syntax.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/tests/test_core.py` & `py_dot-0.6.0/py_dot/core/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/tests/test_dicts.py` & `py_dot-0.6.0/py_dot/core/tests/test_dicts.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/tests/test_route.py` & `py_dot-0.6.0/py_dot/core/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/core/timer.py` & `py_dot-0.6.0/py_dot/core/timer.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/data/__init__.py` & `py_dot-0.6.0/py_dot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/data/frame.py` & `py_dot-0.6.0/py_dot/data/frame.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/data/tests/test_data.py` & `py_dot-0.6.0/py_dot/data/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/data/tests/test_frame.py` & `py_dot-0.6.0/py_dot/data/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/prompt/__init__.py` & `py_dot-0.6.0/py_dot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/store/arrange.py` & `py_dot-0.6.0/py_dot/store/arrange.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/store/sqlalchemies/__init__.py` & `py_dot-0.6.0/py_dot/store/sqlalchemies/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/store/sqlalchemies/filter_from_query_string.py` & `py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_query_string.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/store/sqlalchemies/filter_from_string.py` & `py_dot-0.6.0/py_dot/store/sqlalchemies/filter_from_string.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/py_dot/store/tests/test_arrange.py` & `py_dot-0.6.0/py_dot/store/tests/test_arrange.py`

 * *Files identical despite different names*

### Comparing `py-dot-0.5.1/setup.py` & `py_dot-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / 'README.md').read_text()
 
 """
+>>> pip install twine
+
 >>> py setup.py sdist bdist_wheel
 ... twine check dist/*
 ... twine upload dist/*
+
+>>> py setup.py sdist bdist_wheel
+... py -m twine check dist/*
+... py -m twine upload dist/*
 """
 
 setuptools.setup(
     name='py-dot',
-    version='0.5.1',
+    version='0.6.0',
     description='Python Base Development Library',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/protyliss/py-dot',
     author='Protyliss',
     author_email='protyliss@gmail.com',
     license='MIT',
```


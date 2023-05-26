# Comparing `tmp/pyinputlib-0.0.1.tar.gz` & `tmp/pyinputlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinputlib-0.0.1.tar", last modified: Fri May 26 11:25:01 2023, max compression
+gzip compressed data, was "pyinputlib-0.0.2.tar", last modified: Fri May 26 11:54:36 2023, max compression
```

## Comparing `pyinputlib-0.0.1.tar` & `pyinputlib-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:25:01.573798 pyinputlib-0.0.1/
--rw-rw-rw-   0        0        0      625 2023-05-26 11:25:01.568208 pyinputlib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 11:25:01.540794 pyinputlib-0.0.1/pyinputlib/
--rw-rw-rw-   0        0        0     1040 2023-05-26 10:51:53.000000 pyinputlib-0.0.1/pyinputlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:25:01.565180 pyinputlib-0.0.1/pyinputlib.egg-info/
--rw-rw-rw-   0        0        0      625 2023-05-26 11:25:01.000000 pyinputlib-0.0.1/pyinputlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-26 11:25:01.000000 pyinputlib-0.0.1/pyinputlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:25:01.000000 pyinputlib-0.0.1/pyinputlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 11:25:01.000000 pyinputlib-0.0.1/pyinputlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 11:25:01.573798 pyinputlib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      805 2023-05-26 11:21:09.000000 pyinputlib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:54:36.928444 pyinputlib-0.0.2/
+-rw-rw-rw-   0        0        0      625 2023-05-26 11:54:36.928444 pyinputlib-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 11:54:36.905343 pyinputlib-0.0.2/pyinputlib/
+-rw-rw-rw-   0        0        0     1056 2023-05-26 11:54:18.000000 pyinputlib-0.0.2/pyinputlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:54:36.924329 pyinputlib-0.0.2/pyinputlib.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-05-26 11:54:36.000000 pyinputlib-0.0.2/pyinputlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-26 11:54:36.000000 pyinputlib-0.0.2/pyinputlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:54:36.000000 pyinputlib-0.0.2/pyinputlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 11:54:36.000000 pyinputlib-0.0.2/pyinputlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 11:54:36.932461 pyinputlib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-05-26 11:54:21.000000 pyinputlib-0.0.2/setup.py
```

### Comparing `pyinputlib-0.0.1/PKG-INFO` & `pyinputlib-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinputlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Input Library
 Author: Monil
 Author-email: <monildarediya1@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `pyinputlib-0.0.1/pyinputlib/__init__.py` & `pyinputlib-0.0.2/pyinputlib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, typing
+import os,time
 
 AnswerList = type("AnswerList", (), {})
 
 def funkyInput(ask_value: str | int | bool, defaultVal: None | str = None) -> AnswerList:
     """Adds A ```Funky``` Input"""
     val = str(ask_value) if type(ask_value) == int else ask_value
     deval = " ()" if not defaultVal and not defaultVal == False else f" ({defaultVal})"
@@ -21,8 +21,9 @@
     if not asky == "":
         os.system('cls')
         print(f'{val}\x1b[34m ({asky})\x1b[39m')
         try:
             integered = int(asky)
             return [integered, type(integered)]
         except ValueError:
-            return [asky, type(asky)]
+            return [asky, type(asky)]
+    time.sleep(2)
```

### Comparing `pyinputlib-0.0.1/pyinputlib.egg-info/PKG-INFO` & `pyinputlib-0.0.2/pyinputlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinputlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Input Library
 Author: Monil
 Author-email: <monildarediya1@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
```

### Comparing `pyinputlib-0.0.1/setup.py` & `pyinputlib-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.7",
         "Operating System :: Microsoft :: Windows :: Windows 10"
     ]
 
 setuptools.setup(
     name="pyinputlib",
-    version="0.0.1",
+    version="0.0.2",
     description="A Input Library",
     long_description="Usage\n-----\n - A Library For Nice Inputs, has A Function Named `funkyInput()` Which Takes 2 Arguments `ask_value` and `defaultVal`, `ask_value` for What Will Be Shown In The Input, `defaultVal` - (Optional), For The Default Value To Be Selected If The User Types Nothing",
     author="Monil",
     author_email="<monildarediya1@gmail.com>",
     packages=setuptools.find_packages(),
     requires=[],
     classifiers=classfirs
```


# Comparing `tmp/pyx-pysite-1.0.0.tar.gz` & `tmp/pyx-pysite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyx-pysite-1.0.0.tar", last modified: Fri May 26 17:02:07 2023, max compression
+gzip compressed data, was "pyx-pysite-1.0.1.tar", last modified: Fri May 26 17:42:46 2023, max compression
```

## Comparing `pyx-pysite-1.0.0.tar` & `pyx-pysite-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:02:07.282478 pyx-pysite-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-05-26 16:50:04.000000 pyx-pysite-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1921 2023-05-26 17:02:07.281576 pyx-pysite-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      871 2023-05-26 17:01:55.000000 pyx-pysite-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-26 17:02:07.258182 pyx-pysite-1.0.0/pysite/
--rw-rw-rw-   0        0        0      102 2023-05-26 17:00:50.000000 pyx-pysite-1.0.0/pysite/__init__.py
--rw-rw-rw-   0        0        0     1461 2023-05-26 16:51:54.000000 pyx-pysite-1.0.0/pysite/__main__.py
--rw-rw-rw-   0        0        0     2282 2023-04-23 19:15:14.000000 pyx-pysite-1.0.0/pysite/tags.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:02:07.275957 pyx-pysite-1.0.0/pyx_pysite.egg-info/
--rw-rw-rw-   0        0        0     1921 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 17:02:07.000000 pyx-pysite-1.0.0/pyx_pysite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 17:02:07.282478 pyx-pysite-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 17:42:46.113967 pyx-pysite-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-26 16:50:04.000000 pyx-pysite-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1921 2023-05-26 17:42:46.112967 pyx-pysite-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      900 2023-05-26 17:41:54.000000 pyx-pysite-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-26 17:42:46.077200 pyx-pysite-1.0.1/pysite/
+-rw-rw-rw-   0        0        0      102 2023-05-26 17:00:50.000000 pyx-pysite-1.0.1/pysite/__init__.py
+-rw-rw-rw-   0        0        0     1461 2023-05-26 16:51:54.000000 pyx-pysite-1.0.1/pysite/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:42:46.087602 pyx-pysite-1.0.1/pysite/pyx/
+-rw-rw-rw-   0        0        0        0 2023-05-26 17:40:03.000000 pyx-pysite-1.0.1/pysite/pyx/__init__.py
+-rw-rw-rw-   0        0        0      594 2023-05-26 17:40:38.000000 pyx-pysite-1.0.1/pysite/pyx/generator.py
+-rw-rw-rw-   0        0        0     2682 2023-05-26 17:41:36.000000 pyx-pysite-1.0.1/pysite/pyx/pyxc.py
+-rw-rw-rw-   0        0        0     1376 2023-05-26 17:40:42.000000 pyx-pysite-1.0.1/pysite/pyx/xmlparser.py
+-rw-rw-rw-   0        0        0     2282 2023-04-23 19:15:14.000000 pyx-pysite-1.0.1/pysite/tags.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:42:46.110959 pyx-pysite-1.0.1/pyx_pysite.egg-info/
+-rw-rw-rw-   0        0        0     1921 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 17:42:46.000000 pyx-pysite-1.0.1/pyx_pysite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:42:46.115323 pyx-pysite-1.0.1/setup.cfg
```

### Comparing `pyx-pysite-1.0.0/LICENSE` & `pyx-pysite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyx-pysite-1.0.0/PKG-INFO` & `pyx-pysite-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyx-pysite
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pysite is a Python web framework, inspired by JSX. It uses Flask in the backend. Common commands for the `pysite` CLI are `new <projectname>` and `run`.
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyx-pysite-1.0.0/pyproject.toml` & `pyx-pysite-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
     "flask >= 2.3.0"
 ]
 
-version = "1.0.0"
+version = "1.0.1"
 description = "Pysite is a Python web framework, inspired by JSX. It uses Flask in the backend. Common commands for the `pysite` CLI are `new <projectname>` and `run`."
 
 [project.urls]
 Home = "https://github.com/User0332/pyx"
 
 [project.scripts]
 pysite = "pysite.__main__:main"
+pyxc = "pysite.pyx.pyxc:main"
```

### Comparing `pyx-pysite-1.0.0/pysite/__main__.py` & `pyx-pysite-1.0.1/pysite/__main__.py`

 * *Files identical despite different names*

### Comparing `pyx-pysite-1.0.0/pysite/tags.py` & `pyx-pysite-1.0.1/pysite/tags.py`

 * *Files identical despite different names*

### Comparing `pyx-pysite-1.0.0/pyx_pysite.egg-info/PKG-INFO` & `pyx-pysite-1.0.1/pyx_pysite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyx-pysite
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pysite is a Python web framework, inspired by JSX. It uses Flask in the backend. Common commands for the `pysite` CLI are `new <projectname>` and `run`.
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


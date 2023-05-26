# Comparing `tmp/mapel-2.0.4.tar.gz` & `tmp/mapel-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-2.0.4.tar", last modified: Fri May 26 10:39:55 2023, max compression
+gzip compressed data, was "mapel-2.0.5.tar", last modified: Fri May 26 20:06:37 2023, max compression
```

## Comparing `mapel-2.0.4.tar` & `mapel-2.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:55.049914 mapel-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 10:39:44.000000 mapel-2.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-26 10:39:55.045914 mapel-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 10:39:44.000000 mapel-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:55.045914 mapel-2.0.4/mapel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-26 10:39:55.000000 mapel-2.0.4/mapel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-26 10:39:55.000000 mapel-2.0.4/mapel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:39:55.000000 mapel-2.0.4/mapel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 10:39:55.000000 mapel-2.0.4/mapel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:39:55.000000 mapel-2.0.4/mapel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 10:39:44.000000 mapel-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 10:39:44.000000 mapel-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:39:55.049914 mapel-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:37.037508 mapel-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 20:06:23.000000 mapel-2.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-26 20:06:37.037508 mapel-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 20:06:23.000000 mapel-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:06:37.037508 mapel-2.0.5/mapel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-26 20:06:37.000000 mapel-2.0.5/mapel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-26 20:06:37.000000 mapel-2.0.5/mapel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:06:37.000000 mapel-2.0.5/mapel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 20:06:37.000000 mapel-2.0.5/mapel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:06:37.000000 mapel-2.0.5/mapel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 20:06:23.000000 mapel-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 20:06:23.000000 mapel-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:06:37.037508 mapel-2.0.5/setup.cfg
```

### Comparing `mapel-2.0.4/LICENSE.txt` & `mapel-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-2.0.4/PKG-INFO` & `mapel-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.0.4
+Version: 2.0.5
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-2.0.4/README.md` & `mapel-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mapel-2.0.4/mapel.egg-info/PKG-INFO` & `mapel-2.0.5/mapel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.0.4
+Version: 2.0.5
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-2.0.4/pyproject.toml` & `mapel-2.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
```


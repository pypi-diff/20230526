# Comparing `tmp/roman-4.0.tar.gz` & `tmp/roman-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roman-4.0.tar", last modified: Tue Feb 28 06:59:47 2023, max compression
+gzip compressed data, was "dist/roman-4.1.tar", last modified: Fri May 26 08:25:05 2023, max compression
```

## Comparing `roman-4.0.tar` & `roman-4.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-28 06:59:47.626606 roman-4.0/
--rw-r--r--   0 mac        (513) staff       (20)      855 2023-02-28 06:59:46.000000 roman-4.0/CHANGES.txt
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-02-28 06:59:46.000000 roman-4.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)    11759 2023-02-28 06:59:46.000000 roman-4.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      196 2023-02-28 06:59:46.000000 roman-4.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     3114 2023-02-28 06:59:47.626749 roman-4.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1148 2023-02-28 06:59:46.000000 roman-4.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      423 2023-02-28 06:59:47.627495 roman-4.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1534 2023-02-28 06:59:46.000000 roman-4.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-28 06:59:47.623985 roman-4.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-28 06:59:47.626286 roman-4.0/src/roman.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     3114 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      311 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       37 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        6 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-28 06:59:47.000000 roman-4.0/src/roman.egg-info/zip-safe
--rw-r--r--   0 mac        (513) staff       (20)     3647 2023-02-28 06:59:46.000000 roman-4.0/src/roman.py
--rw-r--r--   0 mac        (513) staff       (20)     2660 2023-02-28 06:59:46.000000 roman-4.0/src/tests.py
--rw-r--r--   0 mac        (513) staff       (20)     1425 2023-02-28 06:59:46.000000 roman-4.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/
+-rw-r--r--   0 jens       (501) staff       (20)     1017 2023-05-26 08:23:27.000000 roman-4.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2023-04-20 08:26:38.000000 roman-4.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       30 2023-05-26 08:23:02.000000 roman-4.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-05-26 08:23:02.000000 roman-4.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      196 2023-04-20 08:26:38.000000 roman-4.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)     4238 2023-05-26 08:25:05.000000 roman-4.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1148 2021-11-02 08:52:53.000000 roman-4.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      423 2023-05-26 08:25:05.000000 roman-4.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2203 2023-05-26 08:23:36.000000 roman-4.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)     4238 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)      325 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       38 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        6 2023-05-26 08:25:05.000000 roman-4.1/src/roman.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-25 13:53:40.000000 roman-4.1/src/roman.egg-info/zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)     4280 2023-05-26 08:23:02.000000 roman-4.1/src/roman.py
+-rw-r--r--   0 jens       (501) staff       (20)     3293 2023-05-26 08:23:02.000000 roman-4.1/src/tests.py
+-rw-r--r--   0 jens       (501) staff       (20)     1425 2023-04-20 08:26:38.000000 roman-4.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `roman-4.0/CONTRIBUTING.md` & `roman-4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `roman-4.0/README.rst` & `roman-4.1/README.rst`

 * *Files identical despite different names*

### Comparing `roman-4.0/src/roman.py` & `roman-4.1/src/roman.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+##############################################################################
+#
+# Copyright (c) 2001 Mark Pilgrim and Contributors.
+# All Rights Reserved.
+#
+# This software is subject to the provisions of the Zope Public License,
+# Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
+# THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
+# WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
+# FOR A PARTICULAR PURPOSE.
+#
+##############################################################################
 """Convert to and from Roman numerals"""
 
 __author__ = "Mark Pilgrim (f8dy@diveintopython.org)"
 __version__ = "1.4"
 __date__ = "8 August 2001"
 __copyright__ = """Copyright (c) 2001 Mark Pilgrim
```

### Comparing `roman-4.0/src/tests.py` & `roman-4.1/src/tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+##############################################################################
+#
+# Copyright (c) 2001 Mark Pilgrim and Contributors.
+# All Rights Reserved.
+#
+# This software is subject to the provisions of the Zope Public License,
+# Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
+# THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
+# WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
+# FOR A PARTICULAR PURPOSE.
+#
+##############################################################################
 import os
 import sys
 import unittest
 from io import StringIO
 
 import roman
```

### Comparing `roman-4.0/tox.ini` & `roman-4.1/tox.ini`

 * *Files identical despite different names*


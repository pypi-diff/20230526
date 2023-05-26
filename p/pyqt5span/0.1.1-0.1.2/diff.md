# Comparing `tmp/pyqt5span-0.1.1.tar.gz` & `tmp/pyqt5span-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5span-0.1.1.tar", last modified: Fri Mar 31 19:49:44 2023, max compression
+gzip compressed data, was "pyqt5span-0.1.2.tar", last modified: Fri May 26 14:34:22 2023, max compression
```

## Comparing `pyqt5span-0.1.1.tar` & `pyqt5span-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 19:49:44.050016 pyqt5span-0.1.1/
--rwxrwxrwx   0 root         (0) root         (0)     1103 2023-03-30 14:59:23.000000 pyqt5span-0.1.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1322 2023-03-31 19:49:44.049413 pyqt5span-0.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      985 2023-03-30 15:13:00.000000 pyqt5span-0.1.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 19:49:44.041751 pyqt5span-0.1.1/pyqt5span/
--rwxrwxrwx   0 root         (0) root         (0)      137 2023-03-25 21:04:44.000000 pyqt5span-0.1.1/pyqt5span/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5351 2023-03-31 19:43:58.000000 pyqt5span-0.1.1/pyqt5span/qspanheadermodel.py
--rwxrwxrwx   0 root         (0) root         (0)    15157 2023-03-30 21:21:26.000000 pyqt5span-0.1.1/pyqt5span/qspanheaderview.py
--rwxrwxrwx   0 root         (0) root         (0)     3930 2023-03-30 21:09:14.000000 pyqt5span-0.1.1/pyqt5span/qspantableview.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 19:49:44.047858 pyqt5span-0.1.1/pyqt5span.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1322 2023-03-31 19:49:43.000000 pyqt5span-0.1.1/pyqt5span.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      299 2023-03-31 19:49:43.000000 pyqt5span-0.1.1/pyqt5span.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-31 19:49:43.000000 pyqt5span-0.1.1/pyqt5span.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-03-31 19:49:43.000000 pyqt5span-0.1.1/pyqt5span.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2023-03-31 19:49:43.000000 pyqt5span-0.1.1/pyqt5span.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-03-31 19:49:44.050191 pyqt5span-0.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-03-31 19:49:11.000000 pyqt5span-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:34:22.680764 pyqt5span-0.1.2/
+-rw-rw-rw-   0        0        0     1121 2023-05-26 14:21:24.000000 pyqt5span-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1361 2023-05-26 14:34:22.679767 pyqt5span-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2023-03-30 15:13:00.000000 pyqt5span-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 14:34:22.637234 pyqt5span-0.1.2/pyqt5span/
+-rw-rw-rw-   0        0        0      137 2023-03-25 21:04:44.000000 pyqt5span-0.1.2/pyqt5span/__init__.py
+-rw-rw-rw-   0        0        0     5351 2023-03-31 19:43:58.000000 pyqt5span-0.1.2/pyqt5span/qspanheadermodel.py
+-rw-rw-rw-   0        0        0    15157 2023-03-30 21:21:26.000000 pyqt5span-0.1.2/pyqt5span/qspanheaderview.py
+-rw-rw-rw-   0        0        0     3930 2023-03-30 21:09:14.000000 pyqt5span-0.1.2/pyqt5span/qspantableview.py
+drwxrwxrwx   0        0        0        0 2023-05-26 14:34:22.677766 pyqt5span-0.1.2/pyqt5span.egg-info/
+-rw-rw-rw-   0        0        0     1361 2023-05-26 14:34:22.000000 pyqt5span-0.1.2/pyqt5span.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-26 14:34:22.000000 pyqt5span-0.1.2/pyqt5span.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 14:34:22.000000 pyqt5span-0.1.2/pyqt5span.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 14:34:22.000000 pyqt5span-0.1.2/pyqt5span.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 14:34:22.000000 pyqt5span-0.1.2/pyqt5span.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 14:34:22.681766 pyqt5span-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      548 2023-05-26 14:23:19.000000 pyqt5span-0.1.2/setup.py
```

### Comparing `pyqt5span-0.1.1/LICENSE` & `pyqt5span-0.1.2/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2023 Edwin Christian Yllanes Cucho, Giovanni L
+Copyright (c) 2019-2023 Edwin Christian Yllanes Cucho, Giovanni Lourenço Fernandes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt5span-0.1.1/PKG-INFO` & `pyqt5span-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: pyqt5span
-Version: 0.1.1
-Summary: Span header for PyQt5
-Home-page: https://github.com/callmegiorgio/pyqt5span
-Author: Edwin Yllanes, Giovanni L
-Author-email: callmegiorgio@hotmail.com
-License: MIT
-Keywords: pyqt5,spanning
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# About
-
-`pyqt5span` is a library extending the PyQt5 framework to provide a way of spanning the
-horizontal and vertical headers of a `QTableView`. Below is a demonstration of this library
-with the script `example.py` in the `samples` directory:
-
-![Example][example-gif]
-
-The source code was adapted from [eyllanesc's solution][eyllanesc-ghrepo] for [this StackOverflow question][so-question-46469720],
-which originally supports the spanning of a header by turning it into a grid. Since that
-solution is meant for a complex use case, it results in an overcomplicated API for simpler
-cases where the user only wants to span rows or columns of standard headers (that is, when
-the user doesn't want a grid header). Hence this small library.
-
-  [example-gif]: <samples/example.gif>
-  [eyllanesc-ghrepo]: <https://github.com/eyllanesc/stackoverflow/tree/master/questions/46469720>
-  [so-question-46469720]: <https://stackoverflow.com/questions/46469720/how-to-make-a-qheaderview-multilevel>
+Metadata-Version: 2.1
+Name: pyqt5span
+Version: 0.1.2
+Summary: Span header for PyQt5
+Home-page: https://github.com/glourencoffee/pyqt5span
+Author: Edwin Yllanes, Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
+License: MIT
+Keywords: pyqt5,spanning
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# About
+
+`pyqt5span` is a library extending the PyQt5 framework to provide a way of spanning the
+horizontal and vertical headers of a `QTableView`. Below is a demonstration of this library
+with the script `example.py` in the `samples` directory:
+
+![Example][example-gif]
+
+The source code was adapted from [eyllanesc's solution][eyllanesc-ghrepo] for [this StackOverflow question][so-question-46469720],
+which originally supports the spanning of a header by turning it into a grid. Since that
+solution is meant for a complex use case, it results in an overcomplicated API for simpler
+cases where the user only wants to span rows or columns of standard headers (that is, when
+the user doesn't want a grid header). Hence this small library.
+
+  [example-gif]: <samples/example.gif>
+  [eyllanesc-ghrepo]: <https://github.com/eyllanesc/stackoverflow/tree/master/questions/46469720>
+  [so-question-46469720]: <https://stackoverflow.com/questions/46469720/how-to-make-a-qheaderview-multilevel>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt5span-0.1.1/README.md` & `pyqt5span-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqt5span-0.1.1/pyqt5span/qspanheadermodel.py` & `pyqt5span-0.1.2/pyqt5span/qspanheadermodel.py`

 * *Files identical despite different names*

### Comparing `pyqt5span-0.1.1/pyqt5span/qspanheaderview.py` & `pyqt5span-0.1.2/pyqt5span/qspanheaderview.py`

 * *Files identical despite different names*

### Comparing `pyqt5span-0.1.1/pyqt5span/qspantableview.py` & `pyqt5span-0.1.2/pyqt5span/qspantableview.py`

 * *Files identical despite different names*

### Comparing `pyqt5span-0.1.1/pyqt5span.egg-info/PKG-INFO` & `pyqt5span-0.1.2/pyqt5span.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: pyqt5span
-Version: 0.1.1
-Summary: Span header for PyQt5
-Home-page: https://github.com/callmegiorgio/pyqt5span
-Author: Edwin Yllanes, Giovanni L
-Author-email: callmegiorgio@hotmail.com
-License: MIT
-Keywords: pyqt5,spanning
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# About
-
-`pyqt5span` is a library extending the PyQt5 framework to provide a way of spanning the
-horizontal and vertical headers of a `QTableView`. Below is a demonstration of this library
-with the script `example.py` in the `samples` directory:
-
-![Example][example-gif]
-
-The source code was adapted from [eyllanesc's solution][eyllanesc-ghrepo] for [this StackOverflow question][so-question-46469720],
-which originally supports the spanning of a header by turning it into a grid. Since that
-solution is meant for a complex use case, it results in an overcomplicated API for simpler
-cases where the user only wants to span rows or columns of standard headers (that is, when
-the user doesn't want a grid header). Hence this small library.
-
-  [example-gif]: <samples/example.gif>
-  [eyllanesc-ghrepo]: <https://github.com/eyllanesc/stackoverflow/tree/master/questions/46469720>
-  [so-question-46469720]: <https://stackoverflow.com/questions/46469720/how-to-make-a-qheaderview-multilevel>
+Metadata-Version: 2.1
+Name: pyqt5span
+Version: 0.1.2
+Summary: Span header for PyQt5
+Home-page: https://github.com/glourencoffee/pyqt5span
+Author: Edwin Yllanes, Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
+License: MIT
+Keywords: pyqt5,spanning
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# About
+
+`pyqt5span` is a library extending the PyQt5 framework to provide a way of spanning the
+horizontal and vertical headers of a `QTableView`. Below is a demonstration of this library
+with the script `example.py` in the `samples` directory:
+
+![Example][example-gif]
+
+The source code was adapted from [eyllanesc's solution][eyllanesc-ghrepo] for [this StackOverflow question][so-question-46469720],
+which originally supports the spanning of a header by turning it into a grid. Since that
+solution is meant for a complex use case, it results in an overcomplicated API for simpler
+cases where the user only wants to span rows or columns of standard headers (that is, when
+the user doesn't want a grid header). Hence this small library.
+
+  [example-gif]: <samples/example.gif>
+  [eyllanesc-ghrepo]: <https://github.com/eyllanesc/stackoverflow/tree/master/questions/46469720>
+  [so-question-46469720]: <https://stackoverflow.com/questions/46469720/how-to-make-a-qheaderview-multilevel>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyqt5span-0.1.1/setup.py` & `pyqt5span-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='pyqt5span',
-    version='0.1.1',
+    version='0.1.2',
     description='Span header for PyQt5',
     long_description=readme,
     long_description_content_type='text/markdown',
-    author='Edwin Yllanes, Giovanni L',
-    author_email='callmegiorgio@hotmail.com',
-    url='https://github.com/callmegiorgio/pyqt5span',
+    author='Edwin Yllanes, Giovanni Lourenço',
+    author_email='gvnl.developer@outlook.com',
+    url='https://github.com/glourencoffee/pyqt5span',
     license='MIT',
     packages=['pyqt5span'],
     keywords=['pyqt5', 'spanning'],
 
     install_requires=['PyQt5'],
 
     python_requires='>=3.7'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


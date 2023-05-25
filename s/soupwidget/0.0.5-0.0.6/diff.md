# Comparing `tmp/soupwidget-0.0.5.tar.gz` & `tmp/soupwidget-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soupwidget-0.0.5.tar", max compression
+gzip compressed data, was "soupwidget-0.0.6.tar", max compression
```

## Comparing `soupwidget-0.0.5.tar` & `soupwidget-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2022-12-12 23:03:27.404206 soupwidget-0.0.5/README.md
--rw-r--r--   0        0        0      359 2023-02-20 13:38:50.551699 soupwidget-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       37 2022-12-12 23:03:27.404206 soupwidget-0.0.5/soupwidget/__init__.py
--rw-r--r--   0        0        0     8505 2023-02-20 13:35:42.749035 soupwidget-0.0.5/soupwidget/widget.py
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 soupwidget-0.0.5/setup.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 soupwidget-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-12 23:03:27.404206 soupwidget-0.0.6/README.md
+-rw-r--r--   0        0        0      360 2023-05-25 23:46:01.123628 soupwidget-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-12-12 23:03:27.404206 soupwidget-0.0.6/soupwidget/__init__.py
+-rw-r--r--   0        0        0     8513 2023-05-25 19:47:00.561755 soupwidget-0.0.6/soupwidget/widget.py
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 soupwidget-0.0.6/PKG-INFO
```

### Comparing `soupwidget-0.0.5/soupwidget/widget.py` & `soupwidget-0.0.6/soupwidget/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import functools
 import bs4
 import json
 
 gen_soup = lambda s='', p='html.parser': bs4.BeautifulSoup(s, p)
 
 def dict_deep_update(orig_dict, new_dict):
-    import collections
+    import collections.abc
     for key, val in new_dict.items():
-        if isinstance(val, collections.Mapping):
+        if isinstance(val, collections.abc.Mapping):
             tmp = dict_deep_update(orig_dict.get(key, { }), val)
             orig_dict[key] = tmp
         elif isinstance(val, list):
             orig_dict[key] = (orig_dict.get(key, []) + val)
         else:
             orig_dict[key] = new_dict[key]
     return orig_dict
```


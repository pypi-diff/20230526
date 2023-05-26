# Comparing `tmp/json-cpp-1.0.7.tar.gz` & `tmp/json-cpp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-cpp-1.0.7.tar", last modified: Mon Dec 27 20:03:18 2021, max compression
+gzip compressed data, was "json-cpp-1.0.9.tar", last modified: Thu Jan 13 17:49:26 2022, max compression
```

## Comparing `json-cpp-1.0.7.tar` & `json-cpp-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-27 20:03:18.049591 json-cpp-1.0.7/
--rwxrwxrwx   0 german    (1000) german    (1000)      217 2021-12-27 20:03:18.037593 json-cpp-1.0.7/PKG-INFO
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-27 20:03:17.399608 json-cpp-1.0.7/json_cpp/
--rwxrwxrwx   0 german    (1000) german    (1000)       45 2021-12-27 20:03:14.000000 json-cpp-1.0.7/json_cpp/__init__.py
--rwxrwxrwx   0 german    (1000) german    (1000)     8557 2021-12-27 20:03:14.000000 json-cpp-1.0.7/json_cpp/json_object.py
--rwxrwxrwx   0 german    (1000) german    (1000)      225 2021-12-27 20:03:15.000000 json-cpp-1.0.7/json_cpp/util.py
-drwxrwxrwx   0 german    (1000) german    (1000)        0 2021-12-27 20:03:17.940593 json-cpp-1.0.7/json_cpp.egg-info/
--rwxrwxrwx   0 german    (1000) german    (1000)      217 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/PKG-INFO
--rwxrwxrwx   0 german    (1000) german    (1000)      260 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/SOURCES.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/dependency_links.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        1 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/not-zip-safe
--rwxrwxrwx   0 german    (1000) german    (1000)        9 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/requires.txt
--rwxrwxrwx   0 german    (1000) german    (1000)        9 2021-12-27 20:03:16.000000 json-cpp-1.0.7/json_cpp.egg-info/top_level.txt
--rwxrwxrwx   0 german    (1000) german    (1000)       38 2021-12-27 20:03:18.054592 json-cpp-1.0.7/setup.cfg
--rwxrwxrwx   0 german    (1000) german    (1000)      251 2021-12-27 20:03:14.000000 json-cpp-1.0.7/setup.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-13 17:49:26.090217 json-cpp-1.0.9/
+-rwxrwxrwx   0 german    (1000) german    (1000)      217 2022-01-13 17:49:26.088226 json-cpp-1.0.9/PKG-INFO
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-13 17:49:26.017550 json-cpp-1.0.9/json_cpp/
+-rwxrwxrwx   0 german    (1000) german    (1000)       45 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp/__init__.py
+-rwxrwxrwx   0 german    (1000) german    (1000)     8653 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp/json_object.py
+-rwxrwxrwx   0 german    (1000) german    (1000)      225 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp/util.py
+drwxrwxrwx   0 german    (1000) german    (1000)        0 2022-01-13 17:49:26.077217 json-cpp-1.0.9/json_cpp.egg-info/
+-rwxrwxrwx   0 german    (1000) german    (1000)      217 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/PKG-INFO
+-rwxrwxrwx   0 german    (1000) german    (1000)      260 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        1 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/not-zip-safe
+-rwxrwxrwx   0 german    (1000) german    (1000)        9 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/requires.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)        9 2022-01-13 17:49:25.000000 json-cpp-1.0.9/json_cpp.egg-info/top_level.txt
+-rwxrwxrwx   0 german    (1000) german    (1000)       38 2022-01-13 17:49:26.090217 json-cpp-1.0.9/setup.cfg
+-rwxrwxrwx   0 german    (1000) german    (1000)      251 2022-01-13 17:49:25.000000 json-cpp-1.0.9/setup.py
```

### Comparing `json-cpp-1.0.7/json_cpp/json_object.py` & `json-cpp-1.0.9/json_cpp/json_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from .util import check_type, unique_string
-
+from datetime import datetime
 
 class classorinstancemethod(classmethod):
 
     def __get__(self, instance, type_):
         descr_get = super().__get__ if instance is None else self.__func__.__get__
         return descr_get(instance, type_)
 
@@ -23,14 +23,16 @@
             if k[0] == "_":
                 continue
             if s:
                 s += ","
             s += "\"%s\":" % k
             if isinstance(v[k], str):
                 s += "%s" % json.dumps(v[k])
+            elif isinstance(v[k], datetime):
+                s += "\"%s\"" % str(v[k])
             elif isinstance(v[k], bool):
                 s += "%s" % str(v[k]).lower()
             else:
                 s += "%s" % str(v[k])
         return "{%s}" % s
 
     def __eq__(self, other):
@@ -182,18 +184,18 @@
         self._typeCheck(val)
         list.insert(self, i, val)
 
     def __str__(self):
         return "[" + ",".join([json.dumps(x) if type(x) is str else str(x) for x in self]) + "]"
 
     def get(self, m):
-        it = type(vars(self.list_type)[m])
-        l = JsonList(list_type=it)
+        l = JsonList()
         for i in self:
-            l.append(vars(i)[m])
+            if m in vars(i):
+                l.append(vars(i)[m])
         return l
 
     def where(self, m, v, o="=="):
         nl = type(self)()
         for i in self:
             if type(vars(i)[m]) is str or issubclass(type(vars(i)[m]), JsonObject):
                 e = "'%s' %s '%s'" % (str(vars(i)[m]), o, str(v))
```


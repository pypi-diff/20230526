# Comparing `tmp/interegular-0.3.1.tar.gz` & `tmp/interegular-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interegular-0.3.1.tar", last modified: Sat Mar 11 15:45:10 2023, max compression
+gzip compressed data, was "interegular-0.3.2.tar", last modified: Fri May 26 11:30:36 2023, max compression
```

## Comparing `interegular-0.3.1.tar` & `interegular-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 15:45:10.243572 interegular-0.3.1/
--rw-rw-rw-   0        0        0     1096 2023-03-02 16:22:45.000000 interegular-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2995 2023-03-11 15:45:10.243572 interegular-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-03-09 12:07:03.000000 interegular-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 15:45:10.232057 interegular-0.3.1/interegular/
--rw-rw-rw-   0        0        0     1104 2023-03-11 15:39:11.000000 interegular-0.3.1/interegular/__init__.py
--rw-rw-rw-   0        0        0     7198 2023-03-11 15:38:01.000000 interegular-0.3.1/interegular/comparator.py
--rw-rw-rw-   0        0        0    38781 2023-03-11 14:16:57.000000 interegular-0.3.1/interegular/fsm.py
--rw-rw-rw-   0        0        0    25887 2023-03-08 18:56:08.000000 interegular-0.3.1/interegular/patterns.py
--rw-rw-rw-   0        0        0        0 2023-03-02 22:21:14.000000 interegular-0.3.1/interegular/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-11 15:45:10.241574 interegular-0.3.1/interegular/utils/
--rw-rw-rw-   0        0        0      451 2023-03-08 19:04:57.000000 interegular-0.3.1/interegular/utils/__init__.py
--rw-rw-rw-   0        0        0     5361 2023-03-02 16:22:45.000000 interegular-0.3.1/interegular/utils/simple_parser.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:45:10.240573 interegular-0.3.1/interegular.egg-info/
--rw-rw-rw-   0        0        0     2995 2023-03-11 15:45:10.000000 interegular-0.3.1/interegular.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-03-11 15:45:10.000000 interegular-0.3.1/interegular.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 15:45:10.000000 interegular-0.3.1/interegular.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-03-11 15:45:10.000000 interegular-0.3.1/interegular.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-11 15:45:10.000000 interegular-0.3.1/interegular.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      150 2023-03-11 15:45:10.248082 interegular-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-03-02 22:21:47.000000 interegular-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-11 15:45:10.243572 interegular-0.3.1/tests/
--rw-rw-rw-   0        0        0     2322 2023-03-11 15:42:00.000000 interegular-0.3.1/tests/test_comparator.py
--rw-rw-rw-   0        0        0     3109 2023-03-02 16:22:45.000000 interegular-0.3.1/tests/test_patterns.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:30:36.803370 interegular-0.3.2/
+-rw-rw-rw-   0        0        0     1096 2023-03-02 16:22:45.000000 interegular-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2995 2023-05-26 11:30:36.803898 interegular-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-03-09 12:07:03.000000 interegular-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 11:30:36.793055 interegular-0.3.2/interegular/
+-rw-rw-rw-   0        0        0     1128 2023-05-26 11:30:13.000000 interegular-0.3.2/interegular/__init__.py
+-rw-rw-rw-   0        0        0     7198 2023-03-11 15:38:01.000000 interegular-0.3.2/interegular/comparator.py
+-rw-rw-rw-   0        0        0    38781 2023-03-11 14:16:57.000000 interegular-0.3.2/interegular/fsm.py
+-rw-rw-rw-   0        0        0    25902 2023-05-26 11:30:13.000000 interegular-0.3.2/interegular/patterns.py
+-rw-rw-rw-   0        0        0        0 2023-03-02 22:21:14.000000 interegular-0.3.2/interegular/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-26 11:30:36.801257 interegular-0.3.2/interegular/utils/
+-rw-rw-rw-   0        0        0      451 2023-03-08 19:04:57.000000 interegular-0.3.2/interegular/utils/__init__.py
+-rw-rw-rw-   0        0        0     5361 2023-03-02 16:22:45.000000 interegular-0.3.2/interegular/utils/simple_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:30:36.799654 interegular-0.3.2/interegular.egg-info/
+-rw-rw-rw-   0        0        0     2995 2023-05-26 11:30:36.000000 interegular-0.3.2/interegular.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-05-26 11:30:36.000000 interegular-0.3.2/interegular.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 11:30:36.000000 interegular-0.3.2/interegular.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-26 11:30:36.000000 interegular-0.3.2/interegular.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-26 11:30:36.000000 interegular-0.3.2/interegular.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      150 2023-05-26 11:30:36.804966 interegular-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-03-02 22:21:47.000000 interegular-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 11:30:36.802848 interegular-0.3.2/tests/
+-rw-rw-rw-   0        0        0     2322 2023-03-11 15:42:00.000000 interegular-0.3.2/tests/test_comparator.py
+-rw-rw-rw-   0        0        0     4480 2023-05-26 11:27:02.000000 interegular-0.3.2/tests/test_patterns.py
```

### Comparing `interegular-0.3.1/LICENSE.txt` & `interegular-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/PKG-INFO` & `interegular-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interegular
-Version: 0.3.1
+Version: 0.3.2
 Summary: a regex intersection checker
 Home-page: https://github.com/MegaIng/regex_intersections
 Download-URL: https://github.com/MegaIng/interegular/tarball/master
 Author: MegaIng
 Author-email: MegaIng <trampchamp@hotmail.de>
 License: MIT
 Classifier: Operating System :: OS Independent
```

### Comparing `interegular-0.3.1/README.md` & `interegular-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/interegular/__init__.py` & `interegular-0.3.2/interegular/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 
 def compare_regexes(*regexes: str) -> Iterable[Tuple[str, str]]:
     """
     Checks the regexes for intersections. Returns all pairs it found
     """
     c = Comparator({r: parse_pattern(r) for r in regexes})
+    print(c._patterns)
     return c.check(regexes)
 
 
 def compare_patterns(*ps: Pattern) -> Iterable[Tuple[Pattern, Pattern]]:
     """
     Checks the Patterns for intersections. Returns all pairs it found
     """
     c = Comparator({p: p for p in ps})
     return c.check(ps)
 
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
```

### Comparing `interegular-0.3.1/interegular/comparator.py` & `interegular-0.3.2/interegular/comparator.py`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/interegular/fsm.py` & `interegular-0.3.2/interegular/fsm.py`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/interegular/patterns.py` & `interegular-0.3.2/interegular/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,18 +168,18 @@
     def simplify(self) -> '_CharGroup':
         return self
 
 
 def _combine_char_groups(*groups: _CharGroup, negate):
     pos = set().union(*(g.chars for g in groups if not g.negated))
     neg = set().union(*(g.chars for g in groups if g.negated))
-    if negate:
-        return _CharGroup(frozenset(neg - pos), False)
+    if neg:
+        return _CharGroup(frozenset(neg - pos), not negate)
     else:
-        return _CharGroup(frozenset(pos - neg), False)
+        return _CharGroup(frozenset(pos - neg), negate)
 
 
 @dataclass(frozen=True)
 class __DotCls(_Repeatable):
 
     def to_fsm(self, alphabet=None, prefix_postfix=None, flags=REFlags(0)) -> FSM:
         if alphabet is None:
@@ -693,15 +693,15 @@
             try:
                 groups.append(self.chargroup_inner())
             except nomatch:
                 break
         self.static("]")
         if len(groups) == 1:
             f = tuple(groups)[0]
-            return _CharGroup(f.chars, negate)
+            return _CharGroup(f.chars, negate ^ f.negated)
         elif len(groups) == 0:
             return _CharGroup(frozenset({}), negate)
         else:
             return _combine_char_groups(*groups, negate=negate)
 
     def chargroup_inner(self) -> _CharGroup:
         start = self.index
```

### Comparing `interegular-0.3.1/interegular/utils/simple_parser.py` & `interegular-0.3.2/interegular/utils/simple_parser.py`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/interegular.egg-info/PKG-INFO` & `interegular-0.3.2/interegular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interegular
-Version: 0.3.1
+Version: 0.3.2
 Summary: a regex intersection checker
 Home-page: https://github.com/MegaIng/regex_intersections
 Download-URL: https://github.com/MegaIng/interegular/tarball/master
 Author: MegaIng
 Author-email: MegaIng <trampchamp@hotmail.de>
 License: MIT
 Classifier: Operating System :: OS Independent
```

### Comparing `interegular-0.3.1/setup.py` & `interegular-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `interegular-0.3.1/tests/test_comparator.py` & `interegular-0.3.2/tests/test_comparator.py`

 * *Files identical despite different names*


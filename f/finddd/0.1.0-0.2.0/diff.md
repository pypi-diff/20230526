# Comparing `tmp/finddd-0.1.0.tar.gz` & `tmp/finddd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finddd-0.1.0.tar", last modified: Thu May 25 06:34:27 2023, max compression
+gzip compressed data, was "finddd-0.2.0.tar", last modified: Fri May 26 21:46:10 2023, max compression
```

## Comparing `finddd-0.1.0.tar` & `finddd-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2023-05-21 03:58:36.724089 finddd-0.1.0/README.md
--rw-r--r--   0        0        0      436 2023-05-25 06:34:27.994629 finddd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-23 16:46:41.626983 finddd-0.1.0/src/finddd/__init__.py
--rw-r--r--   0        0        0      183 2023-05-24 07:49:06.111382 finddd-0.1.0/src/finddd/const.py
--rw-r--r--   0        0        0     3379 2023-05-24 18:24:11.411402 finddd-0.1.0/src/finddd/find.py
--rw-r--r--   0        0        0     9192 2023-05-24 18:19:05.634800 finddd-0.1.0/src/finddd/match.py
--rw-r--r--   0        0        0        0 2023-05-23 18:15:54.195230 finddd-0.1.0/src/finddd/py.typed
--rw-r--r--   0        0        0      209 2023-05-24 18:19:05.549394 finddd-0.1.0/src/finddd/test_find.py
--rw-r--r--   0        0        0     2885 2023-05-21 17:57:29.429850 finddd-0.1.0/src/finddd/test_match.py
--rw-r--r--   0        0        0      212 1970-01-01 00:00:00.000000 finddd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      192 2023-05-26 21:37:40.678372 finddd-0.2.0/README.md
+-rw-r--r--   0        0        0      436 2023-05-26 21:46:10.467428 finddd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-23 16:46:41.626983 finddd-0.2.0/src/finddd/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-24 07:49:06.111382 finddd-0.2.0/src/finddd/const.py
+-rw-r--r--   0        0        0     3379 2023-05-24 18:24:11.411402 finddd-0.2.0/src/finddd/find.py
+-rw-r--r--   0        0        0     9571 2023-05-26 21:28:44.039733 finddd-0.2.0/src/finddd/match.py
+-rw-r--r--   0        0        0        0 2023-05-23 18:15:54.195230 finddd-0.2.0/src/finddd/py.typed
+-rw-r--r--   0        0        0      190 2023-05-26 21:44:14.370483 finddd-0.2.0/src/finddd/test_find.py
+-rw-r--r--   0        0        0     6373 2023-05-26 21:44:14.492275 finddd-0.2.0/src/finddd/test_match.py
+-rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 finddd-0.2.0/PKG-INFO
```

### Comparing `finddd-0.1.0/src/finddd/find.py` & `finddd-0.2.0/src/finddd/find.py`

 * *Files identical despite different names*

### Comparing `finddd-0.1.0/src/finddd/match.py` & `finddd-0.2.0/src/finddd/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,26 @@
     def __init__(
         self,
         pattern: Union[str, re.Pattern[str]],
         *,
         ignore_case: bool = False,
         mode: FilenameMatchMode = FMM_RE,
     ):
+        """init
+
+        Args:
+            pattern (Union[str, re.Pattern[str]]): match pattern
+
+            ignore_case (bool, optional): ignore case. Defaults to False.
+
+            glob mode will be always ignore case.
+            if pattern is a compiled regex object, this option will do nothing.
+
+            mode (FilenameMatchMode, optional): match mode. Defaults to FMM_RE.
+        """
         if ignore_case and isinstance(pattern, str) and mode != FMM_RE:
             pattern = pattern.lower()
 
         if isinstance(pattern, re.Pattern):
             mode = FMM_RE
         if mode == FMM_RE and isinstance(pattern, str):
             pattern = re.compile(pattern)
@@ -63,22 +75,22 @@
         self.ignore_case = ignore_case
 
     def match(self, path: Path) -> bool:  # type: ignore
         name = path.name
         if self.ignore_case:
             name = name.lower()
         if self.mode == FMM_EXACT:
-            return path.name == self.pattern
+            return name == self.pattern
         if self.mode == FMM_STR:
-            return self.pattern in path.name  # type: ignore
+            return self.pattern in name  # type: ignore
         if self.mode == FMM_GLOB:
-            return fnmatch.fnmatch(path.name, self.pattern)  # type: ignore
+            return fnmatch.fnmatch(name, self.pattern)  # type: ignore
         if self.mode == FMM_RE:
             try:
-                next(self.pattern.finditer(path.name))  # type: ignore
+                next(self.pattern.finditer(name))  # type: ignore
             except StopIteration:
                 return False
             return True
         assert isinstance(self.mode, FilenameMatchMode)
 
 
 class SizeMatcher(Matcher):
@@ -249,19 +261,19 @@
 
     def match(self, path: Path) -> bool:
         depth = len(path.parts) - len(self.cur.parts)
         assert depth >= 0
         if self.exact is not None:
             return self.exact == depth
         if self.within:
-            return self.min < depth < self.max  # type: ignore
+            return self.min <= depth <= self.max  # type: ignore
         if self.min is not None:
-            return depth > self.min
+            return depth >= self.min
         if self.max is not None:
-            return depth < self.max
+            return depth <= self.max
         return True
 
 
 class ChangeTimeMatcher(Matcher):
     def __init__(
         self,
         *,
```


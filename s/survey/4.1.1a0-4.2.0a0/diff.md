# Comparing `tmp/survey-4.1.1a0.tar.gz` & `tmp/survey-4.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.1.1a0.tar", last modified: Sat May 13 11:54:14 2023, max compression
+gzip compressed data, was "survey-4.2.0a0.tar", last modified: Fri May 26 21:23:12 2023, max compression
```

## Comparing `survey-4.1.1a0.tar` & `survey-4.2.0a0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:54:14.444218 survey-4.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-13 11:54:02.000000 survey-4.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-13 11:54:14.440218 survey-4.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-13 11:54:02.000000 survey-4.1.1a0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:54:14.444218 survey-4.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-13 11:54:02.000000 survey-4.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:54:14.440218 survey-4.1.1a0/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:54:14.440218 survey-4.1.1a0/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    58488 2023-05-13 11:54:02.000000 survey-4.1.1a0/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:54:14.440218 survey-4.1.1a0/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-13 11:54:14.000000 survey-4.1.1a0/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-13 11:54:14.000000 survey-4.1.1a0/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:54:14.000000 survey-4.1.1a0/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-13 11:54:14.000000 survey-4.1.1a0/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-13 11:54:14.000000 survey-4.1.1a0/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:23:12.434557 survey-4.2.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-26 21:23:02.000000 survey-4.2.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 21:23:12.434557 survey-4.2.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 21:23:02.000000 survey-4.2.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:23:12.434557 survey-4.2.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-26 21:23:02.000000 survey-4.2.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:23:12.430557 survey-4.2.0a0/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:23:12.434557 survey-4.2.0a0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58488 2023-05-26 21:23:02.000000 survey-4.2.0a0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:23:12.434557 survey-4.2.0a0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 21:23:12.000000 survey-4.2.0a0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-26 21:23:12.000000 survey-4.2.0a0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:23:12.000000 survey-4.2.0a0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-26 21:23:12.000000 survey-4.2.0a0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 21:23:12.000000 survey-4.2.0a0/survey.egg-info/top_level.txt
```

### Comparing `survey-4.1.1a0/LICENSE` & `survey-4.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/PKG-INFO` & `survey-4.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.1.1a0
+Version: 4.2.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.1.1a0/README.rst` & `survey-4.2.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/setup.py` & `survey-4.2.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.rst') as file:
     readme = file.read()
 
 author = 'Exahilosys'
 project = 'survey'
-version = '4.1.1-alpha'
+version = '4.2.0-alpha'
 
 url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
     name = project,
     python_requires = '>=3.11',
     version = version,
```

### Comparing `survey-4.1.1a0/survey/__init__.py` & `survey-4.2.0a0/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_colors.py` & `survey-4.2.0a0/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_controls.py` & `survey-4.2.0a0/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/__init__.py` & `survey-4.2.0a0/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_ansi.py` & `survey-4.2.0a0/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_console.py` & `survey-4.2.0a0/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_cursor.py` & `survey-4.2.0a0/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_handle.py` & `survey-4.2.0a0/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_helpers.py` & `survey-4.2.0a0/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_io.py` & `survey-4.2.0a0/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_io_os.py` & `survey-4.2.0a0/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_io_os_nt.py` & `survey-4.2.0a0/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_io_os_posix.py` & `survey-4.2.0a0/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_render.py` & `survey-4.2.0a0/survey/_core/_render.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_screen.py` & `survey-4.2.0a0/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_core/_source.py` & `survey-4.2.0a0/survey/_core/_source.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_funnels.py` & `survey-4.2.0a0/survey/_funnels.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     :param rune:
         The rune used to fill empty space.
 
     .. code-block::
 
         'The quic k brown fox'
         'jumps ov|er the lazy dog'
-        'and falls on its face'
+        'and fall s on its face'
 
         >>> text_min_horizontal(JustType.center, 25, ' ')
 
         '   The qu ick brown fox   '
         ' jumps ov|er the lazy dog '
         '  and fal ls on its face  '
     """
@@ -553,23 +553,14 @@
 
     return functools.partial(_mesh_delegate, check, aware, function)
 
 
 def _mesh_delimit(axis, rune,
                   tiles, point):
     
-    """
-    Insert text between tiles.
-
-    :param axis:
-        The axis considered for the operation.
-    :param rune:
-        The text to insert.
-    """
-    
     all_a = (spot[axis] for spot in tiles)
     max_a = max(all_a)
 
     def check(spot, tile):
         return spot[axis] < max_a
     
     bloat = _text_bloat_horizontal if axis else _text_bloat_vertical
@@ -580,22 +571,20 @@
 
 
 @_call_direct
 def mesh_delimit(axis: int, 
                  rune: str):
     
     """
-    Call a function on each tile of the mesh.
+    Insert text between tiles.
 
-    :param function:
-        The function called.
-    :param check:
-        Used as :code:`(spot, tile) -> bool` to denote whether the specific tile gets ignored.
-    :param aware:
-        Whether to prepend the tile's ``spot`` to the function's arguments.
+    :param axis:
+        The axis considered for the operation.
+    :param rune:
+        The text to insert.
     """
 
     return functools.partial(_mesh_delimit, axis, rune)
 
 
 def _mesh_focal(function,
                 tiles, point):
@@ -667,15 +656,15 @@
 
 
 @_call_direct
 def mesh_point(focus_rune: str,
                evade_rune: str):
     
     """
-    Prepend a to the pointed tile's first line and another to all others.
+    Prepend a rune to the pointed tile's first line and another to all others.
 
     All other lines have empty characters prepended to align with the first.
 
     :param focus_rune:
         The rune for the pointed tile.
     :param evade_rune:
         The rune for the other tiles.
```

### Comparing `survey-4.1.1a0/survey/_graphics.py` & `survey-4.2.0a0/survey/_graphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,33 +24,33 @@
 class Graphic(abc.ABC):
 
     """
     Base for graphics.
 
     :param inline:
         Whether ``\\n`` should **not** be used upon closing.
-    :param frequency:
+    :param throttle:
         Seconds for printing time throttling.
     :param epilogue:
         Shown upon closing instead of the completed graphic.
     """
 
     _lock = threading.RLock()
 
     _top_point = (0, 0)
     _cur_count = 0
 
     def __init__(self, 
                  inline   : bool = False, 
-                 frequency: float = 0.1,
+                 throttle : float = 0.1,
                  epilogue : str | typing.Callable[[], str] | None = None):
 
         self._inline = inline
 
-        self._frequency = frequency
+        self._throttle = throttle
         self._time_last = 0
 
         self._epilogue = epilogue
 
         io = _system.io
         cursor = _system.cursor
         render = _core.Render(cursor, io)
@@ -88,15 +88,15 @@
         return (lines, point)
     
     @_helpers.ctxmethod(lambda self: self._lock)
     def _print(self, check, *, close = False):
 
         time_next = time.time()
 
-        if check and time_next - self._time_last < self._frequency:
+        if check and time_next - self._time_last < self._throttle:
             return
         
         self._time_last = time_next
 
         sketch = functools.partial(self._sketch, close)
 
         self._screen.print(sketch, True, clean = False)
@@ -168,17 +168,25 @@
         self._cursor.hidden.leave()
 
 
 class BaseProgress(Graphic):
 
     """
     Base for progress graphics.
+
+    :param frequency:
+       The amount to wait between automatically adding 1.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, 
+                 *args, 
+                 frequency: float = None,
+                 **kwargs):
+        
+        self._frequency = frequency
 
         self._cycle_actual = 0
         self._cycle_memory = 0
 
         super().__init__(*args, **kwargs)
 
     def _print(self, check, *args, **kwargs):
@@ -189,14 +197,36 @@
             return
         
         self._cycle_actual += size
         self._cycle_memory = 0
 
         super()._print(check, *args, **kwargs)
 
+    def _start_auto(self):
+
+        while not self._frequency is None:
+            self._add(1)
+            time.sleep(self._frequency)
+
+    def _start(self):
+
+        super()._start()
+
+        self._frequency_rolling = self._frequency
+
+        self._thread = thread = threading.Thread(target = self._start_auto, daemon = True)
+        
+        thread.start()
+
+    def _close(self):
+
+        self._frequency_rolling = None
+
+        super()._close()
+
     def _set(self, step):
 
         self._cycle_memory = max(0, step)
 
         self._print(True)
 
     def set(self, step):
```

### Comparing `survey-4.1.1a0/survey/_handle.py` & `survey-4.2.0a0/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_helpers.py` & `survey-4.2.0a0/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_mutates.py` & `survey-4.2.0a0/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_printers.py` & `survey-4.2.0a0/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_routines.py` & `survey-4.2.0a0/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_searches.py` & `survey-4.2.0a0/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_stage.py` & `survey-4.2.0a0/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_theme.py` & `survey-4.2.0a0/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_utils.py` & `survey-4.2.0a0/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_visuals.py` & `survey-4.2.0a0/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey/_widgets.py` & `survey-4.2.0a0/survey/_widgets.py`

 * *Files identical despite different names*

### Comparing `survey-4.1.1a0/survey.egg-info/PKG-INFO` & `survey-4.2.0a0/survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.1.1a0
+Version: 4.2.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.1.1a0/survey.egg-info/SOURCES.txt` & `survey-4.2.0a0/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*


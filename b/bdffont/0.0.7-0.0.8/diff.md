# Comparing `tmp/bdffont-0.0.7.tar.gz` & `tmp/bdffont-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.7.tar", last modified: Mon May  8 07:42:13 2023, max compression
+gzip compressed data, was "bdffont-0.0.8.tar", last modified: Fri May 26 07:35:00 2023, max compression
```

## Comparing `bdffont-0.0.7.tar` & `bdffont-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 07:41:54.000000 bdffont-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 07:42:13.065421 bdffont-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-08 07:41:54.000000 bdffont-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-08 07:41:54.000000 bdffont-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:42:13.065421 bdffont-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.061421 bdffont-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/src/bdffont/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-08 07:41:54.000000 bdffont-0.0.7/src/bdffont/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/src/bdffont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 07:42:13.000000 bdffont-0.0.7/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:42:13.065421 bdffont-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_damaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-08 07:41:54.000000 bdffont-0.0.7/tests/test_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:34:46.000000 bdffont-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 07:35:00.775603 bdffont-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-26 07:34:46.000000 bdffont-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 07:34:46.000000 bdffont-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:35:00.775603 bdffont-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.771603 bdffont-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.771603 bdffont-0.0.8/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-26 07:34:46.000000 bdffont-0.0.8/src/bdffont/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 07:35:00.000000 bdffont-0.0.8/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:35:00.775603 bdffont-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-26 07:34:46.000000 bdffont-0.0.8/tests/test_type.py
```

### Comparing `bdffont-0.0.7/LICENSE` & `bdffont-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/PKG-INFO` & `bdffont-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BdfFont
 
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
-BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format), written in Python.
+BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format).
 
 ## Installation
 
 ```commandline
 pip install bdffont
 ```
```

### Comparing `bdffont-0.0.7/README.md` & `bdffont-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # BdfFont
 
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
-BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format), written in Python.
+BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format).
 
 ## Installation
 
 ```commandline
 pip install bdffont
 ```
```

### Comparing `bdffont-0.0.7/pyproject.toml` & `bdffont-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.7"
+version = "0.0.8"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.7/src/bdffont/error.py` & `bdffont-0.0.8/src/bdffont/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 class BdfValueIncorrect(BdfException):
     def __init__(self, word: str):
         self.word = word
         super().__init__(f"'{word}' value incorrect")
 
 
 class BdfIllegalBitmap(BdfException):
-    pass
+    def __init__(self, code_point: int, reason: str):
+        self.code_point = code_point
+        super().__init__(f"Glyph '{code_point}': {reason}")
 
 
 class BdfIllegalPropertiesKey(BdfException):
     pass
 
 
 class BdfIllegalPropertiesValue(BdfException):
```

### Comparing `bdffont-0.0.7/src/bdffont/font.py` & `bdffont-0.0.8/src/bdffont/font.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/src/bdffont/glyph.py` & `bdffont-0.0.8/src/bdffont/glyph.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,18 +93,18 @@
 
     @bounding_box.setter
     def bounding_box(self, value: tuple[int, int, int, int]):
         self.bounding_box_width, self.bounding_box_height, self.bounding_box_offset_x, self.bounding_box_offset_y = value
 
     def check_bitmap_validity(self):
         if len(self.bitmap) != self.bounding_box_height:
-            raise BdfIllegalBitmap("Glyph bitmap height not equals 'bounding_box_height'")
+            raise BdfIllegalBitmap(self.code_point, f"bitmap height not equals 'bounding_box_height'")
         for bitmap_row in self.bitmap:
             if len(bitmap_row) != self.bounding_box_width:
-                raise BdfIllegalBitmap("Glyph bitmap width not equals 'bounding_box_width'")
+                raise BdfIllegalBitmap(self.code_point, f"bitmap width not equals 'bounding_box_width'")
 
     def get_8bit_aligned_bitmap(self, optimize_bitmap: bool = False) -> tuple[tuple[int, int], tuple[int, int], list[list[int]]]:
         self.check_bitmap_validity()
         bounding_box_width = self.bounding_box_width
         bounding_box_height = self.bounding_box_height
         bounding_box_offset_x = self.bounding_box_offset_x
         bounding_box_offset_y = self.bounding_box_offset_y
```

### Comparing `bdffont-0.0.7/src/bdffont/parser.py` & `bdffont-0.0.8/src/bdffont/parser.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/src/bdffont/properties.py` & `bdffont-0.0.8/src/bdffont/properties.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/src/bdffont.egg-info/PKG-INFO` & `bdffont-0.0.8/src/bdffont.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BdfFont
 
 [![PyPI](https://img.shields.io/pypi/v/bdffont)](https://pypi.org/project/bdffont/)
 
-BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format), written in Python.
+BdfFont is a library for manipulating [`.bdf` format fonts](https://en.wikipedia.org/wiki/Glyph_Bitmap_Distribution_Format).
 
 ## Installation
 
 ```commandline
 pip install bdffont
 ```
```

### Comparing `bdffont-0.0.7/tests/test_damaged.py` & `bdffont-0.0.8/tests/test_damaged.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/tests/test_demo.py` & `bdffont-0.0.8/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.7/tests/test_type.py` & `bdffont-0.0.8/tests/test_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -242,33 +242,40 @@
 
 def test_bitmap():
     glyph = BdfGlyph(
         name='A',
         code_point=ord('A'),
         scalable_width=(0, 0),
         device_width=(0, 0),
-        bounding_box_size=(5, 5),
+        bounding_box_size=(5, 10),
         bounding_box_offset=(0, 0),
         bitmap=[
             [0, 1, 1, 1, 0],
             [0, 1, 1, 1, 0],
             [0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0],
         ]
     )
     glyph.check_bitmap_validity()
 
     glyph.bitmap.pop()
-    with pytest.raises(BdfIllegalBitmap):
+    with pytest.raises(BdfIllegalBitmap) as info:
         glyph.check_bitmap_validity()
+    assert info.value.code_point == glyph.code_point
 
     glyph.bitmap.append([0, 0, 0, 0, 0, 0])
-    with pytest.raises(BdfIllegalBitmap):
+    with pytest.raises(BdfIllegalBitmap) as info:
         glyph.check_bitmap_validity()
+    assert info.value.code_point == glyph.code_point
 
     glyph.bitmap[-1].pop()
     glyph.check_bitmap_validity()
 
     (width, height), (offset_x, offset_y), bitmap = glyph.get_8bit_aligned_bitmap()
     assert len(bitmap) == height == glyph.bounding_box_height
     for bitmap_row in bitmap:
@@ -279,8 +286,8 @@
 
     (width, height), (offset_x, offset_y), bitmap = glyph.get_8bit_aligned_bitmap(optimize_bitmap=True)
     assert len(bitmap) == height == 2
     for bitmap_row in bitmap:
         assert width == 3
         assert len(bitmap_row) == 8
     assert offset_x == 1
-    assert offset_y == 3
+    assert offset_y == 8
```


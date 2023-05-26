# Comparing `tmp/nico-font-tool-0.0.3.tar.gz` & `tmp/nico-font-tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nico-font-tool-0.0.3.tar", last modified: Wed May 24 06:44:47 2023, max compression
+gzip compressed data, was "nico-font-tool-0.0.4.tar", last modified: Fri May 26 07:39:47 2023, max compression
```

## Comparing `nico-font-tool-0.0.3.tar` & `nico-font-tool-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.736398 nico-font-tool-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/src/nico_font_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/nicofont.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/src/nico_font_tool/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 06:44:47.000000 nico-font-tool-0.0.3/src/nico_font_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 06:44:47.740398 nico-font-tool-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-24 06:44:32.000000 nico-font-tool-0.0.3/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:39:47.676383 nico-font-tool-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/nico_font_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/nicofont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/src/nico_font_tool/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 07:39:47.000000 nico-font-tool-0.0.4/src/nico_font_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:39:47.672383 nico-font-tool-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 07:39:33.000000 nico-font-tool-0.0.4/tests/test_.py
```

### Comparing `nico-font-tool-0.0.3/LICENSE` & `nico-font-tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.3/PKG-INFO` & `nico-font-tool-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
```

### Comparing `nico-font-tool-0.0.3/README.md` & `nico-font-tool-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.3/pyproject.toml` & `nico-font-tool-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nico-font-tool"
-version = "0.0.3"
+version = "0.0.4"
 description = "A tool for converting fonts to NICO Game Framework format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool/__init__.py` & `nico-font-tool-0.0.4/src/nico_font_tool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,16 +41,16 @@
             font_file_path,
             glyph_offset_x,
             glyph_offset_y,
             glyph_adjust_width,
             glyph_adjust_height,
         )
     else:
-        raise Exception(f'font file type not supported: {font_ext}')
-    logger.info(f'loaded font file: {font_file_path}')
+        raise Exception(f'Font file type not supported: {font_ext}')
+    logger.info(f"Loaded font file: '{font_file_path}'")
 
     # 图集对象，初始化左边界
     sheet_data = [[_glyph_data_border] for _ in range(font_rasterizer.adjusted_line_height)]
 
     # 字母表
     alphabet = []
 
@@ -60,15 +60,15 @@
         if not c.isprintable():
             continue
 
         # 栅格化
         glyph_data, adjusted_advance_width = font_rasterizer.rasterize_glyph(code_point)
         if glyph_data is None:
             continue
-        logger.info(f'rasterize glyph: {code_point} - {c} - {adjusted_advance_width}')
+        logger.info(f'Rasterize glyph: {code_point} - {c} - {adjusted_advance_width}')
 
         # 合并到图集
         for y in range(font_rasterizer.adjusted_line_height):
             for x in range(adjusted_advance_width):
                 if glyph_data[y][x] > 0:
                     sheet_data[y].append(_glyph_data_solid)
                 else:
@@ -87,15 +87,15 @@
         outputs_name: str,
 ):
     palette = [(255, 255, 255), (0, 0, 0), (255, 0, 255)]
     writer = png.Writer(len(sheet_data[0]), len(sheet_data), palette=palette)
     png_file_path = os.path.join(outputs_dir, f'{outputs_name}.png')
     with open(png_file_path, 'wb') as file:
         writer.write(file, sheet_data)
-    logger.info(f'make {png_file_path}')
+    logger.info(f"Make: '{png_file_path}'")
 
 
 def save_rgba_png(
         sheet_data: list[list[int]],
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
         outputs_name: str,
 ):
@@ -118,19 +118,19 @@
                 rgba_bitmap_row.append(0)
                 rgba_bitmap_row.append(255)
                 rgba_bitmap_row.append(255)
         rgba_bitmap.append(rgba_bitmap_row)
     image = png.from_array(rgba_bitmap, 'RGBA')
     png_file_path = os.path.join(outputs_dir, f'{outputs_name}.png')
     image.save(png_file_path)
-    logger.info(f'make {png_file_path}')
+    logger.info(f"Make: '{png_file_path}'")
 
 
 def save_dat_file(
         alphabet: list[str],
         outputs_dir: str | bytes | os.PathLike[str] | os.PathLike[bytes],
         outputs_name: str,
 ):
     dat_file_path = os.path.join(outputs_dir, f'{outputs_name}.png.dat')
     with open(dat_file_path, 'w', encoding='utf-8') as file:
         file.write(''.join(alphabet))
-    logger.info(f'make {dat_file_path}')
+    logger.info(f"Make: '{dat_file_path}'")
```

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool/bdf.py` & `nico-font-tool-0.0.4/src/nico_font_tool/bdf.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool/font.py` & `nico-font-tool-0.0.4/src/nico_font_tool/font.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool/nicofont.py` & `nico-font-tool-0.0.4/src/nico_font_tool/nicofont.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     glyph_offset_x = args.glyph_offset_x
     glyph_offset_y = args.glyph_offset_y
     glyph_adjust_width = args.glyph_adjust_width
     glyph_adjust_height = args.glyph_adjust_height
     mode = args.mode
 
     if mode != 'palette' and mode != 'rgba':
-        raise Exception(f"unsupported png mode: '{mode}'")
+        raise Exception(f"Unsupported png mode: '{mode}'")
 
     if not os.path.exists(outputs_dir):
         os.makedirs(outputs_dir)
 
     sheet_data, alphabet = nico_font_tool.create_sheet(
         font_file_path,
         font_size,
```

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool/opentype.py` & `nico-font-tool-0.0.4/src/nico_font_tool/opentype.py`

 * *Files identical despite different names*

### Comparing `nico-font-tool-0.0.3/src/nico_font_tool.egg-info/PKG-INFO` & `nico-font-tool-0.0.4/src/nico_font_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nico-font-tool
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for converting fonts to NICO Game Framework format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: source, https://github.com/TakWolf/nico-font-tool.python
 Project-URL: issues, https://github.com/TakWolf/nico-font-tool.python/issues
```


# Comparing `tmp/mb_base-1.0.202305250354-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305260118-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 1827 bytes, number of entries: 7
+Zip file size: 3210 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
+-rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
+-rw-rw-r--  2.0 unx     3343 b- defN 23-May-26 01:17 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-25 03:54 mb_base-1.0.202305250354.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 03:54 mb_base-1.0.202305250354.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-25 03:54 mb_base-1.0.202305250354.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      567 b- defN 23-May-25 03:54 mb_base-1.0.202305250354.dist-info/RECORD
-7 files, 1286 bytes uncompressed, 807 bytes compressed:  37.2%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/RECORD
+9 files, 4830 bytes uncompressed, 1968 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: mb/numpy/__init__.py
 Comment: 
 
 Filename: mb/pandas/__init__.py
 Comment: 
 
+Filename: mb/plt/__init__.py
+Comment: 
+
+Filename: mb/plt/emb_viz.py
+Comment: 
+
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305250354.dist-info/METADATA
+Filename: mb_base-1.0.202305260118.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305250354.dist-info/WHEEL
+Filename: mb_base-1.0.202305260118.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305250354.dist-info/top_level.txt
+Filename: mb_base-1.0.202305260118.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305250354.dist-info/RECORD
+Filename: mb_base-1.0.202305260118.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mb_base-1.0.202305250354.dist-info/RECORD` & `mb_base-1.0.202305260118.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
+mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
+mb/plt/emb_viz.py,sha256=tC41ANXChvGIuxf5AXTobiLm7NIzqltQUR5C5z7uxcQ,3343
 mb/utils/__init__.py,sha256=d-IZbbU-gBC7zOXgiH5SqYVSP6XNaQ8da5153sNLSaY,26
-mb_base-1.0.202305250354.dist-info/METADATA,sha256=OR_DIdwHSQGui8PvqDOqsDRjtQg9BxG1Qm5-kbkobvM,226
-mb_base-1.0.202305250354.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305250354.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305250354.dist-info/RECORD,,
+mb_base-1.0.202305260118.dist-info/METADATA,sha256=xkVeIibG4qDQBBQ5WMTnFSC9EBfZ8bYHuCsnyn2XcHQ,226
+mb_base-1.0.202305260118.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305260118.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305260118.dist-info/RECORD,,
```


# Comparing `tmp/character-encoding-utils-0.0.3.tar.gz` & `tmp/character-encoding-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "character-encoding-utils-0.0.3.tar", last modified: Fri May 19 13:00:43 2023, max compression
+gzip compressed data, was "character-encoding-utils-0.0.4.tar", last modified: Fri May 26 07:20:02 2023, max compression
```

## Comparing `character-encoding-utils-0.0.3.tar` & `character-encoding-utils-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/character_encoding_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/src/character_encoding_utils/shiftjis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 13:00:43.000000 character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 13:00:43.790450 character-encoding-utils-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_big5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_gb2312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_ksx1001.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-19 13:00:31.000000 character-encoding-utils-0.0.3/tests/test_shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.410071 character-encoding-utils-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.414071 character-encoding-utils-0.0.4/src/character_encoding_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/src/character_encoding_utils/shiftjis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.414071 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 07:20:02.000000 character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:20:02.418071 character-encoding-utils-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_big5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_gb2312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_ksx1001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-26 07:19:47.000000 character-encoding-utils-0.0.4/tests/test_shiftjis.py
```

### Comparing `character-encoding-utils-0.0.3/LICENSE` & `character-encoding-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/PKG-INFO` & `character-encoding-utils-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
```

### Comparing `character-encoding-utils-0.0.3/README.md` & `character-encoding-utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/pyproject.toml` & `character-encoding-utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "character-encoding-utils"
-version = "0.0.3"
+version = "0.0.4"
 description = "Some character encoding utils."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils/big5.py` & `character-encoding-utils-0.0.4/src/character_encoding_utils/big5.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 raise Big5DecodeError(bc, passed, e.reason) from e
         passed += len(bc)
     return ''.join(cs)
 
 
 def query_code(c: str) -> int:
     if len(c) != 1:
-        raise Big5Exception('must be one character')
+        raise Big5Exception('Must be one character')
     try:
         bs = encode(c)
     except Big5EncodeError as e:
         raise Big5Exception(f"'{c}' is not a 'big5' character") from e
     if len(bs) == 1:
         raise Big5Exception(f"'{c}' is a ascii character")
     code = int(f'{bs[0]:02x}{bs[1]:02x}', 16)
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils/gb2312.py` & `character-encoding-utils-0.0.4/src/character_encoding_utils/gb2312.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             raise GB2312DecodeError(bc, passed, e.reason) from e
         passed += len(bc)
     return ''.join(cs)
 
 
 def query_coord(c: str) -> tuple[int, int]:
     if len(c) != 1:
-        raise GB2312Exception('must be one character')
+        raise GB2312Exception('Must be one character')
     try:
         bs = encode(c)
     except GB2312EncodeError as e:
         raise GB2312Exception(f"'{c}' is not a 'gb2312' character") from e
     if len(bs) == 1:
         raise GB2312Exception(f"'{c}' is a ascii character")
     row = bs[0] - _euc_offset
@@ -93,15 +93,15 @@
     if 1 <= row <= 9:
         return 'other'
     elif 16 <= row <= 55:
         return 'level-1'
     elif 56 <= row <= 87:
         return 'level-2'
     else:
-        raise None
+        return None
 
 
 def _build_alphabet_by_rows_between(row_start: int, row_end: int) -> list[str]:
     alphabet = []
     for row in range(row_start, row_end + 1):
         for col in range(1, 94 + 1):
             try:
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils/ksx1001.py` & `character-encoding-utils-0.0.4/src/character_encoding_utils/ksx1001.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 raise KSX1001DecodeError(bc, passed, e.reason) from e
         passed += len(bc)
     return ''.join(cs)
 
 
 def query_coord(c: str) -> tuple[int, int]:
     if len(c) != 1:
-        raise KSX1001Exception('must be one character')
+        raise KSX1001Exception('Must be one character')
     try:
         bs = encode(c)
     except KSX1001EncodeError as e:
         raise KSX1001Exception(f"'{c}' is not a 'ksx1001' character") from e
     if len(bs) == 1:
         raise KSX1001Exception(f"'{c}' is a ascii character")
     elif bs.startswith(b'\xa4\xd4') and len(bs) > 2:
@@ -109,15 +109,15 @@
     if 1 <= row <= 12:
         return 'other'
     elif 16 <= row <= 40:
         return 'syllable'
     elif 42 <= row <= 93:
         return 'hanja'
     else:
-        raise None
+        return None
 
 
 def _build_alphabet_by_rows_between(row_start: int, row_end: int) -> list[str]:
     alphabet = []
     for row in range(row_start, row_end + 1):
         for col in range(1, 94 + 1):
             try:
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils/shiftjis.py` & `character-encoding-utils-0.0.4/src/character_encoding_utils/shiftjis.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,23 +87,23 @@
         if 0x00 <= first_byte <= 0x1F or first_byte == 0x7F:
             return 'single-byte-ascii-control'
         elif 0x20 <= first_byte <= 0x7E:
             return 'single-byte-ascii-printable'
         elif 0xA1 <= first_byte <= 0xDF:
             return 'single-byte-half-width-katakana'
         else:
-            raise None
+            return None
     else:
         second_byte = bs[1]
         if 0x81 <= first_byte <= 0x87 or (first_byte == 0x88 and second_byte <= 0x9E):
             return 'double-byte-other'
         elif (first_byte == 0x88 and second_byte >= 0x9F) or 0x89 <= first_byte <= 0x9F or 0xE0 <= first_byte <= 0xEF:
             return 'double-byte-kanji'
         else:
-            raise None
+            return None
 
 
 def _build_alphabet_single_byte(byte_start: int, byte_end: int) -> list[str]:
     alphabet = []
     for code in range(byte_start, byte_end + 1):
         try:
             c = decode(bytes([code]))
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/PKG-INFO` & `character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: character-encoding-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Some character encoding utils.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/character-encoding-utils
 Project-URL: source, https://github.com/TakWolf/character-encoding-utils
 Project-URL: issues, https://github.com/TakWolf/character-encoding-utils/issues
```

### Comparing `character-encoding-utils-0.0.3/src/character_encoding_utils.egg-info/SOURCES.txt` & `character-encoding-utils-0.0.4/src/character_encoding_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/tests/test_big5.py` & `character-encoding-utils-0.0.4/tests/test_big5.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/tests/test_gb2312.py` & `character-encoding-utils-0.0.4/tests/test_gb2312.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/tests/test_ksx1001.py` & `character-encoding-utils-0.0.4/tests/test_ksx1001.py`

 * *Files identical despite different names*

### Comparing `character-encoding-utils-0.0.3/tests/test_shiftjis.py` & `character-encoding-utils-0.0.4/tests/test_shiftjis.py`

 * *Files identical despite different names*


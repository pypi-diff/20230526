# Comparing `tmp/pyemerald-0.3.2.tar.gz` & `tmp/pyemerald-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyemerald-0.3.2.tar", max compression
+gzip compressed data, was "pyemerald-0.4.0.tar", max compression
```

## Comparing `pyemerald-0.3.2.tar` & `pyemerald-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0     3316 2023-05-24 15:13:40.755134 pyemerald-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.3.2/pyemerald/__init__.py
--rw-r--r--   0        0        0    12171 2023-05-23 13:28:34.597606 pyemerald-0.3.2/pyemerald/codec.py
--rw-r--r--   0        0        0      641 2023-05-23 13:28:34.597606 pyemerald-0.3.2/pyemerald/constants.py
--rw-r--r--   0        0        0     1656 2023-05-23 13:28:34.597606 pyemerald-0.3.2/pyemerald/game.py
--rw-r--r--   0        0        0     9027 2023-05-23 13:28:34.597606 pyemerald-0.3.2/pyemerald/items.py
--rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/moves.py
--rw-r--r--   0        0        0    18971 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/pokemon.py
--rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/raw_section.py
--rw-r--r--   0        0        0     6323 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/save.py
--rw-r--r--   0        0        0     7157 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/section.py
--rw-r--r--   0        0        0     1288 2023-05-23 13:28:34.600939 pyemerald-0.3.2/pyemerald/utils.py
--rw-r--r--   0        0        0      449 2023-05-24 15:44:56.690400 pyemerald-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4014 2023-05-24 15:45:27.270445 pyemerald-0.3.2/setup.py
--rw-r--r--   0        0        0     3939 2023-05-24 15:45:27.270861 pyemerald-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-05-24 15:11:53.898358 pyemerald-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     1928 2023-05-26 09:18:23.811297 pyemerald-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 11:52:31.804082 pyemerald-0.4.0/pyemerald/__init__.py
+-rw-r--r--   0        0        0    12667 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/codec.py
+-rw-r--r--   0        0        0      641 2023-05-23 13:28:34.597606 pyemerald-0.4.0/pyemerald/constants.py
+-rw-r--r--   0        0        0     1656 2023-05-23 13:28:34.597606 pyemerald-0.4.0/pyemerald/game.py
+-rw-r--r--   0        0        0     9108 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/items.py
+-rw-r--r--   0        0        0     1922 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/level.py
+-rw-r--r--   0        0        0    60162 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/moves.py
+-rw-r--r--   0        0        0     3843 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/nature_stats.py
+-rw-r--r--   0        0        0    34516 2023-05-26 09:18:23.811297 pyemerald-0.4.0/pyemerald/pokemon.py
+-rw-r--r--   0        0        0    97687 2023-05-26 09:18:23.814630 pyemerald-0.4.0/pyemerald/pokemon_info.py
+-rw-r--r--   0        0        0     4510 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/raw_section.py
+-rw-r--r--   0        0        0     6323 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/save.py
+-rw-r--r--   0        0        0     7157 2023-05-23 13:28:34.600939 pyemerald-0.4.0/pyemerald/section.py
+-rw-r--r--   0        0        0     2497 2023-05-25 18:51:11.499441 pyemerald-0.4.0/pyemerald/utils.py
+-rw-r--r--   0        0        0      531 2023-05-26 09:21:29.622887 pyemerald-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2568 2023-05-26 09:23:12.700552 pyemerald-0.4.0/setup.py
+-rw-r--r--   0        0        0     2551 2023-05-26 09:23:12.700879 pyemerald-0.4.0/PKG-INFO
```

### Comparing `pyemerald-0.3.2/LICENSE.txt` & `pyemerald-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/codec.py` & `pyemerald-0.4.0/pyemerald/codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -226,25 +226,31 @@
         name: str,
         data_type: Union[str, int, bytes],
         offset: int,
         size: int,
         value_map: Optional[Dict[int, str]] = None,
         reverse_value_map: Optional[Dict[int, str]] = None,
         deserialize_skip: bool = False,
+        serialize_skip: bool = False,
     ):
         """deserialize_skip if this is True when creating object from bytes it will
         just set the raw bytes on the given attribute. If False (which is default)
-        it will deserialize as specified"""
+        it will deserialize as specified.
+
+        serialize_skip will set the given field will be filled with
+        0xFF.
+        """
         self.name = name
         self.data_type = data_type
         self.offset = offset
         self.size = size
         self.value_map = value_map
         self.reverse_value_map = reverse_value_map
         self.deserialize_skip = deserialize_skip
+        self.serialize_skip = serialize_skip
 
         if (self.value_map is not None and self.reverse_value_map is None) or (
             self.value_map is None and self.reverse_value_map is not None
         ):
             raise ValueError(
                 "Both value_map and reverse_value_map must be set on ByteFieldCode"
             )
@@ -273,14 +279,19 @@
             if self.value_map is not None:
                 return self.value_map[value]
             else:
                 return value
 
     def to_bytes(self, value: Union[str, int]) -> bytes:
         """Convert a value to bytes"""
+        if self.serialize_skip:
+
+            # Fill with 0xFF
+            value = int_to_bytes(256**self.size - 1, self.size)
+            return value
         if self.value_map is not None:
             value = self.reverse_value_map[value]
 
         if self.data_type is int:
             return int_to_bytes(value, self.size)
         elif self.data_type is str:
             raw_bytes = str_to_bytes(value)
@@ -294,14 +305,17 @@
             # Assumes data has been converted into bytes already!
             if isinstance(value, bytes):
                 return value
             else:
                 raise ValueError(
                     "Can't turn list into bytes! Please convert value to bytes manually!"
                 )
+        elif isinstance(self.data_type, type(Serializable)):
+            # Let the object serialize itself to bytes
+            return value.to_bytes()
         else:
             raise ValueError(f"Type {self.data_type} is not supported!")
 
     def add_offset(self, offset):
         self.offset += offset
 
     def __repr__(self) -> str:
@@ -344,29 +358,29 @@
 
         return res
 
     def to_object(self, data: bytes) -> "Object":
         """Create instance of a object based on the bytes data"""
         values = self.to_values(data)
         object_class = self.object_class
+        obj = object_class(**values)
 
-        return object_class(**values)
+        return obj
 
     def to_bytes(self, _object: object) -> bytes:
         """Take an object and serialize it using the codec.
         It has to have attribute values corresponding to
         ByteFieldCodec values"""
 
         # Order by offset
         sorted_fields = sorted(self.fields, key=lambda x: x.offset)
 
         buffer = bytearray()
 
         for field in sorted_fields:
-
             # Pad buffer up to the current offset
             buffer = buffer.ljust(field.offset, b"\x00")
 
             # Get value from _object
             value = getattr(_object, field.name)
             field_bytes = field.to_bytes(value)
```

### Comparing `pyemerald-0.3.2/pyemerald/constants.py` & `pyemerald-0.4.0/pyemerald/constants.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/game.py` & `pyemerald-0.4.0/pyemerald/game.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/items.py` & `pyemerald-0.4.0/pyemerald/items.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     quantity: int
     _codec: ClassVar[Codec] = ItemCodec
 
     @classmethod
     def from_number(cls, item_number: int, quantity: int):
         cls(ITEM_INDEX_TO_NAME[item_number], quantity)
 
+    @property
+    def index(self):
+        return ITEM_NAME_TO_INDEX[self.name]
+
 
 ITEM_INDEX_TO_NAME = {
     0: "Nothing",
     1: "Master Ball",
     2: "Ultra Ball",
     3: "Great Ball",
     4: "Poké Ball",
```

### Comparing `pyemerald-0.3.2/pyemerald/moves.py` & `pyemerald-0.4.0/pyemerald/moves.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/raw_section.py` & `pyemerald-0.4.0/pyemerald/raw_section.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/save.py` & `pyemerald-0.4.0/pyemerald/save.py`

 * *Files identical despite different names*

### Comparing `pyemerald-0.3.2/pyemerald/section.py` & `pyemerald-0.4.0/pyemerald/section.py`

 * *Files identical despite different names*


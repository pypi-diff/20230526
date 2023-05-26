# Comparing `tmp/pyquet-0.0.3.tar.gz` & `tmp/pyquet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquet-0.0.3.tar", last modified: Fri May 26 18:42:31 2023, max compression
+gzip compressed data, was "pyquet-0.0.4.tar", last modified: Fri May 26 19:39:34 2023, max compression
```

## Comparing `pyquet-0.0.3.tar` & `pyquet-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:42:31.288602 pyquet-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      546 2023-05-26 18:42:31.288602 pyquet-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-05-06 12:45:59.000000 pyquet-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      674 2023-05-26 18:42:31.289607 pyquet-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 18:42:31.269222 pyquet-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 18:42:31.275210 pyquet-0.0.3/src/pyquet/
--rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.0.3/src/pyquet/__init__.py
--rw-rw-rw-   0        0        0      628 2023-05-26 11:30:34.000000 pyquet-0.0.3/src/pyquet/common.py
--rw-rw-rw-   0        0        0     5208 2023-05-26 18:31:15.000000 pyquet-0.0.3/src/pyquet/generator.py
--rw-rw-rw-   0        0        0     2132 2023-05-26 18:31:16.000000 pyquet-0.0.3/src/pyquet/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:42:31.287588 pyquet-0.0.3/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-05-26 18:42:31.000000 pyquet-0.0.3/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-26 18:42:31.000000 pyquet-0.0.3/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:42:31.000000 pyquet-0.0.3/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-26 18:42:31.000000 pyquet-0.0.3/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 18:42:31.000000 pyquet-0.0.3/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 18:42:31.287588 pyquet-0.0.3/tests/
--rw-rw-rw-   0        0        0     2078 2023-05-26 18:31:16.000000 pyquet-0.0.3/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:39:34.723407 pyquet-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-05-26 19:39:34.724407 pyquet-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-06 12:45:59.000000 pyquet-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      674 2023-05-26 19:39:34.725405 pyquet-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 19:39:34.605690 pyquet-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 19:39:34.704942 pyquet-0.0.4/src/pyquet/
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.0.4/src/pyquet/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-05-26 11:30:34.000000 pyquet-0.0.4/src/pyquet/common.py
+-rw-rw-rw-   0        0        0     5712 2023-05-26 19:38:57.000000 pyquet-0.0.4/src/pyquet/generator.py
+-rw-rw-rw-   0        0        0     2132 2023-05-26 18:31:16.000000 pyquet-0.0.4/src/pyquet/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:39:34.721899 pyquet-0.0.4/src/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-05-26 19:39:34.000000 pyquet-0.0.4/src/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-26 19:39:34.000000 pyquet-0.0.4/src/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 19:39:34.000000 pyquet-0.0.4/src/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-26 19:39:34.000000 pyquet-0.0.4/src/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 19:39:34.000000 pyquet-0.0.4/src/pyquet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 19:39:34.721899 pyquet-0.0.4/tests/
+-rw-rw-rw-   0        0        0     2078 2023-05-26 18:31:16.000000 pyquet-0.0.4/tests/test_reader.py
```

### Comparing `pyquet-0.0.3/LICENSE` & `pyquet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.0.3/PKG-INFO` & `pyquet-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.0.3/setup.cfg` & `pyquet-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e30 2e33 0d0a 6175 7468  on = 0.0.3..auth
+00000020: 6f6e 203d 2030 2e30 2e34 0d0a 6175 7468  on = 0.0.4..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `pyquet-0.0.3/src/pyquet/common.py` & `pyquet-0.0.4/src/pyquet/common.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.0.3/src/pyquet/generator.py` & `pyquet-0.0.4/src/pyquet/generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,118 +7,113 @@
 import pandas as pd
 from src.pyquet import common
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 
-def generate_test_table(schema, catalog_path):
-    catalog = common.read_json(catalog_path)
-    min_rows = len(max(catalog.values(), key=lambda x: len(x)))
-    data = {}
-    field_format = []
-    for field in schema["fields"]:
-        name = field["name"]
-        data_type = field["logicalFormat"]
-        if data_type.startswith("ALPHANUMERIC"):
-            match = re.match(r'ALPHANUMERIC\(([0-9]*)\)', data_type)
-            string_len = match.group(1)
-            data[name] = generate_alphanumeric(min_rows, int(string_len))
-            field_format.append((field["name"], pa.string()))
-        elif data_type.startswith("NUMERIC SHORT"):
-            data[name] = generate_int(min_rows)
-            field_format.append((field["name"], pa.int64()))
-        elif data_type.startswith("DECIMAL"):
-            match = re.match(r'DECIMAL\(([0-9]*),?([0-9]*)\)', data_type)
-            decimal_precision = int(match.group(1))
-            decimal_scale = match.group(2)
-            decimal_scale = int(decimal_scale) if decimal_scale != "" else 0
-            data[name] = generate_decimal(min_rows, decimal_precision, decimal_scale)
-            field_format.append((field["name"], pa.decimal128(decimal_precision, decimal_scale)))
-        elif data_type.startswith("DATE"):
-            data[name] = generate_date(min_rows)
-            field_format.append((field["name"], pa.date32()))
-        elif data_type.startswith("TIMESTAMP"):
-            data[name] = generate_timestamp(min_rows)
-            field_format.append((field["name"], pa.timestamp("ms")))
-        elif data_type.startswith("TIME"):
-            data[name] = generate_time(min_rows)
-            field_format.append((field["name"], pa.time32("ms")))
-        else:
-            print("Unrecognized logicalFormat:", data_type)
-
-    write_parquet_table(data, schema["physicalPath"], pa.schema(field_format))
-
-
-def generate_alphanumeric(num_rows, size=1):
-    alphanumeric_list = []
-    for _ in range(num_rows):
-        value = "".join(random.choices(string.ascii_letters + string.digits, k=size))
-        alphanumeric_list.append(value)
-    return alphanumeric_list
-
-
-def generate_int(num_rows, size=1000):
-    int_list = []
-    for _ in range(num_rows):
-        value = random.randint(0, size)
-        int_list.append(value)
-    return int_list
-
-
-def generate_decimal(num_rows, decimal_precision=12, decimal_scale=6):
-    decimal_list = []
-    for _ in range(num_rows):
-        value = Decimal(random.randrange(10 ** decimal_precision)) / (10 ** decimal_scale)
-        decimal_list.append(value)
-    return decimal_list
-
-
-def generate_date(num_rows, date_format='%Y-%m-%d'):
-    date_list = []
-    for _ in range(num_rows):
-        date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
-                                            hours=random.randint(0, 24),
-                                            minutes=random.randint(0, 60),
-                                            seconds=random.randint(0, 60))
-        date_list.append(str(date.strftime(date_format)))
-    date_list = pd.Series(date_list).apply(lambda x: datetime.strptime(x, date_format))
-    return date_list
-
-
-def generate_timestamp(num_rows, date_format='%Y-%m-%d %H:%M:%S'):
-    timestamp_list = []
-    for _ in range(num_rows):
-        date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
-                                            hours=random.randint(0, 24),
-                                            minutes=random.randint(0, 60),
-                                            seconds=random.randint(0, 60))
-        timestamp_list.append(str(date.strftime(date_format)))
-    timestamp_list = pd.Series(timestamp_list).apply(lambda x: datetime.strptime(x, date_format))
-    return timestamp_list
-
-
-def generate_time(num_rows, date_format='%H:%M:%S'):
-    time_list = []
-    for _ in range(num_rows):
-        date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
-                                            hours=random.randint(0, 24),
-                                            minutes=random.randint(0, 60),
-                                            seconds=random.randint(0, 60))
-        time_list.append(str(date.strftime(date_format)))
-    time_list = pd.Series(time_list).apply(lambda x: datetime.strptime(x, date_format))
-    return time_list
-
-
-def write_parquet_table(data, path, schema, destination_dir="."):
-    destination_path = os.path.join(destination_dir, path)
-    destination_dir = os.path.dirname(destination_path)
-    if not os.path.isdir(destination_dir):
-        os.makedirs(destination_dir)
-    if os.path.isfile(destination_path):
-        os.remove(destination_path)
-    df = pd.DataFrame(data)
-    table = pa.Table.from_pandas(df)
-    target_schema = pa.schema(schema)
-    table = table.cast(target_schema)
-    pq.write_table(table, destination_path)
-
+class DataGenerator:
+    def __init__(self, catalog_path):
+        self.catalog = common.read_json(catalog_path)
+        self.min_rows = len(max(self.catalog.values(), key=lambda x: len(x)))
+
+    def generate_data(self, schema_path, destination_dir="."):
+        data = {}
+        field_format = []
+        schema = common.read_json(schema_path)
+        schema_physical_path = os.path.normpath(schema["physicalPath"])
+        for field in schema["fields"]:
+            name = field["name"]
+            data_type = field["logicalFormat"]
+            if data_type.startswith("ALPHANUMERIC"):
+                match = re.match(r'ALPHANUMERIC\(([0-9]*)\)', data_type)
+                string_len = match.group(1)
+                data[name] = self.generate_alphanumeric(int(string_len))
+                field_format.append((field["name"], pa.string()))
+            elif data_type.startswith("NUMERIC SHORT"):
+                data[name] = self.generate_int()
+                field_format.append((field["name"], pa.int64()))
+            elif data_type.startswith("DECIMAL"):
+                match = re.match(r'DECIMAL\(([0-9]*),?([0-9]*)\)', data_type)
+                decimal_precision = int(match.group(1))
+                decimal_scale = match.group(2)
+                decimal_scale = int(decimal_scale) if decimal_scale != "" else 0
+                data[name] = self.generate_decimal(decimal_precision, decimal_scale)
+                field_format.append((field["name"], pa.decimal128(decimal_precision, decimal_scale)))
+            elif data_type.startswith("DATE"):
+                data[name] = self.generate_date()
+                field_format.append((field["name"], pa.date32()))
+            elif data_type.startswith("TIMESTAMP"):
+                data[name] = self.generate_timestamp()
+                field_format.append((field["name"], pa.timestamp("ms")))
+            elif data_type.startswith("TIME"):
+                data[name] = self.generate_time()
+                field_format.append((field["name"], pa.time32("ms")))
+            else:
+                print("Unrecognized logicalFormat:", data_type)
+
+        destination_path = os.path.abspath(destination_dir + "/" + schema_physical_path)
+        destination_path_dir = os.path.dirname(destination_path)
+        if not os.path.isdir(destination_path_dir):
+            os.makedirs(destination_path_dir)
+        if os.path.isfile(destination_path):
+            os.remove(destination_path)
+        df = pd.DataFrame(data)
+        table = pa.Table.from_pandas(df)
+        target_schema = pa.schema(pa.schema(field_format))
+        table = table.cast(target_schema)
+        pq.write_table(table, destination_path)
+        print("Wrote: ", destination_path)
+
+    def generate_alphanumeric(self, size=1):
+        alphanumeric_list = []
+        for _ in range(self.min_rows):
+            value = "".join(random.choices(string.ascii_letters + string.digits, k=size))
+            alphanumeric_list.append(value)
+        return alphanumeric_list
+
+    def generate_int(self, size=1000):
+        int_list = []
+        for _ in range(self.min_rows):
+            value = random.randint(0, size)
+            int_list.append(value)
+        return int_list
+
+    def generate_decimal(self, decimal_precision=12, decimal_scale=6):
+        decimal_list = []
+        for _ in range(self.min_rows):
+            value = Decimal(random.randrange(10 ** decimal_precision)) / (10 ** decimal_scale)
+            decimal_list.append(value)
+        return decimal_list
+
+    def generate_date(self, date_format='%Y-%m-%d'):
+        date_list = []
+        for _ in range(self.min_rows):
+            date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
+                                                hours=random.randint(0, 24),
+                                                minutes=random.randint(0, 60),
+                                                seconds=random.randint(0, 60))
+            date_list.append(str(date.strftime(date_format)))
+        date_list = pd.Series(date_list).apply(lambda x: datetime.strptime(x, date_format))
+        return date_list
+
+    def generate_timestamp(self, date_format='%Y-%m-%d %H:%M:%S'):
+        timestamp_list = []
+        for _ in range(self.min_rows):
+            date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
+                                                hours=random.randint(0, 24),
+                                                minutes=random.randint(0, 60),
+                                                seconds=random.randint(0, 60))
+            timestamp_list.append(str(date.strftime(date_format)))
+        timestamp_list = pd.Series(timestamp_list).apply(lambda x: datetime.strptime(x, date_format))
+        return timestamp_list
+
+    def generate_time(self, date_format='%H:%M:%S'):
+        time_list = []
+        for _ in range(self.min_rows):
+            date = datetime.today() - timedelta(days=random.randint(0, 365 * 5),
+                                                hours=random.randint(0, 24),
+                                                minutes=random.randint(0, 60),
+                                                seconds=random.randint(0, 60))
+            time_list.append(str(date.strftime(date_format)))
+        time_list = pd.Series(time_list).apply(lambda x: datetime.strptime(x, date_format))
+        return time_list
```

### Comparing `pyquet-0.0.3/src/pyquet/schemas.py` & `pyquet-0.0.4/src/pyquet/schemas.py`

 * *Files identical despite different names*

### Comparing `pyquet-0.0.3/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.0.4/src/pyquet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.0.3/tests/test_reader.py` & `pyquet-0.0.4/tests/test_reader.py`

 * *Files identical despite different names*


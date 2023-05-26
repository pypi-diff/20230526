# Comparing `tmp/slot_machine_serializers-0.3.0.tar.gz` & `tmp/slot_machine_serializers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slot_machine_serializers-0.3.0.tar", last modified: Wed Apr 26 12:07:26 2023, max compression
+gzip compressed data, was "slot_machine_serializers-0.4.0.tar", last modified: Fri May 26 14:19:40 2023, max compression
```

## Comparing `slot_machine_serializers-0.3.0.tar` & `slot_machine_serializers-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.361143 slot_machine_serializers-0.3.0/
--rw-r--r--   0 ochsner    (502) staff       (20)     1912 2023-04-26 12:07:26.361224 slot_machine_serializers-0.3.0/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)     1654 2023-04-26 11:52:54.000000 slot_machine_serializers-0.3.0/README.md
--rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.3.0/pyproject.toml
--rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-26 12:07:26.361548 slot_machine_serializers-0.3.0/setup.cfg
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.359373 slot_machine_serializers-0.3.0/slot_machine/
--rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.3.0/slot_machine/__init__.py
--rw-r--r--   0 ochsner    (502) staff       (20)     3167 2023-04-26 12:04:52.000000 slot_machine_serializers-0.3.0/slot_machine/samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     4085 2023-04-26 11:53:00.000000 slot_machine_serializers-0.3.0/slot_machine/serializers.py
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.360335 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/
--rw-r--r--   0 ochsner    (502) staff       (20)     1912 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/SOURCES.txt
--rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/dependency_links.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/requires.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-26 12:07:26.000000 slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/top_level.txt
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-26 12:07:26.360831 slot_machine_serializers-0.3.0/tests/
--rw-r--r--   0 ochsner    (502) staff       (20)     1869 2023-04-26 12:03:58.000000 slot_machine_serializers-0.3.0/tests/test_samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.3.0/tests/test_serializers.py
+drwxr-xr-x   0 TheUser    (501) staff       (20)        0 2023-05-26 14:19:40.046167 slot_machine_serializers-0.4.0/
+-rw-r--r--   0 TheUser    (501) staff       (20)     1911 2023-05-26 14:19:40.046339 slot_machine_serializers-0.4.0/PKG-INFO
+-rw-r--r--   0 TheUser    (501) staff       (20)     1653 2023-05-26 13:53:15.000000 slot_machine_serializers-0.4.0/README.md
+-rw-r--r--   0 TheUser    (501) staff       (20)       90 2023-05-26 13:53:15.000000 slot_machine_serializers-0.4.0/pyproject.toml
+-rw-r--r--   0 TheUser    (501) staff       (20)      595 2023-05-26 14:19:40.047084 slot_machine_serializers-0.4.0/setup.cfg
+drwxr-xr-x   0 TheUser    (501) staff       (20)        0 2023-05-26 14:19:40.042723 slot_machine_serializers-0.4.0/slot_machine/
+-rw-r--r--   0 TheUser    (501) staff       (20)       51 2023-05-26 13:53:15.000000 slot_machine_serializers-0.4.0/slot_machine/__init__.py
+-rw-r--r--   0 TheUser    (501) staff       (20)     3167 2023-05-26 13:53:15.000000 slot_machine_serializers-0.4.0/slot_machine/samplers.py
+-rw-r--r--   0 TheUser    (501) staff       (20)     4377 2023-05-26 14:00:13.000000 slot_machine_serializers-0.4.0/slot_machine/serializers.py
+drwxr-xr-x   0 TheUser    (501) staff       (20)        0 2023-05-26 14:19:40.044771 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/
+-rw-r--r--   0 TheUser    (501) staff       (20)     1911 2023-05-26 14:19:40.000000 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/PKG-INFO
+-rw-r--r--   0 TheUser    (501) staff       (20)      400 2023-05-26 14:19:40.000000 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/SOURCES.txt
+-rw-r--r--   0 TheUser    (501) staff       (20)        1 2023-05-26 14:19:40.000000 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/dependency_links.txt
+-rw-r--r--   0 TheUser    (501) staff       (20)       49 2023-05-26 14:19:40.000000 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/requires.txt
+-rw-r--r--   0 TheUser    (501) staff       (20)       13 2023-05-26 14:19:40.000000 slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/top_level.txt
+drwxr-xr-x   0 TheUser    (501) staff       (20)        0 2023-05-26 14:19:40.045832 slot_machine_serializers-0.4.0/tests/
+-rw-r--r--   0 TheUser    (501) staff       (20)     1869 2023-05-26 13:53:15.000000 slot_machine_serializers-0.4.0/tests/test_samplers.py
+-rw-r--r--   0 TheUser    (501) staff       (20)     3196 2023-05-26 14:03:06.000000 slot_machine_serializers-0.4.0/tests/test_serializers.py
```

### Comparing `slot_machine_serializers-0.3.0/PKG-INFO` & `slot_machine_serializers-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot_machine_serializers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -29,15 +29,15 @@
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
 chicken_nuggets: !SampleRange 5..20
-price: !SampleUniform 9..99..20
+price: !SampleUniform 9.99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
```

### Comparing `slot_machine_serializers-0.3.0/README.md` & `slot_machine_serializers-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
 chicken_nuggets: !SampleRange 5..20
-price: !SampleUniform 9..99..20
+price: !SampleUniform 9.99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
```

### Comparing `slot_machine_serializers-0.3.0/setup.cfg` & `slot_machine_serializers-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slot_machine_serializers
-version = 0.3.0
+version = 0.4.0
 description = Ordered dataclass serializer mixin for sloted dataclasses
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 url = https://github.com/sirno/slot_machine
 license = MIT
 python_requires = ">=3.10"
```

### Comparing `slot_machine_serializers-0.3.0/slot_machine/samplers.py` & `slot_machine_serializers-0.4.0/slot_machine/samplers.py`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.3.0/slot_machine/serializers.py` & `slot_machine_serializers-0.4.0/slot_machine/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,22 @@
     @classmethod
     def from_yaml_file(cls, path) -> Self:
         """Read from yaml file."""
         with open(path, "r") as f:
             return cls.from_yaml(f.read())
 
     @classmethod
+    def from_yaml_file_stream(cls, path) -> list[Self]:
+        """Read from yaml file stream."""
+        with open(path, "r") as f:
+            content = f.read()
+            stream = content.split("---")
+            return [cls.from_yaml(yaml) for yaml in stream if yaml]
+
+    @classmethod
     def show_tag(cls, subclass) -> Self:
         """Decorator to show tag in yaml output."""
         subclass._show_tag = True
         return subclass
 
 
 def _try_issubclass(cls, classinfo):
```

### Comparing `slot_machine_serializers-0.3.0/slot_machine_serializers.egg-info/PKG-INFO` & `slot_machine_serializers-0.4.0/slot_machine_serializers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot-machine-serializers
-Version: 0.3.0
+Version: 0.4.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -29,15 +29,15 @@
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
 chicken_nuggets: !SampleRange 5..20
-price: !SampleUniform 9..99..20
+price: !SampleUniform 9.99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
```

### Comparing `slot_machine_serializers-0.3.0/tests/test_samplers.py` & `slot_machine_serializers-0.4.0/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.3.0/tests/test_serializers.py` & `slot_machine_serializers-0.4.0/tests/test_serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,32 @@
     """Test `from_yaml` method for simple class."""
     params = Parameters.from_yaml(SIMPLE_YAML)
     assert params.a == 2
     assert params.b == 0.0
     assert params.c == "abc"
 
 
+def test_simple_from_yaml_file():
+    """Test `from_yaml_file` method for simple class."""
+    params = Parameters.from_yaml_file("tests/data/parameters.yaml")
+    assert params.a == 2
+    assert params.b == 0.0
+    assert params.c == "abc"
+
+def test_simple_from_yaml_file_stream():
+    """Test `from_yaml_file_stream` method for simple class."""
+    params_list = Parameters.from_yaml_file_stream("tests/data/parameters_stream.yaml")
+    assert len(params_list) == 2
+    assert params_list[0].a == 2
+    assert params_list[0].b == 0.0
+    assert params_list[0].c == "abc"
+    assert params_list[1].a == 3
+    assert params_list[1].b == 1.0
+    assert params_list[1].c == "def"
+
 @dataclass(slots=True)
 class Inner(SlotsSerializer):
     value: int
 
 
 @dataclass(slots=True)
 class Outer(SlotsSerializer):
```


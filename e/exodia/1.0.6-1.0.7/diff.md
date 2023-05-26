# Comparing `tmp/exodia-1.0.6.tar.gz` & `tmp/exodia-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exodia-1.0.6.tar", last modified: Thu May 25 16:25:18 2023, max compression
+gzip compressed data, was "exodia-1.0.7.tar", last modified: Fri May 26 09:00:30 2023, max compression
```

## Comparing `exodia-1.0.6.tar` & `exodia-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 16:25:18.789851 exodia-1.0.6/
--rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.6/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 16:25:18.789734 exodia-1.0.6/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     5743 2023-05-25 15:19:46.000000 exodia-1.0.6/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 16:25:18.788787 exodia-1.0.6/exodia/
--rw-r--r--   0 leondaz    (501) staff       (20)      396 2023-05-25 16:23:53.000000 exodia-1.0.6/exodia/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1632 2023-05-25 16:23:46.000000 exodia-1.0.6/exodia/bases.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1034 2023-05-25 16:24:35.000000 exodia-1.0.6/exodia/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     6933 2023-05-25 16:23:46.000000 exodia-1.0.6/exodia/fields.py
--rw-r--r--   0 leondaz    (501) staff       (20)      185 2023-05-25 16:24:04.000000 exodia-1.0.6/exodia/utils.py
--rw-r--r--   0 leondaz    (501) staff       (20)    10516 2023-05-25 16:23:53.000000 exodia-1.0.6/exodia/validators.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 16:25:18.789241 exodia-1.0.6/exodia.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 16:25:18.000000 exodia-1.0.6/exodia.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-25 16:25:18.000000 exodia-1.0.6/exodia.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-25 16:25:18.000000 exodia-1.0.6/exodia.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-25 16:25:18.000000 exodia-1.0.6/exodia.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-25 16:25:18.789890 exodia-1.0.6/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-25 16:25:02.000000 exodia-1.0.6/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 16:25:18.789559 exodia-1.0.6/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)     1289 2023-05-25 16:23:46.000000 exodia-1.0.6/tests/test_instance_creation.py
--rw-r--r--   0 leondaz    (501) staff       (20)     3556 2023-05-25 15:32:13.000000 exodia-1.0.6/tests/test_validation.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-26 09:00:30.115841 exodia-1.0.7/
+-rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.7/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-26 09:00:30.115724 exodia-1.0.7/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     5762 2023-05-25 16:26:25.000000 exodia-1.0.7/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-26 09:00:30.114574 exodia-1.0.7/exodia/
+-rw-r--r--   0 leondaz    (501) staff       (20)      453 2023-05-26 09:00:22.000000 exodia-1.0.7/exodia/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2133 2023-05-26 07:38:23.000000 exodia-1.0.7/exodia/bases.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1034 2023-05-25 16:24:35.000000 exodia-1.0.7/exodia/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     7261 2023-05-26 08:54:19.000000 exodia-1.0.7/exodia/fields.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-26 07:13:50.000000 exodia-1.0.7/exodia/utils.py
+-rw-r--r--   0 leondaz    (501) staff       (20)    11286 2023-05-26 09:00:22.000000 exodia-1.0.7/exodia/validators.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-26 09:00:30.115008 exodia-1.0.7/exodia.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-26 09:00:30.000000 exodia-1.0.7/exodia.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-26 09:00:30.000000 exodia-1.0.7/exodia.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-26 09:00:30.000000 exodia-1.0.7/exodia.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-26 09:00:30.000000 exodia-1.0.7/exodia.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-26 09:00:30.115884 exodia-1.0.7/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-26 09:00:06.000000 exodia-1.0.7/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-26 09:00:30.115560 exodia-1.0.7/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1289 2023-05-25 16:23:46.000000 exodia-1.0.7/tests/test_instance_creation.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     3935 2023-05-26 09:00:22.000000 exodia-1.0.7/tests/test_validation.py
```

### Comparing `exodia-1.0.6/LICENSE` & `exodia-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exodia-1.0.6/README.md` & `exodia-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,23 @@
 
 Exodia supports date/time/datetime objects as well with operators working as expected
 
 ```python
 from datetime import datetime, date
 import exodia as ex
 
-ex.Date().before(date(year=3000, month=1, day=1)).validate(date(year=1971, month=1, day=1).isoformat())  # works
-ex.DateTime().validate(datetime(year=1971, month=1, day=1, hour=1, minute=1, second=1).isoformat())  # works
+ex.Date().before(
+    date(year=3000, month=1, day=1)
+).validate(
+    date(year=1971, month=1, day=1).isoformat()
+)  # works
+
+ex.DateTime().validate(
+    datetime(year=1971, month=1, day=1, hour=1, minute=1, second=1).isoformat()
+)  # works
 ```
 
 ### What if you have dependant fields?
 
 ```python
 import exodia as ex
```

### Comparing `exodia-1.0.6/exodia/bases.py` & `exodia-1.0.7/exodia/bases.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,43 +18,57 @@
             if isinstance(value, ex.Field):
                 result[key] = value
 
         return result
 
     def _validate_kwargs(self, kwargs):
         errors = []
+
         unknown_attrs = []
         valid_fields = self._get_valid_fields()
         valid_attrs = {key: kwargs.get(key) for key in valid_fields.keys()}
 
         for key, value in kwargs.items():
             if not valid_fields.get(key):
                 unknown_attrs.append(key)
 
         for attr in unknown_attrs:
             error = ex.ExodiaException("unexpected attribute {attr}".format(attr=attr))
             errors.append(error)
 
         for key, field in valid_fields.items():
             value = valid_attrs.get(key)
+
             try:
-                field._run_validators(value, key, self)
+                self.validate_field(field, key, value)
             except ex.ExodiaException as e:
                 errors += [e]
 
-            self.post_field_validation(key, value)
+            setattr(self, key, value)
 
         try:
             self.validate(valid_attrs)
         except AssertionError as e:
             errors.append(ex.ExodiaException(*e.args))
         except ex.ExodiaException as e:
             errors.append(e)
 
         if errors:
             raise ex.ExodiaException(errors)
 
-    def validate(self, attrs):
-        pass
+    def validate_field(self, field, field_name, value):
+        """
+        This is the initial Field validation, runs before validate, during the validation process.
+        :param field: An ex.Field instance
+        :param field_name: A string with the field name
+        :param value: The value to validate
+        :return: None
+        :raises: ex.ExodiaException
+        """
+        field._run_validators(value, field_name, self)
 
-    def post_field_validation(self, field, value):
-        setattr(self, field, value)
+    def validate(self, attrs):
+        """
+        Override to do custom validation, runs after the validation happens
+        :param attrs: Mapping of attributes to validate
+        :return: None
+        """
```

### Comparing `exodia-1.0.6/exodia/exceptions.py` & `exodia-1.0.7/exodia/exceptions.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.6/exodia/fields.py` & `exodia-1.0.7/exodia/fields.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+import typing
 from collections.abc import Callable, Mapping
 from datetime import date, datetime
 
+from typing_extensions import Self
+
 from exodia import ExodiaException, validators
-from exodia.utils import logger
 
 __all__ = ("Field", "String", "Integer", "Func", "List", "Exodia", "Date", "DateTime")
 
+T = typing.TypeVar("T")
+
 
-class Field:
+class Field(typing.Generic[T]):
     """
     Represents a Field
 
     class Person:
         name = ex.Field()
 
     except that you don't create Field instances, you create subclasses only.
 
     :param of_type: represents the allowed types to be worked with during validation process
     """
 
-    of_type = None
+    of_type: typing.Any = None
 
     def __init__(self, *args, **kwargs):
         self._name = None
         self.args = args
         self.kwargs = kwargs
+        self._validators = []
 
         assert self.of_type, "of_type can't be of value None"
-
-        self._validators = [
-            self.get_type_validator(),
-        ]
+        self.reset()
 
     def __set_name__(self, owner, name):
         self._name = name
 
     def _add_validator(self, v: validators.Validator):
         for validator in self._validators:
             if validator == v:
@@ -72,187 +74,187 @@
                 raise ExodiaException(
                     "Can't have validators [{v1}, {v2}] at the same time".format(
                         v1=validator.__class__.__name__,
                         v2=v.__name__,
                     )
                 )
 
-    def prepare_for_validation(self, v):
+    def prepare_for_validation(self, v: typing.Any) -> T:
         return v
 
-    def validate(self, value):
+    def validate(self, value) -> T:
         self._run_validators(self.prepare_for_validation(value))
         return self.to_repr(value)
 
     def get_type_validator(self):
         return validators.Type(self.of_type)
 
-    def to_repr(self, v):
+    def to_repr(self, v) -> T:
         return v
 
-    def optional(self):
-        required = self._pop_validator(validators.Required())
+    def optional(self) -> Self:
+        self._pop_validator(validators.Required())
         self._add_validator(validators.Optional())
 
-        if required:
-            logger.info("Found an optional() constraint followed by required()")
-
         # generate an optional self.of_type validator
         current_type_validator = self._pop_validator(self.get_type_validator())
         OptionalTypeValidator = current_type_validator.merge(validators.Type(None))
 
         self._add_validator(OptionalTypeValidator)
         return self
 
-    def required(self):
-        optional = self._pop_validator(validators.Optional())
-
-        if optional:
-            logger.info("Found a required() constraint followed by optional()")
-
+    def required(self) -> Self:
+        self._pop_validator(validators.Optional())
         self._add_validator(validators.Required())
 
         current_type_validator = self._pop_validator(self.get_type_validator())
         RequiredTypeValidator = current_type_validator.__class__(self.of_type)
 
         self._add_validator(RequiredTypeValidator)
         return self
 
-    def function(self, f, message):
+    def function(self, f, message) -> Self:
         self._add_validator(validators.Function(f, message))
         return self
 
-    def enum(self, options):
+    def enum(self, options) -> Self:
         self._add_validator(validators.Enum(options))
         return self
 
-    def ref(self, field, expr, message=None):
+    def ref(self, field, expr, message=None) -> Self:
         self._add_validator(validators.Ref(field, expr, message))
         return self
 
-    def reset(self, v):
+    def reset(self):
         self._validators = [
             self.get_type_validator(),
         ]
 
-        return self
-
-    def __set__(self, instance, value):
+    def __set__(self, instance, value) -> None:
         self._run_validators(self.prepare_for_validation(value), self._name, instance)
         instance.__dict__[self._name] = self.to_repr(value)
 
-    def __get__(self, instance, owner):
+    def __get__(self, instance, owner) -> T:
         return instance.__dict__[self._name]
 
 
-class String(Field):
-    of_type = str
+class String(Field[str]):
+    of_type: typing.Any = str
 
     def __init__(self, length=None, **kwargs):
         super().__init__(length, **kwargs)
 
         if length:
             self._add_validator(validators.Length(length))
 
-    def min(self, value: int):
+    def min(self, value: int) -> Self:
         self._add_validator(validators.MinLength(value))
         return self
 
-    def max(self, value: int):
+    def max(self, value: int) -> Self:
         self._add_validator(validators.MaxLength(value))
         return self
 
-    def not_empty(self):
+    def not_empty(self) -> Self:
         self._add_validator(validators.NotEmpty())
+        return self
 
 
-class Integer(Field):
-    of_type = int
+class Integer(Field[int]):
+    of_type: typing.Any = int
 
-    def min(self, value: int):
+    def min(self, value: int) -> Self:
         self._add_validator(
             validators.Stack(
                 [
                     validators.GreaterThan(value),
                     validators.Equal(value),
                 ]
             )
         )
 
         return self
 
-    def max(self, value: int):
+    def max(self, value: int) -> Self:
         self._add_validator(
             validators.Stack(
                 [
                     validators.LessThan(value),
                     validators.Equal(value),
                 ]
             )
         )
 
         return self
 
-    def between(self, min: int, max: int):
+    def between(self, min: int, max: int) -> Self:
         self._add_validator(validators.Between(min, max))
         return self
 
-    def multiple_of(self, n):
+    def multiple_of(self, n) -> Self:
         self._add_validator(validators.MultipleOf(n))
         return self
 
 
-class List(String):
-    of_type = list
+class List(String, Field[typing.List]):
+    of_type: typing.Any = list
 
 
-class Func(Field):
-    of_type = Callable
+class Func(Field[typing.Callable]):
+    of_type: typing.Any = Callable
 
 
-class Exodia(Field):
-    of_type = Mapping
+class Exodia(Field[typing.Mapping]):
+    of_type: typing.Any = Mapping
 
     def __init__(self, schema, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._add_validator(validators.Exodia(schema))
 
 
-class Date(Field):
-    of_type = [str, date]
-
-    def prepare_for_validation(self, v):
-        return date.fromisoformat(v)
-
-    def to_repr(self, v):
-        return date.fromisoformat(v)
+class DateTime(Field[datetime]):
+    of_type = [str, datetime]
 
-    def between(self, start: date, end: date):
-        self._add_validator(validators.Between(start, end))
-        return self
+    def prepare_for_validation(self, v: str) -> datetime:
+        return datetime.fromisoformat(v)
 
-    def before(self, d: date):
+    def before(self, d: datetime) -> Self:
         self._add_validator(validators.LessThan(d))
         return self
 
-    def after(self, d: date):
+    def after(self, d: datetime) -> Self:
         self._add_validator(validators.GreaterThan(d))
         return self
 
+    def between(self, start: datetime, end: datetime) -> Self:
+        self._add_validator(validators.Between(start, end))
+        return self
 
-class DateTime(Date):
-    of_type = [str, datetime]
 
-    def prepare_for_validation(self, v: str):
-        return datetime.fromisoformat(v)
+class Date(DateTime, Field[date]):
+    of_type = [str, date]
+
+    def prepare_for_validation(self, v) -> date:
+        return date.fromisoformat(v)
+
+    def to_repr(self, v) -> date:
+        return date.fromisoformat(v)
 
-    def before(self, d: datetime):
+    def between(self, start: date, end: date) -> Self:
+        self._add_validator(validators.Between(start, end))
+        return self
+
+    def before(self, d: date) -> Self:
         self._add_validator(validators.LessThan(d))
         return self
 
-    def after(self, d: datetime):
+    def after(self, d: date) -> Self:
         self._add_validator(validators.GreaterThan(d))
         return self
 
-    def between(self, start: datetime, end: datetime):
-        self._add_validator(validators.Between(start, end))
+
+class Any(Field[T]):
+    of_type = object
+
+    def of(self, *fields) -> Self:
+        self._add_validator(validators.Any(fields))
         return self
```

### Comparing `exodia-1.0.6/exodia/validators.py` & `exodia-1.0.7/exodia/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 from collections.abc import Callable, Iterable, Mapping
 from typing import List
 
 from exodia import ExodiaException
 from exodia.utils import get_callable_params
 
 __all__ = (
@@ -19,14 +20,15 @@
     "Optional",
     "Required",
     "Enum",
     "Between",
     "Function",
     "Ref",
     "MultipleOf",
+    "Any",
 )
 
 
 class Validator:
     field_message = "You've forgot to include a message for validator {class_name}"
     generic_message = "You've forgot to include a message for validator {class_name}"
 
@@ -304,15 +306,15 @@
         return self.message
 
     def validate(self, value, field_name=None, instance=None):
         return self.f(value)
 
 
 class Stack(Validator):
-    def __init__(self, validators: List[Validator]):
+    def __init__(self, validators: Iterable[Validator]):
         for i, validator in enumerate(validators):
             assert isinstance(
                 validator, Validator
             ), "validators[{}] is not ex.validators.Validator instance".format(str(i))
 
         self.validators = validators
         self.validator_names = list(map(lambda v: v.__class__.__name__, validators))
@@ -355,7 +357,33 @@
                     class_name=instance.__class__.__name__,
                     field=self.field,
                 )
             )
 
         # no __dict__ because validation is still running
         return self.expr(value, instance.__dict__[field_name])
+
+
+class Any(Validator):
+    def __init__(self, fields):
+        self.fields = fields
+        super().__init__()
+
+    def validate(self, value, field_name=None, instance=None):
+        for field in self.fields:
+            try:
+                field._run_validators(value, field_name, instance)
+                return True
+            except ExodiaException:
+                continue
+
+        return False
+
+    def get_message(self, field_name):
+        fields = ", ".join(cls.__class__.__qualname__ for cls in self.fields)
+
+        if field_name:
+            return "{field_name} not of types ({fields})".format(
+                field_name=field_name, fields=fields
+            )
+
+        return "value not of types ({})".format(fields)
```

### Comparing `exodia-1.0.6/tests/test_instance_creation.py` & `exodia-1.0.7/tests/test_instance_creation.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.6/tests/test_validation.py` & `exodia-1.0.7/tests/test_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,7 +128,24 @@
             # no need to check if age in attrs, you can't get into this step
             # without providing both because both are required
             # any assertion errors are transformed into ex.ExodiaException instances
             assert attrs["age"] > attrs["younger_brother_age"]
 
     with pytest.raises(ex.ExodiaException):
         Person(age=25, younger_brother_age=30)
+
+
+def test_any():
+    class Person(ex.Base):
+        age = ex.Any().of(ex.String(), ex.Integer())
+
+    Person(age=25)
+    Person(age="25")
+
+    with pytest.raises(ex.ExodiaException):
+        Person(age=dict())
+
+    with pytest.raises(ex.ExodiaException):
+        Person(age=type("Name", (type,), {}))
+
+    with pytest.raises(ex.ExodiaException):
+        Person(age=Exception())
```


# Comparing `tmp/data-spec-validator-3.1.0.tar.gz` & `tmp/data-spec-validator-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/data-spec-validator-3.1.0.tar", last modified: Wed May 24 06:13:10 2023, max compression
+gzip compressed data, was "dist/data-spec-validator-3.2.0.tar", last modified: Fri May 26 03:49:04 2023, max compression
```

## Comparing `data-spec-validator-3.1.0.tar` & `data-spec-validator-3.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    14029 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/PKG-INFO
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/test/
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1813 2023-02-23 07:51:32.000000 data-spec-validator-3.1.0/test/test_nested_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     4764 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/test/test_class_type_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     5664 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/test_decorator_drf.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    58443 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/test/test_spec.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/test/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1633 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     6290 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/test/test_decorator_dj.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       46 2023-05-24 04:08:19.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     6567 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/data_spec_validator/decorator/decorators.py
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/spec/
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/
--rw-r--r--   0 kilikkuo   (501) staff       (20)       30 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      917 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    18501 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/validators.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     7490 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/checks.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     3408 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/actions.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      629 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2101 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/features.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      168 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/utils.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      404 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/spec/wrappers.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)     2664 2023-03-01 07:50:37.000000 data-spec-validator-3.1.0/data_spec_validator/spec/defines.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.1.0/data_spec_validator/__init__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)       22 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/data_spec_validator/__version__.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)    10614 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/README.md
--rw-r--r--   0 kilikkuo   (501) staff       (20)     1253 2023-05-24 06:12:07.000000 data-spec-validator-3.1.0/setup.py
--rw-r--r--   0 kilikkuo   (501) staff       (20)      458 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/setup.cfg
-drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/
--rw-r--r--   0 kilikkuo   (501) staff       (20)    14029 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/PKG-INFO
--rw-r--r--   0 kilikkuo   (501) staff       (20)      939 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/SOURCES.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       79 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/requires.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)       25 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/top_level.txt
--rw-r--r--   0 kilikkuo   (501) staff       (20)        1 2023-05-24 06:13:10.000000 data-spec-validator-3.1.0/data_spec_validator.egg-info/dependency_links.txt
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    14202 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/PKG-INFO
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/test/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1813 2023-02-23 07:51:32.000000 data-spec-validator-3.2.0/test/test_nested_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     4764 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/test/test_class_type_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     6069 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_decorator_drf.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    58976 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_spec.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/test/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1703 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/utils.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     6695 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/test/test_decorator_dj.py
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       46 2023-05-24 04:08:19.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     7125 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/decorator/decorators.py
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/spec/
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       30 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      917 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/defines.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    19000 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/spec/validators.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     7788 2023-05-26 03:24:49.000000 data-spec-validator-3.2.0/data_spec_validator/spec/checks.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     3408 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/actions.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      629 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     2101 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/features.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      168 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/utils.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      404 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/spec/wrappers.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     2664 2023-03-01 07:50:37.000000 data-spec-validator-3.2.0/data_spec_validator/spec/defines.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        0 2022-05-22 06:41:36.000000 data-spec-validator-3.2.0/data_spec_validator/__init__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       22 2023-05-26 03:47:52.000000 data-spec-validator-3.2.0/data_spec_validator/__version__.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    10747 2023-05-26 03:47:52.000000 data-spec-validator-3.2.0/README.md
+-rw-r--r--   0 kilikkuo   (501) staff       (20)     1253 2023-05-24 06:12:07.000000 data-spec-validator-3.2.0/setup.py
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      458 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/setup.cfg
+drwxr-xr-x   0 kilikkuo   (501) staff       (20)        0 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/
+-rw-r--r--   0 kilikkuo   (501) staff       (20)    14202 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/PKG-INFO
+-rw-r--r--   0 kilikkuo   (501) staff       (20)      939 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       79 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/requires.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)       25 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/top_level.txt
+-rw-r--r--   0 kilikkuo   (501) staff       (20)        1 2023-05-26 03:49:04.000000 data-spec-validator-3.2.0/data_spec_validator.egg-info/dependency_links.txt
```

### Comparing `data-spec-validator-3.1.0/PKG-INFO` & `data-spec-validator-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-spec-validator
-Version: 3.1.0
+Version: 3.2.0
 Summary: Validation tool for API/Function parameters
 Home-page: https://github.com/hardcoretech/data-spec-validator
 Author: GoFreight
 Author-email: pypi@hardcoretech.co
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md
 Description: # data-spec-validator
@@ -48,28 +48,33 @@
         pip install data-spec-validator[decorator-dj]  # Django Only
         pip install data-spec-validator[decorator]  # Django Rest Framework
         ```
         
         ## Quick Example
         * Do `validate_data_spec` directly wherever you like
         ```python
-        from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
+        from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, LIST_OF, Checker, CheckerOP, validate_data_spec
         
         class SomeSpec:
             field_a = Checker([INT])
             field_b = Checker([DIGIT_STR], optional=True)
             field_c = Checker([DIGIT_STR, INT], op=CheckerOP.ANY)
+            filed_d_array = Checker([LIST_OF], LIST_OF=int, alias='field_d[]', optional=True)
         
         some_data = dict(field_a=4, field_b='3', field_c=1, field_dont_care=[5,6])
         validate_data_spec(some_data, SomeSpec) # return True
         
         some_data = dict(field_a=4, field_c='1')
         validate_data_spec(some_data, SomeSpec) # return True
         
-        some_data = dict(field_a=4, field_c=1)
+        some_data = {
+            'field_a': 4,
+            'field_c': 1,
+            'field_d[]': [5, 6],
+        }
         validate_data_spec(some_data, SomeSpec) # return True
         
         some_data = dict(field_a='4', field_c='1')
         validate_data_spec(some_data, SomeSpec) # raise Exception
         
         some_data = dict(field_a='4', field_c='1')
         validate_data_spec(some_data, SomeSpec, nothrow=True) # return False
```

### Comparing `data-spec-validator-3.1.0/test/test_nested_spec.py` & `data-spec-validator-3.2.0/test/test_nested_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/test/test_class_type_spec.py` & `data-spec-validator-3.2.0/test/test_class_type_spec.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/test/test_decorator_drf.py` & `data-spec-validator-3.2.0/test/test_decorator_drf.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,36 +88,40 @@
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
     @parameterized.expand(['PUT', 'PATCH', 'DELETE'])
     def test_query_params_with_data(self, method):
         # arrange
-        qs = 'q_a=3&q_b=true'
-        payload = {'test_a': 'TEST A'}
+        qs = 'q_a=3&q_b=true&d.o.t=dot&array[]=a1&array[]=a2&array[]=a3'
+        payload = {'test_a': 'TEST A', 'test_f[]': [1, 2, 3]}
 
         fake_request = make_request(Request, method='POST', data=payload, qs=qs)
 
-        kwargs = {'test_b': 'TEST_B'}
+        kwargs = {'test_b': 'TEST_B', 'test_c.d.e': 'TEST C.D.E'}
 
         @dsv_feature(strict=True)
         class _ViewSpec:
             q_a = Checker([LIST_OF], LIST_OF=STR)
             q_b = Checker([LIST_OF], LIST_OF=STR)
             test_a = Checker([ONE_OF], ONE_OF='TEST A')
             test_b = Checker([ONE_OF], ONE_OF='TEST_B')
+            test_c_d_e = Checker([ONE_OF], ONE_OF='TEST C.D.E', alias='test_c.d.e')
+            test_f_array = Checker([LIST_OF], LIST_OF=int, alias='test_f[]')
+            d_o_t = Checker([LIST_OF], LIST_OF=str, alias='d.o.t')
+            array = Checker([LIST_OF], LIST_OF=str, alias='array[]')
 
         class _View(View):
             @dsv(_ViewSpec)
             def decorated_func(self, req, *_args, **_kwargs):
-                pass
+                return True
 
         view = _View(request=fake_request)
         with override_method(view, fake_request, method) as request:
-            view.decorated_func(request, **kwargs)
+            assert view.decorated_func(request, **kwargs)
 
     def test_req_list_data_with_no_multirow_set(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
         fake_request = make_request(Request, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
```

### Comparing `data-spec-validator-3.1.0/test/test_spec.py` & `data-spec-validator-3.2.0/test/test_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1228,14 +1228,32 @@
         assert is_something_error(KeyError, validate_data_spec, dict(b=1, c=1), _CondExistOtherFailAOBCSpec)
         assert is_something_error(LookupError, validate_data_spec, dict(a=1), _CondExistOtherFailAOBCSpec)
         assert is_something_error(LookupError, validate_data_spec, dict(b=1), _CondExistOtherFailAOBCSpec)
         assert is_something_error(LookupError, validate_data_spec, dict(c=1), _CondExistOtherFailAOBCSpec)
         assert is_something_error(LookupError, validate_data_spec, dict(d=1), _CondExistOtherFailAOBCSpec)
         # ==========================
 
+    def test_alias(self):
+        class AliasSpec:
+            dot_field = Checker([int], alias='dot.field')
+            array_field = Checker([LIST_OF], LIST_OF=str, alias='array_field[]')
+
+        ok_data = {
+            'dot.field': 3,
+            'array_field[]': ['a', 'b'],
+        }
+
+        assert validate_data_spec(ok_data, AliasSpec)
+
+        nok_data = {
+            'dot_field': 3,
+            'array_field': ['a', 'b'],
+        }
+        assert is_something_error(LookupError, validate_data_spec, nok_data, AliasSpec)
+
 
 class TestCustomSpec(unittest.TestCase):
     def test_incorrect_validator_class(self):
         some_check = 'some_check'
 
         class InvalidClassValidator:
             name = some_check
```

### Comparing `data-spec-validator-3.1.0/test/utils.py` & `data-spec-validator-3.2.0/test/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     except TypeError:
         return True
     return False
 
 
 def is_django_installed():
     try:
-        pass
+        import django  # noqa
     except ImportError:
         return False
     return True
 
 
 def is_drf_installed():
     try:
-        pass
+        import rest_framework  # noqa
     except ImportError:
         return False
     return True
 
 
 def make_request(cls, path='/', method='GET', user=None, headers=None, data=None, qs=None):
     assert is_django_installed()
@@ -47,15 +47,15 @@
 
     if headers:
         req.META.update(headers)
 
     if data:
         if method == 'GET':
             setattr(req, 'GET', data)
-        elif method == 'POST':
+        elif method in ['POST', 'PUT', 'PATCH', 'DELETE']:
             req.read()  # trigger RawPostDataException and force DRF to load data from req.POST
             req.META.update(
                 {
                     'CONTENT_TYPE': 'application/x-www-form-urlencoded',
                     'CONTENT_LENGTH': len(str(data)),
                 }
             )
```

### Comparing `data-spec-validator-3.1.0/test/test_decorator_dj.py` & `data-spec-validator-3.2.0/test/test_decorator_dj.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,35 +109,39 @@
 
         view = _View(request=fake_request)
         view.decorated_func(fake_request, **kwargs)
 
     @parameterized.expand(['PUT', 'PATCH', 'DELETE'])
     def test_query_params_with_data(self, method):
         # arrange
-        qs = 'q_a=3&q_b=true'
-        payload = {'test_a': 'TEST A'}
+        qs = 'q_a=3&q_b=true&d.o.t=dot&array[]=a1&array[]=a2&array[]=a3'
+        payload = {'test_a': 'TEST A', 'test_f[]': [1, 2, 3]}
 
         fake_request = make_request(WSGIRequest, method=method, data=payload, qs=qs)
 
-        kwargs = {'test_b': 'TEST_B'}
+        kwargs = {'test_b': 'TEST_B', 'test_c.d.e': 'TEST C.D.E'}
 
         @dsv_feature(strict=True)
         class _ViewSpec:
             q_a = Checker([LIST_OF], LIST_OF=STR)
             q_b = Checker([LIST_OF], LIST_OF=STR)
             test_a = Checker([ONE_OF], ONE_OF='TEST A')
             test_b = Checker([ONE_OF], ONE_OF='TEST_B')
+            test_c_d_e = Checker([ONE_OF], ONE_OF='TEST C.D.E', alias='test_c.d.e')
+            test_f_array = Checker([LIST_OF], LIST_OF=int, alias='test_f[]')
+            d_o_t = Checker([LIST_OF], LIST_OF=str, alias='d.o.t')
+            array = Checker([LIST_OF], LIST_OF=str, alias='array[]')
 
         class _View(View):
             @dsv(_ViewSpec)
             def decorated_func(self, req, *_args, **_kwargs):
-                pass
+                return True
 
         view = _View(request=fake_request)
-        view.decorated_func(fake_request, **kwargs)
+        assert view.decorated_func(fake_request, **kwargs)
 
     def test_req_list_data_with_no_multirow_set(self):
         # arrange
         payload = [{'test_a': 'TEST A1'}, {'test_a': 'TEST A2'}, {'test_a': 'TEST A3'}]
         fake_request = make_request(WSGIRequest, method='POST', data=payload)
         kwargs = {'test_b': 'TEST_B'}
```

### Comparing `data-spec-validator-3.1.0/data_spec_validator/decorator/decorators.py` & `data-spec-validator-3.2.0/data_spec_validator/decorator/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import wraps
 from typing import Dict, List, Union
 
 from data_spec_validator.spec import DSVError, raise_if, validate_data_spec
 
 try:
+    import django
     from django.core.handlers.wsgi import WSGIRequest
     from django.http import HttpResponseBadRequest, HttpResponseForbidden, QueryDict
     from django.views.generic.base import View
 except ModuleNotFoundError as e:
     print(f'[DSV][WARNING] decorator: "dsv" cannot be used, {e}')
 
 _enabled_drf = False
@@ -15,14 +16,23 @@
     import rest_framework.exceptions as drf_exceptions
     from rest_framework.request import Request
 
     _enabled_drf = True
 except ModuleNotFoundError:
     print('[DSV][INFO] decorator: using "dsv" without djangorestframework')
 
+# try importing ASGIRequest (released since Django 3.0)
+if django.__version__ >= '3':
+    try:
+        from django.core.handlers.asgi import ASGIRequest
+
+        _has_support_asgi_request = True
+    except ModuleNotFoundError:
+        _has_support_asgi_request = False
+
 
 class ValidationError(Exception):
     def __init__(self, message):
         self.message = message
 
 
 class PermissionDenied(Exception):
@@ -35,20 +45,26 @@
         self.message = message
 
 
 def _is_wsgi_request(obj):
     return isinstance(obj, WSGIRequest)
 
 
+def _is_asgi_request(obj):
+    if not _has_support_asgi_request:
+        return False
+    return isinstance(obj, ASGIRequest)
+
+
 def _is_drf_request(obj):
     return _enabled_drf and isinstance(obj, Request)
 
 
 def _is_request(obj):
-    return _is_wsgi_request(obj) or _is_drf_request(obj)
+    return _is_wsgi_request(obj) or _is_asgi_request(obj) or _is_drf_request(obj)
 
 
 def _is_view(obj):
     return issubclass(type(obj), View)
 
 
 def _combine_named_params(data, **kwargs):
@@ -70,38 +86,39 @@
     else:
         data = combine_params(data, kwargs)
     return data
 
 
 def _extract_request_meta(req, **kwargs):
     raise_if(
-        not _is_wsgi_request(req) and not _is_drf_request(req),
+        not _is_wsgi_request(req) and not _is_asgi_request(req) and not _is_drf_request(req),
         RuntimeError(f'Unsupported req type, {type(req)}'),
     )
     return _combine_named_params(req.META, **kwargs)
 
 
 def _extract_request_param_data(req, **kwargs):
     is_wsgi_request = _is_wsgi_request(req)
+    is_asgi_request = _is_asgi_request(req)
     is_request = _is_drf_request(req)
     raise_if(
-        not is_wsgi_request and not is_request,
+        not is_wsgi_request and not is_asgi_request and not is_request,
         RuntimeError(f'Unsupported req type, {type(req)}'),
     )
 
     def _collect_data(method, req_qp, req_data) -> Dict:
         if method == 'GET':
             return req_qp
         else:
             if req_qp and issubclass(type(req_qp), dict) and type(req_data) is not list:
                 return {**req_qp, **req_data}
             # TODO: Don't care about the query_params if it's not a dict or the payload is in list.
             return req_data
 
-    if is_wsgi_request:
+    if is_wsgi_request or is_asgi_request:
         data = _collect_data(req.method, req.GET, req.POST)
     else:
         data = _collect_data(req.method, req.query_params, req.data)
 
     return _combine_named_params(data, **kwargs)
```

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/custom_spec/defines.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/custom_spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/validators.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import copy
 import datetime
 import json
 import re
 import uuid
+from dataclasses import dataclass
 from decimal import Decimal
 from functools import lru_cache
-from typing import Any, Dict, Iterable, List, Tuple, Type, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, Union
 
 import dateutil.parser
 
 from .checks import (
     _TYPE,
     AMOUNT,
     AMOUNT_RANGE,
@@ -49,27 +50,33 @@
 _SPEC_WISE_CHECKS = [COND_EXIST]
 
 
 class UnknownFieldValue:
     message = 'This field cannot be found in this SPEC'
 
 
+@dataclass(frozen=True)
+class FieldKey:
+    spec_field: str
+    data_field: Optional[str] = None
+
+
 @lru_cache(1)
 def get_unknown_field_value() -> UnknownFieldValue:
     return UnknownFieldValue()
 
 
-def _extract_value(checks: list, data: dict, field: str):
+def _extract_value(checks: list, data: dict, field_key: FieldKey):
     if LIST_OF in checks and hasattr(data, 'getlist'):
         # For QueryDict, all query values are put into list for the same key.
         # It should be client side's (Spec maker) responsibility to indicate that
         # whether the field is a list or not.
-        value = data.getlist(field, get_unknown_field_value())
+        value = data.getlist(field_key.data_field, get_unknown_field_value())
     else:
-        value = data.get(field, get_unknown_field_value())
+        value = data.get(field_key.data_field, get_unknown_field_value())
     return value
 
 
 def _makeup_internals_to_extra(spec: Type, checks: List[str], raw_extra: Dict, allow_optional: bool) -> Dict:
     extra = copy.deepcopy(raw_extra)
     if extra.get(SpecValidator.name) == SELF:
         extra[SpecValidator.name] = spec
@@ -87,22 +94,22 @@
     return value is None and allow_none
 
 
 def _pass_unknown(_extra: Dict, value: Any) -> bool:
     return value == get_unknown_field_value() and _ALLOW_UNKNOWN in _extra
 
 
-def _validate_field(data, field, spec) -> Tuple[bool, List[ValidateResult]]:
-    checker = getattr(spec, field)
+def _validate_field(data, field_key: FieldKey, spec) -> Tuple[bool, List[ValidateResult]]:
+    checker = getattr(spec, field_key.spec_field)
 
     checks = checker.checks
     allow_optional = checker.allow_optional
     allow_none = checker.allow_none
 
-    value = _extract_value(checks, data, field)
+    value = _extract_value(checks, data, field_key)
     extra = _makeup_internals_to_extra(spec, checks, checker.extra, allow_optional)
 
     results = []
 
     if _pass_optional(allow_optional, checks, value):
         # Skip all the other checks' validations
         return True, []
@@ -122,15 +129,15 @@
                 else:
                     ok, error = False, RuntimeError(f'{repr(ae)}')
             except NotImplementedError:
                 raise
             except Exception as e:
                 # For any unwell-handled case, go this way for now.
                 ok, error = False, RuntimeError(f'{repr(e)}')
-            _acc_results.append((ok, ValidateResult(spec, field, _value, _check, error)))
+            _acc_results.append((ok, ValidateResult(spec, field_key.data_field, _value, _check, error)))
 
         spec_wise_checks = set(filter(lambda c: c in _SPEC_WISE_CHECKS, checks))
         field_wise_checks = set(checks) - spec_wise_checks
 
         for chk in spec_wise_checks:
             _do_validate(results, spec, chk, value, data, extra)
 
@@ -142,17 +149,17 @@
     if checker.is_op_any and len(nok_results) == len(checks):
         return False, nok_results
     if checker.is_op_all and nok_results:
         return False, nok_results
     return True, []
 
 
-def _validate_spec_features(data, fields, spec) -> Tuple[bool, List[ValidateResult]]:
+def _validate_spec_features(data, data_fields, spec) -> Tuple[bool, List[ValidateResult]]:
     if is_strict(spec):
-        unexpected = set(data.keys()) - set(fields)
+        unexpected = set(data.keys()) - set(data_fields)
         if unexpected:
             error = ValueError(f'Unexpected field keys({unexpected}) found in strict mode spec')
             return False, [ValidateResult(spec, str(unexpected), data, 'strict', error)]
 
     any_keys_set = get_any_keys_set(spec)
     if any_keys_set:
         data_keys = set(data.keys())
@@ -161,16 +168,16 @@
                 str_keys = ", ".join(keys)
                 error = KeyError('At least one of these fields must exist')
                 return False, [ValidateResult(spec, str_keys, data, 'any_keys_set', error)]
 
     return True, [ValidateResult()]
 
 
-def _validate_spec_fields(data, fields, spec) -> List[Tuple[bool, List[ValidateResult]]]:
-    rs = [_validate_field(data, f, spec) for f in fields]
+def _validate_spec_fields(data, field_keys: List[FieldKey], spec) -> List[Tuple[bool, List[ValidateResult]]]:
+    rs = [_validate_field(data, fk, spec) for fk in field_keys]
     return rs
 
 
 class DummyValidator(BaseValidator):
     name = DUMMY
 
     @staticmethod
@@ -357,29 +364,36 @@
         return ok, info
 
 
 class SpecValidator(BaseValidator):
     name = SPEC
 
     @staticmethod
-    def _extract_fields(spec) -> List[str]:
+    def _extract_field_keys(spec) -> List[FieldKey]:
         raise_if(type(spec) != type, RuntimeError(f'{spec} should be a spec class'))
-        return [f_name for f_name, checker in spec.__dict__.items() if isinstance(checker, Checker)]
+
+        fields = []
+        for f_name, checker in spec.__dict__.items():
+            if isinstance(checker, Checker):
+                key = FieldKey(spec_field=f_name, data_field=checker.alias if checker.alias else f_name)
+                fields.append(key)
+
+        return fields
 
     @staticmethod
     def validate(value, extra, data) -> Tuple[bool, List[Tuple[bool, List[ValidateResult]]]]:
         target_spec = extra.get(SpecValidator.name)
 
-        fields = SpecValidator._extract_fields(target_spec)
+        field_keys = SpecValidator._extract_field_keys(target_spec)
 
-        result = _validate_spec_features(value, fields, target_spec)
+        result = _validate_spec_features(value, [fk.data_field for fk in field_keys], target_spec)
         if not result[0]:
             return False, [result]
 
-        results = _validate_spec_fields(value, fields, target_spec)
+        results = _validate_spec_fields(value, field_keys, target_spec)
         failures = [r for r in results if not r[0]]
 
         ok = len(failures) == 0
         return ok, failures
 
 
 class ListOfValidator(BaseValidator):
```

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/checks.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,29 +148,34 @@
 class Checker:
     def __init__(
         self,
         raw_checks: List[RAW_CHECK_TYPE],
         optional: bool = False,
         allow_none: bool = False,
         op: CheckerOP = CheckerOP.ALL,
+        alias: Optional[str] = None,
         **kwargs,
     ):
         """
         checks: list of str/class (Check)
         optional: boolean
                   Set optional to True, the validation process will be passed if the field is absent
         allow_none: boolean
                   Set allow_none to True, the field value can be None
         op: CheckerOP
+        alias: str or None
+               A string that represents the field name which will be used when extracting values from data payload
+        kwargs: dict
         """
         self.checks, class_check_type = self._sanitize_checks(raw_checks)
 
         self._op = op
         self._optional = optional
         self._allow_none = allow_none
+        self._alias = alias
 
         self._ensure(kwargs)
         self.extra = self._build_extra(class_check_type, kwargs)
 
     @staticmethod
     def _sanitize_checks(raw_checks: List[RAW_CHECK_TYPE]) -> Tuple[List[str], Optional[Type[Any]]]:
         class_type_check = None
@@ -247,7 +252,11 @@
     @property
     def is_op_any(self) -> bool:
         return self._op == CheckerOP.ANY
 
     @property
     def is_op_all(self) -> bool:
         return self._op == CheckerOP.ALL
+
+    @property
+    def alias(self) -> str:
+        return self._alias
```

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/actions.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/actions.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/__init__.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/features.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/features.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/data_spec_validator/spec/defines.py` & `data-spec-validator-3.2.0/data_spec_validator/spec/defines.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/README.md` & `data-spec-validator-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,28 +39,33 @@
 pip install data-spec-validator[decorator-dj]  # Django Only
 pip install data-spec-validator[decorator]  # Django Rest Framework
 ```
 
 ## Quick Example
 * Do `validate_data_spec` directly wherever you like
 ```python
-from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
+from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, LIST_OF, Checker, CheckerOP, validate_data_spec
 
 class SomeSpec:
     field_a = Checker([INT])
     field_b = Checker([DIGIT_STR], optional=True)
     field_c = Checker([DIGIT_STR, INT], op=CheckerOP.ANY)
+    filed_d_array = Checker([LIST_OF], LIST_OF=int, alias='field_d[]', optional=True)
 
 some_data = dict(field_a=4, field_b='3', field_c=1, field_dont_care=[5,6])
 validate_data_spec(some_data, SomeSpec) # return True
 
 some_data = dict(field_a=4, field_c='1')
 validate_data_spec(some_data, SomeSpec) # return True
 
-some_data = dict(field_a=4, field_c=1)
+some_data = {
+    'field_a': 4,
+    'field_c': 1,
+    'field_d[]': [5, 6],
+}
 validate_data_spec(some_data, SomeSpec) # return True
 
 some_data = dict(field_a='4', field_c='1')
 validate_data_spec(some_data, SomeSpec) # raise Exception
 
 some_data = dict(field_a='4', field_c='1')
 validate_data_spec(some_data, SomeSpec, nothrow=True) # return False
```

### Comparing `data-spec-validator-3.1.0/setup.py` & `data-spec-validator-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `data-spec-validator-3.1.0/data_spec_validator.egg-info/PKG-INFO` & `data-spec-validator-3.2.0/data_spec_validator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-spec-validator
-Version: 3.1.0
+Version: 3.2.0
 Summary: Validation tool for API/Function parameters
 Home-page: https://github.com/hardcoretech/data-spec-validator
 Author: GoFreight
 Author-email: pypi@hardcoretech.co
 License: UNKNOWN
 Project-URL: Changelog, https://github.com/hardcoretech/data-spec-validator/blob/develop/CHANGELOG.md
 Description: # data-spec-validator
@@ -48,28 +48,33 @@
         pip install data-spec-validator[decorator-dj]  # Django Only
         pip install data-spec-validator[decorator]  # Django Rest Framework
         ```
         
         ## Quick Example
         * Do `validate_data_spec` directly wherever you like
         ```python
-        from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, Checker, CheckerOP, validate_data_spec
+        from data_spec_validator.spec import INT, DIGIT_STR, ONE_OF, LIST_OF, Checker, CheckerOP, validate_data_spec
         
         class SomeSpec:
             field_a = Checker([INT])
             field_b = Checker([DIGIT_STR], optional=True)
             field_c = Checker([DIGIT_STR, INT], op=CheckerOP.ANY)
+            filed_d_array = Checker([LIST_OF], LIST_OF=int, alias='field_d[]', optional=True)
         
         some_data = dict(field_a=4, field_b='3', field_c=1, field_dont_care=[5,6])
         validate_data_spec(some_data, SomeSpec) # return True
         
         some_data = dict(field_a=4, field_c='1')
         validate_data_spec(some_data, SomeSpec) # return True
         
-        some_data = dict(field_a=4, field_c=1)
+        some_data = {
+            'field_a': 4,
+            'field_c': 1,
+            'field_d[]': [5, 6],
+        }
         validate_data_spec(some_data, SomeSpec) # return True
         
         some_data = dict(field_a='4', field_c='1')
         validate_data_spec(some_data, SomeSpec) # raise Exception
         
         some_data = dict(field_a='4', field_c='1')
         validate_data_spec(some_data, SomeSpec, nothrow=True) # return False
```

### Comparing `data-spec-validator-3.1.0/data_spec_validator.egg-info/SOURCES.txt` & `data-spec-validator-3.2.0/data_spec_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


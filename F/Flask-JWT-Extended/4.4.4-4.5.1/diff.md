# Comparing `tmp/Flask-JWT-Extended-4.4.4.tar.gz` & `tmp/Flask-JWT-Extended-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-JWT-Extended-4.4.4.tar", last modified: Mon Aug 15 16:32:28 2022, max compression
+gzip compressed data, was "Flask-JWT-Extended-4.5.1.tar", last modified: Fri May 26 17:19:20 2023, max compression
```

## Comparing `Flask-JWT-Extended-4.4.4.tar` & `Flask-JWT-Extended-4.5.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:28.219014 Flask-JWT-Extended-4.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:28.215014 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-15 16:32:28.000000 Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-08-15 16:32:28.219014 Flask-JWT-Extended-4.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:28.215014 Flask-JWT-Extended-4.4.4/flask_jwt_extended/
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9999 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/default_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    23844 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/jwt_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)    15880 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12886 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/flask_jwt_extended/view_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-15 16:32:28.219014 Flask-JWT-Extended-4.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:28.219014 Flask-JWT-Extended-4.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_add_context_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4941 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_additional_claims_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_asymmetric_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_blocklist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_claims_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)    13210 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    19917 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (121)    12938 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_decode_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_get_jwt_in_non_protected_contexts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_get_methods_in_optional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7162 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_jwt_header_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     6262 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_multiple_token_locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_options_method.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_query_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_user_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)    17187 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/test_view_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-08-15 16:32:16.000000 Flask-JWT-Extended-4.4.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.202373 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/flask_jwt_extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/default_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23923 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/jwt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/view_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_add_context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_additional_claims_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_asymmetric_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_blocklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_claims_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_decode_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_get_jwt_in_non_protected_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_get_methods_in_optional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_jwt_header_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_multiple_token_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_options_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_query_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_user_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_view_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tox.ini
```

### Comparing `Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/PKG-INFO` & `Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-JWT-Extended
-Version: 4.4.4
+Version: 4.5.1
 Summary: Extended JWT integration with Flask
 Home-page: https://github.com/vimalloc/flask-jwt-extended
 Author: Lily Acadia Gilbert
 Author-email: lily.gilbert@hey.com
 License: MIT
 Keywords: flask,jwt,json web token
 Platform: any
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: asymmetric_crypto
 License-File: LICENSE
```

### Comparing `Flask-JWT-Extended-4.4.4/Flask_JWT_Extended.egg-info/SOURCES.txt` & `Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/LICENSE` & `Flask-JWT-Extended-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/PKG-INFO` & `Flask-JWT-Extended-4.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-JWT-Extended
-Version: 4.4.4
+Version: 4.5.1
 Summary: Extended JWT integration with Flask
 Home-page: https://github.com/vimalloc/flask-jwt-extended
 Author: Lily Acadia Gilbert
 Author-email: lily.gilbert@hey.com
 License: MIT
 Keywords: flask,jwt,json web token
 Platform: any
@@ -17,14 +17,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Provides-Extra: asymmetric_crypto
 License-File: LICENSE
```

### Comparing `Flask-JWT-Extended-4.4.4/README.md` & `Flask-JWT-Extended-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/__init__.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from .utils import set_refresh_cookies as set_refresh_cookies
 from .utils import unset_access_cookies as unset_access_cookies
 from .utils import unset_jwt_cookies as unset_jwt_cookies
 from .utils import unset_refresh_cookies as unset_refresh_cookies
 from .view_decorators import jwt_required as jwt_required
 from .view_decorators import verify_jwt_in_request as verify_jwt_in_request
 
-__version__ = "4.4.4"
+__version__ = "4.5.1"
```

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/config.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/config.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/default_callbacks.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/default_callbacks.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/exceptions.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/internal_utils.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/internal_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,10 +89,10 @@
     Lookup Order:
       - app.json_encoder - For Flask < 2.2
       - app.json_provider_class.default
       - flask.json.provider.DefaultJSONProvider.default
 
     """
     if not HAS_JSON_PROVIDER:  # pragma: no cover
-        return app.json_encoder
+        return app.json_encoder  # type: ignore
 
     return JSONEncoder
```

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/jwt_manager.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/jwt_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,31 @@
 from flask_jwt_extended.exceptions import RevokedTokenError
 from flask_jwt_extended.exceptions import UserClaimsVerificationError
 from flask_jwt_extended.exceptions import UserLookupError
 from flask_jwt_extended.exceptions import WrongTokenError
 from flask_jwt_extended.tokens import _decode_jwt
 from flask_jwt_extended.tokens import _encode_jwt
 from flask_jwt_extended.typing import ExpiresDelta
+from flask_jwt_extended.typing import Fresh
 from flask_jwt_extended.utils import current_user_context_processor
 
 
 class JWTManager(object):
     """
     An object used to hold JWT settings and callback functions for the
     Flask-JWT-Extended extension.
 
     Instances of :class:`JWTManager` are *not* bound to specific apps, so
     you can create one in the main body of your code and then bind it
     to your app in a factory function.
     """
 
-    def __init__(self, app: Flask = None, add_context_processor: bool = False) -> None:
+    def __init__(
+        self, app: Optional[Flask] = None, add_context_processor: bool = False
+    ) -> None:
         """
         Create the JWTManager instance. You can either pass a flask application
         in directly here to register this extension with the flask app, or
         call init_app after creating this object (in a factory pattern).
 
         :param app:
             The Flask Application object
@@ -487,16 +490,16 @@
         return callback
 
     def _encode_jwt_from_config(
         self,
         identity: Any,
         token_type: str,
         claims=None,
-        fresh: bool = False,
-        expires_delta: ExpiresDelta = None,
+        fresh: Fresh = False,
+        expires_delta: Optional[ExpiresDelta] = None,
         headers=None,
     ) -> str:
         header_overrides = self._jwt_additional_header_callback(identity)
         if headers is not None:
             header_overrides.update(headers)
 
         claim_overrides = self._user_claims_callback(identity)
```

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/tokens.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 from typing import Union
 
 import jwt
 
 from flask_jwt_extended.exceptions import CSRFError
 from flask_jwt_extended.exceptions import JWTDecodeError
 from flask_jwt_extended.typing import ExpiresDelta
+from flask_jwt_extended.typing import Fresh
 
 
 def _encode_jwt(
     algorithm: str,
     audience: Union[str, Iterable[str]],
     claim_overrides: dict,
     csrf: bool,
     expires_delta: ExpiresDelta,
-    fresh: bool,
+    fresh: Fresh,
     header_overrides: dict,
     identity: Any,
     identity_claim_key: str,
     issuer: str,
     json_encoder: Type[JSONEncoder],
     secret: str,
     token_type: str,
```

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/utils.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-import datetime
 from typing import Any
 from typing import Optional
 
 import jwt
 from flask import g
 from flask import Response
 from werkzeug.local import LocalProxy
 
 from flask_jwt_extended.config import config
 from flask_jwt_extended.internal_utils import get_jwt_manager
+from flask_jwt_extended.typing import ExpiresDelta
+from flask_jwt_extended.typing import Fresh
 
 # Proxy to access the current user
 current_user: Any = LocalProxy(lambda: get_current_user())
 
 
 def get_jwt() -> dict:
     """
@@ -97,15 +98,15 @@
             "You must provide a `@jwt.user_lookup_loader` callback to use "
             "this method"
         )
     return jwt_user_dict["loaded_user"]
 
 
 def decode_token(
-    encoded_token: str, csrf_value: str = None, allow_expired: bool = False
+    encoded_token: str, csrf_value: Optional[str] = None, allow_expired: bool = False
 ) -> dict:
     """
     Returns the decoded token (python dict) from an encoded JWT. This does all
     the checks to ensure that the decoded token is valid before returning it.
 
     This will not fire the user loader callbacks, save the token for access
     in protected endpoints, checked if a token is revoked, etc. This is puerly
@@ -125,16 +126,16 @@
     """
     jwt_manager = get_jwt_manager()
     return jwt_manager._decode_jwt_from_config(encoded_token, csrf_value, allow_expired)
 
 
 def create_access_token(
     identity: Any,
-    fresh: bool = False,
-    expires_delta: datetime.timedelta = None,
+    fresh: Fresh = False,
+    expires_delta: Optional[ExpiresDelta] = None,
     additional_claims=None,
     additional_headers=None,
 ):
     """
     Create a new access token.
 
     :param identity:
@@ -179,15 +180,15 @@
         identity=identity,
         token_type="access",
     )
 
 
 def create_refresh_token(
     identity: Any,
-    expires_delta: datetime.timedelta = None,
+    expires_delta: Optional[ExpiresDelta] = None,
     additional_claims=None,
     additional_headers=None,
 ):
     """
     Create a new refresh token.
 
     :param identity:
@@ -316,16 +317,16 @@
             samesite=config.cookie_samesite,
         )
 
 
 def set_refresh_cookies(
     response: Response,
     encoded_refresh_token: str,
-    max_age: int = None,
-    domain: str = None,
+    max_age: Optional[int] = None,
+    domain: Optional[str] = None,
 ) -> None:
     """
     Modifiy a Flask Response to set a cookie containing the refresh JWT.
     Also sets the corresponding CSRF cookies if ``JWT_CSRF_IN_COOKIES`` is ``True``
     (see :ref:`Configuration Options`)
 
     :param response:
@@ -366,27 +367,27 @@
             httponly=False,
             domain=domain or config.cookie_domain,
             path=config.refresh_csrf_cookie_path,
             samesite=config.cookie_samesite,
         )
 
 
-def unset_jwt_cookies(response: Response, domain: str = None) -> None:
+def unset_jwt_cookies(response: Response, domain: Optional[str] = None) -> None:
     """
     Modifiy a Flask Response to delete the cookies containing access or refresh
     JWTs.  Also deletes the corresponding CSRF cookies if applicable.
 
     :param response:
         A Flask Response object
     """
     unset_access_cookies(response, domain)
     unset_refresh_cookies(response, domain)
 
 
-def unset_access_cookies(response: Response, domain: str = None) -> None:
+def unset_access_cookies(response: Response, domain: Optional[str] = None) -> None:
     """
     Modifiy a Flask Response to delete the cookie containing an access JWT.
     Also deletes the corresponding CSRF cookie if applicable.
 
     :param response:
         A Flask Response object
 
@@ -416,15 +417,15 @@
             httponly=False,
             domain=domain or config.cookie_domain,
             path=config.access_csrf_cookie_path,
             samesite=config.cookie_samesite,
         )
 
 
-def unset_refresh_cookies(response: Response, domain: str = None) -> None:
+def unset_refresh_cookies(response: Response, domain: Optional[str] = None) -> None:
     """
     Modifiy a Flask Response to delete the cookie containing a refresh JWT.
     Also deletes the corresponding CSRF cookie if applicable.
 
     :param response:
         A Flask Response object
```

### Comparing `Flask-JWT-Extended-4.4.4/flask_jwt_extended/view_decorators.py` & `Flask-JWT-Extended-4.5.1/flask_jwt_extended/view_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,17 @@
             raise FreshTokenRequired("Fresh token required", jwt_header, jwt_data)
 
 
 def verify_jwt_in_request(
     optional: bool = False,
     fresh: bool = False,
     refresh: bool = False,
-    locations: LocationType = None,
+    locations: Optional[LocationType] = None,
     verify_type: bool = True,
+    skip_revocation_check: bool = False,
 ) -> Optional[Tuple[dict, dict]]:
     """
     Verify that a valid JWT is present in the request, unless ``optional=True`` in
     which case no JWT is also considered valid.
 
     :param optional:
         If ``True``, do not raise an error if no JWT is present in the request.
@@ -72,26 +73,38 @@
         ``JWT_TOKEN_LOCATION`` configuration option.
 
     :param verify_type:
         If ``True``, the token type (access or refresh) will be checked according
         to the ``refresh`` argument. If ``False``, type will not be checked and both
         access and refresh tokens will be accepted.
 
+    :param skip_revocation_check:
+        If ``True``, revocation status of the token will be *not* checked. If ``False``,
+        revocation status of the token will be checked.
+
+    :param skip_revocation_check:
+        If ``True``, revocation status of the token will be *not* checked. If ``False``,
+        revocation status of the token will be checked.
+
     :return:
         A tuple containing the jwt_header and the jwt_data if a valid JWT is
         present in the request. If ``optional=True`` and no JWT is in the request,
         ``None`` will be returned instead. Raise an exception if an invalid JWT
         is in the request.
     """
     if request.method in config.exempt_methods:
         return None
 
     try:
         jwt_data, jwt_header, jwt_location = _decode_jwt_from_request(
-            locations, fresh, refresh=refresh, verify_type=verify_type
+            locations,
+            fresh,
+            refresh=refresh,
+            verify_type=verify_type,
+            skip_revocation_check=skip_revocation_check,
         )
 
     except NoAuthorizationError:
         if not optional:
             raise
         g._jwt_extended_jwt = {}
         g._jwt_extended_jwt_header = {}
@@ -109,16 +122,17 @@
     return jwt_header, jwt_data
 
 
 def jwt_required(
     optional: bool = False,
     fresh: bool = False,
     refresh: bool = False,
-    locations: LocationType = None,
+    locations: Optional[LocationType] = None,
     verify_type: bool = True,
+    skip_revocation_check: bool = False,
 ) -> Any:
     """
     A decorator to protect a Flask endpoint with JSON Web Tokens.
 
     Any route decorated with this will require a valid JWT to be present in the
     request (unless optional=True, in which case no JWT is also valid) before the
     endpoint can be called.
@@ -141,20 +155,26 @@
         which indicates that JWTs will be looked for in the locations defined by the
         ``JWT_TOKEN_LOCATION`` configuration option.
 
     :param verify_type:
         If ``True``, the token type (access or refresh) will be checked according
         to the ``refresh`` argument. If ``False``, type will not be checked and both
         access and refresh tokens will be accepted.
+
+    :param skip_revocation_check:
+        If ``True``, revocation status of the token will be *not* checked. If ``False``,
+        revocation status of the token will be checked.
     """
 
     def wrapper(fn):
         @wraps(fn)
         def decorator(*args, **kwargs):
-            verify_jwt_in_request(optional, fresh, refresh, locations, verify_type)
+            verify_jwt_in_request(
+                optional, fresh, refresh, locations, verify_type, skip_revocation_check
+            )
             return current_app.ensure_sync(fn)(*args, **kwargs)
 
         return decorator
 
     return wrapper
 
 
@@ -280,14 +300,15 @@
 
 
 def _decode_jwt_from_request(
     locations: LocationType,
     fresh: bool,
     refresh: bool = False,
     verify_type: bool = True,
+    skip_revocation_check: bool = False,
 ) -> Tuple[dict, dict, str]:
     # Figure out what locations to look for the JWT in this request
     if isinstance(locations, str):
         locations = [locations]
 
     if not locations:
         locations = config.token_location
@@ -342,11 +363,14 @@
 
     # Additional verifications provided by this extension
     if verify_type:
         verify_token_type(decoded_token, refresh)
 
     if fresh:
         _verify_token_is_fresh(jwt_header, decoded_token)
-    verify_token_not_blocklisted(jwt_header, decoded_token)
+
+    if not skip_revocation_check:
+        verify_token_not_blocklisted(jwt_header, decoded_token)
+
     custom_verification_for_token(jwt_header, decoded_token)
 
     return decoded_token, jwt_header, jwt_location
```

### Comparing `Flask-JWT-Extended-4.4.4/setup.py` & `Flask-JWT-Extended-4.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,12 +46,14 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_add_context_processor.py` & `Flask-JWT-Extended-4.5.1/tests/test_add_context_processor.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_additional_claims_loader.py` & `Flask-JWT-Extended-4.5.1/tests/test_additional_claims_loader.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_asymmetric_crypto.py` & `Flask-JWT-Extended-4.5.1/tests/test_asymmetric_crypto.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_blocklist.py` & `Flask-JWT-Extended-4.5.1/tests/test_blocklist.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,75 @@
     JWTManager(app)
 
     @app.route("/protected", methods=["GET"])
     @jwt_required()
     def access_protected():
         return jsonify(foo="bar")
 
+    @app.route("/protected_skip_blocklist", methods=["GET"])
+    @jwt_required(verify_type=False, skip_revocation_check=True)
+    def access_protected_skip_blocklist():
+        return jsonify(foo="bar")
+
+    @app.route("/protected_noskip_blocklist", methods=["GET"])
+    @jwt_required(verify_type=False)
+    def access_protected_no_skip_blocklist():
+        return jsonify(foo="bar")
+
     @app.route("/refresh_protected", methods=["GET"])
     @jwt_required(refresh=True)
     def refresh_protected():
         return jsonify(foo="bar")
 
     return app
 
 
 @pytest.mark.parametrize("blocklist_type", [["access"], ["refresh", "access"]])
+def test_blocklisted_access_token_revocation_skip(app, blocklist_type):
+    jwt = get_jwt_manager(app)
+
+    @jwt.token_in_blocklist_loader
+    def check_blocklisted(jwt_header, jwt_data):
+        assert jwt_header["alg"] == "HS256"
+        assert jwt_data["sub"] == "username"
+        return True
+
+    with app.test_request_context():
+        access_token = create_access_token("username")
+
+    test_client = app.test_client()
+    response = test_client.get(
+        "/protected_skip_blocklist", headers=make_headers(access_token)
+    )
+    assert response.get_json() == {"foo": "bar"}
+    assert response.status_code == 200
+
+
+@pytest.mark.parametrize("blocklist_type", [["access"], ["refresh", "access"]])
+def test_blocklisted_access_token_revocation_no_skip(app, blocklist_type):
+    jwt = get_jwt_manager(app)
+
+    @jwt.token_in_blocklist_loader
+    def check_blocklisted(jwt_header, jwt_data):
+        assert jwt_header["alg"] == "HS256"
+        assert jwt_data["sub"] == "username"
+        return True
+
+    with app.test_request_context():
+        access_token = create_access_token("username")
+
+    test_client = app.test_client()
+    response = test_client.get(
+        "/protected_noskip_blocklist", headers=make_headers(access_token)
+    )
+    assert response.get_json() == {"msg": "Token has been revoked"}
+    assert response.status_code == 401
+
+
+@pytest.mark.parametrize("blocklist_type", [["access"], ["refresh", "access"]])
 def test_non_blocklisted_access_token(app, blocklist_type):
     jwt = get_jwt_manager(app)
 
     @jwt.token_in_blocklist_loader
     def check_blocklisted(jwt_header, jwt_data):
         assert jwt_header["alg"] == "HS256"
         assert jwt_data["sub"] == "username"
```

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_claims_verification.py` & `Flask-JWT-Extended-4.5.1/tests/test_claims_verification.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_config.py` & `Flask-JWT-Extended-4.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_cookies.py` & `Flask-JWT-Extended-4.5.1/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_decode_tokens.py` & `Flask-JWT-Extended-4.5.1/tests/test_decode_tokens.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_get_jwt_in_non_protected_contexts.py` & `Flask-JWT-Extended-4.5.1/tests/test_get_jwt_in_non_protected_contexts.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_get_methods_in_optional_endpoint.py` & `Flask-JWT-Extended-4.5.1/tests/test_get_methods_in_optional_endpoint.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_headers.py` & `Flask-JWT-Extended-4.5.1/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_json.py` & `Flask-JWT-Extended-4.5.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_jwt_header_loader.py` & `Flask-JWT-Extended-4.5.1/tests/test_jwt_header_loader.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_multiple_token_locations.py` & `Flask-JWT-Extended-4.5.1/tests/test_multiple_token_locations.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_options_method.py` & `Flask-JWT-Extended-4.5.1/tests/test_options_method.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_query_string.py` & `Flask-JWT-Extended-4.5.1/tests/test_query_string.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_user_lookup.py` & `Flask-JWT-Extended-4.5.1/tests/test_user_lookup.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.4.4/tests/test_view_decorators.py` & `Flask-JWT-Extended-4.5.1/tests/test_view_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
     assert response.status_code == 422
     assert response.get_json() == {"msg": 'Token is missing the "aud" claim'}
 
     # Audience claim still expected and wrong one provided - not OK
     access_token = encode_token(app, {"aud": "different_audience", "sub": "me"})
     response = test_client.get(url, headers=make_headers(access_token))
     assert response.status_code == 422
-    assert response.get_json() == {"msg": "Invalid audience"}
+    assert response.get_json() == {"msg": "Audience doesn't match"}
 
 
 def test_jwt_invalid_issuer(app):
     url = "/protected"
     test_client = app.test_client()
 
     # No issuer claim expected or provided - OK
```

### Comparing `Flask-JWT-Extended-4.4.4/tox.ini` & `Flask-JWT-Extended-4.5.1/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (http://tox.testrun.org/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py37,py38,py39,py310,pypy3.9,flask21,mypy,coverage,style,docs
+envlist = py37,py38,py39,py310,py311,pypy3.9,flask21,mypy,coverage,style,docs
 
 [testenv]
 commands =
   pytest tests/
 deps =
   pytest
   cryptography
```


# Comparing `tmp/Flask-JWT-Extended-4.5.1.tar.gz` & `tmp/Flask-JWT-Extended-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-JWT-Extended-4.5.1.tar", last modified: Fri May 26 17:19:20 2023, max compression
+gzip compressed data, was "Flask-JWT-Extended-4.5.2.tar", last modified: Fri May 26 19:16:32 2023, max compression
```

## Comparing `Flask-JWT-Extended-4.5.1.tar` & `Flask-JWT-Extended-4.5.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.202373 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 17:19:20.000000 Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/flask_jwt_extended/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/default_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23923 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/jwt_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/flask_jwt_extended/view_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:20.206373 Flask-JWT-Extended-4.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_add_context_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_additional_claims_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_asymmetric_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_blocklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_claims_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_decode_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_get_jwt_in_non_protected_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_get_methods_in_optional_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_jwt_header_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_multiple_token_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_options_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_query_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_user_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/test_view_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 17:19:05.000000 Flask-JWT-Extended-4.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:32.357577 Flask-JWT-Extended-4.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:32.353577 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 19:16:32.000000 Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-26 19:16:32.357577 Flask-JWT-Extended-4.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:32.357577 Flask-JWT-Extended-4.5.2/flask_jwt_extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/default_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23923 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/jwt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/flask_jwt_extended/view_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 19:16:32.357577 Flask-JWT-Extended-4.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:32.357577 Flask-JWT-Extended-4.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_add_context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_additional_claims_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_asymmetric_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_blocklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_claims_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19917 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_decode_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_get_jwt_in_non_protected_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_get_methods_in_optional_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_jwt_header_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_multiple_token_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_options_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_query_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_user_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/test_view_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-26 19:16:17.000000 Flask-JWT-Extended-4.5.2/tox.ini
```

### Comparing `Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/PKG-INFO` & `Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-JWT-Extended
-Version: 4.5.1
+Version: 4.5.2
 Summary: Extended JWT integration with Flask
 Home-page: https://github.com/vimalloc/flask-jwt-extended
 Author: Lily Acadia Gilbert
 Author-email: lily.gilbert@hey.com
 License: MIT
 Keywords: flask,jwt,json web token
 Platform: any
```

### Comparing `Flask-JWT-Extended-4.5.1/Flask_JWT_Extended.egg-info/SOURCES.txt` & `Flask-JWT-Extended-4.5.2/Flask_JWT_Extended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/LICENSE` & `Flask-JWT-Extended-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/PKG-INFO` & `Flask-JWT-Extended-4.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-JWT-Extended
-Version: 4.5.1
+Version: 4.5.2
 Summary: Extended JWT integration with Flask
 Home-page: https://github.com/vimalloc/flask-jwt-extended
 Author: Lily Acadia Gilbert
 Author-email: lily.gilbert@hey.com
 License: MIT
 Keywords: flask,jwt,json web token
 Platform: any
```

### Comparing `Flask-JWT-Extended-4.5.1/README.md` & `Flask-JWT-Extended-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/__init__.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 from .utils import set_refresh_cookies as set_refresh_cookies
 from .utils import unset_access_cookies as unset_access_cookies
 from .utils import unset_jwt_cookies as unset_jwt_cookies
 from .utils import unset_refresh_cookies as unset_refresh_cookies
 from .view_decorators import jwt_required as jwt_required
 from .view_decorators import verify_jwt_in_request as verify_jwt_in_request
 
-__version__ = "4.5.1"
+__version__ = "4.5.2"
```

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/config.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/config.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/default_callbacks.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/default_callbacks.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/exceptions.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/internal_utils.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/internal_utils.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/jwt_manager.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/jwt_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/tokens.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/tokens.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/utils.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/utils.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/flask_jwt_extended/view_decorators.py` & `Flask-JWT-Extended-4.5.2/flask_jwt_extended/view_decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/setup.py` & `Flask-JWT-Extended-4.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_add_context_processor.py` & `Flask-JWT-Extended-4.5.2/tests/test_add_context_processor.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_additional_claims_loader.py` & `Flask-JWT-Extended-4.5.2/tests/test_additional_claims_loader.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_asymmetric_crypto.py` & `Flask-JWT-Extended-4.5.2/tests/test_asymmetric_crypto.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_blocklist.py` & `Flask-JWT-Extended-4.5.2/tests/test_blocklist.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_claims_verification.py` & `Flask-JWT-Extended-4.5.2/tests/test_claims_verification.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_config.py` & `Flask-JWT-Extended-4.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_cookies.py` & `Flask-JWT-Extended-4.5.2/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_decode_tokens.py` & `Flask-JWT-Extended-4.5.2/tests/test_decode_tokens.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_get_jwt_in_non_protected_contexts.py` & `Flask-JWT-Extended-4.5.2/tests/test_get_jwt_in_non_protected_contexts.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_get_methods_in_optional_endpoint.py` & `Flask-JWT-Extended-4.5.2/tests/test_get_methods_in_optional_endpoint.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_headers.py` & `Flask-JWT-Extended-4.5.2/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_json.py` & `Flask-JWT-Extended-4.5.2/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_jwt_header_loader.py` & `Flask-JWT-Extended-4.5.2/tests/test_jwt_header_loader.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_multiple_token_locations.py` & `Flask-JWT-Extended-4.5.2/tests/test_multiple_token_locations.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_options_method.py` & `Flask-JWT-Extended-4.5.2/tests/test_options_method.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_query_string.py` & `Flask-JWT-Extended-4.5.2/tests/test_query_string.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_user_lookup.py` & `Flask-JWT-Extended-4.5.2/tests/test_user_lookup.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tests/test_view_decorators.py` & `Flask-JWT-Extended-4.5.2/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-JWT-Extended-4.5.1/tox.ini` & `Flask-JWT-Extended-4.5.2/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 deps = pre-commit
 skip_install = true
 commands = pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
 # This gets color output working when run through tox
 passenv=TERM
-deps =
-  Sphinx
-  Pallets-Sphinx-Themes
+deps = -rdocs/requirements.txt
+#deps =
+#  Sphinx
+#  Pallets-Sphinx-Themes
 changedir = docs
 allowlist_externals = make
 commands =
   make dummy
   make linkcheck
```


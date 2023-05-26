# Comparing `tmp/fastapi_authlib-0.0.1.tar.gz` & `tmp/fastapi_authlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authlib-0.0.1.tar", max compression
+gzip compressed data, was "fastapi_authlib-0.0.2.tar", max compression
```

## Comparing `fastapi_authlib-0.0.1.tar` & `fastapi_authlib-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.1/LICENSE
--rw-r--r--   0        0        0     1809 2023-05-26 01:57:13.116256 fastapi_authlib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3712 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.1/README.md
--rw-r--r--   0        0        0       36 2023-05-26 01:57:13.139770 fastapi_authlib-0.0.1/src/fastapi_authlib/__init__.py
--rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/alembic.ini
--rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/env.py
--rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/README
--rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/script.py.mako
--rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
--rw-r--r--   0        0        0      356 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.1/src/fastapi_authlib/config/__init__.py
--rw-r--r--   0        0        0       11 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.1/src/fastapi_authlib/config/settings.yml
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.1/src/fastapi_authlib/messages/__init__.py
--rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.1/src/fastapi_authlib/messages/base.py
--rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.1/src/fastapi_authlib/messages/user.py
--rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.1/src/fastapi_authlib/models.py
--rw-r--r--   0        0        0     3289 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.1/src/fastapi_authlib/oidc.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/__init__.py
--rw-r--r--   0        0        0     5767 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/base.py
--rw-r--r--   0        0        0      825 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/group.py
--rw-r--r--   0        0        0     1177 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/group_user_map.py
--rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/session.py
--rw-r--r--   0        0        0      365 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.1/src/fastapi_authlib/repository/user.py
--rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/__init__.py
--rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/handler/__init__.py
--rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/handler/exception_handlers.py
--rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/__init__.py
--rw-r--r--   0        0        0      867 2023-05-25 10:40:40.934448 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/login.py
--rw-r--r--   0        0        0      559 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/logout.py
--rw-r--r--   0        0        0      499 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/user.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/__init__.py
--rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/base.py
--rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/group.py
--rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/group_user_map.py
--rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/session.py
--rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/user.py
--rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.1/src/fastapi_authlib/services/__init__.py
--rw-r--r--   0        0        0     9167 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.1/src/fastapi_authlib/services/auth.py
--rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.1/src/fastapi_authlib/services/base.py
--rw-r--r--   0        0        0        0 2023-05-25 09:49:48.774785 fastapi_authlib-0.0.1/src/fastapi_authlib/utils/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-25 10:08:49.119535 fastapi_authlib-0.0.1/src/fastapi_authlib/utils/check_user_depend.py
--rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.1/src/fastapi_authlib/utils/exceptions.py
--rw-r--r--   0        0        0      439 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.1/src/fastapi_authlib/utils/types.py
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.1/setup.py
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-25 09:49:48.758784 fastapi_authlib-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1809 2023-05-26 08:06:01.388930 fastapi_authlib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3702 2023-05-26 02:36:13.115572 fastapi_authlib-0.0.2/README.md
+-rw-r--r--   0        0        0       36 2023-05-26 08:06:01.426754 fastapi_authlib-0.0.2/src/fastapi_authlib/__init__.py
+-rw-r--r--   0        0        0     3313 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/alembic.ini
+-rw-r--r--   0        0        0     2794 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/env.py
+-rw-r--r--   0        0        0       38 2023-05-25 09:49:48.762785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/README
+-rw-r--r--   0        0        0      534 2023-05-25 09:49:48.763786 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/script.py.mako
+-rw-r--r--   0        0        0     3390 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py
+-rw-r--r--   0        0        0      356 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/config/__init__.py
+-rw-r--r--   0        0        0       11 2023-05-25 09:49:48.764785 fastapi_authlib-0.0.2/src/fastapi_authlib/config/settings.yml
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/base.py
+-rw-r--r--   0        0        0      236 2023-05-25 09:49:48.765787 fastapi_authlib-0.0.2/src/fastapi_authlib/messages/user.py
+-rw-r--r--   0        0        0     2906 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.2/src/fastapi_authlib/models.py
+-rw-r--r--   0        0        0     3268 2023-05-26 08:06:03.392694 fastapi_authlib-0.0.2/src/fastapi_authlib/oidc.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.766785 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/__init__.py
+-rw-r--r--   0        0        0     5767 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/base.py
+-rw-r--r--   0        0        0      825 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group.py
+-rw-r--r--   0        0        0     1177 2023-05-25 09:49:48.767786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group_user_map.py
+-rw-r--r--   0        0        0     1121 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/session.py
+-rw-r--r--   0        0        0      365 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/repository/user.py
+-rw-r--r--   0        0        0       23 2023-05-25 09:49:48.768786 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/exception_handlers.py
+-rw-r--r--   0        0        0       13 2023-05-25 09:49:48.769785 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-26 02:01:54.573018 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/login.py
+-rw-r--r--   0        0        0      559 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/logout.py
+-rw-r--r--   0        0        0      499 2023-05-25 09:49:48.770784 fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/user.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/base.py
+-rw-r--r--   0        0        0      504 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group.py
+-rw-r--r--   0        0        0      597 2023-05-25 09:49:48.771784 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group_user_map.py
+-rw-r--r--   0        0        0     1011 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/session.py
+-rw-r--r--   0        0        0      684 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/user.py
+-rw-r--r--   0        0        0      102 2023-05-25 09:49:48.772785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/__init__.py
+-rw-r--r--   0        0        0     9167 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/auth.py
+-rw-r--r--   0        0        0     3882 2023-05-25 09:49:48.773785 fastapi_authlib-0.0.2/src/fastapi_authlib/services/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 09:49:48.774785 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-26 02:32:44.712026 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/check_user_depend.py
+-rw-r--r--   0        0        0      870 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/exceptions.py
+-rw-r--r--   0        0        0      439 2023-05-25 09:49:48.775786 fastapi_authlib-0.0.2/src/fastapi_authlib/utils/types.py
+-rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.2/setup.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 fastapi_authlib-0.0.2/PKG-INFO
```

### Comparing `fastapi_authlib-0.0.1/LICENSE` & `fastapi_authlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/pyproject.toml` & `fastapi_authlib-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-authlib"
-version = "0.0.1"
+version = "0.0.2"
 description = "A fastapi authlib authentication library"
 readme = "README.md"
 authors = ["qiang.xie <qiang.xie@zncdata.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
```

### Comparing `fastapi_authlib-0.0.1/README.md` & `fastapi_authlib-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# fastapi-oidc-support
+# fastapi-authlib
 
-fastapi-oidc-support provides easy integration between FastAPI and openid connection in your application.
+fastapi-authlib provides easy integration between FastAPI and openid connection in your application.
 Provides the initialization and dependencies of oidc, aiming to unify authentication management and
 reduce the difficulty of use.
 
 ## Installing
 
 install and update using pip:
```

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/alembic.ini` & `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/env.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/script.py.mako` & `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/alembic/versions/a55b1fb4f129_init_database.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/models.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/repository/base.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/repository/group.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/repository/group_user_map.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/group_user_map.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/repository/session.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/repository/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/handler/__init__.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/handler/exception_handlers.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/handler/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/login.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/login.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""login"""
-
-from urllib.parse import urlencode
-
-from fastapi import APIRouter, Depends
-from starlette.requests import Request
-from starlette.responses import RedirectResponse
-
-from fastapi_authlib.services import AuthService
-
-router = APIRouter()
-
-
-@router.get('/login')
-async def login(
-    request: Request,
-    service: AuthService = Depends()
-):
-    """
-    Login
-    """
-    redirect_uri = request.url_for('auth')
-    url = f"{str(redirect_uri)}{'?' + urlencode(request.query_params) if request.query_params else ''}"
-    return await service.login(request, url)
-
-
-@router.get('/auth')
-async def auth(
-    callback_url: str,
-    request: Request,
-    service: AuthService = Depends(),
-):
-    """
-    Auth
-    """
-    user = await service.auth(request)
-    request.session.clear()
-    request.session['user'] = user
-    return RedirectResponse(url=callback_url)
+"""login"""
+
+from urllib.parse import urlencode
+
+from fastapi import APIRouter, Depends
+from starlette.requests import Request
+from starlette.responses import RedirectResponse
+
+from fastapi_authlib.services import AuthService
+
+router = APIRouter()
+
+
+@router.get('/login')
+async def login(
+    request: Request,
+    service: AuthService = Depends()
+):
+    """
+    Login
+    """
+    redirect_uri = request.url_for('auth')
+    url = f"{str(redirect_uri)}{'?' + urlencode(request.query_params) if request.query_params else ''}"
+    return await service.login(request, url)
+
+
+@router.get('/auth')
+async def auth(
+    callback_url: str,
+    request: Request,
+    service: AuthService = Depends(),
+):
+    """
+    Auth
+    """
+    user = await service.auth(request)
+    request.session.clear()
+    request.session['user'] = user
+    return RedirectResponse(url=callback_url)
```

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/rest_api/routers/logout.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/rest_api/routers/logout.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/group_user_map.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/group_user_map.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/session.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/session.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/schemas/user.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/services/auth.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/services/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/services/base.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/services/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/src/fastapi_authlib/utils/exceptions.py` & `fastapi_authlib-0.0.2/src/fastapi_authlib/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_authlib-0.0.1/setup.py` & `fastapi_authlib-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,17 @@
  'inflection>=0.5.1,<0.6.0',
  'itsdangerous>=2.1.2,<3.0.0',
  'sqlalchemy==1.4.46',
  'uvicorn>=0.21.1,<0.22.0']
 
 setup_kwargs = {
     'name': 'fastapi-authlib',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'A fastapi authlib authentication library',
-    'long_description': '# fastapi-oidc-support\n\nfastapi-oidc-support provides easy integration between FastAPI and openid connection in your application.\nProvides the initialization and dependencies of oidc, aiming to unify authentication management and\nreduce the difficulty of use.\n\n## Installing\n\ninstall and update using pip:\n\n```shell\npip install fastapi-authlib\n```\n\n## Examples\n\n### Create settings for examples, `settings.py`\n\n```python\nconfig = {\n    \'database\': \'sqlite+aiosqlite:////tmp/oidc_demo.db\',\n    \'oauth_client_id\': \'client_id\',\n    \'oauth_client_secret\': \'client_secret\',\n    \'oauth_conf_url\': \'conf_url\',\n    \'session_secret\': \'secret_key\',\n    \'router_prefix\': \'\',\n}\n```\n\nsettings.py is a simple configuration file of the use case, which mainly provides the database link,\nthe necessary parameters used by oidc, the session authentication key and the routing prefix.\n\nPlease use your authentication server configuration to populate the parameter value prefixed with oauth.\nOther parameters can be modified according to the actual situation.\n\n### Create api route, `api_router.py`\n\n```python\nfrom fastapi import APIRouter\nfrom starlette.requests import Request\n\nrouter = APIRouter()\n\n\n@router.get(\'/index\')\nasync def index(\n        *,\n        request: Request,\n):\n    """\n    User\n    """\n    user_info = request.state.user\n    return {\'name\': user_info.get(\'user_name\')}\n```\n\nFor authenticated api, you can use `request.state.user` to get the current user.\n\n### Create oidc demo entry, `main.py`\n\n```python\n"""main"""\nimport uvicorn\nfrom fastapi import Depends, FastAPI\nfrom fastapi_sa.database import db\nfrom fastapi_sa.middleware import DBSessionMiddleware\n\nfrom fastapi_authlib.oidc import OIDCClient\nfrom fastapi_authlib.utils.check_user_depend import check_auth_session\nfrom api_router import index\nfrom .settings import config\n\n\nclass OIDCDemo:\n    """OIDCDemo"""\n\n    def __init__(self, settings: dict):\n        self.settings = settings\n        self.router_prefix = self.settings.get(\'router_prefix\')\n\n    def run(self):\n        """Run"""\n        # Early environment initialization\n        app = FastAPI(title=\'FastAPIOIDCSupportDemo\', version=\'0.1.0\')\n        db.init(self.settings.get(\'database\'))\n\n        # Oidc environment initialization\n        client = OIDCClient(\n            app=app,\n            **config\n        )\n        # If you only init app, you should use init_app() instead\n        client.init_oidc()\n\n        # Customize the environment initialization\n        # add dependencies to the interface that needs to be authenticated\n        app.include_router(index.router, tags=[\'index\'], prefix=config.get(\'router_prefix\'),\n                           dependencies=[Depends(check_auth_session)])\n        app.add_middleware(DBSessionMiddleware)\n        return app\n\n\nif __name__ == \'__main__\':\n    client_app = OIDCDemo(config).run()\n    uvicorn.run(client_app, host="0.0.0.0", port=8001)\n\n```\n\n### Use Step\n\n- Create app and init db\n- Init the environment of oidc, If you don\'t want to do data migration, you should use init_app method.\n  Usually database migration and oidc initialization are performed together\n- Register routing and other middleware, the DBSessionMiddleware is required\n- Start a fastapi server with uvicorn or other\n\n## Based on\n\n- [FastAPI](https://github.com/tiangolo/fastapi)\n- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)\n- [Fastapi-sa](https://github.com/whg517/fastapi-sa)\n- [Authlib](https://github.com/lepture/authlib)\n\n## Develop\n\nYou may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.\n',
+    'long_description': '# fastapi-authlib\n\nfastapi-authlib provides easy integration between FastAPI and openid connection in your application.\nProvides the initialization and dependencies of oidc, aiming to unify authentication management and\nreduce the difficulty of use.\n\n## Installing\n\ninstall and update using pip:\n\n```shell\npip install fastapi-authlib\n```\n\n## Examples\n\n### Create settings for examples, `settings.py`\n\n```python\nconfig = {\n    \'database\': \'sqlite+aiosqlite:////tmp/oidc_demo.db\',\n    \'oauth_client_id\': \'client_id\',\n    \'oauth_client_secret\': \'client_secret\',\n    \'oauth_conf_url\': \'conf_url\',\n    \'session_secret\': \'secret_key\',\n    \'router_prefix\': \'\',\n}\n```\n\nsettings.py is a simple configuration file of the use case, which mainly provides the database link,\nthe necessary parameters used by oidc, the session authentication key and the routing prefix.\n\nPlease use your authentication server configuration to populate the parameter value prefixed with oauth.\nOther parameters can be modified according to the actual situation.\n\n### Create api route, `api_router.py`\n\n```python\nfrom fastapi import APIRouter\nfrom starlette.requests import Request\n\nrouter = APIRouter()\n\n\n@router.get(\'/index\')\nasync def index(\n        *,\n        request: Request,\n):\n    """\n    User\n    """\n    user_info = request.state.user\n    return {\'name\': user_info.get(\'user_name\')}\n```\n\nFor authenticated api, you can use `request.state.user` to get the current user.\n\n### Create oidc demo entry, `main.py`\n\n```python\n"""main"""\nimport uvicorn\nfrom fastapi import Depends, FastAPI\nfrom fastapi_sa.database import db\nfrom fastapi_sa.middleware import DBSessionMiddleware\n\nfrom fastapi_authlib.oidc import OIDCClient\nfrom fastapi_authlib.utils.check_user_depend import check_auth_session\nfrom api_router import index\nfrom .settings import config\n\n\nclass OIDCDemo:\n    """OIDCDemo"""\n\n    def __init__(self, settings: dict):\n        self.settings = settings\n        self.router_prefix = self.settings.get(\'router_prefix\')\n\n    def run(self):\n        """Run"""\n        # Early environment initialization\n        app = FastAPI(title=\'FastAPIOIDCSupportDemo\', version=\'0.1.0\')\n        db.init(self.settings.get(\'database\'))\n\n        # Oidc environment initialization\n        client = OIDCClient(\n            app=app,\n            **config\n        )\n        # If you only init app, you should use init_app() instead\n        client.init_oidc()\n\n        # Customize the environment initialization\n        # add dependencies to the interface that needs to be authenticated\n        app.include_router(index.router, tags=[\'index\'], prefix=config.get(\'router_prefix\'),\n                           dependencies=[Depends(check_auth_session)])\n        app.add_middleware(DBSessionMiddleware)\n        return app\n\n\nif __name__ == \'__main__\':\n    client_app = OIDCDemo(config).run()\n    uvicorn.run(client_app, host="0.0.0.0", port=8001)\n\n```\n\n### Use Step\n\n- Create app and init db\n- Init the environment of oidc, If you don\'t want to do data migration, you should use init_app method.\n  Usually database migration and oidc initialization are performed together\n- Register routing and other middleware, the DBSessionMiddleware is required\n- Start a fastapi server with uvicorn or other\n\n## Based on\n\n- [FastAPI](https://github.com/tiangolo/fastapi)\n- [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy)\n- [Fastapi-sa](https://github.com/whg517/fastapi-sa)\n- [Authlib](https://github.com/lepture/authlib)\n\n## Develop\n\nYou may need to read the [develop document](./docs/development.md) to use SRC Layout in your IDE.\n',
     'author': 'qiang.xie',
     'author_email': 'qiang.xie@zncdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fastapi_authlib-0.0.1/PKG-INFO` & `fastapi_authlib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-authlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fastapi authlib authentication library
 License: MIT
 Author: qiang.xie
 Author-email: qiang.xie@zncdata.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,17 +21,17 @@
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
 Requires-Dist: sqlalchemy (==1.4.46)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
-# fastapi-oidc-support
+# fastapi-authlib
 
-fastapi-oidc-support provides easy integration between FastAPI and openid connection in your application.
+fastapi-authlib provides easy integration between FastAPI and openid connection in your application.
 Provides the initialization and dependencies of oidc, aiming to unify authentication management and
 reduce the difficulty of use.
 
 ## Installing
 
 install and update using pip:
```


# Comparing `tmp/palantir-oauth-client-1.5.5.tar.gz` & `tmp/palantir-oauth-client-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palantir-oauth-client-1.5.5.tar", max compression
+gzip compressed data, was "palantir-oauth-client-1.5.6.tar", max compression
```

## Comparing `palantir-oauth-client-1.5.5.tar` & `palantir-oauth-client-1.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/LICENSE
--rw-r--r--   0        0        0     3585 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/README.md
--rw-r--r--   0        0        0      928 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/__init__.py
--rw-r--r--   0        0        0     3585 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/_client.py
--rw-r--r--   0        0        0     8217 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/_flow.py
--rw-r--r--   0        0        0     2179 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/_utils.py
--rw-r--r--   0        0        0       22 2023-03-22 13:16:33.444063 palantir-oauth-client-1.5.5/palantir_oauth_client/_version.py
--rw-r--r--   0        0        0     1512 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/_webserver.py
--rw-r--r--   0        0        0    10661 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/auth.py
--rw-r--r--   0        0        0     6354 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/cache.py
--rw-r--r--   0        0        0     7211 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/credentials.py
--rw-r--r--   0        0        0     1095 2023-03-22 13:16:33.288061 palantir-oauth-client-1.5.5/palantir_oauth_client/errors.py
--rw-r--r--   0        0        0      776 2023-03-22 13:16:33.864068 palantir-oauth-client-1.5.5/pyproject.toml
--rw-r--r--   0        0        0     4444 2023-03-22 13:16:34.685058 palantir-oauth-client-1.5.5/setup.py
--rw-r--r--   0        0        0     4339 2023-03-22 13:16:34.685447 palantir-oauth-client-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/LICENSE
+-rw-r--r--   0        0        0     3585 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/README.md
+-rw-r--r--   0        0        0      928 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/__init__.py
+-rw-r--r--   0        0        0     3585 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_client.py
+-rw-r--r--   0        0        0     8217 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_flow.py
+-rw-r--r--   0        0        0     2179 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_utils.py
+-rw-r--r--   0        0        0       22 2023-05-26 07:27:48.483569 palantir-oauth-client-1.5.6/palantir_oauth_client/_version.py
+-rw-r--r--   0        0        0     1512 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/_webserver.py
+-rw-r--r--   0        0        0    10661 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/auth.py
+-rw-r--r--   0        0        0     6354 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/cache.py
+-rw-r--r--   0        0        0     7211 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/credentials.py
+-rw-r--r--   0        0        0     1095 2023-05-26 07:27:48.327569 palantir-oauth-client-1.5.6/palantir_oauth_client/errors.py
+-rw-r--r--   0        0        0      754 2023-05-26 07:27:48.931567 palantir-oauth-client-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4416 2023-05-26 07:27:49.916967 palantir-oauth-client-1.5.6/setup.py
+-rw-r--r--   0        0        0     4297 2023-05-26 07:27:49.917483 palantir-oauth-client-1.5.6/PKG-INFO
```

### Comparing `palantir-oauth-client-1.5.5/LICENSE` & `palantir-oauth-client-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/README.md` & `palantir-oauth-client-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/__init__.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/_client.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/_client.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/_flow.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/_flow.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/_utils.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/_utils.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/_webserver.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/_webserver.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/auth.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/auth.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/cache.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/cache.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/credentials.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/credentials.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/palantir_oauth_client/errors.py` & `palantir-oauth-client-1.5.6/palantir_oauth_client/errors.py`

 * *Files identical despite different names*

### Comparing `palantir-oauth-client-1.5.5/pyproject.toml` & `palantir-oauth-client-1.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "palantir-oauth-client"
-version = "1.5.5"  # placeholder, updated by git describe during publish
+version = "1.5.6" # placeholder, updated by git describe during publish
 description = "OAuth2 client for Palantir Foundry"
 license = "Apache-2.0"
-authors = ["Thomas Powell <tpowell@palantir.com>", "Andrew Higgins <ahiggins@palantir.com>"]
+authors = [
+  "Thomas Powell <tpowell@palantir.com>",
+  "Andrew Higgins <ahiggins@palantir.com>",
+]
 readme = "README.md"
-packages = [{include = "palantir_oauth_client"}]
+packages = [{ include = "palantir_oauth_client" }]
 include = ["palantir_oauth_client/_version.py"]
 homepage = "https://github.com/palantir/palantir-oauth-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 oauthlib = "^3.2.2"
 requests = "^2.28.2"
 requests-oauthlib = "^1.3.1"
-urllib3 = "^1.26.14"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 
 [build-system]
-requires = [
-    "setuptools >= 35.0.2",
-    "poetry-core>=1.0.0"
-]
-build-backend = "poetry.core.masonry.api"
+requires = ["setuptools >= 35.0.2", "poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `palantir-oauth-client-1.5.5/setup.py` & `palantir-oauth-client-1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['oauthlib>=3.2.2,<4.0.0',
  'requests-oauthlib>=1.3.1,<2.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'urllib3>=1.26.14,<2.0.0']
+ 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'palantir-oauth-client',
-    'version': '1.5.5',
+    'version': '1.5.6',
     'description': 'OAuth2 client for Palantir Foundry',
     'long_description': 'Palantir OAuth Client\n==============\n\nA library for performing OAuth2 authentication with Multipass in order to obtain credentials for querying Foundry APIs.\n\nThis library supports two modes of operation for the [Authorization code](https://oauth.net/2/grant-types/authorization-code/)\nOAuth2 flow:\n\n1. Command line prompt: A user will be prompted to navigate to Foundry and enter the resulting ``authorization_code``\n   in their console after successful authentication.\n   \n2. Local webserver: A local webserver will be created to receive the redirect after successful authentication. The token\n   exchange will be performed automatically.\n\nIf the ``offline_access`` scope is specified, the credential will additionally contain a refresh token. When loading\ncached credentials (see below), the refresh token will be used to update invalid or expired credentials. In the case\ncredentials cannot be obtained the user will be prompted to log in as above.\n\nUsage\n-----\nUse the ``palantir_oauth_client.get_user_credentials()`` function to authenticate to Foundry APIs. \n\n```python\nimport requests\nfrom palantir_oauth_client import get_user_credentials\n\nhostname = "127.0.0.1:8080"\nclient_id = "f5496be223e4db85c6a7c99bc5c2d81a"\ncredentials = get_user_credentials(["offline_access"], hostname, client_id)\n\nheaders = {"Authorization": "Bearer " + credentials.token}\nresponse = requests.get(f"https://{hostname}/multipass/api/me", headers=headers)\nprint("Hello, {}!".format(response.json().get("username")))\n```\n\n## Client Registration\n\nA third-party client application needs to have been created in Multipass and the ``client_id`` provided when calling\n``palantir_oauth_client.get_user_credentials()``. This client should be registered as a _Public client_ (native or single-page\napplication) when it is not possible to securely store the ``client_secret``. The library uses the\n[PKCE OAuth2 extension](https://oauth.net/2/pkce/) for all requests regardless of the type of client that has been\nregistered.\n\nThe following redirect URIs should use be specified for each mode of operation:\n\n1. Command line prompt: ``https://<hostname>/multipass/api/oauth2/callback``\n\n2. Local webserver: ``http://127.0.0.1/``\n\n## Caching\n\nWhen obtaining credentials using ``palantir_oauth_client.get_user_credentials()`` you may specify a\n``palantir_oauth_client.cache.CredentialsCache``. There are three implementations:\n\n1. ``palantir_oauth_client.cache.READ_WRITE`` (default): A read-write cache that will persist credentials to disk when\n   ``offline_access`` scope is requested. The cached refresh tokens will be used when obtaining credentials where\n   possible to avoid explicit re-authentication.\n   \n2. ``palantir_oauth_client.cache.REAUTH``: A write-only cache that will persist credentials to disk when ``offline_access``\n   scope is requested but will require reauthentication when obtaining credentials.\n   \n3. ``palantir_oauth_client.cache.NOOP``: Always requires reauthentication and never persists credentials to disk.\n\nPersisted credentials will be stored in the default user home directory at ``~/.foundry/oauth``. Caching should\nonly be used when this home directory is secure and inaccessible by other users who would not otherwise have access to\nthe Foundry credentials.\n\n## Contributing\n\nSee the [CONTRIBUTING.md](./CONTRIBUTING.md) document. Releases are published to [pypi](https://pypi.org/project/palantir-oauth-client/) on tag builds and are automatically re-published to conda using conda-forge.\n\n## License\nThis project is made available under the [Apache 2.0 License](/LICENSE).\n',
     'author': 'Thomas Powell',
     'author_email': 'tpowell@palantir.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/palantir/palantir-oauth-client',
```

### Comparing `palantir-oauth-client-1.5.5/PKG-INFO` & `palantir-oauth-client-1.5.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: palantir-oauth-client
-Version: 1.5.5
+Version: 1.5.6
 Summary: OAuth2 client for Palantir Foundry
 Home-page: https://github.com/palantir/palantir-oauth-client
 License: Apache-2.0
 Author: Thomas Powell
 Author-email: tpowell@palantir.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
-Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Description-Content-Type: text/markdown
 
 Palantir OAuth Client
 ==============
 
 A library for performing OAuth2 authentication with Multipass in order to obtain credentials for querying Foundry APIs.
```


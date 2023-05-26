# Comparing `tmp/revproxy_auth-0.1.5.tar.gz` & `tmp/revproxy_auth-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.5.tar", last modified: Thu May 25 08:06:59 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.6.tar", last modified: Fri May 26 11:53:09 2023, max compression
```

## Comparing `revproxy_auth-0.1.5.tar` & `revproxy_auth-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-25 08:06:58.000000 revproxy_auth-0.1.5/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 08:06:58.000000 revproxy_auth-0.1.5/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:06:58.000000 revproxy_auth-0.1.5/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 08:06:58.000000 revproxy_auth-0.1.5/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 08:06:58.000000 revproxy_auth-0.1.5/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:06:59.020456 revproxy_auth-0.1.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-25 08:06:49.000000 revproxy_auth-0.1.5/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.917979 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.5/PKG-INFO` & `revproxy_auth-0.1.6/revproxy_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: revproxy_auth
-Version: 0.1.5
+Name: revproxy-auth
+Version: 0.1.6
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.5/README.md` & `revproxy_auth-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.5/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.6/revproxy_auth/revproxy_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     def get_auth_response(self, req, callback) -> Response:
         """ If valid auth token comes fromt he client, return none
             Otherwise, it will return a response so that the client opens again the Auth Popup
         Returns:
             Response: Http response with the auth popup, or 
                       None if auth request is not needed because already are authenticated
         """
+        self.logger.debug(f'Request from host --> {req.host} | endpoint --> {req.path}')
+
         response = None
 
         if req.form.get('revproxy_auth', None):
             session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
             if session_cookie_name:
                 self.logger.info('Credentials validated.')
                 # To get rid of the POST form data, and reenter with the valid session token
@@ -247,15 +249,15 @@
                              timeout=10)
         return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
     def _reask_credentials(self, req: Request, old_cookie_name: str = None) -> Response:
         new_cookie, new_cookie_name = self._build_auth_cookie(req)
         if not new_cookie: # Unable to build cookie for requested path: host unknown
             return Response(f'Host {req.host} not found on revproxy_auth config translation table',
-                            status=HTTP_501_NOT_IMPLEMENTED, 
+                            status=HTTP_501_NOT_IMPLEMENTED,
                             content_type='text/plain')
         self.logger.info(f'Creating new auth cookie {new_cookie_name} and reasking to user...')
         self._write_cookie(new_cookie, self.auth_cookie_folder, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
         if old_cookie_name:
             self.logger.info(f'Deleting cookie in response: {old_cookie_name}')
             self._clear_local_cookie(self.auth_cookie_folder, old_cookie_name)
@@ -268,40 +270,48 @@
 
         Returns:
             Tuple(dict, str): Dict with the new session cookie created (None if credentials invalid or not found)
                               str with the name of the session cookie created
         """
         session_cookie_name = None
         session_cookie = None
-        cookie_name = req.form.get('revproxy_auth', None)
-        auth_cookie = self._get_local_auth_cookie(cookie_name)
+        auth_cookie_name = req.form.get('revproxy_auth', None)
+        auth_cookie = self._get_local_auth_cookie(auth_cookie_name)
         if auth_cookie:
             if self._credentials_valid(req.form):
-                self.logger.info(f'Auth Local cookie {cookie_name} still alive and valid.')
+                self.logger.info(f'Auth Local cookie {auth_cookie_name} still alive and valid.')
                 session_cookie, session_cookie_name = self._build_session_cookie(auth_cookie)
                 self.logger.info(f'Creating new session cookie {session_cookie_name}...')
                 self._write_cookie(session_cookie, self.session_cookie_folder, session_cookie_name)
             else:
-                self.logger.info(f'Auth Local cookie {cookie_name} still alive but credentials are invalid.')
+                self.logger.info(f'Auth Local cookie {auth_cookie_name} still alive but credentials are invalid.')
+            # Auth token can only be used once.
+            self._clear_local_cookie(self.auth_cookie_folder, auth_cookie_name)
         else:
-            self.logger.info(f'Auth Local cookie {cookie_name} doesnt exist.')
+            self.logger.info(f'Auth Local cookie {auth_cookie_name} doesnt exist.')
         return session_cookie, session_cookie_name
 
     def _first_auth_and_redirect(self, req: Request) -> Response:
         cookie_name = req.form.get('revproxy_auth', None)
         cookie = self._get_local_auth_cookie(cookie_name)
         if cookie:
             self.logger.info(f'Local cookie {cookie_name} still alive')
             if self._credentials_valid(req.form):
                 self.logger.info('Credentials validated.')
                 # Search for the cookie and redirect to related URL if present
                 if cookie['method'] == 'GET':
-                    response = self._call_inner_get(cookie['host'], cookie['endpoint'], cookie['params'], cookie['headers'])
+                    response = self._call_inner_get(cookie['host'],
+                                                    cookie['endpoint'],
+                                                    cookie['params'],
+                                                    cookie['headers'])
                 else:
-                    response = self._call_inner_post(cookie['host'], cookie['endpoint'], cookie['content'], cookie['headers'])
+                    response = self._call_inner_post(cookie['host'],
+                                                     cookie['endpoint'],
+                                                     cookie['content'],
+                                                     cookie['headers'])
                 response.set_cookie('token', cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else: # We come from the auth popup, but credentials are invalid --> ask again for credentials
                 self.logger.info('Credentials rejected. Reopening auth popup')
                 response = self._build_auth_popup(cookie_name)
         else: # We got a token, but its no longer valid --> ask again for credentials
             self.logger.info('Local cookie expired. Reopening auth popup')
             response = self._reask_credentials(req, cookie_name)
@@ -328,17 +338,21 @@
             return self._get_static_content(req.path)
 
         if req.form.get('revproxy_auth', None):
             session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
             if session_cookie_name:
                 self.logger.info('Credentials validated by synology NAS')
                 if session_cookie['method'] == 'GET':
-                    response = self._call_inner_get(session_cookie['host'], session_cookie['endpoint'], session_cookie['params'], {})
+                    response = self._call_inner_get(session_cookie['host'],
+                                                    session_cookie['endpoint'],
+                                                    session_cookie['params'], {})
                 else:
-                    response = self._call_inner_post(session_cookie['host'], session_cookie['endpoint'], session_cookie['content'], {})
+                    response = self._call_inner_post(session_cookie['host'],
+                                                     session_cookie['endpoint'],
+                                                     session_cookie['content'], {})
                 # # To get rid of the POST form data, and reenter with the valid session token
                 # response = redirect(session_cookie['endpoint'])
                 response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else:
                 response = self._reask_credentials(req)
         else:
             # Try to get authentication from the cookie
@@ -370,9 +384,9 @@
                     else:
                         response = self._call_inner_post(cookie['host'], path, data, headers)
                 else: # We got a session, but its no longer valid --> ask again for credentials
                     self.logger.debug(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
                     response = self._reask_credentials(req, old_cookie_name=cookie_name)
             else:  # No session cookie... and no form data with credendials
                 response = self._reask_credentials(req)
-      
+
         return response
```

### Comparing `revproxy_auth-0.1.5/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.5/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.6/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.5/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: revproxy-auth
-Version: 0.1.5
+Name: revproxy_auth
+Version: 0.1.6
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.5/setup.py` & `revproxy_auth-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.1.5",
+    version="0.1.6",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
```

### Comparing `revproxy_auth-0.1.5/tests/test_000.py` & `revproxy_auth-0.1.6/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.5/tests/test_001.py` & `revproxy_auth-0.1.6/tests/test_001.py`

 * *Files identical despite different names*


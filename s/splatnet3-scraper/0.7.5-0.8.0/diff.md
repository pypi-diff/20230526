# Comparing `tmp/splatnet3_scraper-0.7.5.tar.gz` & `tmp/splatnet3_scraper-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splatnet3_scraper-0.7.5.tar", max compression
+gzip compressed data, was "splatnet3_scraper-0.8.0.tar", max compression
```

## Comparing `splatnet3_scraper-0.7.5.tar` & `splatnet3_scraper-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.7.5/LICENSE.md
--rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.245111 splatnet3_scraper-0.7.5/README.md
--rw-r--r--   0        0        0     1916 2023-04-16 07:20:32.988479 splatnet3_scraper-0.7.5/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-16 07:20:32.988479 splatnet3_scraper-0.7.5/splatnet3_scraper/__init__.py
--rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/__init__.py
--rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/environment_manager.py
--rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/exceptions.py
--rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.106500 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/graph_ql_queries.py
--rw-r--r--   0        0        0    41667 2023-04-14 23:55:14.106500 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/nso.py
--rw-r--r--   0        0        0    28908 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/auth/token_manager.py
--rw-r--r--   0        0        0     7847 2023-04-14 23:55:14.106500 splatnet3_scraper-0.7.5/splatnet3_scraper/constants.py
--rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/query/__init__.py
--rw-r--r--   0        0        0    13307 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/query/config.py
--rw-r--r--   0        0        0    16840 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.5/splatnet3_scraper/query/handler.py
--rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.5/splatnet3_scraper/query/json_parser.py
--rw-r--r--   0        0        0    26227 2023-04-16 07:20:32.988479 splatnet3_scraper-0.7.5/splatnet3_scraper/query/responses.py
--rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.5/splatnet3_scraper/scraper/__init__.py
--rw-r--r--   0        0        0     9382 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.5/splatnet3_scraper/scraper/main.py
--rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.7.5/splatnet3_scraper/scraper/query_map.py
--rw-r--r--   0        0        0    18732 2023-04-16 03:44:19.509582 splatnet3_scraper-0.7.5/splatnet3_scraper/utils.py
--rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.7.5/setup.py
--rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0    10984 2023-04-15 00:47:42.245111 splatnet3_scraper-0.8.0/README.md
+-rw-r--r--   0        0        0     1916 2023-05-25 23:35:06.235602 splatnet3_scraper-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-26 01:54:11.649921 splatnet3_scraper-0.8.0/splatnet3_scraper/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/environment_manager.py
+-rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/exceptions.py
+-rw-r--r--   0        0        0    10032 2023-04-14 23:55:14.106500 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/graph_ql_queries.py
+-rw-r--r--   0        0        0    44111 2023-05-26 02:08:31.401413 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/nso.py
+-rw-r--r--   0        0        0    28908 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/auth/token_manager.py
+-rw-r--r--   0        0        0     7847 2023-05-25 23:34:03.272956 splatnet3_scraper-0.8.0/splatnet3_scraper/constants.py
+-rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/query/__init__.py
+-rw-r--r--   0        0        0    13307 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/query/config.py
+-rw-r--r--   0        0        0    16840 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.0/splatnet3_scraper/query/handler.py
+-rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.0/splatnet3_scraper/query/json_parser.py
+-rw-r--r--   0        0        0    26227 2023-04-16 07:20:32.988479 splatnet3_scraper-0.8.0/splatnet3_scraper/query/responses.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.8.0/splatnet3_scraper/scraper/__init__.py
+-rw-r--r--   0        0        0     9382 2023-04-10 05:20:16.704543 splatnet3_scraper-0.8.0/splatnet3_scraper/scraper/main.py
+-rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.8.0/splatnet3_scraper/scraper/query_map.py
+-rw-r--r--   0        0        0    18732 2023-04-16 03:44:19.509582 splatnet3_scraper-0.8.0/splatnet3_scraper/utils.py
+-rw-r--r--   0        0        0    12156 1970-01-01 00:00:00.000000 splatnet3_scraper-0.8.0/setup.py
+-rw-r--r--   0        0        0    11882 1970-01-01 00:00:00.000000 splatnet3_scraper-0.8.0/PKG-INFO
```

### Comparing `splatnet3_scraper-0.7.5/LICENSE.md` & `splatnet3_scraper-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/README.md` & `splatnet3_scraper-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/pyproject.toml` & `splatnet3_scraper-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splatnet3_scraper"
-version = "0.7.5"
+version = "0.8.0"
 description = "Scraper for SplatNet 3 for Splatoon 3"
 authors = ["Cesar E Garza <cesar@cegarza.com>"]
 readme = "README.md"
 packages = [{include = "splatnet3_scraper"}]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
```

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/auth/environment_manager.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/auth/environment_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/auth/graph_ql_queries.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/auth/graph_ql_queries.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/auth/nso.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/auth/nso.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import base64
 import hashlib
-import json
 import logging
 import os
 import re
 from typing import Callable, Literal, TypeAlias, cast
 
 import requests
 
@@ -25,15 +24,16 @@
 from splatnet3_scraper.utils import get_splatnet_version, retry
 
 version_re = re.compile(
     r"(?<=whats\-new\_\_latest\_\_version\"\>Version)\s+\d+\.\d+\.\d+"
 )
 
 FToken_Gen: TypeAlias = Callable[
-    [str, str, Literal[1] | Literal[2]], tuple[str, str, str]
+    [str, str, Literal[1] | Literal[2], str, str | None],
+    tuple[str, str, str],
 ]
 
 
 class NSO:
     """The NSO class contains all the logic to proceed through the login flow.
     This class also holds various properties that are used to make requests to
     the Nintendo Switch Online API. Login flow is roughly as follows, assuming
@@ -138,14 +138,16 @@
         self._state: bytes | None = None
         self._verifier: bytes | None = None
         self._version: str | None = None
         self._web_view_version: str | None = None
         self._session_token: str | None = None
         self._user_access_token: str | None = None
         self._id_token: str | None = None
+        self._nintendo_account_id: str | None = None
+        self._coral_user_id: str | None = None
         self._gtoken: str | None = None
         self._user_info: dict[str, str] | None = None
         self._f_token_function: FToken_Gen = self.get_ftoken
 
     @staticmethod
     def new_instance() -> "NSO":
         """Creates a new instance of the NSO class with a new requests session.
@@ -492,21 +494,32 @@
                 "Failed to get user access token. "
                 + f"Response: {user_access_response}"
             )
 
         logging.info("Getting user info")
         user_info = self.get_user_info(self._user_access_token)
         self._user_info = user_info
+        self._nintendo_account_id = user_info["id"]
         logging.info("Getting Web Service Access Token")
-        web_service_access_token = self.g_token_generation_phase_1(
-            self._id_token, user_info, f_token_url
+        (
+            web_service_access_token,
+            coral_user_id,
+        ) = self.g_token_generation_phase_1(
+            self._id_token,
+            user_info,
+            self._nintendo_account_id,
+            f_token_url=f_token_url,
         )
         logging.info("Getting gtoken")
+        self._coral_user_id = coral_user_id
         gtoken = self.g_token_generation_phase_2(
-            web_service_access_token, f_token_url
+            web_service_access_token,
+            self._nintendo_account_id,
+            self._coral_user_id,
+            f_token_url=f_token_url,
         )
         self._gtoken = gtoken
         return gtoken
 
     def set_new_f_token_function(
         self, new_function: FToken_Gen | None = None
     ) -> None:
@@ -548,15 +561,20 @@
             logging.info("Restoring default ftoken generation method")
             self._f_token_function = self.get_ftoken
         else:
             logging.info("Setting new ftoken generation method")
             self._f_token_function = new_function
 
     def get_ftoken(
-        self, f_token_url: str, id_token: str, step: Literal[1] | Literal[2]
+        self,
+        f_token_url: str,
+        id_token: str,
+        step: Literal[1] | Literal[2],
+        na_id: str,
+        coral_user_id: str | None = None,
     ) -> tuple[str, str, str]:
         """Given the ``f_token_url``, ``id_token``, and ``step``, returns the
         ``f_token``, ``request_id``, and ``timestamp`` from the response.
 
         Note that this is a third party method, and is not officially
         sanctioned by Nintendo. The default ftoken generation URL used by this
         library is provided by `imink <https://github.com/imink-app>`_. In
@@ -589,34 +607,53 @@
                 obtained from the user access token response, and is used to
                 identify the user. This cannot be used to identify the user
                 without the user's access token, which is not provided to the
                 ftoken generation URL.
             step (Literal[1] | Literal[2]): The step number. This is either
                 ``1`` or ``2``. This is used to identify the step in the
                 ``f_token`` generation process.
+            na_id (str): The Nintendo Account ID of the user. As of version
+                2.5.1, this is not used for anything. However, it is still
+                required to futureproof in case Nintendo decides to enforce
+                verification of this value.
+            coral_user_id (str | None): The Coral user ID of the user. This is
+                used to verify the ftoken generation process. This is only
+                required for step ``2``.
 
         Raises:
+            ValueError: In the case that the ``coral_user_id`` is not provided
+                for step ``2``.
             FTokenException: In the case that the ftoken cannot be obtained
                 from the ftoken generation URL.
 
         Returns:
             str: The f token.
             str: The request ID.
             str: The timestamp.
         """
         header = {
             "User-Agent": f"splatnet3_scraper/{__version__}",
             "Content-Type": "application/json; charset=utf-8",
+            "X-znca-Platform": "Android",
+            "X-znca-Version": self.version,
         }
         body = {
             "token": id_token,
             "hash_method": step,
+            "na_id": na_id,
         }
-        bodystr = json.dumps(body)
-        response = self.session.post(f_token_url, headers=header, data=bodystr)
+
+        if coral_user_id is not None:
+            body["coral_user_id"] = coral_user_id
+        elif step == 2:
+            raise ValueError(
+                "Coral user ID is required for step 2 of ftoken generation"
+            )
+
+        response = self.session.post(f_token_url, headers=header, json=body)
         response_json = response.json()
         try:
             f_token = response_json["f"]
             request_id = response_json["request_id"]
             timestamp = response_json["timestamp"]
         except (KeyError, TypeError, AttributeError):
             raise FTokenException(
@@ -625,16 +662,17 @@
         return (f_token, request_id, timestamp)
 
     @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
     def g_token_generation_phase_1(
         self,
         id_token: str,
         user_info: dict[str, str],
+        na_id: str,
         f_token_url: str,
-    ) -> str:
+    ) -> tuple[str, str]:
         """First phase of the ``gtoken`` generation process.
 
         This is the first phase of the ``gtoken`` generation process. This is
         abstracted away into a separate method to allow the request to be
         retried once in the event of a failure. This phase involves two steps:
         first, the ``id_token`` is sent to the ``f_token_url`` in a request to
         obtain the ``f_token``, which is a ``HMAC`` necessary to obtain the
@@ -647,32 +685,39 @@
             id_token (str): ID token from user access token response. This is
                 obtained from the user access token response, and is used to
                 identify the user to Nintendo's servers. However, this cannot
                 be used to identify the user by a third party by itself.
             user_info (dict[str, str]): The dictionary of user info returned by
                 ``get_user_info``. This must contain the keys ``language``,
                 ``birthday``, and ``country``.
+            na_id (str): The Nintendo Account ID of the user. As of version
+                2.5.1, this is not used for anything. However, it is still
+                required to futureproof in case Nintendo decides to enforce
+                verification of this value.
             f_token_url (str): URL to use for f token generation. This package
                 provides a default URL, but you can provide your own. The
                 default URL is provided by `imink`.
 
         Returns:
             str: The Web Service Credential Access Token.
+            str: The Coral user ID.
         """
         f_token, request_id, timestamp = self._f_token_function(
-            f_token_url, id_token, 1
+            f_token_url, id_token, 1, na_id, None
         )
         return self.get_web_service_access_token(
             id_token, user_info, f_token, request_id, timestamp
         )
 
     @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
     def g_token_generation_phase_2(
         self,
         web_service_access_token: str,
+        na_id: str,
+        coral_user_id: str,
         f_token_url: str,
     ) -> str:
         """Final phase of the ``gtoken`` generation process.
 
         This is the second phase of the ``gtoken`` generation process. This is
         abstracted away into a separate method to allow the request to be
         retried once in the event of a failure. This phase involves two steps:
@@ -683,37 +728,44 @@
         then sent to Nintendo's servers along with the
         ``web_service_access_token`` to obtain the ``gtoken``.
 
         Args:
             web_service_access_token (str): The Web Service Credential Access
                 Token obtained from the first half of the gtoken generation
                 process.
+            na_id (str): The Nintendo Account ID of the user. As of version
+                2.5.1, this is not used for anything. However, it is still
+                required to futureproof in case Nintendo decides to enforce
+                verification of this value.
+            coral_user_id (str): The Coral user ID of the user. This is
+                used to verify the ftoken generation process. This is only
+                required for step ``2``.
             f_token_url (str): URL to use for f token generation. This package
                 provides a default URL, but you can provide your own. The
                 default URL is provided by `imink`.
 
         Returns:
             str: The gtoken from the response.
         """
         f_token, request_id, timestamp = self._f_token_function(
-            f_token_url, web_service_access_token, 2
+            f_token_url, web_service_access_token, 2, na_id, coral_user_id
         )
 
         return self.get_gtoken_request(
             web_service_access_token, f_token, request_id, timestamp
         )
 
     def get_web_service_access_token(
         self,
         id_token: str,
         user_info: dict[str, str],
         f_token: str,
         request_id: str,
         timestamp: str,
-    ) -> str:
+    ) -> tuple[str, str]:
         """Given the ``id_token``, user data, ``f_token``, ``request_id``, and
         ``timestamp``, returns the Web Service Credential Access Token.
 
         This is the first step of the ``gtoken`` generation process. This will
         return the Web Service Credential Access Token from Nintendo's servers,
         which is then used to obtain the ``gtoken``.
 
@@ -728,14 +780,15 @@
             request_id (str): The ``request_id`` returned alongside the
                 ``f_token`` and ``timestamp``.
             timestamp (str): The ``timestamp`` returned alongside the
                 ``f_token`` and ``request_id``.
 
         Returns:
             str: The Web Service Credential Access Token.
+            str: The coral user ID.
         """
         header = {
             "X-Platform": "Android",
             "X-ProductVersion": self.version,
             "Content-Type": "application/json; charset=utf-8",
             "Content-Length": str(990 + len(f_token)),
             "Connection": "Keep-Alive",
@@ -753,15 +806,19 @@
                 "naIdToken": id_token,
                 "requestId": request_id,
                 "timestamp": timestamp,
             }
         }
         url = "https://api-lp1.znc.srv.nintendo.net/v3/Account/Login"
         response = self.session.post(url, headers=header, json=body).json()
-        return response["result"]["webApiServerCredential"]["accessToken"]
+        response_result = response["result"]
+        return (
+            response_result["webApiServerCredential"]["accessToken"],
+            response_result["user"]["id"],
+        )
 
     def get_gtoken_request(
         self,
         web_service_access_token: str,
         f_token: str,
         request_id: str,
         timestamp: str,
```

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/auth/token_manager.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/auth/token_manager.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/constants.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 000001f0: 2f39 342e 302e 3436 3036 2e36 3120 220a  /94.0.4606.61 ".
 00000200: 2020 2020 2b20 224d 6f62 696c 6520 5361      + "Mobile Sa
 00000210: 6661 7269 2f35 3337 2e33 3622 0a29 0a57  fari/537.36".).W
 00000220: 4542 5f56 4945 575f 5645 5253 494f 4e5f  EB_VIEW_VERSION_
 00000230: 4641 4c4c 4241 434b 203d 2022 332e 302e  FALLBACK = "3.0.
 00000240: 302d 3037 3432 6264 6130 220a 4150 505f  0-0742bda0".APP_
 00000250: 5645 5253 494f 4e5f 4641 4c4c 4241 434b  VERSION_FALLBACK
-00000260: 203d 2022 322e 352e 3022 0a48 4153 4845   = "2.5.0".HASHE
+00000260: 203d 2022 322e 352e 3122 0a48 4153 4845   = "2.5.1".HASHE
 00000270: 535f 4641 4c4c 4241 434b 203d 207b 0a20  S_FALLBACK = {. 
 00000280: 2020 2022 4261 6e6b 6172 6142 6174 746c     "BankaraBattl
 00000290: 6548 6973 746f 7269 6573 5175 6572 7922  eHistoriesQuery"
 000002a0: 3a20 2230 3433 3865 6136 3937 3861 6538  : "0438ea6978ae8
 000002b0: 6264 3737 6335 6431 3235 3066 3466 3834  bd77c5d1250f4f84
 000002c0: 3830 3322 2c0a 2020 2020 2242 616e 6b61  803",.    "Banka
 000002d0: 7261 4261 7474 6c65 4869 7374 6f72 6965  raBattleHistorie
```

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/query/config.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/query/config.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/query/handler.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/query/handler.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/query/json_parser.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/query/json_parser.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/query/responses.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/query/responses.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/scraper/main.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/scraper/main.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/scraper/query_map.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/scraper/query_map.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/splatnet3_scraper/utils.py` & `splatnet3_scraper-0.8.0/splatnet3_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `splatnet3_scraper-0.7.5/setup.py` & `splatnet3_scraper-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'examples': ['pandas[examples]>=1.5.3,<2.0.0',
               'sqlalchemy[examples]>=2.0.1,<3.0.0',
               'psycopg2[examples]>=2.9.5,<3.0.0'],
  'parquet': ['pyarrow[parquet]>=10.0.1,<11.0.0']}
 
 setup_kwargs = {
     'name': 'splatnet3-scraper',
-    'version': '0.7.5',
+    'version': '0.8.0',
     'description': 'Scraper for SplatNet 3 for Splatoon 3',
     'long_description': '# SplatNet 3 Scraper\n\n[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.\n\n**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.\n\n## Table of Contents\n\n1. [Features](#features)\n2. [Documentation](#documentation)\n3. [Installation](#installation)\n4. [Usage](#usage)\n   - [Using the `scraper` module](#using-the-scraper-module)\n   - [Using the `query` module](#using-the-query-module)\n   - [Using the `auth` module](#using-the-auth-module)\n5. [Roadmap](#roadmap)\n6. [Contributing](#contributing)\n7. [License](#license)\n\n## Features\n\n- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.\n- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.\n- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.\n- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.\n- Compatibility with the configuration file format used by `s3s`.\n- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:\n  - JSON\n  - gzip-compressed JSON\n  - csv\n  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).\n\n## Documentation\n\nDetailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:\n\n[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)\n\nWe highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.\n\n## Installation\n\n**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:\n\n```bash\npip install splatnet3_scraper\n```\n\nNote that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.\n\n## Usage\n\nThere are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can\'t find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.\n\n### Using the `scraper` module\n\nThe `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.\n\nThis module is currently under active development and is not yet complete. Please check back later for more functions.\n\n### Using the `query` module\n\nThe `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.\n\nThe `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.\n\n### Using the `auth` module\n\n:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**\n\nThe `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.\n\nTo use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.\n\n#### Instantiating the `QueryHandler` class by providing a session token\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_session_token("session_token")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by providing the path to a configuration file\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_config_file(".splatnet3_scraper")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by loading environment variables\n\nThe following environment variables are supported:\n\n- `SN3S_SESSION_TOKEN`\n- `SN3S_GTOKEN`\n- `SN3S_BULLET_TOKEN`\n\n```python\nfrom splatnet3_scrape.query import QueryHandler\nhandler = QueryHandler.from_env()\nhandler.query("StageScheduleQuery")\n```\n\n#### Querying the SplatNet 3 API\n\nThe `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nprint(response["xSchedules", "nodes", 0, "vsRule", "name"])\n```\n\n#### Saving and loading responses\n\nThe `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:\n\n- JSON\n- gzip-compressed JSON\n- csv\n- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n\nNote: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.\n\nThe following code will save the response data to a file named `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nresponse.parsed_json().to_json("response.json")\n```\n\nAdditionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import JSONParser\nparser = JSONParser.from_json("response.json")\n```\n\n## Symbols\n\n| Symbol | Meaning |\n| ------ | ------- |\n| :white_check_mark: | Implemented |\n| :construction: | In progress |\n| :world_map: | Planned |\n| :x: | Not planned |\n\n## Roadmap\n\n| Feature | Status |\n| ------- | ------ |\n| Support for the SplatNet 3 API | :white_check_mark: |\n| Full support for the SplatNet 3 API | :white_check_mark: |\n| Support for the SplatNet 2 API | :x: |\n| Obtaining session tokens | :white_check_mark: |\n| Full documentation | :white_check_mark: |\n| Full unit test coverage | :white_check_mark: |\n| Columnar data format support | :construction: |\n| CLI interface | :x: |\n| Integration with stat.ink | :x: |\n| PyPI package | :white_check_mark: |\n| Docker image | :world_map: |\n| Executable binary | :x: |\n\n## Contributing\n\nWe welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.\n\nTo report issues or request new features, please open an issue on the GitHub repository.\n\n## License\n\nSplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.\n',
     'author': 'Cesar E Garza',
     'author_email': 'cesar@cegarza.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `splatnet3_scraper-0.7.5/PKG-INFO` & `splatnet3_scraper-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splatnet3-scraper
-Version: 0.7.5
+Version: 0.8.0
 Summary: Scraper for SplatNet 3 for Splatoon 3
 License: GPL-3.0-or-later
 Author: Cesar E Garza
 Author-email: cesar@cegarza.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


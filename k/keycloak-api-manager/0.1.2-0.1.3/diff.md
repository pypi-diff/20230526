# Comparing `tmp/keycloak_api_manager-0.1.2.tar.gz` & `tmp/keycloak_api_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_api_manager-0.1.2.tar", last modified: Thu May 25 13:56:37 2023, max compression
+gzip compressed data, was "keycloak_api_manager-0.1.3.tar", last modified: Fri May 26 08:27:58 2023, max compression
```

## Comparing `keycloak_api_manager-0.1.2.tar` & `keycloak_api_manager-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:56:37.566889 keycloak_api_manager-0.1.2/
--rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2729 2023-05-25 13:56:37.566229 keycloak_api_manager-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2023-05-25 13:51:19.000000 keycloak_api_manager-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:56:37.530281 keycloak_api_manager-0.1.2/keycloak_api_manager/
--rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-0.1.2/keycloak_api_manager/__init__.py
--rw-rw-rw-   0        0        0     8348 2023-05-25 13:20:04.000000 keycloak_api_manager-0.1.2/keycloak_api_manager/keycloak_api_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:56:37.564296 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/
--rw-rw-rw-   0        0        0     2729 2023-05-25 13:56:37.000000 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-25 13:56:37.000000 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:56:37.000000 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 13:56:37.000000 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-25 13:56:37.000000 keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      920 2023-05-25 13:55:23.000000 keycloak_api_manager-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 13:56:37.566889 keycloak_api_manager-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.978978 keycloak_api_manager-0.1.3/
+-rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2935 2023-05-26 08:27:58.977199 keycloak_api_manager-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-05-26 08:25:03.000000 keycloak_api_manager-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.937004 keycloak_api_manager-0.1.3/keycloak_api_manager/
+-rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-0.1.3/keycloak_api_manager/__init__.py
+-rw-rw-rw-   0        0        0     8346 2023-05-26 08:17:40.000000 keycloak_api_manager-0.1.3/keycloak_api_manager/keycloak_api_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.974217 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/
+-rw-rw-rw-   0        0        0     2935 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      825 2023-05-26 08:25:34.000000 keycloak_api_manager-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 08:27:58.979228 keycloak_api_manager-0.1.3/setup.cfg
```

### Comparing `keycloak_api_manager-0.1.2/LICENSE.txt` & `keycloak_api_manager-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-0.1.2/PKG-INFO` & `keycloak_api_manager-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: keycloak_api_manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
-Project-URL: Changelog, https://github.com/martinlauren55/keycloak-api-manager/blob/main/CHANGELOG.md
 Keywords: keycloak,API,keycloak API management
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -24,37 +23,46 @@
 **REALM_NAME** = "realm_name" <br/>
 **CLIENT_SECRET** = "40j32-5860-4d79-ad16-9c39897w083" <br/>
 **USERNAME** = "username@gmail.com"   - User name with admin's rules <br/> 
 **PASSWORD** = "f232@3s456S#422" <br/>
 **SERVER_URL** = "http://localhost:8080/auth/" - url keykcloak server <br/>
 <br/>
 
-## Quickstart
 
-Create a file **keycloak_test.py** with:
+# Installation
 
+```pip install keycloak-api-manager```
+
+# Example
+### Create it
+Create a file ```main.py``` with:
 ```
 from keycloak_api_manager import KeycloakAPIManager
 
 CLIENT_ID = "test_client_name"
 REALM_NAME = "realm_name"
 CLIENT_SECRET = "40j32-5860-4d79-ad16-9c39897w083"
-USERNAME = 'username@gmail.com'
+USERNAME = 'username@gmail.com'                         # KEYCLOAK user's USERNAME or EMAIL User with admin's
 PASSWORD = 'f232@3s456S#422'
-SERVER_URL = "http://localhost:8080/auth/"
+SERVER_URL = "http://localhost:8080/auth/"              # KEYCLOAK URL http://localhost:8080/auth/ or
+                                                        # http://server_url/auth/
 
 
 keycloak_api = KeycloakAPIManager(keycloak_url=SERVER_URL, realm_name=REALM_NAME,
                            client_id=CLIENT_ID, client_secret=CLIENT_SECRET,
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
-Run a file: **python keycloak_test.py**
+
+### Run it
+Run a file: ```python keycloak_test.py```
+
+<br/>
 
 ___
 
 ### Create user
 
 
 Method **Create_user** with parameter _**payload**_  <br/>
@@ -76,10 +84,11 @@
     payload_update = {
         "attributes": {
             "phoneNumber": "1234567890",
             "testKey": "testValue"
         }
     }
 
+
 ____
 
 ### All functions see on page [Documentation](https://github.com/martinlauren55/keycloakAPI/blob/main/DOCS/DOCS.md)
```

### Comparing `keycloak_api_manager-0.1.2/README.md` & `keycloak_api_manager-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,37 +7,46 @@
 **REALM_NAME** = "realm_name" <br/>
 **CLIENT_SECRET** = "40j32-5860-4d79-ad16-9c39897w083" <br/>
 **USERNAME** = "username@gmail.com"   - User name with admin's rules <br/> 
 **PASSWORD** = "f232@3s456S#422" <br/>
 **SERVER_URL** = "http://localhost:8080/auth/" - url keykcloak server <br/>
 <br/>
 
-## Quickstart
 
-Create a file **keycloak_test.py** with:
+# Installation
 
+```pip install keycloak-api-manager```
+
+# Example
+### Create it
+Create a file ```main.py``` with:
 ```
 from keycloak_api_manager import KeycloakAPIManager
 
 CLIENT_ID = "test_client_name"
 REALM_NAME = "realm_name"
 CLIENT_SECRET = "40j32-5860-4d79-ad16-9c39897w083"
-USERNAME = 'username@gmail.com'
+USERNAME = 'username@gmail.com'                         # KEYCLOAK user's USERNAME or EMAIL User with admin's
 PASSWORD = 'f232@3s456S#422'
-SERVER_URL = "http://localhost:8080/auth/"
+SERVER_URL = "http://localhost:8080/auth/"              # KEYCLOAK URL http://localhost:8080/auth/ or
+                                                        # http://server_url/auth/
 
 
 keycloak_api = KeycloakAPIManager(keycloak_url=SERVER_URL, realm_name=REALM_NAME,
                            client_id=CLIENT_ID, client_secret=CLIENT_SECRET,
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
-Run a file: **python keycloak_test.py**
+
+### Run it
+Run a file: ```python keycloak_test.py```
+
+<br/>
 
 ___
 
 ### Create user
 
 
 Method **Create_user** with parameter _**payload**_  <br/>
@@ -59,10 +68,11 @@
     payload_update = {
         "attributes": {
             "phoneNumber": "1234567890",
             "testKey": "testValue"
         }
     }
 
+
 ____
 
 ### All functions see on page [Documentation](https://github.com/martinlauren55/keycloakAPI/blob/main/DOCS/DOCS.md)
```

### Comparing `keycloak_api_manager-0.1.2/keycloak_api_manager/keycloak_api_manager.py` & `keycloak_api_manager-0.1.3/keycloak_api_manager/keycloak_api_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,50 +58,50 @@
         """
         :return: number of realm users
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users/count"
         headers = {"Authorization": "Bearer " + self._access_token}
         return requests.get(url=url, headers=headers).json()
 
-    def get_user(self, user_id):
+    def get_user(self, user_id: str) -> bool:
         """
         :param user_id: KEYCLOAK ID
-        :return: KEYCLOAK USER ID
+        :return: info about user
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users/{user_id}"
         headers = {"Authorization": "Bearer " + self._access_token}
         return requests.get(url=url, headers=headers).json()
 
     def add_or_update_user_attributes(self, attributes: dict, user_id: str) -> bool:
         """
         :param attributes: {'key1': 'value1', 'key2': 'value2'}
         :param user_id: KEYCLOAK USER ID
-        :return:
+        :return: bool
         """
         attr = dict()
         for k, v in self.get_user_attributes(user_id=user_id).items():
             attr[k] = v[0]
         for k, v in attributes.items():
             attr[k] = v
         return self.update_user(payload={"attributes": attr}, user_id=user_id)
 
     def delete_user_attributes(self, attributes: list, user_id: str) -> bool:
         """
         :param attributes:  list -> ['phone', 'newTest']
         :param user_id: KEYCLOAK USER ID
-        :return:
+        :return: bool
         """
         attr = dict()
         for k, v in self.get_user_attributes(user_id=user_id).items():
             attr[k] = v[0]
         for key in attributes:
             del attr[key]
         return self.update_user(payload={"attributes": attr}, user_id=user_id)
 
-    def get_user_attributes(self, user_id):
+    def get_user_attributes(self, user_id: str):
         """
         :parame user_id: KEYCLOAK ID
         :return: KEYCLOAK USER attributes
         """
         user = self.get_user(user_id=user_id)
         if "attributes" in user.keys():
             return user['attributes']
@@ -112,32 +112,32 @@
         """
         :return: realm clients
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/clients"
         headers = {"Authorization": "Bearer " + self._access_token}
         return requests.get(url=url, headers=headers).json()
 
-    def create_user(self, payload: dict):
+    def create_user(self, payload: dict) -> bool:
         """
         :param payload: Dict with params {"username": "some_user", "enabled": True,
         "credentials": [{"temporary": False, "value": "raw_password"}]}
-        :return: KEYCLOAK USER ID
+        :return: bool
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users"
         headers = {"Authorization": "Bearer " + self._access_token, "Content-Type": "application/json",
                    "Accept": "application/json"}
         response = requests.post(url=url, headers=headers, data=json.dumps(payload))
 
         if response.status_code == 201:
             return True
         else:
             raise Exception(response.text)
 
     def create_identity_provider_links_for_user(self, provider_identity: str, provider_user_id: str,
-                                                provider_username: str, user_id: str):
+                                                provider_username: str, user_id: str) -> bool:
         """
         :param provider_identity: Identity Provider Alias (from method get_identity_providers)
         :param provider_user_id: Provider User ID
         :param provider_username: Provider Username
         :param user_id: KEYCLOAK USER ID
         :return:
         """
@@ -162,17 +162,17 @@
         providers = []
         for i in response['identityProviders']:
             providers.append(i['alias'])
         return providers
 
     def update_user(self, payload, user_id: str) -> bool:
         """
-        :param payload: POST REQUEST PAYLOAD
+        :param payload:
         :param user_id: KEYCLOAK ID
-        :return: KEYCLOAK USER ID
+        :return: bool
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users/{user_id}"
         headers = {"Authorization": "Bearer " + self._access_token, "Content-Type": "application/json",
                    "Accept": "application/json"}
         response = requests.put(url=url, headers=headers, data=json.dumps(payload))
         if response.status_code == 204:
             return True
```

### Comparing `keycloak_api_manager-0.1.2/keycloak_api_manager.egg-info/PKG-INFO` & `keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: keycloak-api-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
-Project-URL: Changelog, https://github.com/martinlauren55/keycloak-api-manager/blob/main/CHANGELOG.md
 Keywords: keycloak,API,keycloak API management
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -24,37 +23,46 @@
 **REALM_NAME** = "realm_name" <br/>
 **CLIENT_SECRET** = "40j32-5860-4d79-ad16-9c39897w083" <br/>
 **USERNAME** = "username@gmail.com"   - User name with admin's rules <br/> 
 **PASSWORD** = "f232@3s456S#422" <br/>
 **SERVER_URL** = "http://localhost:8080/auth/" - url keykcloak server <br/>
 <br/>
 
-## Quickstart
 
-Create a file **keycloak_test.py** with:
+# Installation
 
+```pip install keycloak-api-manager```
+
+# Example
+### Create it
+Create a file ```main.py``` with:
 ```
 from keycloak_api_manager import KeycloakAPIManager
 
 CLIENT_ID = "test_client_name"
 REALM_NAME = "realm_name"
 CLIENT_SECRET = "40j32-5860-4d79-ad16-9c39897w083"
-USERNAME = 'username@gmail.com'
+USERNAME = 'username@gmail.com'                         # KEYCLOAK user's USERNAME or EMAIL User with admin's
 PASSWORD = 'f232@3s456S#422'
-SERVER_URL = "http://localhost:8080/auth/"
+SERVER_URL = "http://localhost:8080/auth/"              # KEYCLOAK URL http://localhost:8080/auth/ or
+                                                        # http://server_url/auth/
 
 
 keycloak_api = KeycloakAPIManager(keycloak_url=SERVER_URL, realm_name=REALM_NAME,
                            client_id=CLIENT_ID, client_secret=CLIENT_SECRET,
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
-Run a file: **python keycloak_test.py**
+
+### Run it
+Run a file: ```python keycloak_test.py```
+
+<br/>
 
 ___
 
 ### Create user
 
 
 Method **Create_user** with parameter _**payload**_  <br/>
@@ -76,10 +84,11 @@
     payload_update = {
         "attributes": {
             "phoneNumber": "1234567890",
             "testKey": "testValue"
         }
     }
 
+
 ____
 
 ### All functions see on page [Documentation](https://github.com/martinlauren55/keycloakAPI/blob/main/DOCS/DOCS.md)
```

### Comparing `keycloak_api_manager-0.1.2/pyproject.toml` & `keycloak_api_manager-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["requests",]
 name = "keycloak_api_manager"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Polyakov Sergey", email = "martinlauren555@gmail.com"},
 ]
 description = "Keycloak API for management"
 readme = "README.md"
 requires-python = ">=3.5"
 keywords = ["keycloak", "API", "keycloak API management"]
@@ -17,9 +17,8 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 ]
 [project.urls]
 "Homepage" = "https://github.com/martinlauren55/keycloak-api-manager"
 "Documentation" = "https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md"
-"Repository" = "https://github.com/martinlauren55/keycloak-api-manager.git"
-"Changelog" = "https://github.com/martinlauren55/keycloak-api-manager/blob/main/CHANGELOG.md"
+"Repository" = "https://github.com/martinlauren55/keycloak-api-manager.git"
```


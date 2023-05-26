# Comparing `tmp/keycloak_api_manager-1.0.0.tar.gz` & `tmp/keycloak_api_manager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_api_manager-1.0.0.tar", last modified: Fri May 26 08:33:23 2023, max compression
+gzip compressed data, was "keycloak_api_manager-1.0.1.tar", last modified: Fri May 26 09:38:35 2023, max compression
```

## Comparing `keycloak_api_manager-1.0.0.tar` & `keycloak_api_manager-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.915617 keycloak_api_manager-1.0.0/
--rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2919 2023-05-26 08:33:23.913991 keycloak_api_manager-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2219 2023-05-26 08:31:47.000000 keycloak_api_manager-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.847629 keycloak_api_manager-1.0.0/keycloak_api_manager/
--rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-1.0.0/keycloak_api_manager/__init__.py
--rw-rw-rw-   0        0        0     8346 2023-05-26 08:17:40.000000 keycloak_api_manager-1.0.0/keycloak_api_manager/keycloak_api_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.910119 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/
--rw-rw-rw-   0        0        0     2919 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      825 2023-05-26 08:32:42.000000 keycloak_api_manager-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 08:33:23.916128 keycloak_api_manager-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 09:38:35.903534 keycloak_api_manager-1.0.1/
+-rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2919 2023-05-26 09:38:35.900837 keycloak_api_manager-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-05-26 08:31:47.000000 keycloak_api_manager-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 09:38:35.846038 keycloak_api_manager-1.0.1/keycloak_api_manager/
+-rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-1.0.1/keycloak_api_manager/__init__.py
+-rw-rw-rw-   0        0        0     8444 2023-05-26 09:35:16.000000 keycloak_api_manager-1.0.1/keycloak_api_manager/keycloak_api_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-26 09:38:35.899794 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/
+-rw-rw-rw-   0        0        0     2919 2023-05-26 09:38:35.000000 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-26 09:38:35.000000 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 09:38:35.000000 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 09:38:35.000000 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 09:38:35.000000 keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      825 2023-05-26 09:37:44.000000 keycloak_api_manager-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 09:38:35.903833 keycloak_api_manager-1.0.1/setup.cfg
```

### Comparing `keycloak_api_manager-1.0.0/LICENSE.txt` & `keycloak_api_manager-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-1.0.0/PKG-INFO` & `keycloak_api_manager-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak_api_manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
 Keywords: keycloak,API,keycloak API management
```

### Comparing `keycloak_api_manager-1.0.0/README.md` & `keycloak_api_manager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-1.0.0/keycloak_api_manager/keycloak_api_manager.py` & `keycloak_api_manager-1.0.1/keycloak_api_manager/keycloak_api_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """
         :return: number of realm users
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users/count"
         headers = {"Authorization": "Bearer " + self._access_token}
         return requests.get(url=url, headers=headers).json()
 
-    def get_user(self, user_id: str) -> bool:
+    def get_user(self, user_id: str):
         """
         :param user_id: KEYCLOAK ID
         :return: info about user
         """
         url = f"{self._keycloak_url}admin/realms/{self._realm_name}/users/{user_id}"
         headers = {"Authorization": "Bearer " + self._access_token}
         return requests.get(url=url, headers=headers).json()
@@ -99,16 +99,19 @@
 
     def get_user_attributes(self, user_id: str):
         """
         :parame user_id: KEYCLOAK ID
         :return: KEYCLOAK USER attributes
         """
         user = self.get_user(user_id=user_id)
-        if "attributes" in user.keys():
-            return user['attributes']
+        if "attributes" in user:
+            user_attr = {}
+            for k, v in user.get('attributes').items():
+                user_attr[k] = v[0]
+            return user_attr
         else:
             return None
 
     def get_realm_clients(self) -> dict:
         """
         :return: realm clients
         """
```

### Comparing `keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/PKG-INFO` & `keycloak_api_manager-1.0.1/keycloak_api_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-api-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
 Keywords: keycloak,API,keycloak API management
```

### Comparing `keycloak_api_manager-1.0.0/pyproject.toml` & `keycloak_api_manager-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["requests",]
 name = "keycloak_api_manager"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name = "Polyakov Sergey", email = "martinlauren555@gmail.com"},
 ]
 description = "Keycloak API for management"
 readme = "README.md"
 requires-python = ">=3.5"
 keywords = ["keycloak", "API", "keycloak API management"]
```


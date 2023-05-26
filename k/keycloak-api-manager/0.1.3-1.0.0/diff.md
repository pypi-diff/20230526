# Comparing `tmp/keycloak_api_manager-0.1.3.tar.gz` & `tmp/keycloak_api_manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_api_manager-0.1.3.tar", last modified: Fri May 26 08:27:58 2023, max compression
+gzip compressed data, was "keycloak_api_manager-1.0.0.tar", last modified: Fri May 26 08:33:23 2023, max compression
```

## Comparing `keycloak_api_manager-0.1.3.tar` & `keycloak_api_manager-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.978978 keycloak_api_manager-0.1.3/
--rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2935 2023-05-26 08:27:58.977199 keycloak_api_manager-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2235 2023-05-26 08:25:03.000000 keycloak_api_manager-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.937004 keycloak_api_manager-0.1.3/keycloak_api_manager/
--rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-0.1.3/keycloak_api_manager/__init__.py
--rw-rw-rw-   0        0        0     8346 2023-05-26 08:17:40.000000 keycloak_api_manager-0.1.3/keycloak_api_manager/keycloak_api_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:27:58.974217 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/
--rw-rw-rw-   0        0        0     2935 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-26 08:27:58.000000 keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      825 2023-05-26 08:25:34.000000 keycloak_api_manager-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 08:27:58.979228 keycloak_api_manager-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.915617 keycloak_api_manager-1.0.0/
+-rw-rw-rw-   0        0        0     1060 2023-05-25 10:35:55.000000 keycloak_api_manager-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2919 2023-05-26 08:33:23.913991 keycloak_api_manager-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-05-26 08:31:47.000000 keycloak_api_manager-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.847629 keycloak_api_manager-1.0.0/keycloak_api_manager/
+-rw-rw-rw-   0        0        0       56 2023-05-25 13:20:41.000000 keycloak_api_manager-1.0.0/keycloak_api_manager/__init__.py
+-rw-rw-rw-   0        0        0     8346 2023-05-26 08:17:40.000000 keycloak_api_manager-1.0.0/keycloak_api_manager/keycloak_api_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:33:23.910119 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/
+-rw-rw-rw-   0        0        0     2919 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 08:33:23.000000 keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      825 2023-05-26 08:32:42.000000 keycloak_api_manager-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 08:33:23.916128 keycloak_api_manager-1.0.0/setup.cfg
```

### Comparing `keycloak_api_manager-0.1.3/LICENSE.txt` & `keycloak_api_manager-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-0.1.3/PKG-INFO` & `keycloak_api_manager-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak_api_manager
-Version: 0.1.3
+Version: 1.0.0
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
 Keywords: keycloak,API,keycloak API management
@@ -52,15 +52,15 @@
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
 
 ### Run it
-Run a file: ```python keycloak_test.py```
+Run a file: ```main.py```
 
 <br/>
 
 ___
 
 ### Create user
```

### Comparing `keycloak_api_manager-0.1.3/README.md` & `keycloak_api_manager-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
 
 ### Run it
-Run a file: ```python keycloak_test.py```
+Run a file: ```main.py```
 
 <br/>
 
 ___
 
 ### Create user
```

### Comparing `keycloak_api_manager-0.1.3/keycloak_api_manager/keycloak_api_manager.py` & `keycloak_api_manager-1.0.0/keycloak_api_manager/keycloak_api_manager.py`

 * *Files identical despite different names*

### Comparing `keycloak_api_manager-0.1.3/keycloak_api_manager.egg-info/PKG-INFO` & `keycloak_api_manager-1.0.0/keycloak_api_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-api-manager
-Version: 0.1.3
+Version: 1.0.0
 Summary: Keycloak API for management
 Author-email: Polyakov Sergey <martinlauren555@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/martinlauren55/keycloak-api-manager
 Project-URL: Documentation, https://github.com/martinlauren55/keycloak-api-manager/blob/main/DOCS/DOCS.md
 Project-URL: Repository, https://github.com/martinlauren55/keycloak-api-manager.git
 Keywords: keycloak,API,keycloak API management
@@ -52,15 +52,15 @@
                            admin_username=USERNAME, admin_password=PASSWORD)
 
 about_me = keycloak_api.get_info_about_me()
 print(about_me)
 ```
 
 ### Run it
-Run a file: ```python keycloak_test.py```
+Run a file: ```main.py```
 
 <br/>
 
 ___
 
 ### Create user
```

### Comparing `keycloak_api_manager-0.1.3/pyproject.toml` & `keycloak_api_manager-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = ["requests",]
 name = "keycloak_api_manager"
-version = "0.1.3"
+version = "1.0.0"
 authors = [
     {name = "Polyakov Sergey", email = "martinlauren555@gmail.com"},
 ]
 description = "Keycloak API for management"
 readme = "README.md"
 requires-python = ">=3.5"
 keywords = ["keycloak", "API", "keycloak API management"]
```


# Comparing `tmp/ana_sdk-0.2.6.tar.gz` & `tmp/ana_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ana_sdk-0.2.6.tar", max compression
+gzip compressed data, was "ana_sdk-0.3.0.tar", max compression
```

## Comparing `ana_sdk-0.2.6.tar` & `ana_sdk-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.2.6/ana_sdk/__init__.py
--rw-r--r--   0        0        0    14807 2023-05-25 20:26:44.762021 ana_sdk-0.2.6/ana_sdk/ana.py
--rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.2.6/ana_sdk/clients/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.2.6/ana_sdk/clients/ana_data_client.py
--rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.2.6/ana_sdk/clients/base_client.py
--rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.2.6/ana_sdk/clients/dashboard_api_client.py
--rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.2.6/ana_sdk/clients/oauth_client.py
--rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.2.6/ana_sdk/clients/rpa_api_client.py
--rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.2.6/ana_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0     4686 2023-05-25 21:33:20.370293 ana_sdk-0.2.6/ana_sdk/result_factory.py
--rw-r--r--   0        0        0      463 2023-05-25 21:33:24.544980 ana_sdk-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.2.6/README.md
--rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-05-22 13:09:55.929573 ana_sdk-0.3.0/ana_sdk/__init__.py
+-rw-r--r--   0        0        0    14807 2023-05-25 20:26:44.762021 ana_sdk-0.3.0/ana_sdk/ana.py
+-rw-r--r--   0        0        0      177 2023-05-23 01:43:08.849263 ana_sdk-0.3.0/ana_sdk/clients/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-23 02:57:33.535000 ana_sdk-0.3.0/ana_sdk/clients/ana_data_client.py
+-rw-r--r--   0        0        0     1770 2023-05-18 23:09:59.503498 ana_sdk-0.3.0/ana_sdk/clients/base_client.py
+-rw-r--r--   0        0        0     4635 2023-05-23 01:51:45.997363 ana_sdk-0.3.0/ana_sdk/clients/dashboard_api_client.py
+-rw-r--r--   0        0        0     1438 2023-05-23 03:23:45.283114 ana_sdk-0.3.0/ana_sdk/clients/oauth_client.py
+-rw-r--r--   0        0        0     3320 2023-05-23 01:51:51.763464 ana_sdk-0.3.0/ana_sdk/clients/rpa_api_client.py
+-rw-r--r--   0        0        0      744 2023-05-25 20:23:48.737805 ana_sdk-0.3.0/ana_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     4934 2023-05-25 23:15:52.044789 ana_sdk-0.3.0/ana_sdk/result_factory.py
+-rw-r--r--   0        0        0      463 2023-05-25 23:17:36.695864 ana_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2105 2023-05-22 13:11:05.921381 ana_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 ana_sdk-0.3.0/PKG-INFO
```

### Comparing `ana_sdk-0.2.6/ana_sdk/ana.py` & `ana_sdk-0.3.0/ana_sdk/ana.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/clients/ana_data_client.py` & `ana_sdk-0.3.0/ana_sdk/clients/ana_data_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/clients/base_client.py` & `ana_sdk-0.3.0/ana_sdk/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/clients/dashboard_api_client.py` & `ana_sdk-0.3.0/ana_sdk/clients/dashboard_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/clients/oauth_client.py` & `ana_sdk-0.3.0/ana_sdk/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/clients/rpa_api_client.py` & `ana_sdk-0.3.0/ana_sdk/clients/rpa_api_client.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/exceptions/__init__.py` & `ana_sdk-0.3.0/ana_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/ana_sdk/result_factory.py` & `ana_sdk-0.3.0/ana_sdk/result_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,23 @@
                 response = requests.get(url)
                 response.raise_for_status()
 
                 with open(full_filename, "w") as file:
                     file.write(response.text)
 
         return self
+    
+    def get_link(self) -> str | None:
+        """
+        Recupera o link do relatório, caso exista um.
+
+        Returns:
+            str: Link do relatório, caso exista. Ou `None`.
+        """
+        return self.file.get("link") 
 
 
 class Task(AbstractResultHandler):
     """
     Classe que lida com resultados de execuções de tasks que não geram
     relatórios.
     """
```

### Comparing `ana_sdk-0.2.6/README.md` & `ana_sdk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ana_sdk-0.2.6/PKG-INFO` & `ana_sdk-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ana-sdk
-Version: 0.2.6
+Version: 0.3.0
 Summary: SDK que visa fornecer uma interface para interagir com os serviços ANA.
 License: MIT
 Author: Jovane Mafort
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


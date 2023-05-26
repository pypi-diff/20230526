# Comparing `tmp/cycleops-0.2.1.tar.gz` & `tmp/cycleops-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.2.1.tar", max compression
+gzip compressed data, was "cycleops-0.2.2.tar", max compression
```

## Comparing `cycleops-0.2.1.tar` & `cycleops-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-24 13:24:39.923886 cycleops-0.2.1/LICENSE
--rw-r--r--   0        0        0     3994 2023-05-24 13:24:39.923886 cycleops-0.2.1/README.md
--rw-r--r--   0        0        0     1125 2023-05-24 13:24:39.923886 cycleops-0.2.1/cycleops/__main__.py
--rw-r--r--   0        0        0      414 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/auth.py
--rw-r--r--   0        0        0     5468 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/client.py
--rw-r--r--   0        0        0     1113 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/exceptions.py
--rw-r--r--   0        0        0    12558 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/services.py
--rw-r--r--   0        0        0     4249 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/setups.py
--rw-r--r--   0        0        0     3047 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/stacks.py
--rw-r--r--   0        0        0      869 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/units.py
--rw-r--r--   0        0        0      972 2023-05-24 13:24:39.927886 cycleops-0.2.1/cycleops/utils.py
--rw-r--r--   0        0        0      556 2023-05-24 13:24:39.927886 cycleops-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 cycleops-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 14:08:21.326726 cycleops-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3994 2023-05-26 14:08:21.326726 cycleops-0.2.2/README.md
+-rw-r--r--   0        0        0     1125 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/auth.py
+-rw-r--r--   0        0        0     5468 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/client.py
+-rw-r--r--   0        0        0     1113 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/exceptions.py
+-rw-r--r--   0        0        0    12653 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/services.py
+-rw-r--r--   0        0        0     4249 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/setups.py
+-rw-r--r--   0        0        0     3047 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/stacks.py
+-rw-r--r--   0        0        0      869 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/units.py
+-rw-r--r--   0        0        0      972 2023-05-26 14:08:21.326726 cycleops-0.2.2/cycleops/utils.py
+-rw-r--r--   0        0        0      556 2023-05-26 14:08:21.326726 cycleops-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4519 1970-01-01 00:00:00.000000 cycleops-0.2.2/PKG-INFO
```

### Comparing `cycleops-0.2.1/LICENSE` & `cycleops-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/README.md` & `cycleops-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/__main__.py` & `cycleops-0.2.2/cycleops/__main__.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/client.py` & `cycleops-0.2.2/cycleops/client.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/exceptions.py` & `cycleops-0.2.2/cycleops/exceptions.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/services.py` & `cycleops-0.2.2/cycleops/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         None,
         help="The image of the container in the following format: <image_name>:<image_tag>",
     ),
     ports: Optional[str] = typer.Option(
         None,
         help="The ports of the container seperated by comma (e.g. 80:80,3000:3000).",
     ),
-    volumes: Optional[List[str]] = typer.Option(
+    volumes: Optional[str] = typer.Option(
         None,
         help="The volumes of the container.",
     ),
     env_file: Optional[str] = typer.Option(
         None,
         help="A file that contains environment variables.",
     ),
@@ -340,15 +340,15 @@
         None,
         help="The image of the container in the following format: <image_name>:<image_tag>",
     ),
     ports: Optional[str] = typer.Option(
         None,
         help="The ports of the container seperated by comma (e.g. 80:80,3000:3000).",
     ),
-    volumes: Optional[List[str]] = typer.Option(
+    volumes: Optional[str] = typer.Option(
         None,
         help="The volumes of the container.",
     ),
     env_file: Optional[str] = typer.Option(
         None,
         help="A file that contains environment variables.",
     ),
@@ -402,24 +402,28 @@
 
         volumes_list = []
         if volumes:
             volumes_list = [volume.strip() for volume in volumes.split(",")]
 
         container_name = name if name else container_name
 
-        service["variables"]["containers"][container_index] = {
+        variables = {
             "name": container_name,
             "image": image_name,
             "tag": image_tag,
             "ports": ports_list,
             "volumes": volumes_list,
             "command": command,
             "env_vars": env_vars,
         }
 
+        for key, value in variables.items():
+            if value:
+                service["variables"]["containers"][container_index][key] = value
+
         service_client.update(
             service_id,
             variables=service["variables"],
         )
 
         display_success_message(
             f"Container {container_name} in Service {service_id} has been updated"
```

### Comparing `cycleops-0.2.1/cycleops/setups.py` & `cycleops-0.2.2/cycleops/setups.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/stacks.py` & `cycleops-0.2.2/cycleops/stacks.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/units.py` & `cycleops-0.2.2/cycleops/units.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/cycleops/utils.py` & `cycleops-0.2.2/cycleops/utils.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.2.1/pyproject.toml` & `cycleops-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycleops"
-version = "0.2.1"
+version = "0.2.2"
 description = "The official command line interface for Cycleops"
 authors = ["George Margaritis <george@withlogic.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cycleops-0.2.1/PKG-INFO` & `cycleops-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycleops
-Version: 0.2.1
+Version: 0.2.2
 Summary: The official command line interface for Cycleops
 License: MIT
 Author: George Margaritis
 Author-email: george@withlogic.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/spai-2023.5.25.post6.tar.gz` & `tmp/spai-2023.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.5.25.post6.tar", max compression
+gzip compressed data, was "spai-2023.5.26.tar", max compression
```

## Comparing `spai-2023.5.25.post6.tar` & `spai-2023.5.26.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.25.post6/README.md
--rw-r--r--   0        0        0      344 2023-05-25 13:57:05.301905 spai-2023.5.25.post6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.25.post6/spai/__init__.py
--rw-r--r--   0        0        0      140 2023-05-21 10:11:30.915314 spai-2023.5.25.post6/spai/cli/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.25.post6/spai/cli/cloud.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.25.post6/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.25.post6/spai/cli/commands/hello.py
--rw-r--r--   0        0        0     5533 2023-05-21 10:50:31.176515 spai-2023.5.25.post6/spai/cli/local.py
--rw-r--r--   0        0        0      647 2023-05-25 09:53:16.130678 spai-2023.5.25.post6/spai/cli/project-template/REDME.md
--rw-r--r--   0        0        0        0 2023-05-25 09:52:27.506558 spai-2023.5.25.post6/spai/cli/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:34.438575 spai-2023.5.25.post6/spai/cli/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:43.562598 spai-2023.5.25.post6/spai/cli/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0        0 2023-05-25 09:46:24.337697 spai-2023.5.25.post6/spai/cli/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0        0 2023-05-25 09:52:54.906626 spai-2023.5.25.post6/spai/cli/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0      232 2023-05-25 09:54:34.271270 spai-2023.5.25.post6/spai/cli/project-template/spai.config.yml
--rw-r--r--   0        0        0        0 2023-05-25 09:53:08.122658 spai-2023.5.25.post6/spai/cli/project-template/uis/map/main.py
--rw-r--r--   0        0        0     2495 2023-05-21 09:35:01.310684 spai-2023.5.25.post6/spai/cli/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.25.post6/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.25.post6/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.25.post6/spai/data/satellite/download.py
--rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.25.post6/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.25.post6/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.25.post6/spai/image/__init__.py
--rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.25.post6/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.25.post6/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.25.post6/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.25.post6/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.25.post6/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.25.post6/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     1631 2023-05-25 10:38:00.746147 spai-2023.5.25.post6/spai/main.py
--rw-r--r--   0        0        0     1915 2023-05-25 11:35:53.721248 spai-2023.5.25.post6/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-25 11:40:20.925888 spai-2023.5.25.post6/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2521 2023-05-25 11:38:44.845657 spai-2023.5.25.post6/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.25.post6/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.25.post6/spai/storage/minio.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 spai-2023.5.25.post6/setup.py
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 spai-2023.5.25.post6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 05:51:22.950543 spai-2023.5.26/README.md
+-rw-r--r--   0        0        0      342 2023-05-26 11:57:32.433786 spai-2023.5.26/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.5.26/spai/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:47:16.135084 spai-2023.5.26/spai/cli/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-21 08:39:35.055997 spai-2023.5.26/spai/cli/cloud.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.5.26/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-12 05:59:27.734580 spai-2023.5.26/spai/cli/commands/hello.py
+-rw-r--r--   0        0        0     3165 2023-05-26 11:47:46.887246 spai-2023.5.26/spai/cli/local.py
+-rw-r--r--   0        0        0     5553 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.5.26/spai/cli/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 11:57:20.229740 spai-2023.5.26/spai/cli/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.5.26/spai/cli/project-template/uis/map/main.py
+-rw-r--r--   0        0        0     3413 2023-05-26 11:46:05.338695 spai-2023.5.26/spai/cli/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.5.26/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.5.26/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.5.26/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.5.26/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.5.26/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.5.26/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.5.26/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.5.26/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.5.26/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.5.26/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.5.26/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.5.26/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.5.26/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.5.26/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.5.26/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.5.26/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.5.26/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.5.26/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     1621 2023-05-26 11:47:17.739093 spai-2023.5.26/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.5.26/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.5.26/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2521 2023-05-26 08:52:44.511236 spai-2023.5.26/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.5.26/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.5.26/spai/storage/minio.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 spai-2023.5.26/setup.py
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 spai-2023.5.26/PKG-INFO
```

### Comparing `spai-2023.5.25.post6/spai/cli/cloud.py` & `spai-2023.5.26/spai/cli/cloud.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/cli/validate.py` & `spai-2023.5.26/spai/cli/validate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 import os
 import yaml
+from pydantic import BaseModel
+from typing import Union, List
+
+
+class ScriptConfig(BaseModel):
+    name: str
+    command: Union[str, None] = None
+    run_every: Union[int, None] = None  # seconds
+    run_on_start: bool = True
+
+
+class NotebookConfig(BaseModel):
+    name: str
+    command: Union[str, None] = None
+    run_every: Union[int, None] = None  # seconds
+    run_on_start: bool = True
+
+
+class APIConfig(BaseModel):
+    name: str
+    command: Union[str, None] = None
+
+
+class UIConfig(BaseModel):
+    name: str
+    command: str  # steamlit, javascript, ...
+
+
+class Config(BaseModel):
+    project: Union[str, None] = None
+    scripts: Union[List[ScriptConfig], None] = None
+    notebooks: Union[List[NotebookConfig], None] = None
+    apis: Union[List[APIConfig], None] = None
+    uis: Union[List[UIConfig], None] = None
 
 
 def validate_folder(dir, folder, typer):
     if not os.path.exists(dir / folder):
         raise typer.BadParameter(f"No {folder} directory found in '{dir}'.")
 
 
 def validate_item(dir, folder, item, name, typer, file="main.py"):
     # check name
-    if not "name" in item:
-        raise typer.BadParameter(
-            f"{name} '{item['name']}' is missing 'name' attribute."
-        )
+    if not item.name:
+        raise typer.BadParameter(f"{name} '{item.name}' is missing 'name' attribute.")
     # check folder has folder with item name
-    if not os.path.exists(dir / folder / item["name"]):
+    if not os.path.exists(dir / folder / item.name):
         raise typer.BadParameter(
-            f"{name} '{item['name']}' cannot be found in {dir}/{folder}."
+            f"{name} '{item.name}' cannot be found in {dir}/{folder}."
         )
     # check folder has file
-    if not file in os.listdir(dir / folder / item["name"]):
-        raise typer.BadParameter(f"{name} '{item['name']}' is missing file 'main.py'.")
+    if not file in os.listdir(dir / folder / item.name):
+        raise typer.BadParameter(f"{name} '{item.name}' is missing file 'main.py'.")
     # TODO: check optionals: reqs, env...
 
 
 def load_and_validate_config(dir, typer, cloud):
     # check dir exists
     if not dir.exists():
         raise typer.BadParameter(f"Directory '{dir}' does not exist.")
@@ -33,35 +65,39 @@
         raise typer.BadParameter(
             f"Directory '{dir}' is not a spai project. No spai.config.yml file found."
         )
     # load config
     config = {}
     with open(dir / "spai.config.yml", "r") as f:
         config = yaml.safe_load(f)
-    # check config has project name if cloud deployment
-    if not "project" in config:
-        raise typer.BadParameter(f"spai.config.yml file is missing 'project' section.")
+    if not config:
+        raise typer.BadParameter(f"spai.config.yml file is empty.")
+    config = Config(**config)
+    # TODO: check if project name is already taken in cloud, locally is not a problem
+    config.project = dir.name if not config.project else config.project
     # check scripts
-    if "scripts" in config:
+    if config.scripts:
         # check project has scripts folder
         validate_folder(dir, "scripts", typer)
-        for script in config["scripts"]:
+        for script in config.scripts:
             validate_item(dir, "scripts", script, "script", typer)
+    else:
+        typer.echo("No scripts found in spai.config.yml.")
     # check notebooks
-    if "notebooks" in config:
+    if config.notebooks:
         # check project has notebooks folder
         validate_folder(dir, "notebooks", typer)
-        for notebook in config["notebooks"]:
+        for notebook in config.notebooks:
             validate_item(dir, "notebooks", notebook, "notebook", typer, "main.ipynb")
     # check apis
-    if "apis" in config:
+    if config.apis:
         # check project has apis folder
         validate_folder(dir, "apis", typer)
-        for api in config["apis"]:
+        for api in config.apis:
             validate_item(dir, "apis", api, "api", typer)
     # check uis
-    if "uis" in config:
+    if config.uis:
         # check project has uis folder
         validate_folder(dir, "uis", typer)
-        for ui in config["uis"]:
+        for ui in config.uis:
             validate_item(dir, "uis", ui, "ui", typer)
     return config
```

### Comparing `spai-2023.5.25.post6/spai/data/satellite/download.py` & `spai-2023.5.26/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/data/satellite/explore.py` & `spai-2023.5.26/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.5.26/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.5.26/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.5.26/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.5.26/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/image/utils.py` & `spai-2023.5.26/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/image/xyz/cache.py` & `spai-2023.5.26/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/image/xyz/errors.py` & `spai-2023.5.26/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/image/xyz/get_image_tile.py` & `spai-2023.5.26/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/image/xyz/image_utils.py` & `spai-2023.5.26/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/main.py` & `spai-2023.5.26/spai/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 sys.path.append(os.path.join(spai_cli_dir))
 
 from cli.commands import hello
 from cli import (
     load_and_validate_config,
     deploy_and_run_cloud,
     run_local,
-    stop_local,
-    list_local,
 )
 
 app = typer.Typer()
 app.add_typer(hello.app, name="hello")
 
 
 @app.command()
@@ -46,24 +44,24 @@
     # print(config)
     # run project
     if cloud:
         return deploy_and_run_cloud(dir, config, typer)
     return run_local(dir, config, typer)
 
 
-@app.command()
-def list(
-    project: str = typer.Option(None, "-p", "--project"),
-):
-    return list_local(typer, project)
+# @app.command()
+# def list(
+#     project: str = typer.Option(None, "-p", "--project"),
+# ):
+#     return list_local(typer, project)
 
 
-@app.command()
-def stop(
-    project: str = typer.Option(None, "-p", "--project"),
-):
-    # TODO: get confirmation
-    return stop_local(typer, project)
+# @app.command()
+# def stop(
+#     project: str = typer.Option(None, "-p", "--project"),
+# ):
+#     # TODO: get confirmation
+#     return stop_local(typer, project)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `spai-2023.5.25.post6/spai/storage/BaseStorage.py` & `spai-2023.5.26/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/spai/storage/CloudStorage.py` & `spai-2023.5.26/spai/storage/CloudStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.client.put_object(
             self.bucket, name, array_bytes, len(array_bytes.getvalue())
         )
         return self.get_url(name)
 
     def create_from_csv(self, data, name):
         csv_bytes = BytesIO()
-        data.to_csv(csv_bytes, index=False)
+        data.to_csv(csv_bytes)
         csv_bytes.seek(0)
         self.client.put_object(self.bucket, name, csv_bytes, len(csv_bytes.getvalue()))
         return self.get_url(name)
 
     def create_from_json(self, data, name):
         json_bytes = BytesIO()
         data.to_json(json_bytes)
@@ -97,11 +97,11 @@
     def read_from_array(self, name):
         return np.load(self.read_object(name))
 
     def read_from_rasterio(self, name):
         return rio.open(self.read_object(name))
 
     def read_from_csv(self, name):
-        return pd.read_csv(self.read_object(name))
+        return pd.read_csv(self.read_object(name), index_col=0)
 
     def read_from_json(self, name):
         return pd.read_json(self.read_object(name))
```

### Comparing `spai-2023.5.25.post6/spai/storage/Storage.py` & `spai-2023.5.26/spai/storage/Storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def create_from_array(self, data, name):
         dst_path = self.get_path(name)
         np.save(dst_path, data)
         return dst_path
 
     def create_from_csv(self, data, name):
         dst_path = self.get_path(name)
-        data.to_csv(dst_path, index=False)
+        data.to_csv(dst_path)
         return dst_path
 
     def create_from_json(self, data, name):
         dst_path = self.get_path(name)
         data.to_json(dst_path)
         return dst_path
 
@@ -72,11 +72,11 @@
             path = self.get_path(name)
         return np.load(path)
 
     def read_from_rasterio(self, name):
         return rio.open(self.get_path(name))
 
     def read_from_csv(self, name):
-        return pd.read_csv(self.get_path(name))
+        return pd.read_csv(self.get_path(name), index_col=0)
 
     def read_from_json(self, name):
         return pd.read_json(self.get_path(name))
```

### Comparing `spai-2023.5.25.post6/spai/storage/minio.py` & `spai-2023.5.26/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.5.25.post6/setup.py` & `spai-2023.5.26/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'spai.cli': ['project-template/*', 'project-template/notebooks/analytics/*']}
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.5.25.post6',
+    'version': '2023.5.26',
     'description': '',
     'long_description': '',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


# Comparing `tmp/datatrail_cli-0.1.2.tar.gz` & `tmp/datatrail_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.1.2.tar", max compression
+gzip compressed data, was "datatrail_cli-0.2.0.tar", max compression
```

## Comparing `datatrail_cli-0.1.2.tar` & `datatrail_cli-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-05-24 15:44:32.472474 datatrail_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0     3492 2023-05-24 15:44:32.472474 datatrail_cli-0.1.2/README.md
--rw-r--r--   0        0        0      214 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/__init__.py
--rw-r--r--   0        0        0      893 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/cli.py
--rw-r--r--   0        0        0     3713 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/config.py
--rw-r--r--   0        0        0     1062 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/config.yaml
--rw-r--r--   0        0        0     3283 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/ls.py
--rw-r--r--   0        0        0     4278 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/ps.py
--rw-r--r--   0        0        0     3717 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/pull.py
--rw-r--r--   0        0        0     8674 2023-05-24 15:44:32.480474 datatrail_cli-0.1.2/dtcli/src/functions.py
--rw-r--r--   0        0        0     8262 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     1151 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1048 2023-05-24 15:44:32.484474 datatrail_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 datatrail_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-26 20:56:06.198466 datatrail_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3558 2023-05-26 20:56:06.198466 datatrail_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      214 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/__init__.py
+-rw-r--r--   0        0        0      893 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/cli.py
+-rw-r--r--   0        0        0     3714 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/config.yaml
+-rw-r--r--   0        0        0     3442 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/ls.py
+-rw-r--r--   0        0        0     4415 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/ps.py
+-rw-r--r--   0        0        0     3978 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/pull.py
+-rw-r--r--   0        0        0     8795 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/src/functions.py
+-rw-r--r--   0        0        0     8262 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     1493 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1048 2023-05-26 20:56:06.210466 datatrail_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 datatrail_cli-0.2.0/PKG-INFO
```

### Comparing `datatrail_cli-0.1.2/LICENSE` & `datatrail_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.2/README.md` & `datatrail_cli-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center">
     <img src="https://github.com/CHIMEFRB/datatrail-cli/blob/main/docs/images/Datatrail-logo.png" width="110", height="100">
 </div>
 
 <h1 align="center">Datatrail CLI</h1>
 
 <h4 align="center">
-  <a href="https://">Install</a>
+  <a href="https://github.com/CHIMEFRB/datatrail-cli/tree/main#%EF%B8%8F-installation">Install</a>
   ·
   <a href="https://chimefrb.github.io/datatrail-cli/">Docs</a>
 </h4>
 
 <p align="center">
     <a href="https://github.com/CHIMEFRB/datatrail-cli/pulse">
       <img src="https://img.shields.io/github/last-commit/CHIMEFRB/datatrail-cli?style=for-the-badge&logo=github&color=7dc4e4&logoColor=D9E0EE&labelColor=302D41"/>
```

### Comparing `datatrail_cli-0.1.2/dtcli/cli.py` & `datatrail_cli-0.2.0/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.2/dtcli/config.py` & `datatrail_cli-0.2.0/dtcli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
     # Default configuration.
     defaults: Dict[str, Any] = {
         "server": "https://frb.chimenet.ca/datatrail",
         "vospace_certfile": f"{Path.home()}/.ssl/cadcproxy.pem",
         "root_mounts": {
             "chime": "/",
-            "canfar": "/arc/project/chime_frb/",
+            "canfar": "/arc/projects/chime_frb/",
             "kko": "/",
             "gbo": "/",
             "hco": "/",
             "local": "./",
         },
     }
     defaults["site"] = site
```

### Comparing `datatrail_cli-0.1.2/dtcli/config.yaml` & `datatrail_cli-0.2.0/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.2/dtcli/ls.py` & `datatrail_cli-0.2.0/dtcli/ls.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional
 
 import click
 from rich.console import Console
 from rich.table import Table
 
 from dtcli.src import functions
+from dtcli.utilities.utilities import validate_scope
 
 logger = logging.getLogger("ls")
 
 console = Console()
 
 
 @click.command(help="List scopes & datasets")
@@ -47,14 +48,17 @@
     elif quiet:
         logger.setLevel("ERROR")
     logger.debug("`list` called with:")
     logger.debug(f"scope: {scope} [{type(scope)}]")
     logger.debug(f"datasets: {datasets} [{type(datasets)}]")
     logger.debug(f"verbose: {verbose} [{type(verbose)}]")
     logger.debug(f"quiet: {quiet} [{type(quiet)}]")
+    if scope:
+        if not validate_scope(scope):
+            raise ValueError("Scope does not exist.")
     results = functions.list(scope, datasets, verbose, quiet)
 
     # Display scopes.
     if "scopes" in results.keys():
         table = Table(
             title="Datatrail: Scopes",
             header_style="magenta",
```

### Comparing `datatrail_cli-0.1.2/dtcli/ps.py` & `datatrail_cli-0.2.0/dtcli/ps.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 import click
 from rich.console import Console
 from rich.table import Table
 
 from dtcli.src import functions
 from dtcli.utilities import cadcclient
+from dtcli.utilities.utilities import validate_scope
 
 logger = logging.getLogger("ps")
 
 
 @click.command(name="ps", help="Details of a dataset.")
 @click.argument("scope", required=True, type=click.STRING, nargs=1)
 @click.argument("dataset", required=True, type=click.STRING, nargs=1)
 @click.option("-s", "--show-files", is_flag=True, help="Show file names.")
 def ps(scope: str, dataset: str, show_files: bool):
     """Detailed status of a dataset."""
+    if not validate_scope(scope):
+        raise ValueError("Scope does not exist.")
     try:
         files, policies = functions.ps(scope, dataset)
     except Exception as e:
         logger.error(e)
         return None
 
     # Info table
```

### Comparing `datatrail_cli-0.1.2/dtcli/pull.py` & `datatrail_cli-0.2.0/dtcli/pull.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import click
 from rich.console import Console
 from rich.prompt import Confirm
 
 from dtcli.config import procure
 from dtcli.src.functions import find_missing_dataset_files, get_files
 from dtcli.utilities.cadcclient import size
+from dtcli.utilities.utilities import validate_scope
 
 logger = logging.getLogger("pull")
 
 console = Console()
 
 
 @click.command(name="pull", help="Download a dataset.")
@@ -83,17 +84,23 @@
             logger.info(f"No directory, setting to: {directory}.")
     except Exception:
         logger.exception(
             "Configuration Missing!! Run `datatrail config init`.",
         )
         raise click.Abort()
 
+    if not validate_scope(scope):
+        raise ValueError("Scope does not exist.")
+
     # Find files missing from localhost.
     console.print(f"\nSearching for files for {dataset} {scope}...\n")
     files = find_missing_dataset_files(scope, dataset)
+    if len(files["missing"]) == 0:
+        console.print("No files found at minoc.", style="bold red")
+        return None
     common_path = path.commonpath(files["missing"])
     if common_path.startswith("cadc:CHIMEFRB"):
         common_path = common_path.replace("cadc:CHIMEFRB", "")
     to_download_size = size(common_path)
     console.print(
         f" - {len(files['existing'])} files found at {site}.",
         style="green",
```

### Comparing `datatrail_cli-0.1.2/dtcli/src/functions.py` & `datatrail_cli-0.2.0/dtcli/src/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,19 @@
             if Path(f).exists():
                 existing_files.append(f)
             else:
                 missing_files.append(f)
 
     # For local, assume no files exist.
     else:
-        missing_files = dataset_locations["file_replica_locations"]["minoc"]
+        file_replicas = dataset_locations.get("file_replica_locations")
+        if file_replicas:
+            missing_files = file_replicas.get("minoc")
+        else:
+            missing_files = []
         existing_files = []
     return {"missing": missing_files, "existing": existing_files}
 
 
 def get_files(
     files: List[str],
     site: str,
```

### Comparing `datatrail_cli-0.1.2/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.2.0/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.1.2/dtcli/utilities/utilities.py` & `datatrail_cli-0.2.0/dtcli/utilities/utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utility functions."""
 
 from typing import Any, Dict, List, Union
 
+import requests
 from requests.models import Response
 
 
 def decode_response(response: Response) -> Union[Dict, str]:
     """Decode response.
 
     Args:
@@ -40,7 +41,21 @@
             idx += batch_size + 1
         else:
             batch = data[idx : idx + batch_size]  # noqa: E203
             idx += batch_size
         if len(batch) > 0:
             batches.append(batch)
     return batches
+
+
+def validate_scope(scope: str) -> bool:
+    """Check if scope is valid.
+
+    Args:
+        scope (str): Scope to check.
+
+    Returns:
+        bool: True if scope is valid.
+    """
+    resp = requests.get("https://frb.chimenet.ca/datatrail/query/dataset/scopes")
+    scopes = decode_response(resp)
+    return scope in scopes
```

### Comparing `datatrail_cli-0.1.2/pyproject.toml` & `datatrail_cli-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.1.2"
+version = "0.2.0"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.1.2/PKG-INFO` & `datatrail_cli-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.1.2
+Version: 0.2.0
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -27,15 +27,15 @@
 <div align="center">
     <img src="https://github.com/CHIMEFRB/datatrail-cli/blob/main/docs/images/Datatrail-logo.png" width="110", height="100">
 </div>
 
 <h1 align="center">Datatrail CLI</h1>
 
 <h4 align="center">
-  <a href="https://">Install</a>
+  <a href="https://github.com/CHIMEFRB/datatrail-cli/tree/main#%EF%B8%8F-installation">Install</a>
   ·
   <a href="https://chimefrb.github.io/datatrail-cli/">Docs</a>
 </h4>
 
 <p align="center">
     <a href="https://github.com/CHIMEFRB/datatrail-cli/pulse">
       <img src="https://img.shields.io/github/last-commit/CHIMEFRB/datatrail-cli?style=for-the-badge&logo=github&color=7dc4e4&logoColor=D9E0EE&labelColor=302D41"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.1.2 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.2.0 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cadcdata (>=2.4,<3.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```


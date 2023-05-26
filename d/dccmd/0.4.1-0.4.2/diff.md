# Comparing `tmp/dccmd-0.4.1.tar.gz` & `tmp/dccmd-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccmd-0.4.1.tar", max compression
+gzip compressed data, was "dccmd-0.4.2.tar", max compression
```

## Comparing `dccmd-0.4.1.tar` & `dccmd-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11343 2022-07-17 08:39:13.687368 dccmd-0.4.1/LICENSE
--rw-r--r--   0        0        0    15516 2023-01-24 17:08:53.088409 dccmd-0.4.1/README.md
--rw-r--r--   0        0        0    37619 2023-05-02 17:15:58.749056 dccmd-0.4.1/dccmd/__init__.py
--rw-r--r--   0        0        0        0 2022-07-17 08:39:13.688213 dccmd-0.4.1/dccmd/main/__init__.py
--rw-r--r--   0        0        0     2693 2022-07-22 20:15:29.962402 dccmd-0.4.1/dccmd/main/auth/__init__.py
--rw-r--r--   0        0        0     1971 2022-07-17 08:39:13.688616 dccmd-0.4.1/dccmd/main/auth/client.py
--rw-r--r--   0        0        0     2434 2022-07-17 08:39:13.688752 dccmd-0.4.1/dccmd/main/auth/credentials.py
--rw-r--r--   0        0        0    10257 2023-01-24 17:08:53.089168 dccmd-0.4.1/dccmd/main/auth/util.py
--rw-r--r--   0        0        0     3645 2022-07-17 08:39:13.689118 dccmd-0.4.1/dccmd/main/crypto/__init__.py
--rw-r--r--   0        0        0     1846 2022-07-17 08:39:13.689243 dccmd-0.4.1/dccmd/main/crypto/keys.py
--rw-r--r--   0        0        0     1769 2023-01-24 17:08:53.089465 dccmd-0.4.1/dccmd/main/crypto/util.py
--rw-r--r--   0        0        0     8669 2023-05-02 16:44:40.001311 dccmd-0.4.1/dccmd/main/download/__init__.py
--rw-r--r--   0        0        0     1516 2023-01-24 17:08:53.090050 dccmd-0.4.1/dccmd/main/models/__init__.py
--rw-r--r--   0        0        0     1158 2022-07-18 05:43:46.467561 dccmd-0.4.1/dccmd/main/models/errors.py
--rw-r--r--   0        0        0    11768 2023-05-02 17:14:14.445184 dccmd-0.4.1/dccmd/main/rooms/__init__.py
--rw-r--r--   0        0        0      118 2023-01-24 17:08:53.090505 dccmd-0.4.1/dccmd/main/rooms/models.py
--rw-r--r--   0        0        0    10440 2023-05-02 17:14:08.232455 dccmd-0.4.1/dccmd/main/rooms/permissions.py
--rw-r--r--   0        0        0     3128 2023-01-24 17:08:53.090892 dccmd-0.4.1/dccmd/main/rooms/print.py
--rw-r--r--   0        0        0    11196 2023-05-02 17:37:42.191534 dccmd-0.4.1/dccmd/main/upload/__init__.py
--rw-r--r--   0        0        0     4423 2022-07-19 16:30:43.809515 dccmd-0.4.1/dccmd/main/users/__init__.py
--rw-r--r--   0        0        0     9731 2023-05-02 16:44:45.195480 dccmd-0.4.1/dccmd/main/users/manage.py
--rw-r--r--   0        0        0     1902 2023-01-24 17:08:53.097355 dccmd-0.4.1/dccmd/main/users/print.py
--rw-r--r--   0        0        0     4747 2023-01-24 17:08:53.097677 dccmd-0.4.1/dccmd/main/util/__init__.py
--rw-r--r--   0        0        0      652 2023-05-02 17:39:22.245290 dccmd-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    17046 2023-05-02 17:39:55.363215 dccmd-0.4.1/setup.py
--rw-r--r--   0        0        0    16186 2023-05-02 17:39:55.363829 dccmd-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-04-03 15:12:02.723336 dccmd-0.4.2/LICENSE
+-rw-r--r--   0        0        0    15516 2023-03-09 19:14:33.534717 dccmd-0.4.2/README.md
+-rw-r--r--   0        0        0    37897 2023-05-26 18:40:10.713334 dccmd-0.4.2/dccmd/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-12 18:48:32.479928 dccmd-0.4.2/dccmd/main/__init__.py
+-rw-r--r--   0        0        0     2693 2022-10-24 16:43:51.513342 dccmd-0.4.2/dccmd/main/auth/__init__.py
+-rw-r--r--   0        0        0     1971 2022-04-03 16:01:57.710024 dccmd-0.4.2/dccmd/main/auth/client.py
+-rw-r--r--   0        0        0     2434 2022-04-02 13:57:48.676773 dccmd-0.4.2/dccmd/main/auth/credentials.py
+-rw-r--r--   0        0        0    10257 2023-03-09 19:14:33.534717 dccmd-0.4.2/dccmd/main/auth/util.py
+-rw-r--r--   0        0        0     3645 2022-07-16 13:22:43.136443 dccmd-0.4.2/dccmd/main/crypto/__init__.py
+-rw-r--r--   0        0        0     1846 2022-07-16 13:22:43.136443 dccmd-0.4.2/dccmd/main/crypto/keys.py
+-rw-r--r--   0        0        0     1769 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/crypto/util.py
+-rw-r--r--   0        0        0     8669 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/download/__init__.py
+-rw-r--r--   0        0        0     1516 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/models/__init__.py
+-rw-r--r--   0        0        0     1158 2022-07-16 12:51:12.543170 dccmd-0.4.2/dccmd/main/models/errors.py
+-rw-r--r--   0        0        0    11768 2023-05-26 18:40:10.716667 dccmd-0.4.2/dccmd/main/rooms/__init__.py
+-rw-r--r--   0        0        0      118 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/rooms/models.py
+-rw-r--r--   0        0        0    10440 2023-05-26 18:40:10.716667 dccmd-0.4.2/dccmd/main/rooms/permissions.py
+-rw-r--r--   0        0        0     3128 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/rooms/print.py
+-rw-r--r--   0        0        0    11512 2023-05-26 18:53:37.146674 dccmd-0.4.2/dccmd/main/upload/__init__.py
+-rw-r--r--   0        0        0     4423 2022-10-24 16:43:51.516675 dccmd-0.4.2/dccmd/main/users/__init__.py
+-rw-r--r--   0        0        0     9731 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/users/manage.py
+-rw-r--r--   0        0        0     1902 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/users/print.py
+-rw-r--r--   0        0        0     4747 2023-03-09 19:14:33.538050 dccmd-0.4.2/dccmd/main/util/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-26 18:40:10.716667 dccmd-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 dccmd-0.4.2/setup.py
+-rw-r--r--   0        0        0    16237 1970-01-01 00:00:00.000000 dccmd-0.4.2/PKG-INFO
```

### Comparing `dccmd-0.4.1/LICENSE` & `dccmd-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/README.md` & `dccmd-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/__init__.py` & `dccmd-0.4.2/dccmd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,16 +232,18 @@
             )
 
         # node id must be from parent room if folder
         if node_info.type == NodeType.folder:
             distrib_node_id = node_info.authParentId
         if node_info.type == NodeType.room:
             distrib_node_id = node_info.id
+        else:
+            distrib_node_id = None
 
-        if node_info.isEncrypted is True:
+        if node_info.isEncrypted is True and distrib_node_id is not None:
             await distribute_missing_keys(dracoon=dracoon, room_id=distrib_node_id)
 
         await dracoon.logout()
 
     asyncio.run(_upload())
 
 
@@ -364,20 +366,20 @@
             cli_mode=cli_mode,
             debug=debug,
         )
 
         # remove base url from path
         parsed_path = parse_new_path(full_path=dir_path)
 
-        if parsed_path != "/":
-            parent_node = await dracoon.nodes.get_node_from_path(path=parsed_path)
-            parent_id = parent_node.id
-        elif parsed_path == "/":
+        if parsed_path == "/":
             parent_node = None
             parent_id = 0
+        else:
+            parent_node = await dracoon.nodes.get_node_from_path(path=parsed_path)
+            parent_id = parent_node.id
 
         room_name = parse_file_name(full_path=dir_path)
 
         if parsed_path != "/" and parent_node is None:
             await dracoon.logout()
             typer.echo(format_error_message(msg=f"Node not found: {parsed_path}"))
             sys.exit(1)
@@ -393,18 +395,18 @@
             typer.echo(
                 format_error_message(msg="An admin user must be provided on root path.")
             )
             sys.exit(1)
 
         if admin_user and parent_id != 0:
             user_info = await find_user_by_username(dracoon=dracoon, user_name=admin_user, as_user_manager=False, room_id=parent_id)
-            payload = dracoon.nodes.make_room(name=room_name, parent_id=parent_id, inherit_perms=False, admin_ids=[user_info.userInfo.id])
+            payload = dracoon.nodes.make_room(name=room_name, parent_id=parent_id, inherit_perms=False, admin_ids=[user_info.userInfo.id]) # type: ignore
         if admin_user and parent_id == 0:
             user_info = await find_user_by_username(dracoon=dracoon, user_name=admin_user)
-            payload = dracoon.nodes.make_room(name=room_name, inherit_perms=False, admin_ids=[user_info.id], parent_id=None)
+            payload = dracoon.nodes.make_room(name=room_name, inherit_perms=False, admin_ids=[user_info.id], parent_id=None) # type: ignore
         else:
             payload = dracoon.nodes.make_room(
             name=room_name, parent_id=parent_id, inherit_perms=True
             )
 
         try:
             await dracoon.nodes.create_room(room=payload, raise_on_err=True)
@@ -608,22 +610,20 @@
             password=password,
             cli_mode=cli_mode,
             debug=debug,
         )
 
         # remove base url from path
         parsed_path = parse_path(full_path=source_path)
-
-        if parsed_path != "/":
-            parent_node = await dracoon.nodes.get_node_from_path(path=parsed_path)
-        elif parsed_path == "/":
+      
+        if parsed_path == "/":
             parent_node = None
             parent_id = 0
-
-        if parent_node:
+        else:
+            parent_node = await dracoon.nodes.get_node_from_path(path=parsed_path)
             parent_id = parent_node.id
 
         if parent_node is None and parsed_path != "/":
             await dracoon.logout()
             typer.echo(format_error_message(msg=f"Node not found: {parsed_path}"))
             sys.exit(1)
         if parent_node and parent_node.type == NodeType.file:
@@ -717,17 +717,21 @@
                     typer.echo(
                         format_error_message(
                             msg="Connection error - could not list nodes."
                         )
                     )
                     sys.exit(1)
 
-        if long_list and parent_id != 0 and human_readable:
-            typer.echo(f"total {to_readable_size(parent_node.size)}")
-        elif long_list and parent_id != 0:
+        if long_list and parent_node is not None and human_readable:
+            if parent_node.size:
+                size = parent_node.size
+            else:
+                size = 0
+            typer.echo(f"total {to_readable_size(size)}")
+        elif long_list and parent_node is not None:
             typer.echo(f"total {parent_node.size}")
 
         for node in nodes.items:
             format_and_print_node(
                 node=node,
                 inode=inode,
                 long_list=long_list,
@@ -857,15 +861,19 @@
                     format_error_message(
                         msg=f"Cannot write on target path ({target_dir_path})"
                     )
                 )
             finally:
                 await dracoon.logout()
         elif is_file_path:
-            transfer = DCTransferList(total=node_info.size, file_count=1)
+            if node_info.size:
+                size = node_info.size
+            else:
+                size = 0
+            transfer = DCTransferList(total=size, file_count=1)
             download_job = DCTransfer(transfer=transfer)
 
             try:
                 await dracoon.download(
                     file_path=parsed_path,
                     target_path=target_dir_path,
                     raise_on_err=True,
```

### Comparing `dccmd-0.4.1/dccmd/main/auth/__init__.py` & `dccmd-0.4.2/dccmd/main/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/auth/client.py` & `dccmd-0.4.2/dccmd/main/auth/client.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/auth/credentials.py` & `dccmd-0.4.2/dccmd/main/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/auth/util.py` & `dccmd-0.4.2/dccmd/main/auth/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/crypto/__init__.py` & `dccmd-0.4.2/dccmd/main/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/crypto/keys.py` & `dccmd-0.4.2/dccmd/main/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/crypto/util.py` & `dccmd-0.4.2/dccmd/main/crypto/util.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/download/__init__.py` & `dccmd-0.4.2/dccmd/main/download/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/models/__init__.py` & `dccmd-0.4.2/dccmd/main/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/models/errors.py` & `dccmd-0.4.2/dccmd/main/models/errors.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/rooms/__init__.py` & `dccmd-0.4.2/dccmd/main/rooms/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/rooms/permissions.py` & `dccmd-0.4.2/dccmd/main/rooms/permissions.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/rooms/print.py` & `dccmd-0.4.2/dccmd/main/rooms/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/upload/__init__.py` & `dccmd-0.4.2/dccmd/main/upload/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import platform
 import sys
 import asyncio
 from pathlib import Path
 
 import typer
 from httpx import WriteTimeout
-from dracoon import DRACOON
+from dracoon import DRACOON, OAuth2ConnectionType
 from dracoon.errors import (
     InvalidPathError,
     HTTPConflictError,
     HTTPForbiddenError,
     DRACOONHttpError,
 )
 from ..models import DCTransfer, DCTransferList
@@ -197,14 +197,16 @@
             asyncio.ensure_future(create_folder(name=item.name, parent_id=parent_id, dracoon=dracoon))
             for item in batch
         ]
 
         # process 10 folders per batch
         for reqs in dracoon.batch_process(coro_list=folder_reqs, batch_size=velocity):
             try:
+                # get new token to avoid rate limiting
+                await dracoon.connect(connection_type=OAuth2ConnectionType.refresh_token)
                 await asyncio.gather(*reqs)
             except HTTPConflictError:
                 pass
             except HTTPForbiddenError:
                 for req in folder_reqs:
                     req.cancel()
                 await dracoon.logout()
@@ -293,14 +295,16 @@
         )
         upload_reqs.append(asyncio.ensure_future(req))
 
     for batch in dracoon.batch_process(
             coro_list=upload_reqs, batch_size=concurrent_reqs
         ):
         try:
+            # get fresh token per batch (avoid rate limiting)
+            await dracoon.connect(connection_type=OAuth2ConnectionType.refresh_token)
             await asyncio.gather(*batch)
         except HTTPConflictError:
             # ignore file already exists error
             continue
         except HTTPForbiddenError:
             for req in upload_reqs:
                 req.cancel()
@@ -325,14 +329,14 @@
 
 def create_folder(name: str, parent_id: int, dracoon: DRACOON):
     """helper to create folder creation requests"""
 
     folder = dracoon.nodes.make_folder(name=name, parent_id=parent_id)
     return dracoon.nodes.create_folder(folder=folder, raise_on_err=True)
 
-def validate_file_name(name: str) -> str:
+def validate_file_name(name: str) -> bool:
     """ validate file name """
     # return false if name length is more than 150 chars
     if len(name) > 150:
         return False
 
     return True
```

### Comparing `dccmd-0.4.1/dccmd/main/users/__init__.py` & `dccmd-0.4.2/dccmd/main/users/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/users/manage.py` & `dccmd-0.4.2/dccmd/main/users/manage.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/users/print.py` & `dccmd-0.4.2/dccmd/main/users/print.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/dccmd/main/util/__init__.py` & `dccmd-0.4.2/dccmd/main/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dccmd-0.4.1/pyproject.toml` & `dccmd-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dccmd"
-version = "0.4.1"
+version = "0.4.2"
 description = "DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)"
 authors = ["Octavio Simone <70800577+unbekanntes-pferd@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dccmd-0.4.1/setup.py` & `dccmd-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,22 @@
  'typer>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['dccmd = dccmd:app']}
 
 setup_kwargs = {
     'name': 'dccmd',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)',
     'long_description': '<h1 align="center">DRACOON Commander</h1>\n\n\n## Table of Contents\n\n* [About the Project](#about-the-project)\n  * [Built With](#built-with)\n* [Getting Started](#getting-started)\n  * [Prerequisites](#prerequisites)\n  * [Installation](#installation)\n* [Usage](#usage)\n* [Configuration](#configuration)\n* [License](#license)\n\n\n## About the project\n_Disclaimer: This is an unofficial client and is not supported by DRACOON._<br>\nThis client is a CLI tool to perform basic commands in DRACOON and comes with the following functionalities:\n\n* Full support for S3 direct up- / download\n    * Chunked up- and downloads\n* Full support for DRACOON end-to-end encryption\n* Optimized for concurrent requests\n* Store credentials in OS-specific secure location\n    * Linux: Freedesktop Secret Service (secretstorage)\n    * macOS: Keychain\n    * Windows: Windows Credential Locker\n\n### Built With\n* [typer](https://typer.tiangolo.com)\n* [keyring](https://pypi.org/project/keyring)\n* [dracoon](https://github.com/unbekanntes-pferd/dracoon-python-api)\n    * [httpx](https://www.python-httpx.org/)\n* [poetry](https://python-poetry.org/)\n\nA full dependency list can be viewed in\n* [pyproject.toml](/pyproject.toml) - list of dependencies and project info\n* [poetry.lock](/poetry.lock)\n\nDRACOON Commander is built with typer as the CLI framework and uses keyring to store all credentials (OAuth2 tokens, client credentials and encryption password). \nThe tool is built on top of dracoon, an async API wrapper for DRACOON based on httpx.\nThe project is managed with poetry (dependencies, release build and publishing).\n\n## Getting Started\nIn order to get started, download the latest tarball from Github or install dccmd from pip:\n[Releases]()\n\n### Prerequisites\nYou need a working Python 3.10 installation – dccmd makes use of type annotations and uses 3.10 features.\nGet the latest Python version from: [python.org](https://python.org).\n\n```bash\npython3 --version\n```\n\nIn order to get going, you can install dccmd either in a virtual environment or globally.\n\n### Installation\n\nTo install a version, use `pip` and install the `dccmd` package.\n\n#### In a virtual environment\n```bash\nvirtualenv <DIR>\nsource <DIR>/bin/activate \npython3 -m pip install dccmd\n```\n#### Globally\n```bash\npython3 -m pip install dccmd\n```\n\n#### Set PATH\nIn order for the script to work, you might need to add the relevant script path to your PATH.\nWhen installing with pip, the output will already indicate if the path is present or not.\nIf you do not add the correct directory to PATH, you will *not* be able to use the `dccmd` command in your preferred shell.\n\n##### Windows\nIn Windows, just add the script path by editing the environment variables for your account:\nLook for an entry called \'Path\' and install the script directory from the `pip install` output.\n\n##### Unix\nOn Linux or macOS you can add a path to PATH by using the following command:<br>\n`export PATH="/your/directory/see/install/output:$PATH"`<br>\n\n\n## Usage\n\n### Display commands\n\nIn order to see all available commands, arguments and options, use the --help flag:\n```bash\ndccmd --help\n```\n\n```\nUsage: dccmd [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n  --help                          Show this message and exit.\n\nCommands:\n  auth\n  client\n  crypto\n  download  Download a file from DRACOON by providing a source path and a...\n  ls        List all nodes in a DRACOON path\n  mkdir     Create a folder in a DRACOON parent path\n  mkroom    Create a room (inherit permissions) in a DRACOON parent path\n  rm        Delete a file / folder / room in DRACOON\n  upload    Upload a file into DRACOON by providing a source path and a...\n```\nAll commands display their own help message, e.g. \n`dccmd upload --help`.\n\n### Client registration and authentication\n\nBefore you can perform any command, you must authenticate and set up the client.\nIf you enter any command which requires authentication (e.g. `dccmd ls your.dracoon.domain.com/`), you will be prompted first for a client configuration:\n* client id\n* client secret\n\n#### Client \nBefore you can use `dccmd` you need to generate a client in your DRACOON instance (config manager role required).\n1. Create a client with a client id and client secret.\nPlease make sure you have the following settings active:\n* Authorization code \n* Redirect URI is set to `https://your.dracoon.domain.com/oauth/callback`\n* Optional: If you wish to use the CLI mode (enter password and username via CLI), you can activate password flow \n\n2. Copy client id and client secret and use any command (e.g. `dccmd ls your.dracoon.domain.com/`).\n\n3. Enter client id and client secret – the information will be securely stored in your OS-specific secret container.\n\n#### Authentication\nOnce the client is set up, you will receive a link to authenticate via OAuth2 authorization code flow – you will then receive a code which you need to enter into the terminal.\nWhen completed, you will be prompted to store credentials securely (OS-specific).\n\nAdditionally, you can skip the authorization code flow and provide credentials directly, e.g. for the `dccmd ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/ --cli-mode username@mail.com topsecret123!\n```\n\n### Upload\n\n**Important: if you use Windows, you need to provide the path with \'/\' instead of \'\\\\\'!**\n\nYou can upload single files using the upload command:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/\n```\nIn order to upload a directory, use the `--recursive` (`-r`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/\n```\n\n#### Conflict resolution\nIf you upload a file which already exists (based on file name), the upload will be rejected.<br> \nIn order to force an overwrite, use the `--overwrite` flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --overwrite\n```\n\nIf you wish to auto-rename the file if it already exists, use the `auto-rename`flag:\n\n```bash\ndccmd upload /path/to/file.pdf your-dracoon.domain.com/ --auto-rename\n```\n\n#### Advanced usage\nIf you upload folders recursively, you might encounter performance issues, specifically when uploading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not upload a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\nIf you need to understand why uploads fail, you can also run the command using the `--debug` flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ --debug\n```\n*Note: This will have impact on performance as the log will be streamed to terminal and the log level will be increased to DEBUG.*\n\n### Create folder\n\nIf you wish to create a folder, use the `mkdir` command:\n\n```bash\ndccmd mkdir your-dracoon.domain.com/parent/newfolder\n```\nJust enter the full new path to create a folder. \nYou will need *create* permission to do so.\n\n\n### Create room\n\nIf you wish to create a room, use the `mkroom` command:\n\n```bash\ndccmd mkroom your-dracoon.domain.com/parent/newroom\n```\nJust enter the full new path to create a room. \nThe room will be created as a room with inherited permissions from the parent.\nYou will need *manage* permission to do so.\n\nTo create a room on the root level (\'/\'), you need to provide an admin user using \nthe corresponding option (`-au` or `--admin-user`):\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/newroom\n```\n*Note: In order to use the username of an OIDC user, you need to escape the `\\`, meaning you need to enter multiple slashes like so: `OIDC\\\\\\user.name`*\n\nTo create a room on any level that does *not* inherit permissions, use the `-au` (`--admin-user`) flag and provide the room admin when creating the room as with root level rooms:\n\n```bash\ndccmd mkroom -au "admin.username" your-dracoon.domain.com/parent-room/newroom\n```\n\n### Delete node\n\nIf you wish to delete a node, use the `rm` command:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/somefile.pdf\n```\nIn order to delete a container (room, folder) you need to use the `--recursive` (`r`) flag:\n\n```bash\ndccmd rm your-dracoon.domain.com/parent/folder/to/delete\n```\n**Warning: Deleting rooms cannot be undone!**\n\n### List nodes\n\nIn order to list all nodes, use the `ls` command:\n\n```bash\ndccmd ls your-dracoon.domain.com/\n```\n*Note: In order to list the root node, you need to provide a trailing `/`*\nFor a specific container (room or folder), use the path:\n```bash\ndccmd ls your-dracoon.domain.com/your/room\n```\n\n#### Displaying additional information\nUsing the `ls` command by default only provides node names.\nIn order to display more information, use relevant flags:\n\n* Display all information (size, last updated, last update user): `--long` (`-l`)\n    * Display sizes in human readable format (B, KB..): `--human-readable` (`-h`)\n* Display node id: `--inode` (`-i`)\n\nExample displaying full information:\n\n```bash\ndccmd ls -h -i -l your-dracoon.domain.com/your/room\n```\n### Download\n\nTo download a file, use the `download` command:\n\n```bash\ndccmd download your-dracoon.domain.com/your/cool-file.mp4 /target/directory\n```\n\nTo download a room or a folder, use the `download` command with `--recursive` (`-r`) flag:\n\n```bash\ndccmd download -r your-dracoon.domain.com/your/cool-folder /target/directory\n```\n\n#### Advanced usage\nIf you download folders recursively, you might encounter performance issues, specifically when downloading many small files. \nYou can therefore adjust concurrent file uploads via the `--velocity` (`-v`) flag:\n\n```bash\ndccmd upload -r /path/to/folder your-dracoon.domain.com/ -v 3\n```\nThe default value is 2 - it does not coincide with real request value.<br>\nMaximum (although not recommended) value is 10. Entering higher numbers will result in max value use.<br>\nMinimum value is 1 - this will not download a folder per file but is the minimum concurrent request value. Entering lower numbers will result in min value use.\n\n### User operations\n\nYou can list, edit and import users with relevant `dccmd users` command:\n\n* csv-import  Add a list of users to DRACOON from a CSV file\n* ls          Get a list of users in DRACOON\n* rm          Delete a user\n\n#### Importing users\n\nYou can import users by using the `csv-import` command and providing a path to the csv file:\n\n```bash\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/\n```\n\nThe csv file must contain a header and should include the following attributes:\n\n* first name\n* last name\n* email \n* login (optional)\n\nBy default, local users are created - if you want to import oidc users, you need pass the oidc config id:\n\n```bash\n#example with OIDC config 5\ndccmd users csv-import /path/to/users.csv your-dracoon.domain.com/ 5\n```\n\n#### Listing users\n\nYou can list all users using the `ls` command:\n\n```bash\ndccmd users ls your-dracoon.domain.com/\n```\n\nYou can get all users also as csv format by using the `--csv` flag:\n\n```bash\ndccmd users ls your-dracoon.domain.com/ --csv > users.csv\n```\n\nTo find a user, you can pass a search string to search for either first name, last name or user name (search string applies to all):\n\n```bash\n# will return all users with either first name, last name or user name containing \'yourname\'\ndccmd users ls your-dracoon.domain.com/ yourname\n```\n\n#### Deleting users\n\nYou can delete a user by providing the username:\n```bash\ndccmd users rm your-dracoon.domain.com/ user123\n```\n\n### Room permissions management\n\nFor an overview of the available commands use \n\n```bash\ndccmd rooms --help\n```\n\n#### List user / group permissions in a room\n\nTo list user permissions in a room, use the `list-users` command:\n\n```bash\ndccmd rooms list-users your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list users.\n\nTo list group permissions in a room, use the `list-groups` command:\n\n```bash\ndccmd rooms list-groups your-dracoon.domain.com/your-room\n```\nYou need minimum `read` permissions to list groups.\n\nAs with other commands, you can use the `--csv` flag to get a csv export for the room\npermissions (users and groups).\n\n#### Add user / group to a room\n\nCurrently, the following templates are available:\n- read: read-only perrmissions for a room \n- edit: edit permissions for a room\n- admin: room admin permissions\n\nThe permissions coincide with the templates in use of the official DRACOON Web App.\n\nYou need `manage` permissions (room admin) to add users / groups.\n\nTo add a user, use the `add-user` command and provide the user and permission template (`-u` and `-p`):\n\n```bash\ndccmd rooms add-user -u "user.name" -p admin your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `add-group` command and provide the group and permission template (`-g` and `-p`):\n\n```bash\ndccmd rooms add-group -g "group.name" -p admin your-dracoon.domain.com/your-room\n```\n\n#### Remove user / group from a room\n\nYou need `manage` permissions (room admin) to remove users / groups.\n\nTo add a user, use the `remove-user` command and provide the user (`-u`):\n\n```bash\ndccmd rooms remove-user -u "user.name" your-dracoon.domain.com/your-room\n```\n\nTo add a group, use the `remove-group` command and provide the group (`-g`):\n\n```bash\ndccmd rooms remove-group -g "group.name" your-dracoon.domain.com/your-room\n```\n\n## Configuration / administration\n\nYou can view / manage the configuration for `dccmd` using the relevant commands:\n\n* `dccmd auth` - manage credentials\n    * `dccmd auth ls your.dracoon.domain.com` will display if a refresh token has been stored for the provided domain\n    * `dccmd auth rm your-dracoon.domain.com` will remove stored credentials for the provided domain\n* `dccmd client` - manage client\n    * `dccmd client register your.dracoon.domain.com` will start the registration process for a client and given domain\n    * `dccmd client ls your.dracoon.domain.com` will display client information for the provided domain\n    * `dccmd client rm your-dracoon.domain.com` will remove the stored client config for the provided domain\n* `dccmd crypto` - manage encryption\n    * `dccmd crypto ls your.dracoon.domain.com` will display if encryption password is stored for the provided domain\n    * `dccmd crypto rm your-dracoon.domain.com` will remove the encryption password for the provided domain\n    * `dccmd crypto distribute your-dracoon.domain.com/` will generate file keys available to distribute - if providing a specific path (`dccmd crypto distribute your-dracoon.domain.com/some/path`), only keys for provided parent room will be generated.\n\n### Logging \nWhen using a command, a log will be created in the current working directory.\nCurrently it is not possible to configure a default path for a log.\n\nYou can stream the log to stdout by using the `--debug` flag with any DRACOON-specific command (`upload`, `download`, `ls`, `rm`, `mkdir`, `mkroom`).\n\n\n## License\nDistributed under the Apache License. See [LICENSE](/LICENSE) for more information.\n',
     'author': 'Octavio Simone',
     'author_email': '70800577+unbekanntes-pferd@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `dccmd-0.4.1/PKG-INFO` & `dccmd-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dccmd
-Version: 0.4.1
+Version: 0.4.2
 Summary: DRACOON Commander – CLI client for DRACOON Cloud (dracoon.com)
 License: Apache-2.0
 Author: Octavio Simone
 Author-email: 70800577+unbekanntes-pferd@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SecretStorage (>=3.3.1,<4.0.0)
 Requires-Dist: dracoon (>=1.10.0,<2.0.0)
 Requires-Dist: keyring (>=23.6.0,<24.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
```


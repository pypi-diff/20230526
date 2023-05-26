# Comparing `tmp/sidetrek-0.0.87.tar.gz` & `tmp/sidetrek-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidetrek-0.0.87.tar", max compression
+gzip compressed data, was "sidetrek-0.0.9.tar", max compression
```

## Comparing `sidetrek-0.0.87.tar` & `sidetrek-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,18 @@
--rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.87/README.md
--rw-r--r--   0        0        0      776 2023-05-26 21:13:07.802650 sidetrek-0.0.87/pyproject.toml
--rw-r--r--   0        0        0      604 2023-05-21 17:56:16.028060 sidetrek-0.0.87/sidetrek/__init__.py
--rw-r--r--   0        0        0     1850 2023-05-23 22:57:40.497644 sidetrek-0.0.87/sidetrek/cli.py
--rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.87/sidetrek/cli_commands/__init__.py
--rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.87/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      308 2023-05-23 22:40:50.433399 sidetrek-0.0.87/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0    10048 2023-05-26 21:00:46.560239 sidetrek-0.0.87/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     2851 2023-05-26 21:00:46.544542 sidetrek-0.0.87/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0      161 2023-05-21 20:54:49.328467 sidetrek-0.0.87/sidetrek/cli_commands/constants.py
--rw-r--r--   0        0        0    11949 2023-05-26 16:16:40.146266 sidetrek-0.0.87/sidetrek/cli_commands/helpers.py
--rw-r--r--   0        0        0     3841 2023-05-26 21:12:03.538765 sidetrek-0.0.87/sidetrek/cli_commands/workflow.py
--rw-r--r--   0        0        0    21676 2023-05-24 17:24:59.596079 sidetrek-0.0.87/sidetrek/collect_env.py
--rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.87/sidetrek/constants.py
--rw-r--r--   0        0        0     1114 2023-05-03 16:51:33.053983 sidetrek-0.0.87/sidetrek/datapipes.py
--rw-r--r--   0        0        0     4354 2023-05-26 15:36:54.943156 sidetrek-0.0.87/sidetrek/dataset.py
--rw-r--r--   0        0        0       15 2023-05-03 16:06:32.112969 sidetrek-0.0.87/sidetrek/flyte/__init__.py
--rw-r--r--   0        0        0      874 2023-05-09 03:56:32.928519 sidetrek-0.0.87/sidetrek/global_fns.py
--rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.87/sidetrek/loggers.py
--rw-r--r--   0        0        0        0 2023-05-07 17:03:01.499766 sidetrek-0.0.87/sidetrek/types/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 15:17:38.985798 sidetrek-0.0.87/sidetrek/types/dataset.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 sidetrek-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-03-09 16:33:17.090578 sidetrek-0.0.9/README.md
+-rw-r--r--   0        0        0      689 2023-04-09 00:09:19.420892 sidetrek-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-04-08 23:51:45.364985 sidetrek-0.0.9/sidetrek/__init__.py
+-rw-r--r--   0        0        0     1607 2023-03-30 15:37:18.710028 sidetrek-0.0.9/sidetrek/cli.py
+-rw-r--r--   0        0        0        0 2023-03-13 16:42:41.918418 sidetrek-0.0.9/sidetrek/cli_commands/__init__.py
+-rw-r--r--   0        0        0      174 2023-03-14 03:00:43.940526 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      388 2023-03-30 16:36:26.685225 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     8815 2023-04-06 20:18:36.881239 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     2395 2023-04-06 20:18:55.453228 sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-30 16:14:08.795493 sidetrek-0.0.9/sidetrek/cli_commands/constants.py
+-rw-r--r--   0        0        0     9970 2023-04-06 20:18:33.249911 sidetrek-0.0.9/sidetrek/cli_commands/helpers.py
+-rw-r--r--   0        0        0     3115 2023-04-06 20:19:34.857751 sidetrek-0.0.9/sidetrek/cli_commands/workflow.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:08:56.569055 sidetrek-0.0.9/sidetrek/core/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-02 20:04:34.987724 sidetrek-0.0.9/sidetrek/core/constants.py
+-rw-r--r--   0        0        0      491 2023-04-08 23:51:25.980013 sidetrek-0.0.9/sidetrek/core/global_fns.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:09:01.575253 sidetrek-0.0.9/sidetrek/loggers/__init__.py
+-rw-r--r--   0        0        0      661 2023-04-09 00:09:05.853814 sidetrek-0.0.9/sidetrek/loggers/loggers.py
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 sidetrek-0.0.9/PKG-INFO
```

### Comparing `sidetrek-0.0.87/pyproject.toml` & `sidetrek-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [tool.poetry]
 name = "sidetrek"
-version = "0.0.87"
+version = "0.0.9"
 description = ""
 authors = ["Seungchan Lee <seunggs@gmail.com>"]
 readme = "README.md"
 exclude = ["sidetrek/test/**"]
 
 [tool.poetry.scripts]
 sidetrek = "sidetrek.cli:app"
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.12"
+python = "^3.10,<3.11"
 typer = {extras = ["all"], version = "^0.7.0"}
 numba = "^0.56.4" # Required for mlflow: mlflow depends on old version of numba which won't install via poetry, so we had to manually include it here
-mlflow = "^2.0"
-flytekit = "^1.2.10,<=1.4.2"
+mlflow = "^2.2.1"
+flytekit = "<=1.4.2"
 requests = "^2.28.2"
 pylint = "^2.17.0"
-torchdata = "^0.6.0"
-fsspec = "^2023.4.0"
-s3fs = "^2023.4.0"
-bentoml = "^1.0.20"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sidetrek-0.0.87/sidetrek/__init__.py` & `sidetrek-0.0.9/sidetrek/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-from sidetrek.loggers import logger
-from sidetrek.global_fns import *
-
-
-__all__ = ["dataset", "types", "flyte", "cli_commands"]
-
+from sidetrek.loggers.loggers import logger
+from sidetrek.core.global_fns import *
 
 __doc__ = """
 sidetrek
 ================
 
 Description
 -----------
```

### Comparing `sidetrek-0.0.87/sidetrek/cli.py` & `sidetrek-0.0.9/sidetrek/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 import json
-import importlib
 from pathlib import Path
 import pickle
 import requests
 import typer
-from typing import Optional
-from typing_extensions import Annotated
 from rich import print
-from sidetrek.cli_commands import workflow
-from sidetrek.cli_commands.constants import APP_NAME
-from sidetrek.cli_commands.helpers import get_node_env, get_auth_api_base_url, version_callback
-
+from cli_commands import workflow
+from cli_commands.constants import NODE_ENV, APP_NAME
+from cli_commands.helpers import get_auth_api_base_url
 
 app = typer.Typer()
 
 app.add_typer(workflow.app, name="workflow")
 
-if get_node_env() != "production":
-    print(f"Environment: {get_node_env()}\n")
-
-
-@app.callback()
-def main(
-    version: bool = typer.Option(None, "--version", callback=version_callback, is_eager=True),
-):
-    return
+# if NODE_ENV == 'development':
+#     print(f"Environment: {NODE_ENV}\n")
+print(f"Environment: {NODE_ENV}\n")
 
 
 @app.command()
 def login(email: str = typer.Option(..., prompt=True), password: str = typer.Option(..., prompt=True, hide_input=True)):
     # Login and get refresh/access tokens
     try:
         auth_api_base_url = get_auth_api_base_url()
```

### Comparing `sidetrek-0.0.87/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc` & `sidetrek-0.0.9/sidetrek/cli_commands/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 16:22:49 2023 UTC, .py size: 3861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,150 @@
-00000000: 6f0d 0d0a 0000 0000 d9dc 7064 150f 0000  o.........pd....
+00000000: 6f0d 0d0a 0000 0000 2c29 2f64 590c 0000  o.......,)/dY...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c04 6d05 5a05 0100 6400 6401 6c06  d.l.m.Z...d.d.l.
-00000060: 5a06 6400 6401 6c07 5a07 6400 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6405 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
-00000090: 6d0e 5a0e 0100 6400 6406 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-000000a0: 6d11 5a11 6d12 5a12 6d13 5a13 6d14 5a14  m.Z.m.Z.m.Z.m.Z.
-000000b0: 6d15 5a15 6d16 5a16 0100 6506 a017 a100  m.Z.m.Z...e.....
-000000c0: 5a18 6518 a019 a100 6506 a01a 6407 a101  Z.e.....e...d...
-000000d0: 6408 6602 6409 651b 640a 651c 6604 640b  d.f.d.e.d.e.f.d.
-000000e0: 640c 8405 8301 5a1d 6401 5300 290d e900  d.....Z.d.S.)...
-000000f0: 0000 004e 2901 da04 5061 7468 2901 da05  ...N)...Path)...
-00000100: 736c 6565 7029 01da 0570 7269 6e74 2903  sleep)...print).
-00000110: da08 5072 6f67 7265 7373 da0d 5370 696e  ..Progress..Spin
-00000120: 6e65 7243 6f6c 756d 6eda 0a54 6578 7443  nerColumn..TextC
-00000130: 6f6c 756d 6e29 07da 1067 6574 5f63 7572  olumn)...get_cur
-00000140: 7265 6e74 5f75 7365 72da 0d67 6574 5f61  rent_user..get_a
-00000150: 7773 5f63 7265 6473 da25 6765 745f 6765  ws_creds.%get_ge
-00000160: 6e65 7261 7465 645f 6c6f 6361 6c5f 7369  nerated_local_si
-00000170: 6465 7472 656b 5f64 6972 5f70 6174 68da  detrek_dir_path.
-00000180: 1b67 6574 5f67 656e 6572 6174 6564 5f77  .get_generated_w
-00000190: 6f72 6b66 6c6f 775f 6e61 6d65 da21 646f  orkflow_name.!do
-000001a0: 776e 6c6f 6164 5f67 656e 6572 6174 6564  wnload_generated
-000001b0: 5f66 6c79 7465 5f77 6f72 6b66 6c6f 77da  _flyte_workflow.
-000001c0: 1a67 6574 5f77 6f72 6b66 6c6f 775f 6472  .get_workflow_dr
-000001d0: 6166 745f 7665 7273 696f 6eda 0b70 7269  aft_version..pri
-000001e0: 6e74 5f74 696d 6572 2e7a 027b 7dda 0b77  nt_timer.z.{}..w
-000001f0: 6f72 6b66 6c6f 775f 6964 da0d 776f 726b  orkflow_id..work
-00000200: 666c 6f77 5f61 7267 7363 0200 0000 0000  flow_argsc......
-00000210: 0000 0000 0000 1100 0000 0900 0000 4300  ..............C.
-00000220: 0000 730c 0200 0074 00a0 00a1 007d 0274  ..s....t.....}.t
-00000230: 0174 0283 0074 0364 0183 0164 0264 038d  .t...t.d...d.d..
-00000240: 038f ee7d 0374 0464 0474 0583 0083 0201  ...}.t.d.t......
-00000250: 007c 036a 0664 0564 0664 078d 027d 0474  .|.j.d.d.d...}.t
-00000260: 0783 007d 0574 0464 087c 059b 009d 0283  ...}.t.d.|......
-00000270: 0101 007c 03a0 087c 04a1 0101 0074 0974  ...|...|.....t.t
-00000280: 00a0 00a1 007c 0218 0064 0983 027d 0674  .....|...d...}.t
-00000290: 0464 0a7c 069b 0064 0b9d 0383 0101 007c  .d.|...d.......|
-000002a0: 036a 0664 0c64 0664 078d 027d 0774 0a7c  .j.d.d.d...}.t.|
-000002b0: 0064 0d8d 017d 0874 0b7c 0564 0e19 007c  .d...}.t.|.d...|
-000002c0: 0864 0f8d 027d 0974 0c7c 0083 017d 0a7c  .d...}.t.|...}.|
-000002d0: 03a0 087c 07a1 0101 0074 0974 00a0 00a1  ...|.....t.t....
-000002e0: 007c 0218 0064 0983 027d 0674 0464 107c  .|...d...}.t.d.|
-000002f0: 069b 0064 117c 09a0 0da1 009b 009d 0483  ...d.|..........
-00000300: 0101 0074 0e83 007d 0b74 0464 127c 0b9b  ...t...}.t.d.|..
-00000310: 009d 0283 0101 007c 036a 0664 1364 0664  .......|.j.d.d.d
-00000320: 078d 027d 0c74 0f6a 1064 1464 157c 097c  ...}.t.j.d.d.|.|
-00000330: 0a64 167c 0167 0674 0583 0074 0f6a 1174  .d.|.g.t...t.j.t
-00000340: 0f6a 1164 1764 0264 188d 068f 517d 0d7c  .j.d.d.d....Q}.|
-00000350: 0d6a 1244 005d 087d 0e74 047c 0e64 1964  .j.D.].}.t.|.d.d
-00000360: 1a8d 0201 0071 977c 0da0 13a1 005c 027d  .....q.|.....\.}
-00000370: 0f7d 107c 0d6a 1464 1b6b 0372 c774 0974  .}.|.j.d.k.r.t.t
-00000380: 00a0 00a1 007c 0218 0064 0983 027d 0674  .....|...d...}.t
-00000390: 0464 1c7c 109b 009d 0283 0101 0074 0464  .d.|.........t.d
-000003a0: 1d7c 069b 0064 0b9d 0383 0101 0074 15a0  .|...d.......t..
-000003b0: 16a1 0082 017c 03a0 087c 0ca1 0101 0074  .....|...|.....t
-000003c0: 0974 00a0 00a1 007c 0218 0064 0983 027d  .t.....|...d...}
-000003d0: 0674 0464 1e7c 069b 0064 0b9d 0383 0101  .t.d.|...d......
-000003e0: 0057 0064 0604 0004 0083 0301 006e 1031  .W.d.........n.1
-000003f0: 0073 e777 0101 0001 0001 0059 0001 0057  .s.w.......Y...W
-00000400: 0064 0604 0004 0083 0301 0064 0653 0057  .d.........d.S.W
-00000410: 0064 0604 0004 0083 0301 0064 0653 0031  .d.........d.S.1
-00000420: 0073 ff77 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-00000430: 0653 0029 1f61 3301 0000 0a20 2020 2045  .S.).a3....    E
-00000440: 7865 6375 7465 2074 6865 2077 6f72 6b66  xecute the workf
-00000450: 6c6f 7720 6c6f 6361 6c6c 7920 2865 2e67  low locally (e.g
-00000460: 2e20 666f 7220 7465 7374 696e 6729 2e0a  . for testing)..
-00000470: 0a20 2020 202a 2059 6f75 2063 616e 2072  .    * You can r
-00000480: 6574 7269 6576 6520 7468 6520 2d2d 776f  etrieve the --wo
-00000490: 726b 666c 6f77 2d69 6420 2865 2e67 2e20  rkflow-id (e.g. 
-000004a0: 3432 2920 6672 6f6d 2053 6964 6574 7265  42) from Sidetre
-000004b0: 6b20 6170 702e 0a20 2020 202a 2057 6f72  k app..    * Wor
-000004c0: 6b66 6c6f 7720 7665 7273 696f 6e20 7573  kflow version us
-000004d0: 6564 2069 7420 616c 7761 7973 2060 6472  ed it always `dr
-000004e0: 6166 7460 2066 6f72 2074 6869 7320 636f  aft` for this co
-000004f0: 6d6d 616e 640a 2020 2020 2a20 2d2d 776f  mmand.    * --wo
-00000500: 726b 666c 6f77 2d61 7267 7320 6973 2061  rkflow-args is a
-00000510: 2073 7472 696e 6769 6669 6564 204a 534f   stringified JSO
-00000520: 4e20 6f66 2079 6f75 7220 776f 726b 666c  N of your workfl
-00000530: 6f77 2061 7267 756d 656e 7473 2028 652e  ow arguments (e.
-00000540: 672e 2027 7b22 6c65 6172 6e69 6e67 5f72  g. '{"learning_r
-00000550: 6174 6522 3d30 2e31 2c20 2265 706f 6368  ate"=0.1, "epoch
-00000560: 7322 3d35 7d27 292e 0a20 2020 207a 285b  s"=5}')..    z([
-00000570: 7072 6f67 7265 7373 2e64 6573 6372 6970  progress.descrip
-00000580: 7469 6f6e 5d7b 7461 736b 2e64 6573 6372  tion]{task.descr
-00000590: 6970 7469 6f6e 7d54 2901 5a09 7472 616e  iption}T).Z.tran
-000005a0: 7369 656e 745a 2167 656e 6572 6174 6564  sientZ!generated
-000005b0: 5f6c 6f63 616c 5f73 6964 6574 7265 6b5f  _local_sidetrek_
-000005c0: 6469 725f 7061 7468 7a11 4175 7468 656e  dir_pathz.Authen
-000005d0: 7469 6361 7469 6e67 2e2e 2e4e 2902 da0b  ticating...N)...
-000005e0: 6465 7363 7269 7074 696f 6eda 0574 6f74  description..tot
-000005f0: 616c 7a0d 6375 7272 656e 745f 7573 6572  alz.current_user
-00000600: 3de9 0200 0000 752c 0000 005b 6772 6565  =.....u,...[gree
-00000610: 6e5d e29c 94ef b88f 205b 7768 6974 655d  n]...... [white]
-00000620: 4175 7468 656e 7469 6361 7465 6420 5b67  Authenticated [g
-00000630: 7265 7938 395d 287a 0273 297a 1a47 656e  rey89](z.s)z.Gen
-00000640: 6572 6174 696e 6720 7468 6520 776f 726b  erating the work
-00000650: 666c 6f77 2e2e 2e29 0172 0f00 0000 da02  flow...).r......
-00000660: 6964 2902 da07 7573 6572 5f69 64da 1077  id)...user_id..w
-00000670: 6f72 6b66 6c6f 775f 7665 7273 696f 6e75  orkflow_versionu
-00000680: 3100 0000 5b67 7265 656e 5de2 9c94 efb8  1...[green].....
-00000690: 8f20 5b77 6869 7465 5d57 6f72 6b66 6c6f  . [white]Workflo
-000006a0: 7720 6765 6e65 7261 7465 6420 5b67 7265  w generated [gre
-000006b0: 7938 395d 287a 1973 2920 2d20 6765 6e65  y89](z.s) - gene
-000006c0: 7261 7465 6420 776f 726b 666c 6f77 3a20  rated workflow: 
-000006d0: 7a0a 6177 735f 6372 6564 733d 7a19 4578  z.aws_creds=z.Ex
-000006e0: 6563 7574 696e 6720 7468 6520 776f 726b  ecuting the work
-000006f0: 666c 6f77 2e2e 2e5a 0770 7966 6c79 7465  flow...Z.pyflyte
-00000700: da03 7275 6e7a 0a2d 2d5f 7766 5f61 7267  ..runz.--_wf_arg
-00000710: 73e9 0100 0000 2905 da03 6377 64da 0673  s.....)...cwd..s
-00000720: 7464 6f75 74da 0673 7464 6572 72da 0762  tdout..stderr..b
-00000730: 7566 7369 7a65 da12 756e 6976 6572 7361  ufsize..universa
-00000740: 6c5f 6e65 776c 696e 6573 da00 2901 da03  l_newlines..)...
-00000750: 656e 6472 0100 0000 7a0d 5b6c 6967 6874  endr....z.[light
-00000760: 5f63 6f72 616c 5d75 3300 0000 5b72 6564  _coral]u3...[red
-00000770: 5de2 9c95 205b 7768 6974 655d 576f 726b  ]... [white]Work
-00000780: 666c 6f77 2065 7865 6375 7469 6f6e 2066  flow execution f
-00000790: 6169 6c65 6420 5b67 7265 7938 395d 2875  ailed [grey89](u
-000007a0: 4000 0000 5b67 7265 656e 5de2 9c94 efb8  @...[green].....
-000007b0: 8f20 5b77 6869 7465 5d57 6f72 6b66 6c6f  . [white]Workflo
-000007c0: 7720 6578 6563 7574 696f 6e20 636f 6d70  w execution comp
-000007d0: 6c65 7465 6420 f09f 8e89 205b 6772 6579  leted .... [grey
-000007e0: 3839 5d28 2917 da04 7469 6d65 7205 0000  89]()...timer...
-000007f0: 0072 0600 0000 7207 0000 0072 0400 0000  .r....r....r....
-00000800: 720a 0000 005a 0861 6464 5f74 6173 6b72  r....Z.add_taskr
-00000810: 0800 0000 5a0b 7265 6d6f 7665 5f74 6173  ....Z.remove_tas
-00000820: 6bda 0572 6f75 6e64 720d 0000 0072 0c00  k..roundr....r..
-00000830: 0000 720b 0000 00da 0861 735f 706f 7369  ..r......as_posi
-00000840: 7872 0900 0000 da0a 7375 6270 726f 6365  xr......subproce
-00000850: 7373 da05 506f 7065 6eda 0450 4950 4572  ss..Popen..PIPEr
-00000860: 1a00 0000 da0b 636f 6d6d 756e 6963 6174  ......communicat
-00000870: 65da 0a72 6574 7572 6e63 6f64 65da 0574  e..returncode..t
-00000880: 7970 6572 da04 4578 6974 2911 720f 0000  yper..Exit).r...
-00000890: 0072 1000 0000 da0a 7374 6172 745f 7469  .r......start_ti
-000008a0: 6d65 da08 7072 6f67 7265 7373 5a09 6175  me..progressZ.au
-000008b0: 7468 5f73 7465 70da 0c63 7572 7265 6e74  th_step..current
-000008c0: 5f75 7365 725a 0c74 696d 655f 656c 6170  _userZ.time_elap
-000008d0: 7365 645a 1277 665f 6765 6e65 7261 7469  sedZ.wf_generati
-000008e0: 6f6e 5f73 7465 7072 1600 0000 5a0c 7766  on_stepr....Z.wf
-000008f0: 5f66 696c 655f 7061 7468 5a11 6765 6e65  _file_pathZ.gene
-00000900: 7261 7465 645f 7766 5f6e 616d 655a 0961  rated_wf_nameZ.a
-00000910: 7773 5f63 7265 6473 5a11 7766 5f65 7865  ws_credsZ.wf_exe
-00000920: 6375 7469 6f6e 5f73 7465 70da 0770 726f  cution_step..pro
-00000930: 6365 7373 da04 6c69 6e65 da01 5fda 0565  cess..line.._..e
-00000940: 7272 6f72 a900 7231 0000 00fa 512f 5573  rror..r1....Q/Us
-00000950: 6572 732f 7365 756e 6763 6861 6e6c 6565  ers/seungchanlee
-00000960: 2f44 6f63 756d 656e 7473 2f53 6964 6574  /Documents/Sidet
-00000970: 7265 6b2f 7369 6465 7472 656b 2f73 6964  rek/sidetrek/sid
-00000980: 6574 7265 6b2f 636c 695f 636f 6d6d 616e  etrek/cli_comman
-00000990: 6473 2f77 6f72 6b66 6c6f 772e 7079 7217  ds/workflow.pyr.
-000009a0: 0000 0018 0000 0073 6000 0000 0809 0202  .......s`.......
-000009b0: 0401 0601 0201 06fd 0204 0c01 0e06 0601  ................
-000009c0: 0e01 0a01 1201 1001 0e03 0a01 1004 0801  ................
-000009d0: 0a01 1201 1801 0603 0e01 0e03 0402 0e01  ................
-000009e0: 0401 0401 0401 0201 0201 06fa 0208 0a01  ................
-000009f0: 0e01 0c02 0a02 1201 0e01 1001 0801 0a02  ................
-00000a00: 1201 1201 1eea 0edb 0225 22db 7217 0000  .........%".r...
-00000a10: 0029 1eda 026f 73da 0373 7973 7220 0000  .)...os..sysr ..
-00000a20: 00da 0974 6872 6561 6469 6e67 da07 7061  ...threading..pa
-00000a30: 7468 6c69 6272 0200 0000 7228 0000 0072  thlibr....r(...r
-00000a40: 2300 0000 7203 0000 00da 0472 6963 6872  #...r......richr
-00000a50: 0400 0000 5a0d 7269 6368 2e70 726f 6772  ....Z.rich.progr
-00000a60: 6573 7372 0500 0000 7206 0000 0072 0700  essr....r....r..
-00000a70: 0000 da1d 7369 6465 7472 656b 2e63 6c69  ....sidetrek.cli
-00000a80: 5f63 6f6d 6d61 6e64 732e 6865 6c70 6572  _commands.helper
-00000a90: 7372 0800 0000 7209 0000 0072 0a00 0000  sr....r....r....
-00000aa0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
-00000ab0: 0e00 0000 da05 5479 7065 72da 0361 7070  ......Typer..app
-00000ac0: da07 636f 6d6d 616e 64da 064f 7074 696f  ..command..Optio
-00000ad0: 6eda 0369 6e74 da03 7374 7272 1700 0000  n..int..strr....
-00000ae0: 7231 0000 0072 3100 0000 7231 0000 0072  r1...r1...r1...r
-00000af0: 3200 0000 da08 3c6d 6f64 756c 653e 0100  2.....<module>..
-00000b00: 0000 731c 0000 0008 0008 0108 0108 010c  ..s.............
-00000b10: 0108 0108 010c 010c 0114 0124 0108 0a06  ...........$....
-00000b20: 0324 01                                  .$.
+00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6400 6401 6c05 5a05 6400 6401 6c06  ..d.d.l.Z.d.d.l.
+00000060: 5a06 6400 6403 6c01 6d07 5a07 0100 6400  Z.d.d.l.m.Z...d.
+00000070: 6404 6c08 6d09 5a09 0100 6400 6405 6c0a  d.l.m.Z...d.d.l.
+00000080: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6400  m.Z.m.Z.m.Z...d.
+00000090: 6406 6c0e 6d0f 5a0f 6d10 5a10 6d11 5a11  d.l.m.Z.m.Z.m.Z.
+000000a0: 6d12 5a12 6d13 5a13 6d14 5a14 0100 6505  m.Z.m.Z.m.Z...e.
+000000b0: a015 a100 5a16 6516 a017 a100 6505 a018  ....Z.e.....e...
+000000c0: 6407 a101 6408 6602 6409 6519 640a 651a  d...d.f.d.e.d.e.
+000000d0: 6604 640b 640c 8405 8301 5a1b 6401 5300  f.d.d.....Z.d.S.
+000000e0: 290d e900 0000 004e 2901 da04 5061 7468  )......N)...Path
+000000f0: 2901 da05 736c 6565 7029 01da 0570 7269  )...sleep)...pri
+00000100: 6e74 2903 da08 5072 6f67 7265 7373 da0d  nt)...Progress..
+00000110: 5370 696e 6e65 7243 6f6c 756d 6eda 0a54  SpinnerColumn..T
+00000120: 6578 7443 6f6c 756d 6e29 06da 1067 6574  extColumn)...get
+00000130: 5f63 7572 7265 6e74 5f75 7365 72da 2567  _current_user.%g
+00000140: 6574 5f67 656e 6572 6174 6564 5f6c 6f63  et_generated_loc
+00000150: 616c 5f73 6964 6574 7265 6b5f 6469 725f  al_sidetrek_dir_
+00000160: 7061 7468 da1b 6765 745f 6765 6e65 7261  path..get_genera
+00000170: 7465 645f 776f 726b 666c 6f77 5f6e 616d  ted_workflow_nam
+00000180: 65da 2164 6f77 6e6c 6f61 645f 6765 6e65  e.!download_gene
+00000190: 7261 7465 645f 666c 7974 655f 776f 726b  rated_flyte_work
+000001a0: 666c 6f77 da1a 6765 745f 776f 726b 666c  flow..get_workfl
+000001b0: 6f77 5f64 7261 6674 5f76 6572 7369 6f6e  ow_draft_version
+000001c0: da0b 7072 696e 745f 7469 6d65 722e 7a02  ..print_timer.z.
+000001d0: 7b7d da0b 776f 726b 666c 6f77 5f69 64da  {}..workflow_id.
+000001e0: 0d77 6f72 6b66 6c6f 775f 6172 6773 6302  .workflow_argsc.
+000001f0: 0000 0000 0000 0000 0000 000d 0000 0009  ................
+00000200: 0000 0043 0000 0073 7e01 0000 7400 7401  ...C...s~...t.t.
+00000210: 8300 7402 6401 8301 6402 6403 8d03 8fab  ..t.d...d.d.....
+00000220: 7d02 7403 6404 7404 8300 8302 0100 7c02  }.t.d.t.......|.
+00000230: 6a05 6405 6406 6407 8d02 7d03 7406 8300  j.d.d.d...}.t...
+00000240: 7d04 7c02 a007 7c03 a101 0100 7403 6408  }.|...|.....t.d.
+00000250: 8301 0100 7c02 6a05 6409 6406 6407 8d02  ....|.j.d.d.d...
+00000260: 7d05 7408 7c00 640a 8d01 7d06 7409 7c04  }.t.|.d...}.t.|.
+00000270: 640b 1900 7c06 640c 8d02 7d07 7403 640d  d...|.d...}.t.d.
+00000280: 7c07 9b00 9d02 8301 0100 740a 7c00 8301  |.........t.|...
+00000290: 7d08 7c02 a007 7c05 a101 0100 7403 640e  }.|...|.....t.d.
+000002a0: 8301 0100 7c02 6a05 640f 6406 6407 8d02  ....|.j.d.d.d...
+000002b0: 7d09 740b 6a0c 6410 6411 7c07 7c08 6412  }.t.j.d.d.|.|.d.
+000002c0: 7c01 6706 7404 8300 740b 6a0d 740b 6a0d  |.g.t...t.j.t.j.
+000002d0: 6413 8d04 8f38 7d0a 7c0a a00e a100 5c02  d....8}.|.....\.
+000002e0: 7d0b 7d0c 7c0a 6a0f 6414 6b03 7283 7403  }.}.|.j.d.k.r.t.
+000002f0: 6415 7c0c a010 6416 a101 9b00 9d02 8301  d.|...d.........
+00000300: 0100 7403 6417 8301 0100 7411 a012 a100  ..t.d.....t.....
+00000310: 8201 7403 6418 7c0b a010 6416 a101 9b00  ..t.d.|...d.....
+00000320: 9d02 8301 0100 7c02 a007 7c09 a101 0100  ......|...|.....
+00000330: 7403 6419 8301 0100 5700 6406 0400 0400  t.d.....W.d.....
+00000340: 8303 0100 6e10 3100 73a0 7701 0100 0100  ....n.1.s.w.....
+00000350: 0100 5900 0100 5700 6406 0400 0400 8303  ..Y...W.d.......
+00000360: 0100 6406 5300 5700 6406 0400 0400 8303  ..d.S.W.d.......
+00000370: 0100 6406 5300 3100 73b8 7701 0100 0100  ..d.S.1.s.w.....
+00000380: 0100 5900 0100 6406 5300 291a 7af0 0a20  ..Y...d.S.).z.. 
+00000390: 2020 2045 7865 6375 7465 2074 6865 2077     Execute the w
+000003a0: 6f72 6b66 6c6f 7720 6c6f 6361 6c6c 7920  orkflow locally 
+000003b0: 2865 2e67 2e20 666f 7220 7465 7374 696e  (e.g. for testin
+000003c0: 6729 2e0a 0a20 2020 2059 6f75 2063 616e  g)...    You can
+000003d0: 2072 6574 7269 6576 6520 7468 6520 2d2d   retrieve the --
+000003e0: 776f 726b 666c 6f77 2d69 6420 2865 2e67  workflow-id (e.g
+000003f0: 2e20 3432 2920 6672 6f6d 2053 6964 6574  . 42) from Sidet
+00000400: 7265 6b20 6170 702e 0a20 2020 202d 2d77  rek app..    --w
+00000410: 6f72 6b66 6c6f 772d 6172 6773 2069 7320  orkflow-args is 
+00000420: 6120 7374 7269 6e67 6966 6965 6420 4a53  a stringified JS
+00000430: 4f4e 206f 6620 796f 7572 2077 6f72 6b66  ON of your workf
+00000440: 6c6f 7720 6172 6775 6d65 6e74 7320 2865  low arguments (e
+00000450: 2e67 2e20 277b 226c 6561 726e 696e 675f  .g. '{"learning_
+00000460: 7261 7465 223d 302e 312c 2022 6570 6f63  rate"=0.1, "epoc
+00000470: 6873 223d 357d 2729 2e0a 2020 2020 7a28  hs"=5}')..    z(
+00000480: 5b70 726f 6772 6573 732e 6465 7363 7269  [progress.descri
+00000490: 7074 696f 6e5d 7b74 6173 6b2e 6465 7363  ption]{task.desc
+000004a0: 7269 7074 696f 6e7d 5429 015a 0974 7261  ription}T).Z.tra
+000004b0: 6e73 6965 6e74 5a21 6765 6e65 7261 7465  nsientZ!generate
+000004c0: 645f 6c6f 6361 6c5f 7369 6465 7472 656b  d_local_sidetrek
+000004d0: 5f64 6972 5f70 6174 687a 1141 7574 6865  _dir_pathz.Authe
+000004e0: 6e74 6963 6174 696e 672e 2e2e 4e29 02da  nticating...N)..
+000004f0: 0b64 6573 6372 6970 7469 6f6e da05 746f  .description..to
+00000500: 7461 6c75 2200 0000 5b67 7265 656e 5de2  talu"...[green].
+00000510: 9c94 efb8 8f20 5b77 6869 7465 5d41 7574  ..... [white]Aut
+00000520: 6865 6e74 6963 6174 6564 7a1a 4765 6e65  henticatedz.Gene
+00000530: 7261 7469 6e67 2074 6865 2077 6f72 6b66  rating the workf
+00000540: 6c6f 772e 2e2e 2901 720e 0000 00da 0269  low...).r......i
+00000550: 6429 02da 0775 7365 725f 6964 da10 776f  d)...user_id..wo
+00000560: 726b 666c 6f77 5f76 6572 7369 6f6e 7a0d  rkflow_versionz.
+00000570: 7766 5f66 696c 655f 7061 7468 3d75 2700  wf_file_path=u'.
+00000580: 0000 5b67 7265 656e 5de2 9c94 efb8 8f20  ..[green]...... 
+00000590: 5b77 6869 7465 5d57 6f72 6b66 6c6f 7720  [white]Workflow 
+000005a0: 6765 6e65 7261 7465 647a 1945 7865 6375  generatedz.Execu
+000005b0: 7469 6e67 2074 6865 2077 6f72 6b66 6c6f  ting the workflo
+000005c0: 772e 2e2e 5a07 7079 666c 7974 65da 0372  w...Z.pyflyte..r
+000005d0: 756e 7a0a 2d2d 5f77 665f 6172 6773 2903  unz.--_wf_args).
+000005e0: da03 6377 64da 0673 7464 6f75 74da 0673  ..cwd..stdout..s
+000005f0: 7464 6572 7272 0100 0000 7a0d 5b6c 6967  tderrr....z.[lig
+00000600: 6874 5f63 6f72 616c 5d7a 0575 7466 2d38  ht_coral]z.utf-8
+00000610: 7529 0000 005b 7265 645d e29c 9520 5b77  u)...[red]... [w
+00000620: 6869 7465 5d57 6f72 6b66 6c6f 7720 6578  hite]Workflow ex
+00000630: 6563 7574 696f 6e20 6661 696c 6564 7a07  ecution failedz.
+00000640: 5b67 7265 656e 5d75 3600 0000 5b67 7265  [green]u6...[gre
+00000650: 656e 5de2 9c94 efb8 8f20 5b77 6869 7465  en]...... [white
+00000660: 5d57 6f72 6b66 6c6f 7720 6578 6563 7574  ]Workflow execut
+00000670: 696f 6e20 636f 6d70 6c65 7465 6420 f09f  ion completed ..
+00000680: 8e89 2913 7205 0000 0072 0600 0000 7207  ..).r....r....r.
+00000690: 0000 0072 0400 0000 7209 0000 005a 0861  ...r....r....Z.a
+000006a0: 6464 5f74 6173 6b72 0800 0000 5a0b 7265  dd_taskr....Z.re
+000006b0: 6d6f 7665 5f74 6173 6b72 0c00 0000 720b  move_taskr....r.
+000006c0: 0000 0072 0a00 0000 da0a 7375 6270 726f  ...r......subpro
+000006d0: 6365 7373 da05 506f 7065 6eda 0450 4950  cess..Popen..PIP
+000006e0: 45da 0b63 6f6d 6d75 6e69 6361 7465 da0a  E..communicate..
+000006f0: 7265 7475 726e 636f 6465 da06 6465 636f  returncode..deco
+00000700: 6465 da05 7479 7065 72da 0445 7869 7429  de..typer..Exit)
+00000710: 0d72 0e00 0000 720f 0000 00da 0870 726f  .r....r......pro
+00000720: 6772 6573 735a 0961 7574 685f 7374 6570  gressZ.auth_step
+00000730: da0c 6375 7272 656e 745f 7573 6572 5a12  ..current_userZ.
+00000740: 7766 5f67 656e 6572 6174 696f 6e5f 7374  wf_generation_st
+00000750: 6570 7214 0000 005a 0c77 665f 6669 6c65  epr....Z.wf_file
+00000760: 5f70 6174 685a 1167 656e 6572 6174 6564  _pathZ.generated
+00000770: 5f77 665f 6e61 6d65 5a11 7766 5f65 7865  _wf_nameZ.wf_exe
+00000780: 6375 7469 6f6e 5f73 7465 70da 0770 726f  cution_step..pro
+00000790: 6365 7373 da06 6f75 7470 7574 da05 6572  cess..output..er
+000007a0: 726f 72a9 0072 2600 0000 fa51 2f55 7365  ror..r&....Q/Use
+000007b0: 7273 2f73 6575 6e67 6368 616e 6c65 652f  rs/seungchanlee/
+000007c0: 446f 6375 6d65 6e74 732f 5369 6465 7472  Documents/Sidetr
+000007d0: 656b 2f73 6964 6574 7265 6b2f 7369 6465  ek/sidetrek/side
+000007e0: 7472 656b 2f63 6c69 5f63 6f6d 6d61 6e64  trek/cli_command
+000007f0: 732f 776f 726b 666c 6f77 2e70 7972 1500  s/workflow.pyr..
+00000800: 0000 1600 0000 734c 0000 0002 0904 0106  ......sL........
+00000810: 0102 0106 fd02 040c 010e 0606 010a 0108  ................
+00000820: 010e 030a 0110 040e 0108 010a 0108 010e  ................
+00000830: 0204 010e 0204 0104 0104 0106 fb02 060c  ................
+00000840: 010a 0214 0108 0108 0114 020a 020a 011e  ................
+00000850: ef0e e302 1d22 e372 1500 0000 291c da03  .....".r....)...
+00000860: 7379 73da 0474 696d 65da 0974 6872 6561  sys..time..threa
+00000870: 6469 6e67 da07 7061 7468 6c69 6272 0200  ding..pathlibr..
+00000880: 0000 721f 0000 0072 1900 0000 7203 0000  ..r....r....r...
+00000890: 00da 0472 6963 6872 0400 0000 5a0d 7269  ...richr....Z.ri
+000008a0: 6368 2e70 726f 6772 6573 7372 0500 0000  ch.progressr....
+000008b0: 7206 0000 0072 0700 0000 da14 636c 695f  r....r......cli_
+000008c0: 636f 6d6d 616e 6473 2e68 656c 7065 7273  commands.helpers
+000008d0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000008e0: 0b00 0000 720c 0000 0072 0d00 0000 da05  ....r....r......
+000008f0: 5479 7065 72da 0361 7070 da07 636f 6d6d  Typer..app..comm
+00000900: 616e 64da 064f 7074 696f 6eda 0369 6e74  and..Option..int
+00000910: da03 7374 7272 1500 0000 7226 0000 0072  ..strr....r&...r
+00000920: 2600 0000 7226 0000 0072 2700 0000 da08  &...r&...r'.....
+00000930: 3c6d 6f64 756c 653e 0100 0000 731a 0000  <module>....s...
+00000940: 0008 0008 0108 010c 0108 0108 010c 010c  ................
+00000950: 0114 0120 0108 0906 0324 01              ... .....$.
```

### Comparing `sidetrek-0.0.87/sidetrek/cli_commands/helpers.py` & `sidetrek-0.0.9/sidetrek/cli_commands/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,19 @@
-import os
-import importlib
 import json
 import time
 import threading
 from pathlib import Path
 import shutil
 import urllib.parse
 import io
-from typing import Union
 from zipfile import ZipFile
 import typer
 from rich import print
 import requests
-from sidetrek.cli_commands.constants import APP_NAME, GENERATED_LOCAL_SIDETREK_DIRNAME, GENERATED_PROJECT_DIRNAME
-
-
-def get_node_env():
-    if os.environ.get("NODE_ENV") == "development":
-        return "development"
-    elif os.environ.get("NODE_ENV") == "staging":
-        return "staging"
-    else:
-        return "production"
-
-
-def version_callback(value: bool):
-    if value:
-        version = importlib.metadata.version("sidetrek")
-        print(f"Sidetrek CLI version: {version}")
-        raise typer.Exit()
+from cli_commands.constants import NODE_ENV, APP_NAME, GENERATED_LOCAL_SIDETREK_DIRNAME, GENERATED_PROJECT_DIRNAME
 
 
 def print_timer(seconds: int = 1):
     start_time = time.time()
 
     def loop():
         while True:
@@ -41,41 +22,23 @@
             elapsed_time = current_time - start_time
             print(f"\r{elapsed_time} seconds...")
 
     threading.Thread(target=loop).start()
 
 
 def get_auth_api_base_url():
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4002/api/v1"
-    elif node_env == "staging":
-        return f"https://auth-staging.sidetrek.com/api/v1"
-    else:
-        return f"https://auth.sidetrek.com/api/v1"
+    return f"http://localhost:4002/api/v1" if NODE_ENV == "development" else f"https://auth.sidetrek.com/api/v1"
 
 
 def get_user_machine_node_api_base_url(user_id):
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4008/p/api/v1"
-    elif node_env == "staging":
-        return f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
-    else:
-        return f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
+    return f"http://localhost:4008/p/api/v1" if NODE_ENV == "development" else f"https://user-machines.sidetrek.com/{user_id}/node/p/api/v1"
 
 
 def get_webapp_api_base_url():
-    node_env = get_node_env()
-    if node_env == "development":
-        return f"http://localhost:4001/p/app/api/v1"
-    elif node_env == "staging":
-        return f"https://app-staging.sidetrek.com/p/app/api/v1"
-    else:
-        return f"https://app.sidetrek.com/p/app/api/v1"
+    return f"http://localhost:4001/p/app/api/v1" if NODE_ENV == "development" else f"https://app.sidetrek.com/p/app/api/v1"
 
 
 def get_generated_local_sidetrek_dir_path() -> Path:
     app_dir = typer.get_app_dir(APP_NAME)
     generated_local_sidetrek_dir_path = Path(app_dir) / GENERATED_LOCAL_SIDETREK_DIRNAME
     Path(generated_local_sidetrek_dir_path).mkdir(parents=True, exist_ok=True)
     return generated_local_sidetrek_dir_path
@@ -109,15 +72,15 @@
 
 def raise_fail_to_authenticate():
     print("[red]Failed to authenticate.[/red]")
     print("Please login first - run: '[blue]sidetrek login[/blue]'\n")
     raise typer.Exit()
 
 
-def get_credentials() -> Union[dict, None]:
+def get_credentials() -> dict | None:
     """
     Get credentials from the saved file (from login)
 
     If credentials don't exist, raise an except with error message asking to login first
     """
     app_dir = typer.get_app_dir(APP_NAME)
     creds_path: Path = Path(app_dir) / ".credentials"
@@ -155,64 +118,37 @@
 
 
 def get_headers() -> dict:
     token = get_token()
     return {"content-type": "application/json", "authorization": f"Bearer {token}"}
 
 
-def get_auth_user() -> Union[dict, None]:
+def get_current_user() -> dict | None:
     try:
         # Retrieve the currently authenticated user from Cognito by using saved refresh token
         creds_header_str = get_credentials_header_str()
         auth_api_base_url = get_auth_api_base_url()
         auth_user_res = requests.get(f"{auth_api_base_url}/auth/current-user", headers={"Cookie": creds_header_str})
         auth_user_res.raise_for_status()
-        return auth_user_res.json()
-    except requests.exceptions.HTTPError as errh:
-        print(f"{errh.response.status_code} {errh.response.text}")
-        raise typer.Exit()
-    except requests.exceptions.RequestException as err:
-        print("Something went wrong: ", err)
-        raise typer.Exit()
-
-
-def get_current_user() -> Union[dict, None]:
-    try:
-        auth_user = get_auth_user()
+        auth_user = auth_user_res.json()
 
         # Retrieve user from webapp db
         webapp_api_base_url = get_webapp_api_base_url()
         current_user_res = requests.get(f"{webapp_api_base_url}/users", params={"email": auth_user["email"]}, headers=get_headers())
         current_user = current_user_res.json()
         return current_user["data"]
     except requests.exceptions.HTTPError as errh:
         print(f"{errh.response.status_code} {errh.response.text}")
         raise typer.Exit()
     except requests.exceptions.RequestException as err:
         print("Something went wrong: ", err)
         raise typer.Exit()
 
 
-def get_aws_creds() -> Union[dict, None]:
-    try:
-        # Retrieve aws credentials from cognito identity pool
-        creds_header_str = get_credentials_header_str()
-        auth_api_base_url = get_auth_api_base_url()
-        aws_creds = requests.get(f"{auth_api_base_url}/auth/aws-credentials", headers={"Cookie": creds_header_str})
-        aws_creds.raise_for_status()
-        return aws_creds.json()
-    except requests.exceptions.HTTPError as errh:
-        print(f"{errh.response.status_code} {errh.response.text}")
-        raise typer.Exit()
-    except requests.exceptions.RequestException as err:
-        print("Something went wrong: ", err)
-        raise typer.Exit()
-
-
-def get_workflow_draft_version(workflow_id: int) -> Union[dict, None]:
+def get_workflow_draft_version(workflow_id: int) -> dict | None:
     try:
         webapp_api_base_url = get_webapp_api_base_url()
         include = {"organization": True, "project": True, "domain": True, "workflow": True}
         include_json_str = json.dumps(include)
         workflow_version_res = requests.get(f"{webapp_api_base_url}/workflow-versions?isDraft=true&workflowId={workflow_id}&include={include_json_str}", headers=get_headers())
         workflow_version_res.raise_for_status()
         workflow_version = workflow_version_res.json()
```

### Comparing `sidetrek-0.0.87/sidetrek/cli_commands/workflow.py` & `sidetrek-0.0.9/sidetrek/cli_commands/workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import os
 import sys
 import time
 import threading
 from pathlib import Path
 import typer
 import subprocess
 from time import sleep
 from rich import print
 from rich.progress import Progress, SpinnerColumn, TextColumn
-from sidetrek.cli_commands.helpers import (
+from cli_commands.helpers import (
     get_current_user,
-    get_aws_creds,
     get_generated_local_sidetrek_dir_path,
     get_generated_workflow_name,
     download_generated_flyte_workflow,
     get_workflow_draft_version,
     print_timer,
 )
 
@@ -22,73 +20,60 @@
 
 
 @app.command()
 def run(workflow_id: int = typer.Option(...), workflow_args: str = "{}"):
     """
     Execute the workflow locally (e.g. for testing).
 
-    * You can retrieve the --workflow-id (e.g. 42) from Sidetrek app.
-    * Workflow version used it always `draft` for this command
-    * --workflow-args is a stringified JSON of your workflow arguments (e.g. '{"learning_rate"=0.1, "epochs"=5}').
+    You can retrieve the --workflow-id (e.g. 42) from Sidetrek app.
+    --workflow-args is a stringified JSON of your workflow arguments (e.g. '{"learning_rate"=0.1, "epochs"=5}').
     """
-    start_time = time.time()
 
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
     ) as progress:
         print("generated_local_sidetrek_dir_path", get_generated_local_sidetrek_dir_path())
-
+        
         # # Add a timer
         # print_timer()
-
+        
         # Get current user
         auth_step = progress.add_task(description="Authenticating...", total=None)
         current_user = get_current_user()
-        print(f"current_user={current_user}")
         progress.remove_task(auth_step)
-        time_elapsed = round(time.time() - start_time, 2)
-        print(f"[green]✔️ [white]Authenticated [grey89]({time_elapsed}s)")
+        print(f"[green]✔️ [white]Authenticated")
 
         # Always use the draft version for testing
         wf_generation_step = progress.add_task(description="Generating the workflow...", total=None)
         workflow_version = get_workflow_draft_version(workflow_id=workflow_id)
         # print(f"workflow_version={workflow_version}")
 
         # Generate the workflow file
         wf_file_path = download_generated_flyte_workflow(user_id=current_user["id"], workflow_version=workflow_version)
         generated_wf_name = get_generated_workflow_name(workflow_id)
         progress.remove_task(wf_generation_step)
-        time_elapsed = round(time.time() - start_time, 2)
-        print(f"[green]✔️ [white]Workflow generated [grey89]({time_elapsed}s) - {wf_file_path.as_posix()}")
-
-        # Get aws credentials and set it as env var for execution (grants temporary local s3 access)
-        aws_creds = get_aws_creds()
-        print(f"aws_creds={aws_creds}")
-        # aws_env = {**os.environ, "AWS_ACCESS_KEY_ID": aws_creds["AccessKeyId"], "AWS_SECRET_ACCESS_KEY": aws_creds["SecretKey"]}
+        print(f"[green]✔️ [white]Workflow generated")
 
         wf_execution_step = progress.add_task(description="Executing the workflow...", total=None)
-        # print(" ".join(["pyflyte", "run", wf_file_path.as_posix(), generated_wf_name, "--_wf_args", workflow_args]))
         with subprocess.Popen(
+            # ["pyflyte", "--pkgs", "project", "package", "--output", "flyte-workflow-package.tgz", "--image", "gcr.io/sidetrek/tylo-birch1-development/wf-22:0.0.39", "--force"],
             ["pyflyte", "run", wf_file_path, generated_wf_name, "--_wf_args", workflow_args],
             cwd=get_generated_local_sidetrek_dir_path(),
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
-            bufsize=1,
-            universal_newlines=True,
-            # env=aws_env,
         ) as process:
-            for line in process.stdout:
-                print(line, end="")
-
-            _, error = process.communicate()
-
-            if process.returncode != 0:
-                time_elapsed = round(time.time() - start_time, 2)
-                print(f"[light_coral]{error}")
-                print(f"[red]✕ [white]Workflow execution failed [grey89]({time_elapsed}s)")
+            output, error = process.communicate()
+            
+            if process.returncode != 0: 
+                print(f"[light_coral]{error.decode('utf-8')}")
+                print(f"[red]✕ [white]Workflow execution failed")
                 raise typer.Exit()
-
+            
+            print(f"[green]{output.decode('utf-8')}")
+            
             progress.remove_task(wf_execution_step)
-            time_elapsed = round(time.time() - start_time, 2)
-            print(f"[green]✔️ [white]Workflow execution completed 🎉 [grey89]({time_elapsed}s)")
+            print(f"[green]✔️ [white]Workflow execution completed 🎉")
+            # while process.poll() == None:
+            #     print(f"{process.stdout.read1().decode('utf-8')}")
+
```

### Comparing `sidetrek-0.0.87/sidetrek/loggers.py` & `sidetrek-0.0.9/sidetrek/loggers/loggers.py`

 * *Files identical despite different names*


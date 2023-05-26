# Comparing `tmp/seqslab-cli-3.2.0.post2.tar.gz` & `tmp/seqslab-cli-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.2.0.post2.tar", last modified: Fri May 26 06:02:23 2023, max compression
+gzip compressed data, was "seqslab-cli-3.2.1.tar", last modified: Fri May 26 06:05:38 2023, max compression
```

## Comparing `seqslab-cli-3.2.0.post2.tar` & `seqslab-cli-3.2.1.tar`

### file list

```diff
@@ -1,27 +1,128 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:02:23.030473 seqslab-cli-3.2.0.post2/
--rw-r--r--   0 chris      (501) staff       (20)      692 2022-04-15 03:12:06.000000 seqslab-cli-3.2.0.post2/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       77 2022-04-15 03:12:06.000000 seqslab-cli-3.2.0.post2/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     8768 2023-05-26 06:02:23.030724 seqslab-cli-3.2.0.post2/PKG-INFO
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:02:23.018608 seqslab-cli-3.2.0.post2/python/
--rw-r--r--   0 chris      (501) staff       (20)      418 2023-02-24 03:14:45.000000 seqslab-cli-3.2.0.post2/python/requirements.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:02:23.025504 seqslab-cli-3.2.0.post2/python/seqslab/
--rw-r--r--   0 chris      (501) staff       (20)     8042 2023-05-26 05:55:52.000000 seqslab-cli-3.2.0.post2/python/seqslab/README.md
--rw-r--r--   0 chris      (501) staff       (20)      791 2023-05-26 06:02:07.000000 seqslab-cli-3.2.0.post2/python/seqslab/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1228 2023-02-08 06:39:25.000000 seqslab-cli-3.2.0.post2/python/seqslab/cli.py
--rw-r--r--   0 chris      (501) staff       (20)      728 2021-07-06 09:40:18.000000 seqslab-cli-3.2.0.post2/python/seqslab/context.py
--rw-r--r--   0 chris      (501) staff       (20)     2285 2022-07-27 01:18:54.000000 seqslab-cli-3.2.0.post2/python/seqslab/exceptions.py
--rw-r--r--   0 chris      (501) staff       (20)     5440 2023-02-24 03:14:45.000000 seqslab-cli-3.2.0.post2/python/seqslab/plugin.py
--rw-r--r--   0 chris      (501) staff       (20)      452 2021-07-06 09:40:18.000000 seqslab-cli-3.2.0.post2/python/seqslab/session_logger.py
--rw-r--r--   0 chris      (501) staff       (20)      824 2022-07-27 01:18:54.000000 seqslab-cli-3.2.0.post2/python/seqslab/settings.py
--rw-r--r--   0 chris      (501) staff       (20)     1370 2021-07-06 09:40:18.000000 seqslab-cli-3.2.0.post2/python/seqslab/statusbar.py
--rw-r--r--   0 chris      (501) staff       (20)      951 2021-07-06 09:40:18.000000 seqslab-cli-3.2.0.post2/python/seqslab/usage_logger.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:02:23.029623 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     8768 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      626 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)      429 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-26 06:02:23.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 05:38:21.000000 seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 chris      (501) staff       (20)      373 2023-05-26 06:02:23.032472 seqslab-cli-3.2.0.post2/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     2182 2023-05-26 05:38:12.000000 seqslab-cli-3.2.0.post2/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.982665 seqslab-cli-3.2.1/
+-rw-r--r--   0 chris      (501) staff       (20)      692 2022-04-15 03:12:06.000000 seqslab-cli-3.2.1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       77 2022-04-15 03:12:06.000000 seqslab-cli-3.2.1/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     8762 2023-05-26 06:05:38.983048 seqslab-cli-3.2.1/PKG-INFO
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.912254 seqslab-cli-3.2.1/python/
+-rw-r--r--   0 chris      (501) staff       (20)      418 2023-02-24 03:14:45.000000 seqslab-cli-3.2.1/python/requirements.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.920783 seqslab-cli-3.2.1/python/seqslab/
+-rw-r--r--   0 chris      (501) staff       (20)     8042 2023-05-26 05:55:52.000000 seqslab-cli-3.2.1/python/seqslab/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      786 2023-05-26 06:05:00.000000 seqslab-cli-3.2.1/python/seqslab/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.922980 seqslab-cli-3.2.1/python/seqslab/auth/
+-rw-r--r--   0 chris      (501) staff       (20)       79 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4514 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/azuread.py
+-rw-r--r--   0 chris      (501) staff       (20)    14275 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/auth/commands.py
+-rw-r--r--   0 chris      (501) staff       (20)     1228 2023-02-08 06:39:25.000000 seqslab-cli-3.2.1/python/seqslab/cli.py
+-rw-r--r--   0 chris      (501) staff       (20)      728 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/context.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.924236 seqslab-cli-3.2.1/python/seqslab/drs/
+-rw-r--r--   0 chris      (501) staff       (20)      228 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.927496 seqslab-cli-3.2.1/python/seqslab/drs/api/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    14655 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)    14735 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     1336 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/common.py
+-rw-r--r--   0 chris      (501) staff       (20)     5116 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/api/template.py
+-rw-r--r--   0 chris      (501) staff       (20)    37707 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.930097 seqslab-cli-3.2.1/python/seqslab/drs/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    20561 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 chris      (501) staff       (20)     1325 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 chris      (501) staff       (20)     4012 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.931817 seqslab-cli-3.2.1/python/seqslab/drs/storage/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    40704 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)    12838 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.933606 seqslab-cli-3.2.1/python/seqslab/drs/utils/
+-rw-r--r--   0 chris      (501) staff       (20)       81 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2075 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 chris      (501) staff       (20)     3180 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 chris      (501) staff       (20)     2285 2022-07-27 01:18:54.000000 seqslab-cli-3.2.1/python/seqslab/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.934960 seqslab-cli-3.2.1/python/seqslab/organization/
+-rw-r--r--   0 chris      (501) staff       (20)      271 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2365 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.936077 seqslab-cli-3.2.1/python/seqslab/organization/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     5440 2023-02-24 03:14:45.000000 seqslab-cli-3.2.1/python/seqslab/plugin.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.937241 seqslab-cli-3.2.1/python/seqslab/role/
+-rw-r--r--   0 chris      (501) staff       (20)      230 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1275 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.938284 seqslab-cli-3.2.1/python/seqslab/role/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1324 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.939974 seqslab-cli-3.2.1/python/seqslab/role/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      865 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)     1286 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.941161 seqslab-cli-3.2.1/python/seqslab/runsheet/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3442 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 chris      (501) staff       (20)      452 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/session_logger.py
+-rw-r--r--   0 chris      (501) staff       (20)      824 2022-07-27 01:18:54.000000 seqslab-cli-3.2.1/python/seqslab/settings.py
+-rw-r--r--   0 chris      (501) staff       (20)     1370 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/statusbar.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.942757 seqslab-cli-3.2.1/python/seqslab/trs/
+-rw-r--r--   0 chris      (501) staff       (20)      227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    20866 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.944484 seqslab-cli-3.2.1/python/seqslab/trs/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1667 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.947924 seqslab-cli-3.2.1/python/seqslab/trs/register/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      940 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)     9941 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     1321 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/common.py
+-rw-r--r--   0 chris      (501) staff       (20)     7345 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.950370 seqslab-cli-3.2.1/python/seqslab/trs/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      883 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)     7267 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     1346 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.952213 seqslab-cli-3.2.1/python/seqslab/trs/template/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7386 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     2897 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/trs/template/template.py
+-rw-r--r--   0 chris      (501) staff       (20)      951 2021-07-06 09:40:18.000000 seqslab-cli-3.2.1/python/seqslab/usage_logger.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.953539 seqslab-cli-3.2.1/python/seqslab/user/
+-rw-r--r--   0 chris      (501) staff       (20)      230 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     6820 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.954461 seqslab-cli-3.2.1/python/seqslab/user/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1327 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.961236 seqslab-cli-3.2.1/python/seqslab/user/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1743 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)     4001 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.965525 seqslab-cli-3.2.1/python/seqslab/wes/
+-rw-r--r--   0 chris      (501) staff       (20)      227 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    23184 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.967039 seqslab-cli-3.2.1/python/seqslab/wes/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1345 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.970187 seqslab-cli-3.2.1/python/seqslab/wes/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      883 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)    11664 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.972233 seqslab-cli-3.2.1/python/seqslab/wes/template/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3467 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     3234 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/template/template.py
+-rw-r--r--   0 chris      (501) staff       (20)     3269 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/wes/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.974208 seqslab-cli-3.2.1/python/seqslab/workspace/
+-rw-r--r--   0 chris      (501) staff       (20)      235 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7064 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.975239 seqslab-cli-3.2.1/python/seqslab/workspace/internal/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1336 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.977268 seqslab-cli-3.2.1/python/seqslab/workspace/resource/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      863 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 chris      (501) staff       (20)     4033 2023-05-26 06:04:46.000000 seqslab-cli-3.2.1/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-26 06:05:38.981816 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     8762 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     3385 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       45 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)      429 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)        8 2023-05-26 06:05:38.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-26 05:38:21.000000 seqslab-cli-3.2.1/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 chris      (501) staff       (20)      373 2023-05-26 06:05:38.984138 seqslab-cli-3.2.1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     2182 2023-05-26 05:38:12.000000 seqslab-cli-3.2.1/setup.py
```

### Comparing `seqslab-cli-3.2.0.post2/LICENSE` & `seqslab-cli-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/PKG-INFO` & `seqslab-cli-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.2.0.post2
+Version: 3.2.1
 Summary: Atgenomix SeqsLab CLI for Python
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/AnomeGAP/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.0.post2 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.1 Summary: Atgenomix
 SeqsLab CLI for Python Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin Author-email: jiayou.lin@atgenomix.com License: MIT license
 Project-URL: Documentation, https://docs.atgenomix.com/ Project-URL:
 Repository, https://github.com/AnomeGAP/seqslab-cli Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/README.md` & `seqslab-cli-3.2.1/python/seqslab/README.md`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/__init__.py` & `seqslab-cli-3.2.1/python/seqslab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.0post2"
+__version__ = "3.2.1"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/cli.py` & `seqslab-cli-3.2.1/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/context.py` & `seqslab-cli-3.2.1/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/exceptions.py` & `seqslab-cli-3.2.1/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/plugin.py` & `seqslab-cli-3.2.1/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/settings.py` & `seqslab-cli-3.2.1/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/statusbar.py` & `seqslab-cli-3.2.1/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab/usage_logger.py` & `seqslab-cli-3.2.1/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.2.0.post2/python/seqslab_cli.egg-info/PKG-INFO` & `seqslab-cli-3.2.1/python/seqslab_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.2.0.post2
+Version: 3.2.1
 Summary: Atgenomix SeqsLab CLI for Python
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/AnomeGAP/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.0.post2 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.2.1 Summary: Atgenomix
 SeqsLab CLI for Python Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin Author-email: jiayou.lin@atgenomix.com License: MIT license
 Project-URL: Documentation, https://docs.atgenomix.com/ Project-URL:
 Repository, https://github.com/AnomeGAP/seqslab-cli Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `seqslab-cli-3.2.0.post2/setup.py` & `seqslab-cli-3.2.1/setup.py`

 * *Files identical despite different names*


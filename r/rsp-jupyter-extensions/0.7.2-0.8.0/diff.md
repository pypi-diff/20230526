# Comparing `tmp/rsp_jupyter_extensions-0.7.2.tar.gz` & `tmp/rsp_jupyter_extensions-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsp_jupyter_extensions-0.7.2.tar", last modified: Wed Jan 25 01:12:33 2023, max compression
+gzip compressed data, was "rsp_jupyter_extensions-0.8.0.tar", last modified: Fri May 26 19:20:13 2023, max compression
```

## Comparing `rsp_jupyter_extensions-0.7.2.tar` & `rsp_jupyter_extensions-0.8.0.tar`

### file list

```diff
@@ -1,59 +1,57 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.249488 rsp_jupyter_extensions-0.7.2/
--rw-r--r--   0 adam       (501) staff       (20)     1068 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      480 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-01-25 01:12:33.249347 rsp_jupyter_extensions-0.7.2/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3072 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/README.md
--rw-r--r--   0 adam       (501) staff       (20)     1146 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/RELEASE.md
--rw-r--r--   0 adam       (501) staff       (20)      205 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/install.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.241062 rsp_jupyter_extensions-0.7.2/jupyter-config/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.243142 rsp_jupyter_extensions-0.7.2/jupyter-config/nb-config/
--rw-r--r--   0 adam       (501) staff       (20)       99 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/jupyter-config/nb-config/rsp_jupyter_extensions.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.243302 rsp_jupyter_extensions-0.7.2/jupyter-config/server-config/
--rw-r--r--   0 adam       (501) staff       (20)       97 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/jupyter-config/server-config/rsp_jupyter_extensions.json
--rw-r--r--   0 adam       (501) staff       (20)     3090 2023-01-25 01:12:11.000000 rsp_jupyter_extensions-0.7.2/package.json
--rw-r--r--   0 adam       (501) staff       (20)      948 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.244411 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/
--rw-r--r--   0 adam       (501) staff       (20)      699 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     2218 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/environment.py
--rw-r--r--   0 adam       (501) staff       (20)     2311 2023-01-24 16:33:37.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/execution.py
--rw-r--r--   0 adam       (501) staff       (20)      916 2023-01-24 16:33:37.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/handlers.py
--rw-r--r--   0 adam       (501) staff       (20)     1573 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/hub.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.245710 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/
--rw-r--r--   0 adam       (501) staff       (20)    20795 2023-01-24 21:09:29.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/build_log.json
--rw-r--r--   0 adam       (501) staff       (20)     3207 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/package.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.247527 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/
--rw-r--r--   0 adam       (501) staff       (20)    28763 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js
--rw-r--r--   0 adam       (501) staff       (20)    20846 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js.map
--rw-r--r--   0 adam       (501) staff       (20)    29309 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js
--rw-r--r--   0 adam       (501) staff       (20)    28195 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js.map
--rw-r--r--   0 adam       (501) staff       (20)      165 2023-01-24 21:09:29.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/style.js
--rw-r--r--   0 adam       (501) staff       (20)     4268 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js
--rw-r--r--   0 adam       (501) staff       (20)     1438 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js.map
--rw-r--r--   0 adam       (501) staff       (20)    12074 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js
--rw-r--r--   0 adam       (501) staff       (20)    13814 2023-01-24 21:09:30.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js.map
--rw-r--r--   0 adam       (501) staff       (20)     3298 2023-01-24 16:33:37.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/query.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.247676 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/templates/
--rw-r--r--   0 adam       (501) staff       (20)     2735 2023-01-24 16:33:37.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/templates/portal_query.ipynb.template
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.245247 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-01-25 01:12:33.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1909 2023-01-25 01:12:33.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-01-25 01:12:33.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-01-24 17:30:14.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       41 2023-01-25 01:12:33.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       29 2023-01-25 01:12:33.000000 rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-01-25 01:12:33.249521 rsp_jupyter_extensions-0.7.2/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     3120 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.248648 rsp_jupyter_extensions-0.7.2/src/
--rw-r--r--   0 adam       (501) staff       (20)     1577 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/DisplayLabVersion.tsx
--rw-r--r--   0 adam       (501) staff       (20)     3708 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/displayversion.ts
--rw-r--r--   0 adam       (501) staff       (20)     1420 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/index.ts
--rw-r--r--   0 adam       (501) staff       (20)     5503 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/query.ts
--rw-r--r--   0 adam       (501) staff       (20)     4737 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/savequit.ts
--rw-r--r--   0 adam       (501) staff       (20)      304 2023-01-24 23:37:47.000000 rsp_jupyter_extensions-0.7.2/src/tokens.ts
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.249034 rsp_jupyter_extensions-0.7.2/style/
--rw-r--r--   0 adam       (501) staff       (20)        0 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/style/base.css
--rw-r--r--   0 adam       (501) staff       (20)       25 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/style/index.css
--rw-r--r--   0 adam       (501) staff       (20)       21 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/style/index.js
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-01-25 01:12:33.249177 rsp_jupyter_extensions-0.7.2/tests/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-01-24 20:02:34.000000 rsp_jupyter_extensions-0.7.2/tests/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)      554 2022-09-04 05:10:15.000000 rsp_jupyter_extensions-0.7.2/tsconfig.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.863293 rsp_jupyter_extensions-0.8.0/
+-rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 19:20:13.862969 rsp_jupyter_extensions-0.8.0/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/RELEASE.md
+-rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/install.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.841004 rsp_jupyter_extensions-0.8.0/jupyter-config/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.845935 rsp_jupyter_extensions-0.8.0/jupyter-config/nb-config/
+-rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/jupyter-config/nb-config/rsp_jupyter_extensions.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.846303 rsp_jupyter_extensions-0.8.0/jupyter-config/server-config/
+-rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/jupyter-config/server-config/rsp_jupyter_extensions.json
+-rw-r--r--   0 adam       (501) staff       (20)     3069 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/package.json
+-rw-r--r--   0 adam       (501) staff       (20)      954 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.849697 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/
+-rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/environment.py
+-rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/execution.py
+-rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/handlers.py
+-rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/hub.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.853092 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/
+-rw-r--r--   0 adam       (501) staff       (20)    20795 2022-09-02 20:40:09.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/build_log.json
+-rw-r--r--   0 adam       (501) staff       (20)     3207 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/package.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.858006 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/
+-rw-r--r--   0 adam       (501) staff       (20)    27460 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js
+-rw-r--r--   0 adam       (501) staff       (20)    19521 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js.map
+-rw-r--r--   0 adam       (501) staff       (20)    28481 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js
+-rw-r--r--   0 adam       (501) staff       (20)    27434 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js.map
+-rw-r--r--   0 adam       (501) staff       (20)      165 2022-09-02 20:40:09.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style.js
+-rw-r--r--   0 adam       (501) staff       (20)     4268 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js
+-rw-r--r--   0 adam       (501) staff       (20)     1438 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js.map
+-rw-r--r--   0 adam       (501) staff       (20)    12074 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js
+-rw-r--r--   0 adam       (501) staff       (20)    13814 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js.map
+-rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/query.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.858470 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/
+-rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/portal_query.ipynb.template
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.852116 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1891 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 19:20:13.863364 rsp_jupyter_extensions-0.8.0/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.861408 rsp_jupyter_extensions-0.8.0/src/
+-rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/DisplayLabVersion.tsx
+-rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/src/displayversion.ts
+-rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/index.ts
+-rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/query.ts
+-rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/savequit.ts
+-rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/tokens.ts
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.862545 rsp_jupyter_extensions-0.8.0/style/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/base.css
+-rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/index.css
+-rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/index.js
+-rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/tsconfig.json
```

### Comparing `rsp_jupyter_extensions-0.7.2/LICENSE` & `rsp_jupyter_extensions-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/PKG-INFO` & `rsp_jupyter_extensions-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp_jupyter_extensions
-Version: 0.7.2
+Version: 0.8.0
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.7.2/README.md` & `rsp_jupyter_extensions-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/RELEASE.md` & `rsp_jupyter_extensions-0.8.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/package.json` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9714285714285713%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.cbd475d0b140d652d3db.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.6.0'"}*

```diff
@@ -45,14 +45,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.cbd475d0b140d652d3db.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "@jupyterlab/statusbar-extension:mode-switch"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "rsp_jupyter_extensions"
@@ -97,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.2"
+    "version": "0.6.0"
 }
```

### Comparing `rsp_jupyter_extensions-0.7.2/pyproject.toml` & `rsp_jupyter_extensions-0.8.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [build-system]
-requires = ["jupyter_packaging~=0.10,<2",
-	 "jupyterlab~=3.1",
+requires = ["jupyter_packaging",
+	 "jupyterlab~=3.6.3",
 	 "isort",
+	 "poetry",
 	 "black",
 	 "pre-commit"
 ]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["rsp_jupyter_extensions/labextension/static/style.js"]
@@ -19,15 +20,15 @@
 npm = ["jlpm"]
 
 [tool.check-manifest]
 ignore = ["rsp_jupyter_extensions/labextension/**", "yarn.lock", ".*", "package-lock.json"]
 
 [tool.black]
 line-length = 79
-target-version = ['py38']
+target-version = ['py310']
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.mypy_cache
   | \.tox
   | \.venv
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/__init__.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/environment.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/environment.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/execution.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/execution.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/handlers.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/handlers.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/hub.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/hub.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/build_log.json` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/build_log.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999137205387206%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^3.4.5'}, '@jupyterlab/application-extension': {'requiredVersion': '^3.4.5'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.4.5'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.4.5'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.4.5'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^3.4.5'}, "*

 * *      "'@jupyterlab/compl […]*

```diff
@@ -112,418 +112,418 @@
                         ],
                         "type": "var"
                     },
                     "name": "rsp-jupyter-extensions",
                     "shared": {
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.5.3",
+                            "requiredVersion": "^5.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.5.3"
+                            "requiredVersion": "^4.4.5"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.5.3",
+                            "requiredVersion": "^6.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.5.3",
+                            "requiredVersion": "^5.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.5.3"
+                            "requiredVersion": "^5.4.5"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.5.3",
+                            "requiredVersion": "^3.4.5",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.5.3"
+                            "requiredVersion": "^3.4.5"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
@@ -591,15 +591,15 @@
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "rsp-jupyter-extensions": {
                             "import": "/Users/adam/git/rsp-jupyter-extensions/lib/index.js",
                             "singleton": true,
-                            "version": "0.7.0"
+                            "version": "0.6.0"
                         },
                         "yjs": {
                             "import": false,
                             "requiredVersion": "^13.5.17",
                             "singleton": true
                         }
                     }
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/package.json` & `rsp_jupyter_extensions-0.8.0/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638888888888889%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3', '@jupyterlab/coreutils': '^5', "*

 * *                   "'@jupyterlab/services': '^6'}",*

 * * "'jupyter-releaser'": "{'hooks': {'before-build-npm': {insert: [(0, 'python -m pip install "*

 * *                       "jupyterlab~=3.3')], delete: [0]}}}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.8.0'"}*

```diff
@@ -6,20 +6,20 @@
     "browser": {
         "URL": "window.URL"
     },
     "bugs": {
         "url": "https://github.com/lsst-sqre/rsp-jupyter-extensions/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.1.0",
+        "@jupyterlab/application": "^3",
         "@jupyterlab/apputils": "^3",
-        "@jupyterlab/coreutils": "^5.1.0",
+        "@jupyterlab/coreutils": "^5",
         "@jupyterlab/docmanager": "^3",
         "@jupyterlab/mainmenu": "^3",
-        "@jupyterlab/services": "^6.1.0",
+        "@jupyterlab/services": "^6",
         "@jupyterlab/statusbar": "^3",
         "@lumino/algorithm": "^1",
         "@lumino/widgets": "^1",
         "@types/core-js": "^2"
     },
     "description": "Jupyter Extensions for the RSP",
     "devDependencies": {
@@ -39,25 +39,20 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/lsst-sqre/rsp-jupyter-extensions",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
+                "python -m pip install jupyterlab~=3.3",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.6537682ba05daa64613a.js",
-            "style": "./style"
-        },
         "disabledExtensions": [
             "@jupyterlab/statusbar-extension:mode-switch"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "rsp_jupyter_extensions"
@@ -102,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.7.0"
+    "version": "0.8.0"
 }
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -38,18 +38,18 @@
                  * A pure function for rendering the displayversion information.
                  *
                  * @param props: the props for rendering the component.
                  *
                  * @returns a tsx component for displaying version information.
                  */
                 function DisplayLabVersionComponent(props) {
-                    return react__WEBPACK_IMPORTED_MODULE_0__.createElement(_jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_2__.TextItem, {
-                        source: `${props.source}`,
-                        title: `${props.title}`
-                    });
+                    return (react__WEBPACK_IMPORTED_MODULE_0__.createElement(_jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_2__.TextItem, {
+                        source: `${(props.source)}`,
+                        title: `${(props.title)}`
+                    }));
                 }
                 class DisplayLabVersion extends _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.VDomRenderer {
                     /**
                      * Create a new DisplayLabVersion widget.
                      */
                     constructor(props) {
                         super(new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.VDomModel());
@@ -69,15 +69,15 @@
                     }
                     /**
                      * Dispose of the item.
                      */
                     dispose() {
                         super.dispose();
                     }
-                }
+                };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (DisplayLabVersion);
 
 
                 /***/
             }),
 
@@ -122,55 +122,43 @@
 
 
                 /**
                  * Activate the extension.
                  */
                 function activateRSPDisplayVersionExtension(app, statusBar) {
                     console.log('RSP DisplayVersion extension: loading...');
-                    const svcManager = app.serviceManager;
-                    const endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__.PageConfig.getBaseUrl() + 'rubin/environment';
-                    const init = {
-                        method: 'GET'
+                    let svcManager = app.serviceManager;
+                    let endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__.PageConfig.getBaseUrl() + "rubin/environment";
+                    let init = {
+                        method: "GET"
                     };
-                    const settings = svcManager.serverSettings;
-                    apiRequest(endpoint, init, settings).then(res => {
-                        const image_description = res.IMAGE_DESCRIPTION || '';
-                        const image_digest = res.IMAGE_DIGEST;
-                        const image_spec = res.JUPYTER_IMAGE_SPEC;
-                        const instance_url = new URL(res.EXTERNAL_INSTANCE_URL || '');
-                        const hostname = ' ' + instance_url.hostname;
-                        let digest_str = '';
-                        let imagename = '';
+                    let settings = svcManager.serverSettings;
+                    apiRequest(endpoint, init, settings).then((res) => {
+                        let image_description = (res.IMAGE_DESCRIPTION || "");
+                        let image_digest = res.IMAGE_DIGEST;
+                        let image_spec = res.JUPYTER_IMAGE_SPEC;
+                        let instance_url = new URL(res.EXTERNAL_INSTANCE_URL || "");
+                        let hostname = " " + instance_url.hostname;
+                        let digest_str = "";
+                        if (image_digest) {
+                            digest_str = " [" + image_digest.substring(0, 8) + "...]";
+                        }
+                        let imagename = "";
                         if (image_spec) {
-                            /* First try to get digest out of image spec (nublado v3) */
-                            const imagearr = image_spec.split('/');
-                            const pullname = imagearr[imagearr.length - 1];
-                            const partsarr = pullname.split('@');
-                            if (partsarr.length === 2) {
-                                /* Split name and sha; "sha256:" is seven characters */
-                                digest_str = ' [' + partsarr[1].substring(7, 7 + 8) + '...]';
-                                imagename = ' (' + partsarr[0] + ')';
-                            } else {
-                                /* Nothing to split; image name is the name we pulled by */
-                                imagename = ' (' + pullname + ')';
-                            }
-                            if (digest_str === '' && image_digest) {
-                                /* No digest in spec?  Well, did we set IMAGE_DIGEST?
-                                   Yes, if we are nubladov2. */
-                                digest_str = ' [' + image_digest.substring(0, 8) + '...]';
-                            }
+                            let imagearr = image_spec.split("/");
+                            imagename = " (" + imagearr[imagearr.length - 1] + ")";
                         }
-                        const label = image_description + digest_str + imagename + hostname;
+                        let label = image_description + digest_str + imagename + hostname;
                         const displayVersionWidget = new _DisplayLabVersion__WEBPACK_IMPORTED_MODULE_3__["default"]({
                             source: label,
                             title: image_description
                         });
                         statusBar.registerStatusItem(_tokens__WEBPACK_IMPORTED_MODULE_4__.DISPLAYVERSION_ID, {
                             item: displayVersionWidget,
-                            align: 'left',
+                            align: "left",
                             rank: 80,
                             isActive: () => true
                         });
                     });
 
                     function apiRequest(url, init, settings) {
                         /**
@@ -191,23 +179,25 @@
                                     throw new _jupyterlab_services__WEBPACK_IMPORTED_MODULE_1__.ServerConnection.ResponseError(response, data.message);
                                 });
                             }
                             return response.json();
                         });
                     }
                     console.log('RSP DisplayVersion extension: ... loaded');
-                }
+                };
                 /**
                  * Initialization data for the RSPdisplayversionextension extension.
                  */
                 const rspDisplayVersionExtension = {
                     activate: activateRSPDisplayVersionExtension,
                     id: _tokens__WEBPACK_IMPORTED_MODULE_4__.DISPLAYVERSION_ID,
-                    requires: [_jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_2__.IStatusBar],
-                    autoStart: false
+                    requires: [
+                        _jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_2__.IStatusBar,
+                    ],
+                    autoStart: false,
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (rspDisplayVersionExtension);
 
 
                 /***/
             }),
@@ -269,16 +259,20 @@
                 }
                 /**
                  * Initialization data for the rspExtensions.
                  */
                 const rspExtension = {
                     activate: activateRSPExtension,
                     id: _tokens__WEBPACK_IMPORTED_MODULE_6__.PLUGIN_ID,
-                    requires: [_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_1__.IMainMenu, _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_2__.IDocumentManager, _jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_0__.IStatusBar],
-                    autoStart: true
+                    requires: [
+                        _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_1__.IMainMenu,
+                        _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_2__.IDocumentManager,
+                        _jupyterlab_statusbar__WEBPACK_IMPORTED_MODULE_0__.IStatusBar
+                    ],
+                    autoStart: true,
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (rspExtension);
 
 
                 /***/
             }),
@@ -340,39 +334,39 @@
 
                 /**
                  * The command IDs used by the plugin.
                  */
                 var CommandIDs;
                 (function(CommandIDs) {
                     CommandIDs.rubinquery = 'rubinquery';
-                })(CommandIDs || (CommandIDs = {}));
+                })(CommandIDs || (CommandIDs = {}));;
                 /**
                  * Activate the extension.
                  */
                 function activateRSPQueryExtension(app, mainMenu, docManager) {
                     console.log('rsp-query...loading');
-                    const svcManager = app.serviceManager;
+                    let svcManager = app.serviceManager;
                     const {
                         commands
                     } = app;
                     commands.addCommand(CommandIDs.rubinquery, {
                         label: 'Open from portal query URL...',
                         caption: 'Open notebook from supplied portal query URL',
                         execute: () => {
                             rubinportalquery(app, docManager, svcManager);
                         }
                     });
                     // Add commands and menu itmes.
-                    const menu = {
+                    let menu = {
                         command: CommandIDs.rubinquery
                     };
-                    const rubinmenu = new _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.Menu({
-                        commands
+                    let rubinmenu = new _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.Menu({
+                        commands,
                     });
-                    rubinmenu.title.label = 'Rubin';
+                    rubinmenu.title.label = "Rubin";
                     rubinmenu.insertItem(0, menu);
                     mainMenu.addMenu(rubinmenu);
                     console.log('rsp-query...loaded');
                 }
                 class QueryHandler extends _lumino_widgets__WEBPACK_IMPORTED_MODULE_0__.Widget {
                     constructor() {
                         super({
@@ -385,44 +379,38 @@
                     }
                     getValue() {
                         return this.inputNode.value;
                     }
                 }
 
                 function queryDialog(manager) {
-                    const options = {
+                    let options = {
                         title: 'Query Value',
                         body: new QueryHandler(),
                         focusNodeSelector: 'input',
                         buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.Dialog.cancelButton(), _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.Dialog.okButton({
                             label: 'CREATE'
                         })]
                     };
                     return (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showDialog)(options).then(result => {
                         if (!result) {
-                            console.log('No result from queryDialog');
-                            return new Promise((res, rej) => {
-                                /* Nothing */
-                            });
+                            console.log("No result from queryDialog");
+                            return new Promise((res, rej) => {});
                         }
-                        console.log('Result from queryDialog: ', result);
+                        console.log("Result from queryDialog: ", result);
                         if (!result.value) {
-                            console.log('No result.value from queryDialog');
-                            return new Promise((res, rej) => {
-                                /* Nothing */
-                            });
+                            console.log("No result.value from queryDialog");
+                            return new Promise((res, rej) => {});
                         }
                         if (result.button.label === 'CREATE') {
-                            console.log('Got result ', result.value, ' from queryDialog: CREATE');
+                            console.log("Got result ", result.value, " from queryDialog: CREATE");
                             return Promise.resolve(result.value);
                         }
-                        console.log('Did not get queryDialog: CREATE');
-                        return new Promise((res, rej) => {
-                            /* Nothing */
-                        });
+                        console.log("Did not get queryDialog: CREATE");
+                        return new Promise((res, rej) => {});
                     });
                 }
 
                 function apiRequest(url, init, settings) {
                     /**
                      * Make a request to our endpoint to get a pointer to a templated
                      *  notebook for a given query
@@ -432,15 +420,15 @@
                      * @param init - The POST + body for the extension
                      *
                      * @param settings - the settings for the current notebook server.
                      *
                      * @returns a Promise resolved with the JSON response
                      */
                     // Fake out URL check in makeRequest
-                    const newSettings = _jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.ServerConnection.makeSettings({
+                    let newSettings = _jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.ServerConnection.makeSettings({
                         baseUrl: settings.baseUrl,
                         appUrl: settings.appUrl,
                         wsUrl: settings.wsUrl,
                         init: settings.init,
                         token: settings.token,
                         Request: settings.Request,
                         Headers: settings.Headers,
@@ -454,61 +442,60 @@
                         }
                         return response.json();
                     });
                 }
 
                 function rubinportalquery(app, docManager, svcManager) {
                     queryDialog(docManager).then(url => {
-                        console.log('Query URL is', url);
+                        console.log("Query URL is", url);
                         if (!url) {
-                            console.log('Query URL was null');
-                            return new Promise((res, rej) => {
-                                /* Nothing */
-                            });
+                            console.log("Query URL was null");
+                            return new Promise((res, rej) => {});
                         }
-                        const body = JSON.stringify({
-                            type: 'portal',
-                            value: url
+                        let body = JSON.stringify({
+                            "type": "portal",
+                            "value": url
                         });
-                        const endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_5__.PageConfig.getBaseUrl() + 'rubin/query';
-                        const init = {
-                            method: 'POST',
+                        let endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_5__.PageConfig.getBaseUrl() + "rubin/query";
+                        let init = {
+                            method: "POST",
                             body: body
                         };
-                        const settings = svcManager.serverSettings;
-                        apiRequest(endpoint, init, settings).then(res => {
-                            const path = res.path;
+                        let settings = svcManager.serverSettings;
+                        apiRequest(endpoint, init, settings).then(function(res) {
+                            let path = res.path;
                             docManager.open(path);
                         });
-                        return new Promise((res, rej) => {
-                            /* Nothing */
-                        });
+                        return new Promise((res, rej) => {});
                     });
                 }
                 /**
                  * Initialization data for the jupyterlab-lsstquery extension.
                  */
                 const rspQueryExtension = {
                     activate: activateRSPQueryExtension,
                     id: _tokens__WEBPACK_IMPORTED_MODULE_6__.QUERY_ID,
-                    requires: [_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_2__.IMainMenu, _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_3__.IDocumentManager],
-                    autoStart: false
+                    requires: [
+                        _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_2__.IMainMenu,
+                        _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_3__.IDocumentManager
+                    ],
+                    autoStart: false,
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (rspQueryExtension);
                 var Private;
                 (function(Private) {
                     /**
                      * Create node for query handler.
                      */
                     function createQueryNode() {
-                        const body = document.createElement('div');
-                        const qidLabel = document.createElement('label');
+                        let body = document.createElement('div');
+                        let qidLabel = document.createElement('label');
                         qidLabel.textContent = 'Enter Query Value';
-                        const name = document.createElement('input');
+                        let name = document.createElement('input');
                         body.appendChild(qidLabel);
                         body.appendChild(name);
                         return body;
                     }
                     Private.createQueryNode = createQueryNode;
                 })(Private || (Private = {}));
 
@@ -571,147 +558,137 @@
 
 
                 /**
                  * The command IDs used by the plugin.
                  */
                 var CommandIDs;
                 (function(CommandIDs) {
-                    CommandIDs.justQuit = 'justquit:justquit';
                     CommandIDs.saveQuit = 'savequit:savequit';
-                    CommandIDs.saveLogout = 'savelogout:savelogout';
-                })(CommandIDs || (CommandIDs = {}));
+                    CommandIDs.justQuit = 'justquit:justquit';
+                })(CommandIDs || (CommandIDs = {}));;
                 /**
                  * Activate the jupyterhub extension.
                  */
                 function activateRSPSavequitExtension(app, mainMenu, docManager) {
                     console.log('rsp-savequit: loading...');
-                    const svcManager = app.serviceManager;
+                    let svcManager = app.serviceManager;
                     const {
                         commands
                     } = app;
-                    commands.addCommand(CommandIDs.justQuit, {
-                        label: 'Exit Without Saving',
-                        caption: 'Destroy container',
-                        execute: () => {
-                            justQuit(app, docManager, svcManager, false);
-                        }
-                    });
                     commands.addCommand(CommandIDs.saveQuit, {
                         label: 'Save All and Exit',
                         caption: 'Save open notebooks and destroy container',
                         execute: () => {
-                            saveAndQuit(app, docManager, svcManager, false);
+                            saveAndQuit(app, docManager, svcManager);
                         }
                     });
-                    commands.addCommand(CommandIDs.saveLogout, {
-                        label: 'Save All, Exit, and Log Out',
-                        caption: 'Save open notebooks, destroy container, and log out',
+                    commands.addCommand(CommandIDs.justQuit, {
+                        label: 'Exit Without Saving',
+                        caption: 'Destroy container',
                         execute: () => {
-                            saveAndQuit(app, docManager, svcManager, true);
+                            justQuit(app, docManager, svcManager);
                         }
                     });
                     // Add commands and menu itmes.
-                    const menu = [{
-                        command: CommandIDs.justQuit
-                    }, {
+                    let menu = [{
                         command: CommandIDs.saveQuit
                     }, {
-                        command: CommandIDs.saveLogout
-                    }];
+                        command: CommandIDs.justQuit
+                    }, ];
                     // Put it at the bottom of file menu
-                    const rank = 150;
+                    let rank = 150;
                     mainMenu.fileMenu.addGroup(menu, rank);
                     console.log('rsp-savequit: ...loaded.');
                 }
 
                 function hubDeleteRequest(app) {
-                    const svcManager = app.serviceManager;
-                    const settings = svcManager.serverSettings;
-                    const endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_3__.PageConfig.getBaseUrl() + 'rubin/hub';
-                    const init = {
-                        method: 'DELETE'
+                    let svcManager = app.serviceManager;
+                    let settings = svcManager.serverSettings;
+                    let endpoint = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_3__.PageConfig.getBaseUrl() + "rubin/hub";
+                    let init = {
+                        method: "DELETE",
                     };
-                    console.log('hubRequest: URL: ', endpoint, ' | Settings:', settings);
+                    console.log("hubRequest: URL: ", endpoint, " | Settings:", settings);
                     return _jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.ServerConnection.makeRequest(endpoint, init, settings);
                 }
 
                 function saveAll(app, docManager, svcManager) {
-                    const promises = [];
+                    let promises = [];
                     (0, _lumino_algorithm__WEBPACK_IMPORTED_MODULE_5__.each)(app.shell.widgets('main'), widget => {
                         if (widget) {
-                            const context = docManager.contextForWidget(widget);
+                            let context = docManager.contextForWidget(widget);
                             if (context) {
-                                console.log('Saving context for widget:', {
+                                console.log("Saving context for widget:", {
                                     id: widget.id
                                 });
                                 promises.push(context.save());
                             } else {
-                                console.log('No context for widget:', {
+                                console.log("No context for widget:", {
                                     id: widget.id
                                 });
                             }
                         }
                     });
-                    console.log('Waiting for all save-document promises to resolve.');
+                    console.log("Waiting for all save-document promises to resolve.");
                     let r = Promise.resolve(1);
                     if (promises) {
                         Promise.all(promises);
                         r = promises[0];
                     }
                     return r;
                 }
 
-                function saveAndQuit(app, docManager, svcManager, logout) {
+                function saveAndQuit(app, docManager, svcManager) {
                     infoDialog();
                     const retval = Promise.resolve(saveAll(app, docManager, svcManager));
-                    retval.then(res => {
-                        return justQuit(app, docManager, svcManager, logout);
+                    retval.then((res) => {
+                        return justQuit(app, docManager, svcManager);
                     });
-                    retval.catch(err => {
-                        console.log('saveAll failed: ', err.message);
+                    retval.catch((err) => {
+                        console.log("saveAll failed: ", err.message);
                     });
-                    console.log('Save and Quit complete.');
+                    console.log("Save and Quit complete.");
                     return retval;
                 }
 
-                function justQuit(app, docManager, svcManager, logout) {
+                function justQuit(app, docManager, svcManager) {
                     infoDialog();
-                    let targetEndpoint = '/';
-                    if (logout) {
-                        targetEndpoint = '/logout';
-                    }
+                    let targetEndpoint = "/";
                     return Promise.resolve(hubDeleteRequest(app)
                         .then(() => {
-                            console.log('Quit complete.');
+                            console.log("Quit complete.");
                         })
                         .then(() => {
                             window.location.replace(targetEndpoint);
                         }));
                 }
 
                 function infoDialog() {
-                    const options = {
-                        title: 'Redirecting to landing page',
-                        body: 'JupyterLab cleaning up and redirecting to landing page.',
+                    let options = {
+                        title: "Redirecting to landing page",
+                        body: "JupyterLab cleaning up and redirecting to landing page.",
                         buttons: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.Dialog.okButton({
                             label: 'Got it!'
                         })]
                     };
                     return (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.showDialog)(options).then(() => {
-                        console.log('Info dialog panel displayed');
+                        console.log("Info dialog panel displayed");
                     });
                 }
                 /**
                  * Initialization data for the rspSavequit extension.
                  */
                 const rspSavequitExtension = {
                     activate: activateRSPSavequitExtension,
                     id: _tokens__WEBPACK_IMPORTED_MODULE_6__.SAVEQUIT_ID,
-                    requires: [_jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_1__.IMainMenu, _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_2__.IDocumentManager],
-                    autoStart: false
+                    requires: [
+                        _jupyterlab_mainmenu__WEBPACK_IMPORTED_MODULE_1__.IMainMenu,
+                        _jupyterlab_docmanager__WEBPACK_IMPORTED_MODULE_2__.IDocumentManager
+                    ],
+                    autoStart: false,
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (rspSavequitExtension);
 
 
                 /***/
             }),
@@ -724,23 +701,23 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "DISPLAYVERSION_ID": () => ( /* binding */ DISPLAYVERSION_ID),
-                    /* harmony export */
                     "NS": () => ( /* binding */ NS),
                     /* harmony export */
                     "PLUGIN_ID": () => ( /* binding */ PLUGIN_ID),
                     /* harmony export */
-                    "QUERY_ID": () => ( /* binding */ QUERY_ID),
+                    "DISPLAYVERSION_ID": () => ( /* binding */ DISPLAYVERSION_ID),
+                    /* harmony export */
+                    "SAVEQUIT_ID": () => ( /* binding */ SAVEQUIT_ID),
                     /* harmony export */
-                    "SAVEQUIT_ID": () => ( /* binding */ SAVEQUIT_ID)
+                    "QUERY_ID": () => ( /* binding */ QUERY_ID)
                     /* harmony export */
                 });
                 /**
                  * Namespace for everything
                  */
                 /*import { Token } from '@lumino/coreutils';*/
                 const NS = 'rsp-jupyterlab';
@@ -751,8 +728,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.141932b86bb94d1168ff.js.map
+//# sourceMappingURL=lib_index_js.e0bf8ba868c627d5e57b.js.map
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js.map` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js.map`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7922077922077921%*

 * *Differences: {"'file'": "'lib_index_js.e0bf8ba868c627d5e57b.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;AAA+B;AACgC;AACd;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,gDAAmB,CAAC,2DAAQ,IAAI,WAAW,eAAe,aAAa,cAAc,GAAG;AACpG;AACO,gCAAgC,8DAAY;AACnD;AACA;AACA;AACA;AACA,kBAAkB,2DAAS;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gDAAmB,+BAA+B,oDAAoD;AACtH;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iEAAe,iBAAiB,EAAC;;;;;;;;;;;;;;;;;;;;;;;;ACtCjC;AACA;AACmD;AACK;AACL;AACC;AAClB;AAClC;AACA;AACA;AACO;AACP;AACA;AA […]*

```diff
@@ -1,23 +1,23 @@
 {
-    "file": "lib_index_js.141932b86bb94d1168ff.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;AAA+B;AACgC;AACd;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,WAAW,gDAAmB,CAAC,2DAAQ,IAAI,WAAW,aAAa,aAAa,YAAY,GAAG;AAC/F;AACO,gCAAgC,8DAAY;AACnD;AACA;AACA;AACA;AACA,kBAAkB,2DAAS;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gDAAmB,+BAA+B,oDAAoD;AACtH;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iEAAe,iBAAiB,EAAC;;;;;;;;;;;;;;;;;;;;;;;;ACrCjC;AACA;AACmD;AACK;AACL;AACC;AAClB;AAClC;AACA;AACA;AACO;AACP;AACA;AACA,qBAAqB,wEAAqB;AAC1C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uCAAuC;AACvC;AACA;AACA;AACA;AACA,qCAAqC;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yCAAyC,0DAAiB;AAC1D;AACA;AACA,SAAS;AACT,qCAAqC,sDAAuB;AAC5D;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,8EAA4B;AAC3C;AACA;AACA,8BAA8B,gFAA8B;AAC5D,iBAAiB;AACjB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,sDAAuB;AAC/B,eAAe,6DAAU;AACzB;AACA;AACA,iEAAe,0BAA0B,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;AC3FS;AACF;AACS;AACY;AAClB;AACM;AACxB;AAClC;AACA;AACA;AACA,IAAI,mFAAkC;AACtC;AACA;AACA,IAAI,uEAA4B;AAChC;AACA;AACA,IAAI,iEAAyB;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAe;AACvB,eAAe,2DAAS,EAAE,oEAAgB,EAAE,6DAAU;AACtD;AACA;AACA,iEAAe,YAAY,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AC7B5B;AACA;AACuC;AACmB;AACT;AACS;AACF;AACL;AACV;AACP;AAClC;AACA;AACA;AACO;AACP;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACO;AACP;AACA;AACA,YAAY,WAAW;AACvB;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA,mBAAmB;AACnB,0BAA0B,iDAAI;AAC9B;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA,2BAA2B,mDAAM;AACjC;AACA,gBAAgB,iCAAiC;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,qEAAmB,IAAI,iEAAe,GAAG,iBAAiB;AAC5E;AACA,WAAW,gEAAU;AACrB;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,wBAAwB,+EAA6B;AACrD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL,WAAW,8EAA4B;AACvC;AACA;AACA,0BAA0B,gFAA8B;AACxD,aAAa;AACb;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,aAAa;AACb;AACA;AACA;AACA;AACA,SAAS;AACT,yBAAyB,wEAAqB;AAC9C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,6CAAc;AACtB,eAAe,2DAAS,EAAE,oEAAgB;AAC1C;AACA;AACA,iEAAe,iBAAiB,EAAC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,0BAA0B;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;AC1K3B;AACA;AAC0D;AACT;AACS;AACP;AACK;AACf;AACP;AAClC;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACO;AACP;AACA;AACA,YAAY,WAAW;AACvB;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,UAAU,8BAA8B;AACxC,UAAU,8BAA8B;AACxC,UAAU;AACV;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qBAAqB,wEAAqB;AAC1C;AACA;AACA;AACA;AACA,WAAW,8EAA4B;AACvC;AACA;AACA;AACA,IAAI,uDAAI;AACR;AACA;AACA;AACA,4DAA4D,eAAe;AAC3E;AACA;AACA;AACA,wDAAwD,eAAe;AACvE;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA,kBAAkB,iEAAe,GAAG,kBAAkB;AACtD;AACA,WAAW,gEAAU;AACrB;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,gDAAiB;AACzB,eAAe,2DAAS,EAAE,oEAAgB;AAC1C;AACA;AACA,iEAAe,oBAAoB,EAAC;;;;;;;;;;;;;;;;;;;ACtIpC;AACA;AACA;AACA,WAAW,QAAQ,yBAAyB;AACrC;AACA,qBAAqB,GAAG;AACxB,6BAA6B,GAAG;AAChC,uBAAuB,GAAG;AAC1B,oBAAoB,GAAG",
+    "file": "lib_index_js.e0bf8ba868c627d5e57b.js",
+    "mappings": ";;;;;;;;;;;;;;;;;;;;AAA+B;AACgC;AACd;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,YAAY,gDAAmB,CAAC,2DAAQ,IAAI,WAAW,eAAe,aAAa,cAAc,GAAG;AACpG;AACO,gCAAgC,8DAAY;AACnD;AACA;AACA;AACA;AACA,kBAAkB,2DAAS;AAC3B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gBAAgB,gDAAmB,+BAA+B,oDAAoD;AACtH;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iEAAe,iBAAiB,EAAC;;;;;;;;;;;;;;;;;;;;;;;;ACtCjC;AACA;AACmD;AACK;AACL;AACC;AAClB;AAClC;AACA;AACA;AACO;AACP;AACA;AACA,mBAAmB,wEAAqB;AACxC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,yCAAyC,0DAAiB;AAC1D;AACA;AACA,SAAS;AACT,qCAAqC,sDAAuB;AAC5D;AACA;AACA;AACA;AACA,SAAS;AACT,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,8EAA4B;AAC3C;AACA;AACA,8BAA8B,gFAA8B;AAC5D,iBAAiB;AACjB;AACA;AACA,SAAS;AACT;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,sDAAuB;AAC/B;AACA,QAAQ,6DAAU;AAClB;AACA;AACA;AACA,iEAAe,0BAA0B,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;ACjFS;AACF;AACS;AACa;AAClB;AACM;AACzB;AAClC;AACA;AACA;AACA,IAAI,mFAAkC;AACtC;AACA;AACA,IAAI,uEAA4B;AAChC;AACA;AACA,IAAI,iEAAyB;AAC7B;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,8CAAe;AACvB;AACA,QAAQ,2DAAS;AACjB,QAAQ,oEAAgB;AACxB,QAAQ,6DAAU;AAClB;AACA;AACA;AACA,iEAAe,YAAY,EAAC;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACjC5B;AACA;AACuC;AACmB;AACT;AACS;AACF;AACL;AACV;AACP;AAClC;AACA;AACA;AACO;AACP;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACA;AACO;AACP;AACA;AACA,YAAY,WAAW;AACvB;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA,iBAAiB;AACjB,wBAAwB,iDAAI;AAC5B;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA,2BAA2B,mDAAM;AACjC;AACA,gBAAgB,iCAAiC;AACjD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,kBAAkB,qEAAmB,IAAI,iEAAe,GAAG,iBAAiB;AAC5E;AACA,WAAW,gEAAU;AACrB;AACA;AACA,gDAAgD;AAChD;AACA;AACA;AACA;AACA,gDAAgD;AAChD;AACA;AACA;AACA;AACA;AACA;AACA,4CAA4C;AAC5C,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,sBAAsB,+EAA6B;AACnD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL,WAAW,8EAA4B;AACvC;AACA;AACA,0BAA0B,gFAA8B;AACxD,aAAa;AACb;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,gDAAgD;AAChD;AACA;AACA;AACA;AACA,SAAS;AACT,uBAAuB,wEAAqB;AAC5C;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,SAAS;AACT,4CAA4C;AAC5C,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,6CAAc;AACtB;AACA,QAAQ,2DAAS;AACjB,QAAQ,oEAAgB;AACxB;AACA;AACA;AACA,iEAAe,iBAAiB,EAAC;AACjC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,0BAA0B;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACpK3B;AACA;AAC0D;AACT;AACS;AACP;AACK;AACf;AACP;AAClC;AACA;AACA;AACO;AACP;AACA;AACA;AACA,CAAC,gCAAgC;AACjC;AACA;AACA;AACA;AACO;AACP;AACA;AACA,YAAY,WAAW;AACvB;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,UAAU,8BAA8B;AACxC,UAAU,8BAA8B;AACxC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,wEAAqB;AACxC;AACA;AACA;AACA;AACA,WAAW,8EAA4B;AACvC;AACA;AACA;AACA,IAAI,uDAAI;AACR;AACA;AACA;AACA,4DAA4D,eAAe;AAC3E;AACA;AACA;AACA,wDAAwD,eAAe;AACvE;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,KAAK;AACL;AACA;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA,kBAAkB,iEAAe,GAAG,kBAAkB;AACtD;AACA,WAAW,gEAAU;AACrB;AACA,KAAK;AACL;AACA;AACA;AACA;AACA;AACA;AACA,QAAQ,gDAAiB;AACzB;AACA,QAAQ,2DAAS;AACjB,QAAQ,oEAAgB;AACxB;AACA;AACA;AACA,iEAAe,oBAAoB,EAAC;;;;;;;;;;;;;;;;;;;AC9HpC;AACA;AACA;AACA,WAAW,QAAQ,yBAAyB;AACrC;AACA,qBAAqB,GAAG;AACxB,6BAA6B,GAAG;AAChC,uBAAuB,GAAG;AAC1B,oBAAoB,GAAG",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://rsp-jupyter-extensions/./lib/DisplayLabVersion.js",
         "webpack://rsp-jupyter-extensions/./lib/displayversion.js",
         "webpack://rsp-jupyter-extensions/./lib/index.js",
         "webpack://rsp-jupyter-extensions/./lib/query.js",
         "webpack://rsp-jupyter-extensions/./lib/savequit.js",
         "webpack://rsp-jupyter-extensions/./lib/tokens.js"
     ],
     "sourcesContent": [
-        "import * as React from 'react';\nimport { VDomModel, VDomRenderer } from '@jupyterlab/apputils';\nimport { TextItem } from '@jupyterlab/statusbar';\n/**\n * A pure function for rendering the displayversion information.\n *\n * @param props: the props for rendering the component.\n *\n * @returns a tsx component for displaying version information.\n */\nfunction DisplayLabVersionComponent(props) {\n    return React.createElement(TextItem, { source: `${props.source}`, title: `${props.title}` });\n}\nexport class DisplayLabVersion extends VDomRenderer {\n    /**\n     * Create a new DisplayLabVersion widget.\n     */\n    constructor(props) {\n        super(new VDomModel());\n        this.props = props;\n    }\n    /**\n     * Render the display Lab version widget.\n     */\n    render() {\n        if (!this.props) {\n            return null;\n        }\n        return (React.createElement(DisplayLabVersionComponent, { source: this.props.source, title: this.props.title }));\n    }\n    /**\n     * Dispose of the item.\n     */\n    dispose() {\n        super.dispose();\n    }\n}\nexport default DisplayLabVersion;\n",
-        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { IStatusBar } from '@jupyterlab/statusbar';\nimport DisplayLabVersion from './DisplayLabVersion';\nimport * as token from './tokens';\n/**\n * Activate the extension.\n */\nexport function activateRSPDisplayVersionExtension(app, statusBar) {\n    console.log('RSP DisplayVersion extension: loading...');\n    const svcManager = app.serviceManager;\n    const endpoint = PageConfig.getBaseUrl() + 'rubin/environment';\n    const init = {\n        method: 'GET'\n    };\n    const settings = svcManager.serverSettings;\n    apiRequest(endpoint, init, settings).then(res => {\n        const image_description = res.IMAGE_DESCRIPTION || '';\n        const image_digest = res.IMAGE_DIGEST;\n        const image_spec = res.JUPYTER_IMAGE_SPEC;\n        const instance_url = new URL(res.EXTERNAL_INSTANCE_URL || '');\n        const hostname = ' ' + instance_url.hostname;\n        let digest_str = '';\n        let imagename = '';\n        if (image_spec) {\n            /* First try to get digest out of image spec (nublado v3) */\n            const imagearr = image_spec.split('/');\n            const pullname = imagearr[imagearr.length - 1];\n            const partsarr = pullname.split('@');\n            if (partsarr.length === 2) {\n                /* Split name and sha; \"sha256:\" is seven characters */\n                digest_str = ' [' + partsarr[1].substring(7, 7 + 8) + '...]';\n                imagename = ' (' + partsarr[0] + ')';\n            }\n            else {\n                /* Nothing to split; image name is the name we pulled by */\n                imagename = ' (' + pullname + ')';\n            }\n            if (digest_str === '' && image_digest) {\n                /* No digest in spec?  Well, did we set IMAGE_DIGEST?\n                   Yes, if we are nubladov2. */\n                digest_str = ' [' + image_digest.substring(0, 8) + '...]';\n            }\n        }\n        const label = image_description + digest_str + imagename + hostname;\n        const displayVersionWidget = new DisplayLabVersion({\n            source: label,\n            title: image_description\n        });\n        statusBar.registerStatusItem(token.DISPLAYVERSION_ID, {\n            item: displayVersionWidget,\n            align: 'left',\n            rank: 80,\n            isActive: () => true\n        });\n    });\n    function apiRequest(url, init, settings) {\n        /**\n         * Make a request to our endpoint to get the version\n         *\n         * @param url - the path for the displayversion extension\n         *\n         * @param init - The GET for the extension\n         *\n         * @param settings - the settings for the current notebook server\n         *\n         * @returns a Promise resolved with the JSON response\n         */\n        // Fake out URL check in makeRequest\n        return ServerConnection.makeRequest(url, init, settings).then(response => {\n            if (response.status !== 200) {\n                return response.json().then(data => {\n                    throw new ServerConnection.ResponseError(response, data.message);\n                });\n            }\n            return response.json();\n        });\n    }\n    console.log('RSP DisplayVersion extension: ... loaded');\n}\n/**\n * Initialization data for the RSPdisplayversionextension extension.\n */\nconst rspDisplayVersionExtension = {\n    activate: activateRSPDisplayVersionExtension,\n    id: token.DISPLAYVERSION_ID,\n    requires: [IStatusBar],\n    autoStart: false\n};\nexport default rspDisplayVersionExtension;\n",
-        "import { IStatusBar } from '@jupyterlab/statusbar';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { activateRSPDisplayVersionExtension } from './displayversion';\nimport { activateRSPQueryExtension } from './query';\nimport { activateRSPSavequitExtension } from './savequit';\nimport * as token from './tokens';\nfunction activateRSPExtension(app, mainMenu, docManager, statusBar) {\n    console.log('rsp-lab-extension: loading...');\n    console.log('...activating displayversion extension...');\n    activateRSPDisplayVersionExtension(app, statusBar);\n    console.log('...activated...');\n    console.log('...activating savequit extension...');\n    activateRSPSavequitExtension(app, mainMenu, docManager);\n    console.log('...activated...');\n    console.log('...activating query extension...');\n    activateRSPQueryExtension(app, mainMenu, docManager);\n    console.log('...activated...');\n    console.log('...loaded rsp-lab-extension.');\n}\n/**\n * Initialization data for the rspExtensions.\n */\nconst rspExtension = {\n    activate: activateRSPExtension,\n    id: token.PLUGIN_ID,\n    requires: [IMainMenu, IDocumentManager, IStatusBar],\n    autoStart: true\n};\nexport default rspExtension;\n",
-        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { Menu } from '@lumino/widgets';\nimport { showDialog, Dialog } from '@jupyterlab/apputils';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { Widget } from '@lumino/widgets';\nimport * as token from './tokens';\n/**\n * The command IDs used by the plugin.\n */\nexport var CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.rubinquery = 'rubinquery';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * Activate the extension.\n */\nexport function activateRSPQueryExtension(app, mainMenu, docManager) {\n    console.log('rsp-query...loading');\n    const svcManager = app.serviceManager;\n    const { commands } = app;\n    commands.addCommand(CommandIDs.rubinquery, {\n        label: 'Open from portal query URL...',\n        caption: 'Open notebook from supplied portal query URL',\n        execute: () => {\n            rubinportalquery(app, docManager, svcManager);\n        }\n    });\n    // Add commands and menu itmes.\n    const menu = { command: CommandIDs.rubinquery };\n    const rubinmenu = new Menu({\n        commands\n    });\n    rubinmenu.title.label = 'Rubin';\n    rubinmenu.insertItem(0, menu);\n    mainMenu.addMenu(rubinmenu);\n    console.log('rsp-query...loaded');\n}\nclass QueryHandler extends Widget {\n    constructor() {\n        super({ node: Private.createQueryNode() });\n        this.addClass('rubin-qh');\n    }\n    get inputNode() {\n        return this.node.getElementsByTagName('input')[0];\n    }\n    getValue() {\n        return this.inputNode.value;\n    }\n}\nfunction queryDialog(manager) {\n    const options = {\n        title: 'Query Value',\n        body: new QueryHandler(),\n        focusNodeSelector: 'input',\n        buttons: [Dialog.cancelButton(), Dialog.okButton({ label: 'CREATE' })]\n    };\n    return showDialog(options).then(result => {\n        if (!result) {\n            console.log('No result from queryDialog');\n            return new Promise((res, rej) => {\n                /* Nothing */\n            });\n        }\n        console.log('Result from queryDialog: ', result);\n        if (!result.value) {\n            console.log('No result.value from queryDialog');\n            return new Promise((res, rej) => {\n                /* Nothing */\n            });\n        }\n        if (result.button.label === 'CREATE') {\n            console.log('Got result ', result.value, ' from queryDialog: CREATE');\n            return Promise.resolve(result.value);\n        }\n        console.log('Did not get queryDialog: CREATE');\n        return new Promise((res, rej) => {\n            /* Nothing */\n        });\n    });\n}\nfunction apiRequest(url, init, settings) {\n    /**\n     * Make a request to our endpoint to get a pointer to a templated\n     *  notebook for a given query\n     *\n     * @param url - the path for the query extension\n     *\n     * @param init - The POST + body for the extension\n     *\n     * @param settings - the settings for the current notebook server.\n     *\n     * @returns a Promise resolved with the JSON response\n     */\n    // Fake out URL check in makeRequest\n    const newSettings = ServerConnection.makeSettings({\n        baseUrl: settings.baseUrl,\n        appUrl: settings.appUrl,\n        wsUrl: settings.wsUrl,\n        init: settings.init,\n        token: settings.token,\n        Request: settings.Request,\n        Headers: settings.Headers,\n        WebSocket: settings.WebSocket\n    });\n    return ServerConnection.makeRequest(url, init, newSettings).then(response => {\n        if (response.status !== 200) {\n            return response.json().then(data => {\n                throw new ServerConnection.ResponseError(response, data.message);\n            });\n        }\n        return response.json();\n    });\n}\nfunction rubinportalquery(app, docManager, svcManager) {\n    queryDialog(docManager).then(url => {\n        console.log('Query URL is', url);\n        if (!url) {\n            console.log('Query URL was null');\n            return new Promise((res, rej) => {\n                /* Nothing */\n            });\n        }\n        const body = JSON.stringify({\n            type: 'portal',\n            value: url\n        });\n        const endpoint = PageConfig.getBaseUrl() + 'rubin/query';\n        const init = {\n            method: 'POST',\n            body: body\n        };\n        const settings = svcManager.serverSettings;\n        apiRequest(endpoint, init, settings).then(res => {\n            const path = res.path;\n            docManager.open(path);\n        });\n        return new Promise((res, rej) => {\n            /* Nothing */\n        });\n    });\n}\n/**\n * Initialization data for the jupyterlab-lsstquery extension.\n */\nconst rspQueryExtension = {\n    activate: activateRSPQueryExtension,\n    id: token.QUERY_ID,\n    requires: [IMainMenu, IDocumentManager],\n    autoStart: false\n};\nexport default rspQueryExtension;\nvar Private;\n(function (Private) {\n    /**\n     * Create node for query handler.\n     */\n    function createQueryNode() {\n        const body = document.createElement('div');\n        const qidLabel = document.createElement('label');\n        qidLabel.textContent = 'Enter Query Value';\n        const name = document.createElement('input');\n        body.appendChild(qidLabel);\n        body.appendChild(name);\n        return body;\n    }\n    Private.createQueryNode = createQueryNode;\n})(Private || (Private = {}));\n",
-        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { showDialog, Dialog } from '@jupyterlab/apputils';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { each } from '@lumino/algorithm';\nimport * as token from './tokens';\n/**\n * The command IDs used by the plugin.\n */\nexport var CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.justQuit = 'justquit:justquit';\n    CommandIDs.saveQuit = 'savequit:savequit';\n    CommandIDs.saveLogout = 'savelogout:savelogout';\n})(CommandIDs || (CommandIDs = {}));\n/**\n * Activate the jupyterhub extension.\n */\nexport function activateRSPSavequitExtension(app, mainMenu, docManager) {\n    console.log('rsp-savequit: loading...');\n    const svcManager = app.serviceManager;\n    const { commands } = app;\n    commands.addCommand(CommandIDs.justQuit, {\n        label: 'Exit Without Saving',\n        caption: 'Destroy container',\n        execute: () => {\n            justQuit(app, docManager, svcManager, false);\n        }\n    });\n    commands.addCommand(CommandIDs.saveQuit, {\n        label: 'Save All and Exit',\n        caption: 'Save open notebooks and destroy container',\n        execute: () => {\n            saveAndQuit(app, docManager, svcManager, false);\n        }\n    });\n    commands.addCommand(CommandIDs.saveLogout, {\n        label: 'Save All, Exit, and Log Out',\n        caption: 'Save open notebooks, destroy container, and log out',\n        execute: () => {\n            saveAndQuit(app, docManager, svcManager, true);\n        }\n    });\n    // Add commands and menu itmes.\n    const menu = [\n        { command: CommandIDs.justQuit },\n        { command: CommandIDs.saveQuit },\n        { command: CommandIDs.saveLogout }\n    ];\n    // Put it at the bottom of file menu\n    const rank = 150;\n    mainMenu.fileMenu.addGroup(menu, rank);\n    console.log('rsp-savequit: ...loaded.');\n}\nfunction hubDeleteRequest(app) {\n    const svcManager = app.serviceManager;\n    const settings = svcManager.serverSettings;\n    const endpoint = PageConfig.getBaseUrl() + 'rubin/hub';\n    const init = {\n        method: 'DELETE'\n    };\n    console.log('hubRequest: URL: ', endpoint, ' | Settings:', settings);\n    return ServerConnection.makeRequest(endpoint, init, settings);\n}\nfunction saveAll(app, docManager, svcManager) {\n    const promises = [];\n    each(app.shell.widgets('main'), widget => {\n        if (widget) {\n            const context = docManager.contextForWidget(widget);\n            if (context) {\n                console.log('Saving context for widget:', { id: widget.id });\n                promises.push(context.save());\n            }\n            else {\n                console.log('No context for widget:', { id: widget.id });\n            }\n        }\n    });\n    console.log('Waiting for all save-document promises to resolve.');\n    let r = Promise.resolve(1);\n    if (promises) {\n        Promise.all(promises);\n        r = promises[0];\n    }\n    return r;\n}\nfunction saveAndQuit(app, docManager, svcManager, logout) {\n    infoDialog();\n    const retval = Promise.resolve(saveAll(app, docManager, svcManager));\n    retval.then(res => {\n        return justQuit(app, docManager, svcManager, logout);\n    });\n    retval.catch(err => {\n        console.log('saveAll failed: ', err.message);\n    });\n    console.log('Save and Quit complete.');\n    return retval;\n}\nfunction justQuit(app, docManager, svcManager, logout) {\n    infoDialog();\n    let targetEndpoint = '/';\n    if (logout) {\n        targetEndpoint = '/logout';\n    }\n    return Promise.resolve(hubDeleteRequest(app)\n        .then(() => {\n        console.log('Quit complete.');\n    })\n        .then(() => {\n        window.location.replace(targetEndpoint);\n    }));\n}\nfunction infoDialog() {\n    const options = {\n        title: 'Redirecting to landing page',\n        body: 'JupyterLab cleaning up and redirecting to landing page.',\n        buttons: [Dialog.okButton({ label: 'Got it!' })]\n    };\n    return showDialog(options).then(() => {\n        console.log('Info dialog panel displayed');\n    });\n}\n/**\n * Initialization data for the rspSavequit extension.\n */\nconst rspSavequitExtension = {\n    activate: activateRSPSavequitExtension,\n    id: token.SAVEQUIT_ID,\n    requires: [IMainMenu, IDocumentManager],\n    autoStart: false\n};\nexport default rspSavequitExtension;\n",
+        "import * as React from 'react';\nimport { VDomModel, VDomRenderer } from '@jupyterlab/apputils';\nimport { TextItem } from '@jupyterlab/statusbar';\n/**\n * A pure function for rendering the displayversion information.\n *\n * @param props: the props for rendering the component.\n *\n * @returns a tsx component for displaying version information.\n */\nfunction DisplayLabVersionComponent(props) {\n    return (React.createElement(TextItem, { source: `${(props.source)}`, title: `${(props.title)}` }));\n}\nexport class DisplayLabVersion extends VDomRenderer {\n    /**\n     * Create a new DisplayLabVersion widget.\n     */\n    constructor(props) {\n        super(new VDomModel());\n        this.props = props;\n    }\n    /**\n     * Render the display Lab version widget.\n     */\n    render() {\n        if (!this.props) {\n            return null;\n        }\n        return (React.createElement(DisplayLabVersionComponent, { source: this.props.source, title: this.props.title }));\n    }\n    /**\n     * Dispose of the item.\n     */\n    dispose() {\n        super.dispose();\n    }\n}\n;\nexport default DisplayLabVersion;\n",
+        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { IStatusBar } from '@jupyterlab/statusbar';\nimport DisplayLabVersion from \"./DisplayLabVersion\";\nimport * as token from \"./tokens\";\n/**\n * Activate the extension.\n */\nexport function activateRSPDisplayVersionExtension(app, statusBar) {\n    console.log('RSP DisplayVersion extension: loading...');\n    let svcManager = app.serviceManager;\n    let endpoint = PageConfig.getBaseUrl() + \"rubin/environment\";\n    let init = {\n        method: \"GET\"\n    };\n    let settings = svcManager.serverSettings;\n    apiRequest(endpoint, init, settings).then((res) => {\n        let image_description = (res.IMAGE_DESCRIPTION || \"\");\n        let image_digest = res.IMAGE_DIGEST;\n        let image_spec = res.JUPYTER_IMAGE_SPEC;\n        let instance_url = new URL(res.EXTERNAL_INSTANCE_URL || \"\");\n        let hostname = \" \" + instance_url.hostname;\n        let digest_str = \"\";\n        if (image_digest) {\n            digest_str = \" [\" + image_digest.substring(0, 8) + \"...]\";\n        }\n        let imagename = \"\";\n        if (image_spec) {\n            let imagearr = image_spec.split(\"/\");\n            imagename = \" (\" + imagearr[imagearr.length - 1] + \")\";\n        }\n        let label = image_description + digest_str + imagename + hostname;\n        const displayVersionWidget = new DisplayLabVersion({\n            source: label,\n            title: image_description\n        });\n        statusBar.registerStatusItem(token.DISPLAYVERSION_ID, {\n            item: displayVersionWidget,\n            align: \"left\",\n            rank: 80,\n            isActive: () => true\n        });\n    });\n    function apiRequest(url, init, settings) {\n        /**\n        * Make a request to our endpoint to get the version\n        *\n        * @param url - the path for the displayversion extension\n        *\n        * @param init - The GET for the extension\n        *\n        * @param settings - the settings for the current notebook server\n        *\n        * @returns a Promise resolved with the JSON response\n        */\n        // Fake out URL check in makeRequest\n        return ServerConnection.makeRequest(url, init, settings).then(response => {\n            if (response.status !== 200) {\n                return response.json().then(data => {\n                    throw new ServerConnection.ResponseError(response, data.message);\n                });\n            }\n            return response.json();\n        });\n    }\n    console.log('RSP DisplayVersion extension: ... loaded');\n}\n;\n/**\n * Initialization data for the RSPdisplayversionextension extension.\n */\nconst rspDisplayVersionExtension = {\n    activate: activateRSPDisplayVersionExtension,\n    id: token.DISPLAYVERSION_ID,\n    requires: [\n        IStatusBar,\n    ],\n    autoStart: false,\n};\nexport default rspDisplayVersionExtension;\n",
+        "import { IStatusBar } from '@jupyterlab/statusbar';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { activateRSPDisplayVersionExtension, } from \"./displayversion\";\nimport { activateRSPQueryExtension, } from \"./query\";\nimport { activateRSPSavequitExtension, } from \"./savequit\";\nimport * as token from \"./tokens\";\nfunction activateRSPExtension(app, mainMenu, docManager, statusBar) {\n    console.log('rsp-lab-extension: loading...');\n    console.log('...activating displayversion extension...');\n    activateRSPDisplayVersionExtension(app, statusBar);\n    console.log('...activated...');\n    console.log('...activating savequit extension...');\n    activateRSPSavequitExtension(app, mainMenu, docManager);\n    console.log('...activated...');\n    console.log('...activating query extension...');\n    activateRSPQueryExtension(app, mainMenu, docManager);\n    console.log('...activated...');\n    console.log('...loaded rsp-lab-extension.');\n}\n/**\n * Initialization data for the rspExtensions.\n */\nconst rspExtension = {\n    activate: activateRSPExtension,\n    id: token.PLUGIN_ID,\n    requires: [\n        IMainMenu,\n        IDocumentManager,\n        IStatusBar\n    ],\n    autoStart: true,\n};\nexport default rspExtension;\n",
+        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { Menu } from '@lumino/widgets';\nimport { showDialog, Dialog } from '@jupyterlab/apputils';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { Widget } from '@lumino/widgets';\nimport * as token from \"./tokens\";\n/**\n * The command IDs used by the plugin.\n */\nexport var CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.rubinquery = 'rubinquery';\n})(CommandIDs || (CommandIDs = {}));\n;\n/**\n * Activate the extension.\n */\nexport function activateRSPQueryExtension(app, mainMenu, docManager) {\n    console.log('rsp-query...loading');\n    let svcManager = app.serviceManager;\n    const { commands } = app;\n    commands.addCommand(CommandIDs.rubinquery, {\n        label: 'Open from portal query URL...',\n        caption: 'Open notebook from supplied portal query URL',\n        execute: () => {\n            rubinportalquery(app, docManager, svcManager);\n        }\n    });\n    // Add commands and menu itmes.\n    let menu = { command: CommandIDs.rubinquery };\n    let rubinmenu = new Menu({\n        commands,\n    });\n    rubinmenu.title.label = \"Rubin\";\n    rubinmenu.insertItem(0, menu);\n    mainMenu.addMenu(rubinmenu);\n    console.log('rsp-query...loaded');\n}\nclass QueryHandler extends Widget {\n    constructor() {\n        super({ node: Private.createQueryNode() });\n        this.addClass('rubin-qh');\n    }\n    get inputNode() {\n        return this.node.getElementsByTagName('input')[0];\n    }\n    getValue() {\n        return this.inputNode.value;\n    }\n}\nfunction queryDialog(manager) {\n    let options = {\n        title: 'Query Value',\n        body: new QueryHandler(),\n        focusNodeSelector: 'input',\n        buttons: [Dialog.cancelButton(), Dialog.okButton({ label: 'CREATE' })]\n    };\n    return showDialog(options).then(result => {\n        if (!result) {\n            console.log(\"No result from queryDialog\");\n            return new Promise((res, rej) => { });\n        }\n        console.log(\"Result from queryDialog: \", result);\n        if (!result.value) {\n            console.log(\"No result.value from queryDialog\");\n            return new Promise((res, rej) => { });\n        }\n        if (result.button.label === 'CREATE') {\n            console.log(\"Got result \", result.value, \" from queryDialog: CREATE\");\n            return Promise.resolve(result.value);\n        }\n        console.log(\"Did not get queryDialog: CREATE\");\n        return new Promise((res, rej) => { });\n    });\n}\nfunction apiRequest(url, init, settings) {\n    /**\n    * Make a request to our endpoint to get a pointer to a templated\n    *  notebook for a given query\n    *\n    * @param url - the path for the query extension\n    *\n    * @param init - The POST + body for the extension\n    *\n    * @param settings - the settings for the current notebook server.\n    *\n    * @returns a Promise resolved with the JSON response\n    */\n    // Fake out URL check in makeRequest\n    let newSettings = ServerConnection.makeSettings({\n        baseUrl: settings.baseUrl,\n        appUrl: settings.appUrl,\n        wsUrl: settings.wsUrl,\n        init: settings.init,\n        token: settings.token,\n        Request: settings.Request,\n        Headers: settings.Headers,\n        WebSocket: settings.WebSocket\n    });\n    return ServerConnection.makeRequest(url, init, newSettings).then(response => {\n        if (response.status !== 200) {\n            return response.json().then(data => {\n                throw new ServerConnection.ResponseError(response, data.message);\n            });\n        }\n        return response.json();\n    });\n}\nfunction rubinportalquery(app, docManager, svcManager) {\n    queryDialog(docManager).then(url => {\n        console.log(\"Query URL is\", url);\n        if (!url) {\n            console.log(\"Query URL was null\");\n            return new Promise((res, rej) => { });\n        }\n        let body = JSON.stringify({\n            \"type\": \"portal\",\n            \"value\": url\n        });\n        let endpoint = PageConfig.getBaseUrl() + \"rubin/query\";\n        let init = {\n            method: \"POST\",\n            body: body\n        };\n        let settings = svcManager.serverSettings;\n        apiRequest(endpoint, init, settings).then(function (res) {\n            let path = res.path;\n            docManager.open(path);\n        });\n        return new Promise((res, rej) => { });\n    });\n}\n/**\n * Initialization data for the jupyterlab-lsstquery extension.\n */\nconst rspQueryExtension = {\n    activate: activateRSPQueryExtension,\n    id: token.QUERY_ID,\n    requires: [\n        IMainMenu,\n        IDocumentManager\n    ],\n    autoStart: false,\n};\nexport default rspQueryExtension;\nvar Private;\n(function (Private) {\n    /**\n     * Create node for query handler.\n     */\n    function createQueryNode() {\n        let body = document.createElement('div');\n        let qidLabel = document.createElement('label');\n        qidLabel.textContent = 'Enter Query Value';\n        let name = document.createElement('input');\n        body.appendChild(qidLabel);\n        body.appendChild(name);\n        return body;\n    }\n    Private.createQueryNode = createQueryNode;\n})(Private || (Private = {}));\n",
+        "// Copyright (c) LSST DM/SQuaRE\n// Distributed under the terms of the MIT License.\nimport { showDialog, Dialog } from '@jupyterlab/apputils';\nimport { IMainMenu } from '@jupyterlab/mainmenu';\nimport { IDocumentManager } from '@jupyterlab/docmanager';\nimport { PageConfig } from '@jupyterlab/coreutils';\nimport { ServerConnection } from '@jupyterlab/services';\nimport { each } from '@lumino/algorithm';\nimport * as token from \"./tokens\";\n/**\n * The command IDs used by the plugin.\n */\nexport var CommandIDs;\n(function (CommandIDs) {\n    CommandIDs.saveQuit = 'savequit:savequit';\n    CommandIDs.justQuit = 'justquit:justquit';\n})(CommandIDs || (CommandIDs = {}));\n;\n/**\n * Activate the jupyterhub extension.\n */\nexport function activateRSPSavequitExtension(app, mainMenu, docManager) {\n    console.log('rsp-savequit: loading...');\n    let svcManager = app.serviceManager;\n    const { commands } = app;\n    commands.addCommand(CommandIDs.saveQuit, {\n        label: 'Save All and Exit',\n        caption: 'Save open notebooks and destroy container',\n        execute: () => {\n            saveAndQuit(app, docManager, svcManager);\n        }\n    });\n    commands.addCommand(CommandIDs.justQuit, {\n        label: 'Exit Without Saving',\n        caption: 'Destroy container',\n        execute: () => {\n            justQuit(app, docManager, svcManager);\n        }\n    });\n    // Add commands and menu itmes.\n    let menu = [\n        { command: CommandIDs.saveQuit },\n        { command: CommandIDs.justQuit },\n    ];\n    // Put it at the bottom of file menu\n    let rank = 150;\n    mainMenu.fileMenu.addGroup(menu, rank);\n    console.log('rsp-savequit: ...loaded.');\n}\nfunction hubDeleteRequest(app) {\n    let svcManager = app.serviceManager;\n    let settings = svcManager.serverSettings;\n    let endpoint = PageConfig.getBaseUrl() + \"rubin/hub\";\n    let init = {\n        method: \"DELETE\",\n    };\n    console.log(\"hubRequest: URL: \", endpoint, \" | Settings:\", settings);\n    return ServerConnection.makeRequest(endpoint, init, settings);\n}\nfunction saveAll(app, docManager, svcManager) {\n    let promises = [];\n    each(app.shell.widgets('main'), widget => {\n        if (widget) {\n            let context = docManager.contextForWidget(widget);\n            if (context) {\n                console.log(\"Saving context for widget:\", { id: widget.id });\n                promises.push(context.save());\n            }\n            else {\n                console.log(\"No context for widget:\", { id: widget.id });\n            }\n        }\n    });\n    console.log(\"Waiting for all save-document promises to resolve.\");\n    let r = Promise.resolve(1);\n    if (promises) {\n        Promise.all(promises);\n        r = promises[0];\n    }\n    return r;\n}\nfunction saveAndQuit(app, docManager, svcManager) {\n    infoDialog();\n    const retval = Promise.resolve(saveAll(app, docManager, svcManager));\n    retval.then((res) => {\n        return justQuit(app, docManager, svcManager);\n    });\n    retval.catch((err) => {\n        console.log(\"saveAll failed: \", err.message);\n    });\n    console.log(\"Save and Quit complete.\");\n    return retval;\n}\nfunction justQuit(app, docManager, svcManager) {\n    infoDialog();\n    let targetEndpoint = \"/\";\n    return Promise.resolve(hubDeleteRequest(app)\n        .then(() => {\n        console.log(\"Quit complete.\");\n    })\n        .then(() => {\n        window.location.replace(targetEndpoint);\n    }));\n}\nfunction infoDialog() {\n    let options = {\n        title: \"Redirecting to landing page\",\n        body: \"JupyterLab cleaning up and redirecting to landing page.\",\n        buttons: [Dialog.okButton({ label: 'Got it!' })]\n    };\n    return showDialog(options).then(() => {\n        console.log(\"Info dialog panel displayed\");\n    });\n}\n/**\n * Initialization data for the rspSavequit extension.\n */\nconst rspSavequitExtension = {\n    activate: activateRSPSavequitExtension,\n    id: token.SAVEQUIT_ID,\n    requires: [\n        IMainMenu,\n        IDocumentManager\n    ],\n    autoStart: false,\n};\nexport default rspSavequitExtension;\n",
         "/**\n * Namespace for everything\n */\n/*import { Token } from '@lumino/coreutils';*/\nexport const NS = 'rsp-jupyterlab';\nexport const PLUGIN_ID = `${NS}:plugin`;\nexport const DISPLAYVERSION_ID = `${NS}:displayversion`;\nexport const SAVEQUIT_ID = `${NS}:savequit`;\nexport const QUERY_ID = `${NS}:query`;\n"
     ],
     "version": 3
 }
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -35,16 +35,16 @@
                         })
                     );
                     __webpack_require__.R = undefined;
                     return getScope;
                 };
                 var init = (shareScope, initScope) => {
                     if (!__webpack_require__.S) return;
+                    var oldScope = __webpack_require__.S["default"];
                     var name = "default"
-                    var oldScope = __webpack_require__.S[name];
                     if (oldScope && oldScope !== shareScope) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                     __webpack_require__.S[name] = shareScope;
                     return __webpack_require__.I(name, initScope);
                 };
 
                 // This exports getters to disallow modifications
                 __webpack_require__.d(exports, {
@@ -182,17 +182,17 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "141932b86bb94d1168ff",
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "16e7a87b76c7b094dea7",
-                "style_index_js": "a3efb51ad79d669c319a"
+                "lib_index_js": "e0bf8ba868c627d5e57b",
+                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "0c809f0d01c979a08eee",
+                "style_index_js": "ace3aff4fb7c19d10cee"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -301,15 +301,17 @@
                 /******/
                 script.parentNode && script.parentNode.removeChild(script);
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
-            };
+            }
+            /******/
+            ;
             /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
@@ -409,29 +411,29 @@
                     /******/
                     var initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))
                     /******/
                     if (module.then) return promises.push(module.then(initFn, handleError));
                     /******/
                     var initResult = initFn(module);
                     /******/
-                    if (initResult && initResult.then) return promises.push(initResult['catch'](handleError));
+                    if (initResult && initResult.then) return promises.push(initResult.catch(handleError));
                     /******/
                 } catch (err) {
                     handleError(err);
                 }
                 /******/
             }
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("rsp-jupyter-extensions", "0.7.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("rsp-jupyter-extensions", "0.6.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -615,43 +617,35 @@
                 /******/
                 return !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;
                 /******/
             }, 0);
             /******/
         };
         /******/
-        var getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {
+        var getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {
             /******/
-            return "Unsatisfied version " + version + " from " + (version && scope[key][version].from) + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
-            /******/
-        };
-        /******/
-        var getSingleton = (scope, scopeName, key, requiredVersion) => {
-            /******/
-            var version = findSingletonVersionKey(scope, key);
-            /******/
-            return get(scope[key][version]);
+            return "Unsatisfied version " + version + " of shared singleton module " + key + " (required " + rangeToString(requiredVersion) + ")"
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var findValidVersion = (scope, key, requiredVersion) => {
             /******/
@@ -736,22 +730,14 @@
             /******/
             ensureExistence(scopeName, key);
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
-        var loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {
-            /******/
-            ensureExistence(scopeName, key);
-            /******/
-            return getSingleton(scope, scopeName, key);
-            /******/
-        });
-        /******/
         var loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {
             /******/
             ensureExistence(scopeName, key);
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -776,22 +762,14 @@
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));
             /******/
         });
         /******/
-        var loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {
-            /******/
-            if (!scope || !__webpack_require__.o(scope, key)) return fallback();
-            /******/
-            return getSingleton(scope, scopeName, key);
-            /******/
-        });
-        /******/
         var loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {
             /******/
             if (!scope || !__webpack_require__.o(scope, key)) return fallback();
             /******/
             return getSingletonVersion(scope, scopeName, key, version);
             /******/
         });
@@ -812,27 +790,27 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statusbar": () => (loadSingletonVersionCheck("default", "@jupyterlab/statusbar", [1, 3, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/statusbar": () => (loadSingletonVersionCheck("default", "@jupyterlab/statusbar", [1, 3, 4, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/mainmenu": () => (loadSingletonVersionCheck("default", "@jupyterlab/mainmenu", [1, 3, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/mainmenu": () => (loadSingletonVersionCheck("default", "@jupyterlab/mainmenu", [1, 3, 4, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/docmanager": () => (loadSingletonVersionCheck("default", "@jupyterlab/docmanager", [1, 3, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/docmanager": () => (loadSingletonVersionCheck("default", "@jupyterlab/docmanager", [1, 3, 4, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 4, 5])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 6, 4, 5])),
             /******/
             "webpack/sharing/consume/default/react": () => (loadSingletonVersionCheck("default", "react", [1, 17, 0, 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 5, 3])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 4, 5])),
             /******/
             "webpack/sharing/consume/default/@lumino/algorithm": () => (loadSingletonVersionCheck("default", "@lumino/algorithm", [1, 1, 9, 0])),
             /******/
             "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 33, 0]))
             /******/
         };
         /******/ // no consumes in initial chunks
@@ -901,15 +879,15 @@
                     /******/
                     try {
                         /******/
                         var promise = moduleToHandlerMapping[id]();
                         /******/
                         if (promise.then) {
                             /******/
-                            promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
+                            promises.push(installedModules[id] = promise.then(onFactory).catch(onError));
                             /******/
                         } else onFactory(promise);
                         /******/
                     } catch (e) {
                         onError(e);
                     }
                     /******/
@@ -1051,15 +1029,15 @@
                 /******/
                 if (__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {
                     /******/
                     installedChunks[chunkId][0]();
                     /******/
                 }
                 /******/
-                installedChunks[chunkId] = 0;
+                installedChunks[chunkIds[i]] = 0;
                 /******/
             }
             /******/
             /******/
         }
         /******/
         /******/
@@ -1067,29 +1045,20 @@
         /******/
         chunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));
         /******/
         chunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));
         /******/
     })();
     /******/
-    /******/
-    /* webpack/runtime/nonce */
-    /******/
-    (() => {
-        /******/
-        __webpack_require__.nc = undefined;
-        /******/
-    })();
-    /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/rsp-jupyter-extensions");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["rsp-jupyter-extensions"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.6537682ba05daa64613a.js.map
+//# sourceMappingURL=remoteEntry.cbd475d0b140d652d3db.js.map
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js.map` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8144841269841271%*

 * *Differences: {"'file'": "'remoteEntry.cbd475d0b140d652d3db.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.6537682ba05daa64613a.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCvLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.cbd475d0b140d652d3db.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC3KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://rsp-jupyter-extensions/webpack/container-entry",
         "webpack://rsp-jupyter-extensions/webpack/bootstrap",
         "webpack://rsp-jupyter-extensions/webpack/runtime/compat get default export",
         "webpack://rsp-jupyter-extensions/webpack/runtime/define property getters",
@@ -14,34 +14,32 @@
         "webpack://rsp-jupyter-extensions/webpack/runtime/hasOwnProperty shorthand",
         "webpack://rsp-jupyter-extensions/webpack/runtime/load script",
         "webpack://rsp-jupyter-extensions/webpack/runtime/make namespace object",
         "webpack://rsp-jupyter-extensions/webpack/runtime/sharing",
         "webpack://rsp-jupyter-extensions/webpack/runtime/publicPath",
         "webpack://rsp-jupyter-extensions/webpack/runtime/consumes",
         "webpack://rsp-jupyter-extensions/webpack/runtime/jsonp chunk loading",
-        "webpack://rsp-jupyter-extensions/webpack/runtime/nonce",
         "webpack://rsp-jupyter-extensions/webpack/before-startup",
         "webpack://rsp-jupyter-extensions/webpack/startup",
         "webpack://rsp-jupyter-extensions/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar oldScope = __webpack_require__.S[\"default\"];\n\tvar name = \"default\"\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"141932b86bb94d1168ff\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"16e7a87b76c7b094dea7\",\"style_index_js\":\"a3efb51ad79d669c319a\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"e0bf8ba868c627d5e57b\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"0c809f0d01c979a08eee\",\"style_index_js\":\"ace3aff4fb7c19d10cee\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"rsp-jupyter-extensions:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"rsp-jupyter-extensions:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\t;\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"rsp-jupyter-extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"rsp-jupyter-extensions\", \"0.7.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"rsp-jupyter-extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult.catch(handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"rsp-jupyter-extensions\", \"0.6.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statusbar\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/docmanager\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,5,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,5,3])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,5,3])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"rsp-jupyter-extensions\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkrsp_jupyter_extensions\"] = self[\"webpackChunkrsp_jupyter_extensions\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
-        "__webpack_require__.nc = undefined;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statusbar\", [1,3,4,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/mainmenu\", [1,3,4,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/docmanager\", [1,3,4,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,4,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,6,4,5])),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,4,5])),\n\t\"webpack/sharing/consume/default/@lumino/algorithm\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/algorithm\", [1,1,9,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,33,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statusbar\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/mainmenu\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/algorithm\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory).catch(onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"rsp-jupyter-extensions\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkIds[i]] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkrsp_jupyter_extensions\"] = self[\"webpackChunkrsp_jupyter_extensions\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/rsp-jupyter-extensions\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -99,8 +99,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=style_index_js.a3efb51ad79d669c319a.js.map
+//# sourceMappingURL=style_index_js.ace3aff4fb7c19d10cee.js.map
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js.map` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js.map`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'style_index_js.ace3aff4fb7c19d10cee.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "style_index_js.a3efb51ad79d669c319a.js",
+    "file": "style_index_js.ace3aff4fb7c19d10cee.js",
     "mappings": ";;;;;;;;;;;;;;;;;AAAA;AACsH;AAC7B;AACzF,8BAA8B,mFAA2B,CAAC,wGAAqC;AAC/F;AACA,iDAAiD,kEAAkE;AACnH;AACA,iEAAe,uBAAuB,EAAC;;;;;;;;;;;;;;;;;;ACPkD;AACzF,YAAsF;;AAEtF;;AAEA;AACA;;AAEA,aAAa,0GAAG,CAAC,qFAAO;;;;AAIxB,iEAAe,4FAAc,MAAM;;;;;;;;;;;;ACZf",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://rsp-jupyter-extensions/./style/base.css",
         "webpack://rsp-jupyter-extensions/./style/base.css?1944",
         "webpack://rsp-jupyter-extensions/./style/index.js"
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -451,8 +451,8 @@
                 };
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js.map
+//# sourceMappingURL=vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js.map
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js.map` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js",
+    "file": "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js",
     "mappings": ";;;;;;;;;AAAa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA,iBAAiB;;AAEjB;AACA;AACA;;AAEA;AACA,4CAA4C,qBAAqB;AACjE;;AAEA;AACA,KAAK;AACL,KAAK;AACL;;;AAGA;AACA;AACA;AACA;AACA;;AAEA;;AAEA;AACA,sBAAsB,iBAAiB;AACvC;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA,qBAAqB,qBAAqB;AAC1C;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;;;;;;;;;ACjEa;;AAEb,kCAAkC;;AAElC,8BAA8B;;AAE9B,kDAAkD,gBAAgB,gEAAgE,wDAAwD,6DAA6D,sDAAsD;;AAE7S,uCAAuC,uDAAuD,uCAAuC,SAAS,OAAO,oBAAoB;;AAEzK,yCAAyC,8FAA8F,wBAAwB,eAAe,eAAe,gBAAgB,YAAY,MAAM,wBAAwB,+BAA+B,aAAa,qBAAqB,uCAAuC,cAAc,WAAW,YAAY,UAAU,MAAM,mDAAmD,UAAU,sBAAsB;;AAEve,gCAAgC;;AAEhC;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA,uDAAuD,cAAc;AACrE;AACA;AACA;AACA,KAAK;AACL;AACA;;AAEA;AACA;;;;;;;;;;ACnCa;;AAEb;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;AACA;AACA;AACA;AACA,wDAAwD;;AAExD;AACA;AACA;AACA;AACA;AACA,UAAU;AACV;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA,CAAC;;AAED;;AAEA;AACA;;AAEA,kBAAkB,wBAAwB;AAC1C;AACA;AACA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA,kBAAkB,iBAAiB;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;AACA,OAAO;AACP;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA,gBAAgB,KAAwC,GAAG,sBAAiB,GAAG,CAAI;;AAEnF;AACA;AACA;AACA;;AAEA;AACA;AACA,GAAG;;AAEH;AACA;AACA,IAAI;AACJ;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;;;AAGA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC;;AAED;AACA,qEAAqE,qBAAqB,cAAc;;AAExG;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA,yDAAyD;AACzD,IAAI;;AAEJ;;;AAGA;AACA;AACA,IAAI;AACJ;AACA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA,MAAM;AACN;AACA;AACA;AACA;;AAEA;AACA,2BAA2B;AAC3B;;AAEA;AACA;AACA;;AAEA;AACA;AACA;AACA;;AAEA;AACA;AACA;;AAEA,oBAAoB,4BAA4B;AAChD;AACA;AACA;AACA;;AAEA;;AAEA,qBAAqB,6BAA6B;AAClD;;AAEA;;AAEA;AACA;;AAEA;AACA;AACA;;AAEA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://rsp-jupyter-extensions/./node_modules/css-loader/dist/runtime/api.js",
         "webpack://rsp-jupyter-extensions/./node_modules/css-loader/dist/runtime/cssWithMappingToString.js",
         "webpack://rsp-jupyter-extensions/./node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js"
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/query.py` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/query.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions/templates/portal_query.ipynb.template` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/portal_query.ipynb.template`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/PKG-INFO` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp-jupyter-extensions
-Version: 0.7.2
+Version: 0.8.0
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.7.2/rsp_jupyter_extensions.egg-info/SOURCES.txt` & `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,27 +19,26 @@
 rsp_jupyter_extensions.egg-info/SOURCES.txt
 rsp_jupyter_extensions.egg-info/dependency_links.txt
 rsp_jupyter_extensions.egg-info/not-zip-safe
 rsp_jupyter_extensions.egg-info/requires.txt
 rsp_jupyter_extensions.egg-info/top_level.txt
 rsp_jupyter_extensions/labextension/build_log.json
 rsp_jupyter_extensions/labextension/package.json
-rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js
-rsp_jupyter_extensions/labextension/static/lib_index_js.141932b86bb94d1168ff.js.map
-rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js
-rsp_jupyter_extensions/labextension/static/remoteEntry.6537682ba05daa64613a.js.map
+rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js
+rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js.map
+rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js
+rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js.map
 rsp_jupyter_extensions/labextension/static/style.js
-rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js
-rsp_jupyter_extensions/labextension/static/style_index_js.a3efb51ad79d669c319a.js.map
-rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js
-rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.16e7a87b76c7b094dea7.js.map
+rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js
+rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js.map
+rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js
+rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js.map
 rsp_jupyter_extensions/templates/portal_query.ipynb.template
 src/DisplayLabVersion.tsx
 src/displayversion.ts
 src/index.ts
 src/query.ts
 src/savequit.ts
 src/tokens.ts
 style/base.css
 style/index.css
-style/index.js
-tests/__init__.py
+style/index.js
```

### Comparing `rsp_jupyter_extensions-0.7.2/setup.py` & `rsp_jupyter_extensions-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/src/DisplayLabVersion.tsx` & `rsp_jupyter_extensions-0.8.0/src/DisplayLabVersion.tsx`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/src/displayversion.ts` & `rsp_jupyter_extensions-0.8.0/src/displayversion.ts`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 import { PageConfig } from '@jupyterlab/coreutils';
 
 interface IEnvResponse {
   IMAGE_DESCRIPTION?: string;
   IMAGE_DIGEST?: string;
   JUPYTER_IMAGE_SPEC?: string;
   EXTERNAL_INSTANCE_URL?: string;
+  CPU_LIMIT?: string;
+  MEM_LIMIT?: string;
+  CONTAINER_SIZE?: string;
 }
 
 import { ServerConnection } from '@jupyterlab/services';
 
 import { IStatusBar } from '@jupyterlab/statusbar';
 
 import DisplayLabVersion from './DisplayLabVersion';
@@ -42,14 +45,21 @@
 
   apiRequest(endpoint, init, settings).then(res => {
     const image_description = res.IMAGE_DESCRIPTION || '';
     const image_digest = res.IMAGE_DIGEST;
     const image_spec = res.JUPYTER_IMAGE_SPEC;
     const instance_url = new URL(res.EXTERNAL_INSTANCE_URL || '');
     const hostname = ' ' + instance_url.hostname;
+    const container_size = res.CONTAINER_SIZE || '';
+    let size = '';
+    if (container_size === '') {
+      size = ' (' + res.CPU_LIMIT + ' CPU, ' + res.MEM_LIMIT + ' B)';
+    } else {
+      size = ' ' + container_size;
+    }
     let digest_str = '';
     let imagename = '';
     if (image_spec) {
       /* First try to get digest out of image spec (nublado v3) */
       const imagearr = image_spec.split('/');
       const pullname = imagearr[imagearr.length - 1];
       const partsarr = pullname.split('@');
@@ -63,15 +73,15 @@
       }
       if (digest_str === '' && image_digest) {
         /* No digest in spec?  Well, did we set IMAGE_DIGEST?
            Yes, if we are nubladov2. */
         digest_str = ' [' + image_digest.substring(0, 8) + '...]';
       }
     }
-    const label = image_description + digest_str + imagename + hostname;
+    const label = image_description + digest_str + imagename + size + hostname;
 
     const displayVersionWidget = new DisplayLabVersion({
       source: label,
       title: image_description
     });
 
     statusBar.registerStatusItem(token.DISPLAYVERSION_ID, {
```

### Comparing `rsp_jupyter_extensions-0.7.2/src/index.ts` & `rsp_jupyter_extensions-0.8.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/src/query.ts` & `rsp_jupyter_extensions-0.8.0/src/query.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/src/savequit.ts` & `rsp_jupyter_extensions-0.8.0/src/savequit.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.7.2/tsconfig.json` & `rsp_jupyter_extensions-0.8.0/tsconfig.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98125%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018', 'skipLibCheck': True}"}*

```diff
@@ -11,16 +11,17 @@
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
+        "skipLibCheck": true,
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "es2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```


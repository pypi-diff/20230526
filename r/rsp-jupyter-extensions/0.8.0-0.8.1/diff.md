# Comparing `tmp/rsp_jupyter_extensions-0.8.0.tar.gz` & `tmp/rsp_jupyter_extensions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsp_jupyter_extensions-0.8.0.tar", last modified: Fri May 26 19:20:13 2023, max compression
+gzip compressed data, was "rsp_jupyter_extensions-0.8.1.tar", last modified: Fri May 26 21:50:27 2023, max compression
```

## Comparing `rsp_jupyter_extensions-0.8.0.tar` & `rsp_jupyter_extensions-0.8.1.tar`

### file list

```diff
@@ -1,57 +1,53 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.863293 rsp_jupyter_extensions-0.8.0/
--rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 19:20:13.862969 rsp_jupyter_extensions-0.8.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/README.md
--rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/RELEASE.md
--rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/install.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.841004 rsp_jupyter_extensions-0.8.0/jupyter-config/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.845935 rsp_jupyter_extensions-0.8.0/jupyter-config/nb-config/
--rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/jupyter-config/nb-config/rsp_jupyter_extensions.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.846303 rsp_jupyter_extensions-0.8.0/jupyter-config/server-config/
--rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/jupyter-config/server-config/rsp_jupyter_extensions.json
--rw-r--r--   0 adam       (501) staff       (20)     3069 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/package.json
--rw-r--r--   0 adam       (501) staff       (20)      954 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.849697 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/
--rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/environment.py
--rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/execution.py
--rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/handlers.py
--rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/hub.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.853092 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/
--rw-r--r--   0 adam       (501) staff       (20)    20795 2022-09-02 20:40:09.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/build_log.json
--rw-r--r--   0 adam       (501) staff       (20)     3207 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/package.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.858006 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/
--rw-r--r--   0 adam       (501) staff       (20)    27460 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js
--rw-r--r--   0 adam       (501) staff       (20)    19521 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/lib_index_js.e0bf8ba868c627d5e57b.js.map
--rw-r--r--   0 adam       (501) staff       (20)    28481 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js
--rw-r--r--   0 adam       (501) staff       (20)    27434 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/remoteEntry.cbd475d0b140d652d3db.js.map
--rw-r--r--   0 adam       (501) staff       (20)      165 2022-09-02 20:40:09.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style.js
--rw-r--r--   0 adam       (501) staff       (20)     4268 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js
--rw-r--r--   0 adam       (501) staff       (20)     1438 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/style_index_js.ace3aff4fb7c19d10cee.js.map
--rw-r--r--   0 adam       (501) staff       (20)    12074 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js
--rw-r--r--   0 adam       (501) staff       (20)    13814 2022-09-02 20:40:10.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c809f0d01c979a08eee.js.map
--rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/query.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.858470 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/
--rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/portal_query.ipynb.template
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.852116 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1891 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 19:20:13.000000 rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 19:20:13.863364 rsp_jupyter_extensions-0.8.0/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.861408 rsp_jupyter_extensions-0.8.0/src/
--rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/DisplayLabVersion.tsx
--rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/src/displayversion.ts
--rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/index.ts
--rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/query.ts
--rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/savequit.ts
--rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.0/src/tokens.ts
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 19:20:13.862545 rsp_jupyter_extensions-0.8.0/style/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/base.css
--rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/index.css
--rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.0/style/index.js
--rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.0/tsconfig.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.580650 rsp_jupyter_extensions-0.8.1/
+-rw-r--r--   0 adam       (501) staff       (20)     1068 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      480 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 21:50:27.579962 rsp_jupyter_extensions-0.8.1/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3072 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     1146 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/RELEASE.md
+-rw-r--r--   0 adam       (501) staff       (20)      205 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/install.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.546509 rsp_jupyter_extensions-0.8.1/jupyter-config/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.556019 rsp_jupyter_extensions-0.8.1/jupyter-config/nb-config/
+-rw-r--r--   0 adam       (501) staff       (20)       99 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/jupyter-config/nb-config/rsp_jupyter_extensions.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.556699 rsp_jupyter_extensions-0.8.1/jupyter-config/server-config/
+-rw-r--r--   0 adam       (501) staff       (20)       97 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/jupyter-config/server-config/rsp_jupyter_extensions.json
+-rw-r--r--   0 adam       (501) staff       (20)     3052 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.1/package.json
+-rw-r--r--   0 adam       (501) staff       (20)      915 2023-05-26 21:43:44.000000 rsp_jupyter_extensions-0.8.1/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.561416 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/
+-rw-r--r--   0 adam       (501) staff       (20)      699 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     2218 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/environment.py
+-rw-r--r--   0 adam       (501) staff       (20)     2311 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/execution.py
+-rw-r--r--   0 adam       (501) staff       (20)      916 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/handlers.py
+-rw-r--r--   0 adam       (501) staff       (20)     1573 2021-09-15 20:02:14.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/hub.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.566196 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/
+-rw-r--r--   0 adam       (501) staff       (20)     3194 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/package.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.570609 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/
+-rw-r--r--   0 adam       (501) staff       (20)     6154 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/360.fc403a4ceb567571372e.js
+-rw-r--r--   0 adam       (501) staff       (20)     3377 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/747.b57adabf32495ac79fb2.js
+-rw-r--r--   0 adam       (501) staff       (20)     6866 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/remoteEntry.ba7b3ca42c9aa9705c93.js
+-rw-r--r--   0 adam       (501) staff       (20)      165 2023-05-26 21:35:51.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/style.js
+-rw-r--r--   0 adam       (501) staff       (20)     2452 2023-05-26 21:35:52.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/static/third-party-licenses.json
+-rw-r--r--   0 adam       (501) staff       (20)     3298 2022-09-06 19:43:05.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/query.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.571323 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/
+-rw-r--r--   0 adam       (501) staff       (20)     2735 2022-09-16 20:51:36.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/portal_query.ipynb.template
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.565625 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3949 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1306 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-09-22 18:31:11.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       41 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       23 2023-05-26 21:50:27.000000 rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-05-26 21:50:27.580813 rsp_jupyter_extensions-0.8.1/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     3120 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.576768 rsp_jupyter_extensions-0.8.1/src/
+-rw-r--r--   0 adam       (501) staff       (20)     1577 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/DisplayLabVersion.tsx
+-rw-r--r--   0 adam       (501) staff       (20)     4015 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.1/src/displayversion.ts
+-rw-r--r--   0 adam       (501) staff       (20)     1420 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/index.ts
+-rw-r--r--   0 adam       (501) staff       (20)     5503 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/query.ts
+-rw-r--r--   0 adam       (501) staff       (20)     4737 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/savequit.ts
+-rw-r--r--   0 adam       (501) staff       (20)      304 2023-05-26 18:02:57.000000 rsp_jupyter_extensions-0.8.1/src/tokens.ts
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-05-26 21:50:27.578913 rsp_jupyter_extensions-0.8.1/style/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/base.css
+-rw-r--r--   0 adam       (501) staff       (20)       25 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/index.css
+-rw-r--r--   0 adam       (501) staff       (20)       21 2021-09-11 03:04:41.000000 rsp_jupyter_extensions-0.8.1/style/index.js
+-rw-r--r--   0 adam       (501) staff       (20)      580 2023-05-26 19:05:55.000000 rsp_jupyter_extensions-0.8.1/tsconfig.json
+-rw-r--r--   0 adam       (501) staff       (20)   203643 2023-05-26 21:35:08.000000 rsp_jupyter_extensions-0.8.1/yarn.lock
```

### Comparing `rsp_jupyter_extensions-0.8.0/LICENSE` & `rsp_jupyter_extensions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/PKG-INFO` & `rsp_jupyter_extensions-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp_jupyter_extensions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.0/README.md` & `rsp_jupyter_extensions-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/RELEASE.md` & `rsp_jupyter_extensions-0.8.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/package.json` & `rsp_jupyter_extensions-0.8.1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9711399711399712%*

 * *Differences: {"'devDependencies'": "{'rimraf': '^5.0.1'}",*

 * * "'jupyter-releaser'": '{\'hooks\': {\'before-build-npm\': {insert: [(0, "python -m pip install '*

 * *                       '\'jupyterlab<4\'")], delete: [0]}}}',*

 * * "'version'": "'0.8.1'"}*

```diff
@@ -28,26 +28,26 @@
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
+        "rimraf": "^5.0.1",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/lsst-sqre/rsp-jupyter-extensions",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
-                "python -m pip install jupyterlab~=3.3",
+                "python -m pip install 'jupyterlab<4'",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "disabledExtensions": [
             "@jupyterlab/statusbar-extension:mode-switch"
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.8.1"
 }
```

### Comparing `rsp_jupyter_extensions-0.8.0/pyproject.toml` & `rsp_jupyter_extensions-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 [build-system]
 requires = ["jupyter_packaging",
-	 "jupyterlab~=3.6.3",
-	 "isort",
-	 "poetry",
-	 "black",
+	 "jupyterlab<4",
 	 "pre-commit"
 ]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["rsp_jupyter_extensions/labextension/static/style.js"]
 ensured-targets = ["rsp_jupyter_extensions/labextension/static/style.js", "rsp_jupyter_extensions/labextension/package.json"]
```

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/__init__.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/environment.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/environment.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/execution.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/execution.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/handlers.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/handlers.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/hub.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/hub.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/labextension/package.json` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/labextension/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671717171717172%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3', '@jupyterlab/coreutils': '^5', "*

 * *                   "'@jupyterlab/services': '^6'}",*

 * * "'devDependencies'": "{'rimraf': '^5.0.1'}",*

 * * "'jupyter-releaser'": '{\'hooks\': {\'before-build-npm\': {insert: [(0, "python -m pip install '*

 * *                       '\'jupyterlab<4\'")], delete: [0]}}}',*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ba7b3ca42c9aa9705c93.js'}}",*

 * * "'version'": "'0.8.1'"}*

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
@@ -28,34 +28,34 @@
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
+        "rimraf": "^5.0.1",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/lsst-sqre/rsp-jupyter-extensions",
     "jupyter-releaser": {
         "hooks": {
             "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
+                "python -m pip install 'jupyterlab<4'",
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cbd475d0b140d652d3db.js",
+            "load": "static/remoteEntry.ba7b3ca42c9aa9705c93.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/statusbar-extension:mode-switch"
         ],
         "discovery": {
             "server": {
@@ -102,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.0"
+    "version": "0.8.1"
 }
```

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/query.py` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/query.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions/templates/portal_query.ipynb.template` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions/templates/portal_query.ipynb.template`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/rsp_jupyter_extensions.egg-info/PKG-INFO` & `rsp_jupyter_extensions-0.8.1/rsp_jupyter_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsp-jupyter-extensions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Jupyter Extensions for the RSP
 Home-page: https://github.com/lsst-sqre/rsp-jupyter-extensions
 Author: Adam Thornton
 Author-email: athornton@lsst.org
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `rsp_jupyter_extensions-0.8.0/setup.py` & `rsp_jupyter_extensions-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/src/DisplayLabVersion.tsx` & `rsp_jupyter_extensions-0.8.1/src/DisplayLabVersion.tsx`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/src/displayversion.ts` & `rsp_jupyter_extensions-0.8.1/src/displayversion.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/src/index.ts` & `rsp_jupyter_extensions-0.8.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/src/query.ts` & `rsp_jupyter_extensions-0.8.1/src/query.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/src/savequit.ts` & `rsp_jupyter_extensions-0.8.1/src/savequit.ts`

 * *Files identical despite different names*

### Comparing `rsp_jupyter_extensions-0.8.0/tsconfig.json` & `rsp_jupyter_extensions-0.8.1/tsconfig.json`

 * *Files identical despite different names*


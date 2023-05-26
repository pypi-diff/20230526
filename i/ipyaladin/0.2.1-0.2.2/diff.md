# Comparing `tmp/ipyaladin-0.2.1.tar.gz` & `tmp/ipyaladin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyaladin-0.2.1.tar", last modified: Mon Dec  5 18:23:52 2022, max compression
+gzip compressed data, was "ipyaladin-0.2.2.tar", last modified: Fri May 26 13:45:09 2023, max compression
```

## Comparing `ipyaladin-0.2.1.tar` & `ipyaladin-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.603166 ipyaladin-0.2.1/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1552 2022-11-08 09:24:52.000000 ipyaladin-0.2.1/LICENSE.md
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      398 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/MANIFEST.in
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     3553 2022-12-05 18:23:52.603247 ipyaladin-0.2.1/PKG-INFO
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1956 2022-12-05 16:54:04.000000 ipyaladin-0.2.1/README.md
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      178 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/install.json
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.597445 ipyaladin-0.2.1/ipyaladin/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1670 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/ipyaladin/__init__.py
--rw-r--r--   0 matthieubaumann   (502) staff       (20)       67 2022-12-05 16:54:33.000000 ipyaladin-0.2.1/ipyaladin/_version.py
--rw-r--r--   0 matthieubaumann   (502) staff       (20)    10852 2022-12-05 15:50:55.000000 ipyaladin-0.2.1/ipyaladin/aladin_widget.py
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.598855 ipyaladin-0.2.1/ipyaladin/labextension/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1611 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/package.json
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.600524 ipyaladin-0.2.1/ipyaladin/labextension/static/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     4882 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/261.bfcaf0ae589773f941db.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     4566 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/678.54afe962dae4bf9693fa.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)    22079 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/794.6f96ca96639b4fa21dce.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     6811 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/remoteEntry.f2d6e628bd28c3f3b3b7.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      118 2022-12-05 16:56:54.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/style.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1311 2022-12-05 16:56:55.000000 ipyaladin-0.2.1/ipyaladin/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.601058 ipyaladin-0.2.1/ipyaladin/nbextension/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      527 2022-12-05 16:56:52.000000 ipyaladin-0.2.1/ipyaladin/nbextension/extension.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)    27293 2022-12-05 16:56:53.000000 ipyaladin-0.2.1/ipyaladin/nbextension/index.js
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.598644 ipyaladin-0.2.1/ipyaladin.egg-info/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     3553 2022-12-05 18:23:52.000000 ipyaladin-0.2.1/ipyaladin.egg-info/PKG-INFO
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      989 2022-12-05 18:23:52.000000 ipyaladin-0.2.1/ipyaladin.egg-info/SOURCES.txt
--rw-r--r--   0 matthieubaumann   (502) staff       (20)        1 2022-12-05 18:23:52.000000 ipyaladin-0.2.1/ipyaladin.egg-info/dependency_links.txt
--rw-r--r--   0 matthieubaumann   (502) staff       (20)        1 2022-12-01 09:51:10.000000 ipyaladin-0.2.1/ipyaladin.egg-info/not-zip-safe
--rw-r--r--   0 matthieubaumann   (502) staff       (20)       21 2022-12-05 18:23:52.000000 ipyaladin-0.2.1/ipyaladin.egg-info/requires.txt
--rw-r--r--   0 matthieubaumann   (502) staff       (20)       10 2022-12-05 18:23:52.000000 ipyaladin-0.2.1/ipyaladin.egg-info/top_level.txt
--rw-r--r--   0 matthieubaumann   (502) staff       (20)       63 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/ipyaladin.json
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.602152 ipyaladin-0.2.1/js/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      134 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/README.md
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      647 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/amd-public-path.js
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.602316 ipyaladin-0.2.1/js/dist/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)    27293 2022-12-05 16:56:53.000000 ipyaladin-0.2.1/js/dist/index.js
-drwxr-xr-x   0 matthieubaumann   (502) staff       (20)        0 2022-12-05 18:23:52.603052 ipyaladin-0.2.1/js/lib/
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      455 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/lib/extension.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      171 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/lib/index.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)    11298 2022-12-05 16:56:41.000000 ipyaladin-0.2.1/js/lib/jupyter-aladin.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      465 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/lib/labplugin.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)   361285 2022-12-05 16:56:50.000000 ipyaladin-0.2.1/js/package-lock.json
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1495 2022-12-05 16:54:46.000000 ipyaladin-0.2.1/js/package.json
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     2822 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/js/webpack.config.js
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      144 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/pyproject.toml
--rw-r--r--   0 matthieubaumann   (502) staff       (20)     1599 2022-12-05 18:23:52.603636 ipyaladin-0.2.1/setup.cfg
--rw-r--r--   0 matthieubaumann   (502) staff       (20)      909 2022-12-05 10:06:41.000000 ipyaladin-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/aladin_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/590.9292295778c3653a0b31.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 13:45:06.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 13:44:51.000000 ipyaladin-0.2.2/ipyaladin/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-26 13:44:54.000000 ipyaladin-0.2.2/ipyaladin/nbextension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:44:38.000000 ipyaladin-0.2.2/ipyaladin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/amd-public-path.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-26 13:44:53.000000 ipyaladin-0.2.2/js/dist/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/jupyter-aladin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/labplugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82531 2023-05-26 13:44:49.000000 ipyaladin-0.2.2/js/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/setup.py
```

### Comparing `ipyaladin-0.2.1/LICENSE.md` & `ipyaladin-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/PKG-INFO` & `ipyaladin-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.1
+Version: 0.2.2
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -30,67 +30,79 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ipyaladin
 
-## Description
-
 A bridge between Jupyter and Aladin Lite, enabling interactive sky visualization in IPython notebooks.
-
-![ipyaladin example](ipyaladin-screenshot.png)
-
 With a couple of lines, you can display Aladin Lite, center it on the target of your choice, and overlay an Astropy table:
 
-![ipyaladin example](ipyaladin-screencast.gif)
+![ipyaladin example](assets/ipyaladin-screencast.gif)
+
+- [ipyaladin](#ipyaladin)
+  - [Examples](#examples)
+  - [Installation](#installation)
+  - [New features corner](#new-features-corner)
+  - [Development installation](#development-installation)
 
 ## Examples
 
 Some example notebooks can be found in the [examples directory](examples).
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master). You can also try it directly [in mybinder](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master), without installing anything.
 
 ## Installation
 
 To install use pip:
 
-    $ pip install ipyaladin
+    pip install ipyaladin
 
 Then, make sure to enable widgetsnbextension:
 
-    $ jupyter nbextension enable --py widgetsnbextension
+    jupyter nbextension enable --py widgetsnbextension
 
 Finally, enable ipyaladin:
 
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
-    $ jupyter labextension develop ipyaladin --overwrite
+    jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    $  conda install -c bmatthieu3 ipyaladin==0.2.1
+    conda install -c bmatthieu3 ipyaladin==0.2.2
+
+## New features corner
+
+![new_features](assets/new_features.gif)
+
+## Development installation
 
-## Development
+First, make sure you have installed jupyter on your python environnement: `pip install jupyter`.
+For a development installation [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/) are also required,
 
-For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
+    git clone https://github.com/cds-astro/ipyaladin.git
+    cd ipyaladin
+    npm install yarn
+    cd js
+    npm install
+    cd ..
+    pip install -e .
 
-    $ git clone https://github.com/cds-astro/ipyaladin.git
-    $ cd ipyaladin
-    $ npm install yarn
-    $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+For Jupyter Notebook, do
+ 
+    jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
-When actively developing your extension for JupyterLab, you will need to run this command too:
+For JupyterLab, you will need to run this command too:
 
-    $ jupyter labextension develop --overwrite ipyaladin
+    jupyter labextension develop --overwrite ipyaladin
 
 Then you need to rebuild the JS when you make a code change:
 
-    $ cd js
-    $ yarn run build
+    cd js
+    yarn run build
 
 You then need to refresh the JupyterLab page when your javascript changes.
```

### Comparing `ipyaladin-0.2.1/README.md` & `ipyaladin-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 # ipyaladin
 
-## Description
-
 A bridge between Jupyter and Aladin Lite, enabling interactive sky visualization in IPython notebooks.
-
-![ipyaladin example](ipyaladin-screenshot.png)
-
 With a couple of lines, you can display Aladin Lite, center it on the target of your choice, and overlay an Astropy table:
 
-![ipyaladin example](ipyaladin-screencast.gif)
+![ipyaladin example](assets/ipyaladin-screencast.gif)
+
+- [ipyaladin](#ipyaladin)
+  - [Examples](#examples)
+  - [Installation](#installation)
+  - [New features corner](#new-features-corner)
+  - [Development installation](#development-installation)
 
 ## Examples
 
 Some example notebooks can be found in the [examples directory](examples).
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master). You can also try it directly [in mybinder](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master), without installing anything.
 
 ## Installation
 
 To install use pip:
 
-    $ pip install ipyaladin
+    pip install ipyaladin
 
 Then, make sure to enable widgetsnbextension:
 
-    $ jupyter nbextension enable --py widgetsnbextension
+    jupyter nbextension enable --py widgetsnbextension
 
 Finally, enable ipyaladin:
 
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
-    $ jupyter labextension develop ipyaladin --overwrite
+    jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    $  conda install -c bmatthieu3 ipyaladin==0.2.1
+    conda install -c bmatthieu3 ipyaladin==0.2.2
+
+## New features corner
+
+![new_features](assets/new_features.gif)
+
+## Development installation
 
-## Development
+First, make sure you have installed jupyter on your python environnement: `pip install jupyter`.
+For a development installation [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/) are also required,
 
-For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
+    git clone https://github.com/cds-astro/ipyaladin.git
+    cd ipyaladin
+    npm install yarn
+    cd js
+    npm install
+    cd ..
+    pip install -e .
 
-    $ git clone https://github.com/cds-astro/ipyaladin.git
-    $ cd ipyaladin
-    $ npm install yarn
-    $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+For Jupyter Notebook, do
+ 
+    jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
-When actively developing your extension for JupyterLab, you will need to run this command too:
+For JupyterLab, you will need to run this command too:
 
-    $ jupyter labextension develop --overwrite ipyaladin
+    jupyter labextension develop --overwrite ipyaladin
 
 Then you need to rebuild the JS when you make a code change:
 
-    $ cd js
-    $ yarn run build
+    cd js
+    yarn run build
 
 You then need to refresh the JupyterLab page when your javascript changes.
```

### Comparing `ipyaladin-0.2.1/ipyaladin/__init__.py` & `ipyaladin-0.2.2/ipyaladin/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/ipyaladin/aladin_widget.py` & `ipyaladin-0.2.2/ipyaladin/aladin_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,67 @@
 import ipywidgets as widgets
 from traitlets import (Float, Unicode, Bool, List, Dict, default)
 from ._version import NPM_PACKAGE_RANGE
+import math
 
 # See js/lib/example.js for the frontend counterpart to this file.
 
 @widgets.register
 class Aladin(widgets.DOMWidget):
-    """An example widget."""
+    """An instance of the Aladin widget.
+    
+    Adaptative attributes can be updated later. The other ones can only
+    be written when creating the widget instance, i.e. when calling Aladin() 
+
+    ...
+    Attributes
+    ----------
+
+    fov : float, default: 60
+        The desired initial field of view, expressed in degrees.
+        adaptative
+    target : string, default: "0 +0"
+        The desired target. 
+        adaptative
+    coo_frame : string, default: "J2000"
+        Reference frame.
+        adaptative
+    survey : string, default: "P/DSS2/color"
+        Name of the survey.
+        adaptative
+    ...
+    height : float, default: 400
+        Height of the Aladin widget in pixels
+    reticle_size : float, default: 22
+        Size of the reticle.
+    reticle_color : string, default: "rgb(178, 50, 178)"
+        The color of the reticle.
+    show_reticle : bool, default: True
+        Controls wether a reticle is present in the middle of the view
+    show_zoom_control : bool, default: True
+    show_fullscreen_control = bool, default: False
+        Wether the fullscreen button appears in the top right corner
+        Defaults to False because this does not work in retrolab. 
+        Can safely be turned to True in Jupyterlab.
+    show_layers_control : bool, default: True
+    show_goto_control, bool, default: True
+    show_simbad_pointer_control : bool, default: True
+        Controls the quick search tool apparition on the left 
+        side of the view.
+    show_share_control : bool, default: False
+        Controls the apparition of the share button in the bottom
+        right corner. This button opens a popup with a sharable link
+        to an Aladin previewer that starts with the actual state of the
+        view.
+    show_context_menu : bool, default: True
+        Controls wether a right click will open a menu. This menu is documented
+        here # TODO add link to documentation when it will exist. 
+        
+    TODO: finish docstring
+    """
 
     # Name of the widget view class in front-end
     _view_name = Unicode('AladinView').tag(sync=True)
 
     # Name of the widget model class in front-end
     _model_name = Unicode('AladinModel').tag(sync=True)
 
@@ -41,24 +92,29 @@
     reticle_size = Float(22).tag(sync=True, o=True)
     reticle_color = Unicode("rgb(178, 50, 178)").tag(sync=True, o=True)
     show_reticle = Bool(True).tag(sync=True, o=True)
     show_zoom_control = Bool(True).tag(sync=True, o=True)
     show_fullscreen_control = Bool(False).tag(sync=True, o=True)
     show_layers_control = Bool(True).tag(sync=True, o=True)
     show_goto_control = Bool(True).tag(sync=True, o=True)
+    show_simbad_pointer_control = Bool(True).tag(sync=True, o=True)
     show_share_control = Bool(False).tag(sync=True, o=True)
+    show_context_menu = Bool(True).tag(sync=True, o=True)
     show_catalog = Bool(True).tag(sync=True, o=True)
     show_frame = Bool(True).tag(sync=True, o=True)
     show_coo_grid = Bool(False).tag(sync=True, o=True)
     full_screen = Bool(False).tag(sync=True, o=True)
     log = Bool(True).tag(sync=True, o=True)
     allow_full_zoomout = Bool(False).tag(sync=True, o=True)
 
     options = List(trait=Unicode).tag(sync=True)
 
+    # this sets the height of the widget
+    height = Float(400).tag(sync=True)
+
     # the following values are used in the classe's functions
 
     # values used in the add_catalog_from_URL function
     votable_URL = Unicode('').tag(sync=True)
     votable_options = Dict().tag(sync=True)
     votable_from_URL_flag = Bool(True).tag(sync=True)
 
@@ -155,19 +211,43 @@
     # Notes:
     # 1 - The loaded table can possess fields tagged as 'masked', who can not be parsed by JSON
     #     As such, the table's columns cant be obtained through the use of table.columns,
     #     and the use of table.__array__() is requiered.
     # 2 - It seems that the list.append() method does not work with traitlets,
     #     the affectation of the columns must be done at once by using a buffer.
     def add_table(self, table):
-        """ load a VOTable -already accessible on the python side- into the widget
-            Args:
-                table: votable object"""
+        """ Load a table into the widget.
+
+        Parameters
+        ----------
+        table : astropy.table.table.QTable or astropy.table.table.Table
+                table that must contain coordinates information
+        
+        Examples
+        --------
+        Cell 1:
+        >>> from ipyaladin import Aladin
+        >>> from astropy.table import QTable
+        >>> aladin = Aladin(fov=2, target='M1')
+        >>> aladin
+        Cell 2:
+        >>> ra = [83.63451584700, 83.61368056017, 83.58780251600]
+        >>> dec = [22.05652591227, 21.97517807639, 21.99277764451]
+        >>> name = ["Gaia EDR3 3403818589184411648",
+                    "Gaia EDR3 3403817661471500416",
+                    "Gaia EDR3 3403817936349408000",
+                   ]
+        >>> table = QTable([ra, dec, name],
+                            names=("ra", "dec", "name"),
+                            meta={"name": "my sample table"})
+        >>> aladin.add_table(table)
+        And the table should appear in the output of Cell 1!
+        """
 
-        # theses library must be installed, and are used in votable operations
+        # this library must be installed, and is used in votable operations
         # http://www.astropy.org/
         import astropy
         
         table_array = table.__array__()
         self.table_keys= table.keys()
         table_columns= []
         for i in range(0,len(table.columns[0])):
@@ -175,15 +255,21 @@
 
             # this step is needed in order to properly retrieve strings data
             # (otherwise, Aladin Lite shows these values as DataView object)
             for item in table_array[i]:
                 if isinstance(item, bytes):
                     row_data.append(item.decode('utf-8'))
                 else:
+                    if not isinstance(item, str):
+                        # replace NaN by " ", this is a quick fix 
+                        # and should be questioned when doing a rework
+                        # of this function
+                        item = " " if math.isnan(item) else item 
                     row_data.append(item)
+                    
             table_columns.append(row_data)
 
         self.table_columns = table_columns
         self.table_flag= not self.table_flag
 
     def add_overlay_from_stcs(self, stc_string, overlay_options={}):
         """ Add an overlay layer defined by a STC-S string
```

### Comparing `ipyaladin-0.2.1/ipyaladin/labextension/package.json` & `ipyaladin-0.2.2/ipyaladin/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8322172619047619%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.0.0 || ^4.0.0'}",*

 * * "'files'": '{delete: [0]}',*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c35d9bcfb9f9c1b91ff1.js'}}",*

 * * "'main'": "'dist/index.js'",*

 * * "'module'": "'dist/index.js'",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -2,26 +2,25 @@
     "author": "Thomas Boch, Jerome Desroziers and Matthieu Baumann",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6",
         "underscore": "^1.13.6"
     },
     "description": "ipyaladin",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^3.0.0 || ^4.0.0",
         "rimraf": "^2.6.1",
         "webpack": "^5"
     },
     "files": [
-        "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f2d6e628bd28c3f3b3b7.js"
+            "load": "static/remoteEntry.c35d9bcfb9f9c1b91ff1.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../ipyaladin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -32,15 +31,16 @@
         "jupyter",
         "widgets",
         "ipython",
         "ipywidgets",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
-    "main": "lib/index.js",
+    "main": "dist/index.js",
+    "module": "dist/index.js",
     "name": "ipyaladin",
     "repository": {
         "type": "git",
         "url": "https://github.com/cds-astro/ipyaladin.git"
     },
     "scripts": {
         "build": "webpack --mode=development && yarn run build:labextension:dev",
@@ -48,9 +48,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../ipyaladin/labextension/ && rimraf ../ipyaladin/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `ipyaladin-0.2.1/ipyaladin/labextension/static/261.bfcaf0ae589773f941db.js` & `ipyaladin-0.2.2/ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,178 +1,170 @@
 "use strict";
 (self.webpackChunkipyaladin = self.webpackChunkipyaladin || []).push([
-    [261, 678], {
-        678: (e, t, a) => {
-            a.r(t), a.d(t, {
-                AladinModel: () => l,
-                AladinView: () => d,
-                version: () => r.i8
+    [563], {
+        563: (t, e, s) => {
+            s.r(e), s.d(e, {
+                aladinWidgetPlugin: () => n,
+                default: () => r
             });
-            var i = a(672);
-            a(297);
-            const o = (e, t = !0, a = "text/javascript") => new Promise(((i, o) => {
+            var i = s(672);
+            s(297);
+            const a = (t, e = !0, s = "text/javascript") => new Promise(((i, a) => {
                 try {
-                    const s = document.createElement("script");
-                    s.type = a, s.async = t, s.src = e, s.addEventListener("load", (e => {
+                    const l = document.createElement("script");
+                    l.type = s, l.async = e, l.src = t, l.addEventListener("load", (t => {
                         i({
                             status: !0
                         })
-                    })), s.addEventListener("error", (e => {
-                        o({
+                    })), l.addEventListener("error", (t => {
+                        a({
                             status: !1,
                             message: "Failed to load the script ＄{FILE_URL}"
                         })
-                    })), document.getElementsByTagName("head")[0].appendChild(s)
-                } catch (e) {
-                    o(e)
+                    })), document.getElementsByTagName("head")[0].appendChild(l)
+                } catch (t) {
+                    a(t)
                 }
             }));
-            var s = o("https://code.jquery.com/jquery-3.6.1.min.js").then((() => o("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
+            let l = a("https://code.jquery.com/jquery-3.6.1.min.js").then((() => a("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
                 await A.init
             }));
-            class l extends i.DOMWidgetModel {
+            class o extends i.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "AladinModel",
                         _view_name: "AladinView",
                         _model_module: "ipyaladin",
                         _view_module: "ipyaladin",
-                        _model_module_version: "0.2.1",
-                        _view_module_version: "0.2.1"
+                        _model_module_version: "0.2.2",
+                        _view_module_version: "0.2.2"
                     }
                 }
             }
-            var n = 0;
+            let h = 0;
             class d extends i.DOMWidgetView {
                 render() {
-                    s.then((() => {
-                        this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(n), n += 1, this.div.setAttribute("style", "width:100%;height:400px;");
-                        for (var e = {}, t = this.model.get("options"), a = 0; a < t.length; a++) e[this.convert_pyname_to_jsname(t[a])] = this.model.get(t[a]);
+                    l.then((() => {
+                        this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(h), h += 1;
+                        let t = this.model.get("height");
+                        this.div.setAttribute("style", "width:100%;height:" + t + "px;");
+                        let e = {},
+                            s = this.model.get("options");
+                        for (let t of s) e[this.convert_pyname_to_jsname(t)] = this.model.get(t);
                         new MutationObserver((t => {
                             t.forEach((t => {
                                 t.addedNodes.forEach((t => {
                                     t.id == this.div.id && setTimeout((() => {
                                         this.al = A.aladin([this.div], e), this.aladin_events(), this.model_events()
                                     }), 1e3)
                                 }))
                             }))
                         })).observe(this.el, {
                             subtree: !1,
                             childList: !0
                         }), this.el.appendChild(this.div)
                     }))
                 }
-                convert_pyname_to_jsname(e) {
-                    var t, a = e.split("_");
-                    for (t = 1; t < a.length; t++) a[t] = a[t].charAt(0).toUpperCase() + a[t].slice(1);
-                    return a.join("")
+                convert_pyname_to_jsname(t) {
+                    let e = t.split("_");
+                    for (let t = 1; t < e.length; t++) e[t] = e[t].charAt(0).toUpperCase() + e[t].slice(1);
+                    return e.join("")
                 }
                 aladin_events() {
-                    var e = this;
-                    this.al.on("zoomChanged", (function(t) {
-                        e.fov_py ? e.fov_py = !1 : (e.fov_js = !0, e.model.set("fov", parseFloat(t.toFixed(5))), e.touch())
-                    })), this.al.on("positionChanged", (function(t) {
-                        e.target_py ? e.target_py = !1 : (e.target_js = !0, e.model.set("target", t.ra.toFixed(6) + " " + t.dec.toFixed(6)), e.touch())
+                    this.al.on("zoomChanged", (t => {
+                        this.fov_py ? this.fov_py = !1 : (this.fov_js = !0, this.model.set("fov", parseFloat(t.toFixed(5))), this.touch())
+                    })), this.al.on("positionChanged", (t => {
+                        this.target_py ? this.target_py = !1 : (this.target_js = !0, this.model.set("target", t.ra.toFixed(6) + " " + t.dec.toFixed(6)), this.touch())
                     }))
                 }
                 model_events() {
-                    var e = this;
-                    this.listenTo(this.model, "change:fov", (function() {
-                        e.fov_js ? e.fov_js = !1 : (e.fov_py = !0, e.al.setFoV(e.model.get("fov")))
-                    }), this), this.listenTo(this.model, "change:target", (function() {
-                        e.target_js ? e.target_js = !1 : (e.target_py = !0, e.al.gotoObject(e.model.get("target")))
-                    }), this), this.listenTo(this.model, "change:coo_frame", (function() {
-                        e.al.setFrame(e.model.get("coo_frame"))
-                    }), this), this.listenTo(this.model, "change:survey", (function() {
-                        e.al.setImageSurvey(e.model.get("survey"))
-                    }), this), this.listenTo(this.model, "change:overlay_survey", (function() {
-                        e.al.setOverlayImageLayer(e.model.get("overlay_survey"))
-                    }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (function() {
-                        e.al.getOverlayImageLayer().setAlpha(e.model.get("overlay_survey_opacity"))
-                    }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (function() {
-                        e.al.addCatalog(A.catalogFromURL(e.model.get("votable_URL"), e.model.get("votable_options")))
-                    }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (function() {
-                        e.al.addMOC(A.MOCFromURL(e.model.get("moc_URL"), e.model.get("moc_options")))
-                    }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (function() {
-                        e.al.addMOC(A.MOCFromJSON(e.model.get("moc_dict"), e.model.get("moc_options")))
-                    }), this), this.listenTo(this.model, "change:table_flag", (function() {
-                        var t = A.catalog({
+                    this.listenTo(this.model, "change:fov", (() => {
+                        this.fov_js ? this.fov_js = !1 : (this.fov_py = !0, this.al.setFoV(this.model.get("fov")))
+                    }), this), this.listenTo(this.model, "change:target", (() => {
+                        this.target_js ? this.target_js = !1 : (this.target_py = !0, this.al.gotoObject(this.model.get("target")))
+                    }), this), this.listenTo(this.model, "change:coo_frame", (() => {
+                        this.al.setFrame(this.model.get("coo_frame"))
+                    }), this), this.listenTo(this.model, "change:height", (() => {
+                        let t = this.model.get("height");
+                        this.div.setAttribute("style", "width:100%;height:" + t + "px;")
+                    }), this), this.listenTo(this.model, "change:survey", (() => {
+                        this.al.setImageSurvey(this.model.get("survey"))
+                    }), this), this.listenTo(this.model, "change:overlay_survey", (() => {
+                        this.al.setOverlayImageLayer(this.model.get("overlay_survey"))
+                    }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (() => {
+                        this.al.getOverlayImageLayer().setAlpha(this.model.get("overlay_survey_opacity"))
+                    }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (() => {
+                        this.al.addCatalog(A.catalogFromURL(this.model.get("votable_URL"), this.model.get("votable_options")))
+                    }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (() => {
+                        this.al.addMOC(A.MOCFromURL(this.model.get("moc_URL"), this.model.get("moc_options")))
+                    }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (() => {
+                        this.al.addMOC(A.MOCFromJSON(this.model.get("moc_dict"), this.model.get("moc_options")))
+                    }), this), this.listenTo(this.model, "change:table_flag", (() => {
+                        let t = A.catalog({
                             onClick: "showTable"
                         });
-                        e.al.addCatalog(t), t.addSourcesAsArray(e.model.get("table_keys"), e.model.get("table_columns"))
-                    }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (function() {
-                        var t = A.graphicOverlay(e.model.get("overlay_options"));
-                        e.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(e.model.get("stc_string")))
-                    }), this), this.listenTo(this.model, "change:listener_flag", (function() {
-                        var t = e.model.get("listener_type");
-                        e.al.on(t, (function(a) {
-                            if ("select" !== t) a && e.send({
+                        this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
+                    }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
+                        let t = A.graphicOverlay(this.model.get("overlay_options"));
+                        this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
+                    }), this), this.listenTo(this.model, "change:listener_flag", (() => {
+                        let t = this.model.get("listener_type");
+                        this.al.on(t, (function(e) {
+                            if ("select" !== t) e && this.send({
                                 event: "callback",
                                 type: t,
                                 data: {
-                                    data: a.data,
-                                    dec: a.dec,
-                                    ra: a.ra,
-                                    x: a.x,
-                                    y: a.y
+                                    data: e.data,
+                                    dec: e.dec,
+                                    ra: e.ra,
+                                    x: e.x,
+                                    y: e.y
                                 }
                             });
                             else {
-                                for (var i = a, o = 0; o < e.al.view.catalogs.length; o++) e.al.view.catalogs[o].deselectAll();
-                                var s = [];
-                                for (o = 0; o < i.length; o++) {
-                                    var l = i[o];
-                                    l.select(), s.push({
-                                        data: l.data,
-                                        dec: l.dec,
-                                        ra: l.ra,
-                                        x: l.x,
-                                        y: l.y
-                                    })
-                                }
-                                e.send({
+                                let s = e;
+                                for (let t of this.al.view.catalogs) t.deselectAll();
+                                let i = [];
+                                for (let t of s) t.select(), i.push({
+                                    data: t.data,
+                                    dec: t.dec,
+                                    ra: t.ra,
+                                    x: t.x,
+                                    y: t.y
+                                });
+                                this.send({
                                     event: "callback",
                                     type: t,
-                                    data: s
+                                    data: i
                                 })
                             }
                         }))
-                    }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (function() {
-                        e.al.select()
-                    })), this.listenTo(this.model, "change:thumbnail_flag", (function() {
-                        e.al.exportAsPNG()
-                    })), this.listenTo(this.model, "change:color_map_flag", (function() {
-                        const t = e.model.get("color_map_name");
-                        e.al.getBaseImageLayer().setColormap(t)
+                    }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (() => {
+                        this.al.select()
+                    })), this.listenTo(this.model, "change:thumbnail_flag", (() => {
+                        this.al.exportAsPNG()
+                    })), this.listenTo(this.model, "change:color_map_flag", (() => {
+                        const t = this.model.get("color_map_name");
+                        this.al.getBaseImageLayer().setColormap(t)
                     }))
                 }
             }
-            const r = {
-                i8: "0.2.1"
-            }
-        },
-        261: (e, t, a) => {
-            a.r(t), a.d(t, {
-                aladinWidgetPlugin: () => o,
-                default: () => s
-            });
-            var i = a(678);
-            const o = {
+            const n = {
                     id: "ipyaladin:plugin",
-                    requires: [a(672).IJupyterWidgetRegistry],
-                    activate: function(e, t) {
-                        t.registerWidget({
+                    requires: [i.IJupyterWidgetRegistry],
+                    activate: function(t, e) {
+                        e.registerWidget({
                             name: "ipyaladin",
-                            version: i.version,
+                            version: "0.2.2",
                             exports: {
-                                AladinModel: i.AladinModel,
-                                AladinView: i.AladinView
+                                AladinModel: o,
+                                AladinView: d
                             }
                         })
                     },
                     autoStart: !0
                 },
-                s = o
+                r = n
         }
     }
 ]);
```

### Comparing `ipyaladin-0.2.1/ipyaladin/labextension/static/794.6f96ca96639b4fa21dce.js` & `ipyaladin-0.2.2/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1037,27 +1037,26 @@
                     var a = e ? e[o] : o;
                     i[o] = t(n[a], a, n)
                 }
                 return i
             }
 
             function Qt(n) {
-                var t = function(t, r, e, u) {
-                    var i = !_t(t) && cn(t),
-                        o = (i || t).length,
-                        a = n > 0 ? 0 : o - 1;
-                    for (u || (e = t[i ? i[a] : a], a += n); a >= 0 && a < o; a += n) {
-                        var c = i ? i[a] : a;
-                        e = r(e, t[c], c, t)
-                    }
-                    return e
-                };
-                return function(n, r, e, u) {
+                return function(t, r, e, u) {
                     var i = arguments.length >= 3;
-                    return t(n, Hn(r, u, 4), e, i)
+                    return function(t, r, e, u) {
+                        var i = !_t(t) && cn(t),
+                            o = (i || t).length,
+                            a = n > 0 ? 0 : o - 1;
+                        for (u || (e = t[i ? i[a] : a], a += n); a >= 0 && a < o; a += n) {
+                            var c = i ? i[a] : a;
+                            e = r(e, t[c], c, t)
+                        }
+                        return e
+                    }(t, Hn(r, u, 4), e, i)
                 }
             }
             const Xt = Qt(1),
                 Yt = Qt(-1);
 
             function Zt(n, t, r) {
                 var e = [];
```

### Comparing `ipyaladin-0.2.1/ipyaladin/labextension/static/remoteEntry.f2d6e628bd28c3f3b3b7.js` & `ipyaladin-0.2.2/ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, s, c, p, h, v, g, m, b = {
-            489: (e, r, t) => {
+    var e, r, t, n, o, a, i, l, d, u, s, f, c, p, h, v, g, b, m, y = {
+            460: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(112), t.e(678)]).then((() => () => t(678))),
-                        "./extension": () => Promise.all([t.e(112), t.e(261)]).then((() => () => t(261)))
+                        "./index": () => Promise.all([t.e(672), t.e(590)]).then((() => () => t(590))),
+                        "./extension": () => Promise.all([t.e(672), t.e(563)]).then((() => () => t(563)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,267 +20,268 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        y = {};
+        w = {};
 
-    function w(e) {
-        var r = y[e];
+    function S(e) {
+        var r = w[e];
         if (void 0 !== r) return r.exports;
-        var t = y[e] = {
+        var t = w[e] = {
+            id: e,
+            loaded: !1,
             exports: {}
         };
-        return b[e](t, t.exports, w), t.exports
+        return y[e](t, t.exports, S), t.loaded = !0, t.exports
     }
-    w.m = b, w.c = y, w.n = e => {
-        var r = e && e.__esModule ? () => e.default : () => e;
-        return w.d(r, {
-            a: r
-        }), r
-    }, w.d = (e, r) => {
-        for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
+    S.m = y, S.c = w, S.d = (e, r) => {
+        for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        112: "ff9a9865b4fcedf7e99c",
-        261: "bfcaf0ae589773f941db",
-        678: "54afe962dae4bf9693fa",
-        794: "6f96ca96639b4fa21dce"
+    }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
+        563: "b311860ae40bdaae42cf",
+        590: "9292295778c3653a0b31",
+        672: "d1c8706d8114ce8e432a",
+        794: "644314dbf6493c3f7619"
     } [e] + ".js?v=" + {
-        112: "ff9a9865b4fcedf7e99c",
-        261: "bfcaf0ae589773f941db",
-        678: "54afe962dae4bf9693fa",
-        794: "6f96ca96639b4fa21dce"
-    } [e], w.g = function() {
+        563: "b311860ae40bdaae42cf",
+        590: "9292295778c3653a0b31",
+        672: "d1c8706d8114ce8e432a",
+        794: "644314dbf6493c3f7619"
+    } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", w.l = (t, n, o, a) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", S.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, u;
+            var i, l;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
+                    var s = d[u];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, w.r = e => {
+    }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, (() => {
-        w.S = {};
+    }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        S.S = {};
         var e = {},
             r = {};
-        w.I = (t, n) => {
+        S.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                w.o(w.S, t) || (w.S[t] = {});
-                var a = w.S[t],
+                S.o(S.S, t) || (S.S[t] = {});
+                var a = S.S[t],
                     i = "ipyaladin",
-                    u = (e, r, t, n) => {
+                    l = (e, r, t, n) => {
                         var o = a[e] = a[e] || {},
-                            u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
+                            l = o[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("ipyaladin", "0.2.1", (() => Promise.all([w.e(112), w.e(678)]).then((() => () => w(678))))), u("underscore", "1.13.6", (() => w.e(794).then((() => () => w(794)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    d = [];
+                return "default" === t && (l("ipyaladin", "0.2.2", (() => Promise.all([S.e(672), S.e(590)]).then((() => () => S(590))))), l("underscore", "1.13.6", (() => S.e(794).then((() => () => S(794)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        w.g.importScripts && (e = w.g.location + "");
-        var r = w.g.document;
+        S.g.importScripts && (e = S.g.location + "");
+        var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), w.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), S.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
                 a = (typeof o)[0];
             if (n >= r.length) return "u" == a;
             var i = r[n],
-                u = (typeof i)[0];
-            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+                l = (typeof i)[0];
+            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
             if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
         for (a = 1; a < e.length; a++) {
-            var u = e[a];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
+            var l = e[a];
+            i.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
-        return l();
+        return d();
 
-        function l() {
+        function d() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
-                } else if (l)
-                    if (s == d)
-                        if (u <= n) {
-                            if (f != e[u]) return !1
+            for (var i = 0, l = 1, d = !0;; l++, i++) {
+                var u, s, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(u = r[i]))[0])) return !d || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == s) {
+                    if (!d || "u" != f) return !1
+                } else if (d)
+                    if (f == s)
+                        if (l <= n) {
+                            if (u != e[l]) return !1
                         } else {
-                            if (o ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (o ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (d = !1)
                         }
-                else if ("s" != s && "n" != s) {
-                    if (o || u <= n) return !1;
-                    l = !1, u--
+                else if ("s" != f && "n" != f) {
+                    if (o || l <= n) return !1;
+                    d = !1, l--
                 } else {
-                    if (u <= n || d < s != o) return !1;
-                    l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                    if (l <= n || s < f != o) return !1;
+                    d = !1
+                } else "s" != f && "n" != f && (d = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
-        var t = w.S[e];
-        if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = S.S[e];
+        if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, u = (e, r) => {
+    }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
-        var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
-    }, d = (e, r, t) => {
+    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
+        var o = l(e, t);
+        return a(n, o) || f(d(e, t, o, n)), c(e[t][o])
+    }, s = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, o) {
-        var a = w.I(r);
-        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = c(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && d(r, t, n);
-        return a ? s(a) : o()
-    })), v = {}, g = {
-        297: () => h("default", "underscore", [1, 1, 13, 6], (() => w.e(794).then((() => () => w(794))))),
-        672: () => p("default", "@jupyter-widgets/base", [, [1, 6],
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
+        var a = S.I(r);
+        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
+        var a = r && S.o(r, t) && s(r, t, n);
+        return a ? c(a) : o()
+    })), g = {}, b = {
+        672: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
-        ])
+        ]),
+        297: () => v("default", "underscore", [1, 1, 13, 6], (() => S.e(794).then((() => () => S(794)))))
     }, m = {
-        112: [297, 672]
-    }, w.f.consumes = (e, r) => {
-        w.o(m, e) && m[e].forEach((e => {
-            if (w.o(v, e)) return r.push(v[e]);
+        563: [297],
+        672: [672]
+    }, S.f.consumes = (e, r) => {
+        S.o(m, e) && m[e].forEach((e => {
+            if (S.o(g, e)) return r.push(g[e]);
             var t = r => {
-                    v[e] = 0, w.m[e] = t => {
-                        delete w.c[e], t.exports = r()
+                    g[e] = 0, S.m[e] = t => {
+                        delete S.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], w.m[e] = t => {
-                        throw delete w.c[e], r
+                    delete g[e], S.m[e] = t => {
+                        throw delete S.c[e], r
                     }
                 };
             try {
-                var o = g[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var o = b[e]();
+                o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             879: 0
         };
-        w.f.j = (r, t) => {
-            var n = w.o(e, r) ? e[r] : void 0;
+        S.f.j = (r, t) => {
+            var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (112 != r) {
+                else if (672 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var a = w.p + w.u(r),
+                var a = S.p + S.u(r),
                     i = new Error;
-                w.l(a, (t => {
-                    if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                S.l(a, (t => {
+                    if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             a = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, i, u] = t,
-                    l = 0;
+                var n, o, [a, i, l] = t,
+                    d = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) w.o(i, n) && (w.m[n] = i[n]);
-                    u && u(w)
+                    for (n in i) S.o(i, n) && (S.m[n] = i[n]);
+                    l && l(S)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); d < a.length; d++) o = a[d], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkipyaladin = self.webpackChunkipyaladin || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var S = w(489);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyaladin = S
+    var E = S(460);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyaladin = E
 })();
```

### Comparing `ipyaladin-0.2.1/ipyaladin/labextension/static/third-party-licenses.json` & `ipyaladin-0.2.2/ipyaladin/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/ipyaladin/nbextension/extension.js` & `ipyaladin-0.2.2/ipyaladin/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/ipyaladin/nbextension/index.js` & `ipyaladin-0.2.2/ipyaladin/nbextension/index.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,358 +1,358 @@
-define(["module", "@jupyter-widgets/base"], ((t, n) => (() => {
+define(["module", "@jupyter-widgets/base"], ((t, e) => (() => {
     "use strict";
-    var e = {
+    var n = {
             146: t => {
-                t.exports = n
+                t.exports = e
             },
-            325: n => {
-                n.exports = t
+            325: e => {
+                e.exports = t
             },
-            50: (t, n, e) => {
-                e.r(n), e.d(n, {
-                    VERSION: () => o,
-                    after: () => Ln,
-                    all: () => ne,
+            50: (t, e, n) => {
+                n.r(e), n.d(e, {
+                    VERSION: () => i,
+                    after: () => Ne,
+                    all: () => tn,
                     allKeys: () => gt,
-                    any: () => ee,
+                    any: () => en,
                     assign: () => Nt,
-                    before: () => Rn,
-                    bind: () => An,
-                    bindAll: () => Sn,
-                    chain: () => _n,
-                    chunk: () => Ue,
+                    before: () => Le,
+                    bind: () => we,
+                    bindAll: () => Oe,
+                    chain: () => ye,
+                    chunk: () => Un,
                     clone: () => Ut,
-                    collect: () => Hn,
-                    compact: () => Me,
-                    compose: () => Nn,
+                    collect: () => Ge,
+                    compact: () => Mn,
+                    compose: () => Fe,
                     constant: () => Y,
-                    contains: () => re,
-                    countBy: () => ye,
+                    contains: () => nn,
+                    countBy: () => mn,
                     create: () => Ct,
-                    debounce: () => Bn,
-                    default: () => We,
+                    debounce: () => Ie,
+                    default: () => Wn,
                     defaults: () => Lt,
-                    defer: () => Tn,
-                    delay: () => En,
-                    detect: () => Kn,
-                    difference: () => Te,
-                    drop: () => Oe,
-                    each: () => Gn,
-                    escape: () => un,
-                    every: () => ne,
+                    defer: () => Ee,
+                    delay: () => Me,
+                    detect: () => $e,
+                    difference: () => Tn,
+                    drop: () => On,
+                    each: () => Je,
+                    escape: () => ae,
+                    every: () => tn,
                     extend: () => Ft,
                     extendOwn: () => Nt,
-                    filter: () => Zn,
-                    find: () => Kn,
-                    findIndex: () => Vn,
-                    findKey: () => Un,
-                    findLastIndex: () => Pn,
-                    findWhere: () => Jn,
-                    first: () => xe,
-                    flatten: () => Ee,
-                    foldl: () => Xn,
-                    foldr: () => Yn,
-                    forEach: () => Gn,
+                    filter: () => Ye,
+                    find: () => $e,
+                    findIndex: () => De,
+                    findKey: () => Ce,
+                    findLastIndex: () => Ve,
+                    findWhere: () => Ke,
+                    first: () => xn,
+                    flatten: () => En,
+                    foldl: () => Qe,
+                    foldr: () => Xe,
+                    forEach: () => Je,
                     functions: () => Bt,
                     get: () => Wt,
-                    groupBy: () => ve,
+                    groupBy: () => vn,
                     has: () => zt,
-                    head: () => xe,
+                    head: () => xn,
                     identity: () => $t,
-                    include: () => re,
-                    includes: () => re,
-                    indexBy: () => ge,
-                    indexOf: () => zn,
-                    initial: () => Ae,
-                    inject: () => Xn,
-                    intersection: () => Fe,
+                    include: () => nn,
+                    includes: () => nn,
+                    indexBy: () => gn,
+                    indexOf: () => We,
+                    initial: () => An,
+                    inject: () => Qe,
+                    intersection: () => Fn,
                     invert: () => It,
-                    invoke: () => oe,
+                    invoke: () => rn,
                     isArguments: () => H,
                     isArray: () => K,
                     isArrayBuffer: () => C,
                     isBoolean: () => E,
                     isDataView: () => $,
                     isDate: () => F,
                     isElement: () => T,
                     isEmpty: () => lt,
                     isEqual: () => vt,
                     isError: () => L,
                     isFinite: () => Q,
                     isFunction: () => V,
                     isMap: () => xt,
-                    isMatch: () => ct,
+                    isMatch: () => st,
                     isNaN: () => X,
                     isNull: () => S,
                     isNumber: () => k,
                     isObject: () => O,
                     isRegExp: () => N,
                     isSet: () => St,
                     isString: () => B,
                     isSymbol: () => R,
-                    isTypedArray: () => ot,
+                    isTypedArray: () => it,
                     isUndefined: () => M,
                     isWeakMap: () => Ot,
                     isWeakSet: () => Mt,
                     iteratee: () => Qt,
                     keys: () => ut,
-                    last: () => Se,
-                    lastIndexOf: () => $n,
-                    map: () => Hn,
+                    last: () => Sn,
+                    lastIndexOf: () => ze,
+                    map: () => Ge,
                     mapObject: () => Yt,
                     matcher: () => Kt,
                     matches: () => Kt,
-                    max: () => ue,
-                    memoize: () => Mn,
+                    max: () => un,
+                    memoize: () => Se,
                     methods: () => Bt,
-                    min: () => le,
-                    mixin: () => Ve,
-                    negate: () => Fn,
+                    min: () => ln,
+                    mixin: () => Vn,
+                    negate: () => ke,
                     noop: () => Zt,
-                    now: () => rn,
-                    object: () => Re,
-                    omit: () => we,
-                    once: () => Cn,
+                    now: () => re,
+                    object: () => Rn,
+                    omit: () => wn,
+                    once: () => Re,
                     pairs: () => Tt,
-                    partial: () => wn,
-                    partition: () => me,
-                    pick: () => je,
-                    pluck: () => ie,
+                    partial: () => je,
+                    partition: () => yn,
+                    pick: () => jn,
+                    pluck: () => on,
                     property: () => Jt,
-                    propertyOf: () => tn,
-                    random: () => en,
-                    range: () => Ce,
-                    reduce: () => Xn,
-                    reduceRight: () => Yn,
-                    reject: () => te,
-                    rest: () => Oe,
+                    propertyOf: () => te,
+                    random: () => ne,
+                    range: () => Cn,
+                    reduce: () => Qe,
+                    reduceRight: () => Xe,
+                    reject: () => Ze,
+                    rest: () => On,
                     restArguments: () => x,
-                    result: () => gn,
-                    sample: () => fe,
-                    select: () => Zn,
-                    shuffle: () => pe,
-                    size: () => _e,
-                    some: () => ee,
-                    sortBy: () => he,
-                    sortedIndex: () => qn,
-                    tail: () => Oe,
-                    take: () => xe,
+                    result: () => ve,
+                    sample: () => fn,
+                    select: () => Ye,
+                    shuffle: () => hn,
+                    size: () => _n,
+                    some: () => en,
+                    sortBy: () => pn,
+                    sortedIndex: () => Pe,
+                    tail: () => On,
+                    take: () => xn,
                     tap: () => Dt,
-                    template: () => vn,
-                    templateSettings: () => cn,
-                    throttle: () => In,
-                    times: () => nn,
-                    toArray: () => se,
+                    template: () => de,
+                    templateSettings: () => le,
+                    throttle: () => Te,
+                    times: () => ee,
+                    toArray: () => cn,
                     toPath: () => Vt,
-                    transpose: () => Ne,
-                    unescape: () => ln,
-                    union: () => ke,
-                    uniq: () => Be,
-                    unique: () => Be,
-                    uniqueId: () => mn,
-                    unzip: () => Ne,
+                    transpose: () => Nn,
+                    unescape: () => ue,
+                    union: () => kn,
+                    uniq: () => Bn,
+                    unique: () => Bn,
+                    uniqueId: () => me,
+                    unzip: () => Nn,
                     values: () => Et,
-                    where: () => ae,
-                    without: () => Ie,
-                    wrap: () => kn,
-                    zip: () => Le
+                    where: () => an,
+                    without: () => In,
+                    wrap: () => Be,
+                    zip: () => Ln
                 });
                 var r = {};
-                e.r(r), e.d(r, {
-                    VERSION: () => o,
-                    after: () => Ln,
-                    all: () => ne,
+                n.r(r), n.d(r, {
+                    VERSION: () => i,
+                    after: () => Ne,
+                    all: () => tn,
                     allKeys: () => gt,
-                    any: () => ee,
+                    any: () => en,
                     assign: () => Nt,
-                    before: () => Rn,
-                    bind: () => An,
-                    bindAll: () => Sn,
-                    chain: () => _n,
-                    chunk: () => Ue,
+                    before: () => Le,
+                    bind: () => we,
+                    bindAll: () => Oe,
+                    chain: () => ye,
+                    chunk: () => Un,
                     clone: () => Ut,
-                    collect: () => Hn,
-                    compact: () => Me,
-                    compose: () => Nn,
+                    collect: () => Ge,
+                    compact: () => Mn,
+                    compose: () => Fe,
                     constant: () => Y,
-                    contains: () => re,
-                    countBy: () => ye,
+                    contains: () => nn,
+                    countBy: () => mn,
                     create: () => Ct,
-                    debounce: () => Bn,
-                    default: () => Pe,
+                    debounce: () => Ie,
+                    default: () => Pn,
                     defaults: () => Lt,
-                    defer: () => Tn,
-                    delay: () => En,
-                    detect: () => Kn,
-                    difference: () => Te,
-                    drop: () => Oe,
-                    each: () => Gn,
-                    escape: () => un,
-                    every: () => ne,
+                    defer: () => Ee,
+                    delay: () => Me,
+                    detect: () => $e,
+                    difference: () => Tn,
+                    drop: () => On,
+                    each: () => Je,
+                    escape: () => ae,
+                    every: () => tn,
                     extend: () => Ft,
                     extendOwn: () => Nt,
-                    filter: () => Zn,
-                    find: () => Kn,
-                    findIndex: () => Vn,
-                    findKey: () => Un,
-                    findLastIndex: () => Pn,
-                    findWhere: () => Jn,
-                    first: () => xe,
-                    flatten: () => Ee,
-                    foldl: () => Xn,
-                    foldr: () => Yn,
-                    forEach: () => Gn,
+                    filter: () => Ye,
+                    find: () => $e,
+                    findIndex: () => De,
+                    findKey: () => Ce,
+                    findLastIndex: () => Ve,
+                    findWhere: () => Ke,
+                    first: () => xn,
+                    flatten: () => En,
+                    foldl: () => Qe,
+                    foldr: () => Xe,
+                    forEach: () => Je,
                     functions: () => Bt,
                     get: () => Wt,
-                    groupBy: () => ve,
+                    groupBy: () => vn,
                     has: () => zt,
-                    head: () => xe,
+                    head: () => xn,
                     identity: () => $t,
-                    include: () => re,
-                    includes: () => re,
-                    indexBy: () => ge,
-                    indexOf: () => zn,
-                    initial: () => Ae,
-                    inject: () => Xn,
-                    intersection: () => Fe,
+                    include: () => nn,
+                    includes: () => nn,
+                    indexBy: () => gn,
+                    indexOf: () => We,
+                    initial: () => An,
+                    inject: () => Qe,
+                    intersection: () => Fn,
                     invert: () => It,
-                    invoke: () => oe,
+                    invoke: () => rn,
                     isArguments: () => H,
                     isArray: () => K,
                     isArrayBuffer: () => C,
                     isBoolean: () => E,
                     isDataView: () => $,
                     isDate: () => F,
                     isElement: () => T,
                     isEmpty: () => lt,
                     isEqual: () => vt,
                     isError: () => L,
                     isFinite: () => Q,
                     isFunction: () => V,
                     isMap: () => xt,
-                    isMatch: () => ct,
+                    isMatch: () => st,
                     isNaN: () => X,
                     isNull: () => S,
                     isNumber: () => k,
                     isObject: () => O,
                     isRegExp: () => N,
                     isSet: () => St,
                     isString: () => B,
                     isSymbol: () => R,
-                    isTypedArray: () => ot,
+                    isTypedArray: () => it,
                     isUndefined: () => M,
                     isWeakMap: () => Ot,
                     isWeakSet: () => Mt,
                     iteratee: () => Qt,
                     keys: () => ut,
-                    last: () => Se,
-                    lastIndexOf: () => $n,
-                    map: () => Hn,
+                    last: () => Sn,
+                    lastIndexOf: () => ze,
+                    map: () => Ge,
                     mapObject: () => Yt,
                     matcher: () => Kt,
                     matches: () => Kt,
-                    max: () => ue,
-                    memoize: () => Mn,
+                    max: () => un,
+                    memoize: () => Se,
                     methods: () => Bt,
-                    min: () => le,
-                    mixin: () => Ve,
-                    negate: () => Fn,
+                    min: () => ln,
+                    mixin: () => Vn,
+                    negate: () => ke,
                     noop: () => Zt,
-                    now: () => rn,
-                    object: () => Re,
-                    omit: () => we,
-                    once: () => Cn,
+                    now: () => re,
+                    object: () => Rn,
+                    omit: () => wn,
+                    once: () => Re,
                     pairs: () => Tt,
-                    partial: () => wn,
-                    partition: () => me,
-                    pick: () => je,
-                    pluck: () => ie,
+                    partial: () => je,
+                    partition: () => yn,
+                    pick: () => jn,
+                    pluck: () => on,
                     property: () => Jt,
-                    propertyOf: () => tn,
-                    random: () => en,
-                    range: () => Ce,
-                    reduce: () => Xn,
-                    reduceRight: () => Yn,
-                    reject: () => te,
-                    rest: () => Oe,
+                    propertyOf: () => te,
+                    random: () => ne,
+                    range: () => Cn,
+                    reduce: () => Qe,
+                    reduceRight: () => Xe,
+                    reject: () => Ze,
+                    rest: () => On,
                     restArguments: () => x,
-                    result: () => gn,
-                    sample: () => fe,
-                    select: () => Zn,
-                    shuffle: () => pe,
-                    size: () => _e,
-                    some: () => ee,
-                    sortBy: () => he,
-                    sortedIndex: () => qn,
-                    tail: () => Oe,
-                    take: () => xe,
+                    result: () => ve,
+                    sample: () => fn,
+                    select: () => Ye,
+                    shuffle: () => hn,
+                    size: () => _n,
+                    some: () => en,
+                    sortBy: () => pn,
+                    sortedIndex: () => Pe,
+                    tail: () => On,
+                    take: () => xn,
                     tap: () => Dt,
-                    template: () => vn,
-                    templateSettings: () => cn,
-                    throttle: () => In,
-                    times: () => nn,
-                    toArray: () => se,
+                    template: () => de,
+                    templateSettings: () => le,
+                    throttle: () => Te,
+                    times: () => ee,
+                    toArray: () => cn,
                     toPath: () => Vt,
-                    transpose: () => Ne,
-                    unescape: () => ln,
-                    union: () => ke,
-                    uniq: () => Be,
-                    unique: () => Be,
-                    uniqueId: () => mn,
-                    unzip: () => Ne,
+                    transpose: () => Nn,
+                    unescape: () => ue,
+                    union: () => kn,
+                    uniq: () => Bn,
+                    unique: () => Bn,
+                    uniqueId: () => me,
+                    unzip: () => Nn,
                     values: () => Et,
-                    where: () => ae,
-                    without: () => Ie,
-                    wrap: () => kn,
-                    zip: () => Le
+                    where: () => an,
+                    without: () => In,
+                    wrap: () => Be,
+                    zip: () => Ln
                 });
-                var o = "1.13.6",
-                    i = "object" == typeof self && self.self === self && self || "object" == typeof global && global.global === global && global || Function("return this")() || {},
+                var i = "1.13.6",
+                    o = "object" == typeof self && self.self === self && self || "object" == typeof global && global.global === global && global || Function("return this")() || {},
                     a = Array.prototype,
                     u = Object.prototype,
                     l = "undefined" != typeof Symbol ? Symbol.prototype : null,
-                    c = a.push,
-                    s = a.slice,
+                    s = a.push,
+                    c = a.slice,
                     f = u.toString,
-                    p = u.hasOwnProperty,
-                    h = "undefined" != typeof ArrayBuffer,
+                    h = u.hasOwnProperty,
+                    p = "undefined" != typeof ArrayBuffer,
                     d = "undefined" != typeof DataView,
                     v = Array.isArray,
                     g = Object.keys,
-                    y = Object.create,
-                    m = h && ArrayBuffer.isView,
+                    m = Object.create,
+                    y = p && ArrayBuffer.isView,
                     _ = isNaN,
                     b = isFinite,
                     j = !{
                         toString: null
                     }.propertyIsEnumerable("toString"),
                     w = ["valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
                     A = Math.pow(2, 53) - 1;
 
-                function x(t, n) {
-                    return n = null == n ? t.length - 1 : +n,
+                function x(t, e) {
+                    return e = null == e ? t.length - 1 : +e,
                         function() {
-                            for (var e = Math.max(arguments.length - n, 0), r = Array(e), o = 0; o < e; o++) r[o] = arguments[o + n];
-                            switch (n) {
+                            for (var n = Math.max(arguments.length - e, 0), r = Array(n), i = 0; i < n; i++) r[i] = arguments[i + e];
+                            switch (e) {
                                 case 0:
                                     return t.call(this, r);
                                 case 1:
                                     return t.call(this, arguments[0], r);
                                 case 2:
                                     return t.call(this, arguments[0], arguments[1], r)
                             }
-                            var i = Array(n + 1);
-                            for (o = 0; o < n; o++) i[o] = arguments[o];
-                            return i[n] = r, t.apply(this, i)
+                            var o = Array(e + 1);
+                            for (i = 0; i < e; i++) o[i] = arguments[i];
+                            return o[e] = r, t.apply(this, o)
                         }
                 }
 
                 function O(t) {
-                    var n = typeof t;
-                    return "function" === n || "object" === n && !!t
+                    var e = typeof t;
+                    return "function" === e || "object" === e && !!t
                 }
 
                 function S(t) {
                     return null === t
                 }
 
                 function M(t) {
@@ -364,43 +364,43 @@
                 }
 
                 function T(t) {
                     return !(!t || 1 !== t.nodeType)
                 }
 
                 function I(t) {
-                    var n = "[object " + t + "]";
+                    var e = "[object " + t + "]";
                     return function(t) {
-                        return f.call(t) === n
+                        return f.call(t) === e
                     }
                 }
                 const B = I("String"),
                     k = I("Number"),
                     F = I("Date"),
                     N = I("RegExp"),
                     L = I("Error"),
                     R = I("Symbol"),
                     C = I("ArrayBuffer");
                 var U = I("Function"),
-                    D = i.document && i.document.childNodes;
+                    D = o.document && o.document.childNodes;
                 "object" != typeof Int8Array && "function" != typeof D && (U = function(t) {
                     return "function" == typeof t || !1
                 });
                 const V = U,
                     P = I("Object");
                 var q = d && P(new DataView(new ArrayBuffer(8))),
                     W = "undefined" != typeof Map && P(new Map),
                     z = I("DataView");
                 const $ = q ? function(t) {
                         return null != t && V(t.getInt8) && C(t.buffer)
                     } : z,
                     K = v || I("Array");
 
-                function J(t, n) {
-                    return null != t && p.call(t, n)
+                function J(t, e) {
+                    return null != t && h.call(t, e)
                 }
                 var G = I("Arguments");
                 ! function() {
                     G(arguments) || (G = function(t) {
                         return J(t, "callee")
                     })
                 }();
@@ -417,1112 +417,1114 @@
                 function Y(t) {
                     return function() {
                         return t
                     }
                 }
 
                 function Z(t) {
-                    return function(n) {
-                        var e = t(n);
-                        return "number" == typeof e && e >= 0 && e <= A
+                    return function(e) {
+                        var n = t(e);
+                        return "number" == typeof n && n >= 0 && n <= A
                     }
                 }
 
                 function tt(t) {
-                    return function(n) {
-                        return null == n ? void 0 : n[t]
+                    return function(e) {
+                        return null == e ? void 0 : e[t]
                     }
                 }
-                const nt = tt("byteLength"),
-                    et = Z(nt);
+                const et = tt("byteLength"),
+                    nt = Z(et);
                 var rt = /\[object ((I|Ui)nt(8|16|32)|Float(32|64)|Uint8Clamped|Big(I|Ui)nt64)Array\]/;
-                const ot = h ? function(t) {
-                        return m ? m(t) && !$(t) : et(t) && rt.test(f.call(t))
+                const it = p ? function(t) {
+                        return y ? y(t) && !$(t) : nt(t) && rt.test(f.call(t))
                     } : Y(!1),
-                    it = tt("length");
+                    ot = tt("length");
 
-                function at(t, n) {
-                    n = function(t) {
-                        for (var n = {}, e = t.length, r = 0; r < e; ++r) n[t[r]] = !0;
+                function at(t, e) {
+                    e = function(t) {
+                        for (var e = {}, n = t.length, r = 0; r < n; ++r) e[t[r]] = !0;
                         return {
                             contains: function(t) {
-                                return !0 === n[t]
+                                return !0 === e[t]
                             },
-                            push: function(e) {
-                                return n[e] = !0, t.push(e)
+                            push: function(n) {
+                                return e[n] = !0, t.push(n)
                             }
                         }
-                    }(n);
-                    var e = w.length,
+                    }(e);
+                    var n = w.length,
                         r = t.constructor,
-                        o = V(r) && r.prototype || u,
-                        i = "constructor";
-                    for (J(t, i) && !n.contains(i) && n.push(i); e--;)(i = w[e]) in t && t[i] !== o[i] && !n.contains(i) && n.push(i)
+                        i = V(r) && r.prototype || u,
+                        o = "constructor";
+                    for (J(t, o) && !e.contains(o) && e.push(o); n--;)(o = w[n]) in t && t[o] !== i[o] && !e.contains(o) && e.push(o)
                 }
 
                 function ut(t) {
                     if (!O(t)) return [];
                     if (g) return g(t);
-                    var n = [];
-                    for (var e in t) J(t, e) && n.push(e);
-                    return j && at(t, n), n
+                    var e = [];
+                    for (var n in t) J(t, n) && e.push(n);
+                    return j && at(t, e), e
                 }
 
                 function lt(t) {
                     if (null == t) return !0;
-                    var n = it(t);
-                    return "number" == typeof n && (K(t) || B(t) || H(t)) ? 0 === n : 0 === it(ut(t))
+                    var e = ot(t);
+                    return "number" == typeof e && (K(t) || B(t) || H(t)) ? 0 === e : 0 === ot(ut(t))
                 }
 
-                function ct(t, n) {
-                    var e = ut(n),
-                        r = e.length;
+                function st(t, e) {
+                    var n = ut(e),
+                        r = n.length;
                     if (null == t) return !r;
-                    for (var o = Object(t), i = 0; i < r; i++) {
-                        var a = e[i];
-                        if (n[a] !== o[a] || !(a in o)) return !1
+                    for (var i = Object(t), o = 0; o < r; o++) {
+                        var a = n[o];
+                        if (e[a] !== i[a] || !(a in i)) return !1
                     }
                     return !0
                 }
 
-                function st(t) {
-                    return t instanceof st ? t : this instanceof st ? void(this._wrapped = t) : new st(t)
+                function ct(t) {
+                    return t instanceof ct ? t : this instanceof ct ? void(this._wrapped = t) : new ct(t)
                 }
 
                 function ft(t) {
-                    return new Uint8Array(t.buffer || t, t.byteOffset || 0, nt(t))
+                    return new Uint8Array(t.buffer || t, t.byteOffset || 0, et(t))
                 }
-                st.VERSION = o, st.prototype.value = function() {
+                ct.VERSION = i, ct.prototype.value = function() {
                     return this._wrapped
-                }, st.prototype.valueOf = st.prototype.toJSON = st.prototype.value, st.prototype.toString = function() {
+                }, ct.prototype.valueOf = ct.prototype.toJSON = ct.prototype.value, ct.prototype.toString = function() {
                     return String(this._wrapped)
                 };
-                var pt = "[object DataView]";
+                var ht = "[object DataView]";
 
-                function ht(t, n, e, r) {
-                    if (t === n) return 0 !== t || 1 / t == 1 / n;
-                    if (null == t || null == n) return !1;
-                    if (t != t) return n != n;
-                    var o = typeof t;
-                    return ("function" === o || "object" === o || "object" == typeof n) && dt(t, n, e, r)
-                }
-
-                function dt(t, n, e, r) {
-                    t instanceof st && (t = t._wrapped), n instanceof st && (n = n._wrapped);
-                    var o = f.call(t);
-                    if (o !== f.call(n)) return !1;
-                    if (q && "[object Object]" == o && $(t)) {
-                        if (!$(n)) return !1;
-                        o = pt
+                function pt(t, e, n, r) {
+                    if (t === e) return 0 !== t || 1 / t == 1 / e;
+                    if (null == t || null == e) return !1;
+                    if (t != t) return e != e;
+                    var i = typeof t;
+                    return ("function" === i || "object" === i || "object" == typeof e) && dt(t, e, n, r)
+                }
+
+                function dt(t, e, n, r) {
+                    t instanceof ct && (t = t._wrapped), e instanceof ct && (e = e._wrapped);
+                    var i = f.call(t);
+                    if (i !== f.call(e)) return !1;
+                    if (q && "[object Object]" == i && $(t)) {
+                        if (!$(e)) return !1;
+                        i = ht
                     }
-                    switch (o) {
+                    switch (i) {
                         case "[object RegExp]":
                         case "[object String]":
-                            return "" + t == "" + n;
+                            return "" + t == "" + e;
                         case "[object Number]":
-                            return +t != +t ? +n != +n : 0 == +t ? 1 / +t == 1 / n : +t == +n;
+                            return +t != +t ? +e != +e : 0 == +t ? 1 / +t == 1 / e : +t == +e;
                         case "[object Date]":
                         case "[object Boolean]":
-                            return +t == +n;
+                            return +t == +e;
                         case "[object Symbol]":
-                            return l.valueOf.call(t) === l.valueOf.call(n);
+                            return l.valueOf.call(t) === l.valueOf.call(e);
                         case "[object ArrayBuffer]":
-                        case pt:
-                            return dt(ft(t), ft(n), e, r)
+                        case ht:
+                            return dt(ft(t), ft(e), n, r)
                     }
-                    var i = "[object Array]" === o;
-                    if (!i && ot(t)) {
-                        if (nt(t) !== nt(n)) return !1;
-                        if (t.buffer === n.buffer && t.byteOffset === n.byteOffset) return !0;
-                        i = !0
+                    var o = "[object Array]" === i;
+                    if (!o && it(t)) {
+                        if (et(t) !== et(e)) return !1;
+                        if (t.buffer === e.buffer && t.byteOffset === e.byteOffset) return !0;
+                        o = !0
                     }
-                    if (!i) {
-                        if ("object" != typeof t || "object" != typeof n) return !1;
+                    if (!o) {
+                        if ("object" != typeof t || "object" != typeof e) return !1;
                         var a = t.constructor,
-                            u = n.constructor;
-                        if (a !== u && !(V(a) && a instanceof a && V(u) && u instanceof u) && "constructor" in t && "constructor" in n) return !1
+                            u = e.constructor;
+                        if (a !== u && !(V(a) && a instanceof a && V(u) && u instanceof u) && "constructor" in t && "constructor" in e) return !1
                     }
                     r = r || [];
-                    for (var c = (e = e || []).length; c--;)
-                        if (e[c] === t) return r[c] === n;
-                    if (e.push(t), r.push(n), i) {
-                        if ((c = t.length) !== n.length) return !1;
-                        for (; c--;)
-                            if (!ht(t[c], n[c], e, r)) return !1
+                    for (var s = (n = n || []).length; s--;)
+                        if (n[s] === t) return r[s] === e;
+                    if (n.push(t), r.push(e), o) {
+                        if ((s = t.length) !== e.length) return !1;
+                        for (; s--;)
+                            if (!pt(t[s], e[s], n, r)) return !1
                     } else {
-                        var s, p = ut(t);
-                        if (c = p.length, ut(n).length !== c) return !1;
-                        for (; c--;)
-                            if (!J(n, s = p[c]) || !ht(t[s], n[s], e, r)) return !1
+                        var c, h = ut(t);
+                        if (s = h.length, ut(e).length !== s) return !1;
+                        for (; s--;)
+                            if (!J(e, c = h[s]) || !pt(t[c], e[c], n, r)) return !1
                     }
-                    return e.pop(), r.pop(), !0
+                    return n.pop(), r.pop(), !0
                 }
 
-                function vt(t, n) {
-                    return ht(t, n)
+                function vt(t, e) {
+                    return pt(t, e)
                 }
 
                 function gt(t) {
                     if (!O(t)) return [];
-                    var n = [];
-                    for (var e in t) n.push(e);
-                    return j && at(t, n), n
+                    var e = [];
+                    for (var n in t) e.push(n);
+                    return j && at(t, e), e
                 }
 
-                function yt(t) {
-                    var n = it(t);
-                    return function(e) {
-                        if (null == e) return !1;
-                        var r = gt(e);
-                        if (it(r)) return !1;
-                        for (var o = 0; o < n; o++)
-                            if (!V(e[t[o]])) return !1;
-                        return t !== wt || !V(e[mt])
+                function mt(t) {
+                    var e = ot(t);
+                    return function(n) {
+                        if (null == n) return !1;
+                        var r = gt(n);
+                        if (ot(r)) return !1;
+                        for (var i = 0; i < e; i++)
+                            if (!V(n[t[i]])) return !1;
+                        return t !== wt || !V(n[yt])
                     }
                 }
-                var mt = "forEach",
+                var yt = "forEach",
                     _t = ["clear", "delete"],
                     bt = ["get", "has", "set"],
-                    jt = _t.concat(mt, bt),
+                    jt = _t.concat(yt, bt),
                     wt = _t.concat(bt),
-                    At = ["add"].concat(_t, mt, "has");
-                const xt = W ? yt(jt) : I("Map"),
-                    Ot = W ? yt(wt) : I("WeakMap"),
-                    St = W ? yt(At) : I("Set"),
+                    At = ["add"].concat(_t, yt, "has");
+                const xt = W ? mt(jt) : I("Map"),
+                    Ot = W ? mt(wt) : I("WeakMap"),
+                    St = W ? mt(At) : I("Set"),
                     Mt = I("WeakSet");
 
                 function Et(t) {
-                    for (var n = ut(t), e = n.length, r = Array(e), o = 0; o < e; o++) r[o] = t[n[o]];
+                    for (var e = ut(t), n = e.length, r = Array(n), i = 0; i < n; i++) r[i] = t[e[i]];
                     return r
                 }
 
                 function Tt(t) {
-                    for (var n = ut(t), e = n.length, r = Array(e), o = 0; o < e; o++) r[o] = [n[o], t[n[o]]];
+                    for (var e = ut(t), n = e.length, r = Array(n), i = 0; i < n; i++) r[i] = [e[i], t[e[i]]];
                     return r
                 }
 
                 function It(t) {
-                    for (var n = {}, e = ut(t), r = 0, o = e.length; r < o; r++) n[t[e[r]]] = e[r];
-                    return n
+                    for (var e = {}, n = ut(t), r = 0, i = n.length; r < i; r++) e[t[n[r]]] = n[r];
+                    return e
                 }
 
                 function Bt(t) {
-                    var n = [];
-                    for (var e in t) V(t[e]) && n.push(e);
-                    return n.sort()
+                    var e = [];
+                    for (var n in t) V(t[n]) && e.push(n);
+                    return e.sort()
                 }
 
-                function kt(t, n) {
-                    return function(e) {
+                function kt(t, e) {
+                    return function(n) {
                         var r = arguments.length;
-                        if (n && (e = Object(e)), r < 2 || null == e) return e;
-                        for (var o = 1; o < r; o++)
-                            for (var i = arguments[o], a = t(i), u = a.length, l = 0; l < u; l++) {
-                                var c = a[l];
-                                n && void 0 !== e[c] || (e[c] = i[c])
+                        if (e && (n = Object(n)), r < 2 || null == n) return n;
+                        for (var i = 1; i < r; i++)
+                            for (var o = arguments[i], a = t(o), u = a.length, l = 0; l < u; l++) {
+                                var s = a[l];
+                                e && void 0 !== n[s] || (n[s] = o[s])
                             }
-                        return e
+                        return n
                     }
                 }
                 const Ft = kt(gt),
                     Nt = kt(ut),
                     Lt = kt(gt, !0);
 
                 function Rt(t) {
                     if (!O(t)) return {};
-                    if (y) return y(t);
-                    var n = function() {};
-                    n.prototype = t;
-                    var e = new n;
-                    return n.prototype = null, e
+                    if (m) return m(t);
+                    var e = function() {};
+                    e.prototype = t;
+                    var n = new e;
+                    return e.prototype = null, n
                 }
 
-                function Ct(t, n) {
-                    var e = Rt(t);
-                    return n && Nt(e, n), e
+                function Ct(t, e) {
+                    var n = Rt(t);
+                    return e && Nt(n, e), n
                 }
 
                 function Ut(t) {
                     return O(t) ? K(t) ? t.slice() : Ft({}, t) : t
                 }
 
-                function Dt(t, n) {
-                    return n(t), t
+                function Dt(t, e) {
+                    return e(t), t
                 }
 
                 function Vt(t) {
                     return K(t) ? t : [t]
                 }
 
                 function Pt(t) {
-                    return st.toPath(t)
+                    return ct.toPath(t)
                 }
 
-                function qt(t, n) {
-                    for (var e = n.length, r = 0; r < e; r++) {
+                function qt(t, e) {
+                    for (var n = e.length, r = 0; r < n; r++) {
                         if (null == t) return;
-                        t = t[n[r]]
+                        t = t[e[r]]
                     }
-                    return e ? t : void 0
+                    return n ? t : void 0
                 }
 
-                function Wt(t, n, e) {
-                    var r = qt(t, Pt(n));
-                    return M(r) ? e : r
+                function Wt(t, e, n) {
+                    var r = qt(t, Pt(e));
+                    return M(r) ? n : r
                 }
 
-                function zt(t, n) {
-                    for (var e = (n = Pt(n)).length, r = 0; r < e; r++) {
-                        var o = n[r];
-                        if (!J(t, o)) return !1;
-                        t = t[o]
+                function zt(t, e) {
+                    for (var n = (e = Pt(e)).length, r = 0; r < n; r++) {
+                        var i = e[r];
+                        if (!J(t, i)) return !1;
+                        t = t[i]
                     }
-                    return !!e
+                    return !!n
                 }
 
                 function $t(t) {
                     return t
                 }
 
                 function Kt(t) {
                     return t = Nt({}, t),
-                        function(n) {
-                            return ct(n, t)
+                        function(e) {
+                            return st(e, t)
                         }
                 }
 
                 function Jt(t) {
                     return t = Pt(t),
-                        function(n) {
-                            return qt(n, t)
+                        function(e) {
+                            return qt(e, t)
                         }
                 }
 
-                function Gt(t, n, e) {
-                    if (void 0 === n) return t;
-                    switch (null == e ? 3 : e) {
+                function Gt(t, e, n) {
+                    if (void 0 === e) return t;
+                    switch (null == n ? 3 : n) {
                         case 1:
-                            return function(e) {
-                                return t.call(n, e)
+                            return function(n) {
+                                return t.call(e, n)
                             };
                         case 3:
-                            return function(e, r, o) {
-                                return t.call(n, e, r, o)
+                            return function(n, r, i) {
+                                return t.call(e, n, r, i)
                             };
                         case 4:
-                            return function(e, r, o, i) {
-                                return t.call(n, e, r, o, i)
+                            return function(n, r, i, o) {
+                                return t.call(e, n, r, i, o)
                             }
                     }
                     return function() {
-                        return t.apply(n, arguments)
+                        return t.apply(e, arguments)
                     }
                 }
 
-                function Ht(t, n, e) {
-                    return null == t ? $t : V(t) ? Gt(t, n, e) : O(t) && !K(t) ? Kt(t) : Jt(t)
+                function Ht(t, e, n) {
+                    return null == t ? $t : V(t) ? Gt(t, e, n) : O(t) && !K(t) ? Kt(t) : Jt(t)
                 }
 
-                function Qt(t, n) {
-                    return Ht(t, n, 1 / 0)
+                function Qt(t, e) {
+                    return Ht(t, e, 1 / 0)
                 }
 
-                function Xt(t, n, e) {
-                    return st.iteratee !== Qt ? st.iteratee(t, n) : Ht(t, n, e)
+                function Xt(t, e, n) {
+                    return ct.iteratee !== Qt ? ct.iteratee(t, e) : Ht(t, e, n)
                 }
 
-                function Yt(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = ut(t), o = r.length, i = {}, a = 0; a < o; a++) {
+                function Yt(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = ut(t), i = r.length, o = {}, a = 0; a < i; a++) {
                         var u = r[a];
-                        i[u] = n(t[u], u, t)
+                        o[u] = e(t[u], u, t)
                     }
-                    return i
+                    return o
                 }
 
                 function Zt() {}
 
-                function tn(t) {
-                    return null == t ? Zt : function(n) {
-                        return Wt(t, n)
+                function te(t) {
+                    return null == t ? Zt : function(e) {
+                        return Wt(t, e)
                     }
                 }
 
-                function nn(t, n, e) {
+                function ee(t, e, n) {
                     var r = Array(Math.max(0, t));
-                    n = Gt(n, e, 1);
-                    for (var o = 0; o < t; o++) r[o] = n(o);
+                    e = Gt(e, n, 1);
+                    for (var i = 0; i < t; i++) r[i] = e(i);
                     return r
                 }
 
-                function en(t, n) {
-                    return null == n && (n = t, t = 0), t + Math.floor(Math.random() * (n - t + 1))
+                function ne(t, e) {
+                    return null == e && (e = t, t = 0), t + Math.floor(Math.random() * (e - t + 1))
                 }
-                st.toPath = Vt, st.iteratee = Qt;
-                const rn = Date.now || function() {
+                ct.toPath = Vt, ct.iteratee = Qt;
+                const re = Date.now || function() {
                     return (new Date).getTime()
                 };
 
-                function on(t) {
-                    var n = function(n) {
-                            return t[n]
+                function ie(t) {
+                    var e = function(e) {
+                            return t[e]
                         },
-                        e = "(?:" + ut(t).join("|") + ")",
-                        r = RegExp(e),
-                        o = RegExp(e, "g");
+                        n = "(?:" + ut(t).join("|") + ")",
+                        r = RegExp(n),
+                        i = RegExp(n, "g");
                     return function(t) {
-                        return t = null == t ? "" : "" + t, r.test(t) ? t.replace(o, n) : t
+                        return t = null == t ? "" : "" + t, r.test(t) ? t.replace(i, e) : t
                     }
                 }
-                const an = {
+                const oe = {
                         "&": "&amp;",
                         "<": "&lt;",
                         ">": "&gt;",
                         '"': "&quot;",
                         "'": "&#x27;",
                         "`": "&#x60;"
                     },
-                    un = on(an),
-                    ln = on(It(an)),
-                    cn = st.templateSettings = {
+                    ae = ie(oe),
+                    ue = ie(It(oe)),
+                    le = ct.templateSettings = {
                         evaluate: /<%([\s\S]+?)%>/g,
                         interpolate: /<%=([\s\S]+?)%>/g,
                         escape: /<%-([\s\S]+?)%>/g
                     };
-                var sn = /(.)^/,
-                    fn = {
+                var se = /(.)^/,
+                    ce = {
                         "'": "'",
                         "\\": "\\",
                         "\r": "r",
                         "\n": "n",
                         "\u2028": "u2028",
                         "\u2029": "u2029"
                     },
-                    pn = /\\|'|\r|\n|\u2028|\u2029/g;
+                    fe = /\\|'|\r|\n|\u2028|\u2029/g;
 
-                function hn(t) {
-                    return "\\" + fn[t]
+                function he(t) {
+                    return "\\" + ce[t]
                 }
-                var dn = /^\s*(\w|\$)+\s*$/;
+                var pe = /^\s*(\w|\$)+\s*$/;
 
-                function vn(t, n, e) {
-                    !n && e && (n = e), n = Lt({}, n, st.templateSettings);
-                    var r = RegExp([(n.escape || sn).source, (n.interpolate || sn).source, (n.evaluate || sn).source].join("|") + "|$", "g"),
-                        o = 0,
-                        i = "__p+='";
-                    t.replace(r, (function(n, e, r, a, u) {
-                        return i += t.slice(o, u).replace(pn, hn), o = u + n.length, e ? i += "'+\n((__t=(" + e + "))==null?'':_.escape(__t))+\n'" : r ? i += "'+\n((__t=(" + r + "))==null?'':__t)+\n'" : a && (i += "';\n" + a + "\n__p+='"), n
-                    })), i += "';\n";
-                    var a, u = n.variable;
+                function de(t, e, n) {
+                    !e && n && (e = n), e = Lt({}, e, ct.templateSettings);
+                    var r = RegExp([(e.escape || se).source, (e.interpolate || se).source, (e.evaluate || se).source].join("|") + "|$", "g"),
+                        i = 0,
+                        o = "__p+='";
+                    t.replace(r, (function(e, n, r, a, u) {
+                        return o += t.slice(i, u).replace(fe, he), i = u + e.length, n ? o += "'+\n((__t=(" + n + "))==null?'':_.escape(__t))+\n'" : r ? o += "'+\n((__t=(" + r + "))==null?'':__t)+\n'" : a && (o += "';\n" + a + "\n__p+='"), e
+                    })), o += "';\n";
+                    var a, u = e.variable;
                     if (u) {
-                        if (!dn.test(u)) throw new Error("variable is not a bare identifier: " + u)
-                    } else i = "with(obj||{}){\n" + i + "}\n", u = "obj";
-                    i = "var __t,__p='',__j=Array.prototype.join,print=function(){__p+=__j.call(arguments,'');};\n" + i + "return __p;\n";
+                        if (!pe.test(u)) throw new Error("variable is not a bare identifier: " + u)
+                    } else o = "with(obj||{}){\n" + o + "}\n", u = "obj";
+                    o = "var __t,__p='',__j=Array.prototype.join,print=function(){__p+=__j.call(arguments,'');};\n" + o + "return __p;\n";
                     try {
-                        a = new Function(u, "_", i)
+                        a = new Function(u, "_", o)
                     } catch (t) {
-                        throw t.source = i, t
+                        throw t.source = o, t
                     }
                     var l = function(t) {
-                        return a.call(this, t, st)
+                        return a.call(this, t, ct)
                     };
-                    return l.source = "function(" + u + "){\n" + i + "}", l
+                    return l.source = "function(" + u + "){\n" + o + "}", l
                 }
 
-                function gn(t, n, e) {
-                    var r = (n = Pt(n)).length;
-                    if (!r) return V(e) ? e.call(t) : e;
-                    for (var o = 0; o < r; o++) {
-                        var i = null == t ? void 0 : t[n[o]];
-                        void 0 === i && (i = e, o = r), t = V(i) ? i.call(t) : i
+                function ve(t, e, n) {
+                    var r = (e = Pt(e)).length;
+                    if (!r) return V(n) ? n.call(t) : n;
+                    for (var i = 0; i < r; i++) {
+                        var o = null == t ? void 0 : t[e[i]];
+                        void 0 === o && (o = n, i = r), t = V(o) ? o.call(t) : o
                     }
                     return t
                 }
-                var yn = 0;
+                var ge = 0;
 
-                function mn(t) {
-                    var n = ++yn + "";
-                    return t ? t + n : n
+                function me(t) {
+                    var e = ++ge + "";
+                    return t ? t + e : e
                 }
 
-                function _n(t) {
-                    var n = st(t);
-                    return n._chain = !0, n
+                function ye(t) {
+                    var e = ct(t);
+                    return e._chain = !0, e
                 }
 
-                function bn(t, n, e, r, o) {
-                    if (!(r instanceof n)) return t.apply(e, o);
-                    var i = Rt(t.prototype),
-                        a = t.apply(i, o);
-                    return O(a) ? a : i
+                function _e(t, e, n, r, i) {
+                    if (!(r instanceof e)) return t.apply(n, i);
+                    var o = Rt(t.prototype),
+                        a = t.apply(o, i);
+                    return O(a) ? a : o
                 }
-                var jn = x((function(t, n) {
-                    var e = jn.placeholder,
+                var be = x((function(t, e) {
+                    var n = be.placeholder,
                         r = function() {
-                            for (var o = 0, i = n.length, a = Array(i), u = 0; u < i; u++) a[u] = n[u] === e ? arguments[o++] : n[u];
-                            for (; o < arguments.length;) a.push(arguments[o++]);
-                            return bn(t, r, this, this, a)
+                            for (var i = 0, o = e.length, a = Array(o), u = 0; u < o; u++) a[u] = e[u] === n ? arguments[i++] : e[u];
+                            for (; i < arguments.length;) a.push(arguments[i++]);
+                            return _e(t, r, this, this, a)
                         };
                     return r
                 }));
-                jn.placeholder = st;
-                const wn = jn,
-                    An = x((function(t, n, e) {
+                be.placeholder = ct;
+                const je = be,
+                    we = x((function(t, e, n) {
                         if (!V(t)) throw new TypeError("Bind must be called on a function");
-                        var r = x((function(o) {
-                            return bn(t, r, n, this, e.concat(o))
+                        var r = x((function(i) {
+                            return _e(t, r, e, this, n.concat(i))
                         }));
                         return r
                     })),
-                    xn = Z(it);
+                    Ae = Z(ot);
 
-                function On(t, n, e, r) {
-                    if (r = r || [], n || 0 === n) {
-                        if (n <= 0) return r.concat(t)
-                    } else n = 1 / 0;
-                    for (var o = r.length, i = 0, a = it(t); i < a; i++) {
-                        var u = t[i];
-                        if (xn(u) && (K(u) || H(u)))
-                            if (n > 1) On(u, n - 1, e, r), o = r.length;
+                function xe(t, e, n, r) {
+                    if (r = r || [], e || 0 === e) {
+                        if (e <= 0) return r.concat(t)
+                    } else e = 1 / 0;
+                    for (var i = r.length, o = 0, a = ot(t); o < a; o++) {
+                        var u = t[o];
+                        if (Ae(u) && (K(u) || H(u)))
+                            if (e > 1) xe(u, e - 1, n, r), i = r.length;
                             else
-                                for (var l = 0, c = u.length; l < c;) r[o++] = u[l++];
-                        else e || (r[o++] = u)
+                                for (var l = 0, s = u.length; l < s;) r[i++] = u[l++];
+                        else n || (r[i++] = u)
                     }
                     return r
                 }
-                const Sn = x((function(t, n) {
-                    var e = (n = On(n, !1, !1)).length;
-                    if (e < 1) throw new Error("bindAll must be passed function names");
-                    for (; e--;) {
-                        var r = n[e];
-                        t[r] = An(t[r], t)
+                const Oe = x((function(t, e) {
+                    var n = (e = xe(e, !1, !1)).length;
+                    if (n < 1) throw new Error("bindAll must be passed function names");
+                    for (; n--;) {
+                        var r = e[n];
+                        t[r] = we(t[r], t)
                     }
                     return t
                 }));
 
-                function Mn(t, n) {
-                    var e = function(r) {
-                        var o = e.cache,
-                            i = "" + (n ? n.apply(this, arguments) : r);
-                        return J(o, i) || (o[i] = t.apply(this, arguments)), o[i]
+                function Se(t, e) {
+                    var n = function(r) {
+                        var i = n.cache,
+                            o = "" + (e ? e.apply(this, arguments) : r);
+                        return J(i, o) || (i[o] = t.apply(this, arguments)), i[o]
                     };
-                    return e.cache = {}, e
+                    return n.cache = {}, n
                 }
-                const En = x((function(t, n, e) {
+                const Me = x((function(t, e, n) {
                         return setTimeout((function() {
-                            return t.apply(null, e)
-                        }), n)
+                            return t.apply(null, n)
+                        }), e)
                     })),
-                    Tn = wn(En, st, 1);
+                    Ee = je(Me, ct, 1);
 
-                function In(t, n, e) {
-                    var r, o, i, a, u = 0;
-                    e || (e = {});
+                function Te(t, e, n) {
+                    var r, i, o, a, u = 0;
+                    n || (n = {});
                     var l = function() {
-                            u = !1 === e.leading ? 0 : rn(), r = null, a = t.apply(o, i), r || (o = i = null)
+                            u = !1 === n.leading ? 0 : re(), r = null, a = t.apply(i, o), r || (i = o = null)
                         },
-                        c = function() {
-                            var c = rn();
-                            u || !1 !== e.leading || (u = c);
-                            var s = n - (c - u);
-                            return o = this, i = arguments, s <= 0 || s > n ? (r && (clearTimeout(r), r = null), u = c, a = t.apply(o, i), r || (o = i = null)) : r || !1 === e.trailing || (r = setTimeout(l, s)), a
+                        s = function() {
+                            var s = re();
+                            u || !1 !== n.leading || (u = s);
+                            var c = e - (s - u);
+                            return i = this, o = arguments, c <= 0 || c > e ? (r && (clearTimeout(r), r = null), u = s, a = t.apply(i, o), r || (i = o = null)) : r || !1 === n.trailing || (r = setTimeout(l, c)), a
                         };
-                    return c.cancel = function() {
-                        clearTimeout(r), u = 0, r = o = i = null
-                    }, c
+                    return s.cancel = function() {
+                        clearTimeout(r), u = 0, r = i = o = null
+                    }, s
                 }
 
-                function Bn(t, n, e) {
-                    var r, o, i, a, u, l = function() {
-                            var c = rn() - o;
-                            n > c ? r = setTimeout(l, n - c) : (r = null, e || (a = t.apply(u, i)), r || (i = u = null))
+                function Ie(t, e, n) {
+                    var r, i, o, a, u, l = function() {
+                            var s = re() - i;
+                            e > s ? r = setTimeout(l, e - s) : (r = null, n || (a = t.apply(u, o)), r || (o = u = null))
                         },
-                        c = x((function(c) {
-                            return u = this, i = c, o = rn(), r || (r = setTimeout(l, n), e && (a = t.apply(u, i))), a
+                        s = x((function(s) {
+                            return u = this, o = s, i = re(), r || (r = setTimeout(l, e), n && (a = t.apply(u, o))), a
                         }));
-                    return c.cancel = function() {
-                        clearTimeout(r), r = i = u = null
-                    }, c
+                    return s.cancel = function() {
+                        clearTimeout(r), r = o = u = null
+                    }, s
                 }
 
-                function kn(t, n) {
-                    return wn(n, t)
+                function Be(t, e) {
+                    return je(e, t)
                 }
 
-                function Fn(t) {
+                function ke(t) {
                     return function() {
                         return !t.apply(this, arguments)
                     }
                 }
 
-                function Nn() {
+                function Fe() {
                     var t = arguments,
-                        n = t.length - 1;
+                        e = t.length - 1;
                     return function() {
-                        for (var e = n, r = t[n].apply(this, arguments); e--;) r = t[e].call(this, r);
+                        for (var n = e, r = t[e].apply(this, arguments); n--;) r = t[n].call(this, r);
                         return r
                     }
                 }
 
-                function Ln(t, n) {
+                function Ne(t, e) {
                     return function() {
-                        if (--t < 1) return n.apply(this, arguments)
+                        if (--t < 1) return e.apply(this, arguments)
                     }
                 }
 
-                function Rn(t, n) {
-                    var e;
+                function Le(t, e) {
+                    var n;
                     return function() {
-                        return --t > 0 && (e = n.apply(this, arguments)), t <= 1 && (n = null), e
+                        return --t > 0 && (n = e.apply(this, arguments)), t <= 1 && (e = null), n
                     }
                 }
-                const Cn = wn(Rn, 2);
+                const Re = je(Le, 2);
 
-                function Un(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r, o = ut(t), i = 0, a = o.length; i < a; i++)
-                        if (n(t[r = o[i]], r, t)) return r
+                function Ce(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r, i = ut(t), o = 0, a = i.length; o < a; o++)
+                        if (e(t[r = i[o]], r, t)) return r
                 }
 
-                function Dn(t) {
-                    return function(n, e, r) {
-                        e = Xt(e, r);
-                        for (var o = it(n), i = t > 0 ? 0 : o - 1; i >= 0 && i < o; i += t)
-                            if (e(n[i], i, n)) return i;
+                function Ue(t) {
+                    return function(e, n, r) {
+                        n = Xt(n, r);
+                        for (var i = ot(e), o = t > 0 ? 0 : i - 1; o >= 0 && o < i; o += t)
+                            if (n(e[o], o, e)) return o;
                         return -1
                     }
                 }
-                const Vn = Dn(1),
-                    Pn = Dn(-1);
+                const De = Ue(1),
+                    Ve = Ue(-1);
 
-                function qn(t, n, e, r) {
-                    for (var o = (e = Xt(e, r, 1))(n), i = 0, a = it(t); i < a;) {
-                        var u = Math.floor((i + a) / 2);
-                        e(t[u]) < o ? i = u + 1 : a = u
+                function Pe(t, e, n, r) {
+                    for (var i = (n = Xt(n, r, 1))(e), o = 0, a = ot(t); o < a;) {
+                        var u = Math.floor((o + a) / 2);
+                        n(t[u]) < i ? o = u + 1 : a = u
                     }
-                    return i
+                    return o
                 }
 
-                function Wn(t, n, e) {
-                    return function(r, o, i) {
+                function qe(t, e, n) {
+                    return function(r, i, o) {
                         var a = 0,
-                            u = it(r);
-                        if ("number" == typeof i) t > 0 ? a = i >= 0 ? i : Math.max(i + u, a) : u = i >= 0 ? Math.min(i + 1, u) : i + u + 1;
-                        else if (e && i && u) return r[i = e(r, o)] === o ? i : -1;
-                        if (o != o) return (i = n(s.call(r, a, u), X)) >= 0 ? i + a : -1;
-                        for (i = t > 0 ? a : u - 1; i >= 0 && i < u; i += t)
-                            if (r[i] === o) return i;
+                            u = ot(r);
+                        if ("number" == typeof o) t > 0 ? a = o >= 0 ? o : Math.max(o + u, a) : u = o >= 0 ? Math.min(o + 1, u) : o + u + 1;
+                        else if (n && o && u) return r[o = n(r, i)] === i ? o : -1;
+                        if (i != i) return (o = e(c.call(r, a, u), X)) >= 0 ? o + a : -1;
+                        for (o = t > 0 ? a : u - 1; o >= 0 && o < u; o += t)
+                            if (r[o] === i) return o;
                         return -1
                     }
                 }
-                const zn = Wn(1, Vn, qn),
-                    $n = Wn(-1, Pn);
+                const We = qe(1, De, Pe),
+                    ze = qe(-1, Ve);
 
-                function Kn(t, n, e) {
-                    var r = (xn(t) ? Vn : Un)(t, n, e);
+                function $e(t, e, n) {
+                    var r = (Ae(t) ? De : Ce)(t, e, n);
                     if (void 0 !== r && -1 !== r) return t[r]
                 }
 
-                function Jn(t, n) {
-                    return Kn(t, Kt(n))
+                function Ke(t, e) {
+                    return $e(t, Kt(e))
                 }
 
-                function Gn(t, n, e) {
-                    var r, o;
-                    if (n = Gt(n, e), xn(t))
-                        for (r = 0, o = t.length; r < o; r++) n(t[r], r, t);
+                function Je(t, e, n) {
+                    var r, i;
+                    if (e = Gt(e, n), Ae(t))
+                        for (r = 0, i = t.length; r < i; r++) e(t[r], r, t);
                     else {
-                        var i = ut(t);
-                        for (r = 0, o = i.length; r < o; r++) n(t[i[r]], i[r], t)
+                        var o = ut(t);
+                        for (r = 0, i = o.length; r < i; r++) e(t[o[r]], o[r], t)
                     }
                     return t
                 }
 
-                function Hn(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = Array(o), a = 0; a < o; a++) {
+                function Ge(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = Array(i), a = 0; a < i; a++) {
                         var u = r ? r[a] : a;
-                        i[a] = n(t[u], u, t)
+                        o[a] = e(t[u], u, t)
                     }
-                    return i
+                    return o
                 }
 
-                function Qn(t) {
-                    var n = function(n, e, r, o) {
-                        var i = !xn(n) && ut(n),
-                            a = (i || n).length,
-                            u = t > 0 ? 0 : a - 1;
-                        for (o || (r = n[i ? i[u] : u], u += t); u >= 0 && u < a; u += t) {
-                            var l = i ? i[u] : u;
-                            r = e(r, n[l], l, n)
-                        }
-                        return r
-                    };
-                    return function(t, e, r, o) {
-                        var i = arguments.length >= 3;
-                        return n(t, Gt(e, o, 4), r, i)
+                function He(t) {
+                    return function(e, n, r, i) {
+                        var o = arguments.length >= 3;
+                        return function(e, n, r, i) {
+                            var o = !Ae(e) && ut(e),
+                                a = (o || e).length,
+                                u = t > 0 ? 0 : a - 1;
+                            for (i || (r = e[o ? o[u] : u], u += t); u >= 0 && u < a; u += t) {
+                                var l = o ? o[u] : u;
+                                r = n(r, e[l], l, e)
+                            }
+                            return r
+                        }(e, Gt(n, i, 4), r, o)
                     }
                 }
-                const Xn = Qn(1),
-                    Yn = Qn(-1);
+                const Qe = He(1),
+                    Xe = He(-1);
 
-                function Zn(t, n, e) {
+                function Ye(t, e, n) {
                     var r = [];
-                    return n = Xt(n, e), Gn(t, (function(t, e, o) {
-                        n(t, e, o) && r.push(t)
+                    return e = Xt(e, n), Je(t, (function(t, n, i) {
+                        e(t, n, i) && r.push(t)
                     })), r
                 }
 
-                function te(t, n, e) {
-                    return Zn(t, Fn(Xt(n)), e)
+                function Ze(t, e, n) {
+                    return Ye(t, ke(Xt(e)), n)
                 }
 
-                function ne(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = 0; i < o; i++) {
-                        var a = r ? r[i] : i;
-                        if (!n(t[a], a, t)) return !1
+                function tn(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = 0; o < i; o++) {
+                        var a = r ? r[o] : o;
+                        if (!e(t[a], a, t)) return !1
                     }
                     return !0
                 }
 
-                function ee(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = 0; i < o; i++) {
-                        var a = r ? r[i] : i;
-                        if (n(t[a], a, t)) return !0
+                function en(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = 0; o < i; o++) {
+                        var a = r ? r[o] : o;
+                        if (e(t[a], a, t)) return !0
                     }
                     return !1
                 }
 
-                function re(t, n, e, r) {
-                    return xn(t) || (t = Et(t)), ("number" != typeof e || r) && (e = 0), zn(t, n, e) >= 0
+                function nn(t, e, n, r) {
+                    return Ae(t) || (t = Et(t)), ("number" != typeof n || r) && (n = 0), We(t, e, n) >= 0
                 }
-                const oe = x((function(t, n, e) {
-                    var r, o;
-                    return V(n) ? o = n : (n = Pt(n), r = n.slice(0, -1), n = n[n.length - 1]), Hn(t, (function(t) {
-                        var i = o;
-                        if (!i) {
+                const rn = x((function(t, e, n) {
+                    var r, i;
+                    return V(e) ? i = e : (e = Pt(e), r = e.slice(0, -1), e = e[e.length - 1]), Ge(t, (function(t) {
+                        var o = i;
+                        if (!o) {
                             if (r && r.length && (t = qt(t, r)), null == t) return;
-                            i = t[n]
+                            o = t[e]
                         }
-                        return null == i ? i : i.apply(t, e)
+                        return null == o ? o : o.apply(t, n)
                     }))
                 }));
 
-                function ie(t, n) {
-                    return Hn(t, Jt(n))
+                function on(t, e) {
+                    return Ge(t, Jt(e))
                 }
 
-                function ae(t, n) {
-                    return Zn(t, Kt(n))
+                function an(t, e) {
+                    return Ye(t, Kt(e))
                 }
 
-                function ue(t, n, e) {
-                    var r, o, i = -1 / 0,
+                function un(t, e, n) {
+                    var r, i, o = -1 / 0,
                         a = -1 / 0;
-                    if (null == n || "number" == typeof n && "object" != typeof t[0] && null != t)
-                        for (var u = 0, l = (t = xn(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r > i && (i = r);
-                    else n = Xt(n, e), Gn(t, (function(t, e, r) {
-                        ((o = n(t, e, r)) > a || o === -1 / 0 && i === -1 / 0) && (i = t, a = o)
+                    if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
+                        for (var u = 0, l = (t = Ae(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r > o && (o = r);
+                    else e = Xt(e, n), Je(t, (function(t, n, r) {
+                        ((i = e(t, n, r)) > a || i === -1 / 0 && o === -1 / 0) && (o = t, a = i)
                     }));
-                    return i
+                    return o
                 }
 
-                function le(t, n, e) {
-                    var r, o, i = 1 / 0,
+                function ln(t, e, n) {
+                    var r, i, o = 1 / 0,
                         a = 1 / 0;
-                    if (null == n || "number" == typeof n && "object" != typeof t[0] && null != t)
-                        for (var u = 0, l = (t = xn(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r < i && (i = r);
-                    else n = Xt(n, e), Gn(t, (function(t, e, r) {
-                        ((o = n(t, e, r)) < a || o === 1 / 0 && i === 1 / 0) && (i = t, a = o)
+                    if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
+                        for (var u = 0, l = (t = Ae(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r < o && (o = r);
+                    else e = Xt(e, n), Je(t, (function(t, n, r) {
+                        ((i = e(t, n, r)) < a || i === 1 / 0 && o === 1 / 0) && (o = t, a = i)
                     }));
-                    return i
+                    return o
                 }
-                var ce = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
+                var sn = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
 
-                function se(t) {
-                    return t ? K(t) ? s.call(t) : B(t) ? t.match(ce) : xn(t) ? Hn(t, $t) : Et(t) : []
+                function cn(t) {
+                    return t ? K(t) ? c.call(t) : B(t) ? t.match(sn) : Ae(t) ? Ge(t, $t) : Et(t) : []
                 }
 
-                function fe(t, n, e) {
-                    if (null == n || e) return xn(t) || (t = Et(t)), t[en(t.length - 1)];
-                    var r = se(t),
-                        o = it(r);
-                    n = Math.max(Math.min(n, o), 0);
-                    for (var i = o - 1, a = 0; a < n; a++) {
-                        var u = en(a, i),
+                function fn(t, e, n) {
+                    if (null == e || n) return Ae(t) || (t = Et(t)), t[ne(t.length - 1)];
+                    var r = cn(t),
+                        i = ot(r);
+                    e = Math.max(Math.min(e, i), 0);
+                    for (var o = i - 1, a = 0; a < e; a++) {
+                        var u = ne(a, o),
                             l = r[a];
                         r[a] = r[u], r[u] = l
                     }
-                    return r.slice(0, n)
+                    return r.slice(0, e)
                 }
 
-                function pe(t) {
-                    return fe(t, 1 / 0)
+                function hn(t) {
+                    return fn(t, 1 / 0)
                 }
 
-                function he(t, n, e) {
+                function pn(t, e, n) {
                     var r = 0;
-                    return n = Xt(n, e), ie(Hn(t, (function(t, e, o) {
+                    return e = Xt(e, n), on(Ge(t, (function(t, n, i) {
                         return {
                             value: t,
                             index: r++,
-                            criteria: n(t, e, o)
+                            criteria: e(t, n, i)
                         }
-                    })).sort((function(t, n) {
-                        var e = t.criteria,
-                            r = n.criteria;
-                        if (e !== r) {
-                            if (e > r || void 0 === e) return 1;
-                            if (e < r || void 0 === r) return -1
+                    })).sort((function(t, e) {
+                        var n = t.criteria,
+                            r = e.criteria;
+                        if (n !== r) {
+                            if (n > r || void 0 === n) return 1;
+                            if (n < r || void 0 === r) return -1
                         }
-                        return t.index - n.index
+                        return t.index - e.index
                     })), "value")
                 }
 
-                function de(t, n) {
-                    return function(e, r, o) {
-                        var i = n ? [
+                function dn(t, e) {
+                    return function(n, r, i) {
+                        var o = e ? [
                             [],
                             []
                         ] : {};
-                        return r = Xt(r, o), Gn(e, (function(n, o) {
-                            var a = r(n, o, e);
-                            t(i, n, a)
-                        })), i
+                        return r = Xt(r, i), Je(n, (function(e, i) {
+                            var a = r(e, i, n);
+                            t(o, e, a)
+                        })), o
                     }
                 }
-                const ve = de((function(t, n, e) {
-                        J(t, e) ? t[e].push(n) : t[e] = [n]
+                const vn = dn((function(t, e, n) {
+                        J(t, n) ? t[n].push(e) : t[n] = [e]
                     })),
-                    ge = de((function(t, n, e) {
-                        t[e] = n
+                    gn = dn((function(t, e, n) {
+                        t[n] = e
                     })),
-                    ye = de((function(t, n, e) {
-                        J(t, e) ? t[e]++ : t[e] = 1
+                    mn = dn((function(t, e, n) {
+                        J(t, n) ? t[n]++ : t[n] = 1
                     })),
-                    me = de((function(t, n, e) {
-                        t[e ? 0 : 1].push(n)
+                    yn = dn((function(t, e, n) {
+                        t[n ? 0 : 1].push(e)
                     }), !0);
 
-                function _e(t) {
-                    return null == t ? 0 : xn(t) ? t.length : ut(t).length
+                function _n(t) {
+                    return null == t ? 0 : Ae(t) ? t.length : ut(t).length
                 }
 
-                function be(t, n, e) {
-                    return n in e
+                function bn(t, e, n) {
+                    return e in n
                 }
-                const je = x((function(t, n) {
-                        var e = {},
-                            r = n[0];
-                        if (null == t) return e;
-                        V(r) ? (n.length > 1 && (r = Gt(r, n[1])), n = gt(t)) : (r = be, n = On(n, !1, !1), t = Object(t));
-                        for (var o = 0, i = n.length; o < i; o++) {
-                            var a = n[o],
+                const jn = x((function(t, e) {
+                        var n = {},
+                            r = e[0];
+                        if (null == t) return n;
+                        V(r) ? (e.length > 1 && (r = Gt(r, e[1])), e = gt(t)) : (r = bn, e = xe(e, !1, !1), t = Object(t));
+                        for (var i = 0, o = e.length; i < o; i++) {
+                            var a = e[i],
                                 u = t[a];
-                            r(u, a, t) && (e[a] = u)
+                            r(u, a, t) && (n[a] = u)
                         }
-                        return e
+                        return n
                     })),
-                    we = x((function(t, n) {
-                        var e, r = n[0];
-                        return V(r) ? (r = Fn(r), n.length > 1 && (e = n[1])) : (n = Hn(On(n, !1, !1), String), r = function(t, e) {
-                            return !re(n, e)
-                        }), je(t, r, e)
+                    wn = x((function(t, e) {
+                        var n, r = e[0];
+                        return V(r) ? (r = ke(r), e.length > 1 && (n = e[1])) : (e = Ge(xe(e, !1, !1), String), r = function(t, n) {
+                            return !nn(e, n)
+                        }), jn(t, r, n)
                     }));
 
-                function Ae(t, n, e) {
-                    return s.call(t, 0, Math.max(0, t.length - (null == n || e ? 1 : n)))
+                function An(t, e, n) {
+                    return c.call(t, 0, Math.max(0, t.length - (null == e || n ? 1 : e)))
                 }
 
-                function xe(t, n, e) {
-                    return null == t || t.length < 1 ? null == n || e ? void 0 : [] : null == n || e ? t[0] : Ae(t, t.length - n)
+                function xn(t, e, n) {
+                    return null == t || t.length < 1 ? null == e || n ? void 0 : [] : null == e || n ? t[0] : An(t, t.length - e)
                 }
 
-                function Oe(t, n, e) {
-                    return s.call(t, null == n || e ? 1 : n)
+                function On(t, e, n) {
+                    return c.call(t, null == e || n ? 1 : e)
                 }
 
-                function Se(t, n, e) {
-                    return null == t || t.length < 1 ? null == n || e ? void 0 : [] : null == n || e ? t[t.length - 1] : Oe(t, Math.max(0, t.length - n))
+                function Sn(t, e, n) {
+                    return null == t || t.length < 1 ? null == e || n ? void 0 : [] : null == e || n ? t[t.length - 1] : On(t, Math.max(0, t.length - e))
                 }
 
-                function Me(t) {
-                    return Zn(t, Boolean)
+                function Mn(t) {
+                    return Ye(t, Boolean)
                 }
 
-                function Ee(t, n) {
-                    return On(t, n, !1)
+                function En(t, e) {
+                    return xe(t, e, !1)
                 }
-                const Te = x((function(t, n) {
-                        return n = On(n, !0, !0), Zn(t, (function(t) {
-                            return !re(n, t)
+                const Tn = x((function(t, e) {
+                        return e = xe(e, !0, !0), Ye(t, (function(t) {
+                            return !nn(e, t)
                         }))
                     })),
-                    Ie = x((function(t, n) {
-                        return Te(t, n)
+                    In = x((function(t, e) {
+                        return Tn(t, e)
                     }));
 
-                function Be(t, n, e, r) {
-                    E(n) || (r = e, e = n, n = !1), null != e && (e = Xt(e, r));
-                    for (var o = [], i = [], a = 0, u = it(t); a < u; a++) {
+                function Bn(t, e, n, r) {
+                    E(e) || (r = n, n = e, e = !1), null != n && (n = Xt(n, r));
+                    for (var i = [], o = [], a = 0, u = ot(t); a < u; a++) {
                         var l = t[a],
-                            c = e ? e(l, a, t) : l;
-                        n && !e ? (a && i === c || o.push(l), i = c) : e ? re(i, c) || (i.push(c), o.push(l)) : re(o, l) || o.push(l)
+                            s = n ? n(l, a, t) : l;
+                        e && !n ? (a && o === s || i.push(l), o = s) : n ? nn(o, s) || (o.push(s), i.push(l)) : nn(i, l) || i.push(l)
                     }
-                    return o
+                    return i
                 }
-                const ke = x((function(t) {
-                    return Be(On(t, !0, !0))
+                const kn = x((function(t) {
+                    return Bn(xe(t, !0, !0))
                 }));
 
-                function Fe(t) {
-                    for (var n = [], e = arguments.length, r = 0, o = it(t); r < o; r++) {
-                        var i = t[r];
-                        if (!re(n, i)) {
+                function Fn(t) {
+                    for (var e = [], n = arguments.length, r = 0, i = ot(t); r < i; r++) {
+                        var o = t[r];
+                        if (!nn(e, o)) {
                             var a;
-                            for (a = 1; a < e && re(arguments[a], i); a++);
-                            a === e && n.push(i)
+                            for (a = 1; a < n && nn(arguments[a], o); a++);
+                            a === n && e.push(o)
                         }
                     }
-                    return n
+                    return e
                 }
 
-                function Ne(t) {
-                    for (var n = t && ue(t, it).length || 0, e = Array(n), r = 0; r < n; r++) e[r] = ie(t, r);
-                    return e
+                function Nn(t) {
+                    for (var e = t && un(t, ot).length || 0, n = Array(e), r = 0; r < e; r++) n[r] = on(t, r);
+                    return n
                 }
-                const Le = x(Ne);
+                const Ln = x(Nn);
 
-                function Re(t, n) {
-                    for (var e = {}, r = 0, o = it(t); r < o; r++) n ? e[t[r]] = n[r] : e[t[r][0]] = t[r][1];
-                    return e
+                function Rn(t, e) {
+                    for (var n = {}, r = 0, i = ot(t); r < i; r++) e ? n[t[r]] = e[r] : n[t[r][0]] = t[r][1];
+                    return n
                 }
 
-                function Ce(t, n, e) {
-                    null == n && (n = t || 0, t = 0), e || (e = n < t ? -1 : 1);
-                    for (var r = Math.max(Math.ceil((n - t) / e), 0), o = Array(r), i = 0; i < r; i++, t += e) o[i] = t;
-                    return o
+                function Cn(t, e, n) {
+                    null == e && (e = t || 0, t = 0), n || (n = e < t ? -1 : 1);
+                    for (var r = Math.max(Math.ceil((e - t) / n), 0), i = Array(r), o = 0; o < r; o++, t += n) i[o] = t;
+                    return i
                 }
 
-                function Ue(t, n) {
-                    if (null == n || n < 1) return [];
-                    for (var e = [], r = 0, o = t.length; r < o;) e.push(s.call(t, r, r += n));
-                    return e
+                function Un(t, e) {
+                    if (null == e || e < 1) return [];
+                    for (var n = [], r = 0, i = t.length; r < i;) n.push(c.call(t, r, r += e));
+                    return n
                 }
 
-                function De(t, n) {
-                    return t._chain ? st(n).chain() : n
+                function Dn(t, e) {
+                    return t._chain ? ct(e).chain() : e
                 }
 
-                function Ve(t) {
-                    return Gn(Bt(t), (function(n) {
-                        var e = st[n] = t[n];
-                        st.prototype[n] = function() {
+                function Vn(t) {
+                    return Je(Bt(t), (function(e) {
+                        var n = ct[e] = t[e];
+                        ct.prototype[e] = function() {
                             var t = [this._wrapped];
-                            return c.apply(t, arguments), De(this, e.apply(st, t))
+                            return s.apply(t, arguments), Dn(this, n.apply(ct, t))
                         }
-                    })), st
+                    })), ct
                 }
-                Gn(["pop", "push", "reverse", "shift", "sort", "splice", "unshift"], (function(t) {
-                    var n = a[t];
-                    st.prototype[t] = function() {
-                        var e = this._wrapped;
-                        return null != e && (n.apply(e, arguments), "shift" !== t && "splice" !== t || 0 !== e.length || delete e[0]), De(this, e)
-                    }
-                })), Gn(["concat", "join", "slice"], (function(t) {
-                    var n = a[t];
-                    st.prototype[t] = function() {
+                Je(["pop", "push", "reverse", "shift", "sort", "splice", "unshift"], (function(t) {
+                    var e = a[t];
+                    ct.prototype[t] = function() {
+                        var n = this._wrapped;
+                        return null != n && (e.apply(n, arguments), "shift" !== t && "splice" !== t || 0 !== n.length || delete n[0]), Dn(this, n)
+                    }
+                })), Je(["concat", "join", "slice"], (function(t) {
+                    var e = a[t];
+                    ct.prototype[t] = function() {
                         var t = this._wrapped;
-                        return null != t && (t = n.apply(t, arguments)), De(this, t)
+                        return null != t && (t = e.apply(t, arguments)), Dn(this, t)
                     }
                 }));
-                const Pe = st;
-                var qe = Ve(r);
-                qe._ = qe;
-                const We = qe
+                const Pn = ct;
+                var qn = Vn(r);
+                qn._ = qn;
+                const Wn = qn
             }
         },
         r = {};
 
-    function o(t) {
-        var n = r[t];
-        if (void 0 !== n) return n.exports;
-        var i = r[t] = {
+    function i(t) {
+        var e = r[t];
+        if (void 0 !== e) return e.exports;
+        var o = r[t] = {
             exports: {}
         };
-        return e[t](i, i.exports, o), i.exports
+        return n[t](o, o.exports, i), o.exports
     }
-    o.n = t => {
-        var n = t && t.__esModule ? () => t.default : () => t;
-        return o.d(n, {
-            a: n
-        }), n
-    }, o.d = (t, n) => {
-        for (var e in n) o.o(n, e) && !o.o(t, e) && Object.defineProperty(t, e, {
+    i.n = t => {
+        var e = t && t.__esModule ? () => t.default : () => t;
+        return i.d(e, {
+            a: e
+        }), e
+    }, i.d = (t, e) => {
+        for (var n in e) i.o(e, n) && !i.o(t, n) && Object.defineProperty(t, n, {
             enumerable: !0,
-            get: n[e]
+            get: e[n]
         })
-    }, o.o = (t, n) => Object.prototype.hasOwnProperty.call(t, n), o.r = t => {
+    }, i.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), i.r = t => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(t, "__esModule", {
             value: !0
         })
-    }, o.p = "";
-    var i = {};
+    }, i.p = "";
+    var o = {};
     return (() => {
-        var t = o(325);
-        const n = new URL(t.uri, document.location);
-        n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), o.p = `${n.origin}${n.pathname}`
+        var t = i(325);
+        const e = new URL(t.uri, document.location);
+        e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
-        o.r(i), o.d(i, {
+        i.r(o), i.d(o, {
             AladinModel: () => r,
             AladinView: () => u,
             version: () => l.i8
         });
-        var t = o(146);
-        o(50);
-        const n = (t, n = !0, e = "text/javascript") => new Promise(((r, o) => {
+        var t = i(146);
+        i(50);
+        const e = (t, e = !0, n = "text/javascript") => new Promise(((r, i) => {
             try {
-                const i = document.createElement("script");
-                i.type = e, i.async = n, i.src = t, i.addEventListener("load", (t => {
+                const o = document.createElement("script");
+                o.type = n, o.async = e, o.src = t, o.addEventListener("load", (t => {
                     r({
                         status: !0
                     })
-                })), i.addEventListener("error", (t => {
-                    o({
+                })), o.addEventListener("error", (t => {
+                    i({
                         status: !1,
                         message: "Failed to load the script ＄{FILE_URL}"
                     })
-                })), document.getElementsByTagName("head")[0].appendChild(i)
+                })), document.getElementsByTagName("head")[0].appendChild(o)
             } catch (t) {
-                o(t)
+                i(t)
             }
         }));
-        var e = n("https://code.jquery.com/jquery-3.6.1.min.js").then((() => n("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
+        let n = e("https://code.jquery.com/jquery-3.6.1.min.js").then((() => e("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
             await A.init
         }));
         class r extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.1",
-                    _view_module_version: "0.2.1"
+                    _model_module_version: "0.2.2",
+                    _view_module_version: "0.2.2"
                 }
             }
         }
-        var a = 0;
+        let a = 0;
         class u extends t.DOMWidgetView {
             render() {
-                e.then((() => {
-                    this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(a), a += 1, this.div.setAttribute("style", "width:100%;height:400px;");
-                    for (var t = {}, n = this.model.get("options"), e = 0; e < n.length; e++) t[this.convert_pyname_to_jsname(n[e])] = this.model.get(n[e]);
-                    new MutationObserver((n => {
-                        n.forEach((n => {
-                            n.addedNodes.forEach((n => {
-                                n.id == this.div.id && setTimeout((() => {
-                                    this.al = A.aladin([this.div], t), this.aladin_events(), this.model_events()
+                n.then((() => {
+                    this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(a), a += 1;
+                    let t = this.model.get("height");
+                    this.div.setAttribute("style", "width:100%;height:" + t + "px;");
+                    let e = {},
+                        n = this.model.get("options");
+                    for (let t of n) e[this.convert_pyname_to_jsname(t)] = this.model.get(t);
+                    new MutationObserver((t => {
+                        t.forEach((t => {
+                            t.addedNodes.forEach((t => {
+                                t.id == this.div.id && setTimeout((() => {
+                                    this.al = A.aladin([this.div], e), this.aladin_events(), this.model_events()
                                 }), 1e3)
                             }))
                         }))
                     })).observe(this.el, {
                         subtree: !1,
                         childList: !0
                     }), this.el.appendChild(this.div)
                 }))
             }
             convert_pyname_to_jsname(t) {
-                var n, e = t.split("_");
-                for (n = 1; n < e.length; n++) e[n] = e[n].charAt(0).toUpperCase() + e[n].slice(1);
+                let e = t.split("_");
+                for (let t = 1; t < e.length; t++) e[t] = e[t].charAt(0).toUpperCase() + e[t].slice(1);
                 return e.join("")
             }
             aladin_events() {
-                var t = this;
-                this.al.on("zoomChanged", (function(n) {
-                    t.fov_py ? t.fov_py = !1 : (t.fov_js = !0, t.model.set("fov", parseFloat(n.toFixed(5))), t.touch())
-                })), this.al.on("positionChanged", (function(n) {
-                    t.target_py ? t.target_py = !1 : (t.target_js = !0, t.model.set("target", n.ra.toFixed(6) + " " + n.dec.toFixed(6)), t.touch())
+                this.al.on("zoomChanged", (t => {
+                    this.fov_py ? this.fov_py = !1 : (this.fov_js = !0, this.model.set("fov", parseFloat(t.toFixed(5))), this.touch())
+                })), this.al.on("positionChanged", (t => {
+                    this.target_py ? this.target_py = !1 : (this.target_js = !0, this.model.set("target", t.ra.toFixed(6) + " " + t.dec.toFixed(6)), this.touch())
                 }))
             }
             model_events() {
-                var t = this;
-                this.listenTo(this.model, "change:fov", (function() {
-                    t.fov_js ? t.fov_js = !1 : (t.fov_py = !0, t.al.setFoV(t.model.get("fov")))
-                }), this), this.listenTo(this.model, "change:target", (function() {
-                    t.target_js ? t.target_js = !1 : (t.target_py = !0, t.al.gotoObject(t.model.get("target")))
-                }), this), this.listenTo(this.model, "change:coo_frame", (function() {
-                    t.al.setFrame(t.model.get("coo_frame"))
-                }), this), this.listenTo(this.model, "change:survey", (function() {
-                    t.al.setImageSurvey(t.model.get("survey"))
-                }), this), this.listenTo(this.model, "change:overlay_survey", (function() {
-                    t.al.setOverlayImageLayer(t.model.get("overlay_survey"))
-                }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (function() {
-                    t.al.getOverlayImageLayer().setAlpha(t.model.get("overlay_survey_opacity"))
-                }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (function() {
-                    t.al.addCatalog(A.catalogFromURL(t.model.get("votable_URL"), t.model.get("votable_options")))
-                }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (function() {
-                    t.al.addMOC(A.MOCFromURL(t.model.get("moc_URL"), t.model.get("moc_options")))
-                }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (function() {
-                    t.al.addMOC(A.MOCFromJSON(t.model.get("moc_dict"), t.model.get("moc_options")))
-                }), this), this.listenTo(this.model, "change:table_flag", (function() {
-                    var n = A.catalog({
+                this.listenTo(this.model, "change:fov", (() => {
+                    this.fov_js ? this.fov_js = !1 : (this.fov_py = !0, this.al.setFoV(this.model.get("fov")))
+                }), this), this.listenTo(this.model, "change:target", (() => {
+                    this.target_js ? this.target_js = !1 : (this.target_py = !0, this.al.gotoObject(this.model.get("target")))
+                }), this), this.listenTo(this.model, "change:coo_frame", (() => {
+                    this.al.setFrame(this.model.get("coo_frame"))
+                }), this), this.listenTo(this.model, "change:height", (() => {
+                    let t = this.model.get("height");
+                    this.div.setAttribute("style", "width:100%;height:" + t + "px;")
+                }), this), this.listenTo(this.model, "change:survey", (() => {
+                    this.al.setImageSurvey(this.model.get("survey"))
+                }), this), this.listenTo(this.model, "change:overlay_survey", (() => {
+                    this.al.setOverlayImageLayer(this.model.get("overlay_survey"))
+                }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (() => {
+                    this.al.getOverlayImageLayer().setAlpha(this.model.get("overlay_survey_opacity"))
+                }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (() => {
+                    this.al.addCatalog(A.catalogFromURL(this.model.get("votable_URL"), this.model.get("votable_options")))
+                }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (() => {
+                    this.al.addMOC(A.MOCFromURL(this.model.get("moc_URL"), this.model.get("moc_options")))
+                }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (() => {
+                    this.al.addMOC(A.MOCFromJSON(this.model.get("moc_dict"), this.model.get("moc_options")))
+                }), this), this.listenTo(this.model, "change:table_flag", (() => {
+                    let t = A.catalog({
                         onClick: "showTable"
                     });
-                    t.al.addCatalog(n), n.addSourcesAsArray(t.model.get("table_keys"), t.model.get("table_columns"))
-                }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (function() {
-                    var n = A.graphicOverlay(t.model.get("overlay_options"));
-                    t.al.addOverlay(n), n.addFootprints(A.footprintsFromSTCS(t.model.get("stc_string")))
-                }), this), this.listenTo(this.model, "change:listener_flag", (function() {
-                    var n = t.model.get("listener_type");
-                    t.al.on(n, (function(e) {
-                        if ("select" !== n) e && t.send({
+                    this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
+                }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
+                    let t = A.graphicOverlay(this.model.get("overlay_options"));
+                    this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
+                }), this), this.listenTo(this.model, "change:listener_flag", (() => {
+                    let t = this.model.get("listener_type");
+                    this.al.on(t, (function(e) {
+                        if ("select" !== t) e && this.send({
                             event: "callback",
-                            type: n,
+                            type: t,
                             data: {
                                 data: e.data,
                                 dec: e.dec,
                                 ra: e.ra,
                                 x: e.x,
                                 y: e.y
                             }
                         });
                         else {
-                            for (var r = e, o = 0; o < t.al.view.catalogs.length; o++) t.al.view.catalogs[o].deselectAll();
-                            var i = [];
-                            for (o = 0; o < r.length; o++) {
-                                var a = r[o];
-                                a.select(), i.push({
-                                    data: a.data,
-                                    dec: a.dec,
-                                    ra: a.ra,
-                                    x: a.x,
-                                    y: a.y
-                                })
-                            }
-                            t.send({
+                            let n = e;
+                            for (let t of this.al.view.catalogs) t.deselectAll();
+                            let r = [];
+                            for (let t of n) t.select(), r.push({
+                                data: t.data,
+                                dec: t.dec,
+                                ra: t.ra,
+                                x: t.x,
+                                y: t.y
+                            });
+                            this.send({
                                 event: "callback",
-                                type: n,
-                                data: i
+                                type: t,
+                                data: r
                             })
                         }
                     }))
-                }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (function() {
-                    t.al.select()
-                })), this.listenTo(this.model, "change:thumbnail_flag", (function() {
-                    t.al.exportAsPNG()
-                })), this.listenTo(this.model, "change:color_map_flag", (function() {
-                    const n = t.model.get("color_map_name");
-                    t.al.getBaseImageLayer().setColormap(n)
+                }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (() => {
+                    this.al.select()
+                })), this.listenTo(this.model, "change:thumbnail_flag", (() => {
+                    this.al.exportAsPNG()
+                })), this.listenTo(this.model, "change:color_map_flag", (() => {
+                    const t = this.model.get("color_map_name");
+                    this.al.getBaseImageLayer().setColormap(t)
                 }))
             }
         }
         const l = {
-            i8: "0.2.1"
+            i8: "0.2.2"
         }
-    })(), i
+    })(), o
 })()));
```

### Comparing `ipyaladin-0.2.1/ipyaladin.egg-info/PKG-INFO` & `ipyaladin-0.2.2/ipyaladin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.1
+Version: 0.2.2
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -30,67 +30,79 @@
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ipyaladin
 
-## Description
-
 A bridge between Jupyter and Aladin Lite, enabling interactive sky visualization in IPython notebooks.
-
-![ipyaladin example](ipyaladin-screenshot.png)
-
 With a couple of lines, you can display Aladin Lite, center it on the target of your choice, and overlay an Astropy table:
 
-![ipyaladin example](ipyaladin-screencast.gif)
+![ipyaladin example](assets/ipyaladin-screencast.gif)
+
+- [ipyaladin](#ipyaladin)
+  - [Examples](#examples)
+  - [Installation](#installation)
+  - [New features corner](#new-features-corner)
+  - [Development installation](#development-installation)
 
 ## Examples
 
 Some example notebooks can be found in the [examples directory](examples).
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master). You can also try it directly [in mybinder](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master), without installing anything.
 
 ## Installation
 
 To install use pip:
 
-    $ pip install ipyaladin
+    pip install ipyaladin
 
 Then, make sure to enable widgetsnbextension:
 
-    $ jupyter nbextension enable --py widgetsnbextension
+    jupyter nbextension enable --py widgetsnbextension
 
 Finally, enable ipyaladin:
 
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
-    $ jupyter labextension develop ipyaladin --overwrite
+    jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    $  conda install -c bmatthieu3 ipyaladin==0.2.1
+    conda install -c bmatthieu3 ipyaladin==0.2.2
+
+## New features corner
+
+![new_features](assets/new_features.gif)
+
+## Development installation
 
-## Development
+First, make sure you have installed jupyter on your python environnement: `pip install jupyter`.
+For a development installation [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/) are also required,
 
-For a development installation (requires [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/)),
+    git clone https://github.com/cds-astro/ipyaladin.git
+    cd ipyaladin
+    npm install yarn
+    cd js
+    npm install
+    cd ..
+    pip install -e .
 
-    $ git clone https://github.com/cds-astro/ipyaladin.git
-    $ cd ipyaladin
-    $ npm install yarn
-    $ pip install -e .
-    $ jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
-    $ jupyter nbextension enable --py --sys-prefix ipyaladin
+For Jupyter Notebook, do
+ 
+    jupyter nbextension install --py --symlink --overwrite --sys-prefix ipyaladin
+    jupyter nbextension enable --py --sys-prefix ipyaladin
 
-When actively developing your extension for JupyterLab, you will need to run this command too:
+For JupyterLab, you will need to run this command too:
 
-    $ jupyter labextension develop --overwrite ipyaladin
+    jupyter labextension develop --overwrite ipyaladin
 
 Then you need to rebuild the JS when you make a code change:
 
-    $ cd js
-    $ yarn run build
+    cd js
+    yarn run build
 
 You then need to refresh the JupyterLab page when your javascript changes.
```

### Comparing `ipyaladin-0.2.1/ipyaladin.egg-info/SOURCES.txt` & `ipyaladin-0.2.2/ipyaladin.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 ipyaladin.egg-info/PKG-INFO
 ipyaladin.egg-info/SOURCES.txt
 ipyaladin.egg-info/dependency_links.txt
 ipyaladin.egg-info/not-zip-safe
 ipyaladin.egg-info/requires.txt
 ipyaladin.egg-info/top_level.txt
 ipyaladin/labextension/package.json
-ipyaladin/labextension/static/261.bfcaf0ae589773f941db.js
-ipyaladin/labextension/static/678.54afe962dae4bf9693fa.js
-ipyaladin/labextension/static/794.6f96ca96639b4fa21dce.js
-ipyaladin/labextension/static/remoteEntry.f2d6e628bd28c3f3b3b7.js
+ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js
+ipyaladin/labextension/static/590.9292295778c3653a0b31.js
+ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
+ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js
 ipyaladin/labextension/static/style.js
 ipyaladin/labextension/static/third-party-licenses.json
 ipyaladin/nbextension/extension.js
 ipyaladin/nbextension/index.js
 js/README.md
 js/amd-public-path.js
-js/package-lock.json
 js/package.json
 js/webpack.config.js
+js/yarn.lock
 js/dist/index.js
 js/lib/extension.js
 js/lib/index.js
 js/lib/jupyter-aladin.js
 js/lib/labplugin.js
```

### Comparing `ipyaladin-0.2.1/js/amd-public-path.js` & `ipyaladin-0.2.2/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/js/dist/index.js` & `ipyaladin-0.2.2/js/dist/index.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,358 +1,358 @@
-define(["module", "@jupyter-widgets/base"], ((t, n) => (() => {
+define(["module", "@jupyter-widgets/base"], ((t, e) => (() => {
     "use strict";
-    var e = {
+    var n = {
             146: t => {
-                t.exports = n
+                t.exports = e
             },
-            325: n => {
-                n.exports = t
+            325: e => {
+                e.exports = t
             },
-            50: (t, n, e) => {
-                e.r(n), e.d(n, {
-                    VERSION: () => o,
-                    after: () => Ln,
-                    all: () => ne,
+            50: (t, e, n) => {
+                n.r(e), n.d(e, {
+                    VERSION: () => i,
+                    after: () => Ne,
+                    all: () => tn,
                     allKeys: () => gt,
-                    any: () => ee,
+                    any: () => en,
                     assign: () => Nt,
-                    before: () => Rn,
-                    bind: () => An,
-                    bindAll: () => Sn,
-                    chain: () => _n,
-                    chunk: () => Ue,
+                    before: () => Le,
+                    bind: () => we,
+                    bindAll: () => Oe,
+                    chain: () => ye,
+                    chunk: () => Un,
                     clone: () => Ut,
-                    collect: () => Hn,
-                    compact: () => Me,
-                    compose: () => Nn,
+                    collect: () => Ge,
+                    compact: () => Mn,
+                    compose: () => Fe,
                     constant: () => Y,
-                    contains: () => re,
-                    countBy: () => ye,
+                    contains: () => nn,
+                    countBy: () => mn,
                     create: () => Ct,
-                    debounce: () => Bn,
-                    default: () => We,
+                    debounce: () => Ie,
+                    default: () => Wn,
                     defaults: () => Lt,
-                    defer: () => Tn,
-                    delay: () => En,
-                    detect: () => Kn,
-                    difference: () => Te,
-                    drop: () => Oe,
-                    each: () => Gn,
-                    escape: () => un,
-                    every: () => ne,
+                    defer: () => Ee,
+                    delay: () => Me,
+                    detect: () => $e,
+                    difference: () => Tn,
+                    drop: () => On,
+                    each: () => Je,
+                    escape: () => ae,
+                    every: () => tn,
                     extend: () => Ft,
                     extendOwn: () => Nt,
-                    filter: () => Zn,
-                    find: () => Kn,
-                    findIndex: () => Vn,
-                    findKey: () => Un,
-                    findLastIndex: () => Pn,
-                    findWhere: () => Jn,
-                    first: () => xe,
-                    flatten: () => Ee,
-                    foldl: () => Xn,
-                    foldr: () => Yn,
-                    forEach: () => Gn,
+                    filter: () => Ye,
+                    find: () => $e,
+                    findIndex: () => De,
+                    findKey: () => Ce,
+                    findLastIndex: () => Ve,
+                    findWhere: () => Ke,
+                    first: () => xn,
+                    flatten: () => En,
+                    foldl: () => Qe,
+                    foldr: () => Xe,
+                    forEach: () => Je,
                     functions: () => Bt,
                     get: () => Wt,
-                    groupBy: () => ve,
+                    groupBy: () => vn,
                     has: () => zt,
-                    head: () => xe,
+                    head: () => xn,
                     identity: () => $t,
-                    include: () => re,
-                    includes: () => re,
-                    indexBy: () => ge,
-                    indexOf: () => zn,
-                    initial: () => Ae,
-                    inject: () => Xn,
-                    intersection: () => Fe,
+                    include: () => nn,
+                    includes: () => nn,
+                    indexBy: () => gn,
+                    indexOf: () => We,
+                    initial: () => An,
+                    inject: () => Qe,
+                    intersection: () => Fn,
                     invert: () => It,
-                    invoke: () => oe,
+                    invoke: () => rn,
                     isArguments: () => H,
                     isArray: () => K,
                     isArrayBuffer: () => C,
                     isBoolean: () => E,
                     isDataView: () => $,
                     isDate: () => F,
                     isElement: () => T,
                     isEmpty: () => lt,
                     isEqual: () => vt,
                     isError: () => L,
                     isFinite: () => Q,
                     isFunction: () => V,
                     isMap: () => xt,
-                    isMatch: () => ct,
+                    isMatch: () => st,
                     isNaN: () => X,
                     isNull: () => S,
                     isNumber: () => k,
                     isObject: () => O,
                     isRegExp: () => N,
                     isSet: () => St,
                     isString: () => B,
                     isSymbol: () => R,
-                    isTypedArray: () => ot,
+                    isTypedArray: () => it,
                     isUndefined: () => M,
                     isWeakMap: () => Ot,
                     isWeakSet: () => Mt,
                     iteratee: () => Qt,
                     keys: () => ut,
-                    last: () => Se,
-                    lastIndexOf: () => $n,
-                    map: () => Hn,
+                    last: () => Sn,
+                    lastIndexOf: () => ze,
+                    map: () => Ge,
                     mapObject: () => Yt,
                     matcher: () => Kt,
                     matches: () => Kt,
-                    max: () => ue,
-                    memoize: () => Mn,
+                    max: () => un,
+                    memoize: () => Se,
                     methods: () => Bt,
-                    min: () => le,
-                    mixin: () => Ve,
-                    negate: () => Fn,
+                    min: () => ln,
+                    mixin: () => Vn,
+                    negate: () => ke,
                     noop: () => Zt,
-                    now: () => rn,
-                    object: () => Re,
-                    omit: () => we,
-                    once: () => Cn,
+                    now: () => re,
+                    object: () => Rn,
+                    omit: () => wn,
+                    once: () => Re,
                     pairs: () => Tt,
-                    partial: () => wn,
-                    partition: () => me,
-                    pick: () => je,
-                    pluck: () => ie,
+                    partial: () => je,
+                    partition: () => yn,
+                    pick: () => jn,
+                    pluck: () => on,
                     property: () => Jt,
-                    propertyOf: () => tn,
-                    random: () => en,
-                    range: () => Ce,
-                    reduce: () => Xn,
-                    reduceRight: () => Yn,
-                    reject: () => te,
-                    rest: () => Oe,
+                    propertyOf: () => te,
+                    random: () => ne,
+                    range: () => Cn,
+                    reduce: () => Qe,
+                    reduceRight: () => Xe,
+                    reject: () => Ze,
+                    rest: () => On,
                     restArguments: () => x,
-                    result: () => gn,
-                    sample: () => fe,
-                    select: () => Zn,
-                    shuffle: () => pe,
-                    size: () => _e,
-                    some: () => ee,
-                    sortBy: () => he,
-                    sortedIndex: () => qn,
-                    tail: () => Oe,
-                    take: () => xe,
+                    result: () => ve,
+                    sample: () => fn,
+                    select: () => Ye,
+                    shuffle: () => hn,
+                    size: () => _n,
+                    some: () => en,
+                    sortBy: () => pn,
+                    sortedIndex: () => Pe,
+                    tail: () => On,
+                    take: () => xn,
                     tap: () => Dt,
-                    template: () => vn,
-                    templateSettings: () => cn,
-                    throttle: () => In,
-                    times: () => nn,
-                    toArray: () => se,
+                    template: () => de,
+                    templateSettings: () => le,
+                    throttle: () => Te,
+                    times: () => ee,
+                    toArray: () => cn,
                     toPath: () => Vt,
-                    transpose: () => Ne,
-                    unescape: () => ln,
-                    union: () => ke,
-                    uniq: () => Be,
-                    unique: () => Be,
-                    uniqueId: () => mn,
-                    unzip: () => Ne,
+                    transpose: () => Nn,
+                    unescape: () => ue,
+                    union: () => kn,
+                    uniq: () => Bn,
+                    unique: () => Bn,
+                    uniqueId: () => me,
+                    unzip: () => Nn,
                     values: () => Et,
-                    where: () => ae,
-                    without: () => Ie,
-                    wrap: () => kn,
-                    zip: () => Le
+                    where: () => an,
+                    without: () => In,
+                    wrap: () => Be,
+                    zip: () => Ln
                 });
                 var r = {};
-                e.r(r), e.d(r, {
-                    VERSION: () => o,
-                    after: () => Ln,
-                    all: () => ne,
+                n.r(r), n.d(r, {
+                    VERSION: () => i,
+                    after: () => Ne,
+                    all: () => tn,
                     allKeys: () => gt,
-                    any: () => ee,
+                    any: () => en,
                     assign: () => Nt,
-                    before: () => Rn,
-                    bind: () => An,
-                    bindAll: () => Sn,
-                    chain: () => _n,
-                    chunk: () => Ue,
+                    before: () => Le,
+                    bind: () => we,
+                    bindAll: () => Oe,
+                    chain: () => ye,
+                    chunk: () => Un,
                     clone: () => Ut,
-                    collect: () => Hn,
-                    compact: () => Me,
-                    compose: () => Nn,
+                    collect: () => Ge,
+                    compact: () => Mn,
+                    compose: () => Fe,
                     constant: () => Y,
-                    contains: () => re,
-                    countBy: () => ye,
+                    contains: () => nn,
+                    countBy: () => mn,
                     create: () => Ct,
-                    debounce: () => Bn,
-                    default: () => Pe,
+                    debounce: () => Ie,
+                    default: () => Pn,
                     defaults: () => Lt,
-                    defer: () => Tn,
-                    delay: () => En,
-                    detect: () => Kn,
-                    difference: () => Te,
-                    drop: () => Oe,
-                    each: () => Gn,
-                    escape: () => un,
-                    every: () => ne,
+                    defer: () => Ee,
+                    delay: () => Me,
+                    detect: () => $e,
+                    difference: () => Tn,
+                    drop: () => On,
+                    each: () => Je,
+                    escape: () => ae,
+                    every: () => tn,
                     extend: () => Ft,
                     extendOwn: () => Nt,
-                    filter: () => Zn,
-                    find: () => Kn,
-                    findIndex: () => Vn,
-                    findKey: () => Un,
-                    findLastIndex: () => Pn,
-                    findWhere: () => Jn,
-                    first: () => xe,
-                    flatten: () => Ee,
-                    foldl: () => Xn,
-                    foldr: () => Yn,
-                    forEach: () => Gn,
+                    filter: () => Ye,
+                    find: () => $e,
+                    findIndex: () => De,
+                    findKey: () => Ce,
+                    findLastIndex: () => Ve,
+                    findWhere: () => Ke,
+                    first: () => xn,
+                    flatten: () => En,
+                    foldl: () => Qe,
+                    foldr: () => Xe,
+                    forEach: () => Je,
                     functions: () => Bt,
                     get: () => Wt,
-                    groupBy: () => ve,
+                    groupBy: () => vn,
                     has: () => zt,
-                    head: () => xe,
+                    head: () => xn,
                     identity: () => $t,
-                    include: () => re,
-                    includes: () => re,
-                    indexBy: () => ge,
-                    indexOf: () => zn,
-                    initial: () => Ae,
-                    inject: () => Xn,
-                    intersection: () => Fe,
+                    include: () => nn,
+                    includes: () => nn,
+                    indexBy: () => gn,
+                    indexOf: () => We,
+                    initial: () => An,
+                    inject: () => Qe,
+                    intersection: () => Fn,
                     invert: () => It,
-                    invoke: () => oe,
+                    invoke: () => rn,
                     isArguments: () => H,
                     isArray: () => K,
                     isArrayBuffer: () => C,
                     isBoolean: () => E,
                     isDataView: () => $,
                     isDate: () => F,
                     isElement: () => T,
                     isEmpty: () => lt,
                     isEqual: () => vt,
                     isError: () => L,
                     isFinite: () => Q,
                     isFunction: () => V,
                     isMap: () => xt,
-                    isMatch: () => ct,
+                    isMatch: () => st,
                     isNaN: () => X,
                     isNull: () => S,
                     isNumber: () => k,
                     isObject: () => O,
                     isRegExp: () => N,
                     isSet: () => St,
                     isString: () => B,
                     isSymbol: () => R,
-                    isTypedArray: () => ot,
+                    isTypedArray: () => it,
                     isUndefined: () => M,
                     isWeakMap: () => Ot,
                     isWeakSet: () => Mt,
                     iteratee: () => Qt,
                     keys: () => ut,
-                    last: () => Se,
-                    lastIndexOf: () => $n,
-                    map: () => Hn,
+                    last: () => Sn,
+                    lastIndexOf: () => ze,
+                    map: () => Ge,
                     mapObject: () => Yt,
                     matcher: () => Kt,
                     matches: () => Kt,
-                    max: () => ue,
-                    memoize: () => Mn,
+                    max: () => un,
+                    memoize: () => Se,
                     methods: () => Bt,
-                    min: () => le,
-                    mixin: () => Ve,
-                    negate: () => Fn,
+                    min: () => ln,
+                    mixin: () => Vn,
+                    negate: () => ke,
                     noop: () => Zt,
-                    now: () => rn,
-                    object: () => Re,
-                    omit: () => we,
-                    once: () => Cn,
+                    now: () => re,
+                    object: () => Rn,
+                    omit: () => wn,
+                    once: () => Re,
                     pairs: () => Tt,
-                    partial: () => wn,
-                    partition: () => me,
-                    pick: () => je,
-                    pluck: () => ie,
+                    partial: () => je,
+                    partition: () => yn,
+                    pick: () => jn,
+                    pluck: () => on,
                     property: () => Jt,
-                    propertyOf: () => tn,
-                    random: () => en,
-                    range: () => Ce,
-                    reduce: () => Xn,
-                    reduceRight: () => Yn,
-                    reject: () => te,
-                    rest: () => Oe,
+                    propertyOf: () => te,
+                    random: () => ne,
+                    range: () => Cn,
+                    reduce: () => Qe,
+                    reduceRight: () => Xe,
+                    reject: () => Ze,
+                    rest: () => On,
                     restArguments: () => x,
-                    result: () => gn,
-                    sample: () => fe,
-                    select: () => Zn,
-                    shuffle: () => pe,
-                    size: () => _e,
-                    some: () => ee,
-                    sortBy: () => he,
-                    sortedIndex: () => qn,
-                    tail: () => Oe,
-                    take: () => xe,
+                    result: () => ve,
+                    sample: () => fn,
+                    select: () => Ye,
+                    shuffle: () => hn,
+                    size: () => _n,
+                    some: () => en,
+                    sortBy: () => pn,
+                    sortedIndex: () => Pe,
+                    tail: () => On,
+                    take: () => xn,
                     tap: () => Dt,
-                    template: () => vn,
-                    templateSettings: () => cn,
-                    throttle: () => In,
-                    times: () => nn,
-                    toArray: () => se,
+                    template: () => de,
+                    templateSettings: () => le,
+                    throttle: () => Te,
+                    times: () => ee,
+                    toArray: () => cn,
                     toPath: () => Vt,
-                    transpose: () => Ne,
-                    unescape: () => ln,
-                    union: () => ke,
-                    uniq: () => Be,
-                    unique: () => Be,
-                    uniqueId: () => mn,
-                    unzip: () => Ne,
+                    transpose: () => Nn,
+                    unescape: () => ue,
+                    union: () => kn,
+                    uniq: () => Bn,
+                    unique: () => Bn,
+                    uniqueId: () => me,
+                    unzip: () => Nn,
                     values: () => Et,
-                    where: () => ae,
-                    without: () => Ie,
-                    wrap: () => kn,
-                    zip: () => Le
+                    where: () => an,
+                    without: () => In,
+                    wrap: () => Be,
+                    zip: () => Ln
                 });
-                var o = "1.13.6",
-                    i = "object" == typeof self && self.self === self && self || "object" == typeof global && global.global === global && global || Function("return this")() || {},
+                var i = "1.13.6",
+                    o = "object" == typeof self && self.self === self && self || "object" == typeof global && global.global === global && global || Function("return this")() || {},
                     a = Array.prototype,
                     u = Object.prototype,
                     l = "undefined" != typeof Symbol ? Symbol.prototype : null,
-                    c = a.push,
-                    s = a.slice,
+                    s = a.push,
+                    c = a.slice,
                     f = u.toString,
-                    p = u.hasOwnProperty,
-                    h = "undefined" != typeof ArrayBuffer,
+                    h = u.hasOwnProperty,
+                    p = "undefined" != typeof ArrayBuffer,
                     d = "undefined" != typeof DataView,
                     v = Array.isArray,
                     g = Object.keys,
-                    y = Object.create,
-                    m = h && ArrayBuffer.isView,
+                    m = Object.create,
+                    y = p && ArrayBuffer.isView,
                     _ = isNaN,
                     b = isFinite,
                     j = !{
                         toString: null
                     }.propertyIsEnumerable("toString"),
                     w = ["valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
                     A = Math.pow(2, 53) - 1;
 
-                function x(t, n) {
-                    return n = null == n ? t.length - 1 : +n,
+                function x(t, e) {
+                    return e = null == e ? t.length - 1 : +e,
                         function() {
-                            for (var e = Math.max(arguments.length - n, 0), r = Array(e), o = 0; o < e; o++) r[o] = arguments[o + n];
-                            switch (n) {
+                            for (var n = Math.max(arguments.length - e, 0), r = Array(n), i = 0; i < n; i++) r[i] = arguments[i + e];
+                            switch (e) {
                                 case 0:
                                     return t.call(this, r);
                                 case 1:
                                     return t.call(this, arguments[0], r);
                                 case 2:
                                     return t.call(this, arguments[0], arguments[1], r)
                             }
-                            var i = Array(n + 1);
-                            for (o = 0; o < n; o++) i[o] = arguments[o];
-                            return i[n] = r, t.apply(this, i)
+                            var o = Array(e + 1);
+                            for (i = 0; i < e; i++) o[i] = arguments[i];
+                            return o[e] = r, t.apply(this, o)
                         }
                 }
 
                 function O(t) {
-                    var n = typeof t;
-                    return "function" === n || "object" === n && !!t
+                    var e = typeof t;
+                    return "function" === e || "object" === e && !!t
                 }
 
                 function S(t) {
                     return null === t
                 }
 
                 function M(t) {
@@ -364,43 +364,43 @@
                 }
 
                 function T(t) {
                     return !(!t || 1 !== t.nodeType)
                 }
 
                 function I(t) {
-                    var n = "[object " + t + "]";
+                    var e = "[object " + t + "]";
                     return function(t) {
-                        return f.call(t) === n
+                        return f.call(t) === e
                     }
                 }
                 const B = I("String"),
                     k = I("Number"),
                     F = I("Date"),
                     N = I("RegExp"),
                     L = I("Error"),
                     R = I("Symbol"),
                     C = I("ArrayBuffer");
                 var U = I("Function"),
-                    D = i.document && i.document.childNodes;
+                    D = o.document && o.document.childNodes;
                 "object" != typeof Int8Array && "function" != typeof D && (U = function(t) {
                     return "function" == typeof t || !1
                 });
                 const V = U,
                     P = I("Object");
                 var q = d && P(new DataView(new ArrayBuffer(8))),
                     W = "undefined" != typeof Map && P(new Map),
                     z = I("DataView");
                 const $ = q ? function(t) {
                         return null != t && V(t.getInt8) && C(t.buffer)
                     } : z,
                     K = v || I("Array");
 
-                function J(t, n) {
-                    return null != t && p.call(t, n)
+                function J(t, e) {
+                    return null != t && h.call(t, e)
                 }
                 var G = I("Arguments");
                 ! function() {
                     G(arguments) || (G = function(t) {
                         return J(t, "callee")
                     })
                 }();
@@ -417,1112 +417,1114 @@
                 function Y(t) {
                     return function() {
                         return t
                     }
                 }
 
                 function Z(t) {
-                    return function(n) {
-                        var e = t(n);
-                        return "number" == typeof e && e >= 0 && e <= A
+                    return function(e) {
+                        var n = t(e);
+                        return "number" == typeof n && n >= 0 && n <= A
                     }
                 }
 
                 function tt(t) {
-                    return function(n) {
-                        return null == n ? void 0 : n[t]
+                    return function(e) {
+                        return null == e ? void 0 : e[t]
                     }
                 }
-                const nt = tt("byteLength"),
-                    et = Z(nt);
+                const et = tt("byteLength"),
+                    nt = Z(et);
                 var rt = /\[object ((I|Ui)nt(8|16|32)|Float(32|64)|Uint8Clamped|Big(I|Ui)nt64)Array\]/;
-                const ot = h ? function(t) {
-                        return m ? m(t) && !$(t) : et(t) && rt.test(f.call(t))
+                const it = p ? function(t) {
+                        return y ? y(t) && !$(t) : nt(t) && rt.test(f.call(t))
                     } : Y(!1),
-                    it = tt("length");
+                    ot = tt("length");
 
-                function at(t, n) {
-                    n = function(t) {
-                        for (var n = {}, e = t.length, r = 0; r < e; ++r) n[t[r]] = !0;
+                function at(t, e) {
+                    e = function(t) {
+                        for (var e = {}, n = t.length, r = 0; r < n; ++r) e[t[r]] = !0;
                         return {
                             contains: function(t) {
-                                return !0 === n[t]
+                                return !0 === e[t]
                             },
-                            push: function(e) {
-                                return n[e] = !0, t.push(e)
+                            push: function(n) {
+                                return e[n] = !0, t.push(n)
                             }
                         }
-                    }(n);
-                    var e = w.length,
+                    }(e);
+                    var n = w.length,
                         r = t.constructor,
-                        o = V(r) && r.prototype || u,
-                        i = "constructor";
-                    for (J(t, i) && !n.contains(i) && n.push(i); e--;)(i = w[e]) in t && t[i] !== o[i] && !n.contains(i) && n.push(i)
+                        i = V(r) && r.prototype || u,
+                        o = "constructor";
+                    for (J(t, o) && !e.contains(o) && e.push(o); n--;)(o = w[n]) in t && t[o] !== i[o] && !e.contains(o) && e.push(o)
                 }
 
                 function ut(t) {
                     if (!O(t)) return [];
                     if (g) return g(t);
-                    var n = [];
-                    for (var e in t) J(t, e) && n.push(e);
-                    return j && at(t, n), n
+                    var e = [];
+                    for (var n in t) J(t, n) && e.push(n);
+                    return j && at(t, e), e
                 }
 
                 function lt(t) {
                     if (null == t) return !0;
-                    var n = it(t);
-                    return "number" == typeof n && (K(t) || B(t) || H(t)) ? 0 === n : 0 === it(ut(t))
+                    var e = ot(t);
+                    return "number" == typeof e && (K(t) || B(t) || H(t)) ? 0 === e : 0 === ot(ut(t))
                 }
 
-                function ct(t, n) {
-                    var e = ut(n),
-                        r = e.length;
+                function st(t, e) {
+                    var n = ut(e),
+                        r = n.length;
                     if (null == t) return !r;
-                    for (var o = Object(t), i = 0; i < r; i++) {
-                        var a = e[i];
-                        if (n[a] !== o[a] || !(a in o)) return !1
+                    for (var i = Object(t), o = 0; o < r; o++) {
+                        var a = n[o];
+                        if (e[a] !== i[a] || !(a in i)) return !1
                     }
                     return !0
                 }
 
-                function st(t) {
-                    return t instanceof st ? t : this instanceof st ? void(this._wrapped = t) : new st(t)
+                function ct(t) {
+                    return t instanceof ct ? t : this instanceof ct ? void(this._wrapped = t) : new ct(t)
                 }
 
                 function ft(t) {
-                    return new Uint8Array(t.buffer || t, t.byteOffset || 0, nt(t))
+                    return new Uint8Array(t.buffer || t, t.byteOffset || 0, et(t))
                 }
-                st.VERSION = o, st.prototype.value = function() {
+                ct.VERSION = i, ct.prototype.value = function() {
                     return this._wrapped
-                }, st.prototype.valueOf = st.prototype.toJSON = st.prototype.value, st.prototype.toString = function() {
+                }, ct.prototype.valueOf = ct.prototype.toJSON = ct.prototype.value, ct.prototype.toString = function() {
                     return String(this._wrapped)
                 };
-                var pt = "[object DataView]";
+                var ht = "[object DataView]";
 
-                function ht(t, n, e, r) {
-                    if (t === n) return 0 !== t || 1 / t == 1 / n;
-                    if (null == t || null == n) return !1;
-                    if (t != t) return n != n;
-                    var o = typeof t;
-                    return ("function" === o || "object" === o || "object" == typeof n) && dt(t, n, e, r)
-                }
-
-                function dt(t, n, e, r) {
-                    t instanceof st && (t = t._wrapped), n instanceof st && (n = n._wrapped);
-                    var o = f.call(t);
-                    if (o !== f.call(n)) return !1;
-                    if (q && "[object Object]" == o && $(t)) {
-                        if (!$(n)) return !1;
-                        o = pt
+                function pt(t, e, n, r) {
+                    if (t === e) return 0 !== t || 1 / t == 1 / e;
+                    if (null == t || null == e) return !1;
+                    if (t != t) return e != e;
+                    var i = typeof t;
+                    return ("function" === i || "object" === i || "object" == typeof e) && dt(t, e, n, r)
+                }
+
+                function dt(t, e, n, r) {
+                    t instanceof ct && (t = t._wrapped), e instanceof ct && (e = e._wrapped);
+                    var i = f.call(t);
+                    if (i !== f.call(e)) return !1;
+                    if (q && "[object Object]" == i && $(t)) {
+                        if (!$(e)) return !1;
+                        i = ht
                     }
-                    switch (o) {
+                    switch (i) {
                         case "[object RegExp]":
                         case "[object String]":
-                            return "" + t == "" + n;
+                            return "" + t == "" + e;
                         case "[object Number]":
-                            return +t != +t ? +n != +n : 0 == +t ? 1 / +t == 1 / n : +t == +n;
+                            return +t != +t ? +e != +e : 0 == +t ? 1 / +t == 1 / e : +t == +e;
                         case "[object Date]":
                         case "[object Boolean]":
-                            return +t == +n;
+                            return +t == +e;
                         case "[object Symbol]":
-                            return l.valueOf.call(t) === l.valueOf.call(n);
+                            return l.valueOf.call(t) === l.valueOf.call(e);
                         case "[object ArrayBuffer]":
-                        case pt:
-                            return dt(ft(t), ft(n), e, r)
+                        case ht:
+                            return dt(ft(t), ft(e), n, r)
                     }
-                    var i = "[object Array]" === o;
-                    if (!i && ot(t)) {
-                        if (nt(t) !== nt(n)) return !1;
-                        if (t.buffer === n.buffer && t.byteOffset === n.byteOffset) return !0;
-                        i = !0
+                    var o = "[object Array]" === i;
+                    if (!o && it(t)) {
+                        if (et(t) !== et(e)) return !1;
+                        if (t.buffer === e.buffer && t.byteOffset === e.byteOffset) return !0;
+                        o = !0
                     }
-                    if (!i) {
-                        if ("object" != typeof t || "object" != typeof n) return !1;
+                    if (!o) {
+                        if ("object" != typeof t || "object" != typeof e) return !1;
                         var a = t.constructor,
-                            u = n.constructor;
-                        if (a !== u && !(V(a) && a instanceof a && V(u) && u instanceof u) && "constructor" in t && "constructor" in n) return !1
+                            u = e.constructor;
+                        if (a !== u && !(V(a) && a instanceof a && V(u) && u instanceof u) && "constructor" in t && "constructor" in e) return !1
                     }
                     r = r || [];
-                    for (var c = (e = e || []).length; c--;)
-                        if (e[c] === t) return r[c] === n;
-                    if (e.push(t), r.push(n), i) {
-                        if ((c = t.length) !== n.length) return !1;
-                        for (; c--;)
-                            if (!ht(t[c], n[c], e, r)) return !1
+                    for (var s = (n = n || []).length; s--;)
+                        if (n[s] === t) return r[s] === e;
+                    if (n.push(t), r.push(e), o) {
+                        if ((s = t.length) !== e.length) return !1;
+                        for (; s--;)
+                            if (!pt(t[s], e[s], n, r)) return !1
                     } else {
-                        var s, p = ut(t);
-                        if (c = p.length, ut(n).length !== c) return !1;
-                        for (; c--;)
-                            if (!J(n, s = p[c]) || !ht(t[s], n[s], e, r)) return !1
+                        var c, h = ut(t);
+                        if (s = h.length, ut(e).length !== s) return !1;
+                        for (; s--;)
+                            if (!J(e, c = h[s]) || !pt(t[c], e[c], n, r)) return !1
                     }
-                    return e.pop(), r.pop(), !0
+                    return n.pop(), r.pop(), !0
                 }
 
-                function vt(t, n) {
-                    return ht(t, n)
+                function vt(t, e) {
+                    return pt(t, e)
                 }
 
                 function gt(t) {
                     if (!O(t)) return [];
-                    var n = [];
-                    for (var e in t) n.push(e);
-                    return j && at(t, n), n
+                    var e = [];
+                    for (var n in t) e.push(n);
+                    return j && at(t, e), e
                 }
 
-                function yt(t) {
-                    var n = it(t);
-                    return function(e) {
-                        if (null == e) return !1;
-                        var r = gt(e);
-                        if (it(r)) return !1;
-                        for (var o = 0; o < n; o++)
-                            if (!V(e[t[o]])) return !1;
-                        return t !== wt || !V(e[mt])
+                function mt(t) {
+                    var e = ot(t);
+                    return function(n) {
+                        if (null == n) return !1;
+                        var r = gt(n);
+                        if (ot(r)) return !1;
+                        for (var i = 0; i < e; i++)
+                            if (!V(n[t[i]])) return !1;
+                        return t !== wt || !V(n[yt])
                     }
                 }
-                var mt = "forEach",
+                var yt = "forEach",
                     _t = ["clear", "delete"],
                     bt = ["get", "has", "set"],
-                    jt = _t.concat(mt, bt),
+                    jt = _t.concat(yt, bt),
                     wt = _t.concat(bt),
-                    At = ["add"].concat(_t, mt, "has");
-                const xt = W ? yt(jt) : I("Map"),
-                    Ot = W ? yt(wt) : I("WeakMap"),
-                    St = W ? yt(At) : I("Set"),
+                    At = ["add"].concat(_t, yt, "has");
+                const xt = W ? mt(jt) : I("Map"),
+                    Ot = W ? mt(wt) : I("WeakMap"),
+                    St = W ? mt(At) : I("Set"),
                     Mt = I("WeakSet");
 
                 function Et(t) {
-                    for (var n = ut(t), e = n.length, r = Array(e), o = 0; o < e; o++) r[o] = t[n[o]];
+                    for (var e = ut(t), n = e.length, r = Array(n), i = 0; i < n; i++) r[i] = t[e[i]];
                     return r
                 }
 
                 function Tt(t) {
-                    for (var n = ut(t), e = n.length, r = Array(e), o = 0; o < e; o++) r[o] = [n[o], t[n[o]]];
+                    for (var e = ut(t), n = e.length, r = Array(n), i = 0; i < n; i++) r[i] = [e[i], t[e[i]]];
                     return r
                 }
 
                 function It(t) {
-                    for (var n = {}, e = ut(t), r = 0, o = e.length; r < o; r++) n[t[e[r]]] = e[r];
-                    return n
+                    for (var e = {}, n = ut(t), r = 0, i = n.length; r < i; r++) e[t[n[r]]] = n[r];
+                    return e
                 }
 
                 function Bt(t) {
-                    var n = [];
-                    for (var e in t) V(t[e]) && n.push(e);
-                    return n.sort()
+                    var e = [];
+                    for (var n in t) V(t[n]) && e.push(n);
+                    return e.sort()
                 }
 
-                function kt(t, n) {
-                    return function(e) {
+                function kt(t, e) {
+                    return function(n) {
                         var r = arguments.length;
-                        if (n && (e = Object(e)), r < 2 || null == e) return e;
-                        for (var o = 1; o < r; o++)
-                            for (var i = arguments[o], a = t(i), u = a.length, l = 0; l < u; l++) {
-                                var c = a[l];
-                                n && void 0 !== e[c] || (e[c] = i[c])
+                        if (e && (n = Object(n)), r < 2 || null == n) return n;
+                        for (var i = 1; i < r; i++)
+                            for (var o = arguments[i], a = t(o), u = a.length, l = 0; l < u; l++) {
+                                var s = a[l];
+                                e && void 0 !== n[s] || (n[s] = o[s])
                             }
-                        return e
+                        return n
                     }
                 }
                 const Ft = kt(gt),
                     Nt = kt(ut),
                     Lt = kt(gt, !0);
 
                 function Rt(t) {
                     if (!O(t)) return {};
-                    if (y) return y(t);
-                    var n = function() {};
-                    n.prototype = t;
-                    var e = new n;
-                    return n.prototype = null, e
+                    if (m) return m(t);
+                    var e = function() {};
+                    e.prototype = t;
+                    var n = new e;
+                    return e.prototype = null, n
                 }
 
-                function Ct(t, n) {
-                    var e = Rt(t);
-                    return n && Nt(e, n), e
+                function Ct(t, e) {
+                    var n = Rt(t);
+                    return e && Nt(n, e), n
                 }
 
                 function Ut(t) {
                     return O(t) ? K(t) ? t.slice() : Ft({}, t) : t
                 }
 
-                function Dt(t, n) {
-                    return n(t), t
+                function Dt(t, e) {
+                    return e(t), t
                 }
 
                 function Vt(t) {
                     return K(t) ? t : [t]
                 }
 
                 function Pt(t) {
-                    return st.toPath(t)
+                    return ct.toPath(t)
                 }
 
-                function qt(t, n) {
-                    for (var e = n.length, r = 0; r < e; r++) {
+                function qt(t, e) {
+                    for (var n = e.length, r = 0; r < n; r++) {
                         if (null == t) return;
-                        t = t[n[r]]
+                        t = t[e[r]]
                     }
-                    return e ? t : void 0
+                    return n ? t : void 0
                 }
 
-                function Wt(t, n, e) {
-                    var r = qt(t, Pt(n));
-                    return M(r) ? e : r
+                function Wt(t, e, n) {
+                    var r = qt(t, Pt(e));
+                    return M(r) ? n : r
                 }
 
-                function zt(t, n) {
-                    for (var e = (n = Pt(n)).length, r = 0; r < e; r++) {
-                        var o = n[r];
-                        if (!J(t, o)) return !1;
-                        t = t[o]
+                function zt(t, e) {
+                    for (var n = (e = Pt(e)).length, r = 0; r < n; r++) {
+                        var i = e[r];
+                        if (!J(t, i)) return !1;
+                        t = t[i]
                     }
-                    return !!e
+                    return !!n
                 }
 
                 function $t(t) {
                     return t
                 }
 
                 function Kt(t) {
                     return t = Nt({}, t),
-                        function(n) {
-                            return ct(n, t)
+                        function(e) {
+                            return st(e, t)
                         }
                 }
 
                 function Jt(t) {
                     return t = Pt(t),
-                        function(n) {
-                            return qt(n, t)
+                        function(e) {
+                            return qt(e, t)
                         }
                 }
 
-                function Gt(t, n, e) {
-                    if (void 0 === n) return t;
-                    switch (null == e ? 3 : e) {
+                function Gt(t, e, n) {
+                    if (void 0 === e) return t;
+                    switch (null == n ? 3 : n) {
                         case 1:
-                            return function(e) {
-                                return t.call(n, e)
+                            return function(n) {
+                                return t.call(e, n)
                             };
                         case 3:
-                            return function(e, r, o) {
-                                return t.call(n, e, r, o)
+                            return function(n, r, i) {
+                                return t.call(e, n, r, i)
                             };
                         case 4:
-                            return function(e, r, o, i) {
-                                return t.call(n, e, r, o, i)
+                            return function(n, r, i, o) {
+                                return t.call(e, n, r, i, o)
                             }
                     }
                     return function() {
-                        return t.apply(n, arguments)
+                        return t.apply(e, arguments)
                     }
                 }
 
-                function Ht(t, n, e) {
-                    return null == t ? $t : V(t) ? Gt(t, n, e) : O(t) && !K(t) ? Kt(t) : Jt(t)
+                function Ht(t, e, n) {
+                    return null == t ? $t : V(t) ? Gt(t, e, n) : O(t) && !K(t) ? Kt(t) : Jt(t)
                 }
 
-                function Qt(t, n) {
-                    return Ht(t, n, 1 / 0)
+                function Qt(t, e) {
+                    return Ht(t, e, 1 / 0)
                 }
 
-                function Xt(t, n, e) {
-                    return st.iteratee !== Qt ? st.iteratee(t, n) : Ht(t, n, e)
+                function Xt(t, e, n) {
+                    return ct.iteratee !== Qt ? ct.iteratee(t, e) : Ht(t, e, n)
                 }
 
-                function Yt(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = ut(t), o = r.length, i = {}, a = 0; a < o; a++) {
+                function Yt(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = ut(t), i = r.length, o = {}, a = 0; a < i; a++) {
                         var u = r[a];
-                        i[u] = n(t[u], u, t)
+                        o[u] = e(t[u], u, t)
                     }
-                    return i
+                    return o
                 }
 
                 function Zt() {}
 
-                function tn(t) {
-                    return null == t ? Zt : function(n) {
-                        return Wt(t, n)
+                function te(t) {
+                    return null == t ? Zt : function(e) {
+                        return Wt(t, e)
                     }
                 }
 
-                function nn(t, n, e) {
+                function ee(t, e, n) {
                     var r = Array(Math.max(0, t));
-                    n = Gt(n, e, 1);
-                    for (var o = 0; o < t; o++) r[o] = n(o);
+                    e = Gt(e, n, 1);
+                    for (var i = 0; i < t; i++) r[i] = e(i);
                     return r
                 }
 
-                function en(t, n) {
-                    return null == n && (n = t, t = 0), t + Math.floor(Math.random() * (n - t + 1))
+                function ne(t, e) {
+                    return null == e && (e = t, t = 0), t + Math.floor(Math.random() * (e - t + 1))
                 }
-                st.toPath = Vt, st.iteratee = Qt;
-                const rn = Date.now || function() {
+                ct.toPath = Vt, ct.iteratee = Qt;
+                const re = Date.now || function() {
                     return (new Date).getTime()
                 };
 
-                function on(t) {
-                    var n = function(n) {
-                            return t[n]
+                function ie(t) {
+                    var e = function(e) {
+                            return t[e]
                         },
-                        e = "(?:" + ut(t).join("|") + ")",
-                        r = RegExp(e),
-                        o = RegExp(e, "g");
+                        n = "(?:" + ut(t).join("|") + ")",
+                        r = RegExp(n),
+                        i = RegExp(n, "g");
                     return function(t) {
-                        return t = null == t ? "" : "" + t, r.test(t) ? t.replace(o, n) : t
+                        return t = null == t ? "" : "" + t, r.test(t) ? t.replace(i, e) : t
                     }
                 }
-                const an = {
+                const oe = {
                         "&": "&amp;",
                         "<": "&lt;",
                         ">": "&gt;",
                         '"': "&quot;",
                         "'": "&#x27;",
                         "`": "&#x60;"
                     },
-                    un = on(an),
-                    ln = on(It(an)),
-                    cn = st.templateSettings = {
+                    ae = ie(oe),
+                    ue = ie(It(oe)),
+                    le = ct.templateSettings = {
                         evaluate: /<%([\s\S]+?)%>/g,
                         interpolate: /<%=([\s\S]+?)%>/g,
                         escape: /<%-([\s\S]+?)%>/g
                     };
-                var sn = /(.)^/,
-                    fn = {
+                var se = /(.)^/,
+                    ce = {
                         "'": "'",
                         "\\": "\\",
                         "\r": "r",
                         "\n": "n",
                         "\u2028": "u2028",
                         "\u2029": "u2029"
                     },
-                    pn = /\\|'|\r|\n|\u2028|\u2029/g;
+                    fe = /\\|'|\r|\n|\u2028|\u2029/g;
 
-                function hn(t) {
-                    return "\\" + fn[t]
+                function he(t) {
+                    return "\\" + ce[t]
                 }
-                var dn = /^\s*(\w|\$)+\s*$/;
+                var pe = /^\s*(\w|\$)+\s*$/;
 
-                function vn(t, n, e) {
-                    !n && e && (n = e), n = Lt({}, n, st.templateSettings);
-                    var r = RegExp([(n.escape || sn).source, (n.interpolate || sn).source, (n.evaluate || sn).source].join("|") + "|$", "g"),
-                        o = 0,
-                        i = "__p+='";
-                    t.replace(r, (function(n, e, r, a, u) {
-                        return i += t.slice(o, u).replace(pn, hn), o = u + n.length, e ? i += "'+\n((__t=(" + e + "))==null?'':_.escape(__t))+\n'" : r ? i += "'+\n((__t=(" + r + "))==null?'':__t)+\n'" : a && (i += "';\n" + a + "\n__p+='"), n
-                    })), i += "';\n";
-                    var a, u = n.variable;
+                function de(t, e, n) {
+                    !e && n && (e = n), e = Lt({}, e, ct.templateSettings);
+                    var r = RegExp([(e.escape || se).source, (e.interpolate || se).source, (e.evaluate || se).source].join("|") + "|$", "g"),
+                        i = 0,
+                        o = "__p+='";
+                    t.replace(r, (function(e, n, r, a, u) {
+                        return o += t.slice(i, u).replace(fe, he), i = u + e.length, n ? o += "'+\n((__t=(" + n + "))==null?'':_.escape(__t))+\n'" : r ? o += "'+\n((__t=(" + r + "))==null?'':__t)+\n'" : a && (o += "';\n" + a + "\n__p+='"), e
+                    })), o += "';\n";
+                    var a, u = e.variable;
                     if (u) {
-                        if (!dn.test(u)) throw new Error("variable is not a bare identifier: " + u)
-                    } else i = "with(obj||{}){\n" + i + "}\n", u = "obj";
-                    i = "var __t,__p='',__j=Array.prototype.join,print=function(){__p+=__j.call(arguments,'');};\n" + i + "return __p;\n";
+                        if (!pe.test(u)) throw new Error("variable is not a bare identifier: " + u)
+                    } else o = "with(obj||{}){\n" + o + "}\n", u = "obj";
+                    o = "var __t,__p='',__j=Array.prototype.join,print=function(){__p+=__j.call(arguments,'');};\n" + o + "return __p;\n";
                     try {
-                        a = new Function(u, "_", i)
+                        a = new Function(u, "_", o)
                     } catch (t) {
-                        throw t.source = i, t
+                        throw t.source = o, t
                     }
                     var l = function(t) {
-                        return a.call(this, t, st)
+                        return a.call(this, t, ct)
                     };
-                    return l.source = "function(" + u + "){\n" + i + "}", l
+                    return l.source = "function(" + u + "){\n" + o + "}", l
                 }
 
-                function gn(t, n, e) {
-                    var r = (n = Pt(n)).length;
-                    if (!r) return V(e) ? e.call(t) : e;
-                    for (var o = 0; o < r; o++) {
-                        var i = null == t ? void 0 : t[n[o]];
-                        void 0 === i && (i = e, o = r), t = V(i) ? i.call(t) : i
+                function ve(t, e, n) {
+                    var r = (e = Pt(e)).length;
+                    if (!r) return V(n) ? n.call(t) : n;
+                    for (var i = 0; i < r; i++) {
+                        var o = null == t ? void 0 : t[e[i]];
+                        void 0 === o && (o = n, i = r), t = V(o) ? o.call(t) : o
                     }
                     return t
                 }
-                var yn = 0;
+                var ge = 0;
 
-                function mn(t) {
-                    var n = ++yn + "";
-                    return t ? t + n : n
+                function me(t) {
+                    var e = ++ge + "";
+                    return t ? t + e : e
                 }
 
-                function _n(t) {
-                    var n = st(t);
-                    return n._chain = !0, n
+                function ye(t) {
+                    var e = ct(t);
+                    return e._chain = !0, e
                 }
 
-                function bn(t, n, e, r, o) {
-                    if (!(r instanceof n)) return t.apply(e, o);
-                    var i = Rt(t.prototype),
-                        a = t.apply(i, o);
-                    return O(a) ? a : i
+                function _e(t, e, n, r, i) {
+                    if (!(r instanceof e)) return t.apply(n, i);
+                    var o = Rt(t.prototype),
+                        a = t.apply(o, i);
+                    return O(a) ? a : o
                 }
-                var jn = x((function(t, n) {
-                    var e = jn.placeholder,
+                var be = x((function(t, e) {
+                    var n = be.placeholder,
                         r = function() {
-                            for (var o = 0, i = n.length, a = Array(i), u = 0; u < i; u++) a[u] = n[u] === e ? arguments[o++] : n[u];
-                            for (; o < arguments.length;) a.push(arguments[o++]);
-                            return bn(t, r, this, this, a)
+                            for (var i = 0, o = e.length, a = Array(o), u = 0; u < o; u++) a[u] = e[u] === n ? arguments[i++] : e[u];
+                            for (; i < arguments.length;) a.push(arguments[i++]);
+                            return _e(t, r, this, this, a)
                         };
                     return r
                 }));
-                jn.placeholder = st;
-                const wn = jn,
-                    An = x((function(t, n, e) {
+                be.placeholder = ct;
+                const je = be,
+                    we = x((function(t, e, n) {
                         if (!V(t)) throw new TypeError("Bind must be called on a function");
-                        var r = x((function(o) {
-                            return bn(t, r, n, this, e.concat(o))
+                        var r = x((function(i) {
+                            return _e(t, r, e, this, n.concat(i))
                         }));
                         return r
                     })),
-                    xn = Z(it);
+                    Ae = Z(ot);
 
-                function On(t, n, e, r) {
-                    if (r = r || [], n || 0 === n) {
-                        if (n <= 0) return r.concat(t)
-                    } else n = 1 / 0;
-                    for (var o = r.length, i = 0, a = it(t); i < a; i++) {
-                        var u = t[i];
-                        if (xn(u) && (K(u) || H(u)))
-                            if (n > 1) On(u, n - 1, e, r), o = r.length;
+                function xe(t, e, n, r) {
+                    if (r = r || [], e || 0 === e) {
+                        if (e <= 0) return r.concat(t)
+                    } else e = 1 / 0;
+                    for (var i = r.length, o = 0, a = ot(t); o < a; o++) {
+                        var u = t[o];
+                        if (Ae(u) && (K(u) || H(u)))
+                            if (e > 1) xe(u, e - 1, n, r), i = r.length;
                             else
-                                for (var l = 0, c = u.length; l < c;) r[o++] = u[l++];
-                        else e || (r[o++] = u)
+                                for (var l = 0, s = u.length; l < s;) r[i++] = u[l++];
+                        else n || (r[i++] = u)
                     }
                     return r
                 }
-                const Sn = x((function(t, n) {
-                    var e = (n = On(n, !1, !1)).length;
-                    if (e < 1) throw new Error("bindAll must be passed function names");
-                    for (; e--;) {
-                        var r = n[e];
-                        t[r] = An(t[r], t)
+                const Oe = x((function(t, e) {
+                    var n = (e = xe(e, !1, !1)).length;
+                    if (n < 1) throw new Error("bindAll must be passed function names");
+                    for (; n--;) {
+                        var r = e[n];
+                        t[r] = we(t[r], t)
                     }
                     return t
                 }));
 
-                function Mn(t, n) {
-                    var e = function(r) {
-                        var o = e.cache,
-                            i = "" + (n ? n.apply(this, arguments) : r);
-                        return J(o, i) || (o[i] = t.apply(this, arguments)), o[i]
+                function Se(t, e) {
+                    var n = function(r) {
+                        var i = n.cache,
+                            o = "" + (e ? e.apply(this, arguments) : r);
+                        return J(i, o) || (i[o] = t.apply(this, arguments)), i[o]
                     };
-                    return e.cache = {}, e
+                    return n.cache = {}, n
                 }
-                const En = x((function(t, n, e) {
+                const Me = x((function(t, e, n) {
                         return setTimeout((function() {
-                            return t.apply(null, e)
-                        }), n)
+                            return t.apply(null, n)
+                        }), e)
                     })),
-                    Tn = wn(En, st, 1);
+                    Ee = je(Me, ct, 1);
 
-                function In(t, n, e) {
-                    var r, o, i, a, u = 0;
-                    e || (e = {});
+                function Te(t, e, n) {
+                    var r, i, o, a, u = 0;
+                    n || (n = {});
                     var l = function() {
-                            u = !1 === e.leading ? 0 : rn(), r = null, a = t.apply(o, i), r || (o = i = null)
+                            u = !1 === n.leading ? 0 : re(), r = null, a = t.apply(i, o), r || (i = o = null)
                         },
-                        c = function() {
-                            var c = rn();
-                            u || !1 !== e.leading || (u = c);
-                            var s = n - (c - u);
-                            return o = this, i = arguments, s <= 0 || s > n ? (r && (clearTimeout(r), r = null), u = c, a = t.apply(o, i), r || (o = i = null)) : r || !1 === e.trailing || (r = setTimeout(l, s)), a
+                        s = function() {
+                            var s = re();
+                            u || !1 !== n.leading || (u = s);
+                            var c = e - (s - u);
+                            return i = this, o = arguments, c <= 0 || c > e ? (r && (clearTimeout(r), r = null), u = s, a = t.apply(i, o), r || (i = o = null)) : r || !1 === n.trailing || (r = setTimeout(l, c)), a
                         };
-                    return c.cancel = function() {
-                        clearTimeout(r), u = 0, r = o = i = null
-                    }, c
+                    return s.cancel = function() {
+                        clearTimeout(r), u = 0, r = i = o = null
+                    }, s
                 }
 
-                function Bn(t, n, e) {
-                    var r, o, i, a, u, l = function() {
-                            var c = rn() - o;
-                            n > c ? r = setTimeout(l, n - c) : (r = null, e || (a = t.apply(u, i)), r || (i = u = null))
+                function Ie(t, e, n) {
+                    var r, i, o, a, u, l = function() {
+                            var s = re() - i;
+                            e > s ? r = setTimeout(l, e - s) : (r = null, n || (a = t.apply(u, o)), r || (o = u = null))
                         },
-                        c = x((function(c) {
-                            return u = this, i = c, o = rn(), r || (r = setTimeout(l, n), e && (a = t.apply(u, i))), a
+                        s = x((function(s) {
+                            return u = this, o = s, i = re(), r || (r = setTimeout(l, e), n && (a = t.apply(u, o))), a
                         }));
-                    return c.cancel = function() {
-                        clearTimeout(r), r = i = u = null
-                    }, c
+                    return s.cancel = function() {
+                        clearTimeout(r), r = o = u = null
+                    }, s
                 }
 
-                function kn(t, n) {
-                    return wn(n, t)
+                function Be(t, e) {
+                    return je(e, t)
                 }
 
-                function Fn(t) {
+                function ke(t) {
                     return function() {
                         return !t.apply(this, arguments)
                     }
                 }
 
-                function Nn() {
+                function Fe() {
                     var t = arguments,
-                        n = t.length - 1;
+                        e = t.length - 1;
                     return function() {
-                        for (var e = n, r = t[n].apply(this, arguments); e--;) r = t[e].call(this, r);
+                        for (var n = e, r = t[e].apply(this, arguments); n--;) r = t[n].call(this, r);
                         return r
                     }
                 }
 
-                function Ln(t, n) {
+                function Ne(t, e) {
                     return function() {
-                        if (--t < 1) return n.apply(this, arguments)
+                        if (--t < 1) return e.apply(this, arguments)
                     }
                 }
 
-                function Rn(t, n) {
-                    var e;
+                function Le(t, e) {
+                    var n;
                     return function() {
-                        return --t > 0 && (e = n.apply(this, arguments)), t <= 1 && (n = null), e
+                        return --t > 0 && (n = e.apply(this, arguments)), t <= 1 && (e = null), n
                     }
                 }
-                const Cn = wn(Rn, 2);
+                const Re = je(Le, 2);
 
-                function Un(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r, o = ut(t), i = 0, a = o.length; i < a; i++)
-                        if (n(t[r = o[i]], r, t)) return r
+                function Ce(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r, i = ut(t), o = 0, a = i.length; o < a; o++)
+                        if (e(t[r = i[o]], r, t)) return r
                 }
 
-                function Dn(t) {
-                    return function(n, e, r) {
-                        e = Xt(e, r);
-                        for (var o = it(n), i = t > 0 ? 0 : o - 1; i >= 0 && i < o; i += t)
-                            if (e(n[i], i, n)) return i;
+                function Ue(t) {
+                    return function(e, n, r) {
+                        n = Xt(n, r);
+                        for (var i = ot(e), o = t > 0 ? 0 : i - 1; o >= 0 && o < i; o += t)
+                            if (n(e[o], o, e)) return o;
                         return -1
                     }
                 }
-                const Vn = Dn(1),
-                    Pn = Dn(-1);
+                const De = Ue(1),
+                    Ve = Ue(-1);
 
-                function qn(t, n, e, r) {
-                    for (var o = (e = Xt(e, r, 1))(n), i = 0, a = it(t); i < a;) {
-                        var u = Math.floor((i + a) / 2);
-                        e(t[u]) < o ? i = u + 1 : a = u
+                function Pe(t, e, n, r) {
+                    for (var i = (n = Xt(n, r, 1))(e), o = 0, a = ot(t); o < a;) {
+                        var u = Math.floor((o + a) / 2);
+                        n(t[u]) < i ? o = u + 1 : a = u
                     }
-                    return i
+                    return o
                 }
 
-                function Wn(t, n, e) {
-                    return function(r, o, i) {
+                function qe(t, e, n) {
+                    return function(r, i, o) {
                         var a = 0,
-                            u = it(r);
-                        if ("number" == typeof i) t > 0 ? a = i >= 0 ? i : Math.max(i + u, a) : u = i >= 0 ? Math.min(i + 1, u) : i + u + 1;
-                        else if (e && i && u) return r[i = e(r, o)] === o ? i : -1;
-                        if (o != o) return (i = n(s.call(r, a, u), X)) >= 0 ? i + a : -1;
-                        for (i = t > 0 ? a : u - 1; i >= 0 && i < u; i += t)
-                            if (r[i] === o) return i;
+                            u = ot(r);
+                        if ("number" == typeof o) t > 0 ? a = o >= 0 ? o : Math.max(o + u, a) : u = o >= 0 ? Math.min(o + 1, u) : o + u + 1;
+                        else if (n && o && u) return r[o = n(r, i)] === i ? o : -1;
+                        if (i != i) return (o = e(c.call(r, a, u), X)) >= 0 ? o + a : -1;
+                        for (o = t > 0 ? a : u - 1; o >= 0 && o < u; o += t)
+                            if (r[o] === i) return o;
                         return -1
                     }
                 }
-                const zn = Wn(1, Vn, qn),
-                    $n = Wn(-1, Pn);
+                const We = qe(1, De, Pe),
+                    ze = qe(-1, Ve);
 
-                function Kn(t, n, e) {
-                    var r = (xn(t) ? Vn : Un)(t, n, e);
+                function $e(t, e, n) {
+                    var r = (Ae(t) ? De : Ce)(t, e, n);
                     if (void 0 !== r && -1 !== r) return t[r]
                 }
 
-                function Jn(t, n) {
-                    return Kn(t, Kt(n))
+                function Ke(t, e) {
+                    return $e(t, Kt(e))
                 }
 
-                function Gn(t, n, e) {
-                    var r, o;
-                    if (n = Gt(n, e), xn(t))
-                        for (r = 0, o = t.length; r < o; r++) n(t[r], r, t);
+                function Je(t, e, n) {
+                    var r, i;
+                    if (e = Gt(e, n), Ae(t))
+                        for (r = 0, i = t.length; r < i; r++) e(t[r], r, t);
                     else {
-                        var i = ut(t);
-                        for (r = 0, o = i.length; r < o; r++) n(t[i[r]], i[r], t)
+                        var o = ut(t);
+                        for (r = 0, i = o.length; r < i; r++) e(t[o[r]], o[r], t)
                     }
                     return t
                 }
 
-                function Hn(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = Array(o), a = 0; a < o; a++) {
+                function Ge(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = Array(i), a = 0; a < i; a++) {
                         var u = r ? r[a] : a;
-                        i[a] = n(t[u], u, t)
+                        o[a] = e(t[u], u, t)
                     }
-                    return i
+                    return o
                 }
 
-                function Qn(t) {
-                    var n = function(n, e, r, o) {
-                        var i = !xn(n) && ut(n),
-                            a = (i || n).length,
-                            u = t > 0 ? 0 : a - 1;
-                        for (o || (r = n[i ? i[u] : u], u += t); u >= 0 && u < a; u += t) {
-                            var l = i ? i[u] : u;
-                            r = e(r, n[l], l, n)
-                        }
-                        return r
-                    };
-                    return function(t, e, r, o) {
-                        var i = arguments.length >= 3;
-                        return n(t, Gt(e, o, 4), r, i)
+                function He(t) {
+                    return function(e, n, r, i) {
+                        var o = arguments.length >= 3;
+                        return function(e, n, r, i) {
+                            var o = !Ae(e) && ut(e),
+                                a = (o || e).length,
+                                u = t > 0 ? 0 : a - 1;
+                            for (i || (r = e[o ? o[u] : u], u += t); u >= 0 && u < a; u += t) {
+                                var l = o ? o[u] : u;
+                                r = n(r, e[l], l, e)
+                            }
+                            return r
+                        }(e, Gt(n, i, 4), r, o)
                     }
                 }
-                const Xn = Qn(1),
-                    Yn = Qn(-1);
+                const Qe = He(1),
+                    Xe = He(-1);
 
-                function Zn(t, n, e) {
+                function Ye(t, e, n) {
                     var r = [];
-                    return n = Xt(n, e), Gn(t, (function(t, e, o) {
-                        n(t, e, o) && r.push(t)
+                    return e = Xt(e, n), Je(t, (function(t, n, i) {
+                        e(t, n, i) && r.push(t)
                     })), r
                 }
 
-                function te(t, n, e) {
-                    return Zn(t, Fn(Xt(n)), e)
+                function Ze(t, e, n) {
+                    return Ye(t, ke(Xt(e)), n)
                 }
 
-                function ne(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = 0; i < o; i++) {
-                        var a = r ? r[i] : i;
-                        if (!n(t[a], a, t)) return !1
+                function tn(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = 0; o < i; o++) {
+                        var a = r ? r[o] : o;
+                        if (!e(t[a], a, t)) return !1
                     }
                     return !0
                 }
 
-                function ee(t, n, e) {
-                    n = Xt(n, e);
-                    for (var r = !xn(t) && ut(t), o = (r || t).length, i = 0; i < o; i++) {
-                        var a = r ? r[i] : i;
-                        if (n(t[a], a, t)) return !0
+                function en(t, e, n) {
+                    e = Xt(e, n);
+                    for (var r = !Ae(t) && ut(t), i = (r || t).length, o = 0; o < i; o++) {
+                        var a = r ? r[o] : o;
+                        if (e(t[a], a, t)) return !0
                     }
                     return !1
                 }
 
-                function re(t, n, e, r) {
-                    return xn(t) || (t = Et(t)), ("number" != typeof e || r) && (e = 0), zn(t, n, e) >= 0
+                function nn(t, e, n, r) {
+                    return Ae(t) || (t = Et(t)), ("number" != typeof n || r) && (n = 0), We(t, e, n) >= 0
                 }
-                const oe = x((function(t, n, e) {
-                    var r, o;
-                    return V(n) ? o = n : (n = Pt(n), r = n.slice(0, -1), n = n[n.length - 1]), Hn(t, (function(t) {
-                        var i = o;
-                        if (!i) {
+                const rn = x((function(t, e, n) {
+                    var r, i;
+                    return V(e) ? i = e : (e = Pt(e), r = e.slice(0, -1), e = e[e.length - 1]), Ge(t, (function(t) {
+                        var o = i;
+                        if (!o) {
                             if (r && r.length && (t = qt(t, r)), null == t) return;
-                            i = t[n]
+                            o = t[e]
                         }
-                        return null == i ? i : i.apply(t, e)
+                        return null == o ? o : o.apply(t, n)
                     }))
                 }));
 
-                function ie(t, n) {
-                    return Hn(t, Jt(n))
+                function on(t, e) {
+                    return Ge(t, Jt(e))
                 }
 
-                function ae(t, n) {
-                    return Zn(t, Kt(n))
+                function an(t, e) {
+                    return Ye(t, Kt(e))
                 }
 
-                function ue(t, n, e) {
-                    var r, o, i = -1 / 0,
+                function un(t, e, n) {
+                    var r, i, o = -1 / 0,
                         a = -1 / 0;
-                    if (null == n || "number" == typeof n && "object" != typeof t[0] && null != t)
-                        for (var u = 0, l = (t = xn(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r > i && (i = r);
-                    else n = Xt(n, e), Gn(t, (function(t, e, r) {
-                        ((o = n(t, e, r)) > a || o === -1 / 0 && i === -1 / 0) && (i = t, a = o)
+                    if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
+                        for (var u = 0, l = (t = Ae(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r > o && (o = r);
+                    else e = Xt(e, n), Je(t, (function(t, n, r) {
+                        ((i = e(t, n, r)) > a || i === -1 / 0 && o === -1 / 0) && (o = t, a = i)
                     }));
-                    return i
+                    return o
                 }
 
-                function le(t, n, e) {
-                    var r, o, i = 1 / 0,
+                function ln(t, e, n) {
+                    var r, i, o = 1 / 0,
                         a = 1 / 0;
-                    if (null == n || "number" == typeof n && "object" != typeof t[0] && null != t)
-                        for (var u = 0, l = (t = xn(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r < i && (i = r);
-                    else n = Xt(n, e), Gn(t, (function(t, e, r) {
-                        ((o = n(t, e, r)) < a || o === 1 / 0 && i === 1 / 0) && (i = t, a = o)
+                    if (null == e || "number" == typeof e && "object" != typeof t[0] && null != t)
+                        for (var u = 0, l = (t = Ae(t) ? t : Et(t)).length; u < l; u++) null != (r = t[u]) && r < o && (o = r);
+                    else e = Xt(e, n), Je(t, (function(t, n, r) {
+                        ((i = e(t, n, r)) < a || i === 1 / 0 && o === 1 / 0) && (o = t, a = i)
                     }));
-                    return i
+                    return o
                 }
-                var ce = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
+                var sn = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
 
-                function se(t) {
-                    return t ? K(t) ? s.call(t) : B(t) ? t.match(ce) : xn(t) ? Hn(t, $t) : Et(t) : []
+                function cn(t) {
+                    return t ? K(t) ? c.call(t) : B(t) ? t.match(sn) : Ae(t) ? Ge(t, $t) : Et(t) : []
                 }
 
-                function fe(t, n, e) {
-                    if (null == n || e) return xn(t) || (t = Et(t)), t[en(t.length - 1)];
-                    var r = se(t),
-                        o = it(r);
-                    n = Math.max(Math.min(n, o), 0);
-                    for (var i = o - 1, a = 0; a < n; a++) {
-                        var u = en(a, i),
+                function fn(t, e, n) {
+                    if (null == e || n) return Ae(t) || (t = Et(t)), t[ne(t.length - 1)];
+                    var r = cn(t),
+                        i = ot(r);
+                    e = Math.max(Math.min(e, i), 0);
+                    for (var o = i - 1, a = 0; a < e; a++) {
+                        var u = ne(a, o),
                             l = r[a];
                         r[a] = r[u], r[u] = l
                     }
-                    return r.slice(0, n)
+                    return r.slice(0, e)
                 }
 
-                function pe(t) {
-                    return fe(t, 1 / 0)
+                function hn(t) {
+                    return fn(t, 1 / 0)
                 }
 
-                function he(t, n, e) {
+                function pn(t, e, n) {
                     var r = 0;
-                    return n = Xt(n, e), ie(Hn(t, (function(t, e, o) {
+                    return e = Xt(e, n), on(Ge(t, (function(t, n, i) {
                         return {
                             value: t,
                             index: r++,
-                            criteria: n(t, e, o)
+                            criteria: e(t, n, i)
                         }
-                    })).sort((function(t, n) {
-                        var e = t.criteria,
-                            r = n.criteria;
-                        if (e !== r) {
-                            if (e > r || void 0 === e) return 1;
-                            if (e < r || void 0 === r) return -1
+                    })).sort((function(t, e) {
+                        var n = t.criteria,
+                            r = e.criteria;
+                        if (n !== r) {
+                            if (n > r || void 0 === n) return 1;
+                            if (n < r || void 0 === r) return -1
                         }
-                        return t.index - n.index
+                        return t.index - e.index
                     })), "value")
                 }
 
-                function de(t, n) {
-                    return function(e, r, o) {
-                        var i = n ? [
+                function dn(t, e) {
+                    return function(n, r, i) {
+                        var o = e ? [
                             [],
                             []
                         ] : {};
-                        return r = Xt(r, o), Gn(e, (function(n, o) {
-                            var a = r(n, o, e);
-                            t(i, n, a)
-                        })), i
+                        return r = Xt(r, i), Je(n, (function(e, i) {
+                            var a = r(e, i, n);
+                            t(o, e, a)
+                        })), o
                     }
                 }
-                const ve = de((function(t, n, e) {
-                        J(t, e) ? t[e].push(n) : t[e] = [n]
+                const vn = dn((function(t, e, n) {
+                        J(t, n) ? t[n].push(e) : t[n] = [e]
                     })),
-                    ge = de((function(t, n, e) {
-                        t[e] = n
+                    gn = dn((function(t, e, n) {
+                        t[n] = e
                     })),
-                    ye = de((function(t, n, e) {
-                        J(t, e) ? t[e]++ : t[e] = 1
+                    mn = dn((function(t, e, n) {
+                        J(t, n) ? t[n]++ : t[n] = 1
                     })),
-                    me = de((function(t, n, e) {
-                        t[e ? 0 : 1].push(n)
+                    yn = dn((function(t, e, n) {
+                        t[n ? 0 : 1].push(e)
                     }), !0);
 
-                function _e(t) {
-                    return null == t ? 0 : xn(t) ? t.length : ut(t).length
+                function _n(t) {
+                    return null == t ? 0 : Ae(t) ? t.length : ut(t).length
                 }
 
-                function be(t, n, e) {
-                    return n in e
+                function bn(t, e, n) {
+                    return e in n
                 }
-                const je = x((function(t, n) {
-                        var e = {},
-                            r = n[0];
-                        if (null == t) return e;
-                        V(r) ? (n.length > 1 && (r = Gt(r, n[1])), n = gt(t)) : (r = be, n = On(n, !1, !1), t = Object(t));
-                        for (var o = 0, i = n.length; o < i; o++) {
-                            var a = n[o],
+                const jn = x((function(t, e) {
+                        var n = {},
+                            r = e[0];
+                        if (null == t) return n;
+                        V(r) ? (e.length > 1 && (r = Gt(r, e[1])), e = gt(t)) : (r = bn, e = xe(e, !1, !1), t = Object(t));
+                        for (var i = 0, o = e.length; i < o; i++) {
+                            var a = e[i],
                                 u = t[a];
-                            r(u, a, t) && (e[a] = u)
+                            r(u, a, t) && (n[a] = u)
                         }
-                        return e
+                        return n
                     })),
-                    we = x((function(t, n) {
-                        var e, r = n[0];
-                        return V(r) ? (r = Fn(r), n.length > 1 && (e = n[1])) : (n = Hn(On(n, !1, !1), String), r = function(t, e) {
-                            return !re(n, e)
-                        }), je(t, r, e)
+                    wn = x((function(t, e) {
+                        var n, r = e[0];
+                        return V(r) ? (r = ke(r), e.length > 1 && (n = e[1])) : (e = Ge(xe(e, !1, !1), String), r = function(t, n) {
+                            return !nn(e, n)
+                        }), jn(t, r, n)
                     }));
 
-                function Ae(t, n, e) {
-                    return s.call(t, 0, Math.max(0, t.length - (null == n || e ? 1 : n)))
+                function An(t, e, n) {
+                    return c.call(t, 0, Math.max(0, t.length - (null == e || n ? 1 : e)))
                 }
 
-                function xe(t, n, e) {
-                    return null == t || t.length < 1 ? null == n || e ? void 0 : [] : null == n || e ? t[0] : Ae(t, t.length - n)
+                function xn(t, e, n) {
+                    return null == t || t.length < 1 ? null == e || n ? void 0 : [] : null == e || n ? t[0] : An(t, t.length - e)
                 }
 
-                function Oe(t, n, e) {
-                    return s.call(t, null == n || e ? 1 : n)
+                function On(t, e, n) {
+                    return c.call(t, null == e || n ? 1 : e)
                 }
 
-                function Se(t, n, e) {
-                    return null == t || t.length < 1 ? null == n || e ? void 0 : [] : null == n || e ? t[t.length - 1] : Oe(t, Math.max(0, t.length - n))
+                function Sn(t, e, n) {
+                    return null == t || t.length < 1 ? null == e || n ? void 0 : [] : null == e || n ? t[t.length - 1] : On(t, Math.max(0, t.length - e))
                 }
 
-                function Me(t) {
-                    return Zn(t, Boolean)
+                function Mn(t) {
+                    return Ye(t, Boolean)
                 }
 
-                function Ee(t, n) {
-                    return On(t, n, !1)
+                function En(t, e) {
+                    return xe(t, e, !1)
                 }
-                const Te = x((function(t, n) {
-                        return n = On(n, !0, !0), Zn(t, (function(t) {
-                            return !re(n, t)
+                const Tn = x((function(t, e) {
+                        return e = xe(e, !0, !0), Ye(t, (function(t) {
+                            return !nn(e, t)
                         }))
                     })),
-                    Ie = x((function(t, n) {
-                        return Te(t, n)
+                    In = x((function(t, e) {
+                        return Tn(t, e)
                     }));
 
-                function Be(t, n, e, r) {
-                    E(n) || (r = e, e = n, n = !1), null != e && (e = Xt(e, r));
-                    for (var o = [], i = [], a = 0, u = it(t); a < u; a++) {
+                function Bn(t, e, n, r) {
+                    E(e) || (r = n, n = e, e = !1), null != n && (n = Xt(n, r));
+                    for (var i = [], o = [], a = 0, u = ot(t); a < u; a++) {
                         var l = t[a],
-                            c = e ? e(l, a, t) : l;
-                        n && !e ? (a && i === c || o.push(l), i = c) : e ? re(i, c) || (i.push(c), o.push(l)) : re(o, l) || o.push(l)
+                            s = n ? n(l, a, t) : l;
+                        e && !n ? (a && o === s || i.push(l), o = s) : n ? nn(o, s) || (o.push(s), i.push(l)) : nn(i, l) || i.push(l)
                     }
-                    return o
+                    return i
                 }
-                const ke = x((function(t) {
-                    return Be(On(t, !0, !0))
+                const kn = x((function(t) {
+                    return Bn(xe(t, !0, !0))
                 }));
 
-                function Fe(t) {
-                    for (var n = [], e = arguments.length, r = 0, o = it(t); r < o; r++) {
-                        var i = t[r];
-                        if (!re(n, i)) {
+                function Fn(t) {
+                    for (var e = [], n = arguments.length, r = 0, i = ot(t); r < i; r++) {
+                        var o = t[r];
+                        if (!nn(e, o)) {
                             var a;
-                            for (a = 1; a < e && re(arguments[a], i); a++);
-                            a === e && n.push(i)
+                            for (a = 1; a < n && nn(arguments[a], o); a++);
+                            a === n && e.push(o)
                         }
                     }
-                    return n
+                    return e
                 }
 
-                function Ne(t) {
-                    for (var n = t && ue(t, it).length || 0, e = Array(n), r = 0; r < n; r++) e[r] = ie(t, r);
-                    return e
+                function Nn(t) {
+                    for (var e = t && un(t, ot).length || 0, n = Array(e), r = 0; r < e; r++) n[r] = on(t, r);
+                    return n
                 }
-                const Le = x(Ne);
+                const Ln = x(Nn);
 
-                function Re(t, n) {
-                    for (var e = {}, r = 0, o = it(t); r < o; r++) n ? e[t[r]] = n[r] : e[t[r][0]] = t[r][1];
-                    return e
+                function Rn(t, e) {
+                    for (var n = {}, r = 0, i = ot(t); r < i; r++) e ? n[t[r]] = e[r] : n[t[r][0]] = t[r][1];
+                    return n
                 }
 
-                function Ce(t, n, e) {
-                    null == n && (n = t || 0, t = 0), e || (e = n < t ? -1 : 1);
-                    for (var r = Math.max(Math.ceil((n - t) / e), 0), o = Array(r), i = 0; i < r; i++, t += e) o[i] = t;
-                    return o
+                function Cn(t, e, n) {
+                    null == e && (e = t || 0, t = 0), n || (n = e < t ? -1 : 1);
+                    for (var r = Math.max(Math.ceil((e - t) / n), 0), i = Array(r), o = 0; o < r; o++, t += n) i[o] = t;
+                    return i
                 }
 
-                function Ue(t, n) {
-                    if (null == n || n < 1) return [];
-                    for (var e = [], r = 0, o = t.length; r < o;) e.push(s.call(t, r, r += n));
-                    return e
+                function Un(t, e) {
+                    if (null == e || e < 1) return [];
+                    for (var n = [], r = 0, i = t.length; r < i;) n.push(c.call(t, r, r += e));
+                    return n
                 }
 
-                function De(t, n) {
-                    return t._chain ? st(n).chain() : n
+                function Dn(t, e) {
+                    return t._chain ? ct(e).chain() : e
                 }
 
-                function Ve(t) {
-                    return Gn(Bt(t), (function(n) {
-                        var e = st[n] = t[n];
-                        st.prototype[n] = function() {
+                function Vn(t) {
+                    return Je(Bt(t), (function(e) {
+                        var n = ct[e] = t[e];
+                        ct.prototype[e] = function() {
                             var t = [this._wrapped];
-                            return c.apply(t, arguments), De(this, e.apply(st, t))
+                            return s.apply(t, arguments), Dn(this, n.apply(ct, t))
                         }
-                    })), st
+                    })), ct
                 }
-                Gn(["pop", "push", "reverse", "shift", "sort", "splice", "unshift"], (function(t) {
-                    var n = a[t];
-                    st.prototype[t] = function() {
-                        var e = this._wrapped;
-                        return null != e && (n.apply(e, arguments), "shift" !== t && "splice" !== t || 0 !== e.length || delete e[0]), De(this, e)
-                    }
-                })), Gn(["concat", "join", "slice"], (function(t) {
-                    var n = a[t];
-                    st.prototype[t] = function() {
+                Je(["pop", "push", "reverse", "shift", "sort", "splice", "unshift"], (function(t) {
+                    var e = a[t];
+                    ct.prototype[t] = function() {
+                        var n = this._wrapped;
+                        return null != n && (e.apply(n, arguments), "shift" !== t && "splice" !== t || 0 !== n.length || delete n[0]), Dn(this, n)
+                    }
+                })), Je(["concat", "join", "slice"], (function(t) {
+                    var e = a[t];
+                    ct.prototype[t] = function() {
                         var t = this._wrapped;
-                        return null != t && (t = n.apply(t, arguments)), De(this, t)
+                        return null != t && (t = e.apply(t, arguments)), Dn(this, t)
                     }
                 }));
-                const Pe = st;
-                var qe = Ve(r);
-                qe._ = qe;
-                const We = qe
+                const Pn = ct;
+                var qn = Vn(r);
+                qn._ = qn;
+                const Wn = qn
             }
         },
         r = {};
 
-    function o(t) {
-        var n = r[t];
-        if (void 0 !== n) return n.exports;
-        var i = r[t] = {
+    function i(t) {
+        var e = r[t];
+        if (void 0 !== e) return e.exports;
+        var o = r[t] = {
             exports: {}
         };
-        return e[t](i, i.exports, o), i.exports
+        return n[t](o, o.exports, i), o.exports
     }
-    o.n = t => {
-        var n = t && t.__esModule ? () => t.default : () => t;
-        return o.d(n, {
-            a: n
-        }), n
-    }, o.d = (t, n) => {
-        for (var e in n) o.o(n, e) && !o.o(t, e) && Object.defineProperty(t, e, {
+    i.n = t => {
+        var e = t && t.__esModule ? () => t.default : () => t;
+        return i.d(e, {
+            a: e
+        }), e
+    }, i.d = (t, e) => {
+        for (var n in e) i.o(e, n) && !i.o(t, n) && Object.defineProperty(t, n, {
             enumerable: !0,
-            get: n[e]
+            get: e[n]
         })
-    }, o.o = (t, n) => Object.prototype.hasOwnProperty.call(t, n), o.r = t => {
+    }, i.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), i.r = t => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(t, "__esModule", {
             value: !0
         })
-    }, o.p = "";
-    var i = {};
+    }, i.p = "";
+    var o = {};
     return (() => {
-        var t = o(325);
-        const n = new URL(t.uri, document.location);
-        n.pathname = n.pathname.slice(0, n.pathname.lastIndexOf("/") + 1), o.p = `${n.origin}${n.pathname}`
+        var t = i(325);
+        const e = new URL(t.uri, document.location);
+        e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
-        o.r(i), o.d(i, {
+        i.r(o), i.d(o, {
             AladinModel: () => r,
             AladinView: () => u,
             version: () => l.i8
         });
-        var t = o(146);
-        o(50);
-        const n = (t, n = !0, e = "text/javascript") => new Promise(((r, o) => {
+        var t = i(146);
+        i(50);
+        const e = (t, e = !0, n = "text/javascript") => new Promise(((r, i) => {
             try {
-                const i = document.createElement("script");
-                i.type = e, i.async = n, i.src = t, i.addEventListener("load", (t => {
+                const o = document.createElement("script");
+                o.type = n, o.async = e, o.src = t, o.addEventListener("load", (t => {
                     r({
                         status: !0
                     })
-                })), i.addEventListener("error", (t => {
-                    o({
+                })), o.addEventListener("error", (t => {
+                    i({
                         status: !1,
                         message: "Failed to load the script ＄{FILE_URL}"
                     })
-                })), document.getElementsByTagName("head")[0].appendChild(i)
+                })), document.getElementsByTagName("head")[0].appendChild(o)
             } catch (t) {
-                o(t)
+                i(t)
             }
         }));
-        var e = n("https://code.jquery.com/jquery-3.6.1.min.js").then((() => n("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
+        let n = e("https://code.jquery.com/jquery-3.6.1.min.js").then((() => e("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js"))).then((async () => {
             await A.init
         }));
         class r extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.1",
-                    _view_module_version: "0.2.1"
+                    _model_module_version: "0.2.2",
+                    _view_module_version: "0.2.2"
                 }
             }
         }
-        var a = 0;
+        let a = 0;
         class u extends t.DOMWidgetView {
             render() {
-                e.then((() => {
-                    this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(a), a += 1, this.div.setAttribute("style", "width:100%;height:400px;");
-                    for (var t = {}, n = this.model.get("options"), e = 0; e < n.length; e++) t[this.convert_pyname_to_jsname(n[e])] = this.model.get(n[e]);
-                    new MutationObserver((n => {
-                        n.forEach((n => {
-                            n.addedNodes.forEach((n => {
-                                n.id == this.div.id && setTimeout((() => {
-                                    this.al = A.aladin([this.div], t), this.aladin_events(), this.model_events()
+                n.then((() => {
+                    this.fov_js = !1, this.fov_py = !1, this.target_js = !1, this.target_py = !1, this.div && this.el.remove(this.div), this.div = document.createElement("div"), this.div.id = "aladin-lite-div" + parseInt(a), a += 1;
+                    let t = this.model.get("height");
+                    this.div.setAttribute("style", "width:100%;height:" + t + "px;");
+                    let e = {},
+                        n = this.model.get("options");
+                    for (let t of n) e[this.convert_pyname_to_jsname(t)] = this.model.get(t);
+                    new MutationObserver((t => {
+                        t.forEach((t => {
+                            t.addedNodes.forEach((t => {
+                                t.id == this.div.id && setTimeout((() => {
+                                    this.al = A.aladin([this.div], e), this.aladin_events(), this.model_events()
                                 }), 1e3)
                             }))
                         }))
                     })).observe(this.el, {
                         subtree: !1,
                         childList: !0
                     }), this.el.appendChild(this.div)
                 }))
             }
             convert_pyname_to_jsname(t) {
-                var n, e = t.split("_");
-                for (n = 1; n < e.length; n++) e[n] = e[n].charAt(0).toUpperCase() + e[n].slice(1);
+                let e = t.split("_");
+                for (let t = 1; t < e.length; t++) e[t] = e[t].charAt(0).toUpperCase() + e[t].slice(1);
                 return e.join("")
             }
             aladin_events() {
-                var t = this;
-                this.al.on("zoomChanged", (function(n) {
-                    t.fov_py ? t.fov_py = !1 : (t.fov_js = !0, t.model.set("fov", parseFloat(n.toFixed(5))), t.touch())
-                })), this.al.on("positionChanged", (function(n) {
-                    t.target_py ? t.target_py = !1 : (t.target_js = !0, t.model.set("target", n.ra.toFixed(6) + " " + n.dec.toFixed(6)), t.touch())
+                this.al.on("zoomChanged", (t => {
+                    this.fov_py ? this.fov_py = !1 : (this.fov_js = !0, this.model.set("fov", parseFloat(t.toFixed(5))), this.touch())
+                })), this.al.on("positionChanged", (t => {
+                    this.target_py ? this.target_py = !1 : (this.target_js = !0, this.model.set("target", t.ra.toFixed(6) + " " + t.dec.toFixed(6)), this.touch())
                 }))
             }
             model_events() {
-                var t = this;
-                this.listenTo(this.model, "change:fov", (function() {
-                    t.fov_js ? t.fov_js = !1 : (t.fov_py = !0, t.al.setFoV(t.model.get("fov")))
-                }), this), this.listenTo(this.model, "change:target", (function() {
-                    t.target_js ? t.target_js = !1 : (t.target_py = !0, t.al.gotoObject(t.model.get("target")))
-                }), this), this.listenTo(this.model, "change:coo_frame", (function() {
-                    t.al.setFrame(t.model.get("coo_frame"))
-                }), this), this.listenTo(this.model, "change:survey", (function() {
-                    t.al.setImageSurvey(t.model.get("survey"))
-                }), this), this.listenTo(this.model, "change:overlay_survey", (function() {
-                    t.al.setOverlayImageLayer(t.model.get("overlay_survey"))
-                }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (function() {
-                    t.al.getOverlayImageLayer().setAlpha(t.model.get("overlay_survey_opacity"))
-                }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (function() {
-                    t.al.addCatalog(A.catalogFromURL(t.model.get("votable_URL"), t.model.get("votable_options")))
-                }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (function() {
-                    t.al.addMOC(A.MOCFromURL(t.model.get("moc_URL"), t.model.get("moc_options")))
-                }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (function() {
-                    t.al.addMOC(A.MOCFromJSON(t.model.get("moc_dict"), t.model.get("moc_options")))
-                }), this), this.listenTo(this.model, "change:table_flag", (function() {
-                    var n = A.catalog({
+                this.listenTo(this.model, "change:fov", (() => {
+                    this.fov_js ? this.fov_js = !1 : (this.fov_py = !0, this.al.setFoV(this.model.get("fov")))
+                }), this), this.listenTo(this.model, "change:target", (() => {
+                    this.target_js ? this.target_js = !1 : (this.target_py = !0, this.al.gotoObject(this.model.get("target")))
+                }), this), this.listenTo(this.model, "change:coo_frame", (() => {
+                    this.al.setFrame(this.model.get("coo_frame"))
+                }), this), this.listenTo(this.model, "change:height", (() => {
+                    let t = this.model.get("height");
+                    this.div.setAttribute("style", "width:100%;height:" + t + "px;")
+                }), this), this.listenTo(this.model, "change:survey", (() => {
+                    this.al.setImageSurvey(this.model.get("survey"))
+                }), this), this.listenTo(this.model, "change:overlay_survey", (() => {
+                    this.al.setOverlayImageLayer(this.model.get("overlay_survey"))
+                }), this), this.listenTo(this.model, "change:overlay_survey_opacity", (() => {
+                    this.al.getOverlayImageLayer().setAlpha(this.model.get("overlay_survey_opacity"))
+                }), this), this.listenTo(this.model, "change:votable_from_URL_flag", (() => {
+                    this.al.addCatalog(A.catalogFromURL(this.model.get("votable_URL"), this.model.get("votable_options")))
+                }), this), this.listenTo(this.model, "change:moc_from_URL_flag", (() => {
+                    this.al.addMOC(A.MOCFromURL(this.model.get("moc_URL"), this.model.get("moc_options")))
+                }), this), this.listenTo(this.model, "change:moc_from_dict_flag", (() => {
+                    this.al.addMOC(A.MOCFromJSON(this.model.get("moc_dict"), this.model.get("moc_options")))
+                }), this), this.listenTo(this.model, "change:table_flag", (() => {
+                    let t = A.catalog({
                         onClick: "showTable"
                     });
-                    t.al.addCatalog(n), n.addSourcesAsArray(t.model.get("table_keys"), t.model.get("table_columns"))
-                }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (function() {
-                    var n = A.graphicOverlay(t.model.get("overlay_options"));
-                    t.al.addOverlay(n), n.addFootprints(A.footprintsFromSTCS(t.model.get("stc_string")))
-                }), this), this.listenTo(this.model, "change:listener_flag", (function() {
-                    var n = t.model.get("listener_type");
-                    t.al.on(n, (function(e) {
-                        if ("select" !== n) e && t.send({
+                    this.al.addCatalog(t), t.addSourcesAsArray(this.model.get("table_keys"), this.model.get("table_columns"))
+                }), this), this.listenTo(this.model, "change:overlay_from_stcs_flag", (() => {
+                    let t = A.graphicOverlay(this.model.get("overlay_options"));
+                    this.al.addOverlay(t), t.addFootprints(A.footprintsFromSTCS(this.model.get("stc_string")))
+                }), this), this.listenTo(this.model, "change:listener_flag", (() => {
+                    let t = this.model.get("listener_type");
+                    this.al.on(t, (function(e) {
+                        if ("select" !== t) e && this.send({
                             event: "callback",
-                            type: n,
+                            type: t,
                             data: {
                                 data: e.data,
                                 dec: e.dec,
                                 ra: e.ra,
                                 x: e.x,
                                 y: e.y
                             }
                         });
                         else {
-                            for (var r = e, o = 0; o < t.al.view.catalogs.length; o++) t.al.view.catalogs[o].deselectAll();
-                            var i = [];
-                            for (o = 0; o < r.length; o++) {
-                                var a = r[o];
-                                a.select(), i.push({
-                                    data: a.data,
-                                    dec: a.dec,
-                                    ra: a.ra,
-                                    x: a.x,
-                                    y: a.y
-                                })
-                            }
-                            t.send({
+                            let n = e;
+                            for (let t of this.al.view.catalogs) t.deselectAll();
+                            let r = [];
+                            for (let t of n) t.select(), r.push({
+                                data: t.data,
+                                dec: t.dec,
+                                ra: t.ra,
+                                x: t.x,
+                                y: t.y
+                            });
+                            this.send({
                                 event: "callback",
-                                type: n,
-                                data: i
+                                type: t,
+                                data: r
                             })
                         }
                     }))
-                }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (function() {
-                    t.al.select()
-                })), this.listenTo(this.model, "change:thumbnail_flag", (function() {
-                    t.al.exportAsPNG()
-                })), this.listenTo(this.model, "change:color_map_flag", (function() {
-                    const n = t.model.get("color_map_name");
-                    t.al.getBaseImageLayer().setColormap(n)
+                }), this), this.listenTo(this.model, "change:rectangular_selection_flag", (() => {
+                    this.al.select()
+                })), this.listenTo(this.model, "change:thumbnail_flag", (() => {
+                    this.al.exportAsPNG()
+                })), this.listenTo(this.model, "change:color_map_flag", (() => {
+                    const t = this.model.get("color_map_name");
+                    this.al.getBaseImageLayer().setColormap(t)
                 }))
             }
         }
         const l = {
-            i8: "0.2.1"
+            i8: "0.2.2"
         }
-    })(), i
+    })(), o
 })()));
```

### Comparing `ipyaladin-0.2.1/js/lib/jupyter-aladin.js` & `ipyaladin-0.2.2/js/lib/jupyter-aladin.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     DOMWidgetModel,
     DOMWidgetView
 } from '@jupyter-widgets/base';
 // Allow us to use the DOMWidgetView base class for our models/views.
 // Additionnaly, this is where we put by default all the external libraries
 // fetched by using webpack (see webpack.config.js file).
-var _ = require("underscore");
+let _ = require("underscore");
 // The sole purpose of this module is to load the css stylesheet when the first instance
 // of the AladinLite widget
 const loadScript = (FILE_URL, async = true, type = "text/javascript") => {
     return new Promise((resolve, reject) => {
         try {
             const scriptEle = document.createElement("script");
             scriptEle.type = type;
@@ -31,15 +31,15 @@
 
             document.getElementsByTagName("head")[0].appendChild(scriptEle);
         } catch (error) {
             reject(error);
         }
     });
 };
-var AladinLiteJS_Loader = loadScript("https://code.jquery.com/jquery-3.6.1.min.js")
+let AladinLiteJS_Loader = loadScript("https://code.jquery.com/jquery-3.6.1.min.js")
     .then(() => {
         return loadScript("https://aladin.u-strasbg.fr/AladinLite/api/v3/latest/aladin.js")
     })
     .then(async () => {
         await A.init;
     });
 
@@ -67,22 +67,22 @@
             ...super.defaults(),
             _model_name: 'AladinModel',
             _view_name: 'AladinView',
 
             _model_module: 'ipyaladin',
             _view_module: 'ipyaladin',
 
-            _model_module_version: '0.2.1',
-            _view_module_version: '0.2.1',
+            _model_module_version: '0.2.2',
+            _view_module_version: '0.2.2',
         };
     }
 }
 
 
-var idxView = 0;
+let idxView = 0;
 export class AladinView extends DOMWidgetView {
     render() {
         // We load the aladin lite script
         AladinLiteJS_Loader.then(() => {
             this.fov_js = false;
             this.fov_py = false;
             this.target_js = false;
@@ -95,22 +95,23 @@
             if (this.div) {
                 this.el.remove(this.div);
             }
 
             this.div = document.createElement('div');
             this.div.id = 'aladin-lite-div' + parseInt(idxView);
             idxView += 1;
-            // TODO: should this style be somehow inherited from the widget Layout attribute?
-            this.div.setAttribute("style", "width:100%;height:400px;");
+            // creates the div section, height is fixed by the user or defaults to 400px
+            let height = this.model.get("height");
+            this.div.setAttribute("style", "width:100%;height:" + height + "px;");
 
             // We get the options set on the python side and create an instance of the AladinLite object.
-            var aladin_options = {};
-            var opt = this.model.get('options');
-            for (var i = 0; i < opt.length; i++) {
-                aladin_options[this.convert_pyname_to_jsname(opt[i])] = this.model.get(opt[i]);
+            let aladin_options = {};
+            let options = this.model.get('options');
+            for (let option of options) {
+                aladin_options[this.convert_pyname_to_jsname(option)] = this.model.get(option);
             }
 
             // Observer triggered when this.el has been changed
             const observer = new MutationObserver((mutations_list) => {
                 mutations_list.forEach((mutation) => {
                     mutation.addedNodes.forEach((added_node) => {
                         if (added_node.id == this.div.id) {
@@ -138,162 +139,163 @@
             });
 
             this.el.appendChild(this.div);
         })
     }
 
     convert_pyname_to_jsname(pyname) {
-        var i, temp = pyname.split('_');
-        for (i = 1; i < temp.length; i++) {
+        let temp = pyname.split('_');
+        for (let i = 1; i < temp.length; i++) {
             temp[i] = temp[i].charAt(0).toUpperCase() + temp[i].slice(1);
         }
         return temp.join('');
     }
 
     aladin_events() {
-        var that = this;
-        this.al.on('zoomChanged', function(fov) {
-            if (!that.fov_py) {
-                that.fov_js = true;
+        this.al.on('zoomChanged', (fov) => {
+            if (!this.fov_py) {
+                this.fov_js = true;
                 // fov MUST be cast into float in order to be sent to the model
-                that.model.set('fov', parseFloat(fov.toFixed(5)));
+                this.model.set('fov', parseFloat(fov.toFixed(5)));
                 // Note: touch function must be called after calling the model's set method
-                that.touch();
+                this.touch();
             } else {
-                that.fov_py = false;
+                this.fov_py = false;
             }
         });
-        this.al.on('positionChanged', function(position) {
-            if (!that.target_py) {
-                that.target_js = true;
-                that.model.set('target', '' + position.ra.toFixed(6) + ' ' + position.dec.toFixed(6));
-                that.touch();
+        this.al.on('positionChanged', (position) => {
+            if (!this.target_py) {
+                this.target_js = true;
+                this.model.set('target', '' + position.ra.toFixed(6) + ' ' + position.dec.toFixed(6));
+                this.touch();
             } else {
-                that.target_py = false;
+                this.target_py = false;
             }
         });
     }
 
     model_events() {
-        var that = this;
         // Model's class parameters listeners
-        this.listenTo(this.model, 'change:fov', function() {
-            if (!that.fov_js) {
-                that.fov_py = true;
-                that.al.setFoV(that.model.get('fov'));
+        this.listenTo(this.model, 'change:fov', () => {
+            if (!this.fov_js) {
+                this.fov_py = true;
+                this.al.setFoV(this.model.get('fov'));
             } else {
-                that.fov_js = false;
+                this.fov_js = false;
             }
         }, this);
-        this.listenTo(this.model, 'change:target', function() {
-            if (!that.target_js) {
-                that.target_py = true;
-                that.al.gotoObject(that.model.get('target'));
+        this.listenTo(this.model, 'change:target', () => {
+            if (!this.target_js) {
+                this.target_py = true;
+                this.al.gotoObject(this.model.get('target'));
             } else {
-                that.target_js = false;
+                this.target_js = false;
             }
         }, this);
-        this.listenTo(this.model, 'change:coo_frame', function() {
-            that.al.setFrame(that.model.get('coo_frame'));
+        this.listenTo(this.model, 'change:coo_frame', () => {
+            this.al.setFrame(this.model.get('coo_frame'));
         }, this);
-        this.listenTo(this.model, 'change:survey', function() {
-            that.al.setImageSurvey(that.model.get('survey'));
+        this.listenTo(this.model, 'change:height', () => {
+            let height = this.model.get('height');
+            this.div.setAttribute("style", "width:100%;height:" + height + "px;");
         }, this);
-        this.listenTo(this.model, 'change:overlay_survey', function() {
-            that.al.setOverlayImageLayer(that.model.get('overlay_survey'));
+        this.listenTo(this.model, 'change:survey', () => {
+            this.al.setImageSurvey(this.model.get('survey'));
         }, this);
-        this.listenTo(this.model, 'change:overlay_survey_opacity', function() {
-            that.al.getOverlayImageLayer().setAlpha(that.model.get('overlay_survey_opacity'));
+        this.listenTo(this.model, 'change:overlay_survey', () => {
+            this.al.setOverlayImageLayer(this.model.get('overlay_survey'));
+        }, this);
+        this.listenTo(this.model, 'change:overlay_survey_opacity', () => {
+            this.al.getOverlayImageLayer().setAlpha(this.model.get('overlay_survey_opacity'));
         }, this);
 
         // Model's functions parameters listeners
-        this.listenTo(this.model, 'change:votable_from_URL_flag', function() {
-            that.al.addCatalog(A.catalogFromURL(that.model.get('votable_URL'), that.model.get('votable_options')));
+        this.listenTo(this.model, 'change:votable_from_URL_flag', () => {
+            this.al.addCatalog(A.catalogFromURL(this.model.get('votable_URL'), this.model.get('votable_options')));
         }, this);
 
-        this.listenTo(this.model, 'change:moc_from_URL_flag', function() {
-            that.al.addMOC(A.MOCFromURL(that.model.get('moc_URL'), that.model.get('moc_options')));
+        this.listenTo(this.model, 'change:moc_from_URL_flag', () => {
+            this.al.addMOC(A.MOCFromURL(this.model.get('moc_URL'), this.model.get('moc_options')));
         }, this);
 
-        this.listenTo(this.model, 'change:moc_from_dict_flag', function() {
-            that.al.addMOC(A.MOCFromJSON(that.model.get('moc_dict'), that.model.get('moc_options')));
+        this.listenTo(this.model, 'change:moc_from_dict_flag', () => {
+            this.al.addMOC(A.MOCFromJSON(this.model.get('moc_dict'), this.model.get('moc_options')));
         }, this);
 
-        this.listenTo(this.model, 'change:table_flag', function() {
-            var cat = A.catalog({
+        this.listenTo(this.model, 'change:table_flag', () => {
+            let cat = A.catalog({
                 onClick: 'showTable'
             });
-            that.al.addCatalog(cat);
-            cat.addSourcesAsArray(that.model.get('table_keys'), that.model.get('table_columns'))
+            this.al.addCatalog(cat);
+            cat.addSourcesAsArray(this.model.get('table_keys'), this.model.get('table_columns'))
         }, this);
 
-        this.listenTo(this.model, 'change:overlay_from_stcs_flag', function() {
-            var overlay = A.graphicOverlay(that.model.get('overlay_options'));
-            that.al.addOverlay(overlay);
-            overlay.addFootprints(A.footprintsFromSTCS(that.model.get('stc_string')));
+        this.listenTo(this.model, 'change:overlay_from_stcs_flag', () => {
+            let overlay = A.graphicOverlay(this.model.get('overlay_options'));
+            this.al.addOverlay(overlay);
+            overlay.addFootprints(A.footprintsFromSTCS(this.model.get('stc_string')));
         }, this);
 
-        this.listenTo(this.model, 'change:listener_flag', function() {
-            var type = that.model.get('listener_type');
-            that.al.on(type, function(object) {
+        this.listenTo(this.model, 'change:listener_flag', () => {
+            let type = this.model.get('listener_type');
+            this.al.on(type, function(object) {
                 if (type === 'select') {
-                    var sources = object;
+                    let sources = object;
                     // first, deselect previously selected sources
-                    for (var k = 0; k < that.al.view.catalogs.length; k++) {
-                        that.al.view.catalogs[k].deselectAll();
+                    for (let catalog of this.al.view.catalogs) {
+                        catalog.deselectAll();
                     }
-                    var sourcesData = [];
-                    for (var k = 0; k < sources.length; k++) {
-                        var source = sources[k];
+                    let sourcesData = [];
+                    for (let source of sources) {
                         source.select();
                         sourcesData.push({
                             data: source.data,
                             dec: source.dec,
                             ra: source.ra,
                             x: source.x,
                             y: source.y
                         });
                     }
-                    that.send({
+                    this.send({
                         'event': 'callback',
                         'type': type,
                         'data': sourcesData,
                     });
 
                     return;
 
                 }
 
                 // Send json object to the python-side of the application
                 // We only send object.data because the whole object possess a catalog attribute
                 // that cause error when trying to convert it into json
                 // (at least on chrome, due to object circularization)
                 if (object) {
-                    that.send({
+                    this.send({
                         'event': 'callback',
                         'type': type,
                         'data': {
                             'data': object.data,
                             'dec': object.dec,
                             'ra': object.ra,
                             'x': object.x,
                             'y': object.y
                         }
                     });
                 }
             });
         }, this);
 
-        this.listenTo(this.model, 'change:rectangular_selection_flag', function() {
-            that.al.select();
+        this.listenTo(this.model, 'change:rectangular_selection_flag', () => {
+            this.al.select();
         });
 
-        this.listenTo(this.model, 'change:thumbnail_flag', function() {
-            that.al.exportAsPNG();
+        this.listenTo(this.model, 'change:thumbnail_flag', () => {
+            this.al.exportAsPNG();
         });
 
-        this.listenTo(this.model, 'change:color_map_flag', function() {
-            const cmap = that.model.get('color_map_name');
-            that.al.getBaseImageLayer().setColormap(cmap);
+        this.listenTo(this.model, 'change:color_map_flag', () => {
+            const cmap = this.model.get('color_map_name');
+            this.al.getBaseImageLayer().setColormap(cmap);
         });
     }
 }
```

### Comparing `ipyaladin-0.2.1/js/package.json` & `ipyaladin-0.2.2/js/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^3.0.0 || ^4.0.0'}",*

 * * "'files'": '{delete: [0]}',*

 * * "'main'": "'dist/index.js'",*

 * * "'module'": "'dist/index.js'",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -2,20 +2,19 @@
     "author": "Thomas Boch, Jerome Desroziers and Matthieu Baumann",
     "dependencies": {
         "@jupyter-widgets/base": "^1.1 || ^2 || ^3 || ^4 || ^6",
         "underscore": "^1.13.6"
     },
     "description": "ipyaladin",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^3.0.0 || ^4.0.0",
         "rimraf": "^2.6.1",
         "webpack": "^5"
     },
     "files": [
-        "lib/**/*.js",
         "dist/*.js"
     ],
     "jupyterlab": {
         "extension": "lib/labplugin",
         "outputDir": "../ipyaladin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
@@ -28,15 +27,16 @@
         "jupyter",
         "widgets",
         "ipython",
         "ipywidgets",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
-    "main": "lib/index.js",
+    "main": "dist/index.js",
+    "module": "dist/index.js",
     "name": "ipyaladin",
     "repository": {
         "type": "git",
         "url": "https://github.com/cds-astro/ipyaladin.git"
     },
     "scripts": {
         "build": "webpack --mode=development && yarn run build:labextension:dev",
@@ -44,9 +44,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../ipyaladin/labextension/ && rimraf ../ipyaladin/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `ipyaladin-0.2.1/js/webpack.config.js` & `ipyaladin-0.2.2/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/setup.cfg` & `ipyaladin-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.1/setup.py` & `ipyaladin-0.2.2/setup.py`

 * *Files identical despite different names*


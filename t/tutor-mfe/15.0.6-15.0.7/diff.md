# Comparing `tmp/tutor-mfe-15.0.6.tar.gz` & `tmp/tutor-mfe-15.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-mfe-15.0.6.tar", last modified: Thu May 11 13:02:07 2023, max compression
+gzip compressed data, was "dist/tutor-mfe-15.0.7.tar", last modified: Fri May 26 15:34:40 2023, max compression
```

## Comparing `tutor-mfe-15.0.6.tar` & `tutor-mfe-15.0.7.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)    15467 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)    14405 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1849 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)    15467 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1174 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        9 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/
--rw-r--r--   0 ci        (1000) ci        (1000)       24 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)      333 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      605 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      168 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      130 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      460 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/local-docker-compose-prod-services
--rw-r--r--   0 ci        (1000) ci        (1000)      476 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-cms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-cms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      356 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3124 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3615 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     5356 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)      629 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/Caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      749 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)     3700 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     1489 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     3717 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)    15577 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)    14515 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1849 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)    15577 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1189 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        9 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutor_mfe.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)       24 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)      333 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      605 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      168 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      130 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      460 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/local-docker-compose-prod-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      476 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-cms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-cms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      357 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3306 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3796 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     5356 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutormfe/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:39.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)      629 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/Caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      749 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3700 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     1489 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-26 15:34:40.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3717 2023-05-26 15:34:30.000000 tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/init
```

### Comparing `tutor-mfe-15.0.6/LICENSE.txt` & `tutor-mfe-15.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/PKG-INFO` & `tutor-mfe-15.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.6
+Version: 15.0.7
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
@@ -43,15 +43,15 @@
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-mfe
+    tutor plugins install mfe
 
 Usage
 -----
 
 To enable this plugin, run::
 
     tutor plugins enable mfe
@@ -177,42 +177,44 @@
     tutor local start -d
 
 Your custom translation strings should now appear in your app.
 
 Customising MFEs
 ~~~~~~~~~~~~~~~~
 
-To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
+To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `mfe-lms-production-settings` and `mfe-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_items(
         [
             (
-                "openedx-lms-development-settings",
+                "mfe-lms-development-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
             (
-                "openedx-lms-production-settings",
+                "mfe-lms-production-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
         ]
     )
 
+If patches are the same in development and production, they can be replaced by a single `mfe-lms-common-settings` patch.
+
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_item(
         (
```

### Comparing `tutor-mfe-15.0.6/README.rst` & `tutor-mfe-15.0.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-mfe
+    tutor plugins install mfe
 
 Usage
 -----
 
 To enable this plugin, run::
 
     tutor plugins enable mfe
@@ -150,42 +150,44 @@
     tutor local start -d
 
 Your custom translation strings should now appear in your app.
 
 Customising MFEs
 ~~~~~~~~~~~~~~~~
 
-To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
+To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `mfe-lms-production-settings` and `mfe-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_items(
         [
             (
-                "openedx-lms-development-settings",
+                "mfe-lms-development-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
             (
-                "openedx-lms-production-settings",
+                "mfe-lms-production-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
         ]
     )
 
+If patches are the same in development and production, they can be replaced by a single `mfe-lms-common-settings` patch.
+
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_item(
         (
```

### Comparing `tutor-mfe-15.0.6/setup.py` & `tutor-mfe-15.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutor_mfe.egg-info/PKG-INFO` & `tutor-mfe-15.0.7/tutor_mfe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.6
+Version: 15.0.7
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
@@ -43,15 +43,15 @@
 Instructions for using each of these MFEs are given below.
 
 Installation
 ------------
 
 ::
 
-    pip install tutor-mfe
+    tutor plugins install mfe
 
 Usage
 -----
 
 To enable this plugin, run::
 
     tutor plugins enable mfe
@@ -177,42 +177,44 @@
     tutor local start -d
 
 Your custom translation strings should now appear in your app.
 
 Customising MFEs
 ~~~~~~~~~~~~~~~~
 
-To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
+To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `mfe-lms-production-settings` and `mfe-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_items(
         [
             (
-                "openedx-lms-development-settings",
+                "mfe-lms-development-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
             (
-                "openedx-lms-production-settings",
+                "mfe-lms-production-settings",
                 """
         MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
         MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
         MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
         MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
         """
             ),
         ]
     )
 
+If patches are the same in development and production, they can be replaced by a single `mfe-lms-common-settings` patch.
+
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
     hooks.Filters.ENV_PATCHES.add_item(
         (
```

### Comparing `tutor-mfe-15.0.6/tutor_mfe.egg-info/SOURCES.txt` & `tutor-mfe-15.0.7/tutor_mfe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_mfe.egg-info/PKG-INFO
 tutor_mfe.egg-info/SOURCES.txt
 tutor_mfe.egg-info/dependency_links.txt
 tutor_mfe.egg-info/entry_points.txt
 tutor_mfe.egg-info/requires.txt
 tutor_mfe.egg-info/top_level.txt
```

### Comparing `tutor-mfe-15.0.6/tutormfe/patches/k8s-deployments` & `tutor-mfe-15.0.7/tutormfe/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-development-settings` & `tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-development-settings`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 {% endfor %}
 
 # Dynamic config API settings
 # https://openedx.github.io/frontend-platform/module-Config.html
 MFE_CONFIG = {
     "BASE_URL": "{{ MFE_HOST }}",
     "CSRF_TOKEN_API_PATH": "/csrf/api/v1/token",
+{%- if MFE_ACCOUNT_MFE_APP %}
+    "ACCOUNT_SETTINGS_URL": ACCOUNT_MICROFRONTEND_URL,
+{%- endif %}
 {%- if MFE_PROFILE_MFE_APP %}
     "ACCOUNT_PROFILE_URL": "http://{{ MFE_HOST }}:{{ MFE_PROFILE_MFE_APP["port"] }}",
 {%- endif %}
     "CREDENTIALS_BASE_URL": "",
     "DISCOVERY_API_BASE_URL": "{% if DISCOVERY_HOST is defined %}http://{{ DISCOVERY_HOST }}:8381{% endif %}",
     "FAVICON_URL": "http://{{ LMS_HOST }}/favicon.ico",
     "LANGUAGE_PREFERENCE_COOKIE_NAME": "openedx-language-preference",
@@ -58,7 +61,10 @@
     "ENABLE_NEW_EDITOR_PAGES": True,
     "ENABLE_PROGRESS_GRAPH_SETTINGS": True,
 {%- endif %}
 {%- if MFE_AUTHN_MFE_APP %}
     "DISABLE_ENTERPRISE_LOGIN": True,
 {%- endif %}
 }
+
+{{ patch("mfe-lms-common-settings") }}
+{{ patch("mfe-lms-development-settings") }}
```

### Comparing `tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-production-settings` & `tutor-mfe-15.0.7/tutormfe/patches/openedx-lms-production-settings`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 CSRF_TRUSTED_ORIGINS.append("{{ MFE_HOST }}")
 
 # Dynamic config API settings
 # https://openedx.github.io/frontend-platform/module-Config.html
 MFE_CONFIG = {
     "BASE_URL": "{{ MFE_HOST }}",
     "CSRF_TOKEN_API_PATH": "/csrf/api/v1/token",
+{%- if MFE_ACCOUNT_MFE_APP %}
+    "ACCOUNT_SETTINGS_URL": ACCOUNT_MICROFRONTEND_URL,
+{%- endif %}
 {%- if MFE_PROFILE_MFE_APP %}
     "ACCOUNT_PROFILE_URL": "{% if ENABLE_HTTPS %}https://{% else %}http://{% endif %}{{ MFE_HOST }}/{{ MFE_PROFILE_MFE_APP["name"] }}",
 {%- endif %}
     "CREDENTIALS_BASE_URL": "",
     "DISCOVERY_API_BASE_URL": "{% if DISCOVERY_HOST is defined %}{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ DISCOVERY_HOST }}{% endif %}",
     "FAVICON_URL": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}/favicon.ico",
     "LANGUAGE_PREFERENCE_COOKIE_NAME": "openedx-language-preference",
@@ -55,7 +58,10 @@
     "ENABLE_NEW_EDITOR_PAGES": True,
     "ENABLE_PROGRESS_GRAPH_SETTINGS": True,
 {%- endif %}
 {%- if MFE_AUTHN_MFE_APP %}
     "DISABLE_ENTERPRISE_LOGIN": True,
 {%- endif %}
 }
+
+{{ patch("mfe-lms-common-settings") }}
+{{ patch("mfe-lms-production-settings") }}
```

### Comparing `tutor-mfe-15.0.6/tutormfe/plugin.py` & `tutor-mfe-15.0.7/tutormfe/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/Caddyfile` & `tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js` & `tutor-mfe-15.0.7/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/Dockerfile` & `tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js` & `tutor-mfe-15.0.7/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/init` & `tutor-mfe-15.0.7/tutormfe/templates/mfe/tasks/lms/init`

 * *Files identical despite different names*


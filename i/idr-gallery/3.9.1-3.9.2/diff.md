# Comparing `tmp/idr-gallery-3.9.1.tar.gz` & `tmp/idr-gallery-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idr-gallery-3.9.1.tar", last modified: Fri Feb  3 11:58:17 2023, max compression
+gzip compressed data, was "idr-gallery-3.9.2.tar", last modified: Thu Mar  9 16:36:45 2023, max compression
```

## Comparing `idr-gallery-3.9.1.tar` & `idr-gallery-3.9.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery/__pycache__/version.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/data/
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/data/background_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/data/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/gallery_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/
--rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    38388 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   121220 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   245960 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    99961 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62927 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/
--rw-r--r--   0 runner    (1001) docker     (123)    55258 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    29110 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/foundation/
--rw-r--r--   0 runner    (1001) docker     (123)    78738 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   107910 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/categories.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/idr.css
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/openmicroscopy.css
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/search_form_styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/logo-idr-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/omero.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/transparent.png
--rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/model.js
--rw-r--r--   0 runner    (1001) docker     (123)    33882 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/omero_search_form.js
--rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/static/idr_gallery/studies.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/background_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/mapr_search.html
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/idr_gallery/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 11:58:17.442875 idr-gallery-3.9.1/idr_gallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-03 11:58:17.000000 idr-gallery-3.9.1/idr_gallery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-03 11:58:17.446875 idr-gallery-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-02-03 11:58:11.000000 idr-gallery-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/data/background_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/data/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/gallery_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    38388 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121220 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   245960 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    99961 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62927 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    55258 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29110 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)    78738 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   107910 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/autocomplete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/categories.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/idr.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/openmicroscopy.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/search_form_styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/logo-idr-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/omero.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/model.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33882 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/omero_search_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23353 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/static/idr_gallery/studies.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.870360 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/background_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/mapr_search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/idr_gallery/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 16:36:45.866361 idr-gallery-3.9.2/idr_gallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 16:36:45.000000 idr-gallery-3.9.2/idr_gallery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 16:36:45.874360 idr-gallery-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-09 16:36:43.000000 idr-gallery-3.9.2/setup.py
```

### Comparing `idr-gallery-3.9.1/LICENSE` & `idr-gallery-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/PKG-INFO` & `idr-gallery-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: idr-gallery
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/IDR/idr-gallery
-Download-URL: https://github.com/IDR/idr-gallery/archive/v3.9.1.tar.gz
+Download-URL: https://github.com/IDR/idr-gallery/archive/v3.9.2.tar.gz
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
 Keywords: OMERO.web,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `idr-gallery-3.9.1/README.rst` & `idr-gallery-3.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/apps.py` & `idr-gallery-3.9.2/idr_gallery/apps.py`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/data/background_images.py` & `idr-gallery-3.9.2/idr_gallery/data/background_images.py`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/data/tabs.py` & `idr-gallery-3.9.2/idr_gallery/data/tabs.py`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/gallery_settings.py` & `idr-gallery-3.9.2/idr_gallery/gallery_settings.py`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/3rdparty/foundation/foundation.min.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/autocomplete.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/autocomplete.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/categories.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/categories.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/idr.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/idr.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/openmicroscopy.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/openmicroscopy.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/css/search_form_styles.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/css/search_form_styles.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/favicon.ico` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/logo-idr-dark.svg` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/logo-idr-dark.svg`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/omero.svg` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/omero.svg`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/images/transparent.png` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/images/transparent.png`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/model.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/model.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/omero_search_form.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/omero_search_form.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/search.js` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/search.js`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/static/idr_gallery/studies.css` & `idr-gallery-3.9.2/idr_gallery/static/idr_gallery/studies.css`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/background_carousel.html` & `idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/background_carousel.html`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/base.html` & `idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/base.html`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/index.html` & `idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/index.html`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/mapr_search.html` & `idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/mapr_search.html`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/templates/idr_gallery/search.html` & `idr-gallery-3.9.2/idr_gallery/templates/idr_gallery/search.html`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/urls.py` & `idr-gallery-3.9.2/idr_gallery/urls.py`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/idr_gallery/views.py` & `idr-gallery-3.9.2/idr_gallery/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from django.http import HttpResponseRedirect
+from django.http import HttpResponseRedirect, HttpResponseBadRequest
 from django.urls import reverse, NoReverseMatch
 import json
 import logging
 import base64
 import urllib
 
 import omero
@@ -46,14 +46,15 @@
     Home page shows a list of groups OR a set of 'categories' from
     user-configured queries.
     """
 
     # template is different for '/search' page
     template = "idr_gallery/index.html"
     if "search" in request.path:
+        template = "idr_gallery/search.html"
         query = request.GET.get("query")
         # Handle old URLs e.g. ?query=mapr_gene:PAX7
         if query:
             # if 'mapr' search, redirect to searchengine page
             if query.startswith("mapr_"):
                 keyval = find_mapr_key_value(request, query)
                 if keyval is not None:
@@ -62,25 +63,26 @@
                     return redirect_with_params('idr_gallery_search',
                                                 key=keyval[0],
                                                 value=keyval[1],
                                                 operator="contains")
             # handle e.g. ?query=Publication%20Authors:smith
             # ?key=Publication+Authors&value=Smith&operator=contains&resource=container
             keyval = query.split(":", 1)
-            # search for studies ("containers") and use "contains"
-            # to match previous behaviour
-            # NB: 'Name' needs to be 'name' for search-engine
-            key = "name" if keyval[0] == "Name" else keyval[0]
-            return redirect_with_params('idr_gallery_search',
-                                        key=key,
-                                        value=keyval[1],
-                                        resource="container",
-                                        operator="contains")
-        else:
-            template = "idr_gallery/search.html"
+            if len(keyval) > 1 and len(keyval[1]) > 0:
+                # search for studies ("containers") and use "contains"
+                # to match previous behaviour
+                # NB: 'Name' needs to be 'name' for search-engine
+                key = "name" if keyval[0] == "Name" else keyval[0]
+                return redirect_with_params('idr_gallery_search',
+                                            key=key,
+                                            value=keyval[1],
+                                            resource="container",
+                                            operator="contains")
+            return HttpResponseBadRequest(
+                "Query should be ?query=key:value format")
     context = {'template': template}
     context["idr_images"] = IDR_IMAGES
     if super_category == "cell":
         context["idr_images"] = CELL_IMAGES
     elif super_category == "tissue":
         context["idr_images"] = TISSUE_IMAGES
     category = settings.SUPER_CATEGORIES.get(super_category)
@@ -94,15 +96,17 @@
     settings_ctx = get_settings_as_context()
     context = {**context, **settings_ctx}
 
     return context
 
 
 def find_mapr_key_value(request, query):
-    key_val = query.split(":")
+    key_val = query.split(":", 1)
+    if len(key_val) < 2:
+        return None
     mapr_key = key_val[0].replace("mapr_", "")
     mapr_value = key_val[1]
     if mapr_settings and mapr_key in mapr_settings.MAPR_CONFIG:
         if len(key_val) > 0:
             # Key could be e.g. 'Gene Symbol' or 'Gene Identifier'
             mapr_config = mapr_settings.MAPR_CONFIG
             all_keys = mapr_config[mapr_key]["all"]
@@ -110,16 +114,19 @@
             # if multiple keys e.g. 'Gene Symbol' or 'Gene Identifier'
             if len(all_keys) > 1:
                 # need to check which Key matches the Value...
                 matching_keys = search_engine_keys(request, mapr_value)
                 all_keys = [key for key in all_keys if key in matching_keys]
             if len(all_keys) > 1 and default_key in all_keys:
                 mapann_key = default_key
-            else:
+            elif len(all_keys) == 1:
                 mapann_key = all_keys[0]
+            else:
+                # no matches -> use default
+                mapann_key = default_key
         return mapann_key, mapr_value
     return None
 
 
 def search_engine_keys(request, value):
     # find keys that are match the given value
     if settings.BASE_URL is not None:
```

### Comparing `idr-gallery-3.9.1/idr_gallery.egg-info/PKG-INFO` & `idr-gallery-3.9.2/idr_gallery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: idr-gallery
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/IDR/idr-gallery
-Download-URL: https://github.com/IDR/idr-gallery/archive/v3.9.1.tar.gz
+Download-URL: https://github.com/IDR/idr-gallery/archive/v3.9.2.tar.gz
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
 Keywords: OMERO.web,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `idr-gallery-3.9.1/idr_gallery.egg-info/SOURCES.txt` & `idr-gallery-3.9.2/idr_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idr-gallery-3.9.1/setup.py` & `idr-gallery-3.9.2/setup.py`

 * *Files identical despite different names*


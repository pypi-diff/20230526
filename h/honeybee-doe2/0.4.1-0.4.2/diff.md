# Comparing `tmp/honeybee-doe2-0.4.1.tar.gz` & `tmp/honeybee-doe2-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.4.1.tar", last modified: Tue May 23 15:50:03 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.4.2.tar", last modified: Fri May 26 01:07:28 2023, max compression
```

## Comparing `honeybee-doe2-0.4.1.tar` & `honeybee-doe2-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 15:50:02.000000 honeybee-doe2-0.4.1/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 15:50:03.000000 honeybee-doe2-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 15:48:50.000000 honeybee-doe2-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/setup.py
```

### Comparing `honeybee-doe2-0.4.1/LICENSE` & `honeybee-doe2-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/PKG-INFO` & `honeybee-doe2-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.4.1/README.md` & `honeybee-doe2-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.4.2/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.4.2/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.4.2/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,19 @@
     @property
     def stories(self):
         # * do tuple, (geom, 'space room whatever') for each 'inpblock' per story
         return self._make_doe_stories(self.host)
 
     @staticmethod
     def _make_doe_stories(obj):
-        grouped = Room.group_by_floor_height(obj.rooms, 0.1)
         stories = []
+        if not obj.rooms:
+            return stories
+
+        grouped = Room.group_by_floor_height(obj.rooms, 0.1)
         for i, story in enumerate(grouped[0]):
             stories.append(Doe2Story(story, i))
         # nl = ''
         # return str(nl.join(str(s) for s in stories))
         return stories
 
     @property
```

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.4.2/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.4.2/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.4.2/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2/writer.py` & `honeybee-doe2-0.4.2/honeybee_doe2/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.4.2/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.4.1
+Version: 0.4.2
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.4.1/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.4.2/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.1/setup.py` & `honeybee-doe2-0.4.2/setup.py`

 * *Files identical despite different names*


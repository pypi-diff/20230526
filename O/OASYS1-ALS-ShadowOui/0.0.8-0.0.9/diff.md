# Comparing `tmp/OASYS1-ALS-ShadowOui-0.0.8.tar.gz` & `tmp/OASYS1-ALS-ShadowOui-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-ALS-ShadowOui-0.0.8.tar", last modified: Fri May 11 12:02:38 2018, max compression
+gzip compressed data, was "dist/OASYS1-ALS-ShadowOui-0.0.9.tar", last modified: Fri Nov 22 00:59:53 2019, max compression
```

## Comparing `OASYS1-ALS-ShadowOui-0.0.8.tar` & `OASYS1-ALS-ShadowOui-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,66 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/
--rw-r--r--   0 root         (0) staff       (20)      176 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/
--rw-r--r--   0 root         (0) staff       (20)        1 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      278 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       93 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2018-05-11 12:00:59.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      851 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       11 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)     1615 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       14 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/
--rw-r--r--   0 root         (0) staff       (20)       55 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/
--rw-r--r--   0 root         (0) staff       (20)       55 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/
--rw-r--r--   0 root         (0) staff       (20)       55 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/
--rw-r--r--   0 root         (0) staff       (20)       55 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    21348 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/ow_als_generic_analyzer.py
--rw-r--r--   0 root         (0) staff       (20)     2400 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/ow_als_shadow_widget.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/
--rw-r--r--   0 root         (0) staff       (20)      185 2018-05-11 12:01:34.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/icons/
--rw-r--r--   0 root         (0) staff       (20)    82709 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/icons/hhlo.png
--rwxr-xr-x   0 root         (0) staff       (20)    14391 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/icons/opticalElements.png
--rw-r--r--   0 root         (0) staff       (20)     9493 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/ow_als_ansys_reader.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/
--rw-r--r--   0 root         (0) staff       (20)      206 2018-05-11 12:01:34.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/icons/
--rw-r--r--   0 root         (0) staff       (20)     7895 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/icons/source.png
--rw-r--r--   0 root         (0) staff       (20)    21621 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/icons/undulator.png
--rw-r--r--   0 root         (0) staff       (20)    51403 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/ow_als_undulator.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/
--rw-r--r--   0 root         (0) staff       (20)      206 2018-05-11 12:01:34.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/
--rw-r--r--   0 root         (0) staff       (20)     5242 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/curved_element_analyzer.png
--rw-r--r--   0 root         (0) staff       (20)   106798 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/grating_analyzer.png
--rwxr-xr-x   0 root         (0) staff       (20)    29342 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/utility.png
--rw-r--r--   0 root         (0) staff       (20)     5301 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/ow_als_curved_element_analyzer.py
--rw-r--r--   0 root         (0) staff       (20)     2143 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/ow_als_grating_analyzer.py
--rw-r--r--   0 root         (0) staff       (20)      851 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)       63 2018-05-09 11:58:22.000000 OASYS1-ALS-ShadowOui-0.0.8/README.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2018-05-11 12:02:38.000000 OASYS1-ALS-ShadowOui-0.0.8/setup.cfg
--rwxr-xr-x   0 root         (0) staff       (20)     3731 2018-05-11 12:02:16.000000 OASYS1-ALS-ShadowOui-0.0.8/setup.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      176 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/MANIFEST.in
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       38 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/setup.cfg
+-rwxr-xr-x   0 manuel    (1000) manuel    (1000)     3731 2019-11-22 00:59:19.000000 OASYS1-ALS-ShadowOui-0.0.9/setup.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       55 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       55 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       55 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     1159 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/gradient.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    10130 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/random_distributions.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     7214 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/random_image.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    10272 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/fast_grid.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     9878 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/image.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3934 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/test_sampling_srio.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    33623 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/util/enhanced_grid.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     9437 2019-08-01 21:38:46.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/ow_als_ansys_reader.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      185 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/icons/
+-rwxr-xr-x   0 manuel    (1000) manuel    (1000)    14391 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/icons/opticalElements.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    82709 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/icons/hhlo.png
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      206 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/icons/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    21621 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/icons/undulator.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     7895 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/icons/source.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    61284 2019-08-01 21:39:07.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/ow_als_undulator.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       55 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     5301 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_curved_element_analyzer.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      206 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      202 2019-11-22 00:49:18.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/resolving_power.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)   156316 2019-08-15 00:10:16.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/predabam.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    29276 2019-11-18 23:18:49.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/caustic.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     5285 2019-11-20 22:47:22.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/integral.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)   210147 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/wavefront_generator.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)   106798 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/grating_analyzer.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     5242 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/curved_element_analyzer.png
+-rwxr-xr-x   0 manuel    (1000) manuel    (1000)    29342 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/utility.png
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     2143 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_grating_analyzer.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    16429 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_wavefront_generator.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    14560 2019-11-22 00:52:00.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_resolving_power.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     7154 2019-11-20 22:58:11.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_slit_integrator.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     8143 2019-11-20 22:48:56.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_caustic.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    21348 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/ow_als_generic_analyzer.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     4220 2019-11-20 22:18:29.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/plots.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     2400 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/ow_als_shadow_widget.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       63 2019-08-01 21:30:58.000000 OASYS1-ALS-ShadowOui-0.0.9/README.txt
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       93 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/namespace_packages.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     2607 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      278 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/entry_points.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      851 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/PKG-INFO
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       11 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/requires.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2019-08-01 21:32:25.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/not-zip-safe
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       14 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/top_level.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      851 2019-11-22 00:59:53.000000 OASYS1-ALS-ShadowOui-0.0.9/PKG-INFO
```

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/OASYS1_ALS_ShadowOui.egg-info/PKG-INFO` & `OASYS1-ALS-ShadowOui-0.0.9/OASYS1_ALS_ShadowOui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ALS-ShadowOui
-Version: 0.0.8
+Version: 0.0.9
 Summary: WIDGETS DEVELOPED FOR ALS TO EXTEND SHADOWOUI FUNCTIONALITIES
 Home-page: http://github.com/lucarebuffi/OASYS1-ALS-ShadowOui
 Author: Luca Rebuffi and Antoine Wojdyla
 Author-email: luca.rebuffi@elettra.eu
 License: MIT
 Download-URL: http://github.com/lucarebuffi/OASYS1-ALS-ShadowOui
 Description: WIDGETS DEVELOPED FOR ALS TO EXTEND SHADOWOUI FUNCTIONALITIES
```

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/ow_als_generic_analyzer.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/ow_als_generic_analyzer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/gui/ow_als_shadow_widget.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/gui/ow_als_shadow_widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/icons/hhlo.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/icons/hhlo.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/icons/opticalElements.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/icons/opticalElements.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/optical_elements/ow_als_ansys_reader.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/optical_elements/ow_als_ansys_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from oasys.widgets import congruence
 from orangewidget import widget
 
 from orangecontrib.shadow.als.widgets.gui.ow_als_shadow_widget import ALSShadowWidget
 
 from orangecontrib.shadow.util.shadow_objects import ShadowPreProcessorData
 
-import scipy.constants as codata
-
-from srwlib import *
-
 class Distribution:
     POSITION = 0
     DIVERGENCE = 1
 
 class ALSAnsysReader(ALSShadowWidget):
 
     name = "ANSYS Reader"
```

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/icons/source.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/icons/source.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/icons/undulator.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/icons/undulator.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/sources/ow_als_undulator.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/sources/ow_als_undulator.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 from orangecontrib.shadow.util.shadow_objects import ShadowBeam, ShadowSource
 from orangecontrib.shadow.als.widgets.gui.ow_als_shadow_widget import ALSShadowWidget
 from orangecontrib.shadow.widgets.gui.ow_generic_element import GenericElement
 
 import scipy.constants as codata
 
-from srwlib import *
+from srxraylib.util.h5_simple_writer import H5SimpleWriter
+
+import h5py
+
+from oasys_srw.srwlib import *
 
 class Distribution:
     POSITION = 0
     DIVERGENCE = 1
 
 #class ALSUndulator(ALSShadowWidget):
 class ALSUndulator(GenericElement):
@@ -72,21 +76,26 @@
 
     angular_distribution_wf_h_slit_gap = Setting(0.02)
     angular_distribution_wf_v_slit_gap = Setting(0.01)
     angular_distribution_wf_h_slit_points=Setting(201)
     angular_distribution_wf_v_slit_points=Setting(101)
     angular_distribution_wf_distance = Setting(100.0)
 
-    save_srw_result = Setting(1)
+    save_srw_result = Setting(2) # 0=nO 1=SRW FILES 2=HDF FILES
 
     # SRW FILE INPUT
 
     source_dimension_srw_file     = Setting("intensity_source_dimension.dat")
     angular_distribution_srw_file = Setting("intensity_angular_distribution.dat")
 
+    # HDF FILE INPUT
+
+    source_dimension_hdf5_file     = Setting("intensity_source_dimension.h5")
+    angular_distribution_hdf5_file = Setting("intensity_angular_distribution.h5")
+
     # ASCII FILE INPUT
 
     x_positions_file = Setting("x_positions.txt")
     z_positions_file = Setting("z_positions.txt")
     x_positions_factor = Setting(0.01)
     z_positions_factor = Setting(0.01)
     x_divergences_file = Setting("x_divergences.txt")
@@ -109,14 +118,22 @@
 
     optimize_source=Setting(0)
     optimize_file_name = Setting("NONESPECIFIED")
     max_number_of_rejected_rays = Setting(10000000)
 
     file_to_write_out = Setting(0)
 
+    # for testing this widget outside OASYS
+    try:
+            tmp = self.workspace_units_to_m
+            tmp = self.workspace_units_to_cm
+    except:
+            workspace_units_to_m  = Setting(1.0)
+            workspace_units_to_cm = Setting(100.0)
+
     def __init__(self, show_automatic_box=False):
         super().__init__(show_automatic_box=show_automatic_box)
 
         self.runaction = widget.OWAction("Run Shadow/Source", self)
         self.runaction.triggered.connect(self.runShadowSource)
         self.addAction(self.runaction)
 
@@ -153,19 +170,20 @@
         tabs_setting.setFixedHeight(self.TABS_AREA_HEIGHT)
         tabs_setting.setFixedWidth(self.CONTROL_AREA_WIDTH-5)
 
         tab_shadow = oasysgui.createTabPage(tabs_setting, "Shadow Setting")
         tab_spdiv = oasysgui.createTabPage(tabs_setting, "Position/Divergence Setting")
 
         gui.comboBox(tab_spdiv, self, "distribution_source", label="Distribution Source", labelWidth=310,
-                     items=["SRW Calculation", "SRW Files", "ASCII Files"], orientation="horizontal", callback=self.set_DistributionSource)
+                     items=["SRW Calculation", "SRW Files", "ASCII Files", "HDF5 Files"], orientation="horizontal", callback=self.set_DistributionSource)
 
         self.srw_box = oasysgui.widgetBox(tab_spdiv, "SRW Setting", addSpace=False, orientation="vertical", height=540)
         self.srw_files_box = oasysgui.widgetBox(tab_spdiv, "SRW Files Load Setting", addSpace=False, orientation="vertical", height=540)
         self.ascii_box = oasysgui.widgetBox(tab_spdiv, "ASCII Files Load Setting", addSpace=False, orientation="vertical", height=540)
+        self.hdf5_files_box = oasysgui.widgetBox(tab_spdiv, "HDF5 Files Load Setting", addSpace=False, orientation="vertical", height=540)
 
         self.set_DistributionSource()
 
         ####################################################################################
         # SHADOW
 
         left_box_1 = oasysgui.widgetBox(tab_shadow, "Monte Carlo and Energy Spectrum", addSpace=False, orientation="vertical")
@@ -215,32 +233,47 @@
 
         ####################################################################################
         # SRW
 
         tabs_srw = oasysgui.tabWidget(self.srw_box)
 
         gui.comboBox(self.srw_box, self, "save_srw_result", label="Save SRW results", labelWidth=310,
-                     items=["No", "Yes"], orientation="horizontal", callback=self.set_SaveFileSRW)
+                     items=["No", "Yes (srw)", "Yes (hdf5)"], orientation="horizontal", callback=self.set_SaveFileSRW)
 
-        self.save_file_box = oasysgui.widgetBox(self.srw_box, "", addSpace=False, orientation="vertical")
+        self.save_file_box_srw = oasysgui.widgetBox(self.srw_box, "", addSpace=False, orientation="vertical")
+        self.save_file_box_hdf5 = oasysgui.widgetBox(self.srw_box, "", addSpace=False, orientation="vertical")
         self.save_file_box_empty = oasysgui.widgetBox(self.srw_box, "", addSpace=False, orientation="vertical", height=55)
 
-        file_box = oasysgui.widgetBox(self.save_file_box, "", addSpace=False, orientation="horizontal", height=25)
+        file_box = oasysgui.widgetBox(self.save_file_box_srw, "", addSpace=False, orientation="horizontal", height=25)
 
-        self.le_source_dimension_srw_file = oasysgui.lineEdit(file_box, self, "source_dimension_srw_file", "Source Dimension File", labelWidth=140,  valueType=str, orientation="horizontal")
+        self.le_source_dimension_srw_file = oasysgui.lineEdit(file_box, self, "source_dimension_srw_file", "Source Dimension SRW File", labelWidth=140,  valueType=str, orientation="horizontal")
 
-        gui.button(file_box, self, "...", callback=self.selectSourceDimensionFile)
+        gui.button(file_box, self, "...", callback=self.selectSourceDimensionFileSrw)
 
-        file_box = oasysgui.widgetBox(self.save_file_box, "", addSpace=False, orientation="horizontal", height=25)
+        file_box = oasysgui.widgetBox(self.save_file_box_hdf5, "", addSpace=False, orientation="horizontal", height=25)
 
-        self.le_angular_distribution_srw_file = oasysgui.lineEdit(file_box, self, "angular_distribution_srw_file", "Angular Distribution File", labelWidth=140,  valueType=str, orientation="horizontal")
+        self.le_source_dimension_hdf5_file = oasysgui.lineEdit(file_box, self, "source_dimension_hdf5_file", "Source Dimension HDF5 File", labelWidth=140,  valueType=str, orientation="horizontal")
 
-        gui.button(file_box, self, "...", callback=self.selectAngularDistributionFile)
+        gui.button(file_box, self, "...", callback=self.selectSourceDimensionFileHdf5)
 
-        self.set_SaveFileSRW()
+
+        file_box = oasysgui.widgetBox(self.save_file_box_srw, "", addSpace=False, orientation="horizontal", height=25)
+
+        self.le_angular_distribution_srw_file = oasysgui.lineEdit(file_box, self, "angular_distribution_srw_file", "Angular Distribution SRW File", labelWidth=140,  valueType=str, orientation="horizontal")
+
+        gui.button(file_box, self, "...", callback=self.selectAngularDistributionFileSrw)
+
+        file_box = oasysgui.widgetBox(self.save_file_box_hdf5, "", addSpace=False, orientation="horizontal", height=25)
+
+        self.le_angular_distribution_hdf_file = oasysgui.lineEdit(file_box, self, "angular_distribution_hdf5_file", "Angular Distribution HDF5 File", labelWidth=140,  valueType=str, orientation="horizontal")
+
+        gui.button(file_box, self, "...", callback=self.selectAngularDistributionFileHdf5)
+
+
+        # self.set_SaveFileSRW()
 
         tab_ls = oasysgui.createTabPage(tabs_srw, "Undulator Setting")
         tab_wf = oasysgui.createTabPage(tabs_srw, "Wavefront Setting")
 
         left_box_1 = oasysgui.widgetBox(tab_ls, "Undulator Parameters", addSpace=False, orientation="vertical")
 
         oasysgui.lineEdit(left_box_1, self, "number_of_periods", "Number of Periods", labelWidth=260,  valueType=float, orientation="horizontal")
@@ -282,21 +315,21 @@
         ####################################################################################
         # SRW FILES
 
         file_box = oasysgui.widgetBox(self.srw_files_box, "", addSpace=True, orientation="horizontal", height=45)
 
         self.le_source_dimension_srw_file = oasysgui.lineEdit(file_box, self, "source_dimension_srw_file", "Source Dimension File", labelWidth=180,  valueType=str, orientation="vertical")
 
-        gui.button(file_box, self, "...", height=45, callback=self.selectSourceDimensionFile)
+        gui.button(file_box, self, "...", height=45, callback=self.selectSourceDimensionFileSrw)
 
         file_box = oasysgui.widgetBox(self.srw_files_box, "", addSpace=True, orientation="horizontal", height=45)
 
-        self.le_angular_distribution_srw_file = oasysgui.lineEdit(file_box, self, "angular_distribution_srw_file", "Angular Distribution File", labelWidth=180,  valueType=str, orientation="vertical")
+        self.le_angular_distribution_srw_file = oasysgui.lineEdit(file_box, self, "angular_distribution_srw_file", "Angular Distribution SRW File", labelWidth=180,  valueType=str, orientation="vertical")
 
-        gui.button(file_box, self, "...", height=45, callback=self.selectAngularDistributionFile)
+        gui.button(file_box, self, "...", height=45, callback=self.selectAngularDistributionFileSrw)
 
 
         ####################################################################################
         # ASCII FILES
 
         file_box = oasysgui.widgetBox(self.ascii_box, "", addSpace=True, orientation="horizontal", height=45)
 
@@ -318,14 +351,32 @@
 
         file_box = oasysgui.widgetBox(self.ascii_box, "", addSpace=True, orientation="horizontal", height=45)
 
         self.le_z_divergences_file = oasysgui.lineEdit(file_box, self, "z_divergences_file", "Z Divergences File", labelWidth=180,  valueType=str, orientation="vertical")
 
         gui.button(file_box, self, "...", height=45, callback=self.selectZDivergencesFile)
 
+        ####################################################################################
+        # HDF5 FILES
+
+        file_box = oasysgui.widgetBox(self.hdf5_files_box, "", addSpace=True, orientation="horizontal", height=45)
+
+        self.le_source_dimension_hdf5_file = oasysgui.lineEdit(file_box, self, "source_dimension_hdf5_file", "Source Dimension HDF5 File", labelWidth=180,  valueType=str, orientation="vertical")
+
+        gui.button(file_box, self, "...", height=45, callback=self.selectSourceDimensionHDF5File)
+
+        file_box = oasysgui.widgetBox(self.hdf5_files_box, "", addSpace=True, orientation="horizontal", height=45)
+
+        self.le_angular_distribution_hdf5_file = oasysgui.lineEdit(file_box, self, "angular_distribution_hdf5_file", "Angular Distribution HDF5 File", labelWidth=180,  valueType=str, orientation="vertical")
+
+        gui.button(file_box, self, "...", height=45, callback=self.selectAngularDistributionHDF5File)
+
+
+        self.set_SaveFileSRW()
+
         gui.separator(self.ascii_box)
 
         oasysgui.lineEdit(self.ascii_box, self, "x_positions_factor",   "X Positions UM to Workspace UM", labelWidth=230, valueType=float, orientation="horizontal")
         oasysgui.lineEdit(self.ascii_box, self, "z_positions_factor",   "Z Positions UM to Workspace UM",  labelWidth=230, valueType=float, orientation="horizontal")
         oasysgui.lineEdit(self.ascii_box, self, "x_divergences_factor", "X Divergences UM to rad", labelWidth=230, valueType=float, orientation="horizontal")
         oasysgui.lineEdit(self.ascii_box, self, "z_divergences_factor", "X Divergences UM to rad", labelWidth=230, valueType=float, orientation="horizontal")
 
@@ -362,33 +413,68 @@
 
         return write_begin_file, write_start_file, write_end_file
 
     def set_DistributionSource(self):
         self.srw_box.setVisible(self.distribution_source == 0)
         self.srw_files_box.setVisible(self.distribution_source == 1)
         self.ascii_box.setVisible(self.distribution_source == 2)
+        self.hdf5_files_box.setVisible(self.distribution_source == 3)
+
 
     def set_Polarization(self):
         self.ewp_box_8.setVisible(self.polarization==1)
 
     def set_OptimizeSource(self):
         self.optimize_file_name_box.setVisible(self.optimize_source != 0)
 
     def set_SaveFileSRW(self):
-        self.save_file_box.setVisible(self.save_srw_result == 1)
-        self.save_file_box_empty.setVisible(self.save_srw_result == 0)
+        if self.save_srw_result ==1:
+            self.save_file_box_srw.setVisible(True)
+            self.save_file_box_hdf5.setVisible(False)
+            self.save_file_box_empty.setVisible(False)
+
+            # self.srw_files_box.setVisible(True)
+            # self.hdf5_files_box.setVisible(False)
+
+        elif self.save_srw_result ==2:
+            self.save_file_box_srw.setVisible(False)
+            self.save_file_box_hdf5.setVisible(True)
+            self.save_file_box_empty.setVisible(False)
+
+            # self.srw_files_box.setVisible(False)
+            # self.hdf5_files_box.setVisible(True)
+        else:
+            # self.save_file_box_srw.setVisible(self.save_srw_result == 2)
+            self.save_file_box_srw.setVisible(False)
+            self.save_file_box_hdf5.setVisible(False)
+            self.save_file_box_empty.setVisible(True)
+
 
     def selectOptimizeFile(self):
         self.le_optimize_file_name.setText(oasysgui.selectFileFromDialog(self, self.optimize_file_name, "Open Optimize Source Parameters File"))
 
-    def selectSourceDimensionFile(self):
-        self.le_source_dimension_srw_file.setText(oasysgui.selectFileFromDialog(self, self.source_dimension_srw_file, "Open Source Dimension File"))
+    def selectSourceDimensionFileSrw(self):
+        self.le_source_dimension_srw_file.setText(oasysgui.selectFileFromDialog(self, self.source_dimension_srw_file, "Open SRW Source Dimension File"))
+
+    def selectAngularDistributionFileSrw(self):
+        self.le_angular_distribution_srw_file.setText(oasysgui.selectFileFromDialog(self, self.angular_distribution_srw_file, "Open SRW Angular Distribution File"))
+
+    def selectSourceDimensionFileHdf5(self):
+        self.le_source_dimension_hdf5_file.setText(oasysgui.selectFileFromDialog(self, self.source_dimension_hdf5_file, "Open HDF5 Source Dimension File"))
+
+    def selectAngularDistributionFileHdf5(self):
+        self.le_angular_distribution_hdf5_file.setText(oasysgui.selectFileFromDialog(self, self.angular_distribution_hdf5_file, "Open HDF5 Angular Distribution File"))
+
+
+    def selectSourceDimensionHDF5File(self):
+        self.le_source_dimension_hdf5_file.setText(oasysgui.selectFileFromDialog(self, self.source_dimension_hdf5_file, "Open HDF5 Source Dimension File"))
+
+    def selectAngularDistributionHDF5File(self):
+        self.le_angular_distribution_hdf5_file.setText(oasysgui.selectFileFromDialog(self, self.angular_distribution_hdf5_file, "Open HDF5 Angular Distribution File"))
 
-    def selectAngularDistributionFile(self):
-        self.le_angular_distribution_srw_file.setText(oasysgui.selectFileFromDialog(self, self.angular_distribution_srw_file, "Open Angular Distribution File"))
 
     def selectXPositionsFile(self):
         self.le_x_positions_file.setText(oasysgui.selectFileFromDialog(self, self.x_positions_file, "Open X Positions File", file_extension_filter="*.dat, *.txt"))
 
     def selectZPositionsFile(self):
         self.le_z_positions_file.setText(oasysgui.selectFileFromDialog(self, self.z_positions_file, "Open Z Positions File", file_extension_filter="*.dat, *.txt"))
 
@@ -435,40 +521,43 @@
 
             self.fix_Intensity(beam_out)
 
             self.progressBarSet(20)
 
             if self.distribution_source == 0:
                 self.setStatusMessage("Running SRW")
-
                 x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution = self.runSRWCalculation()
             elif self.distribution_source == 1:
                 self.setStatusMessage("Loading SRW files")
-
                 x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution = self.loadSRWFiles()
             elif self.distribution_source == 2: # ASCII FILES
                 self.setStatusMessage("Loading Ascii files")
-
                 x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution = self.loadASCIIFiles()
+            elif self.distribution_source == 3: # HDF5 FILES
+                self.setStatusMessage("Loading HDF5 files")
+                x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution = self.loadHDF5Files()
+
+            # from srxraylib.plot.gol import plot_image
+            # plot_image(intensity_angular_distribution,x_first, z_first,xtitle="X [%d pixels]"%x_first.size,ytitle="Y [%d pixels]"%z_first.size)
 
             self.progressBarSet(50)
 
             self.setStatusMessage("Applying new Spatial/Angular Distribution")
 
             self.progressBarSet(60)
 
-            self.generate_user_defined_distribution_from_srw(beam_out=beam_out,
+            self.generate_user_defined_distribution_from_srw_srio(beam_out=beam_out,
                                                              coord_x=x,
                                                              coord_y=z,
                                                              intensity=intensity_source_dimension,
                                                              distribution_type=Distribution.POSITION)
 
             self.progressBarSet(70)
 
-            self.generate_user_defined_distribution_from_srw(beam_out=beam_out,
+            self.generate_user_defined_distribution_from_srw_srio(beam_out=beam_out,
                                                              coord_x=x_first,
                                                              coord_y=z_first,
                                                              intensity=intensity_angular_distribution,
                                                              distribution_type=Distribution.DIVERGENCE)
 
 
 
@@ -616,14 +705,18 @@
         congruence.checkGreaterOrEqualThan(self.angular_distribution_wf_distance, self.get_minimum_propagation_distance(),
                                            "Wavefront Propagation Distance", "Minimum Distance out of the Source: " + str(self.get_minimum_propagation_distance()))
 
         if self.save_srw_result == 1:
             congruence.checkDir(self.source_dimension_srw_file)
             congruence.checkDir(self.angular_distribution_srw_file)
 
+        if self.save_srw_result == 2:
+            congruence.checkDir(self.source_dimension_hdf5_file)
+            congruence.checkDir(self.angular_distribution_hdf5_file)
+
     def get_minimum_propagation_distance(self):
         return round(self.get_source_length()*1.01, 6)
 
     def get_source_length(self):
         return self.undulator_period*self.number_of_periods
 
     def magnetic_field_from_K(self):
@@ -790,22 +883,30 @@
         srwl.PropagElecField(wfrSouDim, optBLSouDim)
         print('done')
 
         print('   Extracting Intensity from the Propagated Electric Field for Dim Nat ... ', end='')
         arI = array('f', [0]*wfrSouDim.mesh.nx*wfrSouDim.mesh.ny) #"flat" 2D array to take intensity data
         srwl.CalcIntFromElecField(arI, wfrSouDim, 6, 1, 3, wfrSouDim.mesh.eStart, 0, 0)
 
-        if self.save_srw_result == 1: srwl_uti_save_intens_ascii(arI, wfrSouDim.mesh, "intensity_source_dimension.dat")
+        x, z, intensity_source_dimension = self.transform_srw_array(arI, wfrSouDim.mesh)
+
+        if self.save_srw_result == 1:
+            srwl_uti_save_intens_ascii(arI, wfrSouDim.mesh, "intensity_source_dimension.dat")
+        elif self.save_srw_result == 2:
+            self.save_hdf5(self.source_dimension_hdf5_file,x, z, intensity_source_dimension)
         print('done')
 
-        x, z, intensity_source_dimension = self.transform_srw_array(arI, wfrSouDim.mesh)
+
 
         # SWITCH FROM SRW METERS TO SHADOWOUI U.M.
-        x = x/self.workspace_units_to_m
-        z = z/self.workspace_units_to_m
+        try:
+            x = x/self.workspace_units_to_m
+            z = z/self.workspace_units_to_m
+        except:
+            pass
 
         # 2 calculate intensity distribution ME convoluted at far field to express it in angular coordinates
 
         print('   Performing Initial Single-E Electric Field calculation ... ', end='')
         arPrecParSpec[6] = sampFactNxNyForProp #sampling factor for adjusting nx, ny (effective if > 0)
         srwl.CalcElecFieldSR(wfrAngDist, 0, magFldCnt, arPrecParSpec)
         print('done')
@@ -819,18 +920,24 @@
         distance = wfrAngDist.mesh.zStart + 0.5*(self.number_of_periods*self.undulator_period)
 
         wfrAngDist.mesh.xStart /= distance
         wfrAngDist.mesh.xFin /= distance
         wfrAngDist.mesh.yStart /= distance
         wfrAngDist.mesh.yFin /= distance
 
-        if self.save_srw_result == 1: srwl_uti_save_intens_ascii(arI, wfrAngDist.mesh, "intensity_angular_distribution.dat")
+        x_first, z_first, intensity_angular_distribution = self.transform_srw_array(arI, wfrAngDist.mesh)
+
+        if self.save_srw_result == 1:
+            srwl_uti_save_intens_ascii(arI, wfrAngDist.mesh, "intensity_angular_distribution.dat")
+        elif self.save_srw_result == 2:
+            self.save_hdf5(self.angular_distribution_hdf5_file,x_first, z_first, intensity_angular_distribution)
         print('done')
 
-        x_first, z_first, intensity_angular_distribution = self.transform_srw_array(arI, wfrAngDist.mesh)
+        # from srxraylib.plot.gol import plot_image
+        # plot_image(intensity_angular_distribution,x_first, z_first, title="DATA WRITTEN TO FILE")
 
         return x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution
 
 
     def extract_distributions_from_srw(self, coor_x, coor_y, intensity):
         distribution_x = []
         distribution_y = []
@@ -862,14 +969,17 @@
         new_coord_y = numpy.arange(0, len(coord_y))
 
         distribution_x, distribution_y = self.extract_distributions_from_srw(new_coord_x, new_coord_y, intensity)
 
         sampled_x = self.sample_from_distribution(distribution_x, len(beam_out._beam.rays))
         sampled_y = self.sample_from_distribution(distribution_y, len(beam_out._beam.rays))
 
+        # from srxraylib.plot.gol import plot_scatter
+        # plot_scatter(sampled_x,sampled_y)
+
         min_value_x = numpy.min(coord_x)
         step_x = numpy.abs(coord_x[1]-coord_x[0])
         min_value_y = numpy.min(coord_y)
         step_y = numpy.abs(coord_y[1]-coord_y[0])
 
         print(min_value_x, step_x, min_value_y, step_y)
 
@@ -881,14 +991,74 @@
             alpha_x = min_value_x + sampled_x*step_x
             alpha_z = min_value_y + sampled_y*step_y
 
             beam_out._beam.rays[:, 3] =  numpy.cos(alpha_z)*numpy.sin(alpha_x)
             beam_out._beam.rays[:, 4] =  numpy.cos(alpha_z)*numpy.cos(alpha_x)
             beam_out._beam.rays[:, 5] =  numpy.sin(alpha_z)
 
+    def generate_user_defined_distribution_from_srw_srio(self,
+                                                    beam_out,
+                                                    coord_x,
+                                                    coord_y,
+                                                    intensity,
+                                                    distribution_type=Distribution.POSITION):
+        npoints = beam_out._beam.rays[:, 0].size
+
+        if distribution_type == Distribution.POSITION:
+            print("  Sampling %d points for position... [slow]"%npoints)
+            sampled_x, sampled_y = self.sample_2d_scattered_points_from_image(intensity,coord_x,coord_y,npoints=npoints)
+            print("  Sampling %d points for position... DONE"%npoints)
+
+            # from srxraylib.plot.gol import plot_scatter
+            # plot_scatter(sampled_x,sampled_y,title="POSITION")
+
+
+            beam_out._beam.rays[:, 0] = sampled_x
+            beam_out._beam.rays[:, 2] = sampled_y
+
+        elif distribution_type == Distribution.DIVERGENCE:
+            print("  Sampling %d points for angle... [slow]"%npoints)
+            alpha_x, alpha_z = self.sample_2d_scattered_points_from_image(intensity,coord_x,coord_y,npoints=npoints)
+            print("  Sampling %d points for angle... DONE"%npoints)
+
+            # from srxraylib.plot.gol import plot_scatter
+            # plot_scatter(alpha_x,alpha_z,title="ANGLE")
+
+            beam_out._beam.rays[:, 3] =  alpha_x # numpy.cos(alpha_z)*numpy.sin(alpha_x)
+            beam_out._beam.rays[:, 4] =  1.0 - numpy.sqrt(alpha_x**2 + alpha_z**2) # numpy.cos(alpha_z)*numpy.cos(alpha_x)
+            beam_out._beam.rays[:, 5] =  alpha_z # numpy.sin(alpha_z)
+
+
+    def sample_2d_scattered_points_from_image(self,image_data,x,y,npoints=10000):
+        from orangecontrib.shadow.als.util.random_distributions import distribution_from_grid, Distribution2D
+        from orangecontrib.shadow.als.util.enhanced_grid import Grid2D
+        from random import random
+
+        grid = Grid2D(image_data.shape)
+
+        grid[..., ...] = image_data.tolist()
+
+        probs = distribution_from_grid(grid, image_data.shape[0], image_data.shape[1])
+
+        d = Distribution2D(probs, (0, 0), (500, 500))
+
+
+        samples_x = numpy.zeros( npoints )
+        samples_y = numpy.zeros( npoints )
+
+
+        for k in range(npoints):
+            samples_x[k],samples_y[k] = (d(random(), random()))
+
+        samples_x = ( x[0] + (x[-1]-x[0])*samples_x)
+        samples_y = ( y[0] + (y[-1]-y[0])*samples_y)
+
+        return samples_x,samples_y
+
+
     ####################################################################################
     # SRW FILES
     ####################################################################################
 
     def checkSRWFilesFields(self):
         congruence.checkFile(self.source_dimension_srw_file)
         congruence.checkFile(self.angular_distribution_srw_file)
@@ -898,17 +1068,46 @@
         self.checkSRWFilesFields()
 
         x, z, intensity_source_dimension = self.loadNumpyFormat(self.source_dimension_srw_file)
         x_first, z_first, intensity_angular_distribution = self.loadNumpyFormat(self.angular_distribution_srw_file)
 
 
         # SWITCH FROM SRW METERS TO SHADOWOUI U.M.
-        x = x/self.workspace_units_to_m
-        z = z/self.workspace_units_to_m
+        try:
+            x = x/self.workspace_units_to_m
+            z = z/self.workspace_units_to_m
+        except:
+            pass
+
+        return x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution
+
+    def loadHDF5Files(self):
+
+        self.checkSRWFilesFields()
+
+        print(">>>> reading files: ",self.angular_distribution_srw_file,self.source_dimension_srw_file)
+        try:
+            f = h5py.File(self.angular_distribution_hdf5_file, 'r')
+            x_first = f["intensity/axis_x"].value
+            z_first = f["intensity/axis_y"].value
+            intensity_angular_distribution = f["intensity/image_data"].value.T
+            f.close()
+        except:
+            raise Exception("Failed to load SRW intensity from h5 file: "+self.angular_distribution_srw_file)
+
+        try:
+            f = h5py.File(self.source_dimension_hdf5_file, 'r')
+            x = f["intensity/axis_x"].value
+            z = f["intensity/axis_y"].value
+            intensity_source_dimension = f["intensity/image_data"].value.T
+            f.close()
+        except:
+            raise Exception("Failed to load SRW intensity from h5 file: "+self.angular_distribution_srw_file)
 
+        print(">>>> read dimensions: ",x.shape, z.shape, intensity_source_dimension.shape, x_first.shape, z_first.shape, intensity_angular_distribution.shape)
         return x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution
 
 
     def file_load(self, _fname, _read_labels=1):
         nLinesHead = 11
         hlp = []
 
@@ -1002,14 +1201,17 @@
 
         x, z, intensity_source_dimension = self.combine_distributions(x_positions, z_positions)
         x_first, z_first, intensity_angular_distribution = self.combine_distributions(x_divergences, z_divergences)
 
         return x, z, intensity_source_dimension, x_first, z_first, intensity_angular_distribution
 
 
+
+
+
     def extract_distribution_from_file(self, distribution_file_name):
         distribution = []
 
         try:
             distribution_file = open(distribution_file_name, "r")
 
             rows = distribution_file.readlines()
@@ -1051,15 +1253,26 @@
         elif self.combine_strategy == 2:
             convoluted_intensity = convolve2d(intensity_x, intensity_y, boundary='fill', mode='same', fillvalue=0)
         elif self.combine_strategy == 3:
             convoluted_intensity = 0.5*(intensity_x + intensity_y)
 
         return coord_x, coord_y, convoluted_intensity
 
+    def save_hdf5(self,filename,x,y,z):
+
+        h5w = H5SimpleWriter.initialize_file(filename,creator="oasys-ow_als_undulator")
+        # h5w.create_entry("wfr",nx_default="wfr")
+        # h5w.add_image(z,x,y,
+        #             entry_name="wfr",image_name="intensity",
+        #             title_x="X",title_y="Y")
+        h5w.add_image(z,x,y,
+                    image_name="intensity",
+                    title_x="X",title_y="Y")
 
 
 if __name__ == "__main__":
     a = QApplication(sys.argv)
     ow = ALSUndulator()
     ow.show()
     a.exec_()
     ow.saveSettings()
+
```

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/curved_element_analyzer.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/curved_element_analyzer.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/grating_analyzer.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/grating_analyzer.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/icons/utility.png` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/icons/utility.png`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/ow_als_curved_element_analyzer.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_curved_element_analyzer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/orangecontrib/shadow/als/widgets/utility/ow_als_grating_analyzer.py` & `OASYS1-ALS-ShadowOui-0.0.9/orangecontrib/shadow/als/widgets/utility/ow_als_grating_analyzer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/PKG-INFO` & `OASYS1-ALS-ShadowOui-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OASYS1-ALS-ShadowOui
-Version: 0.0.8
+Version: 0.0.9
 Summary: WIDGETS DEVELOPED FOR ALS TO EXTEND SHADOWOUI FUNCTIONALITIES
 Home-page: http://github.com/lucarebuffi/OASYS1-ALS-ShadowOui
 Author: Luca Rebuffi and Antoine Wojdyla
 Author-email: luca.rebuffi@elettra.eu
 License: MIT
 Download-URL: http://github.com/lucarebuffi/OASYS1-ALS-ShadowOui
 Description: WIDGETS DEVELOPED FOR ALS TO EXTEND SHADOWOUI FUNCTIONALITIES
```

### Comparing `OASYS1-ALS-ShadowOui-0.0.8/setup.py` & `OASYS1-ALS-ShadowOui-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import imp
 import os
 import sys
 import subprocess
 
 NAME = 'OASYS1-ALS-ShadowOui'
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'WIDGETS DEVELOPED FOR ALS TO EXTEND SHADOWOUI FUNCTIONALITIES'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi and Antoine Wojdyla'
 AUTHOR_EMAIL = 'luca.rebuffi@elettra.eu'
```


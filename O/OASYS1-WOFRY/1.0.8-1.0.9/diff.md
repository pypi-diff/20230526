# Comparing `tmp/OASYS1-WOFRY-1.0.8.tar.gz` & `tmp/OASYS1-WOFRY-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-WOFRY-1.0.8.tar", last modified: Mon Sep 16 20:46:51 2019, max compression
+gzip compressed data, was "dist/OASYS1-WOFRY-1.0.9.tar", last modified: Tue Jan  7 20:30:34 2020, max compression
```

## Comparing `OASYS1-WOFRY-1.0.8.tar` & `OASYS1-WOFRY-1.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/
--rw-r--r--   0 manuel    (1000) manuel    (1000)      171 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/MANIFEST.in
--rw-r--r--   0 manuel    (1000) manuel    (1000)       38 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/setup.cfg
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/
--rw-r--r--   0 manuel    (1000) manuel    (1000)       62 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/namespace_packages.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3244 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/SOURCES.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)      260 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/entry_points.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)      826 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/PKG-INFO
--rw-r--r--   0 manuel    (1000) manuel    (1000)       15 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/requires.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2019-09-03 16:34:48.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/not-zip-safe
--rw-r--r--   0 manuel    (1000) manuel    (1000)       14 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/top_level.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/dependency_links.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2768 2019-09-16 20:43:39.000000 OASYS1-WOFRY-1.0.8/setup.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/
--rw-r--r--   0 manuel    (1000) manuel    (1000)       81 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/__init__.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/
--rw-r--r--   0 manuel    (1000) manuel    (1000)       81 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/__init__.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/util/
--rw-r--r--   0 manuel    (1000) manuel    (1000)    14305 2019-09-16 17:48:07.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/util/wofry_util.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1343 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_screen_1d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1185 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_screen.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1879 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_stop.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3006 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_stop_1d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2268 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_double_slit.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)      264 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2687 2019-09-13 23:39:32.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2319 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/screen.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     5397 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/double_slit.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    56527 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/ideal_lens.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3846 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/ideallens_1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)      664 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    30978 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/beamline_elements.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1558 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/screen1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     3980 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/slit.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    37988 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    18439 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop.jpg
--rw-r--r--   0 manuel    (1000) manuel    (1000)      516 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/slit1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1558 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_slits_1d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2175 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens_1d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     1830 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_slits.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)       81 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/__init__.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/
--rw-r--r--   0 manuel    (1000) manuel    (1000)    22527 2019-09-16 20:25:28.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_2D.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    21514 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_1D.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)      272 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/__init__.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/
--rw-r--r--   0 manuel    (1000) manuel    (1000)   301469 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw2d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    38769 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/wavefront_propagation.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    31549 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw1d.png
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/
--rw-r--r--   0 manuel    (1000) manuel    (1000)     5950 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_1D_to_2D.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     5062 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_2D_to_1D.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)      240 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/__init__.py
--rwxr-xr-x   0 manuel    (1000) manuel    (1000)     4179 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_wavefront_file_writer.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/
--rw-r--r--   0 manuel    (1000) manuel    (1000)    12503 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/2d_to_1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    53714 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/accumulation.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    63980 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/tools.png
--rwxr-xr-x   0 manuel    (1000) manuel    (1000)      514 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/wv1d.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2611 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/file_reader.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)     2013 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/file_writer.png
--rw-r--r--   0 manuel    (1000) manuel    (1000)    13166 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/1d_to_2d.png
--rwxr-xr-x   0 manuel    (1000) manuel    (1000)     1168 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/wv2d.png
--rwxr-xr-x   0 manuel    (1000) manuel    (1000)     5027 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_wavefront_file_reader.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    12854 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_2d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)     9485 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_1D.py
-drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/
--rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/__init__.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    12514 2019-09-16 20:28:03.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_wofry_widget.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    55864 2019-09-16 20:19:49.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_optical_element.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)    24066 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_optical_element_1d.py
--rw-r--r--   0 manuel    (1000) manuel    (1000)      147 2019-09-03 16:21:33.000000 OASYS1-WOFRY-1.0.8/README.txt
--rw-r--r--   0 manuel    (1000) manuel    (1000)      826 2019-09-16 20:46:51.000000 OASYS1-WOFRY-1.0.8/PKG-INFO
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/
+-rw-rw-rw-   0 bishop    (1601)      907      171 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/MANIFEST.in
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      679 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     3243 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907      260 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/entry_points.txt
+-rw-rw-rw-   0 bishop    (1601)      907       62 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2018-10-04 14:55:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907       15 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907       14 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907      679 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       40 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/
+-rw-rw-rw-   0 bishop    (1601)      907       81 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/
+-rw-rw-rw-   0 bishop    (1601)      907       81 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/util/
+-rw-rw-rw-   0 bishop    (1601)      907    14305 2019-09-17 21:39:10.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/util/wofry_util.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907       81 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/
+-rw-rw-rw-   0 bishop    (1601)      907      264 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    30978 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/beamline_elements.png
+-rw-rw-rw-   0 bishop    (1601)      907     5397 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/double_slit.png
+-rw-rw-rw-   0 bishop    (1601)      907    56527 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/ideal_lens.png
+-rw-rw-rw-   0 bishop    (1601)      907     3846 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/ideallens_1d.png
+-rw-rw-rw-   0 bishop    (1601)      907     2319 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/screen.png
+-rw-rw-rw-   0 bishop    (1601)      907     1558 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/screen1d.png
+-rw-rw-rw-   0 bishop    (1601)      907     3980 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/slit.png
+-rw-rw-rw-   0 bishop    (1601)      907      516 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/slit1d.png
+-rw-rw-rw-   0 bishop    (1601)      907    18439 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop.jpg
+-rw-rw-rw-   0 bishop    (1601)      907    37988 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop.png
+-rw-rw-rw-   0 bishop    (1601)      907      664 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop1d.png
+-rw-rw-rw-   0 bishop    (1601)      907     2268 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_double_slit.py
+-rw-rw-rw-   0 bishop    (1601)      907     2687 2019-09-17 21:39:10.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens.py
+-rw-rw-rw-   0 bishop    (1601)      907     2175 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens_1d.py
+-rw-rw-rw-   0 bishop    (1601)      907     1185 2018-11-27 15:29:38.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_screen.py
+-rw-rw-rw-   0 bishop    (1601)      907     1343 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_screen_1d.py
+-rw-rw-rw-   0 bishop    (1601)      907     1830 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_slits.py
+-rw-rw-rw-   0 bishop    (1601)      907     1558 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_slits_1d.py
+-rw-rw-rw-   0 bishop    (1601)      907     1879 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_stop.py
+-rw-rw-rw-   0 bishop    (1601)      907     3006 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_stop_1d.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/
+-rw-rw-rw-   0 bishop    (1601)      907        0 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    55864 2019-09-17 21:39:10.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_optical_element.py
+-rw-rw-rw-   0 bishop    (1601)      907    24066 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_optical_element_1d.py
+-rw-rw-rw-   0 bishop    (1601)      907    12514 2019-09-17 21:39:10.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_wofry_widget.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/
+-rw-rw-rw-   0 bishop    (1601)      907      240 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     9485 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_1D.py
+-rw-rw-rw-   0 bishop    (1601)      907    12854 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_2d.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    13166 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/1d_to_2d.png
+-rw-rw-rw-   0 bishop    (1601)      907    12503 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/2d_to_1d.png
+-rw-rw-rw-   0 bishop    (1601)      907    53714 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/accumulation.png
+-rw-rw-rw-   0 bishop    (1601)      907     2611 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/file_reader.png
+-rw-rw-rw-   0 bishop    (1601)      907     2013 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/file_writer.png
+-rw-rw-rw-   0 bishop    (1601)      907    63980 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/tools.png
+-rwxrwxrwx   0 bishop    (1601)      907      514 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/wv1d.png
+-rwxrwxrwx   0 bishop    (1601)      907     1168 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/wv2d.png
+-rw-rw-rw-   0 bishop    (1601)      907     5950 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_1D_to_2D.py
+-rw-rw-rw-   0 bishop    (1601)      907     5062 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_2D_to_1D.py
+-rwxrwxrwx   0 bishop    (1601)      907     5027 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_wavefront_file_reader.py
+-rwxrwxrwx   0 bishop    (1601)      907     4179 2018-11-14 21:33:16.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_wavefront_file_writer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/
+-rw-rw-rw-   0 bishop    (1601)      907      272 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/
+-rw-rw-rw-   0 bishop    (1601)      907    31549 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw1d.png
+-rw-rw-rw-   0 bishop    (1601)      907   301469 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw2d.png
+-rw-rw-rw-   0 bishop    (1601)      907    38769 2018-10-04 14:50:28.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/wavefront_propagation.png
+-rw-rw-rw-   0 bishop    (1601)      907    21514 2019-03-28 19:01:51.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_1D.py
+-rw-rw-rw-   0 bishop    (1601)      907    22527 2019-09-17 21:39:10.000000 OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_2D.py
+-rw-r--r--   0 bishop    (1601)      907       38 2020-01-07 20:30:34.000000 OASYS1-WOFRY-1.0.9/setup.cfg
+-rw-rw-rw-   0 bishop    (1601)      907     2767 2020-01-07 20:30:22.000000 OASYS1-WOFRY-1.0.9/setup.py
```

### Comparing `OASYS1-WOFRY-1.0.8/OASYS1_WOFRY.egg-info/SOURCES.txt` & `OASYS1-WOFRY-1.0.9/OASYS1_WOFRY.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MANIFEST.in
-README.txt
+README.md
 setup.py
 OASYS1_WOFRY.egg-info/PKG-INFO
 OASYS1_WOFRY.egg-info/SOURCES.txt
 OASYS1_WOFRY.egg-info/dependency_links.txt
 OASYS1_WOFRY.egg-info/entry_points.txt
 OASYS1_WOFRY.egg-info/namespace_packages.txt
 OASYS1_WOFRY.egg-info/not-zip-safe
```

### Comparing `OASYS1-WOFRY-1.0.8/setup.py` & `OASYS1-WOFRY-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'OASYS1-WOFRY'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'WOFRY (Wave Optics FRamework in pYthon)'
-README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
+README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Manuel Sanchez del Rio, Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
 URL = 'https://github.com/oasys-kit/OASYS-WOFRY'
 DOWNLOAD_URL = 'https://github.com/oasys-kit/OASYS-WOFRY'
 LICENSE = 'GPLv3'
```

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/util/wofry_util.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/util/wofry_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_screen_1d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_screen_1d.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_screen.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_screen.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_stop.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_stop.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_stop_1d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_stop_1d.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_double_slit.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_double_slit.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/screen.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/screen.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/double_slit.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/double_slit.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/ideal_lens.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/ideal_lens.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/ideallens_1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/ideallens_1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/beamline_elements.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/beamline_elements.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/screen1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/screen1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/slit.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/slit.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/stop.jpg` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/stop.jpg`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/icons/slit1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/icons/slit1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_slits_1d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_slits_1d.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens_1d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_ideal_lens_1d.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/beamline_elements/ow_slits.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/beamline_elements/ow_slits.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_2D.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_2D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_1D.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/ow_generic_wavefront_1D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw2d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw2d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/wavefront_propagation.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/wavefront_propagation.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/wavefront_propagation/icons/gw1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_1D_to_2D.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_1D_to_2D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_2D_to_1D.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_2D_to_1D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_wavefront_file_writer.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_wavefront_file_writer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/2d_to_1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/2d_to_1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/accumulation.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/accumulation.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/tools.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/tools.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/wv1d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/wv1d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/file_reader.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/file_reader.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/file_writer.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/file_writer.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/1d_to_2d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/1d_to_2d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/icons/wv2d.png` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/icons/wv2d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/ow_wavefront_file_reader.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/ow_wavefront_file_reader.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_2d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_2d.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_1D.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/tools/generic_wavefront_viewer_1D.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_wofry_widget.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_wofry_widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_optical_element.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_optical_element.py`

 * *Files identical despite different names*

### Comparing `OASYS1-WOFRY-1.0.8/orangecontrib/wofry/widgets/gui/ow_optical_element_1d.py` & `OASYS1-WOFRY-1.0.9/orangecontrib/wofry/widgets/gui/ow_optical_element_1d.py`

 * *Files identical despite different names*


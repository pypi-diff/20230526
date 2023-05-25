# Comparing `tmp/fstd2nc-0.20230515.0.tar.gz` & `tmp/fstd2nc-0.20230515.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20230515.0.tar", last modified: Mon May 15 23:30:03 2023, max compression
+gzip compressed data, was "dist/fstd2nc-0.20230515.1.tar", last modified: Thu May 25 22:34:38 2023, max compression
```

## Comparing `fstd2nc-0.20230515.0.tar` & `fstd2nc-0.20230515.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.451427 fstd2nc-0.20230515.0/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.0/COPYING
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.0/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-15 23:30:03.451173 fstd2nc-0.20230515.0/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230515.0/README.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.439498 fstd2nc-0.20230515.0/cccbuffer/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/cccdump.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.442374 fstd2nc-0.20230515.0/cccbuffer/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3910 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/ccc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/char.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/grid.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/levels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/superlabels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/cccbuffer/mixins/times.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.443501 fstd2nc-0.20230515.0/fstd2nc/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-05-15 23:27:01.000000 fstd2nc-0.20230515.0/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/extra.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.436426 fstd2nc-0.20230515.0/fstd2nc/locale/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.436484 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.445032 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22410 2023-05-15 23:29:20.000000 fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.450803 fstd2nc-0.20230515.0/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35585 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20216 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    19350 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9126 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    15447 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7119 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4929 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20811 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-04-12 22:40:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    32765 2023-04-13 18:26:53.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37809 2023-05-15 23:00:04.000000 fstd2nc-0.20230515.0/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-04-12 22:40:03.000000 fstd2nc-0.20230515.0/fstd2nc/stdout.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-15 23:30:03.444792 fstd2nc-0.20230515.0/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-15 23:30:02.000000 fstd2nc-0.20230515.0/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1183 2023-05-15 23:30:03.444001 fstd2nc-0.20230515.0/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-05-15 23:30:02.000000 fstd2nc-0.20230515.0/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      170 2023-05-15 23:30:03.444396 fstd2nc-0.20230515.0/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-05-15 23:30:03.444605 fstd2nc-0.20230515.0/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2023-05-15 23:30:03.444833 fstd2nc-0.20230515.0/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230515.0/pyproject.toml
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-05-15 23:30:03.451490 fstd2nc-0.20230515.0/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2514 2023-05-10 00:52:26.000000 fstd2nc-0.20230515.0/setup.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.684986 fstd2nc-0.20230515.1/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.1/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.1/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-25 22:34:38.684718 fstd2nc-0.20230515.1/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230515.1/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.672565 fstd2nc-0.20230515.1/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.675480 fstd2nc-0.20230515.1/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3910 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.676904 fstd2nc-0.20230515.1/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.610655 fstd2nc-0.20230515.1/fstd2nc/locale/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.610728 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.678906 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22410 2023-05-25 22:33:03.000000 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.684293 fstd2nc-0.20230515.1/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35592 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20216 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    19526 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9126 2023-05-25 00:10:49.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    17534 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7119 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4210 2023-05-25 22:08:50.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20811 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    32765 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37809 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.678620 fstd2nc-0.20230515.1/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-25 22:34:38.677185 fstd2nc-0.20230515.1/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1183 2023-05-25 22:34:38.677367 fstd2nc-0.20230515.1/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-05-25 22:34:38.677811 fstd2nc-0.20230515.1/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      170 2023-05-25 22:34:38.678211 fstd2nc-0.20230515.1/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-05-25 22:34:38.678440 fstd2nc-0.20230515.1/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2023-05-25 22:34:38.678661 fstd2nc-0.20230515.1/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230515.1/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-05-25 22:34:38.685044 fstd2nc-0.20230515.1/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2514 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/setup.py
```

### Comparing `fstd2nc-0.20230515.0/COPYING` & `fstd2nc-0.20230515.1/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/COPYING.LESSER` & `fstd2nc-0.20230515.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/PKG-INFO` & `fstd2nc-0.20230515.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20230515.0
+Version: 0.20230515.1
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20230515.0/README.md` & `fstd2nc-0.20230515.1/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/__init__.py` & `fstd2nc-0.20230515.1/cccbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/ccc.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/ccc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/char.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/char.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/grid.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/grid.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/levels.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/levels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/superlabels.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/superlabels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/cccbuffer/mixins/times.py` & `fstd2nc-0.20230515.1/cccbuffer/mixins/times.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/__init__.py` & `fstd2nc-0.20230515.1/fstd2nc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20230515.0"
+__version__ = "0.20230515.1"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/__main__.py` & `fstd2nc-0.20230515.1/fstd2nc/__main__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/extra.py` & `fstd2nc-0.20230515.1/fstd2nc/extra.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-15 23:29+0000\n"
+"POT-Creation-Date: 2023-05-25 22:33+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
 
     # Use existing Buffer object data, if that was provided instead of files.
     if existing_buffer is not None:
       self._files = list(existing_buffer._files)
       headers = {k:v.copy() for k,v in existing_buffer._headers.items()}
 
     nfiles = len(self._files)
-    if nfiles == 0 and len(infiles) > 0:
+    if nfiles == 0 and existing_buffer is None:
       error(_("no input files found!"))
     elif nfiles > 10:
       global _pandas_needed
       _pandas_needed = True
     info(_("Found %d %s"%(nfiles,self._format_plural)))
 
     self._headers = headers
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/ascii.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/compat.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/compat.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/dates.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/dates.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/diaghacks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/ensembles.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/extern.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/extern.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,22 @@
   except (ImportError,AttributeError):
     pass
   fixed[0] = True
 
 class ExternInput (BufferBase):
   @classmethod
   def from_fstpy (cls, table, **kwargs):
+    """
+    Create a Buffer object from an fstpy table of records.
+
+    Parameters
+    ----------
+    table : pandas DataFrame
+        The table of records from fstpy.
+    """
     import numpy as np
     if hasattr(table,'to_pandas'):
       table = table.to_pandas()
     # Construct the record header info from the table.
     fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'nk', 'dateo', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
     headers = {}
     for col in fields:
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/filter.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/filter.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/fstd.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/gridhacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,19 @@
     prm['nbits'] = gid.get('nbits',32)
     prm['etiket'] = gid.get('etiket','ETIKET').ljust(12)
     prm['ni'] = 1; prm['nj'] = 1; prm['nk'] = 1
     prm['ismeta'] = True
     nrecs = len(self._headers['name'])
     new_recs = []
     if 'ax' in gid:
-      new_recs.append(dict(prm, nomvar='>>  ', ni=gid['ni'], d=gid['ax']))
+      new_recs.append(dict(prm, nomvar='>>  ', ni=gid['ni'], d=gid['ax'], dtype=gid['ax'].dtype))
     if 'ay' in gid:
-      new_recs.append(dict(prm, nomvar='^^  ', nj=gid['nj'], d=gid['ay']))
+      new_recs.append(dict(prm, nomvar='^^  ', nj=gid['nj'], d=gid['ay'], dtype=gid['ay'].dtype))
     if 'axy' in gid:
-      new_recs.append(dict(prm, nomvar='^>  ', ni=gid['ni'], nj=gid['nj'], d=gid['axy']))
+      new_recs.append(dict(prm, nomvar='^>  ', ni=gid['ni'], nj=gid['nj'], d=gid['axy'], dtype=gid['axy'].dtype))
     for k,v in self._headers.items():
       if hasattr(v,'mask'):
         self._headers[k] = np.ma.zeros(shape=nrecs + len(new_recs), dtype=v.dtype)
       else:
         self._headers[k] = np.zeros(shape=nrecs + len(new_recs), dtype=v.dtype)
       self._headers[k][:nrecs] = v[:]
     for i in range(len(new_recs)):
@@ -114,16 +114,70 @@
     grid_args = [number(v) for v in interp[1:] if '=' not in v]
     grid_kwargs = dict(v.split('=') for v in interp[1:] if '=' in v)
     grid_kwargs = dict((k,number(v)) for k,v in grid_kwargs.items())
     if not hasattr(rmn,'defGrid_'+grtyp):
       error(_("Unknown grid '%s'")%grtyp)
     return getattr(rmn,'defGrid_'+grtyp)(*grid_args,**grid_kwargs)
 
-# Keep track of valid grid ids (to detect if we have a problem with grid ids)
-_valid_gids = set()
+# Helper method - pack up grid id for transport to other processes.
+# Converts to a dictionary, then to a tuple of key/value pairs.
+from fstd2nc.mixins import vectorize
+@vectorize
+def _pack_grid (gid):
+  import rpnpy.librmn.all as rmn
+  def _pack_item (item):
+    k, v = item
+    if k == 'subgrid':
+      return (k,tuple(map(_pack_dict,v)))
+    if hasattr(v,'dumps'):  # Numpy array
+      return (k,v.dumps())
+    return (k,v)
+  def _pack_dict (d):
+    d = d.copy()
+    d.pop('id',None)
+    d.pop('subgridid',None)
+    return tuple(map(_pack_item,d.items()))
+  if gid < 0: return None
+  with _lock:
+    grid = rmn.decodeGrid(int(gid))
+    return _pack_dict(grid)
+del vectorize
+
+# Helper method - unpack a grid after transport to another processor.
+# Returns an active grid id that's valid for this processor.
+_grid_lookup = {}
+def _unpack_grid (grid):
+  import rpnpy.librmn.all as rmn
+  from pickle import loads
+  def _unpack_item (item):
+    k, v = item
+    if k == 'subgrid':
+      return (k,list(map(_unpack_dict,v)))
+    if isinstance(v,bytes):  # Numpy array
+      return (k,loads(v))
+    return (k,v)
+  def _unpack_dict (d):
+    return dict(map(_unpack_item,d))
+  if grid is None: return -1
+  # Check if grid already handled.
+  for gid, g in _grid_lookup.items():
+    if g is grid: return gid
+  # Otherwise, start unpacking it.
+  packed_grid = grid
+  grid = _unpack_dict(grid)
+  with _lock:
+    # Special case: super grid
+    if 'subgrid' in grid:
+      subgrids = [rmn.encodeGrid(subgrid)['id'] for subgrid in grid['subgrid']]
+      gid = rmn.ezgdef_supergrid(grid['ni'], grid['nj'], grid['grtyp'], grid['grref'], grid['version'], subgrids)
+    else:
+      gid = rmn.encodeGrid(grid)['id']
+  _grid_lookup[gid] = packed_grid
+  return gid
+
 
 class Interp (BufferBase):
 
   @classmethod
   def _cmdline_args (cls, parser):
     from argparse import SUPPRESS
     super(Interp,cls)._cmdline_args(parser)
@@ -141,20 +195,19 @@
     super(Interp,self).__init__(*args,**kwargs)
     # Extract interpolation grid.
     if interp is not None:
       interp_grid = _get_interp_grid(interp)
       self._interp_grid = interp_grid
       # Hack the new grid descriptors into the headers.
       self._writeGrid (interp_grid)
-      _valid_gids.add(interp_grid['id'])
 
       # Store original and modified versions of the grid descriptors.
-      self._decoder_extra_args = self._decoder_extra_args + ('source_gid','dest_gid')
-      self._ignore_atts = self._ignore_atts + ('source_gid','dest_gid')
-      self._headers['source_gid'] = np.empty(self._nrecs,dtype=object)
+      self._decoder_extra_args = self._decoder_extra_args + ('source_grid','dest_grid')
+      self._ignore_atts = self._ignore_atts + ('source_grid','dest_grid')
+      self._headers['source_grid'] = np.empty(self._nrecs,dtype=object)
 
       # Set up some options for ezsint.
       import rpnpy.librmn.all as rmn
       rmn.ezsetopt (rmn.EZ_OPT_EXTRAP_DEGREE, rmn.EZ_EXTRAP_VALUE)
       rmn.ezsetopt (rmn.EZ_OPT_EXTRAP_VALUE, self._fill_value)
 
 
@@ -166,16 +219,15 @@
       return super(Interp,self)._makevars()
 
     # Run _makevars chain with original grid descriptors to allow
     # xycoords to give us source grid ids,
     # switch out the grid descriptors in the table, then let xycoords
     # construct the target grid axes for us.
     super(Interp,self)._makevars()
-    self._headers['source_gid'][:] = np.array(self._gids)
-    _valid_gids.update(g for g in self._gids if g >= 0)
+    self._headers['source_grid'][:] = _pack_grid(self._gids)
     # Now, use interpolated grid descriptors.
     ismeta = self._headers['ismeta']
     for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
       self._headers[key][:] = np.where(ismeta, self._headers[key], self._interp_grid[key])
     super(Interp,self)._makevars()
 
     # Add fill value to the data.
@@ -185,37 +237,37 @@
     for var in self._varlist:
       if isinstance(var,_iter_type):
         var.atts['_FillValue'] = var.dtype.type(self._fill_value)
 
   def _decoder_scalar_args (self):
     args = super(Interp,self)._decoder_scalar_args()
     if hasattr(self,'_interp_grid'):
-      args['dest_gid'] = self._interp_grid['id']
+      args['dest_grid'] = _pack_grid(self._interp_grid['id'])
     return args
 
   # Handle grid interpolations from raw binary array.
   @classmethod
-  def _decode (cls, data, source_gid=None, dest_gid=None, **kwargs):
+  def _decode (cls, data, source_grid=None, dest_grid=None, **kwargs):
     import rpnpy.librmn.all as rmn
     import numpy as np
-    if source_gid is None or dest_gid is None:
+    # If no interpolation requested, nothing to do.
+    if source_grid is None or dest_grid is None:
       return super(Interp,cls)._decode (data, **kwargs)
-    if source_gid not in _valid_gids or dest_gid not in _valid_gids:
-      error(_("Problem finding grid id.  It's possible that you're running this in a multi-processing environment, which does not support the 'interp' option."))
-    # Retrieve an active librmn grid id associated with this grid.
-    if source_gid < 0:
+    source_grid = _unpack_grid(source_grid)
+    dest_grid = _unpack_grid(dest_grid)
+    if source_grid < 0:
       raise ValueError("Source data is not on a recognized grid.  Unable to interpolate.")
     d = super(Interp,cls)._decode (data, **kwargs).T
     with _lock:
       # Propogate any fill values to the interpolated grid.
       fill_value = kwargs.get('fill_value')
       in_mask = np.zeros(d.shape, order='F', dtype='float32')
       in_mask[d==fill_value] = 1.0
-      d = rmn.ezsint (dest_gid, source_gid, d)
-      out_mask = rmn.ezsint (dest_gid, source_gid, in_mask)
+      d = rmn.ezsint (dest_grid, source_grid, d)
+      out_mask = rmn.ezsint (dest_grid, source_grid, in_mask)
       d[out_mask!=0] = fill_value
       # Return the data for the interpolated field.
       return d.T
 
 
 #################################################
 # Mixin for yin/yang grid subsetting.
@@ -322,18 +374,25 @@
     # Load the metadata from the file(s).
     super(Crop,self).__init__(*args,**kwargs)
 
     if not self._crop_to_smallest_grid:
       return
 
     # Keep track of cropping regions for the data.
-    self._decoder_extra_args = self._decoder_extra_args + ('crop_j','crop_i')
-    self._headers['crop_j'] = np.empty(self._nrecs,object)
-    self._headers['crop_i'] = np.empty(self._nrecs,object)
-    self._ignore_atts = self._ignore_atts + ('crop_j','crop_i')
+    self._decoder_extra_args = self._decoder_extra_args + ('crop_j0','crop_jN','crop_i0','crop_iN')
+    self._headers['crop_j0'] = np.empty(self._nrecs,'int32')
+    self._headers['crop_jN'] = np.empty(self._nrecs,'int32')
+    self._headers['crop_i0'] = np.empty(self._nrecs,'int32')
+    self._headers['crop_iN'] = np.empty(self._nrecs,'int32')
+    # Initialize with default values, to avoid processing garbage indices.
+    self._headers['crop_j0'][:] = 0
+    self._headers['crop_jN'][:] = self._headers['nj']
+    self._headers['crop_i0'][:] = 0
+    self._headers['crop_iN'][:] = self._headers['ni']
+    self._ignore_atts = self._ignore_atts + ('crop_j0','crop_jN','crop_i0','crop_iN')
 
     # Run _makevars early to generate grid ids with xycoords mixin.
     # Silence warnings from makevars, which might not be relevant to the final
     # state after we make our grid modifications.
     import fstd2nc
     streams = fstd2nc.stdout.streams
     fstd2nc.stdout.streams = ()
@@ -375,21 +434,23 @@
         if jN-j0 != smallest_grid['nj']: continue
         if np.any(grid['ax'].flatten()[i0:iN] != smallest_grid['ax'].flatten()): continue
         if np.any(grid['ay'].flatten()[j0:jN] != smallest_grid['ay'].flatten()): continue
         # Able to crop, so update the headers to point to the cropped coordinates.
         submask = (self._headers['ig1'] == grid['tag1']) & (self._headers['ig2'] == grid['tag2']) & (self._headers['ig3'] == grid['tag3'])
         for key in ('grtyp','ni','nj','ig1','ig2','ig3','ig4'):
           self._headers[key][submask] = smallest_grid[key]
-        self._headers['crop_j'][submask] = slice(j0,jN)
-        self._headers['crop_i'][submask] = slice(i0,iN)
+        self._headers['crop_j0'][submask] = j0
+        self._headers['crop_jN'][submask] = jN
+        self._headers['crop_i0'][submask] = i0
+        self._headers['crop_iN'][submask] = iN
 
   # Handle cropping from raw binary array.
   @classmethod
-  def _decode (cls, data, crop_j=None, crop_i=None, **kwargs):
+  def _decode (cls, data, crop_j0=None, crop_jN=None, crop_i0=None, crop_iN=None, **kwargs):
     d = super(Crop,cls)._decode (data, **kwargs)
-    if crop_j is not None:
-      d = d[crop_j,:]
-    if crop_i is not None:
-      d = d[:,crop_i]
+    if crop_j0 is not None and crop_jN is not None:
+      d = d[crop_j0:crop_jN,:]
+    if crop_i0 is not None and crop_iN is not None:
+      d = d[:,crop_i0:crop_iN]
     return d
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/masks.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/masks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/mesh.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #
 # https://ugrid-conventions.github.io/ugrid-conventions/
 #
 
 class Mesh (BufferBase):
   def __init__ (self, *args, **kwargs):
     # Tell the decoder not to process horizontal records as variables.
-    #self._maybe_meta_records = self._maybe_meta_records + (b'##',)
+    self._maybe_meta_records = self._maybe_meta_records + (b'##',)
     super(Mesh,self).__init__(*args,**kwargs)
 
   # Add horizontal coordinate info to the data.
   def _makevars (self):
     from fstd2nc.mixins import _iter_type, _var_type, _axis_type, _dim_type
     from collections import OrderedDict
     import numpy as np
@@ -43,51 +43,44 @@
 
     # Scan for mesh coordinates.
     three = _dim_type ('Three', 3)
     mesh_indices = OrderedDict()
     lats = OrderedDict()
     lons = OrderedDict()
     for var in self._varlist:
-      # Look for face node indices ('##' field).
-      if var.name == '##':
-        var.name = 'mesh_face_nodes'
-        # Reshape to (nFaces,3)
-        if 'i' in var.dims:
-          ind = var.dims.index('i')
-          faces = _dim_type ('nFaces', var.shape[ind]//3)
-          if var.shape[ind] % 3 == 0:
-            var.axes = var.axes[:ind] + [faces, three] + var.axes[ind+1:]
-            shape = var.record_id.shape
-        # Remove degenerate height dimension.
-        if 'height' in var.dims:
-          ind = var.dims.index('height')
-          var.axes = var.axes[:ind] + var.axes[ind+1:]
-          var.record_id = var.record_id.reshape(shape[:ind]+shape[ind+1:])
-        mesh_indices[(var.atts['ip1'],var.atts['ip2'])] = var
-        # Remove coordinate arrays.
-        var.atts.pop('coordinates',None)
+      if var.atts.get('grtyp',None) != 'M': continue
+      key = (var.atts['ig1'], var.atts['ig2'])
+      if key not in mesh_indices:
+        # Look for face node indices ('##' field).
+        mesh = self._find_coord(var,b'##  ')  # Borrowed from xycoords.
+        d = mesh['d'].transpose().squeeze()
+        if (d.ndim == 1):
+          faces = _dim_type ('nFaces', len(d)//3)
+          d = d.reshape(len(d)//3,-1)
+          atts = OrderedDict([("long_name","Vertices index of triangular meshe (TIN)"),("description","Index of the vertices position encoded in the ^^ >> fields which constitutes a triangular mesh")])
+          mesh = _var_type('mesh_face_nodes',atts, [faces,three], d)
+          mesh_indices[key] = mesh
       # Look for lat/lon coordinates.
-      if var.atts.get('grtyp',None) == 'M':
-        for coord in var.atts.get('coordinates',[]):
-          if coord.name == 'lat':
-            lats[var.atts['ig1'],var.atts['ig2']] = coord
-          if coord.name == 'lon':
-            lons[var.atts['ig1'],var.atts['ig2']] = coord
+      for coord in var.atts.get('coordinates',[]):
+        if coord.name == 'lat':
+          lats[key] = coord
+        if coord.name == 'lon':
+          lons[key] = coord
 
     if len(mesh_indices) == 0: return
 
     # Create toplogy variable(s)
     topos = OrderedDict()
     for key in mesh_indices.keys():
       coordinates = []
       if key in lats: coordinates.append(lats[key])
       if key in lons: coordinates.append(lons[key])
       atts = OrderedDict()
       atts['cf_role'] = 'mesh_topology'
-      atts['topology_dimension'] = 2
+      atts['topology_dimension'] = np.int32(2)
       atts['node_coordinates'] = coordinates
       atts['face_node_connectivity'] = mesh_indices[key]
       topo = _var_type ('Mesh', atts, (), np.int32(0))
       topos[key] = topo
 
     # Add toplogy information to data variables.
     # Also, update 'i' dimension to be nNodes for the data variables.
@@ -106,20 +99,7 @@
         if key not in reftimes:
           for coord in var.atts.get('coordinates',[]):
             if coord.name == 'reftime':
               reftimes[key] = coord
           if 'time' in var.dims:
             times[key] = var.axes[var.dims.index('time')]
 
-    # Need to fix the time axis for the lat / lon / triangle indices
-    # (from '^^', '>>', '##' records).
-    # They may not include the forecast period.
-    for key in topos.keys():
-      if key in times and key in reftimes:
-        for category in mesh_indices, lats, lons:
-          if key in category:
-            var = category[key]
-            if 'time' in var.dims:
-              ind = var.dims.index('time')
-              if np.all(var.axes[ind].array == reftimes[key].array):
-                var.axes[ind] = times[key]
-
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/misc.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/misc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/netcdf.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/pruneaxes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/removestuff.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/select.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/select.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/series.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/series.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/sfc_codes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/vardict.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/vcoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20230515.1/fstd2nc/mixins/xycoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc/stdout.py` & `fstd2nc-0.20230515.1/fstd2nc/stdout.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20230515.1/fstd2nc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20230515.0
+Version: 0.20230515.1
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20230515.0/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20230515.1/fstd2nc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.0/setup.py` & `fstd2nc-0.20230515.1/setup.py`

 * *Files identical despite different names*


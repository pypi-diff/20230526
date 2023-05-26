# Comparing `tmp/tmart-1.3.5.tar.gz` & `tmp/tmart-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-1.3.5.tar", last modified: Tue Apr 18 04:12:39 2023, max compression
+gzip compressed data, was "tmart-1.3.6.tar", last modified: Fri May 26 07:15:41 2023, max compression
```

## Comparing `tmart-1.3.5.tar` & `tmart-1.3.6.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.030787 tmart-1.3.5/
--rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.5/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     3891 2023-04-18 04:12:39.030585 tmart-1.3.5/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     3269 2023-04-13 02:42:26.000000 tmart-1.3.5/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-18 04:12:39.030847 tmart-1.3.5/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-18 04:12:02.000000 tmart-1.3.5/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.007312 tmart-1.3.5/tests/
--rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.5/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.5/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.5/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.5/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.5/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.5/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.5/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.5/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.5/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.5/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.016323 tmart-1.3.5/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.018388 tmart-1.3.5/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)      449 2023-04-12 06:15:34.000000 tmart-1.3.5/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5017 2023-04-18 02:10:19.000000 tmart-1.3.5/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)     1411 2023-04-12 07:00:02.000000 tmart-1.3.5/tmart/AEC/read_PRISMA_north.py
--rw-r--r--   0 yw         (501) staff       (20)     2864 2023-04-12 04:52:05.000000 tmart-1.3.5/tmart/AEC/read_PRISMA_vaa.py
--rw-r--r--   0 yw         (501) staff       (20)     3140 2023-04-18 01:29:46.000000 tmart-1.3.5/tmart/AEC/reflectance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.5/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.5/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.5/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.5/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.5/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.5/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.022246 tmart-1.3.5/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.029112 tmart-1.3.5/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.5/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.5/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.5/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.5/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.5/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.5/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.5/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.5/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.5/tmart/ancillary/whitecap_factor.csv
--rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.5/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.5/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.5/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.5/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.5/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.5/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.5/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.017042 tmart-1.3.5/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     3891 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     1335 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.044920 tmart-1.3.6/
+-rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.6/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     4092 2023-05-26 07:15:41.044727 tmart-1.3.6/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     3470 2023-04-18 23:02:02.000000 tmart-1.3.6/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2023-05-26 07:15:41.044979 tmart-1.3.6/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     1986 2023-05-26 07:13:23.000000 tmart-1.3.6/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.026492 tmart-1.3.6/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.6/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     2960 2023-05-23 22:19:27.000000 tmart-1.3.6/tests/test_AE_modelling.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.6/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.6/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.6/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.6/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)      824 2023-05-26 03:52:15.000000 tmart-1.3.6/tests/test_calc_rho.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.6/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     2036 2023-05-23 20:57:30.000000 tmart-1.3.6/tests/test_plot.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.6/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.6/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.6/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.6/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.030748 tmart-1.3.6/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.033163 tmart-1.3.6/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)      449 2023-04-12 06:15:34.000000 tmart-1.3.6/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5018 2023-05-13 21:27:01.000000 tmart-1.3.6/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)     1138 2023-05-13 21:27:35.000000 tmart-1.3.6/tmart/AEC/read_PRISMA_north.py
+-rw-r--r--   0 yw         (501) staff       (20)     2905 2023-05-13 21:26:48.000000 tmart-1.3.6/tmart/AEC/read_PRISMA_vaa.py
+-rw-r--r--   0 yw         (501) staff       (20)     3141 2023-05-13 21:27:47.000000 tmart-1.3.6/tmart/AEC/reflectance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     2319 2023-05-13 21:28:04.000000 tmart-1.3.6/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    10525 2023-05-13 21:28:08.000000 tmart-1.3.6/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)    10106 2023-05-13 21:28:16.000000 tmart-1.3.6/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13617 2023-05-13 21:28:56.000000 tmart-1.3.6/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    41653 2023-05-23 22:09:09.000000 tmart-1.3.6/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      550 2023-05-26 03:08:33.000000 tmart-1.3.6/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.037169 tmart-1.3.6/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.042977 tmart-1.3.6/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.6/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.6/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.6/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.6/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.6/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.6/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.6/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.6/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.6/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.6/tmart/ancillary/whitecap_factor.csv
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.044501 tmart-1.3.6/tmart/surface_rho/
+-rw-r--r--   0 yw         (501) staff       (20)      341 2023-05-23 22:27:30.000000 tmart-1.3.6/tmart/surface_rho/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5038 2023-05-26 03:24:34.000000 tmart-1.3.6/tmart/surface_rho/calculate.py
+-rw-r--r--   0 yw         (501) staff       (20)     2681 2023-05-13 21:28:43.000000 tmart-1.3.6/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)    11782 2023-05-13 21:28:20.000000 tmart-1.3.6/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     4097 2023-05-13 21:28:28.000000 tmart-1.3.6/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    19401 2023-05-13 21:28:34.000000 tmart-1.3.6/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11285 2023-05-13 21:28:39.000000 tmart-1.3.6/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     8647 2023-05-13 21:28:47.000000 tmart-1.3.6/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    20016 2023-05-13 21:28:52.000000 tmart-1.3.6/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-05-26 07:15:41.031751 tmart-1.3.6/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     4092 2023-05-26 07:15:40.000000 tmart-1.3.6/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     1465 2023-05-26 07:15:40.000000 tmart-1.3.6/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2023-05-26 07:15:40.000000 tmart-1.3.6/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       50 2023-05-26 07:15:40.000000 tmart-1.3.6/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2023-05-26 07:15:40.000000 tmart-1.3.6/tmart.egg-info/top_level.txt
```

### Comparing `tmart-1.3.5/PKG-INFO` & `tmart-1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746d 6172  : 2.1.Name: tmar
-00000020: 740a 5665 7273 696f 6e3a 2031 2e33 2e35  t.Version: 1.3.5
+00000020: 740a 5665 7273 696f 6e3a 2031 2e33 2e36  t.Version: 1.3.6
 00000030: 0a53 756d 6d61 7279 3a20 5261 6469 6174  .Summary: Radiat
 00000040: 6976 6520 7472 616e 7366 6572 206d 6f64  ive transfer mod
 00000050: 656c 6c69 6e67 2066 6f72 2061 7175 6174  elling for aquat
 00000060: 6963 2072 656d 6f74 6520 7365 6e73 696e  ic remote sensin
 00000070: 670a 4175 7468 6f72 3a20 5975 6c75 6e20  g.Author: Yulun 
 00000080: 5775 0a43 6c61 7373 6966 6965 723a 2049  Wu.Classifier: I
 00000090: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
@@ -161,84 +161,96 @@
 00000a00: 756d 6d65 7229 200a 6165 726f 736f 6c5f  ummer) .aerosol_
 00000a10: 7479 7065 203d 2027 4d61 7269 7469 6d65  type = 'Maritime
 00000a20: 2720 200a 6d79 5f61 746d 203d 2074 6d61  '  .my_atm = tma
 00000a30: 7274 2e41 746d 6f73 7068 6572 6528 6174  rt.Atmosphere(at
 00000a40: 6d5f 7072 6f66 696c 652c 2061 6f74 3535  m_profile, aot55
 00000a50: 3020 3d20 302c 2061 6572 6f73 6f6c 5f74  0 = 0, aerosol_t
 00000a60: 7970 6520 3d20 274d 6172 6974 696d 6527  ype = 'Maritime'
-00000a70: 2020 290a 0a23 2323 2052 756e 6e69 6e67    )..### Running
-00000a80: 2054 2d4d 6172 7420 2323 230a 6d79 5f74   T-Mart ###.my_t
-00000a90: 6d61 7274 203d 2074 6d61 7274 2e54 6d61  mart = tmart.Tma
-00000aa0: 7274 2853 7572 6661 6365 203d 206d 795f  rt(Surface = my_
-00000ab0: 7375 7266 6163 652c 2041 746d 6f73 7068  surface, Atmosph
-00000ac0: 6572 653d 206d 795f 6174 6d2c 2073 6861  ere= my_atm, sha
-00000ad0: 646f 773d 4661 6c73 6529 0a6d 795f 746d  dow=False).my_tm
-00000ae0: 6172 742e 7365 745f 6765 6f6d 6574 7279  art.set_geometry
-00000af0: 2873 656e 736f 725f 636f 6f72 6473 3d5b  (sensor_coords=[
-00000b00: 3531 2c35 302c 3133 305f 3030 305d 2c20  51,50,130_000], 
-00000b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b20: 2020 2020 2020 2074 6172 6765 745f 7074         target_pt
-00000b30: 5f64 6972 6563 7469 6f6e 3d5b 3138 302c  _direction=[180,
-00000b40: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00000b50: 2020 2020 2020 2020 2020 7375 6e5f 6469            sun_di
-00000b60: 723d 5b30 2c30 5d29 0a0a 7265 7375 6c74  r=[0,0])..result
-00000b70: 7320 3d20 6d79 5f74 6d61 7274 2e72 756e  s = my_tmart.run
-00000b80: 2877 6c3d 776c 2c20 6261 6e64 3d4e 6f6e  (wl=wl, band=Non
-00000b90: 652c 206e 5f70 686f 746f 6e3d 3130 5f30  e, n_photon=10_0
-00000ba0: 3030 290a 0a23 2043 616c 6375 6c61 7465  00)..# Calculate
-00000bb0: 2072 6566 6c65 6374 616e 6365 7320 7573   reflectances us
-00000bc0: 696e 6720 7265 636f 7264 6564 2070 686f  ing recorded pho
-00000bd0: 746f 6e20 696e 666f 726d 6174 696f 6e20  ton information 
-00000be0: 0a52 203d 2074 6d61 7274 2e63 616c 635f  .R = tmart.calc_
-00000bf0: 7265 6628 7265 7375 6c74 7329 0a66 6f72  ref(results).for
-00000c00: 206b 2c20 7620 696e 2052 2e69 7465 6d73   k, v in R.items
-00000c10: 2829 3a0a 2020 2020 7072 696e 7428 6b2c  ():.    print(k,
-00000c20: 2027 2020 2020 2027 202c 2076 290a 0a60   '     ' , v)..`
-00000c30: 6060 0a0a 4f75 7470 7574 2073 686f 756c  ``..Output shoul
-00000c40: 6420 6265 2073 696d 696c 6172 2074 6f20  d be similar to 
-00000c50: 7468 6973 3a20 0a0a 6060 600a 3d3d 3d3d  this: ..```.====
-00000c60: 3d3d 3d3d 3d20 496e 6974 6961 7469 6e67  ===== Initiating
-00000c70: 2054 2d4d 6172 7420 3d3d 3d3d 3d3d 3d3d   T-Mart ========
-00000c80: 3d0a 4e75 6d62 6572 206f 6620 7068 6f74  =.Number of phot
-00000c90: 6f6e 733a 2031 3030 3030 0a55 7369 6e67  ons: 10000.Using
-00000ca0: 2031 3020 636f 7265 2873 290a 4e75 6d62   10 core(s).Numb
-00000cb0: 6572 206f 6620 6a6f 6228 7329 3a20 3130  er of job(s): 10
-00000cc0: 300a 5761 7665 6c65 6e67 7468 3a20 3430  0.Wavelength: 40
-00000cd0: 300a 7461 7267 6574 5f70 745f 6469 7265  0.target_pt_dire
-00000ce0: 6374 696f 6e3a 205b 3138 302c 2030 5d0a  ction: [180, 0].
-00000cf0: 7375 6e5f 6469 723a 205b 302c 2030 5d0a  sun_dir: [0, 0].
-00000d00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d20: 3d3d 3d3d 3d0a 5461 736b 7320 7265 6d61  =====.Tasks rema
-00000d30: 696e 696e 6720 3d20 3130 320a 5461 736b  ining = 102.Task
-00000d40: 7320 7265 6d61 696e 696e 6720 3d20 3732  s remaining = 72
-00000d50: 0a54 6173 6b73 2072 656d 6169 6e69 6e67  .Tasks remaining
-00000d60: 203d 2034 320a 5461 736b 7320 7265 6d61   = 42.Tasks rema
-00000d70: 696e 696e 6720 3d20 3132 0a3d 3d3d 3d3d  ining = 12.=====
-00000d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000da0: 0a43 616c 6375 6c61 7469 6e67 2072 6164  .Calculating rad
-00000db0: 6961 7469 7665 2070 726f 7065 7274 6965  iative propertie
-00000dc0: 732e 2e2e 0a52 5f61 746d 2020 2020 2020  s....R_atm      
-00000dd0: 2030 2e31 3237 3630 3538 3938 3839 3832   0.1276058988982
-00000de0: 3335 3837 0a52 5f64 6972 2020 2020 2020  3587.R_dir      
-00000df0: 2030 2e30 3630 3436 3431 3930 3137 3230   0.0604641901720
-00000e00: 3130 3637 0a52 5f65 6e76 2020 2020 2020  1067.R_env      
-00000e10: 2030 2e30 3132 3838 3835 3930 3534 3731   0.0128885905471
-00000e20: 3239 3830 350a 525f 746f 7461 6c20 2020  29805.R_total   
-00000e30: 2020 2020 302e 3230 3039 3538 3637 3936      0.2009586796
-00000e40: 3137 3337 3633 350a 0a60 6060 0a0a 0a0a  1737635..```....
-00000e50: 2323 204f 7468 6572 0a0a 542d 4d61 7274  ## Other..T-Mart
-00000e60: 2063 616e 2063 616c 6375 6c61 7465 2072   can calculate r
-00000e70: 6566 6c65 6374 616e 6365 7320 6f66 2076  eflectances of v
-00000e80: 6172 696f 7573 2075 6e69 7473 2c20 7365  arious units, se
-00000e90: 6520 5461 626c 6520 3120 696e 2057 7520  e Table 1 in Wu 
-00000ea0: 6574 2061 6c2e 2028 3230 3233 292e 200a  et al. (2023). .
-00000eb0: 0a46 6f72 2071 7565 7374 696f 6e73 2061  .For questions a
-00000ec0: 6e64 2073 7567 6765 7374 696f 6e73 2028  nd suggestions (
-00000ed0: 7768 6963 6820 4927 6d20 616c 7761 7973  which I'm always
-00000ee0: 206f 7065 6e20 746f 2129 2c20 706c 6561   open to!), plea
-00000ef0: 7365 2065 6d61 696c 2059 756c 756e 2061  se email Yulun a
-00000f00: 7420 5b79 756c 756e 7775 3840 676d 6169  t [yulunwu8@gmai
-00000f10: 6c2e 636f 6d5d 286d 6169 6c74 6f3a 7975  l.com](mailto:yu
-00000f20: 6c75 6e77 7538 4067 6d61 696c 2e63 6f6d  lunwu8@gmail.com
-00000f30: 290a 0a                                  )..
+00000a70: 2020 290a 0a23 2323 2043 7265 6174 6520    )..### Create 
+00000a80: 542d 4d61 7274 204f 626a 6563 7420 2323  T-Mart Object ##
+00000a90: 230a 6d79 5f74 6d61 7274 203d 2074 6d61  #.my_tmart = tma
+00000aa0: 7274 2e54 6d61 7274 2853 7572 6661 6365  rt.Tmart(Surface
+00000ab0: 203d 206d 795f 7375 7266 6163 652c 2041   = my_surface, A
+00000ac0: 746d 6f73 7068 6572 653d 206d 795f 6174  tmosphere= my_at
+00000ad0: 6d2c 2073 6861 646f 773d 4661 6c73 6529  m, shadow=False)
+00000ae0: 0a6d 795f 746d 6172 742e 7365 745f 6765  .my_tmart.set_ge
+00000af0: 6f6d 6574 7279 2873 656e 736f 725f 636f  ometry(sensor_co
+00000b00: 6f72 6473 3d5b 3531 2c35 302c 3133 305f  ords=[51,50,130_
+00000b10: 3030 305d 2c20 0a20 2020 2020 2020 2020  000], .         
+00000b20: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00000b30: 6765 745f 7074 5f64 6972 6563 7469 6f6e  get_pt_direction
+00000b40: 3d5b 3138 302c 305d 2c0a 2020 2020 2020  =[180,0],.      
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 7375 6e5f 6469 723d 5b30 2c30 5d29 0a0a  sun_dir=[0,0])..
+00000b70: 2323 2320 4d75 6c74 6970 726f 6365 7373  ### Multiprocess
+00000b80: 696e 6720 6e65 6564 7320 746f 2062 6520  ing needs to be 
+00000b90: 7772 6170 7065 6420 696e 2027 6966 205f  wrapped in 'if _
+00000ba0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
+00000bb0: 696e 5f5f 223a 2720 666f 7220 5769 6e64  in__":' for Wind
+00000bc0: 6f77 7320 7379 7374 656d 732e 200a 2323  ows systems. .##
+00000bd0: 2320 5468 6973 2063 616e 2062 6520 6967  # This can be ig
+00000be0: 6e6f 7265 6420 666f 7220 4c69 6e75 782d  nored for Linux-
+00000bf0: 6261 7365 6420 7379 7374 656d 732e 200a  based systems. .
+00000c00: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+00000c10: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2072  __main__":.    r
+00000c20: 6573 756c 7473 203d 206d 795f 746d 6172  esults = my_tmar
+00000c30: 742e 7275 6e28 776c 3d77 6c2c 2062 616e  t.run(wl=wl, ban
+00000c40: 643d 4e6f 6e65 2c20 6e5f 7068 6f74 6f6e  d=None, n_photon
+00000c50: 3d31 305f 3030 3029 0a20 2020 200a 2020  =10_000).    .  
+00000c60: 2020 2320 4361 6c63 756c 6174 6520 7265    # Calculate re
+00000c70: 666c 6563 7461 6e63 6573 2075 7369 6e67  flectances using
+00000c80: 2072 6563 6f72 6465 6420 7068 6f74 6f6e   recorded photon
+00000c90: 2069 6e66 6f72 6d61 7469 6f6e 200a 2020   information .  
+00000ca0: 2020 5220 3d20 746d 6172 742e 6361 6c63    R = tmart.calc
+00000cb0: 5f72 6566 2872 6573 756c 7473 290a 2020  _ref(results).  
+00000cc0: 2020 666f 7220 6b2c 2076 2069 6e20 522e    for k, v in R.
+00000cd0: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00000ce0: 2070 7269 6e74 286b 2c20 2720 2020 2020   print(k, '     
+00000cf0: 2720 2c20 7629 0a0a 6060 600a 0a4f 7574  ' , v)..```..Out
+00000d00: 7075 7420 7368 6f75 6c64 2062 6520 7369  put should be si
+00000d10: 6d69 6c61 7220 746f 2074 6869 733a 200a  milar to this: .
+00000d20: 0a60 6060 0a3d 3d3d 3d3d 3d3d 3d3d 2049  .```.========= I
+00000d30: 6e69 7469 6174 696e 6720 542d 4d61 7274  nitiating T-Mart
+00000d40: 203d 3d3d 3d3d 3d3d 3d3d 0a4e 756d 6265   =========.Numbe
+00000d50: 7220 6f66 2070 686f 746f 6e73 3a20 3130  r of photons: 10
+00000d60: 3030 300a 5573 696e 6720 3130 2063 6f72  000.Using 10 cor
+00000d70: 6528 7329 0a4e 756d 6265 7220 6f66 206a  e(s).Number of j
+00000d80: 6f62 2873 293a 2031 3030 0a57 6176 656c  ob(s): 100.Wavel
+00000d90: 656e 6774 683a 2034 3030 0a74 6172 6765  ength: 400.targe
+00000da0: 745f 7074 5f64 6972 6563 7469 6f6e 3a20  t_pt_direction: 
+00000db0: 5b31 3830 2c20 305d 0a73 756e 5f64 6972  [180, 0].sun_dir
+00000dc0: 3a20 5b30 2c20 305d 0a3d 3d3d 3d3d 3d3d  : [0, 0].=======
+00000dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000de0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a54  ==============.T
+00000df0: 6173 6b73 2072 656d 6169 6e69 6e67 203d  asks remaining =
+00000e00: 2031 3032 0a54 6173 6b73 2072 656d 6169   102.Tasks remai
+00000e10: 6e69 6e67 203d 2037 320a 5461 736b 7320  ning = 72.Tasks 
+00000e20: 7265 6d61 696e 696e 6720 3d20 3432 0a54  remaining = 42.T
+00000e30: 6173 6b73 2072 656d 6169 6e69 6e67 203d  asks remaining =
+00000e40: 2031 320a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   12.============
+00000e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000e60: 3d3d 3d3d 3d3d 3d3d 3d0a 4361 6c63 756c  =========.Calcul
+00000e70: 6174 696e 6720 7261 6469 6174 6976 6520  ating radiative 
+00000e80: 7072 6f70 6572 7469 6573 2e2e 2e0a 525f  properties....R_
+00000e90: 6174 6d20 2020 2020 2020 302e 3132 3736  atm       0.1276
+00000ea0: 3035 3839 3838 3938 3233 3538 370a 525f  0589889823587.R_
+00000eb0: 6469 7220 2020 2020 2020 302e 3036 3034  dir       0.0604
+00000ec0: 3634 3139 3031 3732 3031 3036 370a 525f  6419017201067.R_
+00000ed0: 656e 7620 2020 2020 2020 302e 3031 3238  env       0.0128
+00000ee0: 3838 3539 3035 3437 3132 3938 3035 0a52  88590547129805.R
+00000ef0: 5f74 6f74 616c 2020 2020 2020 2030 2e32  _total       0.2
+00000f00: 3030 3935 3836 3739 3631 3733 3736 3335  0095867961737635
+00000f10: 0a0a 6060 600a 0a0a 0a23 2320 4f74 6865  ..```....## Othe
+00000f20: 720a 0a54 2d4d 6172 7420 6361 6e20 6361  r..T-Mart can ca
+00000f30: 6c63 756c 6174 6520 7265 666c 6563 7461  lculate reflecta
+00000f40: 6e63 6573 206f 6620 7661 7269 6f75 7320  nces of various 
+00000f50: 756e 6974 732c 2073 6565 2054 6162 6c65  units, see Table
+00000f60: 2031 2069 6e20 5775 2065 7420 616c 2e20   1 in Wu et al. 
+00000f70: 2832 3032 3329 2e20 0a0a 466f 7220 7175  (2023). ..For qu
+00000f80: 6573 7469 6f6e 7320 616e 6420 7375 6767  estions and sugg
+00000f90: 6573 7469 6f6e 7320 2877 6869 6368 2049  estions (which I
+00000fa0: 276d 2061 6c77 6179 7320 6f70 656e 2074  'm always open t
+00000fb0: 6f21 292c 2070 6c65 6173 6520 656d 6169  o!), please emai
+00000fc0: 6c20 5975 6c75 6e20 6174 205b 7975 6c75  l Yulun at [yulu
+00000fd0: 6e77 7538 4067 6d61 696c 2e63 6f6d 5d28  nwu8@gmail.com](
+00000fe0: 6d61 696c 746f 3a79 756c 756e 7775 3840  mailto:yulunwu8@
+00000ff0: 676d 6169 6c2e 636f 6d29 0a0a            gmail.com)..
```

### Comparing `tmart-1.3.5/README.md` & `tmart-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -122,84 +122,96 @@
 00000790: 6553 756d 6d65 7229 200a 6165 726f 736f  eSummer) .aeroso
 000007a0: 6c5f 7479 7065 203d 2027 4d61 7269 7469  l_type = 'Mariti
 000007b0: 6d65 2720 200a 6d79 5f61 746d 203d 2074  me'  .my_atm = t
 000007c0: 6d61 7274 2e41 746d 6f73 7068 6572 6528  mart.Atmosphere(
 000007d0: 6174 6d5f 7072 6f66 696c 652c 2061 6f74  atm_profile, aot
 000007e0: 3535 3020 3d20 302c 2061 6572 6f73 6f6c  550 = 0, aerosol
 000007f0: 5f74 7970 6520 3d20 274d 6172 6974 696d  _type = 'Maritim
-00000800: 6527 2020 290a 0a23 2323 2052 756e 6e69  e'  )..### Runni
-00000810: 6e67 2054 2d4d 6172 7420 2323 230a 6d79  ng T-Mart ###.my
-00000820: 5f74 6d61 7274 203d 2074 6d61 7274 2e54  _tmart = tmart.T
-00000830: 6d61 7274 2853 7572 6661 6365 203d 206d  mart(Surface = m
-00000840: 795f 7375 7266 6163 652c 2041 746d 6f73  y_surface, Atmos
-00000850: 7068 6572 653d 206d 795f 6174 6d2c 2073  phere= my_atm, s
-00000860: 6861 646f 773d 4661 6c73 6529 0a6d 795f  hadow=False).my_
-00000870: 746d 6172 742e 7365 745f 6765 6f6d 6574  tmart.set_geomet
-00000880: 7279 2873 656e 736f 725f 636f 6f72 6473  ry(sensor_coords
-00000890: 3d5b 3531 2c35 302c 3133 305f 3030 305d  =[51,50,130_000]
-000008a0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-000008b0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-000008c0: 7074 5f64 6972 6563 7469 6f6e 3d5b 3138  pt_direction=[18
-000008d0: 302c 305d 2c0a 2020 2020 2020 2020 2020  0,0],.          
-000008e0: 2020 2020 2020 2020 2020 2020 7375 6e5f              sun_
-000008f0: 6469 723d 5b30 2c30 5d29 0a0a 7265 7375  dir=[0,0])..resu
-00000900: 6c74 7320 3d20 6d79 5f74 6d61 7274 2e72  lts = my_tmart.r
-00000910: 756e 2877 6c3d 776c 2c20 6261 6e64 3d4e  un(wl=wl, band=N
-00000920: 6f6e 652c 206e 5f70 686f 746f 6e3d 3130  one, n_photon=10
-00000930: 5f30 3030 290a 0a23 2043 616c 6375 6c61  _000)..# Calcula
-00000940: 7465 2072 6566 6c65 6374 616e 6365 7320  te reflectances 
-00000950: 7573 696e 6720 7265 636f 7264 6564 2070  using recorded p
-00000960: 686f 746f 6e20 696e 666f 726d 6174 696f  hoton informatio
-00000970: 6e20 0a52 203d 2074 6d61 7274 2e63 616c  n .R = tmart.cal
-00000980: 635f 7265 6628 7265 7375 6c74 7329 0a66  c_ref(results).f
-00000990: 6f72 206b 2c20 7620 696e 2052 2e69 7465  or k, v in R.ite
-000009a0: 6d73 2829 3a0a 2020 2020 7072 696e 7428  ms():.    print(
-000009b0: 6b2c 2027 2020 2020 2027 202c 2076 290a  k, '     ' , v).
-000009c0: 0a60 6060 0a0a 4f75 7470 7574 2073 686f  .```..Output sho
-000009d0: 756c 6420 6265 2073 696d 696c 6172 2074  uld be similar t
-000009e0: 6f20 7468 6973 3a20 0a0a 6060 600a 3d3d  o this: ..```.==
-000009f0: 3d3d 3d3d 3d3d 3d20 496e 6974 6961 7469  ======= Initiati
-00000a00: 6e67 2054 2d4d 6172 7420 3d3d 3d3d 3d3d  ng T-Mart ======
-00000a10: 3d3d 3d0a 4e75 6d62 6572 206f 6620 7068  ===.Number of ph
-00000a20: 6f74 6f6e 733a 2031 3030 3030 0a55 7369  otons: 10000.Usi
-00000a30: 6e67 2031 3020 636f 7265 2873 290a 4e75  ng 10 core(s).Nu
-00000a40: 6d62 6572 206f 6620 6a6f 6228 7329 3a20  mber of job(s): 
-00000a50: 3130 300a 5761 7665 6c65 6e67 7468 3a20  100.Wavelength: 
-00000a60: 3430 300a 7461 7267 6574 5f70 745f 6469  400.target_pt_di
-00000a70: 7265 6374 696f 6e3a 205b 3138 302c 2030  rection: [180, 0
-00000a80: 5d0a 7375 6e5f 6469 723a 205b 302c 2030  ].sun_dir: [0, 0
-00000a90: 5d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ].==============
-00000aa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000ab0: 3d3d 3d3d 3d3d 3d0a 5461 736b 7320 7265  =======.Tasks re
-00000ac0: 6d61 696e 696e 6720 3d20 3130 320a 5461  maining = 102.Ta
-00000ad0: 736b 7320 7265 6d61 696e 696e 6720 3d20  sks remaining = 
-00000ae0: 3732 0a54 6173 6b73 2072 656d 6169 6e69  72.Tasks remaini
-00000af0: 6e67 203d 2034 320a 5461 736b 7320 7265  ng = 42.Tasks re
-00000b00: 6d61 696e 696e 6720 3d20 3132 0a3d 3d3d  maining = 12.===
-00000b10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000b20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000b30: 3d3d 0a43 616c 6375 6c61 7469 6e67 2072  ==.Calculating r
-00000b40: 6164 6961 7469 7665 2070 726f 7065 7274  adiative propert
-00000b50: 6965 732e 2e2e 0a52 5f61 746d 2020 2020  ies....R_atm    
-00000b60: 2020 2030 2e31 3237 3630 3538 3938 3839     0.12760589889
-00000b70: 3832 3335 3837 0a52 5f64 6972 2020 2020  823587.R_dir    
-00000b80: 2020 2030 2e30 3630 3436 3431 3930 3137     0.06046419017
-00000b90: 3230 3130 3637 0a52 5f65 6e76 2020 2020  201067.R_env    
-00000ba0: 2020 2030 2e30 3132 3838 3835 3930 3534     0.01288859054
-00000bb0: 3731 3239 3830 350a 525f 746f 7461 6c20  7129805.R_total 
-00000bc0: 2020 2020 2020 302e 3230 3039 3538 3637        0.20095867
-00000bd0: 3936 3137 3337 3633 350a 0a60 6060 0a0a  961737635..```..
-00000be0: 0a0a 2323 204f 7468 6572 0a0a 542d 4d61  ..## Other..T-Ma
-00000bf0: 7274 2063 616e 2063 616c 6375 6c61 7465  rt can calculate
-00000c00: 2072 6566 6c65 6374 616e 6365 7320 6f66   reflectances of
-00000c10: 2076 6172 696f 7573 2075 6e69 7473 2c20   various units, 
-00000c20: 7365 6520 5461 626c 6520 3120 696e 2057  see Table 1 in W
-00000c30: 7520 6574 2061 6c2e 2028 3230 3233 292e  u et al. (2023).
-00000c40: 200a 0a46 6f72 2071 7565 7374 696f 6e73   ..For questions
-00000c50: 2061 6e64 2073 7567 6765 7374 696f 6e73   and suggestions
-00000c60: 2028 7768 6963 6820 4927 6d20 616c 7761   (which I'm alwa
-00000c70: 7973 206f 7065 6e20 746f 2129 2c20 706c  ys open to!), pl
-00000c80: 6561 7365 2065 6d61 696c 2059 756c 756e  ease email Yulun
-00000c90: 2061 7420 5b79 756c 756e 7775 3840 676d   at [yulunwu8@gm
-00000ca0: 6169 6c2e 636f 6d5d 286d 6169 6c74 6f3a  ail.com](mailto:
-00000cb0: 7975 6c75 6e77 7538 4067 6d61 696c 2e63  yulunwu8@gmail.c
-00000cc0: 6f6d 290a 0a                             om)..
+00000800: 6527 2020 290a 0a23 2323 2043 7265 6174  e'  )..### Creat
+00000810: 6520 542d 4d61 7274 204f 626a 6563 7420  e T-Mart Object 
+00000820: 2323 230a 6d79 5f74 6d61 7274 203d 2074  ###.my_tmart = t
+00000830: 6d61 7274 2e54 6d61 7274 2853 7572 6661  mart.Tmart(Surfa
+00000840: 6365 203d 206d 795f 7375 7266 6163 652c  ce = my_surface,
+00000850: 2041 746d 6f73 7068 6572 653d 206d 795f   Atmosphere= my_
+00000860: 6174 6d2c 2073 6861 646f 773d 4661 6c73  atm, shadow=Fals
+00000870: 6529 0a6d 795f 746d 6172 742e 7365 745f  e).my_tmart.set_
+00000880: 6765 6f6d 6574 7279 2873 656e 736f 725f  geometry(sensor_
+00000890: 636f 6f72 6473 3d5b 3531 2c35 302c 3133  coords=[51,50,13
+000008a0: 305f 3030 305d 2c20 0a20 2020 2020 2020  0_000], .       
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000008c0: 6172 6765 745f 7074 5f64 6972 6563 7469  arget_pt_directi
+000008d0: 6f6e 3d5b 3138 302c 305d 2c0a 2020 2020  on=[180,0],.    
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 7375 6e5f 6469 723d 5b30 2c30 5d29    sun_dir=[0,0])
+00000900: 0a0a 2323 2320 4d75 6c74 6970 726f 6365  ..### Multiproce
+00000910: 7373 696e 6720 6e65 6564 7320 746f 2062  ssing needs to b
+00000920: 6520 7772 6170 7065 6420 696e 2027 6966  e wrapped in 'if
+00000930: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00000940: 6d61 696e 5f5f 223a 2720 666f 7220 5769  main__":' for Wi
+00000950: 6e64 6f77 7320 7379 7374 656d 732e 200a  ndows systems. .
+00000960: 2323 2320 5468 6973 2063 616e 2062 6520  ### This can be 
+00000970: 6967 6e6f 7265 6420 666f 7220 4c69 6e75  ignored for Linu
+00000980: 782d 6261 7365 6420 7379 7374 656d 732e  x-based systems.
+00000990: 200a 6966 205f 5f6e 616d 655f 5f20 3d3d   .if __name__ ==
+000009a0: 2022 5f5f 6d61 696e 5f5f 223a 0a20 2020   "__main__":.   
+000009b0: 2072 6573 756c 7473 203d 206d 795f 746d   results = my_tm
+000009c0: 6172 742e 7275 6e28 776c 3d77 6c2c 2062  art.run(wl=wl, b
+000009d0: 616e 643d 4e6f 6e65 2c20 6e5f 7068 6f74  and=None, n_phot
+000009e0: 6f6e 3d31 305f 3030 3029 0a20 2020 200a  on=10_000).    .
+000009f0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+00000a00: 7265 666c 6563 7461 6e63 6573 2075 7369  reflectances usi
+00000a10: 6e67 2072 6563 6f72 6465 6420 7068 6f74  ng recorded phot
+00000a20: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 200a  on information .
+00000a30: 2020 2020 5220 3d20 746d 6172 742e 6361      R = tmart.ca
+00000a40: 6c63 5f72 6566 2872 6573 756c 7473 290a  lc_ref(results).
+00000a50: 2020 2020 666f 7220 6b2c 2076 2069 6e20      for k, v in 
+00000a60: 522e 6974 656d 7328 293a 0a20 2020 2020  R.items():.     
+00000a70: 2020 2070 7269 6e74 286b 2c20 2720 2020     print(k, '   
+00000a80: 2020 2720 2c20 7629 0a0a 6060 600a 0a4f    ' , v)..```..O
+00000a90: 7574 7075 7420 7368 6f75 6c64 2062 6520  utput should be 
+00000aa0: 7369 6d69 6c61 7220 746f 2074 6869 733a  similar to this:
+00000ab0: 200a 0a60 6060 0a3d 3d3d 3d3d 3d3d 3d3d   ..```.=========
+00000ac0: 2049 6e69 7469 6174 696e 6720 542d 4d61   Initiating T-Ma
+00000ad0: 7274 203d 3d3d 3d3d 3d3d 3d3d 0a4e 756d  rt =========.Num
+00000ae0: 6265 7220 6f66 2070 686f 746f 6e73 3a20  ber of photons: 
+00000af0: 3130 3030 300a 5573 696e 6720 3130 2063  10000.Using 10 c
+00000b00: 6f72 6528 7329 0a4e 756d 6265 7220 6f66  ore(s).Number of
+00000b10: 206a 6f62 2873 293a 2031 3030 0a57 6176   job(s): 100.Wav
+00000b20: 656c 656e 6774 683a 2034 3030 0a74 6172  elength: 400.tar
+00000b30: 6765 745f 7074 5f64 6972 6563 7469 6f6e  get_pt_direction
+00000b40: 3a20 5b31 3830 2c20 305d 0a73 756e 5f64  : [180, 0].sun_d
+00000b50: 6972 3a20 5b30 2c20 305d 0a3d 3d3d 3d3d  ir: [0, 0].=====
+00000b60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000b70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000b80: 0a54 6173 6b73 2072 656d 6169 6e69 6e67  .Tasks remaining
+00000b90: 203d 2031 3032 0a54 6173 6b73 2072 656d   = 102.Tasks rem
+00000ba0: 6169 6e69 6e67 203d 2037 320a 5461 736b  aining = 72.Task
+00000bb0: 7320 7265 6d61 696e 696e 6720 3d20 3432  s remaining = 42
+00000bc0: 0a54 6173 6b73 2072 656d 6169 6e69 6e67  .Tasks remaining
+00000bd0: 203d 2031 320a 3d3d 3d3d 3d3d 3d3d 3d3d   = 12.==========
+00000be0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000bf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 4361 6c63  ===========.Calc
+00000c00: 756c 6174 696e 6720 7261 6469 6174 6976  ulating radiativ
+00000c10: 6520 7072 6f70 6572 7469 6573 2e2e 2e0a  e properties....
+00000c20: 525f 6174 6d20 2020 2020 2020 302e 3132  R_atm       0.12
+00000c30: 3736 3035 3839 3838 3938 3233 3538 370a  760589889823587.
+00000c40: 525f 6469 7220 2020 2020 2020 302e 3036  R_dir       0.06
+00000c50: 3034 3634 3139 3031 3732 3031 3036 370a  046419017201067.
+00000c60: 525f 656e 7620 2020 2020 2020 302e 3031  R_env       0.01
+00000c70: 3238 3838 3539 3035 3437 3132 3938 3035  2888590547129805
+00000c80: 0a52 5f74 6f74 616c 2020 2020 2020 2030  .R_total       0
+00000c90: 2e32 3030 3935 3836 3739 3631 3733 3736  .200958679617376
+00000ca0: 3335 0a0a 6060 600a 0a0a 0a23 2320 4f74  35..```....## Ot
+00000cb0: 6865 720a 0a54 2d4d 6172 7420 6361 6e20  her..T-Mart can 
+00000cc0: 6361 6c63 756c 6174 6520 7265 666c 6563  calculate reflec
+00000cd0: 7461 6e63 6573 206f 6620 7661 7269 6f75  tances of variou
+00000ce0: 7320 756e 6974 732c 2073 6565 2054 6162  s units, see Tab
+00000cf0: 6c65 2031 2069 6e20 5775 2065 7420 616c  le 1 in Wu et al
+00000d00: 2e20 2832 3032 3329 2e20 0a0a 466f 7220  . (2023). ..For 
+00000d10: 7175 6573 7469 6f6e 7320 616e 6420 7375  questions and su
+00000d20: 6767 6573 7469 6f6e 7320 2877 6869 6368  ggestions (which
+00000d30: 2049 276d 2061 6c77 6179 7320 6f70 656e   I'm always open
+00000d40: 2074 6f21 292c 2070 6c65 6173 6520 656d   to!), please em
+00000d50: 6169 6c20 5975 6c75 6e20 6174 205b 7975  ail Yulun at [yu
+00000d60: 6c75 6e77 7538 4067 6d61 696c 2e63 6f6d  lunwu8@gmail.com
+00000d70: 5d28 6d61 696c 746f 3a79 756c 756e 7775  ](mailto:yulunwu
+00000d80: 3840 676d 6169 6c2e 636f 6d29 0a0a       8@gmail.com)..
```

### Comparing `tmart-1.3.5/setup.py` & `tmart-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="1.3.5",                       
+    version="1.3.6",                       
     author="Yulun Wu",                     # Full name of the author
     description="Radiative transfer modelling for aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
-    packages = ['tmart','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF'],
+    packages = ['tmart','tmart.surface_rho','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF'],
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3",
```

### Comparing `tmart-1.3.5/tests/test_E_diffuse.py` & `tmart-1.3.6/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_L_sky.py` & `tmart-1.3.6/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_basic.py` & `tmart-1.3.6/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_basic_import.py` & `tmart-1.3.6/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_calcref.py` & `tmart-1.3.6/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_quickstart.py` & `tmart-1.3.6/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_specular_contribution.py` & `tmart-1.3.6/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_typical_ocean.py` & `tmart-1.3.6/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tests/test_whales_SR.py` & `tmart-1.3.6/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/AEC/get_parameters.py` & `tmart-1.3.6/tmart/AEC/get_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
 # Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.5/tmart/AEC/read_PRISMA_north.py` & `tmart-1.3.6/tmart/AEC/read_PRISMA_north.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
 # Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -10,50 +10,36 @@
 
 ### read PRSIMA north
 
 
 def read_PRISMA_north(file): 
     # assume PRISMA images are 1000x1000
 
-    
     import pyproj
     import netCDF4 as nc4
     
-    # file = '/Volumes/San/ACIX_S2_AC/test_image/test_Ottawa/S2A_MSI_2022_07_09_16_00_51_T18TVR_L1R.nc'
-        
-    # file = '/Users/yw/Local_storage/221220_ACIX/Wendtorf_ACOLITE/PRISMA_2022_08_31_10_28_15_L1R.nc'
-    
-    
     with nc4.Dataset(file, 'r')  as dset:
     
         a_lat = dset['lat'][:]
         a_lon = dset['lon'][:]
         
         # image = dset['rhot_505'][:]
     
-        
     # lat lon
     top_left = [a_lat[0,0],a_lon[0,0]]
     top_right = [a_lat[0,999],a_lon[0,999]]
     bot_left = [a_lat[999,0],a_lon[999,0]]
     bot_right = [a_lat[999,999],a_lon[999,999]]
     
-    
-    
     geodesic = pyproj.Geod(ellps='WGS84')
     
-    
     up_left,__,__ = geodesic.inv(bot_left[1], bot_left[0], top_left[1], top_left[0])
-    
     # print(up_left)
     
-    
-    
     up_right,__,__ = geodesic.inv(bot_right[1], bot_right[0], top_right[1], top_right[0])
-    
     # print(up_right)
     
     return (up_left + up_right) / 2
```

### Comparing `tmart-1.3.5/tmart/AEC/read_PRISMA_vaa.py` & `tmart-1.3.6/tmart/AEC/read_PRISMA_vaa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
 # Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,15 +12,15 @@
 
 
 def read_PRISMA_vaa(file):
     
     import h5py
     import numpy as np
 
-    
+    # From Dr. Claudia Giardino, giardino.c@irea.cnr.it
     def view_angles(xPos, yPos, zPos, lon , lat , h=0):
         phiRad = lat * np.pi / 180;
         lamRad = lon * np.pi / 180;
 
         a_ax = 6378137.
         b_ax = 6356752.314205;
         e2 = 1 - (np.power(b_ax, 2) / np.power(a_ax, 2));
@@ -87,19 +87,8 @@
 
 
 
 
 
 
 
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `tmart-1.3.5/tmart/AEC/reflectance_correction.py` & `tmart-1.3.6/tmart/AEC/reflectance_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
 # Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.5/tmart/Aerosol.py` & `tmart-1.3.6/tmart/Aerosol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
-
-
 # Aerosol SPF
 
 import numpy as np
 import pandas as pd
 import os.path
 
 def find_aerosolSPF(aerosol_type,wl):
```

### Comparing `tmart-1.3.5/tmart/Atmosphere.py` & `tmart-1.3.6/tmart/Atmosphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
-
-
 # Atmosphere object  
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 
 import Py6S
```

### Comparing `tmart-1.3.5/tmart/Surface.py` & `tmart-1.3.6/tmart/Surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
+
 # Surface object
 
 import numpy as np
 import pandas as pd
 
 from scipy.interpolate import interp1d
```

### Comparing `tmart-1.3.5/tmart/Tmart.py` & `tmart-1.3.6/tmart/Tmart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
-
-
-
 # Replacing tmart_class
 
 # TMart: Topography-adjusted Monte-Carlo Adjacency-effect Radiative Transfer code
 
 from multiprocessing import cpu_count
 from pathos.multiprocessing import ProcessingPool
 import numpy as np
```

### Comparing `tmart-1.3.5/tmart/Tmart2.py` & `tmart-1.3.6/tmart/Tmart2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
 
-
-
 # Replacing tm
-
 # function as second page 
-
 # Overall control of photon movement
 
 
-
-
-
-
 # T-MART: Topography-adjusted Monte-Carlo Adjacency-effect Radiative Transfer code  
 
 
 import sys
 import numpy as np
 import pandas as pd
 import random
```

### Comparing `tmart-1.3.5/tmart/__init__.py` & `tmart-1.3.6/tmart/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
-
-
 from .Surface import Surface, SpectralSurface
 from .Atmosphere import Atmosphere
 
 from .Tmart import Tmart
 
 from .tm_calcref import calc_ref 
 from .tm_geometry import dirP_to_coord
 
 from tmart import AEC
-
+from tmart import surface_rho
```

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-1.3.6/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/conifer_forest.csv` & `tmart-1.3.6/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/dry_beach_sand.csv` & `tmart-1.3.6/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/lawn_grass.csv` & `tmart-1.3.6/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/soil.csv` & `tmart-1.3.6/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/vegetation.csv` & `tmart-1.3.6/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/water_chl1.csv` & `tmart-1.3.6/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/ancillary/wet_beach_sand.csv` & `tmart-1.3.6/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.5/tmart/tm_OT.py` & `tmart-1.3.6/tmart/tm_OT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
-
-
-
-
 import numpy as np
 
 # Calculate the absorption optical thickness between two points 
 def find_OT(q0,q1,atm_profile):
  
     topP = max(q0[2],q1[2])
     bottomP = min(q0[2],q1[2])
```

### Comparing `tmart-1.3.5/tmart/tm_calcref.py` & `tmart-1.3.6/tmart/tm_calcref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
 
-
-
-
 # Analyze the output of TMart and differentiate direct, env and atm intrinsic reflectances  
 
 import numpy as np 
 import pandas as pd
 import sys
 from copy import copy
```

### Comparing `tmart-1.3.5/tmart/tm_geometry.py` & `tmart-1.3.6/tmart/tm_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
+
+
 # Geometry 
 
 
 import math
 import numpy as np
 import sys
```

### Comparing `tmart-1.3.5/tmart/tm_intersect.py` & `tmart-1.3.6/tmart/tm_intersect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
+
 # intersect
 
 
 import pandas as pd
 import numpy as np
 import sys
```

### Comparing `tmart-1.3.5/tmart/tm_move.py` & `tmart-1.3.6/tmart/tm_move.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
-
-
-
-
-
 # Photon movement
 
 
 import numpy as np
 import math
 import sys
```

### Comparing `tmart-1.3.5/tmart/tm_sampling.py` & `tmart-1.3.6/tmart/tm_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
-
-
-
 # Sampling 
 
 import random
 import math
 import numpy as np
 
 from .tm_geometry import dirP_to_coord, rotation_matrix, dirC_to_dirP
```

### Comparing `tmart-1.3.5/tmart/tm_water.py` & `tmart-1.3.6/tmart/tm_water.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# This file is part of TMart.
+# This file is part of T-Mart.
 #
-# Copyright 2022 Yulun Wu.
+# Copyright 2023 Yulun Wu.
 #
 # T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
 
 
-
-
-
 # Water 
 
 import random
 import math
 import numpy as np
 import pandas as pd
```

### Comparing `tmart-1.3.5/tmart.egg-info/PKG-INFO` & `tmart-1.3.6/tmart.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 746d 6172  : 2.1.Name: tmar
-00000020: 740a 5665 7273 696f 6e3a 2031 2e33 2e35  t.Version: 1.3.5
+00000020: 740a 5665 7273 696f 6e3a 2031 2e33 2e36  t.Version: 1.3.6
 00000030: 0a53 756d 6d61 7279 3a20 5261 6469 6174  .Summary: Radiat
 00000040: 6976 6520 7472 616e 7366 6572 206d 6f64  ive transfer mod
 00000050: 656c 6c69 6e67 2066 6f72 2061 7175 6174  elling for aquat
 00000060: 6963 2072 656d 6f74 6520 7365 6e73 696e  ic remote sensin
 00000070: 670a 4175 7468 6f72 3a20 5975 6c75 6e20  g.Author: Yulun 
 00000080: 5775 0a43 6c61 7373 6966 6965 723a 2049  Wu.Classifier: I
 00000090: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
@@ -161,84 +161,96 @@
 00000a00: 756d 6d65 7229 200a 6165 726f 736f 6c5f  ummer) .aerosol_
 00000a10: 7479 7065 203d 2027 4d61 7269 7469 6d65  type = 'Maritime
 00000a20: 2720 200a 6d79 5f61 746d 203d 2074 6d61  '  .my_atm = tma
 00000a30: 7274 2e41 746d 6f73 7068 6572 6528 6174  rt.Atmosphere(at
 00000a40: 6d5f 7072 6f66 696c 652c 2061 6f74 3535  m_profile, aot55
 00000a50: 3020 3d20 302c 2061 6572 6f73 6f6c 5f74  0 = 0, aerosol_t
 00000a60: 7970 6520 3d20 274d 6172 6974 696d 6527  ype = 'Maritime'
-00000a70: 2020 290a 0a23 2323 2052 756e 6e69 6e67    )..### Running
-00000a80: 2054 2d4d 6172 7420 2323 230a 6d79 5f74   T-Mart ###.my_t
-00000a90: 6d61 7274 203d 2074 6d61 7274 2e54 6d61  mart = tmart.Tma
-00000aa0: 7274 2853 7572 6661 6365 203d 206d 795f  rt(Surface = my_
-00000ab0: 7375 7266 6163 652c 2041 746d 6f73 7068  surface, Atmosph
-00000ac0: 6572 653d 206d 795f 6174 6d2c 2073 6861  ere= my_atm, sha
-00000ad0: 646f 773d 4661 6c73 6529 0a6d 795f 746d  dow=False).my_tm
-00000ae0: 6172 742e 7365 745f 6765 6f6d 6574 7279  art.set_geometry
-00000af0: 2873 656e 736f 725f 636f 6f72 6473 3d5b  (sensor_coords=[
-00000b00: 3531 2c35 302c 3133 305f 3030 305d 2c20  51,50,130_000], 
-00000b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b20: 2020 2020 2020 2074 6172 6765 745f 7074         target_pt
-00000b30: 5f64 6972 6563 7469 6f6e 3d5b 3138 302c  _direction=[180,
-00000b40: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
-00000b50: 2020 2020 2020 2020 2020 7375 6e5f 6469            sun_di
-00000b60: 723d 5b30 2c30 5d29 0a0a 7265 7375 6c74  r=[0,0])..result
-00000b70: 7320 3d20 6d79 5f74 6d61 7274 2e72 756e  s = my_tmart.run
-00000b80: 2877 6c3d 776c 2c20 6261 6e64 3d4e 6f6e  (wl=wl, band=Non
-00000b90: 652c 206e 5f70 686f 746f 6e3d 3130 5f30  e, n_photon=10_0
-00000ba0: 3030 290a 0a23 2043 616c 6375 6c61 7465  00)..# Calculate
-00000bb0: 2072 6566 6c65 6374 616e 6365 7320 7573   reflectances us
-00000bc0: 696e 6720 7265 636f 7264 6564 2070 686f  ing recorded pho
-00000bd0: 746f 6e20 696e 666f 726d 6174 696f 6e20  ton information 
-00000be0: 0a52 203d 2074 6d61 7274 2e63 616c 635f  .R = tmart.calc_
-00000bf0: 7265 6628 7265 7375 6c74 7329 0a66 6f72  ref(results).for
-00000c00: 206b 2c20 7620 696e 2052 2e69 7465 6d73   k, v in R.items
-00000c10: 2829 3a0a 2020 2020 7072 696e 7428 6b2c  ():.    print(k,
-00000c20: 2027 2020 2020 2027 202c 2076 290a 0a60   '     ' , v)..`
-00000c30: 6060 0a0a 4f75 7470 7574 2073 686f 756c  ``..Output shoul
-00000c40: 6420 6265 2073 696d 696c 6172 2074 6f20  d be similar to 
-00000c50: 7468 6973 3a20 0a0a 6060 600a 3d3d 3d3d  this: ..```.====
-00000c60: 3d3d 3d3d 3d20 496e 6974 6961 7469 6e67  ===== Initiating
-00000c70: 2054 2d4d 6172 7420 3d3d 3d3d 3d3d 3d3d   T-Mart ========
-00000c80: 3d0a 4e75 6d62 6572 206f 6620 7068 6f74  =.Number of phot
-00000c90: 6f6e 733a 2031 3030 3030 0a55 7369 6e67  ons: 10000.Using
-00000ca0: 2031 3020 636f 7265 2873 290a 4e75 6d62   10 core(s).Numb
-00000cb0: 6572 206f 6620 6a6f 6228 7329 3a20 3130  er of job(s): 10
-00000cc0: 300a 5761 7665 6c65 6e67 7468 3a20 3430  0.Wavelength: 40
-00000cd0: 300a 7461 7267 6574 5f70 745f 6469 7265  0.target_pt_dire
-00000ce0: 6374 696f 6e3a 205b 3138 302c 2030 5d0a  ction: [180, 0].
-00000cf0: 7375 6e5f 6469 723a 205b 302c 2030 5d0a  sun_dir: [0, 0].
-00000d00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d20: 3d3d 3d3d 3d0a 5461 736b 7320 7265 6d61  =====.Tasks rema
-00000d30: 696e 696e 6720 3d20 3130 320a 5461 736b  ining = 102.Task
-00000d40: 7320 7265 6d61 696e 696e 6720 3d20 3732  s remaining = 72
-00000d50: 0a54 6173 6b73 2072 656d 6169 6e69 6e67  .Tasks remaining
-00000d60: 203d 2034 320a 5461 736b 7320 7265 6d61   = 42.Tasks rema
-00000d70: 696e 696e 6720 3d20 3132 0a3d 3d3d 3d3d  ining = 12.=====
-00000d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000da0: 0a43 616c 6375 6c61 7469 6e67 2072 6164  .Calculating rad
-00000db0: 6961 7469 7665 2070 726f 7065 7274 6965  iative propertie
-00000dc0: 732e 2e2e 0a52 5f61 746d 2020 2020 2020  s....R_atm      
-00000dd0: 2030 2e31 3237 3630 3538 3938 3839 3832   0.1276058988982
-00000de0: 3335 3837 0a52 5f64 6972 2020 2020 2020  3587.R_dir      
-00000df0: 2030 2e30 3630 3436 3431 3930 3137 3230   0.0604641901720
-00000e00: 3130 3637 0a52 5f65 6e76 2020 2020 2020  1067.R_env      
-00000e10: 2030 2e30 3132 3838 3835 3930 3534 3731   0.0128885905471
-00000e20: 3239 3830 350a 525f 746f 7461 6c20 2020  29805.R_total   
-00000e30: 2020 2020 302e 3230 3039 3538 3637 3936      0.2009586796
-00000e40: 3137 3337 3633 350a 0a60 6060 0a0a 0a0a  1737635..```....
-00000e50: 2323 204f 7468 6572 0a0a 542d 4d61 7274  ## Other..T-Mart
-00000e60: 2063 616e 2063 616c 6375 6c61 7465 2072   can calculate r
-00000e70: 6566 6c65 6374 616e 6365 7320 6f66 2076  eflectances of v
-00000e80: 6172 696f 7573 2075 6e69 7473 2c20 7365  arious units, se
-00000e90: 6520 5461 626c 6520 3120 696e 2057 7520  e Table 1 in Wu 
-00000ea0: 6574 2061 6c2e 2028 3230 3233 292e 200a  et al. (2023). .
-00000eb0: 0a46 6f72 2071 7565 7374 696f 6e73 2061  .For questions a
-00000ec0: 6e64 2073 7567 6765 7374 696f 6e73 2028  nd suggestions (
-00000ed0: 7768 6963 6820 4927 6d20 616c 7761 7973  which I'm always
-00000ee0: 206f 7065 6e20 746f 2129 2c20 706c 6561   open to!), plea
-00000ef0: 7365 2065 6d61 696c 2059 756c 756e 2061  se email Yulun a
-00000f00: 7420 5b79 756c 756e 7775 3840 676d 6169  t [yulunwu8@gmai
-00000f10: 6c2e 636f 6d5d 286d 6169 6c74 6f3a 7975  l.com](mailto:yu
-00000f20: 6c75 6e77 7538 4067 6d61 696c 2e63 6f6d  lunwu8@gmail.com
-00000f30: 290a 0a                                  )..
+00000a70: 2020 290a 0a23 2323 2043 7265 6174 6520    )..### Create 
+00000a80: 542d 4d61 7274 204f 626a 6563 7420 2323  T-Mart Object ##
+00000a90: 230a 6d79 5f74 6d61 7274 203d 2074 6d61  #.my_tmart = tma
+00000aa0: 7274 2e54 6d61 7274 2853 7572 6661 6365  rt.Tmart(Surface
+00000ab0: 203d 206d 795f 7375 7266 6163 652c 2041   = my_surface, A
+00000ac0: 746d 6f73 7068 6572 653d 206d 795f 6174  tmosphere= my_at
+00000ad0: 6d2c 2073 6861 646f 773d 4661 6c73 6529  m, shadow=False)
+00000ae0: 0a6d 795f 746d 6172 742e 7365 745f 6765  .my_tmart.set_ge
+00000af0: 6f6d 6574 7279 2873 656e 736f 725f 636f  ometry(sensor_co
+00000b00: 6f72 6473 3d5b 3531 2c35 302c 3133 305f  ords=[51,50,130_
+00000b10: 3030 305d 2c20 0a20 2020 2020 2020 2020  000], .         
+00000b20: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00000b30: 6765 745f 7074 5f64 6972 6563 7469 6f6e  get_pt_direction
+00000b40: 3d5b 3138 302c 305d 2c0a 2020 2020 2020  =[180,0],.      
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 7375 6e5f 6469 723d 5b30 2c30 5d29 0a0a  sun_dir=[0,0])..
+00000b70: 2323 2320 4d75 6c74 6970 726f 6365 7373  ### Multiprocess
+00000b80: 696e 6720 6e65 6564 7320 746f 2062 6520  ing needs to be 
+00000b90: 7772 6170 7065 6420 696e 2027 6966 205f  wrapped in 'if _
+00000ba0: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
+00000bb0: 696e 5f5f 223a 2720 666f 7220 5769 6e64  in__":' for Wind
+00000bc0: 6f77 7320 7379 7374 656d 732e 200a 2323  ows systems. .##
+00000bd0: 2320 5468 6973 2063 616e 2062 6520 6967  # This can be ig
+00000be0: 6e6f 7265 6420 666f 7220 4c69 6e75 782d  nored for Linux-
+00000bf0: 6261 7365 6420 7379 7374 656d 732e 200a  based systems. .
+00000c00: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+00000c10: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2072  __main__":.    r
+00000c20: 6573 756c 7473 203d 206d 795f 746d 6172  esults = my_tmar
+00000c30: 742e 7275 6e28 776c 3d77 6c2c 2062 616e  t.run(wl=wl, ban
+00000c40: 643d 4e6f 6e65 2c20 6e5f 7068 6f74 6f6e  d=None, n_photon
+00000c50: 3d31 305f 3030 3029 0a20 2020 200a 2020  =10_000).    .  
+00000c60: 2020 2320 4361 6c63 756c 6174 6520 7265    # Calculate re
+00000c70: 666c 6563 7461 6e63 6573 2075 7369 6e67  flectances using
+00000c80: 2072 6563 6f72 6465 6420 7068 6f74 6f6e   recorded photon
+00000c90: 2069 6e66 6f72 6d61 7469 6f6e 200a 2020   information .  
+00000ca0: 2020 5220 3d20 746d 6172 742e 6361 6c63    R = tmart.calc
+00000cb0: 5f72 6566 2872 6573 756c 7473 290a 2020  _ref(results).  
+00000cc0: 2020 666f 7220 6b2c 2076 2069 6e20 522e    for k, v in R.
+00000cd0: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00000ce0: 2070 7269 6e74 286b 2c20 2720 2020 2020   print(k, '     
+00000cf0: 2720 2c20 7629 0a0a 6060 600a 0a4f 7574  ' , v)..```..Out
+00000d00: 7075 7420 7368 6f75 6c64 2062 6520 7369  put should be si
+00000d10: 6d69 6c61 7220 746f 2074 6869 733a 200a  milar to this: .
+00000d20: 0a60 6060 0a3d 3d3d 3d3d 3d3d 3d3d 2049  .```.========= I
+00000d30: 6e69 7469 6174 696e 6720 542d 4d61 7274  nitiating T-Mart
+00000d40: 203d 3d3d 3d3d 3d3d 3d3d 0a4e 756d 6265   =========.Numbe
+00000d50: 7220 6f66 2070 686f 746f 6e73 3a20 3130  r of photons: 10
+00000d60: 3030 300a 5573 696e 6720 3130 2063 6f72  000.Using 10 cor
+00000d70: 6528 7329 0a4e 756d 6265 7220 6f66 206a  e(s).Number of j
+00000d80: 6f62 2873 293a 2031 3030 0a57 6176 656c  ob(s): 100.Wavel
+00000d90: 656e 6774 683a 2034 3030 0a74 6172 6765  ength: 400.targe
+00000da0: 745f 7074 5f64 6972 6563 7469 6f6e 3a20  t_pt_direction: 
+00000db0: 5b31 3830 2c20 305d 0a73 756e 5f64 6972  [180, 0].sun_dir
+00000dc0: 3a20 5b30 2c20 305d 0a3d 3d3d 3d3d 3d3d  : [0, 0].=======
+00000dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000de0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a54  ==============.T
+00000df0: 6173 6b73 2072 656d 6169 6e69 6e67 203d  asks remaining =
+00000e00: 2031 3032 0a54 6173 6b73 2072 656d 6169   102.Tasks remai
+00000e10: 6e69 6e67 203d 2037 320a 5461 736b 7320  ning = 72.Tasks 
+00000e20: 7265 6d61 696e 696e 6720 3d20 3432 0a54  remaining = 42.T
+00000e30: 6173 6b73 2072 656d 6169 6e69 6e67 203d  asks remaining =
+00000e40: 2031 320a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   12.============
+00000e50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000e60: 3d3d 3d3d 3d3d 3d3d 3d0a 4361 6c63 756c  =========.Calcul
+00000e70: 6174 696e 6720 7261 6469 6174 6976 6520  ating radiative 
+00000e80: 7072 6f70 6572 7469 6573 2e2e 2e0a 525f  properties....R_
+00000e90: 6174 6d20 2020 2020 2020 302e 3132 3736  atm       0.1276
+00000ea0: 3035 3839 3838 3938 3233 3538 370a 525f  0589889823587.R_
+00000eb0: 6469 7220 2020 2020 2020 302e 3036 3034  dir       0.0604
+00000ec0: 3634 3139 3031 3732 3031 3036 370a 525f  6419017201067.R_
+00000ed0: 656e 7620 2020 2020 2020 302e 3031 3238  env       0.0128
+00000ee0: 3838 3539 3035 3437 3132 3938 3035 0a52  88590547129805.R
+00000ef0: 5f74 6f74 616c 2020 2020 2020 2030 2e32  _total       0.2
+00000f00: 3030 3935 3836 3739 3631 3733 3736 3335  0095867961737635
+00000f10: 0a0a 6060 600a 0a0a 0a23 2320 4f74 6865  ..```....## Othe
+00000f20: 720a 0a54 2d4d 6172 7420 6361 6e20 6361  r..T-Mart can ca
+00000f30: 6c63 756c 6174 6520 7265 666c 6563 7461  lculate reflecta
+00000f40: 6e63 6573 206f 6620 7661 7269 6f75 7320  nces of various 
+00000f50: 756e 6974 732c 2073 6565 2054 6162 6c65  units, see Table
+00000f60: 2031 2069 6e20 5775 2065 7420 616c 2e20   1 in Wu et al. 
+00000f70: 2832 3032 3329 2e20 0a0a 466f 7220 7175  (2023). ..For qu
+00000f80: 6573 7469 6f6e 7320 616e 6420 7375 6767  estions and sugg
+00000f90: 6573 7469 6f6e 7320 2877 6869 6368 2049  estions (which I
+00000fa0: 276d 2061 6c77 6179 7320 6f70 656e 2074  'm always open t
+00000fb0: 6f21 292c 2070 6c65 6173 6520 656d 6169  o!), please emai
+00000fc0: 6c20 5975 6c75 6e20 6174 205b 7975 6c75  l Yulun at [yulu
+00000fd0: 6e77 7538 4067 6d61 696c 2e63 6f6d 5d28  nwu8@gmail.com](
+00000fe0: 6d61 696c 746f 3a79 756c 756e 7775 3840  mailto:yulunwu8@
+00000ff0: 676d 6169 6c2e 636f 6d29 0a0a            gmail.com)..
```

### Comparing `tmart-1.3.5/tmart.egg-info/SOURCES.txt` & `tmart-1.3.6/tmart.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 MANIFEST.in
 README.md
 setup.py
 tests/test_AEC.py
+tests/test_AE_modelling.py
 tests/test_E_diffuse.py
 tests/test_L_sky.py
 tests/test_basic.py
 tests/test_basic_import.py
+tests/test_calc_rho.py
 tests/test_calcref.py
+tests/test_plot.py
 tests/test_quickstart.py
 tests/test_specular_contribution.py
 tests/test_typical_ocean.py
 tests/test_whales_SR.py
 tmart/Aerosol.py
 tmart/Atmosphere.py
 tmart/Surface.py
@@ -44,8 +47,10 @@
 tmart/ancillary/wet_beach_sand.csv
 tmart/ancillary/whitecap_factor.csv
 tmart/ancillary/aerosolSPF/BiomassBurning.csv
 tmart/ancillary/aerosolSPF/Continental.csv
 tmart/ancillary/aerosolSPF/Desert.csv
 tmart/ancillary/aerosolSPF/Maritime.csv
 tmart/ancillary/aerosolSPF/Stratospheric.csv
-tmart/ancillary/aerosolSPF/Urban.csv
+tmart/ancillary/aerosolSPF/Urban.csv
+tmart/surface_rho/__init__.py
+tmart/surface_rho/calculate.py
```


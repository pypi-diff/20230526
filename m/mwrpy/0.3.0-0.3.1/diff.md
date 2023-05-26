# Comparing `tmp/mwrpy-0.3.0.tar.gz` & `tmp/mwrpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.3.0.tar", last modified: Thu May 25 10:22:43 2023, max compression
+gzip compressed data, was "mwrpy-0.3.1.tar", last modified: Fri May 26 08:48:21 2023, max compression
```

## Comparing `mwrpy-0.3.0.tar` & `mwrpy-0.3.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-25 10:22:33.000000 mwrpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 10:22:33.000000 mwrpy-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-25 10:22:43.312654 mwrpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-25 10:22:33.000000 mwrpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51810 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.308654 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)  1208422 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.308654 mwrpy-0.3.0/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/juelich/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/lindenberg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.312654 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/site_config/lindenberg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 10:22:33.000000 mwrpy-0.3.0/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:22:43.304654 mwrpy-0.3.0/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 10:22:43.000000 mwrpy-0.3.0/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-25 10:22:33.000000 mwrpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:22:43.312654 mwrpy-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.205765 mwrpy-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 08:48:11.000000 mwrpy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 08:48:11.000000 mwrpy-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-26 08:48:21.205765 mwrpy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-26 08:48:11.000000 mwrpy-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.177764 mwrpy-0.3.1/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.181764 mwrpy-0.3.1/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.185764 mwrpy-0.3.1/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.185764 mwrpy-0.3.1/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51810 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.185764 mwrpy-0.3.1/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.185764 mwrpy-0.3.1/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.189764 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)  1208422 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.193765 mwrpy-0.3.1/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.201765 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/juelich/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.201765 mwrpy-0.3.1/mwrpy/site_config/lindenberg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.205765 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/site_config/lindenberg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 08:48:11.000000 mwrpy-0.3.1/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:48:21.181764 mwrpy-0.3.1/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-26 08:48:21.000000 mwrpy-0.3.1/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-26 08:48:21.000000 mwrpy-0.3.1/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:48:21.000000 mwrpy-0.3.1/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 08:48:21.000000 mwrpy-0.3.1/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 08:48:21.000000 mwrpy-0.3.1/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-26 08:48:11.000000 mwrpy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:48:21.205765 mwrpy-0.3.1/setup.cfg
```

### Comparing `mwrpy-0.3.0/LICENSE` & `mwrpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/PKG-INFO` & `mwrpy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Author-email: University of Cologne <actris-ccres-mwr@uni-koeln.de>
 License: MIT License
         
         Copyright (c) 2021-2023 University of Cologne
         Copyright (c) 2023 Finnish Meteorological Institute
```

### Comparing `mwrpy-0.3.0/README.md` & `mwrpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/atmos.py` & `mwrpy-0.3.1/mwrpy/atmos.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/cli.py` & `mwrpy-0.3.1/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.3.1/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level1/met_quality_control.py` & `mwrpy-0.3.1/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level1/quality_control.py` & `mwrpy-0.3.1/mwrpy/level1/quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level1/rpg_bin.py` & `mwrpy-0.3.1/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.3.1/mwrpy/level1/write_lev1_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.3.1/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.3.1/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level2/lwp_offset.py` & `mwrpy-0.3.1/mwrpy/level2/lwp_offset.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.3.1/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/plots/generate_plots.py` & `mwrpy-0.3.1/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/plots/plot_meta.py` & `mwrpy-0.3.1/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/plots/plot_utils.py` & `mwrpy-0.3.1/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/process_mwrpy.py` & `mwrpy-0.3.1/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/rpg_mwr.py` & `mwrpy-0.3.1/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.3.1/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.3.1/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.3.1/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/juelich/config.yaml` & `mwrpy-0.3.1/mwrpy/site_config/juelich/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/site_config/lindenberg/config.yaml` & `mwrpy-0.3.1/mwrpy/site_config/lindenberg/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/mwrpy/utils.py` & `mwrpy-0.3.1/mwrpy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,17 +271,23 @@
     return f_list
 
 
 def read_yaml_config(site: str) -> tuple[dict, dict]:
     """Reads config yaml files."""
     dir_name = os.path.dirname(os.path.realpath(__file__))
     site_file = os.path.join(dir_name, "site_config", site, "config.yaml")
+    if not os.path.isfile(site_file):
+        raise NotImplementedError(f"Error: site config file {site_file} not found")
     with open(site_file, "r", encoding="utf8") as f:
         site_config = yaml.load(f, Loader=SafeLoader)
     inst_file = os.path.join(dir_name, "site_config", f"{site_config['type']}.yaml")
+    if not os.path.isfile(inst_file):
+        raise NotImplementedError(
+            f"Error: instrument config file {site_file} not found"
+        )
     with open(inst_file, "r", encoding="utf8") as f:
         inst_config = yaml.load(f, Loader=SafeLoader)
     inst_config["global_specs"].update(site_config["global_specs"])
     for name in inst_config["params"].keys():
         site_config["params"][name] = inst_config["params"][name]
 
     return inst_config["global_specs"], site_config["params"]
```

### Comparing `mwrpy-0.3.0/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.3.1/mwrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Author-email: University of Cologne <actris-ccres-mwr@uni-koeln.de>
 License: MIT License
         
         Copyright (c) 2021-2023 University of Cologne
         Copyright (c) 2023 Finnish Meteorological Institute
```

### Comparing `mwrpy-0.3.0/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.3.1/mwrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwrpy-0.3.0/pyproject.toml` & `mwrpy-0.3.1/pyproject.toml`

 * *Files identical despite different names*


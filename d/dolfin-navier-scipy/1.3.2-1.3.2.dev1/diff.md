# Comparing `tmp/dolfin_navier_scipy-1.3.2.tar.gz` & `tmp/dolfin_navier_scipy-1.3.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolfin_navier_scipy-1.3.2.tar", last modified: Fri May 26 11:58:53 2023, max compression
+gzip compressed data, was "dolfin_navier_scipy-1.3.2.dev1.tar", last modified: Fri May 26 11:58:10 2023, max compression
```

## Comparing `dolfin_navier_scipy-1.3.2.tar` & `dolfin_navier_scipy-1.3.2.dev1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.509266 dolfin_navier_scipy-1.3.2/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      580 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/.readthedocs.yml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      726 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/.zenodo.json
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      135 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/AUTHORS
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      171 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/CHANGELOG.md
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      522 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/CODE.yml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    16765 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/ChangeLog
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    35121 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/LICENSE.md
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3863 2023-05-26 11:58:53.509266 dolfin_navier_scipy-1.3.2/PKG-INFO
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3123 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2/README.md
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.497266 dolfin_navier_scipy-1.3.2/docs/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      444 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/docs/Code.rst
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     5651 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/docs/Makefile
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     8687 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/docs/conf.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      899 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/docs/index.rst
--rw-rw-r--   0 heiland   (1001) heiland   (1001)       52 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/docs/readthedocs-pip-requirements.txt
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.497266 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      345 2022-03-24 20:40:42.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/__init__.py
--rw-r--r--   0 heiland   (1001) heiland   (1001)     2364 2020-06-26 05:15:59.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/cache_simustates_utils.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    12747 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/data_output_utils.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    25779 2023-02-05 09:49:45.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/dolfin_to_sparrays.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    52740 2023-01-31 21:38:35.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/problem_setups.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3439 2023-02-13 05:26:25.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/residual_checks.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    60844 2023-05-23 10:50:02.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/stokes_navier_utils.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    22494 2023-03-17 10:38:52.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/time_int_utils.py
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.497266 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/
--rw-r--r--   0 heiland   (1001) heiland   (1001)     3863 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/PKG-INFO
--rw-r--r--   0 heiland   (1001) heiland   (1001)     2862 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/SOURCES.txt
--rw-r--r--   0 heiland   (1001) heiland   (1001)        1 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/dependency_links.txt
--rw-rw-r--   0 heiland   (1001) heiland   (1001)        1 2022-03-24 20:34:30.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/not-zip-safe
--rw-rw-r--   0 heiland   (1001) heiland   (1001)       46 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/pbr.json
--rw-r--r--   0 heiland   (1001) heiland   (1001)       53 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/requires.txt
--rw-r--r--   0 heiland   (1001) heiland   (1001)       20 2023-05-26 11:58:53.000000 dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/top_level.txt
--rw-rw-r--   0 heiland   (1001) heiland   (1001)       53 2022-03-28 14:30:04.000000 dolfin_navier_scipy-1.3.2/requirements.txt
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      717 2023-05-26 11:58:53.509266 dolfin_navier_scipy-1.3.2/setup.cfg
--rw-rw-r--   0 heiland   (1001) heiland   (1001)       76 2022-03-28 14:30:04.000000 dolfin_navier_scipy-1.3.2/setup.py
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.501266 dolfin_navier_scipy-1.3.2/tests/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)        0 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/__init__.py
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.501266 dolfin_navier_scipy-1.3.2/tests/deprecatedtests/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     7063 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/deprecatedtests/solve_nse_quadraticterm.py
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.501266 dolfin_navier_scipy-1.3.2/tests/lilchecks/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3067 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/check_evals.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2687 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/check_int_cylboundary.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     1128 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/checkdofmap.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      298 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/slicedatrange.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     1090 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/test_boundaries_poisson.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2781 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/lilchecks/test_penarobinbc_cyl.py
-drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:53.509266 dolfin_navier_scipy-1.3.2/tests/mesh/
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      592 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_geo_cntrlbc.json
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      560 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_geo_cntrlbc_rotcntrl.json
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   150127 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl1.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    24475 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl1_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   269677 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl2.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    42852 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl2_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    84641 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_0.xml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   127538 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_1.xml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   208003 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_2.xml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    34234 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_2.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   434276 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_3.xml
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   648509 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_4.xml
--rw-r--r--   0 heiland   (1001) heiland   (1001)      702 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_geo_cntrlbc.json
--rw-r--r--   0 heiland   (1001) heiland   (1001)   246966 2020-04-20 06:11:55.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl1.xml.gz
--rw-r--r--   0 heiland   (1001) heiland   (1001)    39919 2020-04-20 06:11:55.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl1_facet_region.xml.gz
--rw-r--r--   0 heiland   (1001) heiland   (1001)   303368 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl2.xml.gz
--rw-r--r--   0 heiland   (1001) heiland   (1001)    48673 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl2_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      483 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl-bm_geo_cntrlbc.json
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   126225 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl1.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    21007 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl1_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   225707 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl2.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    36861 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl2_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   320808 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl3.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)    51735 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl3_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   810649 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl4.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)   124932 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl4_facet_region.xml.gz
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     1356 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/mini_setup.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)      180 2023-03-13 03:16:04.000000 dolfin_navier_scipy-1.3.2/tests/start-generic-stst-sim.sh
--rwxrwxr-x   0 heiland   (1001) heiland   (1001)      454 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/start-generic-tdp-sim.sh
--rwxrwxr-x   0 heiland   (1001) heiland   (1001)      472 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/start-tdp-convcheck.sh
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3008 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2/tests/steadystate_double_rotcyl.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2863 2021-01-05 14:05:23.000000 dolfin_navier_scipy-1.3.2/tests/steadystate_generic.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2027 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/steadystate_nse_brob.py
--rw-r--r--   0 heiland   (1001) heiland   (1001)     7697 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2/tests/steadystate_rotcyl.py
--rw-r--r--   0 heiland   (1001) heiland   (1001)     4959 2021-10-15 11:17:41.000000 dolfin_navier_scipy-1.3.2/tests/steadystate_schaefer-turek_2D-1.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     9897 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/tdp_2D_simu.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     6349 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/tdp_convcheck.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     6852 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/test_units_fenicsci.py
--rw-r--r--   0 heiland   (1001) heiland   (1001)     1578 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2/tests/test_units_pfromv.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     5268 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/test_units_residuals.py
--rw-r--r--   0 heiland   (1001) heiland   (1001)     2410 2021-01-07 09:40:14.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2555 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_bcrob.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2907 2022-08-28 09:42:56.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_bigchannel.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2606 2023-05-23 14:00:55.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_double_rotcyl_bcrob.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2425 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_expnonl.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     3664 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_generic.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     1974 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_krylov.py
--rw-rw-r--   0 heiland   (1001) heiland   (1001)     2159 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2/tests/time_dep_nse_linearizations.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.457172 dolfin_navier_scipy-1.3.2.dev1/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      580 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/.readthedocs.yml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      726 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/.zenodo.json
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      135 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/AUTHORS
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      171 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/CHANGELOG.md
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      522 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/CODE.yml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    16752 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/ChangeLog
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    35121 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/LICENSE.md
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3868 2023-05-26 11:58:10.457172 dolfin_navier_scipy-1.3.2.dev1/PKG-INFO
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3123 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2.dev1/README.md
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.437172 dolfin_navier_scipy-1.3.2.dev1/docs/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      444 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/docs/Code.rst
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     5651 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/docs/Makefile
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     8687 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/docs/conf.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      899 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/docs/index.rst
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)       52 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/docs/readthedocs-pip-requirements.txt
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.437172 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      345 2022-03-24 20:40:42.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/__init__.py
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     2364 2020-06-26 05:15:59.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/cache_simustates_utils.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    12747 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/data_output_utils.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    25779 2023-02-05 09:49:45.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/dolfin_to_sparrays.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    52740 2023-01-31 21:38:35.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/problem_setups.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3439 2023-02-13 05:26:25.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/residual_checks.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    60844 2023-05-23 10:50:02.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/stokes_navier_utils.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    22494 2023-03-17 10:38:52.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/time_int_utils.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.437172 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     3868 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/PKG-INFO
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     2862 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/SOURCES.txt
+-rw-r--r--   0 heiland   (1001) heiland   (1001)        1 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/dependency_links.txt
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)        1 2022-03-24 20:34:30.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/not-zip-safe
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)       47 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/pbr.json
+-rw-r--r--   0 heiland   (1001) heiland   (1001)       53 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/requires.txt
+-rw-r--r--   0 heiland   (1001) heiland   (1001)       20 2023-05-26 11:58:10.000000 dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/top_level.txt
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)       53 2022-03-28 14:30:04.000000 dolfin_navier_scipy-1.3.2.dev1/requirements.txt
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      717 2023-05-26 11:58:10.457172 dolfin_navier_scipy-1.3.2.dev1/setup.cfg
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)       76 2022-03-28 14:30:04.000000 dolfin_navier_scipy-1.3.2.dev1/setup.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.441172 dolfin_navier_scipy-1.3.2.dev1/tests/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)        0 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/__init__.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.441172 dolfin_navier_scipy-1.3.2.dev1/tests/deprecatedtests/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     7063 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/deprecatedtests/solve_nse_quadraticterm.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.441172 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3067 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/check_evals.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2687 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/check_int_cylboundary.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     1128 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/checkdofmap.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      298 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/slicedatrange.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     1090 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/test_boundaries_poisson.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2781 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/test_penarobinbc_cyl.py
+drwxrwxr-x   0 heiland   (1001) heiland   (1001)        0 2023-05-26 11:58:10.457172 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      592 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_geo_cntrlbc.json
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      560 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_geo_cntrlbc_rotcntrl.json
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   150127 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl1.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    24475 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl1_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   269677 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl2.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    42852 2020-12-01 18:44:15.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl2_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    84641 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_0.xml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   127538 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_1.xml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   208003 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_2.xml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    34234 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_2.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   434276 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_3.xml
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   648509 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_4.xml
+-rw-r--r--   0 heiland   (1001) heiland   (1001)      702 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_geo_cntrlbc.json
+-rw-r--r--   0 heiland   (1001) heiland   (1001)   246966 2020-04-20 06:11:55.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl1.xml.gz
+-rw-r--r--   0 heiland   (1001) heiland   (1001)    39919 2020-04-20 06:11:55.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl1_facet_region.xml.gz
+-rw-r--r--   0 heiland   (1001) heiland   (1001)   303368 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl2.xml.gz
+-rw-r--r--   0 heiland   (1001) heiland   (1001)    48673 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl2_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      483 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl-bm_geo_cntrlbc.json
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   126225 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl1.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    21007 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl1_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   225707 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl2.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    36861 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl2_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   320808 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl3.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)    51735 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl3_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   810649 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl4.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)   124932 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl4_facet_region.xml.gz
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     1356 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/mini_setup.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)      180 2023-03-13 03:16:04.000000 dolfin_navier_scipy-1.3.2.dev1/tests/start-generic-stst-sim.sh
+-rwxrwxr-x   0 heiland   (1001) heiland   (1001)      454 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/start-generic-tdp-sim.sh
+-rwxrwxr-x   0 heiland   (1001) heiland   (1001)      472 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/start-tdp-convcheck.sh
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3008 2022-01-07 10:00:01.000000 dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_double_rotcyl.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2863 2021-01-05 14:05:23.000000 dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_generic.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2027 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_nse_brob.py
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     7697 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_rotcyl.py
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     4959 2021-10-15 11:17:41.000000 dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_schaefer-turek_2D-1.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     9897 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/tdp_2D_simu.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     6349 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/tdp_convcheck.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     6852 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/test_units_fenicsci.py
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     1578 2020-06-26 05:12:53.000000 dolfin_navier_scipy-1.3.2.dev1/tests/test_units_pfromv.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     5268 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/test_units_residuals.py
+-rw-r--r--   0 heiland   (1001) heiland   (1001)     2410 2021-01-07 09:40:14.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2555 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_bcrob.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2907 2022-08-28 09:42:56.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_bigchannel.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2606 2023-05-23 14:00:55.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_double_rotcyl_bcrob.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2425 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_expnonl.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     3664 2021-09-30 15:49:07.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_generic.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     1974 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_krylov.py
+-rw-rw-r--   0 heiland   (1001) heiland   (1001)     2159 2019-11-13 15:26:05.000000 dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_linearizations.py
```

### Comparing `dolfin_navier_scipy-1.3.2/.readthedocs.yml` & `dolfin_navier_scipy-1.3.2.dev1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/.zenodo.json` & `dolfin_navier_scipy-1.3.2.dev1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/CODE.yml` & `dolfin_navier_scipy-1.3.2.dev1/CODE.yml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/ChangeLog` & `dolfin_navier_scipy-1.3.2.dev1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 CHANGES
 =======
 
-1.3.2
------
-
 * double cyl and time integration
 
 1.3.1
 -----
 
 * added basic semi-implicit euler scheme + some cleanup + check for data point filtering
 * documentation in the residual check
```

### Comparing `dolfin_navier_scipy-1.3.2/LICENSE.md` & `dolfin_navier_scipy-1.3.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/PKG-INFO` & `dolfin_navier_scipy-1.3.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolfin_navier_scipy
-Version: 1.3.2
+Version: 1.3.2.dev1
 Summary: A Scipy-Fenics interface for incompressible Navier-Stokes
 Home-page: https://github.com/highlando/dolfin_navier_scipy
 Author: Jan Heiland
 Author-email: jnhlnd@gmail.com
 Maintainer: Jan Heiland
 Maintainer-email: jnhlnd@gmail.com
 License: GPLv3
```

### Comparing `dolfin_navier_scipy-1.3.2/README.md` & `dolfin_navier_scipy-1.3.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/docs/Makefile` & `dolfin_navier_scipy-1.3.2.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/docs/conf.py` & `dolfin_navier_scipy-1.3.2.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/docs/index.rst` & `dolfin_navier_scipy-1.3.2.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/cache_simustates_utils.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/cache_simustates_utils.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/data_output_utils.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/data_output_utils.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/dolfin_to_sparrays.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/dolfin_to_sparrays.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/problem_setups.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/problem_setups.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/residual_checks.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/residual_checks.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/stokes_navier_utils.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/stokes_navier_utils.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy/time_int_utils.py` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy/time_int_utils.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/PKG-INFO` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolfin-navier-scipy
-Version: 1.3.2
+Version: 1.3.2.dev1
 Summary: A Scipy-Fenics interface for incompressible Navier-Stokes
 Home-page: https://github.com/highlando/dolfin_navier_scipy
 Author: Jan Heiland
 Author-email: jnhlnd@gmail.com
 Maintainer: Jan Heiland
 Maintainer-email: jnhlnd@gmail.com
 License: GPLv3
```

### Comparing `dolfin_navier_scipy-1.3.2/dolfin_navier_scipy.egg-info/SOURCES.txt` & `dolfin_navier_scipy-1.3.2.dev1/dolfin_navier_scipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/setup.cfg` & `dolfin_navier_scipy-1.3.2.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/deprecatedtests/solve_nse_quadraticterm.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/deprecatedtests/solve_nse_quadraticterm.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/lilchecks/check_evals.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/check_evals.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/lilchecks/check_int_cylboundary.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/check_int_cylboundary.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/lilchecks/checkdofmap.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/checkdofmap.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/lilchecks/test_boundaries_poisson.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/test_boundaries_poisson.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/lilchecks/test_penarobinbc_cyl.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/lilchecks/test_penarobinbc_cyl.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_geo_cntrlbc.json` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_geo_cntrlbc.json`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_geo_cntrlbc_rotcntrl.json` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_geo_cntrlbc_rotcntrl.json`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl1.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl1.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl1_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl1_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl2.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl2.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/2D-double-rotcyl_lvl2_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/2D-double-rotcyl_lvl2_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_0.xml` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_0.xml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_1.xml` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_1.xml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_2.xml` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_2.xml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_2.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_2.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_3.xml` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_3.xml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/cylinder_4.xml` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/cylinder_4.xml`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_geo_cntrlbc.json` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_geo_cntrlbc.json`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl1.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl1.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl1_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl1_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl2.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl2.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-outlets_lvl2_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-outlets_lvl2_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl1.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl1.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl1_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl1_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl2.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl2.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl2_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl2_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl3.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl3.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl3_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl3_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl4.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl4.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mesh/karman2D-rotcyl_lvl4_facet_region.xml.gz` & `dolfin_navier_scipy-1.3.2.dev1/tests/mesh/karman2D-rotcyl_lvl4_facet_region.xml.gz`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/mini_setup.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/mini_setup.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/steadystate_double_rotcyl.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_double_rotcyl.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/steadystate_generic.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_generic.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/steadystate_nse_brob.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_nse_brob.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/steadystate_rotcyl.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_rotcyl.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/steadystate_schaefer-turek_2D-1.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/steadystate_schaefer-turek_2D-1.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/tdp_2D_simu.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/tdp_2D_simu.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/tdp_convcheck.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/tdp_convcheck.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/test_units_fenicsci.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/test_units_fenicsci.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/test_units_pfromv.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/test_units_pfromv.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/test_units_residuals.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/test_units_residuals.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_bcrob.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_bcrob.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_bigchannel.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_bigchannel.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_double_rotcyl_bcrob.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_double_rotcyl_bcrob.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_expnonl.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_expnonl.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_generic.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_generic.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_krylov.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_krylov.py`

 * *Files identical despite different names*

### Comparing `dolfin_navier_scipy-1.3.2/tests/time_dep_nse_linearizations.py` & `dolfin_navier_scipy-1.3.2.dev1/tests/time_dep_nse_linearizations.py`

 * *Files identical despite different names*


# Comparing `tmp/wofryimpl-1.0.8.tar.gz` & `tmp/wofryimpl-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wofryimpl-1.0.8.tar", last modified: Mon Jul 12 14:35:29 2021, max compression
+gzip compressed data, was "dist/wofryimpl-1.0.9.tar", last modified: Thu Mar 31 10:57:37 2022, max compression
```

## Comparing `wofryimpl-1.0.8.tar` & `wofryimpl-1.0.9.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/
--rwxr-xr-x   0 srio      (4230) soft      (3401)       86 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/MANIFEST.in
--rw-r--r--   0 srio      (4230) soft      (3401)     1162 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)       57 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/README.md
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/examples/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4563 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/example_arago_poisson.py
--rw-r--r--   0 srio      (4230) soft      (3401)    16488 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/example_ideal_lens.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5832 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/json_tools.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21090 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/run_wofry_beamline_and_dump_files.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2177 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/examples/run_wofry_beamline_from_files.py
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/setup.cfg
--rwxr-xr-x   0 srio      (4230) soft      (3401)     4303 2021-07-12 14:34:46.000000 wofryimpl-1.0.8/setup.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/beamline/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    11592 2021-02-22 08:17:47.000000 wofryimpl-1.0.8/wofryimpl/beamline/beamline.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3022 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/beam_stopper.py
--rw-r--r--   0 srio      (4230) soft      (3401)     7530 2021-01-14 08:31:23.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/slit.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2071 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/lens.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1169 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/screen.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/examples/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/examples/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     7246 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/examples/propagation_scaling_therorem_1D.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3539 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/examples/propagation_spherical_wave.py
--rw-r--r--   0 srio      (4230) soft      (3401)    13824 2021-01-14 08:31:23.000000 wofryimpl-1.0.8/wofryimpl/propagator/light_source.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/
--rw-r--r--   0 srio      (4230) soft      (3401)      899 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5296 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fraunhofer.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1731 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2192 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_convolution.py
--rw-r--r--   0 srio      (4230) soft      (3401)     2408 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_zoom.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3404 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_zoom_scaling_theorem.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3908 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/integral.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/
--rw-r--r--   0 srio      (4230) soft      (3401)      755 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4868 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fraunhofer.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3878 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4165 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel_convolution.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5866 2021-07-12 13:29:58.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel_zoom_xy.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6747 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/integral.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/propagators/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/propagators/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     3412 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/propagators/srw_fresnel.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21402 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/propagators1D_test.py
--rw-r--r--   0 srio      (4230) soft      (3401)    33050 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/propagators2D_test.py
--rw-r--r--   0 srio      (4230) soft      (3401)    29472 2021-01-07 09:22:42.000000 wofryimpl-1.0.8/wofryimpl/propagator/test/wavefronts_test.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/propagator/util/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-02-22 08:17:47.000000 wofryimpl-1.0.8/wofryimpl/propagator/util/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    20824 2021-07-12 14:19:43.000000 wofryimpl-1.0.8/wofryimpl/propagator/util/undulator_coherent_mode_decomposition_1d.py
--rw-r--r--   0 srio      (4230) soft      (3401)      256 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl/version.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)     1162 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     2226 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2021-07-12 12:14:54.000000 wofryimpl-1.0.8/wofryimpl.egg-info/not-zip-safe
--rw-r--r--   0 srio      (4230) soft      (3401)       28 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       19 2021-07-12 14:35:29.000000 wofryimpl-1.0.8/wofryimpl.egg-info/top_level.txt
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1096 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/LICENSE
+-rwxr-xr-x   0 srio      (4230) soft      (3401)       86 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/MANIFEST.in
+-rw-r--r--   0 srio      (4230) soft      (3401)     1157 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)       57 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/README.md
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/examples/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4563 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/example_arago_poisson.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    16488 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/example_ideal_lens.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5832 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/json_tools.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21090 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/run_wofry_beamline_and_dump_files.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2177 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/examples/run_wofry_beamline_from_files.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/setup.cfg
+-rwxr-xr-x   0 srio      (4230) soft      (3401)     4303 2022-03-31 10:56:55.000000 wofryimpl-1.0.9/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/beamline/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    11592 2021-02-22 08:17:47.000000 wofryimpl-1.0.9/wofryimpl/beamline/beamline.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3055 2022-03-31 10:56:02.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/beam_stopper.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     7530 2021-01-14 08:31:23.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/slit.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2071 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/lens.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1169 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/screen.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/examples/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/examples/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     7246 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/examples/propagation_scaling_therorem_1D.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3539 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/examples/propagation_spherical_wave.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    13824 2021-01-14 08:31:23.000000 wofryimpl-1.0.9/wofryimpl/propagator/light_source.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/
+-rw-r--r--   0 srio      (4230) soft      (3401)      899 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5296 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fraunhofer.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1731 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2192 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_convolution.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     2408 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_zoom.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3404 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_zoom_scaling_theorem.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3908 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/integral.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/
+-rw-r--r--   0 srio      (4230) soft      (3401)      755 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4868 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fraunhofer.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3878 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4165 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel_convolution.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5866 2021-07-12 13:29:58.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel_zoom_xy.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6747 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/integral.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/propagators/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/propagators/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     3412 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/propagators/srw_fresnel.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21402 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/propagators1D_test.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    33050 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/propagators2D_test.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    29472 2021-01-07 09:22:42.000000 wofryimpl-1.0.9/wofryimpl/propagator/test/wavefronts_test.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/propagator/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2021-02-22 08:17:47.000000 wofryimpl-1.0.9/wofryimpl/propagator/util/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    20824 2021-07-12 14:19:43.000000 wofryimpl-1.0.9/wofryimpl/propagator/util/undulator_coherent_mode_decomposition_1d.py
+-rw-r--r--   0 srio      (4230) soft      (3401)      256 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl/version.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1157 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     2234 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2021-07-12 12:14:54.000000 wofryimpl-1.0.9/wofryimpl.egg-info/not-zip-safe
+-rw-r--r--   0 srio      (4230) soft      (3401)       28 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       19 2022-03-31 10:57:37.000000 wofryimpl-1.0.9/wofryimpl.egg-info/top_level.txt
```

### Comparing `wofryimpl-1.0.8/PKG-INFO` & `wofryimpl-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: wofryimpl
-Version: 1.0.8
+Version: 1.0.9
 Summary: WOFRY (Wave Optics FRamework in pYthon) standard implementation
 Home-page: https://github.com/oasys-kit/wofryimpl
 Author: Manuel Sanchez del Rio, Luca Rebuffi
 Author-email: srio@esrf.eu
 Maintainer: Manuel Sanchez del Rio
 Maintainer-email: srio@esrf.eu
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/wofryimpl
-Description: # wofryimpl
-        Standard implementation of the wofry library
-        
 Keywords: dictionary,glossary,synchrotronsimulation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+License-File: LICENSE
+
+# wofryimpl
+Standard implementation of the wofry library
+
+
```

### Comparing `wofryimpl-1.0.8/examples/example_arago_poisson.py` & `wofryimpl-1.0.9/examples/example_arago_poisson.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/examples/example_ideal_lens.py` & `wofryimpl-1.0.9/examples/example_ideal_lens.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/examples/json_tools.py` & `wofryimpl-1.0.9/examples/json_tools.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/examples/run_wofry_beamline_and_dump_files.py` & `wofryimpl-1.0.9/examples/run_wofry_beamline_and_dump_files.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/examples/run_wofry_beamline_from_files.py` & `wofryimpl-1.0.9/examples/run_wofry_beamline_from_files.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/setup.py` & `wofryimpl-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'wofryimpl'
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 ISRELEASED = True
 
 DESCRIPTION = 'WOFRY (Wave Optics FRamework in pYthon) standard implementation'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Manuel Sanchez del Rio, Luca Rebuffi'
 AUTHOR_EMAIL = 'srio@esrf.eu'
```

### Comparing `wofryimpl-1.0.8/wofryimpl/beamline/beamline.py` & `wofryimpl-1.0.9/wofryimpl/beamline/beamline.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/beam_stopper.py` & `wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/beam_stopper.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         else:
             raise NotImplementedError("to be implemented")
 
         return wavefront
 
     def to_python_code(self):
         boundary_shape = self.get_boundary_shape()
-        txt = "\nfrom syned.beamline.shape import *"
+        txt = "\nfrom syned.beamline.shape import Rectangle, Circle, Ellipse"
         if isinstance(boundary_shape, Rectangle):
             txt += "\nboundary_shape=Rectangle(%g, %g, %g, %g)" % boundary_shape.get_boundaries()
         elif isinstance(boundary_shape, Circle):
             txt += "\nboundary_shape=Circle(%g, %g, %g)" % boundary_shape.get_boundaries()
         elif isinstance(boundary_shape, Ellipse):
             txt += "\nboundary_shape=Ellipse(%g, %g, %g, %g)" % boundary_shape.get_boundaries()
         txt += "\n"
@@ -49,15 +49,15 @@
         else:
             raise NotImplementedError("to be implemented")
 
         return wavefront
 
     def to_python_code(self):
         boundary_shape = self.get_boundary_shape()
-        txt = "\nfrom syned.beamline.shape import *"
+        txt = "\nfrom syned.beamline.shape import Rectangle"
         if isinstance(boundary_shape, Rectangle):
             txt += "\nboundary_shape=Rectangle(%g, %g, %g, %g)" % boundary_shape.get_boundaries()
         else:
             txt += "\n# ERROR getting boundary shape..."
         txt += "\n"
         txt += "from wofryimpl.beamline.optical_elements.absorbers.beam_stopper import WOBeamStopper1D"
         txt += "\n"
```

### Comparing `wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/absorbers/slit.py` & `wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/absorbers/slit.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/lens.py` & `wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/lens.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/beamline/optical_elements/ideal_elements/screen.py` & `wofryimpl-1.0.9/wofryimpl/beamline/optical_elements/ideal_elements/screen.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/examples/propagation_scaling_therorem_1D.py` & `wofryimpl-1.0.9/wofryimpl/propagator/examples/propagation_scaling_therorem_1D.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/examples/propagation_spherical_wave.py` & `wofryimpl-1.0.9/wofryimpl/propagator/examples/propagation_spherical_wave.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/light_source.py` & `wofryimpl-1.0.9/wofryimpl/propagator/light_source.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/__init__.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/__init__.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fraunhofer.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fraunhofer.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_convolution.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_convolution.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_zoom.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_zoom.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/fresnel_zoom_scaling_theorem.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/fresnel_zoom_scaling_theorem.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators1D/integral.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators1D/integral.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/__init__.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/__init__.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fraunhofer.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fraunhofer.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel_convolution.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel_convolution.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/fresnel_zoom_xy.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/fresnel_zoom_xy.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/propagators2D/integral.py` & `wofryimpl-1.0.9/wofryimpl/propagator/propagators2D/integral.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/test/propagators/srw_fresnel.py` & `wofryimpl-1.0.9/wofryimpl/propagator/test/propagators/srw_fresnel.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/test/propagators1D_test.py` & `wofryimpl-1.0.9/wofryimpl/propagator/test/propagators1D_test.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/test/propagators2D_test.py` & `wofryimpl-1.0.9/wofryimpl/propagator/test/propagators2D_test.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/test/wavefronts_test.py` & `wofryimpl-1.0.9/wofryimpl/propagator/test/wavefronts_test.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl/propagator/util/undulator_coherent_mode_decomposition_1d.py` & `wofryimpl-1.0.9/wofryimpl/propagator/util/undulator_coherent_mode_decomposition_1d.py`

 * *Files identical despite different names*

### Comparing `wofryimpl-1.0.8/wofryimpl.egg-info/PKG-INFO` & `wofryimpl-1.0.9/wofryimpl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: wofryimpl
-Version: 1.0.8
+Version: 1.0.9
 Summary: WOFRY (Wave Optics FRamework in pYthon) standard implementation
 Home-page: https://github.com/oasys-kit/wofryimpl
 Author: Manuel Sanchez del Rio, Luca Rebuffi
 Author-email: srio@esrf.eu
 Maintainer: Manuel Sanchez del Rio
 Maintainer-email: srio@esrf.eu
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/wofryimpl
-Description: # wofryimpl
-        Standard implementation of the wofry library
-        
 Keywords: dictionary,glossary,synchrotronsimulation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+License-File: LICENSE
+
+# wofryimpl
+Standard implementation of the wofry library
+
+
```

### Comparing `wofryimpl-1.0.8/wofryimpl.egg-info/SOURCES.txt` & `wofryimpl-1.0.9/wofryimpl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 examples/__init__.py
 examples/example_arago_poisson.py
 examples/example_ideal_lens.py
 examples/json_tools.py
```


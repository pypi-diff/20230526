# Comparing `tmp/scipion-em-reliontomo-3.1.6.tar.gz` & `tmp/scipion-em-reliontomo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-reliontomo-3.1.6.tar", last modified: Mon Apr 24 13:54:51 2023, max compression
+gzip compressed data, was "scipion-em-reliontomo-3.2.0.tar", last modified: Fri May 26 08:50:28 2023, max compression
```

## Comparing `scipion-em-reliontomo-3.1.6.tar` & `scipion-em-reliontomo-3.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/bibtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/cmd/compareStarFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convert30_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21765 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convert40_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/convert/convertBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.600925 scipion-em-reliontomo-3.1.6/reliontomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_3d_classify_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_import_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_per_part_per_tilt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_relion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_ctf_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_de_novo_initial_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_edit_particles_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_coordinates_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_subtomograms_from_star.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_make_pseudo_subtomos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_matching_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_tomogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_refine_subtomograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_tomo_frame_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/relion_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/reliontomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_compare_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_import_star_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/tests/test_refine_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/viewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/reliontomo/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:54:51.000000 scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:54:51.604925 scipion-em-reliontomo-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-24 13:52:47.000000 scipion-em-reliontomo-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.758902 scipion-em-reliontomo-3.2.0/reliontomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.758902 scipion-em-reliontomo-3.2.0/reliontomo/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/cmd/compareStarFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.758902 scipion-em-reliontomo-3.2.0/reliontomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/convert/convert30_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21780 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/convert/convert40_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/convert/convertBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/reliontomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_3d_classify_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_import_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_per_part_per_tilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_relion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_ctf_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_de_novo_initial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_edit_particles_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_import_coordinates_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_import_subtomograms_from_star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_make_pseudo_subtomos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_matching_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17922 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_rec_tomogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19089 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_refine_subtomograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_tomo_frame_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/relion_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/reliontomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/tests/test_compare_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/tests/test_import_star_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/tests/test_refine_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/reliontomo/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-26 08:50:28.000000 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-26 08:50:28.000000 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:50:28.000000 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 08:50:28.000000 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 08:50:28.000000 scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:50:28.762902 scipion-em-reliontomo-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-26 08:48:47.000000 scipion-em-reliontomo-3.2.0/setup.py
```

### Comparing `scipion-em-reliontomo-3.1.6/LICENSE` & `scipion-em-reliontomo-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/PKG-INFO` & `scipion-em-reliontomo-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.6
+Version: 3.2.0
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.6/README.rst` & `scipion-em-reliontomo-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/__init__.py` & `scipion-em-reliontomo-3.2.0/reliontomo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import pwem
 import relion
 from reliontomo.constants import RELIONTOMO_HOME, RELIONTOMO_DEFAULT, RELION, RELIONTOMO_CUDA_LIB, V4_0
 
 _logo = "relion_logo.png"
 _references = ['Scheres2012a', 'Scheres2012b', 'Kimanius2016', 'Zivanov2018']
-__version__ = '3.1.6'
+__version__ = '3.2.0'
 
 
 class Plugin(relion.Plugin):
     _supportedVersions = [V4_0]
     _homeVar = RELIONTOMO_HOME
     _pathVars = [RELIONTOMO_HOME]
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/bibtex.py` & `scipion-em-reliontomo-3.2.0/reliontomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/cmd/compareStarFiles.py` & `scipion-em-reliontomo-3.2.0/reliontomo/cmd/compareStarFiles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/constants.py` & `scipion-em-reliontomo-3.2.0/reliontomo/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,16 +139,27 @@
 IN_TOMOS_STAR = 'inTomos.star'
 OUT_TOMOS_STAR = 'tomograms.star'
 IN_COORDS_STAR = 'inCoords.star'
 IN_PARTICLES_STAR = 'inSubtomos.star'
 OUT_PARTICLES_STAR = 'particles.star'
 TRAJECTORIES_STAR = 'trajectories.star'
 MANIFOLDS_STAR = 'manifolds.star'
+
+REFINE_FSC_REF_STAR = '_model.star'
+REFINE_STAR_FSC_TABLE = 'model_class_1'
+REFINE_STAR_FSC_COLUMNS = ['rlnGoldStandardFsc', 'rlnFourierCompleteness']
+
 POSTPROCESS_DIR = 'PostProcess'
 FSC_REF_STAR = join(POSTPROCESS_DIR, 'postprocess.star')
+POSTPROCESS_STAR_FSC_TABLE = 'fsc'
+POSTPROCESS_STAR_FSC_COLUMNS = ['rlnFourierShellCorrelationCorrected',
+                                'rlnFourierShellCorrelationUnmaskedMaps',
+                                'rlnFourierShellCorrelationMaskedMaps',
+                                'rlnCorrectedFourierShellCorrelationPhaseRandomizedMaskedMaps']
+
 RE4_INDIV_GEN_FILES = [OUT_TOMOS_STAR, OUT_PARTICLES_STAR, TRAJECTORIES_STAR, MANIFOLDS_STAR, FSC_REF_STAR]
 OPTIMISATION_SET_STAR = 'optimisation_set.star'
 PSUBTOMOS_SQLITE = 'pseudosubtomograms%s.sqlite'
 
 
 # Initial models
 REC_PARTICLES_DIR = 'recParticles'
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/convert/__init__.py` & `scipion-em-reliontomo-3.2.0/reliontomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/convert/convert30_tomo.py` & `scipion-em-reliontomo-3.2.0/reliontomo/convert/convert30_tomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/convert/convert40_tomo.py` & `scipion-em-reliontomo-3.2.0/reliontomo/convert/convert40_tomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         optGroup = OpticsGroups.fromString(pSubtomoSet.getAcquisition().opticsGroupInfo.get())
         with open(outStar, 'w') as f:
             optGroup.toStar(f)
             # Write header first
             partsWriter = Table.Writer(f)
             partsWriter.writeTableName(PARTICLES_TABLE)
             partsWriter.writeHeader(tomoTable.getColumns())
-            for pSubtomo in pSubtomoSet:
+            for pSubtomo in pSubtomoSet.iterSubtomos():
                 angles, shifts = getTransformInfoFromCoordOrSubtomo(pSubtomo, pSubtomo.getSamplingRate())
                 pSubtomoFile = pSubtomo.getFileName()
                 pSubtomoFile = pSubtomoFile.replace(':' + MRC, '') if pSubtomoFile else FILE_NOT_FOUND
                 pSubtomoCtfFile = pSubtomo.getCtfFile() if pSubtomo.getCtfFile() else FILE_NOT_FOUND
 
                 # Add row to the table which will be used to generate the STAR file
                 rowsValues = [
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/convert/convertBase.py` & `scipion-em-reliontomo-3.2.0/reliontomo/convert/convertBase.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/objects.py` & `scipion-em-reliontomo-3.2.0/reliontomo/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/__init__.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_3d_classify_subtomograms.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_3d_classify_subtomograms.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     """3D Classification of subtomograms."""
 
     _label = '3D Classification of subtomograms'
     modelTable = Table()
     classesTable = Table()
     opticsTable = Table()
     particlesTable = Table()
+    _possibleOutputs = outputObjects
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         super()._defineInputParams(form)
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_import_from_star.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_import_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_make_pseusosubtomos_and_rec_particle.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_per_part_per_tilt.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_per_part_per_tilt.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_refine.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,30 +286,34 @@
 
     def convertInputStep(self):
         self.genInStarFile(withPriors=self.alignmentAsPriors)
 
     # -------------------------- INFO functions -------------------------------
 
     # --------------------------- UTILS functions -----------------------------
-    def _genBaseCommand(self):
+    def _genBaseCommand(self, useOptimizationSet=True ):
         cmd = ''
-        cmd += self._genIOBaseCmd()  # I/O args
+        cmd += self._genIOBaseCmd(useOptimizationSet=useOptimizationSet)  # I/O args
         cmd += self._genCTFBaseCmd()  # CTF args
         cmd += self._genOptimisationBaseCmd()  # Optimisation args
         cmd += self._genComputeBaseCmd()  # Compute args
         cmd += self._genAddiotionalBaseCmd()  # Additional args
         return cmd
 
-    def _genIOBaseCmd(self):
+    def _genIOBaseCmd(self, useOptimizationSet=True):
 
         inRelionParticles = self.getInputParticles()
 
-        # Use optimization set file
-        self.info("Using optimization_set: %s" % inRelionParticles.filesMaster)
-        cmd = '--ios %s ' % inRelionParticles.filesMaster
+        cmd = ''
+
+        if useOptimizationSet:
+            # Use optimization set file
+            self.info("Using optimization_set: %s" % inRelionParticles.filesMaster)
+            cmd += '--ios %s ' % inRelionParticles.filesMaster
+
 
         cmd += '--i %s ' % self.getOutStarFileName()
         cmd += '--o %s ' % (self._getExtraPath() + '/')  # If not, Relion will concatenate it directly as a prefix
         cmd += '--j %i ' % self.numberOfThreads
         return cmd
 
     def _genCTFBaseCmd(self):
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_base_relion.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_base_relion.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion-users@lists.sourceforge.net'
 # *
 # **************************************************************************
 from os.path import exists, join
+from emtable import Table
 
-from pwem.objects import VolumeMask
+from pwem.objects import VolumeMask, FSC
 from pwem.protocols import EMProtocol
 from pyworkflow.protocol import PointerParam
 from pyworkflow.utils import Message, createLink
 from reliontomo.constants import IN_PARTICLES_STAR, POSTPROCESS_DIR, OPTIMISATION_SET_STAR, PSUBTOMOS_SQLITE, \
     OUT_PARTICLES_STAR
 from reliontomo.convert import writeSetOfPseudoSubtomograms, readSetOfPseudoSubtomograms
 from reliontomo.objects import createSetOfRelionPSubtomograms, RelionSetOfPseudoSubtomograms
@@ -101,7 +102,20 @@
             psubtomoSet.setBoxSize(boxSize)
 
         # Fill the items (pseudo subtomos/particles) from de particles star file
         readSetOfPseudoSubtomograms(psubtomoSet)
 
         return psubtomoSet
 
+    def genFSCs(self, starFile, tableName, fscColumns):
+        fscSet = self._createSetOfFSCs()
+        table = Table(fileName=starFile, tableName=tableName)
+        resolution_inv = table.getColumnValues('rlnResolution')
+        for columnName in fscColumns:
+            columValues = table.getColumnValues(columnName)
+            fsc = FSC(objLabel=columnName[3:])
+            fsc.setData(resolution_inv, columValues)
+            fscSet.append(fsc)
+
+        fscSet.write()
+        return fscSet
+
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_ctf_refine.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_ctf_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_de_novo_initial_model.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_de_novo_initial_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self._defineSourceRelation(inRelionParticles, vol)
 
     # -------------------------- INFO functions -------------------------------
 
     # --------------------------- UTILS functions -----------------------------
     def _genInitModelCommand(self):
         # Common parameters from base protocol
-        cmd = self._genBaseCommand()
+        cmd = self._genBaseCommand(useOptimizationSet=False)
 
         # Initial model specific commands
         cmd += ' --denovo_3dref --grad --zero_mask --auto_sampling --pad 1 '
         #   Optimisation args
         cmd += '--iter %i ' % self.nVdamMiniBatches.get()
         cmd += '--tau2_fudge %d ' % self.regularisation.get()
         cmd += '--K %i ' % self.numberOfClasses.get()
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_edit_particles_star.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_edit_particles_star.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from enum import Enum
 from pyworkflow import BETA
-from pyworkflow.protocol import BooleanParam, FloatParam, EnumParam
+from pyworkflow.protocol import BooleanParam, FloatParam, EnumParam, \
+    PointerParam
 from reliontomo import Plugin
 from reliontomo.constants import OUT_PARTICLES_STAR, COORD_X, COORD_Y, COORD_Z, SHIFTX_ANGST, SHIFTY_ANGST, \
     SHIFTZ_ANGST, ROT, TILT, PSI
 from reliontomo.objects import RelionSetOfPseudoSubtomograms
 from reliontomo.protocols.protocol_base_relion import ProtRelionTomoBase
 from reliontomo.utils import genEnumParamDict
 
@@ -69,14 +70,20 @@
         super()._defineCommonInputParams(form)
         form.addSection(label='Center')
         form.addParam('doRecenter', BooleanParam,
                       label='Perform centering of particles',
                       default=False,
                       help='Perform centering of particles according to a position in the reference.')
         group = form.addGroup('Shift center', condition='doRecenter')
+        group.addParam('averageSubTomogram', PointerParam, pointerClass='AverageSubTomogram',
+                      label='Average of subtomogram (optional)', allowsNull=True,
+                      )
+        group.addParam('refMask', PointerParam, pointerClass='VolumeMask',
+                       label='Reference mask (optional)', allowsNull=True,
+                       )
         group.addParam('shiftX', FloatParam,
                        label='X (pix.)',
                        default=0,
                        help='X-coordinate in the reference to center particles on (in pix)')
         group.addParam('shiftY', FloatParam,
                        label='Y (pix.)',
                        default=0,
@@ -212,7 +219,13 @@
                     operateCmd += '--operate %s ' % label
                 else:
                     operateCmd += '--operate%i %s ' % (counter, label)
                 counter += 1
 
         return operateCmd
 
+    def getAverageSubTomogram(self):
+        return self.averageSubTomogram.get()
+
+    def getMask3D(self):
+        return self.refMask.get()
+
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_coordinates_from_star.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_import_coordinates_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_import_subtomograms_from_star.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_import_subtomograms_from_star.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_make_pseudo_subtomos.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_make_pseudo_subtomos.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_matching_coordinates.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_matching_coordinates.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_post_process.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_post_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,32 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from enum import Enum
-from pwem.objects import VolumeMask
+from pwem.objects import VolumeMask, FSC
 from pyworkflow import BETA
 from pyworkflow.protocol import PointerParam, BooleanParam, FloatParam, GE, LE, IntParam, FileParam
 from pyworkflow.utils import makePath
 from reliontomo import Plugin
-from reliontomo.constants import POST_PROCESS_MRC, POSTPROCESS_DIR
+from reliontomo.constants import POST_PROCESS_MRC, POSTPROCESS_DIR, \
+    POSTPROCESS_STAR_FSC_TABLE, \
+    POSTPROCESS_STAR_FSC_COLUMNS, FSC_REF_STAR
 from reliontomo.objects import RelionSetOfPseudoSubtomograms
 from reliontomo.protocols.protocol_base_relion import ProtRelionTomoBase
 
 NO_MTF_FILE = 0
 
 
 class outputObjects(Enum):
     relionParticles = RelionSetOfPseudoSubtomograms
     postProcessVolume = VolumeMask
+    outputFSC = FSC
 
 
 class ProtRelionPostProcess(ProtRelionTomoBase):
     """Sharpen a 3D reference map and estimate the gold-standard FSC curves for subtomogram averaging"""
 
     _label = 'postprocessing'
     _devStatus = BETA
@@ -150,16 +153,24 @@
     def relionPostProcessStep(self):
         Plugin.runRelionTomo(self, 'relion_postprocess', self.genPostProcessCmd())
 
     def createOutputStep(self):
         inParticles = self.inReParticles.get()
         pSubtomoSet = self.genRelionParticles()
         postProccesMrc = self._genPostProcessOutputMrcFile(POST_PROCESS_MRC)
+
+        # Output FSC
+
+        fn = self._getExtraPath(FSC_REF_STAR)
+        setOfFSC = self.genFSCs(fn, POSTPROCESS_STAR_FSC_TABLE,
+                                POSTPROCESS_STAR_FSC_COLUMNS)
+
         self._defineOutputs(**{outputObjects.postProcessVolume.name: postProccesMrc,
-                               outputObjects.relionParticles.name: pSubtomoSet})
+                               outputObjects.relionParticles.name: pSubtomoSet,
+                               outputObjects.outputFSC.name: setOfFSC})
         self._defineSourceRelation(inParticles, postProccesMrc)
         self._defineSourceRelation(inParticles, pSubtomoSet)
 
     # -------------------------- INFO functions -------------------------------
     def _validate(self):
         pass
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_prepare_data.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_prepare_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_rec_particle_from_subtomograms.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_rec_tomogram.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_rec_tomogram.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_reconstruc_particle_from_ts.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_refine_subtomograms.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_refine_subtomograms.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,33 @@
 # *
 # **************************************************************************
 import glob
 import re
 from enum import Enum
 from emtable import Table
 from pwem.convert.headers import fixVolume
-from pwem.objects import FSC
+from pwem.objects import SetOfFSCs
 from pyworkflow import BETA
 from reliontomo.objects import RelionSetOfPseudoSubtomograms
 from reliontomo.protocols.protocol_base_refine import ProtRelionRefineBase
 from reliontomo import Plugin
 from os.path import getmtime
 from pyworkflow.protocol import PointerParam, LEVEL_ADVANCED, FloatParam, StringParam, BooleanParam, EnumParam
 from pyworkflow.utils import createLink
-from reliontomo.constants import ANGULAR_SAMPLING_LIST, SYMMETRY_HELP_MSG, OUT_PARTICLES_STAR
+from reliontomo.constants import ANGULAR_SAMPLING_LIST, SYMMETRY_HELP_MSG, \
+    OUT_PARTICLES_STAR, REFINE_FSC_REF_STAR, REFINE_STAR_FSC_TABLE, \
+    REFINE_STAR_FSC_COLUMNS
 from reliontomo.utils import getProgram
 from tomo.objects import AverageSubTomogram
 
 
 class outputObjects(Enum):
     relionParticles = RelionSetOfPseudoSubtomograms
     average = AverageSubTomogram
-    outputFSC = FSC
+    outputFSC = SetOfFSCs
 
 
 class ProtRelionRefineSubtomograms(ProtRelionRefineBase):
     """Auto-refinement of subtomograms."""
 
     _label = 'Auto-refinement of subtomograms'
     _devStatus = BETA
@@ -225,28 +227,26 @@
         vol.setSamplingRate(relionParticles.getCurrentSamplingRate())
         pattern = '*it*half%s_class*.mrc'
         half1 = self._getLastFileName(self._getExtraPath(pattern % 1))
         half2 = self._getLastFileName(self._getExtraPath(pattern % 2))
         vol.setHalfMaps([half1, half2])
 
         # Output FSC
-        fsc = FSC(objLabel=self.getRunName())
-        fn = self._getExtraPath("_model.star")
-        table = Table(fileName=fn, tableName='model_class_1')
-        resolution_inv = table.getColumnValues('rlnResolution')
-        frc = table.getColumnValues('rlnGoldStandardFsc')
-        fsc.setData(resolution_inv, frc)
+        fn = self._getExtraPath(REFINE_FSC_REF_STAR)
+
+        setOfFSC = self.genFSCs(fn, REFINE_STAR_FSC_TABLE,
+                                REFINE_STAR_FSC_COLUMNS)
 
         outputDict = {outputObjects.relionParticles.name: relionParticles,
                       outputObjects.average.name: vol,
-                      outputObjects.outputFSC.name: fsc}
+                      outputObjects.outputFSC.name: setOfFSC}
         self._defineOutputs(**outputDict)
         self._defineSourceRelation(inParticles, relionParticles)
         self._defineSourceRelation(inParticles, vol)
-        self._defineSourceRelation(inParticles, fsc)
+        self._defineSourceRelation(inParticles, setOfFSC)
 
     # -------------------------- INFO functions -------------------------------
 
     # --------------------------- UTILS functions -----------------------------
     def _genAutoRefineCommand(self):
         cmd = self._genBaseCommand()
         cmd += ' --auto_refine --split_random_halves --low_resol_join_halves 40 --norm --scale --flatten_solvent '
```

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols/protocol_tomo_frame_align.py` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols/protocol_tomo_frame_align.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/protocols.conf` & `scipion-em-reliontomo-3.2.0/reliontomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/relion_logo.png` & `scipion-em-reliontomo-3.2.0/reliontomo/relion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/tests/__init__.py` & `scipion-em-reliontomo-3.2.0/reliontomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_compare_star_files.py` & `scipion-em-reliontomo-3.2.0/reliontomo/tests/test_compare_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_conversion.py` & `scipion-em-reliontomo-3.2.0/reliontomo/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_import_star_files.py` & `scipion-em-reliontomo-3.2.0/reliontomo/tests/test_import_star_files.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/tests/test_refine_cycle.py` & `scipion-em-reliontomo-3.2.0/reliontomo/tests/test_refine_cycle.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/reliontomo/utils.py` & `scipion-em-reliontomo-3.2.0/reliontomo/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/PKG-INFO` & `scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-reliontomo
-Version: 3.1.6
+Version: 3.2.0
 Summary: Plugin to use Relion programs for tomography within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-reliontomo
 Author: CNB-CSIC
 Author-email: jjimenez@cnb.csic.es, scipion-users@lists.sourceforge.net
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-reliontomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-reliontomo/
```

### Comparing `scipion-em-reliontomo-3.1.6/scipion_em_reliontomo.egg-info/SOURCES.txt` & `scipion-em-reliontomo-3.2.0/scipion_em_reliontomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-reliontomo-3.1.6/setup.py` & `scipion-em-reliontomo-3.2.0/setup.py`

 * *Files identical despite different names*


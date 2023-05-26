# Comparing `tmp/scipion-em-cryosparc2-4.0.5.tar.gz` & `tmp/scipion-em-cryosparc2-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.0.5.tar", last modified: Fri May 26 15:55:45 2023, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.0.6.tar", last modified: Fri May 26 16:04:54 2023, max compression
```

## Comparing `scipion-em-cryosparc2-4.0.5.tar` & `scipion-em-cryosparc2-4.0.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.395722 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryorefine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 15:55:45.000000 scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:55:45.399722 scipion-em-cryosparc2-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-26 15:53:59.000000 scipion-em-cryosparc2-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.758321 scipion-em-cryosparc2-4.0.6/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32630 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryorefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24057 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14362 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32686 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23794 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46792 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34295 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.762321 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 16:04:54.000000 scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:04:54.766321 scipion-em-cryosparc2-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-26 16:03:02.000000 scipion-em-cryosparc2-4.0.6/setup.py
```

### Comparing `scipion-em-cryosparc2-4.0.5/LICENSE` & `scipion-em-cryosparc2-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/PKG-INFO` & `scipion-em-cryosparc2-4.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.5
+Version: 4.0.6
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,30 +34,19 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.3**
+        **v4.0.6**
         -----------
         * **new**     :  Compatibility with cryoSPARC v4.2.1
-        
-        **v4.0.3**
-        -----------
-        * **new**     :  Compatibility with cryoSPARC v4.2
-        * **fixed**   :  Fixed an error importing volumes with halves
-        * **fixed**   :  Fixed an error launching the protocols viewers
-        
-        
-        **v4.0.2**
-        -----------
-        * **new**     :  Compatibility with cryoSPARC v4.1.0, 4.1.1 and 4.1.2
-        * **updated** :  Creating an environment for pyem package
-        * **updated** :  3D homogeneous refinement(Legacy), 3D non-uniform refinement(Legacy) and Naive local refinement(Legacy) protocols are deprecated
+        * **new**        Plugin operation in a cluster
+        * **fixed**      Fixed an installation error
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.5/README.rst` & `scipion-em-cryosparc2-4.0.6/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -24,30 +24,19 @@
 * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
 * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
 * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
 
 **Latest plugin version**
 ==========================
 
-**v4.0.3**
+**v4.0.6**
 -----------
 * **new**     :  Compatibility with cryoSPARC v4.2.1
-
-**v4.0.3**
------------
-* **new**     :  Compatibility with cryoSPARC v4.2
-* **fixed**   :  Fixed an error importing volumes with halves
-* **fixed**   :  Fixed an error launching the protocols viewers
-
-
-**v4.0.2**
------------
-* **new**     :  Compatibility with cryoSPARC v4.1.0, 4.1.1 and 4.1.2
-* **updated** :  Creating an environment for pyem package
-* **updated** :  3D homogeneous refinement(Legacy), 3D non-uniform refinement(Legacy) and Naive local refinement(Legacy) protocols are deprecated
+* **new**        Plugin operation in a cluster
+* **fixed**      Fixed an installation error
 
 **Installing the plugin**
 =========================
 
 In order to install the plugin follow these instructions:
 
 1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.0.5'
+__version__ = '4.0.6'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
```

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/cs2Start.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.0.6/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_base.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryorefine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryorefine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_naive_local_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.0.6/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/viewers/viewer_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.0.6/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.5
+Version: 4.0.6
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -34,30 +34,19 @@
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.3**
+        **v4.0.6**
         -----------
         * **new**     :  Compatibility with cryoSPARC v4.2.1
-        
-        **v4.0.3**
-        -----------
-        * **new**     :  Compatibility with cryoSPARC v4.2
-        * **fixed**   :  Fixed an error importing volumes with halves
-        * **fixed**   :  Fixed an error launching the protocols viewers
-        
-        
-        **v4.0.2**
-        -----------
-        * **new**     :  Compatibility with cryoSPARC v4.1.0, 4.1.1 and 4.1.2
-        * **updated** :  Creating an environment for pyem package
-        * **updated** :  3D homogeneous refinement(Legacy), 3D non-uniform refinement(Legacy) and Naive local refinement(Legacy) protocols are deprecated
+        * **new**        Plugin operation in a cluster
+        * **fixed**      Fixed an installation error
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.5/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.0.6/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.5/setup.py` & `scipion-em-cryosparc2-4.0.6/setup.py`

 * *Files identical despite different names*

